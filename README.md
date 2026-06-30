# Customer Churn Prediction using Machine Learning

## Overview

Customer churn prediction is an important machine learning application that helps businesses identify customers who are likely to stop using their services. Early prediction enables companies to improve customer retention through targeted interventions.

This project implements a complete machine learning workflow for customer churn prediction, including data preprocessing, handling missing values, class imbalance correction, model comparison, and deployment-ready model serialization.

---

## Features

- Data preprocessing and cleaning
- Missing value imputation
- One-hot encoding of categorical variables
- Class imbalance handling using SMOTE
- Comparison of multiple machine learning algorithms
- Cross-validation based model evaluation
- ROC curve comparison
- Feature importance analysis
- Model serialization for deployment

---

## Dataset

The dataset used in this project was obtained from **Kaggle**.

It contains customer information such as:

- Age
- Gender
- Monthly Usage Hours
- Number of Transactions
- Subscription Type
- Complaint Count
- Customer Churn (Target)

The original dataset is **not included** in this repository due to Kaggle licensing.

You can download a similar dataset from Kaggle and place it inside the `data/` directory.

---

## Machine Learning Workflow

```
Customer Dataset
        │
        ▼
Data Cleaning
        │
        ▼
Missing Value Imputation
        │
        ▼
Categorical Encoding
        │
        ▼
SMOTE Oversampling
        │
        ▼
Train-Test Split
        │
        ▼
Model Training
        │
        ▼
Model Comparison
        │
        ▼
Best Model Selection
        │
        ▼
Model Saving
```

---

## Models Evaluated

- Logistic Regression
- Random Forest
- K-Nearest Neighbors
- AdaBoost
- Bagging
- Gradient Boosting
- Ridge Classifier
- XGBoost

---

## Best Performing Model

After comparing multiple machine learning algorithms using cross-validation, **XGBoost** achieved the best overall performance and was selected as the final model.

Evaluation metrics included:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- Matplotlib
- Seaborn
- Pickle

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/customer-churn-prediction.git
```

Install required packages

```bash
pip install -r requirements.txt
```

---

## Running the Project

Open the notebook

```
notebook/customer-churn-prediction.ipynb
```

Run all cells sequentially.

The notebook performs:

- Data preprocessing
- Exploratory Data Analysis
- Model training
- Model evaluation
- Feature importance analysis
- Model saving

---

## Outputs

The project generates:

- Exploratory plots
- ROC curve comparison
- Confusion Matrix
- Feature Importance Plot
- Saved XGBoost model
- Feature column names for deployment

---

## Deployment

The trained model is saved as

```
churn_prediction_model.pkl
```

This model can be integrated with:

- Flask
- FastAPI
- Streamlit
- Django
- REST APIs

---

## Repository Structure

```
Customer-Churn-Prediction/
│
├── notebook/
│   └── customer-churn-prediction.ipynb
│
├── data/
│   └── README.md
│
├── models/
│   ├── churn_prediction_model.pkl
│   └── feature_columns.pkl
│
├── docs/
│   └── Report.pdf
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Future Improvements

- Hyperparameter optimization
- Explainable AI using SHAP
- Streamlit web application
- Docker deployment
- Automated model retraining

---

## Author

**Mayuri Dhakane**
M.Tech Computational Biology
IIITD
---

## License

This repository is intended for educational and research purposes.
