# Loan Acceptance Prediction – Binary Classification Model

A predictive model built using Logistic Regression to determine whether a loan application will be accepted or rejected based on applicant features. This project walks through the full Data Science Lifecycle from data loading to model evaluation on a real-world loan dataset.

---

## Overview

This project explores how individual demographic and financial factors influence loan acceptance. By applying machine learning techniques—specifically Logistic Regression—the model learns to classify loan status based on applicant details like income, education, credit history, and more.

---

## Objective

To develop a binary classification model that predicts whether a loan will be approved (`Loan_Status = Y`) or rejected (`Loan_Status = N`) based on input features using logistic regression.

---

## Dataset Description

The dataset contains 614 rows and 14 features, including:

- **Applicant Information**: Gender, Marital Status, Dependents, Education, Employment  
- **Financial Metrics**: ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History  
- **Geographic Indicator**: Property_Area  
- **Target Variable**: Loan_Status (Y/N)

---

## Exploratory Data Analysis (EDA)

- **Missing Values**: Detected in `Gender`, `Married`, `Dependents`, `Self_Employed`, `LoanAmount`, `Loan_Amount_Term`, and `Credit_History`. These were cleaned and imputed appropriately.
- **Data Types**: Mix of categorical and numerical data, requiring encoding for modeling.
- **Insights**:
  - Credit history was found to be a **strong predictor** of loan approval.
  - Higher applicant income correlated with approval likelihood.
  - Urban and semi-urban applicants had higher acceptance rates.

---

## Model Used

- **Logistic Regression**: Chosen for its interpretability and effectiveness on binary classification problems.
- **Evaluation Metrics**:
  - Accuracy  
  - Confusion Matrix  
  - Precision, Recall, F1-Score

---

## Results & Evaluation

- The logistic regression model achieved strong performance in predicting loan approval.
- Credit history emerged as the **most influential feature**, followed by income.
- Evaluation metrics confirmed balanced performance between precision and recall.

---

## Technologies Used

- **Language**: Python  
- **Libraries**: `pandas`, `matplotlib`, `seaborn`, `scikit-learn`  
- **Model**: Logistic Regression (via `sklearn.linear_model`)

---

## Future Enhancements

- Try ensemble models like Random Forest or XGBoost for improved accuracy.
- Use feature selection techniques to eliminate redundant inputs.
- Deploy the model via a web interface or API for real-time loan screening.
