# Predicting Major Interventions through Network Medicine using Machine Learning
#### Submitted by: Ori Shai and Osnat Blau 
#### Course: Machine Learning in Medicine - 6811902 
#### Lecturer: DR. Eliahoo Galit 
##### Date: July 29, 2026 
This repository/project develops an interpretable, fair, and calibrated machine learning framework using electronic health record (EHR) data from the **MIMIC-IV** database. By combining **Network Medicine** principles, **K-Means clustering** (patient archetyping), and **tree-based ensemble algorithms (Random Forest & XGBoost)**, the system predicts the need for major clinical interventions upon hospital admission.

---

## 🔗 Project Links

* **Article:** [Predicting Major Interventions through Network Medicine using Machine Learning]()
* **Colab Notebook:** [Predicting Major Interventions Notebook]()

---
**Project Objective & Research Question**
The primary objective of this project is to develop an interpretable, fair, and calibrated Machine Learning framework to predict the requirement for major clinical interventions upon hospital admission using Electronic Health Record (EHR) data from the MIMIC-IV database.
**Research Question**
"To what extent can Network Medicine features and unsupervised patient archetypes, when combined with explainable tree-based ensemble algorithms, accurately and fairly forecast the early need for major invasive medical procedures upon hospital admission without compromising demographic equity?"


## 📌 Key Features
* **Comorbidity Networks & Archetypes:** Maps disease co-occurrence and identifies patient archetypes (e.g., Cardiorenal, Metabolic Syndrome) via K-Means and t-SNE.
* **Leakage-Free Pipeline:** Employs `StratifiedGroupKFold` cross-validation grouped by patient IDs with in-fold SMOTE oversampling.
* **Model Calibration & Explainability:** Evaluates ROC-AUC, PR-AUC, and Brier Score, using SHAP values for clinical interpretability.
* **Gender-Stratified Analysis:** Assesses model fairness and performance disparities across male and female patient cohorts.
