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
