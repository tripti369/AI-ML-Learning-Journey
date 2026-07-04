# Day 14 – Transformers & Attention

## Introduction

Transformers are deep learning models introduced in the paper:

> "Attention Is All You Need" (Google, 2017)

They became the foundation of modern Artificial Intelligence because they process data in parallel and understand relationships between words using Attention.

---

# Why did AI move from RNN/LSTM to Transformers?

RNN and LSTM process words one at a time.

Problems:

- Slow training
- Cannot process long sequences efficiently
- Forget older information
- Difficult to parallelize

Transformers solve these problems using Self-Attention.

---

# What is a Transformer?

A Transformer is a neural network architecture that processes all words simultaneously using the Attention Mechanism.

Main Components:

- Input Embedding
- Positional Encoding
- Encoder
- Decoder
- Self Attention
- Feed Forward Network

---

# Attention Mechanism

Attention allows the model to focus on the most relevant words while understanding a sentence.

Example:

"The cat sat on the mat because it was tired."

The word "it" refers to "cat".

Attention helps identify this relationship.

---

# Self-Attention

Self-Attention compares every word with every other word.

Each word asks:

- Which words are important?
- How important are they?

Output is a weighted representation.

---

# Encoder

Encoder understands the input.

Each encoder layer contains:

- Multi-Head Self Attention
- Feed Forward Neural Network
- Residual Connection
- Layer Normalization

The encoder creates contextual embeddings.

---

# Decoder

Decoder generates output one token at a time.

Components:

- Masked Self Attention
- Encoder-Decoder Attention
- Feed Forward Network

Used in translation and text generation.

---

# Positional Encoding

Transformers process all words simultaneously.

Therefore they don't know word order.

Positional Encoding adds position information.

Example:

"I love AI"

is different from

"AI love I"

Position vectors solve this issue.

---

# Parallel Processing

Unlike RNNs,

Transformer processes

All Words → At Once

Advantages:

- Faster Training
- Better GPU Utilization
- Easier Scaling

---

# Benefits

- Fast Training
- Handles long context
- Parallel computation
- Better accuracy
- State-of-the-art performance

---

# Limitations

- High memory usage
- Computationally expensive
- Needs large datasets
- Expensive to train

---

# Applications

- ChatGPT
- Google Translate
- BERT Search
- Code Generation
- Image Captioning
- Text Summarization
- Speech Recognition
