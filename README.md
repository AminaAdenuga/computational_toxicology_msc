# computational_toxicology_msc
# Machine Learning Prediction of Aquatic Toxicity of Pesticides Using Molecular Descriptors

## MSc Industrial Chemistry Research Project

This repository contains the computational workflow developed for my MSc research in Industrial Chemistry. The project integrates **computational toxicology**, **cheminformatics**, and **machine learning** to predict the acute aquatic toxicity (96-hour LC₅₀) of pesticides using molecular descriptors generated from chemical structures.

---

## Research Objective

The aim of this study is to develop a machine learning model capable of predicting the acute aquatic toxicity (96-hour LC₅₀) of pesticides detected in aquatic environments using molecular descriptors and fingerprints generated from their chemical structures.

Ultimately, the developed workflow will support rapid toxicity assessment while complementing conventional laboratory-based ecotoxicological studies.

---

## Research Workflow

```text
US EPA ECOTOX Database
          │
          ▼
Data Collection
          │
          ▼
Exploratory Data Analysis
          │
          ▼
Data Cleaning & Preprocessing
          │
          ▼
Chemical Structure Retrieval
(PubChem)
          │
          ▼
Structure Standardization
          │
          ▼
RDKit Descriptor Generation
          │
          ▼
Feature Engineering
          │
          ▼
Feature Selection
          │
          ▼
Machine Learning Model Development
          │
          ▼
Model Evaluation
          │
          ▼
Toxicity Prediction Pipeline
```

---

# Current Project Status

| Phase | Status |
|--------|--------|
| ECOTOX Data Collection | ✅ Completed |
| Exploratory Data Analysis | ✅ Completed |
| Data Cleaning & Preprocessing | ✅ Completed |
| Chemical Structure Retrieval | ⏳ In Progress |
| Molecular Descriptor Generation | ⏳ Pending |
| Feature Engineering | ⏳ Pending |
| Machine Learning Model Development | ⏳ Pending |
| Model Evaluation | ⏳ Pending |
| Prediction Pipeline | ⏳ Pending |

---

# Dataset Summary

Current cleaned dataset:

- **4,584 toxicity records**
- **1,302 unique chemicals**
- **96-hour LC₅₀ endpoint**
- **Species:** *Pimephales promelas* (Fathead Minnow)
- **Target Variable:** log₁₀(LC₅₀)

Data source:

- US EPA ECOTOX Knowledgebase

---

# Repository Structure

```text
computational_toxicology_msc/

├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_ecotox_exploration.ipynb
│   └── 02_data_cleaning.ipynb
│
├── reports/
│   ├── figures/
│   ├── tables/
│   ├── data_quality_report.ipynb
│   └── preprocessing_summary.csv
│
└── README.md
```

---

# Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- RDKit *(planned)*
- Scikit-learn *(planned)*
- Jupyter Notebook
- Git
- GitHub

---

# Data Preprocessing

Completed preprocessing steps include:

- Removal of duplicate records
- Missing value assessment
- Removal of variables with excessive missingness
- Removal of non-informative metadata columns
- Concentration unit inspection
- Log transformation of LC₅₀ values
- Dataset quality assessment

---

# Planned Machine Learning Models

The following regression algorithms will be evaluated:

- Linear Regression
- Random Forest Regression
- Gradient Boosting
- XGBoost
- Support Vector Regression
- Extra Trees Regression

The final model will be selected based on predictive performance.

---

# Evaluation Metrics

Model performance will be evaluated using:

- R²
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Squared Error (MSE)

---

# Research Significance

This research contributes to computational toxicology by developing an interpretable machine learning workflow for predicting pesticide toxicity. The proposed framework aims to reduce dependence on laboratory toxicity testing while supporting environmental risk assessment and chemical prioritization.

---

# Author

**Amina Adenuga**

MSc Industrial Chemistry

Bells University of Technology, Ota

Nigeria

---

# Supervisor

*(To be updated)*

---

# License

This repository is maintained for academic research purposes.
