# Bridging Silence: A CNN-Based Approach to Sign Language Recognition

This repository contains the code and resources for the **"Bridging Silence: A CNN-Based Approach to Static Sign Language Recognition"** project, developed as part of the YZV303(2)E/BLG561E Deep Learning course at Istanbul Technical University (ITU). The project aligns with ITU's 251st anniversary vision by contributing to an inclusive campus experience through advanced deep learning techniques.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Model Architecture](#model-architecture)
4. [Training and Evaluation](#training-and-evaluation)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Acknowledgements](#acknowledgements)

---

## Project Overview
The aim of this project is to develop a robust deep learning framework to recognize and classify static hand gestures in sign language. By leveraging Convolutional Neural Networks (CNNs) and a diverse dataset, this project seeks to facilitate communication for hearing-impaired individuals.

---

## Dataset
The dataset comprises:
- Custom-collected static hand gesture images from ITU students during sign language training sessions.
- Complementary datasets sourced from public platforms such as Kaggle to ensure diversity.

### Data Processing
- Images are pre-processed through normalization and augmentation techniques like rotation, flipping, and scaling.
- KVKK compliance is ensured by excluding personal or sensitive data.

---

## Model Architecture
The project explores the following CNN architectures:
- **LeNet-5**: Lightweight, suitable for foundational image recognition.
- **AlexNet**: Deeper architecture for moderately complex datasets.
- **VGG-16**: Known for its simplicity and high accuracy.

Transfer learning is employed to enhance model performance with limited data.

---

## Training and Evaluation
### Metrics
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

### Statistical Tests
- 5x2 cross-validation
- Hyperparameter tuning for optimal performance.

---

## Installation
### Prerequisites
- Python >= 3.8
- PyTorch >= 1.10
- Other dependencies are listed in `requirements.txt`.

### Steps
1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/bridging-silence.git
    cd bridging-silence
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

---

## Usage
1. Prepare your dataset by placing images in the `data/` directory.
2. Run the training script:
    ```bash
    python train.py
    ```
3. Evaluate the model using:
    ```bash
    python evaluate.py
    ```

For more detailed instructions, refer to the documentation in the `docs/` directory.

---

## Acknowledgements
- This project was developed as part of the ITU Deep Learning course.
- Special thanks to ITU's Volunteer Club for organizing the sign language training sessions.
- Public datasets were sourced from Kaggle and similar platforms.

---

### License
This project is licensed under the MIT License. See `LICENSE` for details.
