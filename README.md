# Pneumonia Detection Using CNN and Deep Learning

## Project Overview

This project presents a **Deep Learning-based Pneumonia Detection System** that classifies chest X-ray images as **Normal** or **Pneumonia**. The model is developed using **Convolutional Neural Networks (CNN)** and also explores **Transfer Learning with MobileNetV2** to improve classification performance.

The objective is to assist healthcare professionals by providing a fast and automated method for detecting pneumonia from chest X-ray images.

---

## Objectives

* Detect pneumonia from chest X-ray images.
* Build a CNN model for binary image classification.
* Improve performance using MobileNetV2 transfer learning.
* Evaluate the model using standard classification metrics.
* Predict pneumonia from new chest X-ray images.

---

##  Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* Google Colab
* CNN (Convolutional Neural Network)
* MobileNetV2 (Transfer Learning)

---

##  Dataset

The project uses a **Chest X-ray Image Dataset** containing two classes:

* **NORMAL**
* **PNEUMONIA**

The dataset is divided into:

* Training Set
* Validation Set
* Test Set

Each image is resized to **224 × 224 pixels** before training.

---

## ⚙️ Project Workflow

1. Load the chest X-ray dataset.
2. Preprocess and normalize images.
3. Perform data augmentation using `ImageDataGenerator`.
4. Build a CNN model.
5. Train the CNN model.
6. Build a MobileNetV2 transfer learning model.
7. Evaluate model performance.
8. Save the trained model.
9. Predict pneumonia from new chest X-ray images.

---

##  CNN Architecture

The custom CNN model consists of:

* Conv2D (32 filters)
* MaxPooling2D
* Conv2D (64 filters)
* MaxPooling2D
* Conv2D (128 filters)
* MaxPooling2D
* Flatten Layer
* Dense Layer (128 neurons)
* Dropout (0.5)
* Output Layer (Sigmoid)

---

##  Transfer Learning

To improve performance, the project also uses **MobileNetV2** with ImageNet pretrained weights.

Features include:

* Pretrained MobileNetV2 backbone
* Frozen convolutional layers
* Global Average Pooling
* Dropout Layer
* Sigmoid output layer for binary classification

---

##  Model Evaluation

The model is evaluated using:

* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss
* Test Prediction

---

##  Prediction

The trained model can classify a new chest X-ray image as:

*  NORMAL
*  PNEUMONIA

It also displays the prediction confidence score.

---
##  Acknowledgements

* TensorFlow & Keras
* Google Colab
* Chest X-ray dataset contributors
* Open-source Deep Learning community
