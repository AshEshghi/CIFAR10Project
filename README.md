# CIFAR10Project

This repository presents a **NumPy-only implementation of a Multilayer Perceptron (MLP)** for **CIFAR-10 image classification**. The project was developed as an educational deep learning assignment focused on understanding the internal mechanics of neural networks without using high-level frameworks such as PyTorch or TensorFlow.

The implementation covers the full pipeline: loading CIFAR-10 data, preprocessing, defining a one-hidden-layer MLP, implementing forward and backward propagation, training with mini-batch gradient descent, comparing activation functions and initialization methods, and visualizing training performance through loss and accuracy curves.

---

## What is this project?

This project uses the **CIFAR-10 dataset** as the image classification task and an **MLP (Multilayer Perceptron)** as the model architecture.

- **CIFAR-10** is a benchmark dataset of 32×32 RGB images from 10 classes.
- **MLP** is a fully connected neural network that learns nonlinear decision boundaries through hidden layers and activation functions.

Although MLPs are not as strong as convolutional neural networks for image tasks, they are highly valuable for learning the mathematical foundations of deep learning.

---

## Project Focus

The main purpose of this repository is to demonstrate:

- neural network implementation from scratch
- the role of activation functions in nonlinear modeling
- the effect of initialization methods on training stability
- forward propagation and backpropagation using NumPy
- experimental comparison of different MLP configurations on CIFAR-10

---

## What I Implemented

This repository contains my own implementation of:

- CIFAR-10 batch loading from the original Python dataset files
- image normalization to the range `[0,1]`
- flattening each `32×32×3` image into a `3072`-dimensional vector
- one-hot encoding of class labels
- custom activation functions:
  - ReLU
  - Tanh
  - Sigmoid
- custom weight initialization methods:
  - random normal
  - Xavier
  - He
- a fully connected linear layer with forward and backward methods
- a one-hidden-layer MLP for multi-class classification
- softmax output
- cross-entropy loss
- classification accuracy metric
- mini-batch SGD-style training
- training history visualization with loss and accuracy plots

> Note: This is a from-scratch educational implementation. The architecture, training flow, experiments, and visualizations were implemented for this project using NumPy.

---

## Dataset

- **Dataset:** CIFAR-10
- **Type:** 32×32 RGB images
- **Classes:** airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- **Included in repository:** No

The dataset is not uploaded to this repository because of size and because it should be downloaded separately.

### Expected local dataset path

```text
cifar-10-batches-py/
