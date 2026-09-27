# Autoencoders, Denoising Autoencoders and Variational Autoencoders

This repository contains the implementation and experimental results for **Experiment 7 of the Deep Learning Laboratory (CS3807)**. The experiment studies different types of autoencoders using the **MNIST dataset**, covering image reconstruction, denoising, latent-space analysis, and image generation.

The work includes fully connected autoencoders, convolutional autoencoders, denoising autoencoders, and variational autoencoders, along with reconstruction metrics, latent-dimension studies, and additional experiments.

---

## Objectives

The objectives of this experiment are to:

- Understand the encoder–latent–decoder architecture of autoencoders.
- Implement a **Fully Connected Autoencoder**.
- Implement a **Convolutional Autoencoder**.
- Implement a **Denoising Autoencoder** using Gaussian and salt-and-pepper noise.
- Evaluate reconstruction using **MSE, MAE, and SSIM**.
- Study the effect of latent-space dimensionality.
- Implement a **Variational Autoencoder (VAE)**.
- Visualize the VAE latent space.
- Generate new images using the learned latent distribution.
- Perform latent-space interpolation.

---

## Models Studied

### Fully Connected Autoencoder

A basic autoencoder using fully connected layers.

```text
784 → 128 → 32 → 16 → 32 → 128 → 784
```

### Convolutional Autoencoder

A convolution-based autoencoder that preserves the spatial structure of MNIST images using convolution, pooling, and upsampling layers.

### Denoising Autoencoder

A convolutional autoencoder trained to reconstruct clean images from corrupted inputs.

Noise types studied:
- **Gaussian noise:** $\sigma = 0.1, 0.2, 0.3$
- **Salt-and-pepper noise:** $p = 0.05, 0.10, 0.20$

### Variational Autoencoder

A VAE with a 2-dimensional latent space, allowing visualization of the learned representation and generation of new MNIST-like images.

---

## Dataset

The experiments use the MNIST Handwritten Digit Dataset.

| Property | Value |
| :--- | :--- |
| **Training Images** | 60,000 |
| **Test Images** | 10,000 |
| **Number of Classes** | 10 |
| **Image Size** | $28 \times 28 \times 1$ |
| **Pixel Range** | $[0, 1]$ |
