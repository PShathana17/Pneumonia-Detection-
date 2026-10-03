# Pneumonia Detection Using CNN

## Project Overview

This project uses **Deep Learning and Convolutional Neural Networks (CNNs)** to classify chest X-ray images into two categories:

* NORMAL
* PNEUMONIA

The main goal of the project is to build and compare different deep learning models and select the model that performs best on the given dataset.

## Dataset

The project uses the **Chest X-Ray Images (Pneumonia)** dataset.

The dataset contains chest X-ray images belonging to:

```text
NORMAL
PNEUMONIA
```

The images are divided into training, validation, and testing sets.

## What We Did in This Project

###  Loaded the Dataset

Loaded the chest X-ray images from the dataset and organized them into training, validation, and test sets.

###  Image Preprocessing

Prepared the images for CNN training by:

* Resizing the images to a fixed size.
* Normalizing pixel values.
* Loading images in batches.


###  Handled Class Imbalance

The training dataset contained more **PNEUMONIA** images than **NORMAL** images.

To handle this imbalance, **balanced class weights** were calculated using Scikit-learn and provided during model training.

This gives more importance to the minority class without changing the actual dataset.

###  Built Three Models

Three different models were trained and compared:

**Basic CNN**
A CNN model built using Keras to learn features directly from the X-ray images.

**Improved CNN**
A more complex CNN architecture was tested to determine whether additional layers could improve performance.

**MobileNetV2**
A pretrained MobileNetV2 model was used with transfer learning.

###  Evaluated the Models

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

These metrics were used to understand how well the models classified NORMAL and PNEUMONIA images.

## Model Results

| Model        | Test Accuracy |
| ------------ | ------------: |
| Basic CNN    |    **84.56%** |
| Improved CNN |        54.83% |
| MobileNetV2  |        82.24% |

The **Basic CNN achieved the highest test accuracy** among the three models.

### Final Model Performance

For the Basic CNN:

* **Test Accuracy:** 84.56%
* **Pneumonia Precision:** 81%
* **Pneumonia Recall:** 95%
* **Pneumonia F1-score:** 87%

The confusion matrix was:

```text
[[169  65]
 [ 15 269]]
```

This shows that the model correctly classified **269 Pneumonia images** and **169 Normal images** in the test set.

## Final Model

Based on the experimental results, the **Basic CNN** was selected as the final model.

The trained model was saved as:

```text
pneumonia_model.keras
```

This saved model can be used later to predict whether a new chest X-ray image belongs to the NORMAL or PNEUMONIA class.

## Technologies Used

* Python
* TensorFlow
* Keras
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook / Google Colab

## Project Workflow

```text
Chest X-ray Dataset
        ↓
Data Loading
        ↓
Image Preprocessing
        ↓
Data Augmentation
        ↓
Class Weight Handling
        ↓
Train Three Models
        ↓
Evaluate Models
        ↓
Compare Results
        ↓
Select Basic CNN
        ↓
Save Final Model
```

Conclusion

This project demonstrates an end-to-end CNN-based image classification workflow for pneumonia detection. The project covers image preprocessing, data augmentation, class imbalance handling, CNN model development, transfer learning, model comparison, and performance evaluation.

Among the three evaluated models, the Basic CNN achieved the best test accuracy of 84.56% with 95% recall for Pneumonia, so it was selected as the final model.
