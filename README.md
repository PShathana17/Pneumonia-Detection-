# Pneumonia Detection Using CNN

## Overview

A deep learning project that detects pneumonia from chest X-ray images using Convolutional Neural Networks (CNN).

The project includes image preprocessing, CNN model development, model comparison, evaluation, and prediction.

## Dataset

**Kaggle – Chest X-Ray Images (Pneumonia)**

* Normal: Chest X-ray images without pneumonia
* Pneumonia: Chest X-ray images showing pneumonia
* Images are resized and normalized before training.

## Technologies Used

* Python
* TensorFlow / Keras
* CNN
* OpenCV
* NumPy
* Matplotlib
* Scikit-learn
* Flask

## Project Workflow

```text
Chest X-ray Images
        ↓
Image Preprocessing
        ↓
Basic CNN
        ↓
Improved CNN
        ↓
MobileNetV2
        ↓
Model Evaluation & Comparison
        ↓
Basic CNN Selected
        ↓
Pneumonia Prediction
```

## Models Compared

Three deep learning approaches were evaluated:

1. Basic CNN
2. Improved CNN
3. MobileNetV2 using Transfer Learning

### Model Performance

| Model        | Test Accuracy |
| ------------ | ------------: |
| Basic CNN    |        83.78% |
| MobileNetV2  |        77.99% |
| Improved CNN |        54.83% |

The Basic CNN achieved the highest test accuracy of 83.78% among the models evaluated on this dataset. Therefore, it was selected as the final model and saved as:

```text
pneumonia_model.keras
```

## Key Features

* Chest X-ray image preprocessing
* CNN-based pneumonia classification
* Comparison of multiple deep learning models
* Model evaluation using test accuracy
* Prediction of Normal/Pneumonia images
* Flask-based prediction API

## Project Structure

```text
Pneumonia-Detection/
│
├── Pneumonia_Detection_Using_CNN.ipynb
├── pneumonia_model.keras
├── app.py
├── requirements.txt
└── README.md
```

