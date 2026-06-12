# Crop-Health
# Paddy Disease Classification using Transfer Learning and 5-Fold Cross Validation

## Project Overview

This project implements a deep learning-based system for automatic paddy leaf disease classification using Transfer Learning with ResNet18 and Stratified 5-Fold Cross Validation.

The objective is to classify paddy leaf images into 10 categories consisting of healthy and diseased plants.

---

## Dataset

**Paddy Disease Classification Dataset**

Total Images: **10,407**

Number of Classes: **10**

Classes:

* bacterial_leaf_blight
* bacterial_leaf_streak
* bacterial_panicle_blight
* blast
* brown_spot
* dead_heart
* downy_mildew
* hispa
* normal
* tungro

---

## Methodology

### Data Preprocessing

* Dataset verification
* RGB image validation
* Image resizing to 224 × 224
* Data augmentation

  * Random Horizontal Flip
  * Random Rotation
* Stratified 5-Fold Cross Validation

### Model

* Transfer Learning using ResNet18
* Pretrained ImageNet weights
* CrossEntropyLoss
* Adam Optimizer
* Learning Rate = 0.0001

### Evaluation Metrics

* Validation Accuracy
* Classification Report
* Confusion Matrix
* Fold-wise Accuracy Analysis

---

## Results

### Fold-wise Accuracy

| Fold | Accuracy (%) |
| ---- | ------------ |
| 0    | 90.00        |
| 1    | 83.48        |
| 2    | 80.87        |
| 3    | 84.14        |
| 4    | 82.94        |

### Average Cross-Validation Accuracy

**84.29%**

### Best Validation Accuracy

**90.00%**

---

## Repository Structure

```text
paddy-disease-classification/
│
├── notebooks/
│   └── paddy_disease_training.ipynb
│
├── models/
│
├── results/
│   ├── confusion_matrix.png
│   ├── accuracy_curve.png
│   ├── fold_accuracy.png
│   └── fold_results.csv
│
├── README.md
└── requirements.txt
```

---

## Generated Outputs

* Trained Model
* Confusion Matrix
* Classification Report
* Accuracy Curve
* Fold Accuracy Plot
* Cross-Validation Results

---

## Technologies Used

* Python
* PyTorch
* TIMM
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* PIL

---

## Future Improvements

* ConvNeXt / EfficientNet based architectures
* Hyperparameter tuning
* Advanced augmentation techniques
* Ensemble learning approaches

---

## Author

Implementation of Paddy Disease Classification using Deep Learning and Transfer Learning with Stratified 5-Fold Cross Validation.
