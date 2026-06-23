# Day 07 - Supervised Learning Algorithms

## What is Supervised Learning?

Supervised Learning is a type of Machine Learning in which the model is trained using labelled data. The dataset contains both input features and correct output values. The model learns patterns from the data and makes predictions on new data.

### Examples
- House Price Prediction
- Email Spam Detection
- Loan Approval Prediction
- Student Pass/Fail Prediction

---

## Classification vs Regression

| Classification | Regression |
|---------------|------------|
| Predicts categories | Predicts numerical values |
| Output is discrete | Output is continuous |
| Example: Spam or Not Spam | Example: House Price Prediction |

---

## Linear Regression

### What problem does it solve?
Linear Regression is used for predicting continuous numerical values.

### How it works
It finds the best-fit line that represents the relationship between input variables and output variables.

### Real-World Applications
- House Price Prediction
- Salary Prediction
- Sales Forecasting
- Demand Forecasting

### Advantages
- Simple and easy to understand
- Fast training
- Easy interpretation

### Limitations
- Assumes linear relationships
- Sensitive to outliers

---

## Logistic Regression

### Why is it used for Classification?
Although its name contains "Regression", Logistic Regression is mainly used for classification problems. It predicts the probability that a data point belongs to a particular class.

### Applications
- Spam Detection
- Disease Prediction
- Student Pass/Fail Prediction

### Advantages
- Fast and efficient
- Easy to interpret
- Works well for binary classification

### Limitations
- Not suitable for highly complex relationships

---

## Decision Tree

### How does it make decisions?
A Decision Tree asks a series of questions and splits data based on conditions.

Example:

Is Income > 50,000?
├── Yes → Approve Loan
└── No → Reject Loan

### Advantages
- Easy to understand
- Handles numerical and categorical data
- No feature scaling required

### Limitations
- Can easily overfit the training data

---

## Random Forest

### Why is it more powerful than a Decision Tree?
Random Forest combines multiple Decision Trees and uses their collective predictions.

### Advantages
- Higher accuracy
- Less overfitting
- More stable predictions

### Limitations
- Less interpretable
- Requires more computation

---

## When to Use Each Algorithm?

| Situation | Recommended Algorithm |
|-----------|----------------------|
| Predict numerical values | Linear Regression |
| Binary classification | Logistic Regression |
| Need easy interpretation | Decision Tree |
| Need higher accuracy | Random Forest |
