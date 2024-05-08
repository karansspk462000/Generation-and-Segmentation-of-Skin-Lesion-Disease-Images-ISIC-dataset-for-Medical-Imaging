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


2. Install necessary dependencies.


3. Download the ISIC 2016 dataset and place it in the `data/` directory.

## Usage:

1. **Segmentation:**

- Run the segmentation module with your chosen dataset.

- This will generate contours for the skin diseases present in the dataset.

2. **Image Generation:**

- Provide the generated contours and labels to the CGAN or ACGAN model for image generation.

3. **Testing:**

- Test the generated images using a pre-trained model.
- 
## Results:
<figure>
<figcaption><em>Deblurred using CNN</em></figcaption>
  <img src="[https://github.com/sohampadhye007/Enhancing-Low-Light-Blurred-Images-using-Image-Processing-Techniques/blob/main/Deblur_CNN.png](https://github.com/karansspk462000/Generation-and-Segmentation-of-Skin-Lesion-Disease-Images-ISIC-dataset-for-Medical-Imaging/blob/main/output_yfys.png)https://github.com/karansspk462000/Generation-and-Segmentation-of-Skin-Lesion-Disease-Images-ISIC-dataset-for-Medical-Imaging/blob/main/output_yfys.png?raw=true" alt="Deblured Image" title="deblured Image">

</figure>
## Acknowledgments:

- ISIC 2016 dataset: [International Skin Imaging Collaboration](https://www.isic-archive.com/#!/topWithHeader/wideContentTop/main)
- PyTorch: [PyTorch](https://pytorch.org/)
- OpenCV: [OpenCV](https://opencv.org/)

Feel free to contribute to this project by forking and submitting pull requests. If you encounter any issues or have suggestions for improvement, please open an issue on the repository.
