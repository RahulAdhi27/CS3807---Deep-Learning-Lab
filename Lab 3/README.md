# Experiment 3: Convolutional Neural Networks for Image Classification

## Objective

To understand and implement Convolutional Neural Networks (CNNs) for multi-class image classification using the CIFAR-10 dataset. The experiment includes studying convolution operations, kernel sizes, stride, padding, pooling methods, feature maps, CNN training, and model evaluation.

## Dataset

**CIFAR-10**

- Training images: 50,000
- Testing images: 10,000
- Classes: 10
- Image size: 32 × 32 × 3
- Classes:
  - Airplane
  - Automobile
  - Bird
  - Cat
  - Deer
  - Dog
  - Frog
  - Horse
  - Ship
  - Truck

The pixel values are normalized to the range `[0, 1]`.

## Tasks Performed

### Task 1: Dataset Exploration

- Loaded the CIFAR-10 dataset
- Printed dataset dimensions
- Displayed sample images
- Visualized class distributions

### Task 2: Kernel Size Comparison

Compared convolution layers using:

- 3 × 3 kernels
- 5 × 5 kernels
- 7 × 7 kernels

The feature-map dimensions were recorded and compared.

### Task 3: Stride and Padding

Studied the effect of:

- Stride = 1
- Stride = 2
- Same padding
- Valid padding

The output feature-map dimensions were calculated and verified experimentally.

### Task 4: Feature Map Visualization

- Extracted intermediate activations from the CNN
- Visualized feature maps after the convolution layers
- Displayed learned filters from the first convolution layer

### Task 5: Pooling Comparison

Compared:

- Max Pooling
- Average Pooling

Both output dimensions and validation performance were analyzed.

### Task 6: CNN Training

The CNN architecture used was:

```text
Input
  ↓
Conv2D
  ↓
ReLU
  ↓
MaxPooling
  ↓
Conv2D
  ↓
ReLU
  ↓
MaxPooling
  ↓
Flatten
  ↓
Dense
  ↓
Softmax
