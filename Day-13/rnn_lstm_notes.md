# Day 13 - Recurrent Neural Networks (RNNs) & LSTMs

## Objective

Understand how neural networks process sequential data and why LSTMs are better than traditional RNNs for long sequences.

---

# What is Sequential Data?

Sequential data is data where the order of elements matters. Changing the order changes the meaning or pattern.

### Examples
- Text
- Speech
- Time Series Data
- Weather Forecasting
- Stock Prices
- Music
- Video Frames

---

# Why Can't Traditional Neural Networks Handle Sequential Data?

Traditional Neural Networks assume that every input is independent. They cannot remember previous inputs, making them unsuitable for sequence-based tasks.

Example:

"I love AI"

AI love I

The order changes the meaning completely.

---

# What is an RNN?

A Recurrent Neural Network (RNN) is a neural network designed for sequential data. It processes one input at a time while remembering information from previous inputs through a hidden state.

---

# Hidden State

The hidden state is the memory of an RNN. It stores useful information from previous time steps and passes it to the next step.

Current Input + Previous Hidden State → Updated Hidden State

---

# Limitations of RNN

- Cannot remember long-term information effectively.
- Suffers from the Vanishing Gradient Problem.
- Performance decreases for long sequences.
- Training becomes difficult for lengthy inputs.

---

# Vanishing Gradient Problem

During training, gradients become extremely small while backpropagating through many time steps.

As a result:
- Earlier information is forgotten.
- Learning long-term dependencies becomes difficult.

---

# What is LSTM?

Long Short-Term Memory (LSTM) is an improved version of RNN that can remember important information for longer periods.

It uses three gates:
- Forget Gate
- Input Gate
- Output Gate

These gates decide what information should be forgotten, stored, and passed forward.

---

# Advantages of LSTM

- Handles long-term dependencies
- Reduces vanishing gradient problem
- Better accuracy
- Suitable for long text and speech sequences
- Widely used in NLP and time-series forecasting

---

# What is GRU?

Gated Recurrent Unit (GRU) is another improved version of RNN.

Features:
- Two gates (Update Gate and Reset Gate)
- Simpler architecture
- Faster training
- Uses less memory than LSTM

---

# Applications of RNNs and LSTMs

- Sentiment Analysis
- Machine Translation
- Speech Recognition
- Chatbots
- Next Word Prediction
- Weather Forecasting
- Stock Price Prediction
- Healthcare Monitoring

---

# Key Takeaways

- Sequential data depends on order.
- RNN remembers previous information using hidden states.
- RNN struggles with long sequences.
- LSTM solves this using memory gates.
- GRU is a lightweight alternative to LSTM.
