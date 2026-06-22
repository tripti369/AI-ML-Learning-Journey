# Day 06 - Evaluating Machine Learning Models

## Why Do We Evaluate a Model?

Model evaluation helps us determine how well a machine learning model performs on unseen data. It allows us to:

* Measure prediction quality
* Identify errors
* Compare different models
* Detect overfitting and underfitting
* Improve model performance

---

## Training Accuracy vs Testing Accuracy

### Training Accuracy

Accuracy calculated on the training dataset used to train the model.

### Testing Accuracy

Accuracy calculated on unseen test data.

### Interpretation

| Scenario     | Training Accuracy | Testing Accuracy | Meaning                  |
| ------------ | ----------------- | ---------------- | ------------------------ |
| Good Model   | High              | High             | Generalizes well         |
| Overfitting  | Very High         | Low              | Memorized training data  |
| Underfitting | Low               | Low              | Failed to learn patterns |

---

## Confusion Matrix

A Confusion Matrix is a table used to evaluate classification models by comparing actual values with predicted values.

| Actual / Predicted | Positive            | Negative            |
| ------------------ | ------------------- | ------------------- |
| Positive           | True Positive (TP)  | False Negative (FN) |
| Negative           | False Positive (FP) | True Negative (TN)  |

### Components

#### True Positive (TP)

Actual Positive and Predicted Positive.

#### True Negative (TN)

Actual Negative and Predicted Negative.

#### False Positive (FP)

Actual Negative but Predicted Positive.

#### False Negative (FN)

Actual Positive but Predicted Negative.

---

## Evaluation Metrics

### Accuracy

Measures overall correctness.

Formula:

Accuracy = (TP + TN) / (TP + TN + FP + FN)

---

### Precision

Measures how many predicted positives are actually positive.

Formula:

Precision = TP / (TP + FP)

---

### Recall

Measures how many actual positives are correctly identified.

Formula:

Recall = TP / (TP + FN)

---

### F1-Score

Harmonic mean of Precision and Recall.

Formula:

F1 = 2 × (Precision × Recall) / (Precision + Recall)

---

## When Accuracy Can Be Misleading

Consider a fraud detection dataset:

* 990 normal transactions
* 10 fraudulent transactions

If a model predicts every transaction as normal:

Accuracy = 99%

However, it detects zero fraud cases.

Therefore, accuracy alone may not reflect actual model performance.

---

## Imbalanced Dataset

An imbalanced dataset occurs when one class has significantly more samples than another.

Example:

| Class  | Count |
| ------ | ----- |
| Normal | 9900  |
| Fraud  | 100   |

In such situations, Precision, Recall, and F1-Score are more informative than Accuracy.
