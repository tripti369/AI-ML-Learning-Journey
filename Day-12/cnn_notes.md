# Day 12 - Convolutional Neural Networks (CNN)

## Why can't a Regular Neural Network Process Images Efficiently?

A traditional Neural Network (MLP) treats every pixel as an independent input. Images usually contain thousands or millions of pixels, resulting in:
- Huge number of parameters
- High memory usage
- Longer training time
- Loss of spatial relationships between pixels
- Higher risk of overfitting

CNN solves these problems by learning local image features.

---

# What is a CNN?

A Convolutional Neural Network (CNN) is a deep learning model specially designed for image processing. Instead of looking at the whole image at once, CNN scans small regions of the image and learns important patterns such as edges, textures, and shapes.

---

# Pixels and Image Representation

A digital image is made of pixels.

- Grayscale image: One value per pixel (0–255)
- RGB image: Three values per pixel (Red, Green, Blue)

Example:
Image Size = 32 × 32 × 3

---

# Convolution

Convolution is the process of sliding a small filter across an image to detect useful features.

The output of convolution is called a Feature Map.

---

# Filter (Kernel)

A Filter is a small matrix (usually 3×3 or 5×5).

Different filters learn different features:
- Vertical edges
- Horizontal edges
- Curves
- Corners
- Textures

The filter values are automatically learned during training.

---

# Feature Maps

Feature Maps are the outputs generated after applying filters.

They highlight important image patterns while ignoring unnecessary information.

---

# Stride

Stride is the number of pixels the filter moves after each step.

Stride = 1
- More detailed output
- Higher computation

Stride = 2
- Smaller output
- Faster computation

---

# Padding

Padding means adding extra pixels (usually zeros) around the image border.

Benefits:
- Preserves image size
- Helps detect features near edges
- Prevents information loss

---

# Pooling Layer

Pooling reduces image dimensions while keeping important information.

Benefits:
- Reduces computation
- Prevents overfitting
- Makes the model faster

## Max Pooling

Selects the maximum value from each region.

Most commonly used.

## Average Pooling

Calculates the average value of each region.

Produces smoother outputs.

---

# Flatten Layer

Converts the 2D feature maps into a 1D vector before classification.

Example:

8 × 8 × 64

↓

4096 neurons

---

# Fully Connected Layer

Acts like a traditional neural network.

Uses extracted features to classify the image.

Example:
Dog
Cat
Car
Person

---

# Real-world Applications of CNN

- Face Recognition
- Medical Image Diagnosis
- Self-driving Cars
- Traffic Sign Detection
- OCR
- Satellite Image Analysis
- Security Surveillance
- Object Detection
- Image Classification

---

# CNN Architecture

Input Image

↓

Convolution Layer

↓

ReLU Activation

↓

Pooling Layer

↓

Repeat Convolution + Pooling

↓

Flatten

↓

Fully Connected Layer

↓

Prediction
