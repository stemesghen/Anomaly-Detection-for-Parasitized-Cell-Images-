Link to Dataset:  https://data.lhncbc.nlm.nih.gov/public/Malaria/cell_images.zip


# Convolutional Neural Network for Image Classification

This project implements a basic Convolutional Neural Network (CNN) using Keras and TensorFlow to classify images into one of 10 categories, such as planes, cars, birds, and animals. The model is trained and evaluated on the CIFAR-10 dataset, a widely-used benchmark for image classification tasks.

## Objective

To develop and train a convolutional neural network capable of classifying low-resolution (32x32) color images into predefined object categories using supervised learning techniques.

## Dataset

- **CIFAR-10**: Contains 60,000 32x32 color images in 10 classes, with 6,000 images per class.
  - 50,000 images for training
  - 10,000 images for testing

## CNN Architecture

The CNN is composed of the following layers:

- **Convolutional Layer 1**: 32 filters, 3x3 kernel, ReLU activation
- **MaxPooling Layer 1**: 2x2 pooling
- **Convolutional Layer 2**: 64 filters, 3x3 kernel, ReLU activation
- **MaxPooling Layer 2**: 2x2 pooling
- **Flatten Layer**: Converts 2D feature maps into a 1D feature vector
- **Dense Layer**: 64 units, ReLU activation
- **Output Layer**: 10 units, Softmax activation for multi-class classification

## Training

- **Loss Function**: Categorical Crossentropy
- **Optimizer**: Adam
- **Metrics**: Accuracy
- **Epochs**: 10 (can be increased for better accuracy)
- **Batch Size**: 64

## Results

- Achieved validation accuracy between 68–72% after 10 epochs.
- Performance is consistent with standard CNNs trained on CIFAR-10 without data augmentation.
- Model performance can be improved with additional convolutional layers, dropout, batch normalization, and data augmentation.

## How to Run

1. Clone this repository.
2. Install dependencies:
   pip install tensorflow numpy matplotlib

