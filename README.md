# Handwritten Digit Classification with PyTorch

A beginner-to-intermediate deep learning journey using the MNIST dataset and PyTorch.

This repository contains three projects showing the evolution from:
1. Simple Artificial Neural Network (ANN)
2. Convolutional Neural Network (CNN)
3. Improved CNN with regularization techniques

---

# Projects Overview

| Project | Description | Accuracy |
|---|---|---|
| ANN Classifier | Basic fully connected neural network | ~96% |
| CNN Classifier | Convolutional neural network for image feature extraction | ~98% |
| Improved CNN | CNN with BatchNorm, Dropout, and Data Augmentation | ~98%+ |

---

# Dataset

Dataset Used:
- MNIST Handwritten Digits Dataset

Dataset Details:
- 70,000 handwritten digit images
- 28×28 grayscale images
- Digits from 0–9
- 60,000 training images
- 10,000 testing images

---

# Tech Stack

- Python
- PyTorch
- torchvision
- matplotlib
- Google Colab

---

# Project 1 — Simple ANN Classifier

## Goal

Learn:
- tensors
- neural networks
- forward pass
- loss functions
- optimizers
- training loop

---

## Architecture

Input (784)
↓
Linear Layer (128)
↓
ReLU
↓
Linear Layer (64)
↓
ReLU
↓
Output Layer (10)

---

## Key Concepts Learned

- Tensor operations
- Flattening images
- Fully connected layers
- Forward propagation
- Backpropagation
- Gradient descent
- CrossEntropyLoss
- Adam optimizer

---

## Result

Test Accuracy: ~96%

---

# Project 2 — CNN Digit Classifier

## Goal

Learn:
- convolution
- feature maps
- pooling
- spatial feature extraction

---

## Why CNN?

ANNs flatten images immediately:

28×28 → 784

This loses spatial relationships.

CNNs preserve image structure and learn visual patterns like:
- edges
- curves
- shapes

---

## CNN Architecture

Input Image
↓
Conv2D
↓
ReLU
↓
MaxPooling
↓
Conv2D
↓
ReLU
↓
MaxPooling
↓
Flatten
↓
Fully Connected Layer
↓
Output

---

## Key Concepts Learned

- Convolution layers
- Kernels / filters
- Feature maps
- ReLU activation
- MaxPooling
- Channels
- Spatial learning

---

## Result

Test Accuracy: ~98%

---

# Project 3 — Improved CNN (Regularization)

## Goal

Reduce overfitting and improve generalization.

---

## Improvements Added

### 1. Batch Normalization

Stabilizes activations during training.

Benefits:
- faster training
- smoother gradients
- better convergence

---

### 2. Dropout

Randomly disables neurons during training.

Benefits:
- reduces memorization
- improves robustness
- prevents overfitting

---

### 3. Data Augmentation

Random image transformations:
- rotations
- shifts
- variations

Benefits:
- improves generalization
- teaches robustness to variations

---

## Improved Architecture

Conv2D
↓
BatchNorm
↓
ReLU
↓
MaxPool
↓
Conv2D
↓
BatchNorm
↓
ReLU
↓
MaxPool
↓
Flatten
↓
Linear
↓
Dropout
↓
Output

---

## Key Concepts Learned

- Overfitting
- Generalization
- BatchNorm
- Dropout
- Data augmentation
- Training vs evaluation mode

---

## Result

Test Accuracy: ~98%+

---

# Training Workflow

All projects follow this deep learning pipeline:

Dataset
↓
DataLoader
↓
Forward Pass
↓
Loss Calculation
↓
Backpropagation
↓
Optimizer Step
↓
Repeat

---

# Installation

## Clone Repository

```bash
git clone <your-repository-url>
