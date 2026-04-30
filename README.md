# 🌿 Plant Disease Severity Estimation using Deep Learning

## 📌 Overview
This project focuses on **Plant Disease Severity Estimation** using deep learning techniques. Unlike traditional plant disease detection systems that classify images as healthy or diseased, this work goes a step further by estimating the **degree of infection (severity level)** in plant leaves.

The study combines both **classification-based** and **segmentation-based** approaches using deep learning models such as CNNs and semantic segmentation networks.

---

## 🎯 Objectives
- To analyze plant disease severity rather than simple detection.
- To compare different deep learning models for classification and segmentation.
- To estimate disease severity as both **discrete classes** and **continuous values (PDI)**.
- To evaluate model performance on real-world agricultural datasets.

---

## 🧠 Techniques Used

### 🔹 Classification Models
- ResNet50
- MobileNetV2

### 🔹 Segmentation Models
- U-Net
- PSPNet (ResNet50 encoder)

### 🔹 Data Processing
- Image resizing (224 × 224)
- HSV color transformation
- Leaf region extraction using thresholding
- Data augmentation (rotation, flipping, scaling, mix-up, DCT)

---

## 📊 Dataset
- Coffee Leaf Biotic Stress Dataset
- 1685 images for classification
- 500 images with pixel-level masks for segmentation
- Severity labels:
  - Healthy
  - Very Low
  - Low
  - High
  - Very High

---

## ⚙️ Methodology
1. Image preprocessing and leaf region extraction  
2. Data augmentation for better generalization  
3. Classification using CNN models (ResNet50, MobileNetV2)  
4. Segmentation using U-Net and PSPNet  
5. Severity estimation using:
   - Classification output (discrete levels)
   - Segmentation output (percentage infected area)

---

## 📈 Results

### 🔹 Classification Performance
- MobileNetV2 Accuracy: **85.71%**
- ResNet50 Accuracy: **84.13%**

### 🔹 Segmentation Performance
- U-Net Accuracy: **99.04%**
- PSPNet Accuracy: **98.76%**

---

## 🚧 Key Challenges
- Limited availability of annotated datasets  
- Domain gap between lab and field images  
- Poor generalization across crops and environments  
- High computational cost of deep learning models  
- Imbalance in severity classes  

---

## 🔍 Research Gaps
- Lack of transformer-based severity estimation models  
- Absence of end-to-end pipelines  
- Limited real-world dataset usage  
- Weak performance in intermediate severity classes  
- No integration of environmental factors (weather, soil, etc.)

---

## 🚀 Future Scope
- Use of attention-based and transformer models  
- Real-time deployment on mobile/edge devices  
- Integration of environmental and multimodal data  
- Improved dataset balancing techniques  
- Development of lightweight models for field usage  

---

## 📌 Conclusion
This study highlights that while deep learning models perform well in plant disease detection, **accurate severity estimation remains a challenging task**. Segmentation-based approaches provide more precise results compared to classification models. Future improvements are required for real-world deployment and generalization.

---

## 👨‍💻 Technologies Used
- Python
- PyTorch / TensorFlow
- OpenCV
- Deep Learning (CNN, U-Net, PSPNet)

---

## 📚 Reference
This project is based on literature survey and experimental analysis in the domain of:
**Plant Disease Detection and Severity Estimation using Deep Learning**
We referred git repo-https://github.com/esgario/lara2018.git
---
