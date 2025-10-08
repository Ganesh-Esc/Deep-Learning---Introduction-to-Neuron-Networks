# Neuron Computations: From Logic Gates to Matrix Operations



An exercise demonstrating how to model basic logic functions (AND, OR, XOR) with neurons and how to represent neural networks using matrix computations.

---

## 🧠 About This Exercise

This project serves as a fundamental introduction to neuron mechanics. The goal is to build an intuition for how neural networks perform computations by starting with the smallest component: a single neuron, also known as a perceptron.

We will explore:
* How simple, **linearly separable** functions like `AND` and `OR` can be modeled by a single neuron by adjusting its weights and bias.
* Why a single neuron **fails** to represent a non-linearly separable function like `XOR`.
* How a **multi-layer structure** (a simple neural network) can successfully model the `XOR` function.
* How the entire process can be generalized into a chain of **matrix computations**, which is the foundation of modern deep learning.

---

## 🔬 Key Concepts Covered

This exercise walks through the core components of neural computation:

* **The Neuron Model**: Understanding the basic computation as a weighted sum of inputs followed by an activation function: `$y = f(\sum_{i} w_i x_i + b)$`.
* **Weights and Biases**: Manually tuning weight ($w$) and bias ($b$) values to achieve a desired logical output.
* **Activation Function**: Using a simple step function to determine the neuron's output (0 or 1).
* **Linear Separability**: Visualizing why a single line can separate the outcomes of AND/OR but not XOR. 
* **Multi-Layer Perceptron (MLP)**: Combining the outputs of multiple neurons to solve a more complex problem.
* **Vectorization**: Representing the inputs, weights, and computations for a layer of neurons using vectors and matrices.

---

## 🛠️ Exercise Structure

The code is structured to guide you through the following parts:

### **Part 1: The AND Gate**
We'll define weights and a bias for a single neuron that correctly computes the AND function.

| X1 | X2 | Output |
|:--:|:--:|:------:|
| 0  | 0  |   0    |
| 0  | 1  |   0    |
| 1  | 0  |   0    |
| 1  | 1  |   1    |

### **Part 2: The OR Gate**
By slightly modifying the parameters from the AND gate, we'll show how the same neuron can represent the OR function.

### **Part 3: The XOR Challenge**
Here, we demonstrate why a single neuron fails to solve the XOR problem. We then build a two-layer network (e.g., by combining `NAND` and `OR` gates) to correctly model `XOR`.

### **Part 4: Neural Networks as Matrix Computations**
Finally, we abstract the concepts from the previous parts to show how a forward pass can be expressed concisely as a matrix equation:
$$ Z = W \cdot X + b $$
$$ A = g(Z) $$
Where $W$ is the weight matrix, $b$ is the bias vector, and $g$ is the activation function.

---
