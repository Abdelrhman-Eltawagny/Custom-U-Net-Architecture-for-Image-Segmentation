# Custom U-Net Architecture for Image Segmentation

## Overview
This project presents a complete implementation of a U-Net architecture for semantic image segmentation using PyTorch. The model is trained on the Oxford-IIIT Pet Dataset to perform pixel-wise segmentation and identify foreground objects from images.

The implementation follows a modular design by building each U-Net component separately, improving code readability, maintainability, and extensibility.

## Project Architecture

The U-Net model consists of:
- Double Convolution Block
- Encoder Block
- Bottleneck Block
- Decoder Block
- Final Output Layer

## Dataset

### Oxford-IIIT Pet Dataset

The dataset contains pet images along with segmentation masks used for supervised semantic segmentation tasks.

Dataset Features:

- RGB Pet Images
- Pixel-level Segmentation Masks
- Multiple Pet Categories
- Binary Segmentation Setup

## Technologies Used
- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib

## Model Components
### DoubleConv Block
Applies:
- Convolution
- Batch Normalization
- ReLU Activation
- Dropout

### Encoder Block
Performs:
- Feature Extraction
- Spatial Downsampling via MaxPooling

### Bottleneck
- Captures high-level semantic features.

### Decoder Block
Performs:
- Transposed Convolution Upsampling
- Skip Connections
- Feature Reconstruction

### Final Output Layer
- Generates pixel-wise segmentation probabilities.

## Results
The model successfully learns to generate segmentation masks for pet images.

Outputs include:
- Training Loss Curve
- Validation Loss Curve
- Ground Truth Masks
- Predicted Segmentation Masks

## Author
**Abdelrhman Samir**
AI Enginner
