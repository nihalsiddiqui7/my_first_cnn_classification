# 😄 Emotion Classification using CNN  
A deep learning model built with **TensorFlow and Keras** to classify human emotions (Happy vs Sad) from images.  

---  

---

## 🧠 Overview  
This project implements a **Convolutional Neural Network (CNN)** to detect emotions from facial expressions.  
The dataset is preprocessed, cleaned, and normalized for efficient training, and the model achieves solid accuracy with early stopping and dropout regularization.  

---

## ✨ Features  
- 🧹 **Automated data cleaning** to remove invalid or corrupted images  
- ⚙️ **Custom CNN architecture** for binary emotion detection  
- 🔄 **Early stopping** to prevent overfitting  
- 🧠 **Trained on 256×256 RGB images** with normalization  
- 💾 Model saved as `emotion_cnn_model.h5` for reuse or deployment  

---

## 🧩 Tech Stack  
- **Python** 🐍  
- **TensorFlow / Keras**  
- **NumPy, OpenCV, Matplotlib**  
- **Google Colab / Jupyter Notebook**  

---

## 🧰 Model Architecture  
| Layer | Type | Filters/Units | Activation |  
|-------|------|---------------|-------------|  
| 1 | Conv2D | 16 | ReLU |  
| 2 | MaxPooling2D | - | - |  
| 3 | Conv2D | 32 | ReLU |  
| 4 | MaxPooling2D | - | - |  
| 5 | Conv2D | 16 | ReLU |  
| 6 | Flatten | - | - |  
| 7 | Dense | 256 | ReLU |  
| 8 | Dense | 1 | Sigmoid |  

---

## 📊 Training Details  
- **Optimizer:** Adam  
- **Loss Function:** Binary Cross-Entropy  
- **Metrics:** Accuracy  
- **Epochs:** 30 (with EarlyStopping)  
- **Validation Split:** 20%  

---


