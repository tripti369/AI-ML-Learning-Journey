## What is Feature Engineering?

Feature Engineering is the process of creating, transforming, or selecting useful features from raw data to improve machine learning model performance.

### Example
- Date of Birth → Age
- Joining Date → Years of Experience
- Purchase History → Total Spending

### Importance
- Improves model accuracy
- Helps models learn patterns better
- Reduces noise
- Makes training more efficient

---

## What is Feature Selection?

Feature Selection means choosing only the most useful features for training a machine learning model.

### Benefits
- Faster training
- Better model performance
- Reduces overfitting
- Simplifies the model

---

## Handling Missing Values

Missing values occur when some data is unavailable.

### Methods

### 1. Remove Missing Data
Delete rows or columns containing missing values.

### 2. Mean Imputation
Replace missing values with the average value.

### 3. Median Imputation
Replace missing values with the middle value.

### 4. Mode Imputation
Replace missing values with the most frequent value.

---

## Encoding Categorical Variables

Machine learning models cannot directly understand text data.

### Label Encoding

Converts categories into numerical values.

Example:
- Male = 0
- Female = 1

### One-Hot Encoding

Creates separate columns for each category.

Example:

| Color | Red | Blue | Green |
|--------|-----|------|------|
| Red | 1 | 0 | 0 |
| Blue | 0 | 1 | 0 |
| Green | 0 | 0 | 1 |

---

## Feature Scaling

Feature Scaling brings numerical values into a similar range.

Example:
- Age = 25
- Salary = 500000

Without scaling, Salary may dominate Age.

---

## Normalization

Scales data between 0 and 1.

Formula:

Xnew = (X − Xmin) / (Xmax − Xmin)

Used in:
- KNN
- Neural Networks

---

## Standardization

Transforms data around the mean.

Formula:

Z = (X − Mean) / Standard Deviation

Used in:
- Linear Regression
- Logistic Regression
- SVM
- PCA

---

## Outliers

Outliers are extreme values that differ significantly from the rest of the data.

Example:
20, 22, 21, 19, 1000

Here, 1000 is an outlier.

### Impact
- Affects model accuracy
- Distorts statistical measures

### Handling Methods
- Remove outliers
- Cap extreme values
- Apply transformations

---

## How Preprocessing Affects Model Performance

Proper preprocessing:
- Improves accuracy
- Reduces errors
- Speeds up training
- Produces reliable predictions
