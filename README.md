
# Neural Network Playground

This repository provides two Python implementations for learning and experimenting with neural networks:

- **Single-Layer Perceptron**: A basic perceptron model for binary classification tasks.
- **Feed-Forward Neural Network**: A single hidden-layer neural network for MNIST digit recognition.

---

## 1. Perceptron Model

Implements a single-layer perceptron with a sigmoid activation function. Trains on sample binary logic gate data and allows interactive predictions.

**Key Features:**

- Sigmoid activation and its derivative
- Backpropagation for weight updates
- Handles 3-input binary patterns
- Interactive user input for predictions

**Workflow:**

1. Randomly initializes weights
2. Trains on sample logic gate data
3. Prompts user for 3-bit binary input and predicts output

---

## 2. Feed-Forward Neural Network for MNIST

Implements a single hidden-layer neural network to classify handwritten digits from the MNIST dataset.

**Architecture:**

- Input layer: 784 nodes (28x28 pixels)
- Hidden layer: 200 nodes
- Output layer: 10 nodes (digits 0-9)

**Training Details:**

- Data normalization: pixel values scaled to [0.01, 0.99]
- One-hot encoding for target labels
- Configurable for small (100 samples) or full MNIST training set
- 5 training epochs, learning rate 0.1

**Results:**

- Achieves ~60% accuracy on test set (with reduced training data)
- Achieves 100% accuracy on full training set

**Visualization:**

- Displays a randomly selected test digit and its label

---

## Getting Started

1. **Install Requirements**
	- Python 3.x
	- NumPy
	- Matplotlib
	- Install dependencies:

	  ```sh
	  pip install -r requirements.txt
	  ```

2. **Prepare Data**
	- Unzip `mnist_train_full.zip` to access the full training CSV file.
	- Place all MNIST CSV files in the project directory.

3. **Run the Notebook**
	- Open `perceptron_mnist.ipynb` in VS Code or Jupyter.
	- Execute cells in order for both perceptron and neural network demos.

---

## File Structure

- `perceptron_mnist.ipynb` — Main notebook with both models
- `mnist_train_100.csv` — Small training set
- `mnist_train_full.csv` — Full training set
- `mnist_test_10.csv` — Small test set
- `mnist_test_full.csv` — Full test set
- `requirements.txt` — Python dependencies
- `mnist_train_full.zip` — Compressed full training set

---

## License

This project is open source and available under the MIT License.
