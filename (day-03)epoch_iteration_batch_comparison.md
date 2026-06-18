# Epoch vs Iteration vs Batch Size

These three terms are closely related and are used during the training of a Machine Learning model.

## 1. Epoch

An Epoch means one complete pass of the entire dataset through the model.

Example:
If a dataset contains 1000 records and the model processes all 1000 records once, then 1 Epoch is completed.

Key Points:

* Uses the complete dataset once.
* Represents one learning cycle.
* Multiple epochs help the model learn better.
* More epochs usually reduce error (up to a limit).

---

## 2. Iteration

An Iteration is one update of the model after processing a batch of data.

Example:
If the dataset has 1000 records and the batch size is 100, then the model will perform 10 iterations to complete 1 epoch.

Key Points:

* One iteration processes one batch.
* Model weights are updated after every iteration.
* Number of iterations depends on batch size.
* More iterations mean more learning updates.

---

## 3. Batch Size

Batch Size is the number of training samples processed at one time before updating the model.

Example:
If the dataset contains 1000 records and batch size is 100, then the model will process 100 records at a time.

Key Points:

* Decided by the user.
* Affects training speed.
* Larger batch sizes require more memory.
* Smaller batch sizes lead to more iterations.

---

## Relationship Between Epoch, Iteration, and Batch Size

Suppose:

Dataset Size = 1000 records

Batch Size = 100

Epochs = 5

Calculations:

Iterations per Epoch = Dataset Size ÷ Batch Size

Iterations per Epoch = 1000 ÷ 100 = 10

Total Iterations = Epochs × Iterations per Epoch

Total Iterations = 5 × 10 = 50

Therefore:

* 1 Epoch = Complete dataset processed once
* 1 Iteration = One batch processed
* Batch Size = Number of samples in one batch

### Simple Formula

Iterations = Dataset Size ÷ Batch Size

Total Iterations = Epochs × Iterations per Epoch

### Quick Summary

Epoch → Complete pass through dataset

Iteration → One batch processed and model updated

Batch Size → Number of samples processed in one batch
