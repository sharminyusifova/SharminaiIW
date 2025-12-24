# SVHN_AI_20240111

This repository contains an individual deep learning project focused on classifying digits from house numbers using a Convolutional Neural Network (CNN) with data augmentation.

## Project Overview
The goal of this project is to train a CNN model on the **SVHN (Street View House Numbers) dataset**. The model learns to classify images of digits (0–9) with reproducible results using a fixed seed (20240111).

## Dataset
- **Name:** SVHN  
- **Classes:** 10 (digits 0–9)  
- **Images:** 32x32 RGB  
- **Splits:** Training and Test sets  

## Model Architecture
- **Input:** 32x32x3 RGB images  
- **Layers:**
  - Conv2D + ReLU + MaxPooling
  - Conv2D + ReLU + MaxPooling
  - Flatten
  - Dense (128 neurons, ReLU)
  - Dense (Softmax output for classification)
- **Optimizer:** Adam  
- **Loss:** Sparse Categorical Crossentropy  
- **Epochs:** 10  

## Data Augmentation
Applied to improve generalization:
- Horizontal flipping
- Random rotations
- Random zooms

## Results
- Training and validation accuracy plotted for analysis
- Test accuracy ~90% (depending on run)
- Model saved as `SVHN_AI_20240111.h5`

## How to Run
1. Install dependencies:
```bash
pip install -r requirements.txt
# SharminaiIW
