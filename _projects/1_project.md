---
layout: page
title: Gradient-Based Learning Applied to Document Recognition
description: "Implementation of a Convolutional Neural Network (LeNet architecture) for text analysis."
img: assets/img/thumb_lenet.png
importance: 8
category: deep-learning
tags: [Deep-Learning, CNN, Python, Computer-Vision, Neural-Networks]
keywords: LeNet, Convolutional Neural Network, Document Recognition, Deep Learning, Statistical Methods in AI, PyTorch, Handwriting Recognition
---

In the domain of Computer Vision, recognizing structured patterns within unstructured text images is a classic problem. For the course *Statistical Methods in AI*, I implemented a **Gradient-Based Learning** model focused on Document Recognition, heavily inspired by the foundational LeNet architecture.

### Model Architecture & Training

Building a robust Convolutional Neural Network (CNN) requires careful tuning of hyperparameters and network depth:

- **Feature Extraction**: Developed multi-layered convolutional layers using **Python** to extract hierarchical features—edges, curves, and advanced geometries—from raw handwritten document datasets. Subsampling (pooling) algorithms were integrated to ensure translational invariance.
- **Gradient Descent Optimization**: Formulated the backpropagation routines to iteratively minimize the loss function via Stochastic Gradient Descent. 
- **Performance Evaluation**: The fully connected layers were trained to classify individual alphanumeric characters, demonstrating high predictive accuracy. The project successfully bridged the gap between theoretical deep learning mathematics and functional software implementations capable of high-fidelity document analysis.