# Pneumonia Detection with Explainable AI

This project focuses on developing a deep learning framework for pneumonia detection in chest X-ray images, with an emphasis on explainable AI to ensure transparency and trustworthiness of predictions. A custom, ethically-compliant dataset has been created specifically for this purpose, adhering to KVKK regulations.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Explainability Techniques](#explainability-techniques)
5. [Usage](#usage)
6. [Results and Evaluation](#results-and-evaluation)
7. [Contributing](#contributing)
8. [License](#license)

---

## Introduction

Pneumonia remains a critical global health issue, particularly in low-resource settings. Accurate and timely diagnosis is essential, but manual interpretation of chest X-rays can lead to errors due to human limitations, such as fatigue or limited expertise.

This project addresses these challenges by:
- Developing robust deep learning models for pneumonia detection.
- Integrating explainability techniques (e.g., Grad-CAM, SHAP) to provide insights into model decisions.

By ensuring interpretability, this system aims to bridge the gap between artificial intelligence and clinical trust, fostering human-AI partnerships in healthcare.

---

## Dataset

### Overview
A custom dataset of chest X-ray images was curated for this project. This dataset was ethically compiled and complies with KVKK guidelines to ensure privacy and security.

### Data Collection Process
1. **Source Images**:
   - Public datasets (e.g., NIH Chest X-Ray Dataset, Kaggle repositories).
   - Additional images collected in compliance with KVKK regulations.
2. **Preprocessing**:
   - Removed duplicate and incomplete entries.
   - Standardized resolution and normalized pixel intensities.
   - Augmentation techniques applied (rotation, flipping, cropping, etc.) to increase robustness.
3. **Ethical Compliance**:
   - Personally identifiable information was anonymized.
   - Metadata (e.g., demographics) was scrubbed for transparency and privacy.

### Key Features
- High diversity in patient demographics and imaging conditions.
- Extensive augmentation to improve model generalization.
- Fully KVKK-compliant.

---

## Methodology

### Models
The project employs the following CNN architectures:
- **ResNet Family**: Effective for deep feature extraction and reducing vanishing gradient issues.
- **VGG-16**: Simplified architecture for hierarchical feature learning.
- **EfficientNet Family**: Optimized for balancing accuracy and computational efficiency.
- **Custom CNN**: Lightweight baseline for rapid prototyping and experimentation.

### Training Strategy
1. **Framework**: Implemented in PyTorch.
2. **Optimization**:
   - Binary cross-entropy loss function.
   - Stochastic Gradient Descent (SGD) and Adam optimizers.
3. **Hyperparameter Tuning**:
   - Experimented with various learning rates and batch sizes.
   - Early stopping and learning rate schedulers to prevent overfitting.
4. **Evaluation Metrics**:
   - Classification: Accuracy, Precision, Recall, F1-Score.
   - Explainability: Fidelity, interpretability scores.

---

## Explainability Techniques

### Grad-CAM
- Visualizes the regions of chest X-ray images most influential in the model's predictions.
- Provides intuitive insights into model behavior, enhancing transparency for medical professionals.

### SHAP (SHapley Additive exPlanations)
- Quantifies the contribution of each feature to the model's decision.
- Helps identify potential biases or anomalies in predictions.

---

## Usage

### Prerequisites
- Python >= 3.8
- PyTorch >= 1.9.0
- Required libraries: NumPy, Matplotlib, OpenCV, SHAP, etc.
