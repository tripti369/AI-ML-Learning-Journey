# Case Study: Loan Approval Prediction

## Objective

Predict whether a loan application will be approved or rejected.

---

## Target Variable

Loan_Status

- Approved
- Rejected

---

## Possible Features

### Numerical Features

1. Applicant Income
2. Coapplicant Income
3. Loan Amount
4. Loan Term
5. Number of Dependents

### Categorical Features

6. Gender
7. Married
8. Education
9. Self Employed
10. Property Area

---

## Features Requiring Scaling

- Applicant Income
- Coapplicant Income
- Loan Amount
- Loan Term

Reason:
These features have different ranges and should be scaled before model training.

---

## Features Requiring Encoding

- Gender
- Married
- Education
- Self Employed
- Property Area

Reason:
Machine learning algorithms cannot directly process text values.

---

## Features That Could Be Removed

### Loan_ID

Reason:
Unique identifier with no predictive value.

### Applicant Name (if available)

Reason:
Names generally do not influence loan approval decisions.

---

# Public Dataset Analysis

Dataset: Titanic Survival Prediction Dataset (Kaggle)

## Target Variable

Survived

- 0 = Did Not Survive
- 1 = Survived

## Number of Features

11 primary features

Examples:
- Age
- Sex
- Fare
- Pclass
- Embarked
- SibSp
- Parch

## Required Preprocessing

- Handle missing values
- Encode categorical variables
- Scale numerical features
- Remove irrelevant columns

## First Algorithm to Try

Decision Tree Classifier

### Why?

- Easy to understand
- Works with mixed data types
- Requires minimal preprocessing
- Good baseline model
