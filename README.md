# PRODIDY_ML_03
# 🐱🐶 Cat vs Dog Image Classification using SVM

This project implements an **SVM-based machine learning model** to classify images of **cats and dogs** using **HOG (Histogram of Oriented Gradients) features**. The dataset is preprocessed, balanced, and normalized for improved accuracy.

## 📌 Features
✔ **Preprocesses images using OpenCV**  
✔ **Extracts HOG features for better classification**  
✔ **Uses Support Vector Machine (SVM) with RBF kernel**  
✔ **Balances the dataset to prevent class bias**  
✔ **Displays test image along with the predicted label**  

---

## 📂 Dataset Structure
The dataset should be **inside a ZIP file** (`training_set.zip`) containing **two folders**:
<BR>
---
##**📜 Code Overview**
**1️⃣ Extract and Preprocess Images**
Converts images to grayscale
Resizes to 64x64 pixels
Extracts HOG features
**2️⃣ Balance Dataset**
Uses RandomUnderSampler() to prevent bias
Ensures equal number of cat and dog images
**3️⃣ Normalize Features**
Applies StandardScaler() for better SVM training
**4️⃣ Train SVM Model**
Uses SVC(kernel='rbf', C=1, gamma='scale')

**5️⃣ Evaluate Model**
Prints accuracy & classification report
**6️⃣ Test on a New Image**
Loads test image
Extracts HOG features
Normalizes & predicts using the trained model
Displays test image with predicted label


