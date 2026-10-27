# Medical Insurance Cost Prediction

A machine learning project that predicts medical insurance charges using **Multiple Linear Regression** with Python and Scikit-learn.

## Overview

This project explores a medical insurance dataset to understand the factors associated with insurance charges and build a regression model to predict individual insurance costs.

The workflow covers data inspection, Exploratory Data Analysis (EDA), data preprocessing, feature engineering, model training, and evaluation.

## Dataset

This project uses the **Medical Cost Personal Dataset** from Kaggle.

- **Source:** [Medical Cost Personal Dataset — Kaggle](https://www.kaggle.com/mirichoi0218/insurance)
- **Dataset file:** `insurance.csv`
- **Records:** 1,338
- **Columns:** 7
- **Target variable:** `charges`
- **Problem type:** Regression

The dataset contains information about age, sex, Body Mass Index (BMI), number of children, smoking status, residential region, and individual medical insurance charges.

**Note:** The dataset file is not included in this repository. Download it from the original source and place `insurance.csv` in the appropriate directory before running the notebook.

### Dataset License

Please refer to the original dataset page for its current license and usage terms.

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Inspection
- Loaded the dataset using Pandas.
- Examined the dataset structure and descriptive statistics.
- Checked for missing values and duplicate records.
- Removed duplicate records.

### 2. Exploratory Data Analysis (EDA)
- Analyzed the distribution of medical insurance charges.
- Examined categorical feature distributions.
- Used correlation analysis to explore relationships between numerical features.
- Created scatter plots and box plots to investigate patterns in the data.

### 3. Data Preprocessing
- Separated the input features and target variable.
- Applied one-hot encoding to categorical variables.
- Preserved numerical feature values for model training.

### 4. Feature Engineering
- Created an interaction feature, `age_smoker`, by multiplying age by the encoded smoking-status feature.

### 5. Model Training
- Split the dataset into training and testing sets.
- Trained a Multiple Linear Regression model using Scikit-learn.

### 6. Model Evaluation
Evaluated the model using the following regression metrics:

- **R² Score:** Measures the proportion of variation in insurance charges explained by the model.
- **Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted values.
- **Root Mean Squared Error (RMSE):** Measures prediction error in the same units as the target variable.

Actual and predicted insurance charges were also compared visually.

## Visualizations

### 1. Insurance Charges Distribution

![Insurance Charges Distribution](images/charges-distribution.png)

### 2. Correlation Heatmap

![Correlation Heatmap](images/correlation-heatmap.png)

### 3. Age vs Insurance Charges

![Age vs Insurance Charges](images/age-vs-charges.png)

### 4. BMI vs Insurance Charges

![BMI vs Insurance Charges](images/bmi-vs-charges.png)

### 5. Actual vs Predicted Charges

![Actual vs Predicted Charges](images/actual-vs-predicted.png)

## Model Evaluation

The notebook calculates R² Score, MSE, and RMSE to assess the model's performance on the test dataset.

The evaluation results and the comparison between actual and predicted charges are available in the notebook.

## Project Structure

```text
medical-insurance-cost-prediction/
├── images/
│   ├── charges-distribution.png
│   ├── correlation-heatmap.png
│   ├── age-vs-charges.png
│   ├── bmi-vs-charges.png
│   └── actual-vs-predicted.png
├── medical_insurance_cost_prediction.ipynb
└── README.md
```

## Key Learning Outcomes

- Exploratory Data Analysis
- Data preprocessing and categorical encoding
- Feature engineering
- Multiple Linear Regression
- Regression model evaluation

---
