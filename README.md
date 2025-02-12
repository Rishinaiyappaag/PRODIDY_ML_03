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
**##📜 Code Overview** <BR>
**1️⃣ Extract and Preprocess Images**
Converts images to grayscale<BR>
Resizes to 64x64 pixels<BR>
Extracts HOG features<BR>
**2️⃣ Balance Dataset**<BR>
Uses RandomUnderSampler() to prevent bias<BR>
Ensures equal number of cat and dog images<BR>
**3️⃣ Normalize Features**<BR>
Applies StandardScaler() for better SVM training<BR>
**4️⃣ Train SVM Model**<BR>
Uses SVC(kernel='rbf', C=1, gamma='scale')<BR>

**5️⃣ Evaluate Model**<BR>
Prints accuracy & classification report<BR>
**6️⃣ Test on a New Image**<BR>
Loads test image<BR>
Extracts HOG features<BR>
Normalizes & predicts using the trained model<BR>
Displays test image with predicted label<BR>


