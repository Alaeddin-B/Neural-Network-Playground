# Perceptron and Neural Network Implementation

This repository contains two Python implementations:
1. A single-layer Perceptron model
2. A feed-forward Neural Network for MNIST digit recognition

## Perceptron Model

A simple perceptron with sigmoid activation trained on binary logic gate data.

### Features:
- Sigmoid activation function
- Backpropagation training
- Handles 3-input binary patterns
- Interactive prediction from user input

### Usage:
1. Initializes with random weights
2. Trains on sample logic gate data (AND/NAND-like behavior)
3. Predicts output for user-provided 3-bit binary inputs

## Neural Network for MNIST

A single hidden-layer network trained on reduced MNIST dataset.

### Features:
- 784 input nodes (28×28 images)
- 200 hidden nodes
- 10 output nodes (digits 0-9)
- Sigmoid activation
- Backpropagation learning

### Data Processing:
- Normalizes pixel values (0.01-0.99)
- One-hot encoding for labels
- Works with 100-sample training set
- Works with a much larger training set

### Training:
- 5 epochs
- 0.1 learning rate
- Achieves ~60% accuracy on test set and 100% accuracy on full training set

### Visualization:
- Includes sample digit display from test set

## Requirements
- Python 3
- NumPy
- Matplotlib (for visualization)

To run, execute the notebook cells in order. The perceptron runs automatically while the neural network requires MNIST data files. You will have to unzip the only zip file in there to be able to access the full training csv file.
