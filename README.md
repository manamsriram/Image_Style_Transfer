# Style Synthesis: Deep Learning Image Style Transfer

This project implements and compares multiple deep learning models for image style transfer, focusing on VGG19, VGG16, Magenta, and ResNet architectures.

## Project Overview

Style Synthesis aims to bridge art and technology through advanced style transfer techniques. The project utilizes pre-trained Convolutional Neural Networks (CNNs) to extract features and transfer artistic styles between images while preserving content and achieving photorealistic results.

## Features

- Implementation of multiple style transfer models (VGG19, VGG16, Magenta, ResNet)
- Custom loss functions including content loss, style loss, and total variation loss
- Optimization using L-BFGS algorithm
- Quantitative evaluation using SSIM and PSNR metrics
- Qualitative assessment through human perception studies

## Requirements

- Python 3.x
- Keras
- TensorFlow
- NumPy
- SciPy
- Pillow

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/your-username/style-synthesis.git
   cd style-synthesis
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

Run the style transfer script with the following command:

```
python style_transfer.py content_image style_reference_image [options]
```

Options:
- `--iter`: Number of iterations (default: 10)
- `--content_weight`: Content weight (default: 0.025)
- `--style_weight`: Style weight (default: 1.0)
- `--tv_weight`: Total Variation weight (default: 1.0)


## Results

The script generates styled images at each iteration. The final output combines the content of the input image with the style of the reference image.

## Evaluation

The project includes both quantitative and qualitative evaluation methods:
- Structural Similarity Index Measure (SSIM)
- Peak Signal-to-Noise Ratio (PSNR)
- Human perception studies for aesthetic assessment


## References

<a href="https://arxiv.org/abs/1703.07511">This paper</a> was our reference to help come up with our own.
