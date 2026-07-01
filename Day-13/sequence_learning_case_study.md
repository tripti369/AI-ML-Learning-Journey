# Case Study: Sentiment Analysis

## Problem Statement

Predict whether a movie review is Positive or Negative using an LSTM model.

---

## Input Sequence

"The movie was absolutely amazing and I loved every scene."

---

## Expected Output

Positive

---

## Why is Sequence Order Important?

The meaning of a sentence depends on the order of words.

Example:

"I do not like this movie."

The word "not" changes the sentiment completely.

Ignoring sequence order may produce incorrect predictions.

---

## Why Does LSTM Perform Better Than a Simple RNN?

LSTM remembers important words such as "not" even after several time steps.

Simple RNNs often forget earlier words due to the vanishing gradient problem.

Therefore, LSTM provides more accurate sentiment classification.

---

## Workflow

Input Review

↓

Word Embedding

↓

LSTM Processes Each Word

↓

Hidden State Updates

↓

Dense Layer

↓

Prediction (Positive / Negative)

---

## Conclusion

LSTM is more suitable than a simple RNN because it captures long-term dependencies and understands sentence context more effectively.
