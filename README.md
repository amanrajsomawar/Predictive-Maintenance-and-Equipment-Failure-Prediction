# Predictive-Maintenance-and-Equipment-Failure-Prediction

## Project Overview

This project develops a Machine Learning model to predict industrial machine failures using the AI4I 2020 Predictive Maintenance Dataset.

The objective is to identify machines that may fail based on their operating parameters, helping industries improve maintenance planning, reduce downtime, and prevent unexpected equipment failures.

## Objectives

- Perform Exploratory Data Analysis (EDA).
- Understand machine operating parameters and failure patterns.
- Preprocess data and prepare features for Machine Learning.
- Train and compare multiple classification algorithms.
- Evaluate model performance using appropriate metrics.
- Identify important features influencing machine failure predictions.
- Develop a reusable prediction function.
- Save and load the trained model using Joblib.

## Dataset

**Dataset:** AI4I 2020 Predictive Maintenance Dataset

The dataset contains 10,000 observations and 14 columns, including:

- Air temperature
- Process temperature
- Rotational speed
- Torque
- Tool wear
- Machine type
- Machine failure
- Individual failure mode indicators

The dataset is used to predict whether a machine will experience failure.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## Project Workflow

1. Data Loading
2. Data Cleaning and Inspection
3. Exploratory Data Analysis
4. Data Visualization
5. Feature Engineering
6. Train, Validation, and Test Split
7. Model Training
8. Model Comparison
9. Threshold Selection
10. Final Model Evaluation
11. Feature Importance Analysis
12. Model Saving and Loading
13. Failure Prediction

## Machine Learning Models

The following classification algorithms were implemented:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

Random Forest achieved the best overall performance among the evaluated models.

## Model Performance

Final Random Forest performance on the test dataset:

| Metric            | Score |
| ----------------- | ----: |
| Accuracy          |   97% |
| Failure Precision |   62% |
| Failure Recall    |   66% |
| Failure F1-score  |  0.64 |

The model detected 45 out of 68 machine failures in the test dataset.

## Feature Importance

The most influential operating parameters identified by the Random Forest model were:

- Rotational speed
- Torque
- Tool wear
- Air temperature
- Process temperature

Rotational speed, torque, and tool wear were the three most important features.

## Model Deployment

The trained Random Forest model was saved using Joblib.

A prediction function was developed to accept machine operating parameters and return:

- Predicted machine status
- Failure probability

This demonstrates how the trained model can be reused for predictive maintenance applications.

## Project Structure

```text
Predictive-Maintenance-and-Equipment-Failure-Prediction/
│
├── data/
│   └── ai4i2020.csv
│
├── model/
│   └── machine_failure_model.pkl
│
├── notebook/
│   └── predictive_maintenance.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Execution

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Navigate to the project folder

```bash
cd Machine-Failure-Prediction
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open `notebooks/predictive_maintenance.ipynb` and run the cells.

## Conclusion

This project demonstrates the application of Machine Learning in predictive maintenance.

By analyzing machine operating parameters and identifying failure patterns, the developed model can help support maintenance decisions and reduce unexpected machine downtime.

## Author
Amanraj Somawar

