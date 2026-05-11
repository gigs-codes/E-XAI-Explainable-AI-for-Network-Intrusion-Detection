# 🔐 E-XAI: Explainable AI for Network Intrusion Detection

An explainable, high-performance intrusion detection framework that evaluates black-box machine learning models using SHAP and LIME for transparent and trustworthy security analytics.

📄 **This project is based on a peer-reviewed research paper published at an international conference (ICDSA 2025).**

---

## 📌 About the Project

Artificial Intelligence–based Intrusion Detection Systems (IDS) often achieve high accuracy but suffer from a lack of interpretability, making them difficult to trust in real-world security environments.

**E-XAI** addresses this problem by combining:
- High-performing **black-box ML and ensemble models**
- **Explainable AI (XAI)** techniques for interpretability
- Multi-dataset evaluation to ensure robustness and generalization

This repository contains the **official implementation and experiments** corresponding to the published research paper.

---

## 🧠 Research Publication

**E-XAI: Evaluating Black-Box Explainable AI Frameworks for Network Intrusion Detection**  
📍 *International Conference on Data Science and Applications (ICDSA 2025)*

### Key highlights from the paper:
- Comprehensive evaluation of black-box ML models for IDS
- Integration of SHAP and LIME for model explainability
- Ensemble Voting Classifier achieving state-of-the-art results
- Strong generalization across multiple benchmark datasets

---

## 📊 Datasets Used

This project evaluates intrusion detection performance on three standard datasets:

- **CIC-IDS 2017** – Realistic modern network traffic with diverse attack types  
- **NSL-KDD** – Improved benchmark dataset with reduced redundancy  
- **SIMARGL 2021** – High-quality bidirectional flow-based intrusion dataset  

---

## ⚙️ Models Implemented

- Deep Neural Network (DNN)
- Multi-Layer Perceptron (MLP)
- Random Forest
- LightGBM
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- AdaBoost
- **Ensemble Voting Classifier (Boosted Decision Trees + Bagging Random Forest)**

---

## 🧪 Explainable AI Techniques

To interpret black-box predictions, the following XAI methods are used:

- **SHAP (SHapley Additive Explanations)**  
  - Global and local feature importance
- **LIME (Local Interpretable Model-Agnostic Explanations)**  
  - Instance-level explanations for individual predictions

These techniques help security analysts understand *why* a flow is classified as benign or malicious.

---

## 📈 Results Summary

The ensemble **Voting Classifier** achieved the best performance across all datasets:

| Dataset | Accuracy | Precision | Recall | F1-Score |
|------|---------|----------|-------|---------|
| CIC-IDS 2017 | 97.9% | 98.1% | 97.9% | 98.0% |
| NSL-KDD | 99.4% | 99.4% | 99.4% | 99.4% |
| SIMARGL 2021 | 100% | 100% | 100% | 100% |

These results demonstrate excellent robustness, generalization, and real-world applicability.

---

## 🖥️ System Pipeline

1. Dataset Collection  
2. Data Preprocessing & Feature Engineering  
3. Model Training and Validation (80:20 split)  
4. Ensemble Learning  
5. Explainability Analysis (SHAP / LIME)  
6. Performance Evaluation (Accuracy, Precision, Recall, F1-score, ROC-AUC)

---

## 🧾 Citation

If you use this work, please cite:


```text
Ankit Kumar et al.,
"E-XAI: Evaluating Black-Box Explainable AI Frameworks for Network Intrusion Detection",
Proceedings of ICDSA 2025.
