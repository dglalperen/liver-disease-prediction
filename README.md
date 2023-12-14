# Indian Liver Patient Classification Project

## Overview

This project focuses on developing a machine learning model to classify patients with liver disease using the Indian Liver Patient Dataset. The primary goal is to accurately identify characteristics that contribute to liver disease and predict patient outcomes.

## Dataset

The dataset used in this project is the "Indian Liver Patient Dataset," which contains various medical measurements. It's located in `data/raw_data/indian_liver_patient.csv`.

## Structure

- **data/**
  - **raw_data/**: Contains the dataset in CSV format.
- **notebooks/**
  - **main.ipynb**: The Jupyter Notebook containing the analysis and model building.

## Features

The dataset includes several features related to liver function tests and patient demographics. Key features include Total Bilirubin, Direct Bilirubin, Alkaline Phosphatase, and others.

## Methodology

The analysis follows these steps:

1. **Data Preprocessing**: Includes encoding categorical variables, handling missing values, and removing duplicates.
2. **Exploratory Data Analysis (EDA)**: Visualizing data distribution and understanding feature relationships.
3. **Feature Engineering**: Selecting important features based on correlation with the target variable.
4. **Handling Class Imbalance**: Using `RandomOverSampler` to balance the dataset.
5. **Feature Importance Visualization**: Employing `RandomForestClassifier` and Yellowbrick's `FeatureImportances` for feature significance.
6. **Model Building**: Creating a stacking classifier with base models (Random Forest, Gradient Boosting, and Extra Trees Classifier) and a meta-model (Logistic Regression).
7. **Model Evaluation**: Using cross-validation and metrics like accuracy, precision, recall, F1 score, and ROC-AUC for performance assessment.

## Running the Project

To run this project:

1. Clone the repository.
2. Ensure you have Jupyter Notebook installed.
3. Navigate to the `notebooks/` directory.
4. Open `main.ipynb` in Jupyter Notebook.
5. Run the cells in the notebook to perform the analysis and model training.

## Requirements

- Python 3.x
- Libraries: `numpy`, `pandas`, `sklearn`, `imblearn`, `seaborn`, `matplotlib`, `xgboost`, `yellowbrick`

## Contributions

Feel free to fork this project, submit issues, and open pull requests to contribute improvements or additional features.
