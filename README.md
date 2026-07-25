# FraudShield – Intelligent Transaction Risk Analyzer

## Project Overview

FraudShield is an end-to-end Machine Learning project developed to analyze and detect fraudulent credit card transactions using historical transaction data.

The project includes data cleaning, exploratory data analysis (EDA), feature engineering, machine learning model building, model evaluation, and business insights

## Objectives

- Analyze fraudulent transaction patterns.
- Build machine learning models to classify fraudulent transactions.
- Compare model performance.
- Generate insights that can help financial institutions understand fraud behaviour.

## Dataset

**Dataset:** IBM Credit Card Transactions Dataset

The dataset contains more than **24 million transaction records** with transaction-related information such as:

- Transaction Amount
- Transaction Date
- Transaction Time
- Merchant Category Code (MCC)
- Transaction Type (Chip / Swipe / Online)
- Fraud Label (Yes/No)

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

## Data Preprocessing

The following preprocessing steps were performed:

- Removed "$" symbol from Amount column
- Converted Amount into numeric values
- Converted Fraud labels into binary values (0 and 1)
- Extracted Hour from transaction time
- Applied One-Hot Encoding on Transaction Type (Use Chip)
- Selected relevant features for model training
  
## Exploratory Data Analysis (EDA)

The project includes analysis of:

- Fraud Transactions by Hour
- Fraud Transactions by Month
- Transaction Type Distribution
- Fraud Amount Distribution
- Merchant Category (MCC) Analysis

---

## Machine Learning Models

The following models were implemented and compared:

1. Logistic Regression
2. Random Forest Classifier
3. XGBoost Classifier

## Model Performance

| Model               | Accuracy | Recall | Dataset Used                |
| ------------------- | -------: | -----: | --------------------------- |
| Logistic Regression |   88.00% |    65% | Full Dataset                |
| Random Forest       |   99.67% |    31% | 50K Train / 10K Test Sample |
| XGBoost             |   99.87% |    N/A | 50K Train / 10K Test Sample |


## Model Evaluation

Models were evaluated using:

- Confusion Matrix
- ROC Curve
- Precision-Recall Curve
- Feature Importance

## Key Insights

- Online transactions recorded the highest number of fraud cases.
- Fraud cases varied across different hours of the day.
- Fraud occurrences also varied by month.
- Certain Merchant Category Codes (MCC) had more fraud transactions than others.
- Logistic Regression achieved the highest fraud recall among the evaluated models.
- Random Forest and XGBoost achieved very high accuracy on the sampled dataset.

## Project Structure

```
FraudShield/
│
├── Fraud Detection.ipynb
└── README.md
```
## Author

**Aditi Kashyap**

B.Tech – Computer Science & Engineering
