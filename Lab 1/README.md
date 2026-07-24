# CS3807 – Deep Learning Laboratory — Experiment 1
## Implementation of a Single Layer Perceptron for Binary Classification

A from-scratch NumPy implementation of the classical Single Layer Perceptron, trained and evaluated on the **UCI Banknote Authentication Dataset** to distinguish authentic banknotes from forged ones.

---

## Overview

This project implements the perceptron learning algorithm without relying on any machine learning framework's built-in perceptron. It covers the full pipeline: exploratory data analysis, preprocessing, from-scratch model implementation, training with weight/bias tracking, evaluation, and a hyperparameter (learning-rate) study.

**Course:** CS3807 – Deep Learning Laboratory
**Institution:** Shiv Nadar University Chennai
**Program:** B.Tech Artificial Intelligence & Data Science, Semester V

---

## Dataset

- **Name:** Banknote Authentication Dataset
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/267/banknote+authentication)
- **Instances:** 1372
- **Features:** 4 numerical (Variance, Skewness, Curtosis, Entropy of wavelet-transformed banknote images)
- **Classes:** 2 — `0` = Authentic (762 samples), `1` = Forged (610 samples)
- **Missing values:** None

---

## Results

| Metric | Value |
|---|---|
| Final Weights | `[-0.1985, -0.2258, -0.2102, -0.0282]` |
| Final Bias | `-0.1000` |
| Accuracy | 0.9891 |
| Precision | 0.9837 |
| Recall | 0.9918 |
| F1-score | 0.9878 |

Only **3 of 275** test samples were misclassified. Full details, all generated plots, and their interpretations are in the lab report.

---

## References

1. F. Rosenblatt, "The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain," *Psychological Review*, 1958.
2. I. Goodfellow, Y. Bengio, A. Courville, *Deep Learning*, MIT Press, 2016.
3. C. M. Bishop, *Pattern Recognition and Machine Learning*, Springer, 2006.
4. S. Haykin, *Neural Networks and Learning Machines*, Pearson, 2009.
5. M. Minsky, S. Papert, *Perceptrons: An Introduction to Computational Geometry*, MIT Press, 1969.
6. UCI Machine Learning Repository – [Banknote Authentication Dataset](https://archive.ics.uci.edu/dataset/267/banknote+authentication)
7. [Scikit-learn Documentation: `sklearn.linear_model.Perceptron`](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Perceptron.html)
