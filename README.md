# Skin Disease Segmentation and Image Generation

## Overview:

This project aims to utilize the ISIC 2016 dataset for segmenting skin disease contours and generating images using Generative Adversarial Networks (GANs). The process involves segmentation of skin disease contours from the dataset, providing sketches and labels to Conditional GAN (CGAN) and Auxiliary Classifier GAN (ACGAN) to generate corresponding images, and finally testing the generated images using a pre-trained model.

## Prerequisites:

- Python 3.x
- PyTorch
- OpenCV
- ISIC 2016 dataset
- CUDA (optional, for GPU acceleration)

## Installation:

1. Clone the repository:

git clone https://github.com/yourusername/skin-disease-segmentation-gan.git


2. Install dependencies:

pip install -r requirements.txt


3. Download the ISIC 2016 dataset and place it in the `data/` directory.

## Usage:

1. **Segmentation:**

- Run the segmentation module with your chosen dataset:

  ```
  python segmentation.py --dataset_path /path/to/dataset
  ```

- This will generate contours for the skin diseases present in the dataset.

2. **Image Generation:**

- Provide the generated contours and labels to the CGAN or ACGAN model for image generation.

  ```
  python generate_images.py --contours /path/to/contours --labels /path/to/labels --model cgan
  ```

  Replace `--model` with `acgan` if using ACGAN.

3. **Testing:**

- Test the generated images using a pre-trained model.

  ```
  python test.py --test_images /path/to/test_images --model /path/to/pretrained_model.pth
  ```

## Directory Structure:

- **data/**: Contains the ISIC 2016 dataset.
- **segmentation.py**: Script for generating contours from the dataset.
- **generate_images.py**: Script for generating images from contours and labels using CGAN or ACGAN.
- **test.py**: Script for testing the generated images using a pre-trained model.
- **models/**: Directory to store trained models.
- **results/**: Directory to store generated images and test results.

## License:

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments:

- ISIC 2016 dataset: [International Skin Imaging Collaboration](https://www.isic-archive.com/#!/topWithHeader/wideContentTop/main)
- PyTorch: [PyTorch](https://pytorch.org/)
- OpenCV: [OpenCV](https://opencv.org/)

Feel free to contribute to this project by forking and submitting pull requests. If you encounter any issues or have suggestions for improvement, please open an issue on the repository. Happy coding!
