# 🧬 Gene Expression Analysis for Glioma Classification

> A statistically rigorous and reproducible framework for analyzing high-dimensional gene expression data (p >> n) for disease classification.

---

## 📌 Overview

This project investigates whether **high-dimensional transcriptomic data** contains statistically significant, reproducible, and interpretable patterns capable of distinguishing glioma from non-tumor brain tissue.

The dataset follows a **large p, small n** structure:

* ~54,613 gene expression features
* 180 samples (157 glioma, 23 controls)

The focus is not only on predictive accuracy, but also on **robustness, reproducibility, and interpretability**.

---

## 🧠 Key Concepts

* High-dimensional statistics (p >> n)
* Differential expression analysis
* Multiple testing correction (FDR)
* Dimensionality reduction (PCA)
* Machine learning classification
* Stability selection

---

## 🧪 Methodology

### 🔹 Data Preparation

* Gene expression data obtained from GEO (GSE4290)
* Metadata verification and consistency checks
* Preprocessing to ensure structural integrity

---

### 🔹 Differential Expression Analysis

* Welch’s t-tests
* Benjamini–Hochberg correction (False Discovery Rate)
* Effect size estimation (Cohen’s d)

---

### 🔹 Dimensionality Reduction

* Principal Component Analysis (PCA)
* Reduced ~54,000+ features to ~149 components
* Retained ~95% of total variance

---

### 🔹 Machine Learning Models

* Support Vector Machine (SVM)
* Logistic Regression
* Random Forest

Evaluation:

* Stratified 5-fold Cross-Validation

---

### 🔹 Stability Selection

* Identifies reproducible gene subsets
* Ensures robustness and reduces overfitting

---

## 📊 Results

* **Accuracy:** ~98.9% ± 1.36%
* **ROC-AUC:** ~0.996 ± 0.008
* Significant differential expression (adjusted p < 1e-45)

Stable gene signals include:

* SOX2, MSI2, CDK17
* RAB family genes
* PRKCZ, DNM3

---

## ⚠️ Limitations

* No external validation dataset
* Risk of overfitting in high-dimensional settings
* Biological interpretation limited to statistical findings

---

## 📁 Project Structure

```id="9xw2ye"
Gene-Expression-Glioma-Classification/
│
├── gene_expression_analysis.ipynb
├── project_report.pdf
├── README.md
└── requirements.txt
```

---

## 📄 Project Report

A detailed report is included covering:

* statistical methodology
* mathematical framework
* experimental results
* biological interpretation

File: `Glioma Classification_report.pdf`

---

## 🛠️ Tech Stack

* Python (NumPy, pandas, scikit-learn, SciPy)
* Matplotlib, Seaborn
* GEO dataset (GSE4290)
* Affymetrix microarray platform

---

## 📚 Research Focus

This work emphasizes:

* statistically valid inference in high-dimensional data
* reproducible machine learning workflows
* interpretable results in biomedical applications

---

## 👩‍💻 Author

Maryam Shaikh

MSc Applied Statistics

Interests: Statistical Learning | Bioinformatics | Data Science
