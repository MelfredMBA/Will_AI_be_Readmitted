Programmer: Melfred P. Sumaya, PTRP, MBA
Project: Will AI be Readmitted?: An AI-assisted hospital readmission assessment.

This project predicts whether a patient is likely to be readmitted to the hospital within 30 days of discharge using previous information from the user. It focuses on using age, BMI, previous admissions, diabetes status, and comorbidities.

Features

- Interactive web form for entering patient details
- Real-time risk output (LOW / MODERATE / HIGH) with probability according to threshold.
- BMI, comorbidity score, and diabetes status are the main factors
- Shows the top risk drivers behind the prediction
- Fairness audit across age, BMI, and diabetes groups
- Bias mitigation tested with reweighting and group thresholds

Program Stack

Backend
- Flask (Python)

Frontend
- HTML, CSS (W3.CSS), JavaScript

Machine Learning
- scikit-learn (Logistic Regression, Decision Tree, Random Forest)
- XGBoost (used for comparison only)
- Final model: Logistic Regression
- Explainability: SHAP, Partial Dependence Plots (PDP + ICE)

Fairness
- Custom metrics: Demographic Parity, Disparate Impact (EEOC 80% rule),
  Equal Opportunity, Equalized Odds to address different scenarios of people.

Deployment
- Google Colab + ngrok

Environment
- Python 3.10+, Jupyter Notebook or Google Colab

Repository structure

hospital-readmission-prediction/
├── data/ Dataset and data dictionary
├── models/ Trained model, scaler, and feature info
├── notebooks/ Full pipeline notebook
├── src/ Python source scripts and Flask app
│ ├── app.py
│ ├── fairness_mitigation.py
│ ├── model.py
│ ├── preprocess.py
│ └── templates/
│ └── index.html
├── docs/ Final report
├── requirements.txt
├── LICENSE
└── README.md
