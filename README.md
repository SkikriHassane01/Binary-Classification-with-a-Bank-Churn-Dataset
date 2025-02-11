# Bank Customer Churn Prediction

## Overview
This project focuses on predicting customer churn in a banking context as part of a Kaggle competition. Two distinct approaches were implemented to solve this binary classification problem, achieving competitive results through different methodologies.

## Project Structure
```
├── notebooks/
│   ├── version1_traditional_approach.ipynb
│   └── version2_pipeline_approach.ipynb
├── requirements.txt/
├── runtime.txt/
├── data/
│   ├── train.csv
│   ├── Churn_Modeling.csv
│   └── test.csv

```

## Approaches & Results

### Version 1: Traditional Approach
The first implementation focused on manual feature engineering and model optimization:

- **Data Preprocessing**:
  - Custom cleaning techniques
  - Feature encoding
  - Feature scaling
  
- **Modeling**:
  - Algorithm: RandomForestClassifier
  - Hyperparameter optimization using Optuna
  - Final Performance: 0.8832 accuracy score

### Version 2: Pipeline-Based Approach
The second version emphasized reproducibility and automation:

- **Exploratory Data Analysis (EDA)**:
  - Distribution analysis
  - Feature correlations
  - Missing value analysis
  
- **Feature Engineering Pipeline**:
  - Automated preprocessing steps
  - Consistent transformation between train and test sets
  
- **Model Evaluation**:
  Multiple models were trained and optimized:
  - Random Forest
  - CatBoost
  - LightGBM
  - XGBoost
  
- **Ensemble Learning**:
  - Implemented Voting Classifier
  - Combined strengths of multiple models
  - Final Performance: 0.8919 accuracy score


## Technologies Used
- Matplotlib
- seaborn
- Scikit-learn
- Optuna
- CatBoost
- LightGBM
- XGBoost
- Pandas
- NumPy

## Getting Started
1. Clone the repository
2. Install required packages: `pip install -r requirements.txt`
3. Run Jupyter notebooks in the `notebooks/` directory

## Future Improvements
- Feature selection optimization
- Deep learning implementation
- Cross-validation strategies
- Hyperparameter tuning for ensemble weights

## Competition Results
This project was developed as part of a Kaggle competition, achieving competitive results through both implementations:
- Traditional Approach: 0.8832
- Pipeline-Based Approach: 0.8919

## Author
hassane skikri