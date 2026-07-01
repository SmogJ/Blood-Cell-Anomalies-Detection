# Automated Detection and Classification of Blood Cell Anomalies Using Machine Learning

## 📌 Overview
This project applies **data science and machine learning** to automate the detection and classification of blood cell anomalies. Accurate identification of abnormal blood cells is critical for diagnosing conditions such as **leukemia, anemia, sickle cell disease, and infections**. Traditional manual microscopy is slow, subjective, and prone to human error. By leveraging modern AI techniques, this project aims to build interpretable, clinically reliable models that generalize across diverse blood cell types and laboratory conditions.

*The Project was done a part of the 3MTT Mentorship.*

---

## 🎯 Problem Statement
1. **Binary Classification** – Distinguish between normal and abnormal blood cells.  
2. **Multi-Class Classification** – Identify specific cell types among 19 categories.  
3. **Disease-Level Prediction** – Predict broader disease categories (Leukemia, Anemia, Sickle Cell, Infection, Artefact).  
4. **Benchmarking** – Compare performance against **CytoDiffusion** benchmarks (AUC = 0.990, Blast Cell sensitivity = 0.905).  
5. **Explainability** – Provide interpretable insights into morphological and clinical features influencing anomaly detection.  

---

## ✅ Expected Outcomes
- A robust ML model (ensemble methods, CNNs, or hybrid approaches) with high accuracy and sensitivity.  
- Feature importance analysis highlighting clinically relevant predictors.  
- Validation against CytoDiffusion benchmarks to assess robustness.  
- A framework adaptable to real-world hematology labs for faster, more reliable diagnostics.  

---

## 📊 Dataset
- **Size**: 5,880 blood cell records across 19 cell types (7 normal, 12 abnormal).  
- **Features (36 total)**:  
  - Morphological (diameter, circularity, eccentricity, nucleus area, chromatin density)  
  - Colorimetric (RGB values, stain intensity)  
  - Clinical CBC metrics (WBC count, hemoglobin, platelet count)  
  - Acquisition metadata (microscope model, magnification, resolution)  
  - AI scores (CytoDiffusion anomaly score, classification confidence)  
- **Source**: Kaggle – *Blood Cell Anomaly Detection 2025*  

---

## 🛠️ Methodology
1. **Data Preprocessing**  
   - Cleaning, handling missing values, normalization, encoding categorical variables.  
2. **Exploratory Data Analysis (EDA)**  
   - Feature visualization, correlation analysis, class imbalance detection.  
3. **Binary Classification**  
   - Logistic Regression, Random Forest baselines.  
4. **Multi-Class Classification**  
   - CNNs, Gradient Boosting, algorithm comparison.  
5. **Feature Importance**  
   - SHAP/LIME interpretability, ranking morphological vs clinical features.  
6. **Benchmarking**  
   - Validation against CytoDiffusion metrics.  
7. **Disease-Level Prediction**  
   - Aggregating cell-level predictions into disease categories.  
8. **Clinical Validation**  
   - Explainability with SHAP/LIME, comparison with hematologist expertise.  

---

## 🚀 Getting Started

### Prerequisites
- Python 3.9+  
- Kaggle Notebook 
- Libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `tensorflow` or `pytorch`, `shap`, `lime`

### Installation
Clone the repository:
```bash
git clone https://github.com/your-username/blood-cell-anomaly-detection.git
cd blood-cell-anomaly-detection
