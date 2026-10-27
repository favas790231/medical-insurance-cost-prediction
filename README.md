# Medical Insurance Cost Prediction Using Multiple Linear Regression

## Overview

This project uses Multiple Linear Regression to predict individual medical insurance charges based on personal and lifestyle-related features.

The project includes Exploratory Data Analysis (EDA), data preprocessing, feature engineering, model training, and evaluation using Python and Scikit-learn.

## Dataset

The dataset used in this project is the Medical Cost Personal Dataset from Kaggle.

- **Source:** [Medical Cost Personal Dataset – Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance)
- **Total Records:** 1,338
- **Total Columns:** 7
- **Target Variable:** `charges`

### Features

| Feature | Description |
|---|---|
| age | Age of the individual |
| sex | Gender of the individual |
| bmi | Body Mass Index |
| children | Number of dependent children |
| smoker | Smoking status |
| region | Residential region |
| charges | Individual medical insurance charges |

The dataset CSV file is not included in this repository. Please refer to the original dataset page for its current licensing and usage terms.

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. **Data Inspection:** Examined the dataset structure, data types, and missing values.
2. **Exploratory Data Analysis:** Analyzed feature distributions and relationships between variables and insurance charges.
3. **Data Preprocessing:** Converted categorical variables into numerical representations using one-hot encoding.
4. **Feature Engineering:** Created an interaction feature between age and smoking status.
5. **Model Training:** Trained a Multiple Linear Regression model using Scikit-learn.
6. **Model Evaluation:** Evaluated the model using R² Score, Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

## Visualizations

### 1. Distribution of Medical Insurance Charges

Examines the distribution of insurance charges and identifies the overall spread of medical costs.

![Distribution of Medical Insurance Charges](images/charges-distribution.png)

### 2. Correlation Heatmap

Visualizes correlations between numerical features and helps explore relationships within the dataset.

![Correlation Heatmap](images/correlation-heatmap.png)

### 3. Age vs. Insurance Charges

Explores the relationship between an individual's age and their medical insurance charges.

![Age vs Insurance Charges](images/age-vs-charges.png)

### 4. BMI vs. Insurance Charges

Examines the relationship between Body Mass Index (BMI) and medical insurance charges.

![BMI vs Insurance Charges](images/bmi-vs-charges.png)

### 5. Actual vs. Predicted Charges

Compares actual insurance charges with the values predicted by the Multiple Linear Regression model.

![Actual vs Predicted Charges](images/actual-vs-predicted.png)

## Model Evaluation Results

The Multiple Linear Regression model was evaluated using the test dataset.

| Evaluation Metric | Result |
|---|---:|
| R² Score | 0.807 |
| RMSE | 5,939 |

- **R² Score:** Indicates how much of the variation in medical insurance charges is explained by the model.
- **RMSE:** Measures the typical scale of prediction errors in the same units as the target variable, `charges`.

The model explains approximately 80.7% of the variation in medical insurance charges on the evaluated test dataset.

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

- Performed Exploratory Data Analysis on a real-world dataset.
- Practiced data preprocessing and categorical variable encoding.
- Applied feature engineering to create an interaction feature.
- Built a Multiple Linear Regression model using Scikit-learn.
- Evaluated regression performance using standard evaluation metrics.
- Visualized relationships between features and model predictions.
