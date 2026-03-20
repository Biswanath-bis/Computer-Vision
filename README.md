# 🧠 CIFAR-10 Image Classification using CNN (PyTorch)

## 📌 Overview
This project implements a Convolutional Neural Network (CNN) using PyTorch to classify images from the CIFAR-10 dataset into 10 categories. The model achieves **74.71% accuracy** on the test dataset.

## 📂 Dataset
- CIFAR-10 (60,000 images: 50,000 train, 10,000 test)
- 10 classes: Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck
- Image size: 32x32 (RGB)

## ⚙️ Tech Stack
- Python  
- PyTorch  
- Torchvision  

## 🏗️ Model Architecture
- Conv2D (3 → 32) → ReLU → MaxPool  
- Conv2D (32 → 64) → ReLU → MaxPool  
- Conv2D (64 → 128) → ReLU → MaxPool  
- Flatten  
- Linear (2048 → 256) → ReLU  
- Linear (256 → 10)

## 🔄 Preprocessing
- Converted images to tensors  
- Normalized using mean = (0.5, 0.5, 0.5), std = (0.5, 0.5, 0.5)

## 🚀 Training
- Loss: CrossEntropyLoss  
- Optimizer: Adam  
- Batch Size: 64  
- Epochs: 10  

## 📉 Training Loss
Epoch 1: 0.755  
Epoch 2: 0.632  
Epoch 3: 0.529  
Epoch 4: 0.428  
Epoch 5: 0.346  
Epoch 6: 0.279  
Epoch 7: 0.211  
Epoch 8: 0.172  
Epoch 9: 0.135  
Epoch 10: 0.113  

## 📊 Results
- Test Accuracy: **74.71%**

📈 Future Improvements
-Add Dropout
-Data Augmentation
-Use pre-trained models (ResNet, VGG)
-Hyperparameter tuning
