# Image Super Resolution Project

This repository contains a deep learning project focused on image super-resolution (SR) techniques. The project implements and compares multiple neural network architectures for enhancing the resolution of images. Read the medium article [here](https://medium.com/@jainpranav635/image-super-resolution-enhancing-visual-quality-with-deep-learning-3fa9ae91051c).

## Overview

Image Super Resolution aims to enhance the resolution and quality of low-resolution images by reconstructing high-resolution details that were lost during downsampling or due to limitations in image acquisition. This project explores several deep learning approaches to this problem.

## Models Implemented

The project implements three different super-resolution architectures:

1. **SRCNN (Super-Resolution CNN)**: A pioneering approach that uses a three-layer CNN to learn the mapping between low and high-resolution images.

2. **ESPCN (Efficient Sub-Pixel CNN)**: Introduces the efficient sub-pixel convolution layer for upsampling, which reduces computational complexity.

3. **EDSR (Enhanced Deep Super-Resolution)**: A more advanced model that uses residual blocks and removes unnecessary modules from conventional residual networks.

## Dataset

The project uses the DIV2K (DIVerse 2K resolution high-quality images) dataset, which contains:
- 800 images for training
- 100 images for validation
- 100 images for testing

## Requirements

- Python 3.8+
- PyTorch 1.8+
- torchvision
- Pillow
- numpy
- matplotlib
- tqdm

You can install the required packages using:

```bash
pip install torch torchvision pillow numpy matplotlib tqdm
```

## Usage

The main notebook `ISR.ipynb` contains all the code for:
- Data preprocessing and loading
- Model implementation
- Training and validation
- Results visualization
- Testing on custom images

## Sample Results

The notebook includes sample results showing:
- Low-resolution input images
- Super-resolution outputs from different models
- Original high-resolution ground truth images

## Custom Image Testing

You can test the trained models on your own images using the `test_on_custom_image` function provided in the notebook.

## Future Work

Potential directions for future work include:
- Exploring GAN-based approaches for more perceptually pleasing results
- Implementing attention mechanisms to focus on important image regions
- Developing lightweight models for mobile applications
- Investigating domain-specific super-resolution for medical or satellite imagery

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- The DIV2K dataset creators for providing high-quality images for super-resolution research
- The authors of the original SRCNN, ESPCN, and EDSR papers for their contributions to the field

## Author

Pranav Jain
