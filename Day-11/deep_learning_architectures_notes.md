# Deep Learning Architectures – Notes

## What is a Deep Learning Architecture?

A Deep Learning Architecture is the structure of a neural network that determines how data flows through different layers to solve a specific problem. Different architectures are designed for different types of data such as images, text, audio, and time-series data.

---

## Why Different Problems Require Different Architectures?

Different types of data contain different patterns.

* Images contain spatial information.
* Text contains sequential information.
* Audio contains temporal dependencies.
* Long documents require understanding relationships between distant words.

Therefore, different architectures are used depending on the problem.

---

# Convolutional Neural Network (CNN)

## Basic Intuition

A CNN is designed to process image data. It automatically learns important visual features such as edges, textures, shapes, and objects by applying convolution filters.

### Best For

* Image Classification
* Object Detection
* Face Recognition
* Medical Imaging

### Advantages

* Excellent at extracting image features.
* Requires fewer parameters due to weight sharing.
* High accuracy for computer vision tasks.

### Limitations

* Not suitable for sequential data.
* Cannot remember previous information.

---

# Recurrent Neural Network (RNN)

## Basic Intuition

An RNN processes sequential data one element at a time while remembering information from previous steps using hidden states.

### Best For

* Text Processing
* Speech Recognition
* Time Series Forecasting

### Advantages

* Can process sequential information.
* Maintains short-term memory.

### Limitations

* Suffers from the vanishing gradient problem.
* Struggles with long sequences.

---

# Long Short-Term Memory (LSTM)

## Why RNN Struggles with Long Sequences

RNNs gradually forget earlier information when sequences become long because of the vanishing gradient problem.

## How LSTM Solves This Problem

LSTM introduces memory cells and three gates:

* Forget Gate
* Input Gate
* Output Gate

These gates decide which information should be remembered and which should be discarded.

### Best For

* Machine Translation
* Speech Recognition
* Text Generation
* Stock Price Prediction

### Advantages

* Learns long-term dependencies.
* Better performance than RNN for long sequences.

### Limitations

* More computationally expensive.
* Slower to train.

---

# Transformer

## Basic Intuition

Transformers process the entire sequence simultaneously instead of one word at a time. They use the Attention Mechanism to identify the most important parts of the input.

### Best For

* Machine Translation
* Chatbots
* Text Summarization
* Question Answering

### Advantages

* Faster training due to parallel processing.
* Excellent at understanding long-range dependencies.
* Highly scalable.

### Limitations

* Requires large datasets.
* Computationally expensive.

---

# Attention Mechanism

Attention helps the model focus on the most relevant parts of the input while making predictions.

Example:

Sentence:
"The food was amazing but the service was terrible."

If predicting sentiment about the service, the model focuses more on the word **"terrible"**.

### Benefits

* Better context understanding.
* Improved translation quality.
* Better performance on long documents.

---

# Comparison Table

| Architecture | Best For              | Strengths                      | Limitations              | Example Applications         |
| ------------ | --------------------- | ------------------------------ | ------------------------ | ---------------------------- |
| CNN          | Images                | Excellent feature extraction   | Poor for sequential data | Face Recognition             |
| RNN          | Sequential Data       | Remembers previous inputs      | Vanishing gradient       | Language Modeling            |
| LSTM         | Long Sequences        | Long-term memory               | Slower training          | Speech Recognition           |
| Transformer  | NLP & Large Sequences | Attention, parallel processing | Expensive                | ChatGPT, Machine Translation |

---

# Reflection

## 1. Why can't CNNs be used for every problem?

CNNs are mainly designed for image data. They cannot naturally understand sequential relationships in text or speech.

## 2. Why did Transformers become more popular than RNNs?

Transformers process all input simultaneously, train faster, capture long-range dependencies better, and avoid the vanishing gradient problem.

## 3. Which architecture would you choose for image classification and why?

I would choose CNN because it automatically extracts visual features and performs exceptionally well on image classification tasks.

## 4. Which architecture interests you the most and why?

The Transformer architecture interests me the most because it powers modern AI systems such as ChatGPT and performs exceptionally well across different domains.
