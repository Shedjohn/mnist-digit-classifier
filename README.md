# MNIST Handwritten Digit Classifier

A deep learning project built using PyTorch and Google Colab to classify handwritten digits from the MNIST dataset. The model was trained on 60,000 images and tested on 10,000 images of handwritten digits (0–9).

## Features
- Built with PyTorch
- Neural network for digit classification
- Training and testing pipeline
- Model evaluation with accuracy score
- Visualization of predictions

## Technologies Used
- Python
- PyTorch
- Torchvision
- Matplotlib
- Google Colab

## Dataset
The project uses the MNIST dataset, a popular benchmark dataset containing grayscale handwritten digit images of size 28×28 pixels.

## Model Architecture
- Flatten Layer
- Fully Connected Layer (784 → 128)
- ReLU Activation
- Fully Connected Layer (128 → 64)
- ReLU Activation
- Output Layer (64 → 10)

## Training
The model was trained using:
- CrossEntropyLoss
- Adam Optimizer
- Batch Size: 64
- Epochs: 5

## Results
Achieved a test accuracy of **96.47%** on the MNIST test dataset.

## Concepts Learned
- Tensors
- Neural Networks
- Forward Pass
- Loss Functions
- Backpropagation
- Optimizers
- Training Loops
- Model Evaluation

## Future Improvements
- Implement Convolutional Neural Networks (CNNs)
- Add Dropout and Batch Normalization
- Experiment with different optimizers and hyperparameters
- Deploy the model as a web application

## Author
Developed as a beginner deep learning project to understand the fundamentals of AI and neural networks.
