# Ensemble Learning - Day 10

## What is Ensemble Learning?

Ensemble Learning is a Machine Learning technique where multiple models are combined to produce a better prediction than a single model.

Instead of relying on one model, several models work together, making predictions more accurate and reliable.

---

## Why Combine Multiple Models?

Using only one model may lead to:

- High variance
- High bias
- Overfitting
- Lower prediction accuracy

Combining models helps to:

- Improve accuracy
- Reduce overfitting
- Increase stability
- Make predictions more reliable

---

## Weak Learner

A Weak Learner is a model that performs only slightly better than random guessing.

Characteristics:

- Simple model
- Low prediction power
- High bias
- Fast training

Example:

- Decision Stump
- Small Decision Tree

---

## Strong Learner

A Strong Learner is a model that provides high prediction accuracy.

Characteristics:

- Better generalization
- Lower error
- More reliable predictions

Strong learners are often created by combining multiple weak learners.

---

# Bagging (Bootstrap Aggregating)

Bagging trains multiple models independently using different random subsets of the dataset.

Each model gives its own prediction.

The final prediction is obtained by:

Classification → Majority Voting

Regression → Average Prediction

Advantages:

- Reduces variance
- Prevents overfitting
- Improves stability

Example:

Random Forest

---

# Boosting

Boosting trains models sequentially.

Each new model focuses on correcting the mistakes made by the previous one.

The final prediction is a weighted combination of all models.

Advantages:

- Reduces bias
- Improves accuracy
- Learns from previous errors

Examples:

- AdaBoost
- Gradient Boosting
- XGBoost

---

# Random Forest

Random Forest is a Bagging-based algorithm.

It creates many Decision Trees using different random samples.

Each tree makes its own prediction.

The final result is obtained using majority voting (classification) or averaging (regression).

Advantages:

- Handles missing values well
- Less overfitting
- High accuracy
- Works with large datasets

Disadvantages:

- Slower than a single tree
- Harder to interpret

---

# AdaBoost

AdaBoost stands for Adaptive Boosting.

It trains models one after another.

Incorrectly classified samples receive higher weights so that the next model focuses more on them.

Advantages:

- Improves weak learners
- Good prediction accuracy
- Easy to implement

Limitations:

- Sensitive to noisy data
- Sensitive to outliers

---

# XGBoost

XGBoost stands for Extreme Gradient Boosting.

It is an advanced version of Gradient Boosting designed for speed and performance.

Why is it popular?

- Fast training
- Parallel processing
- Regularization reduces overfitting
- Handles missing values automatically
- Excellent prediction accuracy

Applications:

- Fraud Detection
- Loan Approval
- Disease Prediction
- Recommendation Systems
- Customer Churn Prediction
- Kaggle Competitions

---

# Real-World Applications

1. Credit Card Fraud Detection
2. Disease Diagnosis
3. Customer Churn Prediction
4. Loan Approval
5. Stock Market Prediction
6. Recommendation Systems
7. Spam Email Detection
8. Insurance Risk Analysis

---

# Summary

Ensemble Learning combines multiple models to produce stronger predictions.

Bagging focuses on reducing variance by training models independently.

Boosting focuses on reducing bias by training models sequentially.

Random Forest is a Bagging algorithm.

AdaBoost and XGBoost are Boosting algorithms.

XGBoost is widely used because of its speed, accuracy, and ability to handle complex datasets.
