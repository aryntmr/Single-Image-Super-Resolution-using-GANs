## Single Image Super Resolution (SISR) using Generative Adversarial Network (GAN)

### Overview
This repository contains the implementation of Single Image Super Resolution (SISR) using Generative Adversarial Network (GAN).

### Project Details
- **Objective**: The goal of this project was to enhance the resolution of single images using deep learning techniques, particularly Generative Adversarial Networks (GANs).
- **Models Implemented**: 
  - SRGAN (Super-Resolution GAN)
  - ESRGAN (Enhanced Super-Resolution GAN)
  - SRResNet (Super-Resolution ResNet)
- **Evaluation Metrics**: The models were compared using PSNR (Peak Signal-to-Noise Ratio) and SSIM (Structural Similarity Index) as evaluation metrics.
- **Key Contributions**:
  - Experimented with various model architecture variations in SRGAN, including:
    - Residual in residual network (double residual connection)
    - Changing depth of the network
    - Implementing new loss functions
  - Using Perceptual Loss function over MSE loss function improved image enhancement (SSIM) from 0.75 (in SRGAN) & 0.78 (in SRResNet) to 0.79 in the newly developed network. Furthermore, the number of parameters was reduced by decreasing the depth of the network by almost 50%.

### Dataset
The DIV2K dataset was used for training and evaluation. DIV2K is a high-quality dataset for single-image super-resolution (SISR). To use the DIV2K dataset, follow these steps:
1. Download the DIV2K dataset from the official website: [DIV2K Dataset](https://data.vision.ee.ethz.ch/cvl/DIV2K/)
2. Extract the dataset files to a directory of your choice.
3. Preprocess the dataset as necessary for training your models. This may include resizing images, splitting into training/validation sets, etc.

### Files
- `SRGAN.py`: This file contains the implementation of the SRGAN (Super-Resolution GAN) model for Single Image Super Resolution.

### Usage
To utilize the SRGAN model for Single Image Super Resolution, follow these steps:
1. Clone the repository.
2. Ensure the necessary dependencies are installed.
3. Download and preprocess the DIV2K dataset (if not already done).
4. Update the file paths in `SRGAN.py` to point to the location of your dataset.
5. Run `SRGAN.py` with the desired image(s) as input.

### References
- [Ledig, Christian, et al. "Photo-realistic single image super-resolution using a generative adversarial network." Proceedings of the IEEE conference on computer vision and pattern recognition. 2017.](https://arxiv.org/abs/1609.04802)
- [Wang, Xintao, et al. "ESRGAN: Enhanced super-resolution generative adversarial networks." Proceedings of the European Conference on Computer Vision (ECCV). 2018.](https://arxiv.org/abs/1809.00219)

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
