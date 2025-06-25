
# 📊 Credit Score Classification using Statistical and Machine Learning Methods

This project explores the classification of credit scores using statistical analysis and machine learning models. The aim is to identify the most effective model for classifying credit scores ("Good", "Standard", "Poor") and discover which features are most influential.

📁 Developed as part of ECSE 411: Statistical Methods for Data Analysis  
🎓 Student: Ilke Kas (ixk238)  

---

## 🎯 Objectives

- ✅ Classify credit scores using models: Linear Regression, Logistic Regression, Decision Tree, and Random Forest.
- ✅ Compare performance across models using accuracy and confusion matrices.
- ✅ Apply dimensionality reduction via PCA.
- ✅ Identify most important features using Random Forest feature importance.
- ✅ Analyze relationships between features using statistical tools (correlation, covariance).

---

## 📦 Dataset

- Source: Kaggle Credit Score Dataset
- Size: ~999,961 records, 20+ features
- Target: `Credit_Score` (Good / Standard / Poor)
- Feature types:
  - Numeric (e.g., Outstanding Debt, Interest Rate)
  - Categorical (e.g., Credit Mix, Payment Behavior) — one-hot encoded

---

## 🧠 Models Implemented

| Model              | Type           | Notes |
|-------------------|----------------|-------|
| Linear Regression | Statistical    | Used with post-processing to classify classes |
| Logistic Regression | Classification | Best result with `newton-cg` solver |
| Decision Tree     | ML (Tree-based) | Default max depth performed best |
| Random Forest     | Ensemble ML     | Achieved ~85% accuracy |

---

## 📉 Dimensionality Reduction

- ✅ Principal Component Analysis (PCA)
  - First 4 components used for training
  - Resulted in lower performance than full model
- ✅ Feature Importance from Random Forest
  - Most influential features:
    - Outstanding Debt
    - Credit History Age
    - Interest Rate

---

## 📊 Statistical Analysis

- 🧮 Sample Mean, Variance, and Standard Deviation
- 🔁 Covariance and Correlation Matrices
- 📈 Visualizations:
  - Histograms
  - Box Plots (by credit score class)
  - Scatter Plots (for correlated features)

---

## 📌 Key Findings

- **Random Forest** outperformed all other models with ~85% accuracy.
- **Linear Regression**, although not ideal for classification, achieved 67%.
- PCA was **less effective** than feature importance for dimensionality reduction.
- Strong **positive correlations** were found among Annual Income, Monthly Inhand Salary, and Monthly Balance.
- Most influential features for classification:  
  🥇 Outstanding Debt → 🥈 Credit History Age → 🥉 Interest Rate

---

## 🛠️ Tools Used

- Python 3.11.8
- Jupyter Notebook (Colab)
- Libraries: `pandas`, `numpy`, `matplotlib`, `scikit-learn`

---


---

## 📚 References

- Dataset: [Kaggle Credit Score Classification Challenge](https://www.kaggle.com/)
- Key references cited in final report [30]-[40]  
(See `ECSE411 Final Report.docx` for detailed citations)

---

## 📬 Contact

For questions or collaboration:  
**Ilke Kas** – [ixk238@case.edu](mailto:ixk238@case.edu)

---

> 📌 *This project was conducted for academic purposes and showcases end-to-end statistical analysis and ML classification workflow on real-world financial data.*


