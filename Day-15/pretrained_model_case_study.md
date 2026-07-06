# 🌱 Case Study – Plant Disease Detection

## 🎯 Target Problem

The goal is to identify diseases in plant leaves using images. Early detection helps farmers reduce crop damage and improve agricultural productivity.

Examples include:

- Healthy Leaf
- Tomato Blight
- Leaf Spot
- Rust Disease

---

## ❓ Why Training From Scratch Is Difficult?

Training a deep learning model from scratch requires:

- Thousands of labeled plant images
- High computational resources
- Long training time
- Expensive GPUs
- Large storage capacity

Since agricultural datasets are often small, training from scratch may lead to poor performance and overfitting.

---

## 🤖 Pretrained Model

**EfficientNet-B0**

EfficientNet is a powerful convolutional neural network that provides excellent accuracy while using fewer parameters than many traditional CNN architectures.

---

## ⚙️ Selected Approach

### Fine-Tuning

Fine-Tuning is chosen because plant diseases often have subtle visual differences such as tiny spots, discoloration, and texture variations. Updating pretrained layers helps the model learn these domain-specific features more effectively.

---

# 💭 Reflection

## Why are pretrained models valuable?

Pretrained models have already learned useful features from large datasets, making it easier to build accurate AI models with less data and training time.

---

## In what situations would you avoid training a model from scratch?

I would avoid training from scratch when the dataset is small, computational resources are limited, or a suitable pretrained model is already available.

---

## How does Transfer Learning save time and resources?

Transfer Learning reuses previously learned knowledge instead of starting from zero. This reduces training time, computational cost, and the amount of labeled data required.

---

## Which application impressed you the most and why?

Brain Tumor Classification impressed me the most because Transfer Learning helps build accurate medical diagnosis systems even with limited medical imaging data, supporting doctors in early disease detection.

---

# 🔬 Mini Research – ResNet

## What task was it originally trained for?

ResNet was originally trained for image classification on the ImageNet dataset, which contains over one million images across 1,000 categories.

---

## What makes it popular?

- Introduced Residual (Skip) Connections
- Solves the Vanishing Gradient Problem
- Supports very deep neural networks
- High image classification accuracy
- Widely used in computer vision applications

---

## Real-World Application

ResNet is widely used in medical image analysis, including disease detection from X-rays, MRI scans, and CT scans. It is also used in autonomous vehicles, face recognition systems, and industrial quality inspection.

---

# ✅ Conclusion

Transfer Learning enables developers to build high-performing AI models efficiently by adapting pretrained models to new tasks. It reduces computational cost, saves time, and delivers excellent performance even when only limited labeled data is available.
