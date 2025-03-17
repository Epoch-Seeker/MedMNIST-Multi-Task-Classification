# 🔥 Multi-Task MedMNIST with PyTorch

## 📌 Overview
This repository contains the implementation of **Multi-Task MedMNIST** using **PyTorch** to maximize the **F1-score**. The project is part of the **Tensor Reloaded: Multi-Task MedMNIST competition**.

## 📂 Dataset
The dataset used in this project is **MedMNIST**, which consists of multiple medical image classification tasks.

### 📥 Download Dataset
You can manually download the dataset from:
- [MedMNIST Dataset](https://www.kaggle.com/competitions/tensor-reloaded-multi-task-med-mnist/data)

Or use the following Python script to download it automatically:
```python
import os
import urllib.request

dataset_url = "kaggle competitions download -c tensor-reloaded-multi-task-med-mnist"
dataset_path = "data/medmnist.zip"

os.makedirs("data", exist_ok=True)
urllib.request.urlretrieve(dataset_url, dataset_path)
print("Dataset downloaded successfully!")
```

## 🚀 Installation
### **Requirements**
Make sure you have the following dependencies installed:
```bash
pip install torch torchvision 
pip install numpy pandas tqdm scikit-learn matplotlib
```

Alternatively, install all dependencies using:
```bash
pip install -r requirements.txt
```

## 🏗️ Project Structure
```
.
├── code.ipynb  # Jupyter Notebook with full pipeline (data preprocessing, training, evaluation)
├── requirements.txt         # Dependencies
├── README.md                # Project documentation
```

## 🎯 Objective
The goal is to **maximize the F1-score** on multiple tasks using deep learning techniques.

## 🏋️‍♂️ Training
To train the model, run:
```bash
python src/train.py --epochs 20 --batch_size 256 --lr 0.001
```

## 📊 Evaluation
To evaluate the model on test data:
```bash
python src/evaluate.py --checkpoint models/best_model.pth
```

## ✨ Results
- The model achieves an **F1-score of 70.01**.
- Performance is benchmarked using the **MedMNIST** dataset.

## 🤝 Contributors
- [Sunny Kumar](https://github.com/Epoch-Seeker)
- [Thefcraft](https://github.com/thefcraft)

## 📜 License
This project is licensed under the **MIT License**.


