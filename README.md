# Electricity Fraud Detection using Machine Learning

## Project Overview
This project focuses on detecting fraudulent electricity consumption using machine learning techniques on highly imbalanced real-world data.

## Business Problem
Electricity fraud causes significant financial losses for utility companies and impacts overall energy distribution systems. Detecting fraudulent behavior is challenging due to the rarity of fraud cases and the lack of direct indicators.

## Dataset
- Source: State Grid Corporation of China (SGCC)
- Type: Time-series electricity consumption data
- Target: Fraud vs Non-Fraud

## Key Challenge: Class Imbalance
The dataset is highly imbalanced, making fraud detection difficult. This project explores multiple strategies to address this issue:
- Class weighting
- Oversampling (SMOTE)
- Undersampling

## Methodology
- Exploratory Data Analysis (EDA)
- Data preprocessing:
  - Missing value imputation
  - Normalization
- Models tested:
  - Logistic Regression
  - Random Forest
  - XGBoost

## Results
- Best model: XGBoost (with imbalance handling)
- Improved recall for fraud detection
- Evaluation metrics:
  - Precision
  - Recall
  - F1-score
  - AUC-PR (key metric for imbalanced data)

## Key Insights
- Proper handling of class imbalance significantly improves fraud detection
- AUC-PR is more reliable than accuracy in this context
- Advanced models outperform baseline approaches

## Future Work
- Deploy model as a real-time fraud detection system
- Incorporate temporal modeling (LSTM / time series models)
- Feature engineering with domain knowledge

## Tech Stack
- Python
- pandas, scikit-learn
- imbalanced-learn
- XGBoost

## Project Structure
```
data/ # Dataset or sample data
notebooks/ # Jupyter notebooks for analysis and modeling
src/ # Source code (preprocessing, modeling, evaluation)
images/ # Visualizations used in the README
README.md # Project documentation
requirements.txt # Dependencies
```
## How to Run
```bash
pip install -r requirements.txt
