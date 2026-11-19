# Project Reference – Sea Creatures Image Classification

## 1. Project Overview
- **Project name:** Sea Creatures Image Classification
- **Course:** WorldQuant University – AI Lab: Deep Learning for Computer Vision
- **Project type:** Deep Learning / Computer Vision
- **Objective:** Build an image classification model that identifies different types of sea creatures from images.
- **Programming language:** Python
- **Framework:** PyTorch
- **Libraries:** Torchvision, NumPy, Scikit-learn

## 2. Dataset Information
- Total images: **6,182**
- Training images: **4,946**
- Validation images: **1,236**
- Number of classes: **9**

### Classification categories
1. Dolphin
2. Jelly Fish
3. Octopus
4. Puffers
5. Sea Rays
6. Sea Urchins
7. Sharks
8. Turtle_Tortoise
9. Whale

## 3. Data Preprocessing
- Converted images to RGB format.
- Resized images to **224 × 224 pixels**.
- Converted images into tensors using PyTorch transforms.
- Calculated dataset-specific mean and standard deviation.
- Applied image normalization.
- Split the dataset into 80% training and 20% validation.
- Used PyTorch DataLoaders with a batch size of 32.

## 4. Model Architecture
Developed a custom Convolutional Neural Network (CNN).

Architecture:
- 3 convolutional layers.
- Convolutional filters: 16, 32, and 64.
- ReLU activation functions.
- Max pooling layers.
- Dropout regularization.
- Flatten layer.
- Fully connected hidden layer with 500 units.
- Output layer with 9 classes.
- Approximately **316,593 trainable parameters**.

## 5. Model Training and Evaluation

### Actual results
- Training accuracy: **67.08%**
- Validation accuracy: **63.75%**
- Training loss: **0.9328**
- Validation loss: **1.0592**
- Weighted precision: **0.63**
- Weighted recall: **0.64**
- Weighted F1-score: **0.63**
- Macro F1-score: **0.57**

### Best-performing categories (F1-score)
- Turtle/Tortoise: 0.82
- Sea Urchins: 0.81
- Jelly Fish: 0.80

### Categories needing improvement
- Sea Rays: 0.23
- Puffers: 0.43
- Sharks: 0.43

Evaluation techniques:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Training and validation loss



