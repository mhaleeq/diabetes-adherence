# 📘 Diabetes Medication Adherence Prediction

## 📌 Problem Statement
Diabetes mellitus is a chronic condition that requires consistent medication adherence to prevent complications. Unfortunately, many patients struggle with adherence, leading to poor outcomes.  
This project builds a machine learning model to **predict which patients are likely to be non-adherent**, based on demographic and clinical data.  

---

**Dataset**: [Diabetes Adherence Data — Mendeley (CC0 1.0)](https://data.mendeley.com/datasets/zkp7sbbx64/2)  

The dataset is provided in `/data/Diabetes_Adherence_Data.csv`.

---

## 🧹 Data Preparation
- Handled missing values.  
- Encoded categorical variables (e.g., gender, education level).  
- Scaled numerical features (age, BMI, blood sugar).  

---

## 🔍 Exploratory Data Analysis (EDA)
Key questions explored:
- What percentage of patients are adherent vs non-adherent?  
- Which factors are most correlated with adherence?  
- Visualized distributions and correlations.  

Example:
![Adherence Distribution](visuals/adherence_distribution.png)  

---

## 🤖 Modeling
Models tested:
- Logistic Regression  
- Random Forest Classifier  
- XGBoost  

Evaluation metrics:
- Accuracy  
- ROC-AUC Score  
- Precision & Recall  

---

## 📈 Results & Insights
- The best-performing model was **Random Forest (ROC-AUC = 0.82)**.  
- Key predictors: **age, education level, number of comorbidities, and prior adherence history**.  
- Insights suggest targeted interventions can help high-risk groups.  

---

## 🚀 Next Steps
- Collect more granular behavioral data (diet, exercise, reminders).  
- Deploy as a **Streamlit app** for clinicians to use.  
- Expand to other chronic diseases.  

---

## 📝 How to Run
```bash
# Clone repo
git clone https://github.com/YourUsername/diabetes-adherence.git
cd diabetes-adherence

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook notebooks/diabetes_adherence.ipynb
 
