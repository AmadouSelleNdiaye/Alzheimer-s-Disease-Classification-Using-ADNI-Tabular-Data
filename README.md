# 🧠 Alzheimer’s Disease Classification Using ADNI Tabular Data

This project explores early detection of Alzheimer’s disease using clinical, cognitive, and biomarker data from the **Alzheimer's Disease Neuroimaging Initiative (ADNI)**. The goal is to classify patients into three diagnostic groups — **Normal Control (NC)**, **Mild Cognitive Impairment (MCI)**, and **Alzheimer's Disease (AD)** — using tabular data and machine learning models.

## 🔍 Key Components

- **Dataset**: 744 patients with over 2,800 features, including:
  - Demographic data
  - Imaging biomarkers (e.g., hippocampal volumes)
  - Biological markers (`amyloid_positive`, `PLASMA_NFL`, etc.)

- **Preprocessing**:
  - Removal of columns with >50% missing values
  - KNN-based imputation of missing data
  - Feature selection based on clinical insight and variance analysis
  - Normalization and dimensionality reduction (PCA, t-SNE)

- **Models Tested**:
  - K-Nearest Neighbors (KNN)
  - Random Forest
  - Neural Network
  - Ensemble Methods (Gradient Boosting, Voting)

## 🏆 Best Performance

- **Random Forest** achieved:
  - **Accuracy**: 86.02%
  - **Macro F1-score**: 0.88
- Most predictive features:
  - `amyloid_positive`
  - `PLASMA_NFL`
  - `TAU`
  - `hippocampus_L/R__volume`

## 📈 Insights & Future Work

- Better handling of missing data
- Addressing class imbalance with SMOTE
- Predicting MCI progression to AD
- Hyperparameter optimization
- Integrating multimodal data
- Towards deployment as a clinical tool

---

Project completed as part of the course **IMN716 – Topics in Computer Vision**  
Supervised by **Prof. Maxime Descoteaux**  
**Université de Sherbrooke – April 2025**
