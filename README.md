# Efficient Rice Variety Classification Using Deep Learning

This repository contains the implementation and evaluation of deep learning models for automated rice variety classification. The project compares a **Custom Convolutional Neural Network (CNN)** built from scratch with a **MobileNetV2 transfer learning model**, focusing on accuracy, efficiency, and deployment feasibility in agricultural applications.

---

## 📌 Project Overview
Rice is a staple food worldwide, and accurate classification of rice varieties is crucial for quality control, supply chain management, and smart agriculture. Traditional manual inspection is slow, error-prone, and inefficient. This project leverages deep learning to automate rice variety classification using image data.

- **Dataset**: [Rice Image Dataset (Koklu et al., 2021)](https://www.muratkoklu.com/datasets/)  
  - 75,000 RGB images  
  - 5 rice varieties: Arborio, Basmati, Ipsala, Jasmine, Karacadag  
  - Balanced dataset (15,000 images per class)

- **Models Implemented**:
  - Custom CNN (baseline + tuned variants)
  - MobileNetV2 (feature extraction + fine-tuning strategies)

- **Evaluation Metrics**:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Robustness under noise and lighting variations

---

## 🚀 Key Results
- **Custom CNN**: Achieved strong performance with careful tuning, but required more training time and resources.  
- **MobileNetV2**: With partial fine-tuning, achieved **99.03% test accuracy** and **0.99 precision/recall/F1-score**, while being lightweight and efficient for deployment on edge devices.  

> Findings demonstrate that lightweight transfer learning models like MobileNetV2 are highly suitable for real-world agricultural applications.

---

## 📂 Repository Structure
├── data_preprocessing/       # Scripts for dataset preparation and augmentation
├── cnn_model/                # Custom CNN implementation (baseline + tuned)
├── mobilenetv2_model/        # MobileNetV2 implementation (transfer learning + fine-tuning)
├── model_comparison/         # Evaluation and comparison scripts
├── results/                  # Accuracy, loss curves, confusion matrices
└── README.md                 # Project documentation


---

## ⚙️ Methodology
1. **Data Acquisition & Preprocessing**  
   - Balanced sampling, augmentation (rotation, noise, lighting variations).  
2. **Model Development**  
   - Custom CNN trained from scratch.  
   - MobileNetV2 with transfer learning and fine-tuning.  
3. **Training & Validation**  
   - Early stopping, hyperparameter tuning.  
4. **Evaluation**  
   - Performance metrics + robustness analysis.  
5. **Visualization**  
   - Accuracy/loss curves, confusion matrices, bar charts.  

---

## 📊 Visualization Examples
- Training & validation accuracy/loss curves  
- Confusion matrices for CNN and MobileNetV2  
- Bar charts of dataset distribution  

---

## 🔮 Future Work
- Explore **EfficientNet** and **Vision Transformers (ViT)** for improved accuracy.  
- Integrate **Explainable AI (XAI)** tools (LIME, SHAP) for model transparency.  
- Deploy models on mobile/edge devices for real-time agricultural use.  

---

## 👩‍💻 Author
**Phyo Phyo San**  
Module Code: CT100-3-M-DL  
Supervisor: Assoc. Prof. Dr. Raja Rajeswari Ponnusamy  

---

## 📜 License
This project is for academic purposes. Please cite appropriately if used in research or development.
