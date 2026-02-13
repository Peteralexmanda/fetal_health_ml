# fetal_health_ml
Jupyter Notebook for fetal health classification using CTG data



# Predictive Modeling for Obstetric Diagnostics Using Machine Learning

**Course:** MDSC 6103 – Artificial Intelligence (Machine Learning & Business Intelligence)  
**Student:** Peter Manda  
**Assignment:** Fetal Health Classification Using CTG Data

---

## Project Overview

This repository contains a Jupyter Notebook that performs exploratory data analysis (EDA) and develops machine learning models to classify fetal health status using CTG (Cardiotocography) datasets. The goal is to support automated fetal health diagnostics and improve clinical decision-making.

---

## Datasets

1. **Fetal Health Dataset (`fetal_health.csv`)**  
   - Includes CTG measurements and fetal health classes.  
   - Target column: `fetal_health`

2. **CTG Dataset (`CTG.csv`)**  
   - Contains additional CTG features and fetal health classification.  
   - Target column: `NSP`  
   - Rows with missing target labels are removed before modeling.

---

## Datasets Source / Acknowledgment

- The **Fetal Health Dataset** and **CTG Dataset** were obtained from [Kaggle](https://www.kaggle.com/).  
- We acknowledge the dataset creators for providing access to this data for research and academic purposes.

---

## Features & Preprocessing

- Only numeric features are used for modeling.  
- StandardScaler is applied to standardize features (mean=0, std=1).  
- Train-test split: 80% training, 20% testing, stratified by the target class.

---

## Machine Learning Models

Four classifiers are implemented:

1. **Logistic Regression** – interpretable baseline model.  
2. **Random Forest** – handles non-linear patterns and imbalanced data.  
3. **Support Vector Machine (SVM)** – effective in high-dimensional space.  
4. **K-Nearest Neighbors (KNN)** – instance-based, captures similar CTG patterns.

---

## Evaluation Metrics

Models are evaluated using:

- Accuracy  
- Confusion Matrix  
- Classification Report (Precision, Recall, F1-score)  

Plots are generated for target distribution, feature distributions, and correlations.

---

## Repository Contents

| File | Description |
|------|-------------|
| `fetal_health_classification.ipynb` | Jupyter Notebook with EDA and ML pipeline |
| `Fetal_Health_Coverpage.docx` | Cover page for submission |
| `fetal_health.csv` | Fetal Health Dataset |
| `CTG.csv` | CTG Dataset |

---

## How to Run

1. Clone the repository:  
```bash
git clone https://github.com/<your-username>/fetal_health_ml.git


2. Open `fetal_health_classification.ipynb` in Jupyter Notebook or JupyterLab.

3. Install required Python packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

4. Run all cells to perform EDA, train models, and evaluate results.

---

## License

This project is for academic purposes only.

