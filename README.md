# Telecom Churn Prediction

This repository contains a Python script for predicting customer churn in a telecom company using logistic regression and random forest classifiers. The script performs data preprocessing, model training, and evaluation to determine which model provides better accuracy.

## Requirements

- Python 3.x
- Pandas
- Scikit-learn

You can install the required packages using pip:

```bash
pip install pandas scikit-learn
```

## Data

The script uses two datasets:

- `telecom_demographics.csv`: Contains demographic information of telecom customers.
- `telecom_usage.csv`: Contains usage information of telecom customers.

Ensure these files are located in the same directory as the script.

## Analysis Overview

### Load and Inspect Data

- Loads the demographic and usage datasets.
- Displays basic information and previews of the datasets.

### Merge the Datasets

- Merges the datasets on the `customer_id` column.

### Calculate Churn Rate

- Computes the churn rate as the mean of the `churn` column, representing the proportion of customers who have churned.

### Data Preprocessing

- Identifies and converts categorical variables into dummy/indicator variables.
- Ensures all features are numeric before scaling.
- Applies feature scaling using `StandardScaler`.

### Split the Data

- Splits the data into training and test sets with a test size of 20%.

### Train Models

- Trains a Logistic Regression model and a Random Forest Classifier model on the training data.

### Evaluate Models

- Assesses the accuracy of both models on the test data.
- Compares the accuracy of Logistic Regression and Random Forest Classifier to determine which model performs better.

## Results

- Displays the accuracy of both models.
- Indicates which model has higher accuracy based on the comparison.


Feel free to adjust the content according to any additional details or requirements specific to your project.
