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

## 🧰 Model Architecture & Summary 


| Layer (type)                    | Output Shape           | Param #     |
|---------------------------------|------------------------|--------------|
| **conv2d_17 (Conv2D)**          | (None, 254, 254, 16)   | 448          |
| **max_pooling2d_15 (MaxPooling2D)** | (None, 127, 127, 16)   | 0            |
| **dropout (Dropout)**           | (None, 127, 127, 16)   | 0            |
| **conv2d_18 (Conv2D)**          | (None, 125, 125, 32)   | 4,640        |
| **max_pooling2d_16 (MaxPooling2D)** | (None, 62, 62, 32)     | 0            |
| **dropout_1 (Dropout)**         | (None, 62, 62, 32)     | 0            |
| **conv2d_19 (Conv2D)**          | (None, 60, 60, 16)     | 4,624        |
| **max_pooling2d_17 (MaxPooling2D)** | (None, 30, 30, 16)     | 0            |
| **dropout_2 (Dropout)**         | (None, 30, 30, 16)     | 0            |
| **flatten_5 (Flatten)**         | (None, 14400)          | 0            |
| **dense_10 (Dense)**            | (None, 256)            | 3,686,656    |
| **dropout_3 (Dropout)**         | (None, 256)            | 0            |
| **dense_11 (Dense)**            | (None, 1)              | 257          |

**Total params:** 3,696,625  
**Trainable params:** 3,696,625  
**Non-trainable params:** 0
  

---

## 📊 Training Details  
- **Optimizer:** Adam  
- **Loss Function:** Binary Cross-Entropy  
- **Metrics:** Accuracy  
- **Epochs:** 30 (with EarlyStopping)  
- **Validation Split:** 20%  

---


