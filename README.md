# Intelligent Model Design using AI Lab

This repository contains lab assignments for the course **Intelligent Model Design using AI**.

## Assignment 01 – CIFAR-10 Image Classification using ANN/MLP

### Objective

To implement a three-hidden-layer Artificial Neural Network (ANN/MLP) for CIFAR-10 image classification and perform hyperparameter tuning using Grid Search and Random Search.

### Dataset

CIFAR-10 dataset was used.

- Training images: 50,000
- Testing images: 10,000
- Classes: 10
- Image size: 32 × 32 × 3
- Color channels: RGB

### Preprocessing

- Pixel values were normalized from `[0, 255]` to `[0, 1]`.
- Class labels were converted to one-hot encoded vectors.

### ANN Architecture

```text
Input: 32 × 32 × 3
        ↓
Flatten
        ↓
Dense: 512 neurons, ReLU
        ↓
Dense: 256 neurons, ReLU
        ↓
Dense: 128 neurons, ReLU
        ↓
Dense: 10 neurons, Softmax
