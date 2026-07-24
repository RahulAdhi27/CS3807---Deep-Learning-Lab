# CS3807 – Deep Learning Laboratory — Experiment 2
## Implementation of a Multi-Layer Perceptron (MLP) for Multi-Class Image Classification

A TensorFlow/Keras MLP trained on the **Fashion-MNIST** dataset, with automated hyperparameter optimization via Randomized Search and a baseline-vs-optimized performance comparison.

---

## Overview

This project builds an MLP image classifier for Fashion-MNIST, covering image preprocessing (flattening and normalization), model construction, training, and evaluation. A baseline model with a fixed architecture is trained first, followed by automated hyperparameter optimization (RandomizedSearchCV with the SciKeras wrapper and 5-fold cross-validation) to find and retrain an improved configuration.

**Course:** CS3807 – Deep Learning Laboratory
**Institution:** Shiv Nadar University Chennai
**Program:** B.Tech Artificial Intelligence & Data Science, Semester V

---

## Dataset

- **Name:** Fashion-MNIST
- **Training images:** 60,000
- **Testing images:** 10,000
- **Classes:** 10 (T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot) — perfectly balanced, 6,000 samples per class
- **Image size:** 28 × 28 grayscale, flattened to a 784-dimensional vector for the Dense layers

---

## Results

**Baseline model:** `784 → Dense(128, ReLU) → Dense(64, ReLU) → Dense(10, Softmax)`

**Optimized model (best hyperparameters found):** 1 hidden layer, 256 neurons, ReLU, Adam optimizer, learning rate 0.001, batch size 128, dropout 0.0

| Metric | Baseline | Optimized |
|---|---|---|
| Accuracy | 0.8838 | 0.8908 |
| Precision | 0.8877 | 0.8909 |
| Recall | 0.8838 | 0.8908 |
| F1-score | 0.8847 | 0.8906 |
| Training Time (s) | 115.73 | 29.70 |

The optimized model improves on every metric while training roughly **4× faster** than the baseline. Full details, all generated plots, and their interpretations are in the lab report.

---

## References

1. I. Goodfellow, Y. Bengio, A. Courville, *Deep Learning*, MIT Press, 2016.
2. C. M. Bishop, *Pattern Recognition and Machine Learning*, Springer, 2006.
3. S. Haykin, *Neural Networks and Learning Machines*, Pearson, 2009.
4. [Fashion-MNIST Dataset](https://github.com/zalandoresearch/fashion-mnist)
5. [TensorFlow/Keras Documentation](https://www.tensorflow.org/api_docs)
6. [SciKeras Documentation](https://www.adriangb.com/scikeras/)
7. [Scikit-learn Documentation: `RandomizedSearchCV`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html)
