# 🧠 CIFAR-10 Image Classification using CNN

## 📌 Project Description
This project implements a Convolutional Neural Network (CNN) for image classification using the CIFAR-10 dataset.  
The model is trained and evaluated using different optimizers (Adam and SGD) to compare performance.

---

## 📊 Dataset
- Dataset: CIFAR-10
- Classes: 10 classes (airplane, car, bird, cat, deer, dog, frog, horse, ship, truck)
- Source: https://www.cs.toronto.edu/~kriz/cifar.html

---

## 🧠 Model Architecture
The CNN consists of:
- 3 Convolutional layers
- Batch Normalization
- ReLU activation
- MaxPooling
- Fully Connected layers
- Dropout for regularization

---

## ⚙️ Enhancements
- Data Augmentation (RandomCrop, HorizontalFlip)
- Batch Normalization
- Dropout

---

## 🧪 Experiments
Two experiments were conducted:

### Experiment A:
- Optimizer: Adam
- Learning Rate: 0.001

### Experiment B:
- Optimizer: SGD
- Learning Rate: 0.01

---

## 📊 Results

| Model | Optimizer | Test Accuracy | Test Loss |
|------|----------|--------------|----------|
| A | Adam | 75.42% | 0.7110 |
| B | SGD | 75.04% | 0.7116 |

---

## 📈 Observations
- Adam converged faster in early epochs
- SGD achieved similar final performance
- Model reached ~75% accuracy on CIFAR-10

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
