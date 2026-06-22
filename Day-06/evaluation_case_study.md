# Evaluation Case Study: Disease Detection

## Problem Statement

Build a machine learning model that predicts whether a patient has a disease.

---

## Confusion Matrix Interpretation

### True Positive (TP)

Patient has the disease and the model predicts disease.

### True Negative (TN)

Patient does not have the disease and the model predicts healthy.

### False Positive (FP)

Patient is healthy but the model predicts disease.

### False Negative (FN)

Patient has the disease but the model predicts healthy.

---

## Most Important Evaluation Metric

### Recall

Recall is the most important metric in disease detection because missing a diseased patient can have serious consequences.

Formula:

Recall = TP / (TP + FN)

A high Recall ensures that most disease cases are detected.

---

## Why Accuracy Alone Is Dangerous

Suppose:

* 950 healthy patients
* 50 diseased patients

If the model predicts every patient as healthy:

Accuracy = 95%

Although accuracy appears high, the model fails to detect any disease cases.

Therefore, relying only on accuracy is dangerous.

---

## Real-World Consequences

### False Positive

* Unnecessary medical tests
* Increased healthcare costs
* Patient anxiety

### False Negative

* Disease remains untreated
* Delayed diagnosis
* Health complications
* Possible loss of life

---

## Conclusion

For disease detection, Recall should be prioritized because identifying diseased patients is more important than avoiding false alarms.
