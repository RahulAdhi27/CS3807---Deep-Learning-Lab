# RNNs, LSTMs, GRUs and Sequence Learning

This repository contains the implementation and experimental results for **Experiment 6 of the Deep Learning Laboratory (CS3807)**. The experiment studies recurrent neural networks for sequence modeling, activity recognition, video classification, and sequence-to-sequence learning.

The work includes Vanilla RNNs, LSTMs, GRUs, sequence-length analysis, CNN-RNN architectures for video understanding, and an Encoder-Decoder LSTM for sequence reversal.

---

## Objectives

The objectives of this experiment are to:

- Understand recurrent neural networks and **Backpropagation Through Time (BPTT)**.
- Implement and compare **Vanilla RNN, LSTM and GRU** models.
- Perform human activity recognition using the **UCI HAR dataset**.
- Study the effect of different sequence lengths on model performance.
- Implement **CNN-LSTM and CNN-GRU** architectures for video classification.
- Understand Encoder-Decoder architectures for sequence-to-sequence learning.
- Perform sequence reversal using an **Encoder-Decoder LSTM**.
- Evaluate models using accuracy, precision, recall, F1-score and confusion matrices.

---

## Models Studied

### Vanilla RNN

A basic recurrent neural network used for modeling temporal dependencies in sequential data.

### LSTM

A Long Short-Term Memory network designed to capture longer-term dependencies using input, forget and output gates.

### GRU

A gated recurrent architecture that provides a simpler alternative to LSTM using update and reset gates.

### CNN-LSTM / CNN-GRU

CNNs are used to extract spatial features from video frames, followed by LSTM or GRU layers to model temporal information.

### Encoder-Decoder LSTM

An Encoder-Decoder architecture is used for sequence-to-sequence learning, with the model trained to reverse input sequences.

---

## Datasets

The experiments use:

- **UCI Human Activity Recognition (HAR)** dataset for sensor-based activity classification.
- **UCF101** dataset for video action recognition.
- Synthetic sequences for the sequence reversal task.

---

## Experiments

The experiments include:

- BPTT implementation and analysis.
- Human activity classification using RNN, LSTM and GRU.
- Sequence-length comparison using different temporal windows.
- Video action classification using CNN-LSTM and CNN-GRU.
- Encoder-Decoder LSTM based sequence reversal.
- Evaluation using classification metrics and confusion matrices.
