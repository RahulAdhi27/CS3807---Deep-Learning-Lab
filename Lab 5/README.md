# Deep Learning Lab 5

This repository contains the implementation and experimental work completed for **Experiment 5** as part of the **CS3807 – Deep Learning Laboratory** course.

## Title

**Performance Optimization and Regularization Techniques for Deep Neural Networks**

## Overview

This experiment investigates different techniques used to improve the training stability, generalization performance, and overall efficiency of deep neural networks.

The experiments focus on understanding the effects of:

- Weight initialization
- Batch normalization
- Regularization techniques
- Different optimizers
- Learning rate
- Batch size
- Dropout rate
- Transfer learning and fine-tuning
- Cross-validation
- Final model evaluation

The objective is to study how architectural and training hyperparameters influence model convergence, overfitting, validation performance, and generalization.

---

## Tasks Performed

### Task 1 – Weight Initialization

Different weight initialization strategies were evaluated by comparing their effect on training loss and model convergence.

The experiment examines how initialization influences:

- Training stability
- Speed of convergence
- Gradient propagation
- Final model performance

---

### Task 2 – Regularization Techniques

Different regularization approaches were applied and compared to study their effectiveness in reducing overfitting.

The following configurations were considered:

- No regularization
- Batch normalization
- Dropout
- L2 regularization

Training and validation accuracy and loss were compared across the different configurations.

---

### Task 3 – Batch Normalization

The effect of batch normalization on model training was investigated.

The comparison focuses on:

- Training behaviour
- Convergence
- Validation accuracy
- Training loss
- Model stability

---

### Task 4 – Optimizer Comparison

Different optimization algorithms were evaluated to compare their effect on the training process.

The experiment compares optimizer performance using training loss and validation accuracy curves, along with an overall numerical comparison of the configurations.

---

### Task 5 – Hyperparameter Study

The influence of important training hyperparameters was investigated.

The following hyperparameters were varied:

- Learning rate
- Batch size
- Dropout rate

The resulting validation performance was compared to identify suitable configurations for the model.

---

### Task 6 – Transfer Learning and Fine-Tuning

Transfer learning was performed using a pretrained deep learning model.

The experiment involved:

1. Using pretrained weights as a feature extractor.
2. Training a classification head on the target dataset.
3. Unfreezing selected pretrained layers.
4. Fine-tuning the model with a smaller learning rate.
5. Comparing feature extraction and fine-tuning performance.

Training and validation behaviour were analysed using accuracy and loss curves.

---

### Task 7 – 5-Fold Cross-Validation

Multiple model configurations were evaluated using **5-fold cross-validation**.

The cross-validation experiment was used to obtain a more reliable estimate of model performance and to compare configurations based on their validation results across multiple folds.

---

### Task 8 – Final Model Evaluation

The selected model configuration was evaluated on the independent test set.

The final evaluation includes:

- Test accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Training time
- Parameter count
- Analysis of misclassified samples

---

## Experimental Results

The experiment generated plots and result tables covering:

- Training loss under different weight initialization methods
- Training and validation accuracy for regularization techniques
- Training and validation loss for regularization techniques
- Batch normalization comparison
- Optimizer training loss comparison
- Optimizer validation accuracy comparison
- Learning rate versus validation accuracy
- Batch size versus validation accuracy
- Dropout rate versus validation accuracy
- Feature extraction versus fine-tuning comparison
- Fine-tuning loss comparison
- Cross-validation accuracy
- Final model confusion matrix
- Misclassified test images
- Overall model metrics

These results were used to analyse the effect of training and regularization choices on model performance and generalization.

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
