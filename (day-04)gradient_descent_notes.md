# Gradient Descent Notes

## What is Gradient Descent?

Gradient Descent is an optimization algorithm used in Machine Learning to reduce errors and improve model predictions.

It helps the model find the best values of parameters (weights and biases) by gradually moving towards the minimum loss.

---

## Why Do Machine Learning Models Need Optimization?

A model initially makes incorrect predictions.

Optimization helps the model:

- Reduce prediction errors
- Improve accuracy
- Learn patterns from data
- Find the best-fit solution

Without optimization, the model cannot learn effectively.

---

## Loss and Gradient Descent Relationship

Loss measures how wrong the model's predictions are.

Gradient Descent uses the loss value to determine how parameters should be adjusted.

Process:

1. Make Prediction
2. Calculate Loss
3. Calculate Gradient
4. Update Parameters
5. Make Better Prediction

The goal is to minimize the loss.

---

## What is Learning Rate?

Learning Rate is a small value that controls how much the model updates its parameters during each step.

Formula:

New Parameter = Old Parameter − Learning Rate × Gradient

---

## Learning Rate Too High

- Large parameter updates
- Faster movement
- Can overshoot the optimal solution
- Training becomes unstable
- Loss may fluctuate

---

## Learning Rate Too Low

- Very small updates
- Stable learning
- Takes longer to train
- Requires more epochs
- May get stuck before reaching the best solution

---

## Best Fit Concept

The best fit is the point where the model achieves the lowest possible loss and makes accurate predictions.

Gradient Descent helps the model move toward this best-fit solution.

---

## Why Multiple Epochs Are Required

One epoch means one complete pass through the dataset.

A model cannot learn everything in one pass because:

- Initial predictions are inaccurate
- Parameters need repeated adjustment
- Learning happens gradually
- Error decreases step by step

Multiple epochs help achieve better performance.

---

## Importance of Optimization

Optimization is important because it:

- Improves model accuracy
- Reduces prediction errors
- Helps the model learn efficiently
- Finds the best parameter values
- Produces reliable predictions

---

## Simple Definition

Gradient Descent is a method that helps Machine Learning models learn from mistakes by gradually reducing errors and improving predictions.
