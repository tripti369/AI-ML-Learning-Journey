# Normalization vs Standardization

Both Normalization and Standardization are feature scaling techniques used in Machine Learning. They help bring numerical values to a similar scale so that no feature dominates others during model training.

## Normalization

Normalization scales data between 0 and 1.

### Formula

(X - Xmin) / (Xmax - Xmin)

### Example

Suppose values are:

10, 20, 30

After normalization:

10 → 0

20 → 0.5

30 → 1

### Advantages

* Values stay between 0 and 1
* Easy to understand
* Works well with KNN and Neural Networks
* Useful when data has fixed boundaries

### Limitations

* Highly affected by outliers
* If a new value appears outside the range, scaling may become inconsistent

---

## Standardization

Standardization transforms data around the mean.

### Formula

(X - Mean) / Standard Deviation

### Example

If average salary is 50,000 and a person's salary is higher than average, its standardized value will be positive. If it is lower than average, the value will be negative.

### Advantages

* Mean becomes approximately 0
* Standard deviation becomes approximately 1
* Less sensitive to outliers than normalization
* Works well for many ML algorithms

### Limitations

* Values are not limited to a fixed range
* Slightly harder to interpret

---

## Key Differences

| Basis          | Normalization        | Standardization             |
| -------------- | -------------------- | --------------------------- |
| Range          | 0 to 1               | No fixed range              |
| Mean           | Not centered         | Around 0                    |
| Outlier Effect | High                 | Lower                       |
| Best Used In   | KNN, Neural Networks | Regression, SVM, PCA        |
| Formula Uses   | Min and Max values   | Mean and Standard Deviation |

---

## When Should We Use Them?

Use **Normalization** when:

* Data has different ranges
* Using KNN
* Using Neural Networks

Use **Standardization** when:

* Using Linear Regression
* Using Logistic Regression
* Using SVM
* Using PCA

---

## Conclusion

Normalization and Standardization are both important preprocessing techniques. Normalization scales data between 0 and 1, while Standardization transforms data around the mean. The choice depends on the dataset and the machine learning algorithm being used.
