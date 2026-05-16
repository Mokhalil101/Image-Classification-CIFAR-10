# 🧠 Handwritten Digit Classification using MLP (PyTorch)

## 📌 Project Overview
This project implements a **Multilayer Perceptron (MLP)** model to classify handwritten digits using the **MNIST dataset**.  
The main goal is to **compare the performance of different optimizers (Adam vs SGD)** in terms of loss convergence and accuracy.

---

## 📂 Dataset
- **Name:** MNIST Handwritten Digits
- **Classes:** 10 (Digits 0 → 9)
- **Image Size:** 28 × 28 grayscale
- **Source:** torchvision.datasets

---

## 🔧 Data Preprocessing
The following preprocessing steps were applied:

- Conversion to Tensor
- Normalization using mean = 0.5 and std = 0.5
- Flattening images from 28×28 to 784 features
- Splitting dataset into:
  - **Training set**
  - **Validation set**

---

## 🏗️ Model Architecture
The implemented MLP architecture consists of:

- Input Layer: 784 neurons
- Hidden Layer 1: Fully Connected + ReLU
- Hidden Layer 2: Fully Connected + ReLU
- Output Layer: 10 neurons (Softmax via CrossEntropyLoss)

---

## ⚙️ Optimizers Used
Two different optimizers were used and compared:

- **Adam Optimizer**
- **Stochastic Gradient Descent (SGD)**

Both optimizers were trained using the same:
- Number of epochs
- Learning rate
- Batch size
- Loss function (CrossEntropyLoss)

---

## 📊 Evaluation Metrics
The model performance was evaluated using:

- Training Loss
- Validation Loss
- Training Accuracy
- Validation Accuracy

---

## 📈 Results & Comparison
The following comparisons were visualized:

- Adam vs SGD Training Loss
- Adam vs SGD Validation Loss
- Adam vs SGD Training Accuracy
- Adam vs SGD Validation Accuracy

### 🔍 Observations
- Adam converges faster during early epochs.
- SGD shows more stable behavior but requires more epochs.
- Adam generally achieves higher validation accuracy.
- Optimizer choice significantly impacts convergence speed and final performance.

---

## 🧪 Experiments
- Experiment 1: Training MLP using **Adam Optimizer**
- Experiment 2: Training MLP using **SGD Optimizer**
- Final comparison between both optimizers using plots.

---

## 🛠️ Technologies Used
- Python
- PyTorch
- Torchvision
- Matplotlib
- Google Colab / Jupyter Notebook

---

## 🚀 How to Run

```bash
pip install -r requirements.txt

---

## 📌 Conclusion
This project demonstrates how optimizer choice affects neural network training.  
Adam provides faster convergence, while SGD offers stable learning behavior.

