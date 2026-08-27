# Comparative Study of Deep CNN Architectures and Transfer Learning

This repository contains the implementation and experimental results for **Experiment 4 of the Deep Learning Laboratory (CS3807)**. The experiment studies the evolution of Convolutional Neural Network architectures and compares classical and modern approaches using the **CIFAR-10 dataset**.

The work includes CNNs trained from scratch, pretrained models using transfer learning, fine-tuning experiments, hyperparameter analysis, and a comparison of model accuracy, parameter count, and training time.

---

## Objectives

The objectives of this experiment are to:

- Study the evolution of major CNN architectures.
- Understand the design principles behind **LeNet-5, AlexNet, VGG16, GoogLeNet, and ResNet**.
- Implement image classification using the **CIFAR-10 dataset**.
- Apply **transfer learning** using pretrained ImageNet models.
- Compare frozen-base training and **fine-tuning**.
- Evaluate the effects of different hyperparameters.
- Compare architectures based on **test accuracy, parameter count, and training time**.

---

## Architectures Studied

### LeNet-5
A lightweight classical CNN used as a baseline. It contains convolution, pooling, and fully connected layers and is significantly smaller than modern architectures.

### AlexNet-style CNN
A deeper CNN inspired by AlexNet and adapted for CIFAR-10's `32×32` input size. The implementation uses convolutional layers, ReLU activation, max pooling, and dropout.

### GoogLeNet / Inception-style CNN
A CIFAR-10 adaptation of GoogLeNet using Inception modules. Each module processes feature maps through multiple parallel branches, including:

- `1×1` convolutions
- `1×1 → 3×3` convolutions
- `1×1 → 5×5` convolutions
- Max pooling followed by a `1×1` projection

The outputs are concatenated to create multi-scale feature representations.

### MobileNetV2
Used as the primary transfer-learning model. The pretrained ImageNet convolutional base is combined with a custom CIFAR-10 classification head and subsequently fine-tuned.

### VGG16
A pretrained VGG16 model used for transfer learning on the CIFAR-10 subset.

### ResNet50
A pretrained ResNet50 model used to investigate residual learning and transfer-learning performance.

---

## Dataset

The experiments use the **CIFAR-10 dataset**.

| Property | Value |
|---|---|
| Training Images | 50,000 |
| Test Images | 10,000 |
| Number of Classes | 10 |
| Image Size | `32 × 32 × 3` |
| Task | Multi-class Image Classification |

The ten classes are:

```text
airplane
automobile
bird
cat
deer
dog
frog
horse
ship
truck
