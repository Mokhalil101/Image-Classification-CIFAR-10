🧠 CIFAR-10 Image Classification using CNN
📌 Project Description

This project implements a Deep Learning Convolutional Neural Network (CNN) for image classification using the CIFAR-10 real-world dataset.
The objective is to build, train, evaluate, and compare CNN models using different optimization techniques and analyze their performance through multiple experiments and visualizations.

📊 Dataset
Dataset Name: CIFAR-10
Type: Real-world image dataset
Number of Classes: 10
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
Image Size: 32 × 32 RGB
Source:
https://www.cs.toronto.edu/~kriz/cifar.html
🔄 Data Preprocessing

The following preprocessing steps were applied:

Normalization of image pixel values
Data Augmentation (for training data only):
Random Horizontal Flip
Random Crop with padding
Dataset Splitting:
80% Training
20% Validation
Separate Test Set
🧠 Model Architecture

A Convolutional Neural Network (CNN) was implemented with the following structure:

Convolutional Layers: 3 layers
Activation Function: ReLU
Batch Normalization
Max Pooling
Fully Connected Layers
Dropout (0.5) for regularization

This architecture contains multiple hidden layers as required.

⚙️ Model Enhancements

The following enhancement techniques were applied:

✅ Data Augmentation
✅ Batch Normalization
✅ Dropout
🏋️ Training Details
Loss Function: CrossEntropyLoss
Metrics Monitored:
Training Loss
Validation Loss
Training Accuracy
Validation Accuracy
🧪 Experiments (Mandatory)

Two experiments were conducted by varying the optimizer, while keeping all other parameters constant.

🔬 Experiment A
Optimizer: Adam
Learning Rate: 0.001
🔬 Experiment B
Optimizer: SGD
Learning Rate: 0.01
📈 Visualizations

The following plots were generated:

Training vs Validation Loss
Training vs Validation Accuracy
Adam vs SGD Training Loss
Adam vs SGD Validation Loss
Adam vs SGD Training Accuracy
Adam vs SGD Validation Accuracy

These visualizations clearly show the learning behavior and convergence differences between optimizers.

📊 Results
Model	Optimizer	Test Accuracy	Test Loss
A	Adam	75.42%	0.7110
B	SGD	75.04%	0.7116
🧠 Observations
Adam converges faster during early epochs.
SGD achieves comparable final performance but with slower convergence.
The CNN model achieved approximately 75% accuracy on the CIFAR-10 test dataset.

## 🚀 How to Run

```bash
pip install -r requirements.txt
