# MedMNIST-Multi-Task-Classification
Multi-Task MedMNIST competition, focusing on multi-task biomedical image classification using the MedMNIST2D dataset. The goal is to develop a model that generalizes across 11 medical imaging tasks, evaluated using the harmonic mean of macro F1 scores.

# Tensor Reloaded: Multi-Task MedMNIST 🏥🔬  

This repository contains our solution for the **Tensor Reloaded: Multi-Task MedMNIST** competition. Our goal is to develop a deep learning model that **maximizes the F1-score** across multiple medical image classification tasks.  

## 👥 Team  
- [**Sunny Kumar**](https://github.com/Epoch-Seeker)
- [**Thefcraft**](https://github.com/thefcraft)  

## 📌 Project Overview  
We focus on improving the **F1-score** by optimizing data preprocessing, augmentations, loss functions, and model architectures.  

## 📂 Dataset  
We use **MedMNIST**, a lightweight medical image dataset containing grayscale and color images, categorized into multiple medical classes.  

## 🛠️ Preprocessing & Transformations  
- **Normalization:** Standardizes pixel values  
- **Augmentations:** Rotation, flipping, color jitter, Gaussian blur  
- **Tensor Conversion:** Converts images to PyTorch tensors  

## 🏗️ Model Architecture  
- **CNN backbone** with **skip connections**  
- Adaptive pooling for dynamic feature extraction  
- Fully connected layers with **dropout** for regularization  
- **F1-score aware loss function** for optimization  

## 🚀 Training Pipeline  
- **Objective:** Maximize F1-score  
- **Optimizer:** Adam  
- **Loss Function:** Weighted F1-loss (custom loss function)  
- **Batch Size:** 256  
- **Learning Rate Scheduling:** Cosine annealing for better convergence  

## 📊 Results & Performance  
Our experiments focus on **improving F1-score** rather than just accuracy. We test multiple architectures and fine-tune hyperparameters to achieve optimal performance.  

## 🛠️ Setup & Usage  
**Install Dependencies:**  
```bash
pip install -r requirements.txt
