# How Machine Learning Models Learn

## 1. What is Model Training?

Model Training is the process where a machine learning model learns patterns from data. During training, the model makes predictions, compares them with actual answers, finds errors, and improves itself.

Example:
A house price prediction model learns from past house sales data to predict future house prices.

---

## 2. What is a Prediction?

A Prediction is the output produced by a machine learning model.

Example:
If a model predicts that a house price is ₹50,00,000, then ₹50,00,000 is the prediction.

---

## 3. What is an Actual Value?

The Actual Value is the real correct answer present in the dataset.

Example:
If the real house price is ₹55,00,000, then ₹55,00,000 is the actual value.

---

## 4. What is an Error?

Error is the difference between the predicted value and the actual value.

Formula:

Error = Actual Value - Predicted Value

Example:

Actual Price = ₹55,00,000

Predicted Price = ₹50,00,000

Error = ₹5,00,000

A smaller error means better predictions.

---

## 5. What is a Loss Function?

A Loss Function measures how wrong the model's predictions are.

It converts the error into a number that the model can understand.

### Why do we need a Loss Function?

* To measure prediction quality
* To tell the model whether it is performing well or poorly
* To help the model improve during training

### How does it help the model?

* Large loss = Poor prediction
* Small loss = Better prediction
* Zero loss = Perfect prediction

---

## 6. What is an Epoch?

An Epoch means one complete pass through the entire training dataset.

Example:

If a dataset contains 1000 records and the model processes all 1000 records once, then 1 Epoch is completed.

---

## 7. What is an Iteration?

An Iteration is one update of the model's parameters.

If data is divided into batches, every batch processed creates one iteration.

Example:

Dataset = 1000 records

Batch Size = 100

Iterations per Epoch = 1000 / 100 = 10

---

## 8. What is Batch Size?

Batch Size is the number of training samples processed at one time before updating the model.

Example:

Dataset = 1000 records

Batch Size = 100

The model processes 100 records at a time.

---

## 9. How Does a Model Improve Over Time?

Step 1: Take data from the dataset

Step 2: Make predictions

Step 3: Compare predictions with actual values

Step 4: Calculate loss

Step 5: Update model parameters

Step 6: Repeat for many epochs

As training continues, loss decreases and predictions become more accurate.
