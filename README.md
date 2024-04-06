## Single Image Super Resolution (SISR) using Generative Adversarial Network (GAN)

### Overview
This repository contains the implementation of Single Image Super Resolution (SISR) using Generative Adversarial Network (GAN). The project was conducted from November 2023 to January 2024.

### Project Details
- **Objective**: The goal of this project was to enhance the resolution of single images using deep learning techniques, particularly Generative Adversarial Networks (GANs).
- **Models Implemented**: 
  - SRGAN (Super-Resolution GAN)
- **Evaluation Metrics**: The models were compared using PSNR (Peak Signal-to-Noise Ratio) and SSIM (Structural Similarity Index) as evaluation metrics.
- **Key Contributions**:
  - Experimented with various model architecture variations in SRGAN, including:
    - Residual in residual network (double residual connection)
    - Changing depth of the network
    - Implementing new loss functions
  - Using Perceptual Loss function over MSE loss function improved image enhancement (SSIM) from 0.75 (in SRGAN) & 0.78 (in SRResNet) to 0.79 in the newly developed network. Furthermore, the number of parameters was reduced by decreasing the depth of the network by almost 50%.

### Files
- `SRGAN.py`: This file contains the implementation of the SRGAN (Super-Resolution GAN) model for Single Image Super Resolution.

### Usage
To utilize the SRGAN model for Single Image Super Resolution, follow these steps:
1. Clone the repository.
2. Ensure the necessary dependencies are installed.
3. Run `SRGAN.py` with the desired image(s) as input.

### Dependencies
- Python 3.x
- PyTorch
- Other dependencies as required (details within the code)

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
