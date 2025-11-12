# Diabetes Prediction (Pima Indians Dataset)

Machine learning project predicting diabetes using Logistic Regression, Decision Tree, and Random Forest models. Includes data cleaning, feature importance, ROC curves, and model export.

---

## Goal  
Predict whether a person has **diabetes (Outcome = 1)** based on medical measurements using **Logistic Regression**, **Decision Tree**, and **Random Forest** models.

Dataset: [Pima Indians Diabetes Database – Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

---

## Project Overview  

This notebook demonstrates an end-to-end ML workflow:

1. **Data cleaning** — replace impossible zero values with NaN  
2. **Train/test split** — 80 % training, 20 % testing (stratified)  
3. **Pipeline models** — imputation, scaling, and classification  
4. **Evaluation** — Accuracy, Precision, Recall, F1, ROC-AUC  
5. **Visualization** — ROC curve & Confusion Matrix  
6. **Feature importance** — via Permutation Importance  
7. **Model saving** — export trained Random Forest model  

---

## Results  

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|:--|--:|--:|--:|--:|--:|
| Logistic Regression | 0.77 | 0.64 | 0.52 | 0.57 | 0.80 |
| Decision Tree (depth = 4) | 0.74 | 0.59 | 0.49 | 0.54 | 0.75 |
| Random Forest | **0.74** | **0.62** | **0.54** | **0.59** | **0.82** |

** Best model:** Random Forest (ROC-AUC = 0.82)  
** Top features:** Glucose, BMI, Age  

---

## Key Insights  

- Random Forest achieved the best overall balance between recall and precision.  
- Glucose and BMI are the strongest indicators of diabetes.  
- The model correctly classifies about **74 %** of patients.  
- Lowering the decision threshold increases recall (detects more diabetics).  

---

## How to Run  

1. **Clone the repository**
   `git clone https://github.com/akerkeabs/diabetes-ml.git`
   `cd diabetes-ml`

2. **Install dependencies**
   `pip install -r requirements.txt`

3. **Run the notebook**
   `jupyter notebook Pima_Indians_Diabetes.ipynb`

---

## Tech Stack
- Python 3

- pandas · numpy · matplotlib

- scikit-learn

- joblib

---

## Folder Structure

diabetes-ml/
├─ images/
│   ├─ confusion_matrix.png
│   └─ roc_curve.png
├─ Pima_Indians_Diabetes.ipynb
├─ requirements.txt
├─ .gitignore
└─ LICENSE

---

## License

This project is released under the MIT License.

---

## **Author:**
Akerke Absalykova

Data Science Portfolio 2025

[GitHub Profile](https://github.com/akerkeabs)

[LinkedIn](https://www.linkedin.com/in/akerke-absalykova/)
