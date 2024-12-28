# Pneumonia Detection with Explainable AI

This project focuses on developing a deep learning framework for pneumonia detection in chest X-ray images with an emphasis on explainable AI to ensure transparency and trustworthiness of predictions.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Usage](#usage)
5. [Contributing](#contributing)
6. [License](#license)

---

## Introduction

Pneumonia remains a critical global health issue, particularly in low-resource settings. Fast and accurate diagnosis is essential, but manual methods are prone to errors due to human limitations. This project aims to address these challenges by:
- Developing deep learning models for pneumonia detection.
- Integrating explainability techniques like Grad-CAM and SHAP for model transparency.

By prioritizing interpretability, the system seeks to assist healthcare professionals in verifying predictions, bridging the gap between AI and clinical trust.

---

## Dataset

The project uses publicly available chest X-ray datasets, including:
- NIH Chest X-Ray Dataset
- Kaggle repositories

### Preprocessing Steps:
- Removal of duplicate and incomplete entries.
- Resizing and normalization of images.
- Data augmentation techniques such as rotation, flipping, and cropping.

All data processing complies with ethical guidelines, including anonymization and KVKK compliance.

---

## Methodology

### Models
This project uses various Convolutional Neural Network (CNN) architectures:
- **ResNet Family**: Robust for deep feature extraction.
- **VGG-16**: Effective for hierarchical feature extraction.
- **EfficientNet Family**: Balances accuracy and computational efficiency.
- **Custom CNN**: Lightweight baseline for experimentation.

> **Note**: U-Net architecture mentioned in the initial proposal is **not used** in this project.

### Explainability
Explainability techniques include:
- **Grad-CAM**: Visualizing regions contributing to predictions.
- **SHAP**: Quantifying feature importance.

### Training
- Implemented with PyTorch.
- Binary cross-entropy loss with SGD/Adam optimizers.
- Hyperparameter tuning for optimal performance.
- Evaluation metrics: Accuracy, Precision, Recall, F1-Score, and interpretability fidelity.

---

## Usage

### Requirements
- Python >= 3.8
- PyTorch >= 1.9.0
- Required libraries: NumPy, Matplotlib, OpenCV, etc.

### Steps to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/pneumonia-ai.git
