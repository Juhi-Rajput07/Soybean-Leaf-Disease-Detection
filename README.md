# Robust Soybean Leaf Disease Detection using Transfer Learning

## Overview
This project implements a deep learning model for detecting 9 soybean leaf diseases using MobileNetV2 transfer learning.

## Dataset
- 11,854 images
- 9 classes:
  bacterial blight, diabrotica specosa, caterpillar,
  downy mildew, healthy, mosaic virus,
  powdery mildew, rust, southern blight
- 80/20 train-validation split

## Model Architecture
- MobileNetV2 (ImageNet pretrained)
- Base layers frozen
- GlobalAveragePooling
- Dense (128)
- Dropout (0.3)
- Softmax output layer

## Training Configuration
- Image size: 160x160
- Optimizer: Adam
- Loss: Categorical Crossentropy
- Epochs: 6
- Early stopping enabled

## Results
Validation Accuracy: 91.63%

Confusion matrix shows strong diagonal performance.

## Research Gap Addressed
Improving generalization of soybean disease detection models trained on controlled datasets.
