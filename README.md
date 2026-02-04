# 🔍 Understanding Drivers of NPS: Logistic Regression Analysis

This project aims to identify **which factors most influence the Net Promoter Score (NPS)** in customer feedback data. By cleaning and preparing the survey data, standardizing variables, and applying logistic regression, we seek to uncover the key variables that drive customer loyalty and satisfaction.


## 🎯 Project Goal

**Primary Objective**:  
To analyze survey responses and **identify which features (e.g., satisfaction with service, product usability, etc.) are most predictive of a high or low NPS**.

---

## ✅ Workflow Summary

### 1. Data Cleaning & Preparation 
- Removed or imputed missing values.
- One-hot encoded categorical variables.
- Standardized numerical features to ensure comparability.
- Detected potential reverse-coded questions — **further review needed**
- 🔄 Automated Preprocessing Added:
A new automated preparation pipeline is included to dynamically:
Detect question types (e.g., Likert scale, binary, categorical)
### 2. Model Building 
- Standardized numerical features to ensure comparability.
- Built a logistic regression model to predict **high vs. low NPS** categories.


## ⚠️ Known Issues & To-Do

- **Reverse-Coded Questions**: Some survey items may be on reversed scales (e.g., 1 = Strongly Agree vs. 1 = Strongly Disagree).
  - It's essential to confirm and adjust these to avoid misleading model results.
  - Special attention needed for the **NPS scale**: check if it follows the traditional 0–10 scale where:
    - 0–6 = Detractors
    - 7–8 = Passives
    - 9–10 = Promoters

- **Model Assumptions**: Logistic regression assumes linear relationships between the log odds and predictors. Consider other models (e.g. tree-based) for comparison.

---

## 🛠️ Tech Stack

- **Languages**: Python
- **Libraries**: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

## 📜 License

This project is licensed under the **MIT License** — free to use and modify.

---

## 👤 Author

Petar Rajic

Install required libraries with:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
