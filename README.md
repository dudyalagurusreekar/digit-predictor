# 🧠 Single Digit Predictor (CNN-Based)

This project implements a Convolutional Neural Network (CNN) model to predict a single handwritten digit (0–9) from an uploaded image file. The system processes external image inputs and returns both the predicted digit and its confidence score.

## 📌 Overview

The model was trained on digit datasets and enhanced through data augmentation and fine-tuning to improve generalization performance. Multiple trained versions are included, enabling comparison between base, augmented, and fine-tuned models.

## 🏗 Model Architecture

The CNN consists of:

- 2 Convolutional layers  
- Max pooling layers  
- 1 Fully connected hidden layer  
- Output layer with 10 classes  

Architecture:
- Conv2D (1 → 16)  
- Conv2D (16 → 32)  
- Linear (1568 → 128)  
- Linear (128 → 10)  

ReLU activation is used in hidden layers, and Softmax is applied during inference to compute class probabilities.

## ⚙️ Workflow

1. Upload an image containing a single digit.  
2. Convert image to grayscale.  
3. Resize to 28×28 pixels (MNIST format).  
4. Normalize pixel values.  
5. Pass the processed image through the trained CNN.  
6. Return predicted digit and confidence score.

## 📂 Model Files

- `digit_model.pth` – Base model  
- `digit_model_augmented.pth` – Augmented training model  
- `digit_model_finetuned.pth` – Fine-tuned model  

## 🛠 Technologies Used

- Python  
- PyTorch  
- OpenCV  
- NumPy  

## 🎯 Objective

To develop a structured, reusable single-digit recognition pipeline capable of performing reliable inference on uploaded image files while demonstrating practical deep learning deployment concepts.
