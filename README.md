# Deep Fake Video Detection Using InceptionV3 and LSTM

## 📌 Project Overview
Deepfake videos pose a serious threat to the authenticity of digital media by manipulating facial expressions and motion using advanced deep learning techniques. Detecting such videos has become critical to prevent misinformation, identity misuse, and loss of trust in visual content.

This project proposes a **hybrid deep learning model combining InceptionV3 and Long Short-Term Memory (LSTM)** networks to detect deepfake videos by learning both **spatial artifacts** and **temporal inconsistencies**. The model effectively distinguishes real and manipulated videos by analyzing frame-level visual features and frame-to-frame motion patterns.

---

## 🎓 Academic Information
- **Program**: M.Sc Data Science  
- **Project Type**: PG 1-Year SET Conference Project  
- **Institution**: Vellore Institute of Technology (VIT), Vellore  

---

## 👨‍💻 Authors
- **Yokesh VP**  
  School of Advanced Sciences, VIT Vellore  

- **Subash G**  
  School of Advanced Sciences, VIT Vellore  

## 🧠 Proposed Methodology

### 🔹 System Architecture
1. Input video is decomposed into frames  
2. Face detection using **MTCNN**  
3. Spatial feature extraction using **InceptionV3 (ImageNet pretrained)**  
4. Temporal feature learning using **LSTM**  
5. Binary classification: **Real / Deepfake**

---

### 🔹 Why InceptionV3 + LSTM?
- **InceptionV3** captures spatial inconsistencies such as texture distortions, blending artifacts, and lighting irregularities.
- **LSTM** models temporal dependencies to identify unnatural facial motion, blinking, and lip-sync inconsistencies.
- The hybrid approach outperforms CNN-only models by combining spatial and temporal learning.

---

## 📊 Dataset

Due to the large size of the dataset, it is **not included** in this repository.

This project uses the **FaceForensics++ dataset**, a widely used benchmark dataset for deepfake detection research.

🔗 **Dataset Link (Kaggle):**  
https://www.kaggle.com/datasets/hungle3401/faceforensics

### Dataset Highlights
- Real and manipulated videos
- Multiple deepfake generation techniques
- Various compression levels
- Real-world benchmark dataset

⚠️ **Note:**  
Please download the dataset manually from Kaggle and place it in the appropriate directory before running the code.

---

## 📁 Expected Dataset Structure
```text
dataset/
├── real/
│   ├── video_01.mp4
│   └── video_02.mp4
├── fake/
│   ├── video_01.mp4
│   └── video_02.mp4
