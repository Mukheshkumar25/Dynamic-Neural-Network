# 🧠 Neural Network Training Framework

A fully customizable, from-scratch implementation of a feedforward artificial neural network in Python — no external libraries used! 🔧✨  
Designed for training on numerical datasets (e.g., diabetes dataset) and predicting outputs using sigmoid activation and backpropagation.

---

## 🚀 Features

- 🏗️ **Flexible Architecture**: Choose predefined, randomized, or default hidden layer configurations
- 🎛️ **Adjustable Hyperparameters**: Set learning rate, epochs, and layer sizes dynamically
- 📊 **Feedforward & Backpropagation**: Full implementation with sigmoid activation and gradient descent
- 💾 **Best Model Retention**: Stores optimal weights and biases with least SSE
- 🧪 **Custom Input Testing**: Predict outcomes for new unseen data after training
- 📉 **Minimal Dependencies**: Written entirely in standard Python

---

## 🧮 Algorithm Used

🧬 The network follows a classical **Feedforward Neural Network** approach trained with **Backpropagation** using the **Gradient Descent** algorithm.

### 🔁 Feedforward

- Weighted inputs are passed through each neuron
- Output calculated using **Sigmoid activation function**  
  \[
  \sigma(x) = \frac{1}{1 + e^{-x}}
  \]

### 🔄 Backpropagation

- Calculates error at output layer (target - predicted)
- Computes **delta** using sigmoid derivative:
  \[
  \delta = (target - output) \times output \times (1 - output)
  \]
- Updates weights and biases using:
  \[
  w = w + \text{learning_rate} \times \delta \times \text{output}\_{\text{previous layer}}
  \]

---

## 🔁 Sample Workflow

```bash
$ python neural_net.py

Choose one of the following options for hidden layers:
1. Predefined hidden layer count
2. Random hidden layer configuration
3. Default (5 hidden layers, 3 nodes)

Enter your choice: 1
Enter the number of layers: 4
Enter number of nodes for layer 2: 6
Enter number of nodes for layer 3: 4
...
```
