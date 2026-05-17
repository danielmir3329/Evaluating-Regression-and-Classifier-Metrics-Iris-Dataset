# Evaluating Regression and Classification Metrics Using the Iris Dataset

## Overview

This project evaluates simple regression and classification estimators using the Iris dataset in Python. The assignment focuses on foundational machine learning concepts including feature engineering, train/test splitting, regression evaluation metrics, classification metrics, and model interpretation.

The project was completed using Python, pandas, NumPy, scikit-learn, seaborn, and matplotlib inside a Jupyter Notebook environment.

---

## Project Objectives

- Load and explore the Iris dataset
- Perform feature engineering
- Split data into training and testing datasets
- Evaluate regression estimators using error metrics
- Evaluate classification estimators using classification metrics
- Interpret model performance
- Compare regression and classification approaches

---

## Dataset

The project uses the built-in Iris dataset from `sklearn.datasets`.

### Features
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

### Target Variable
- Iris flower type:
  - Setosa
  - Versicolor
  - Virginica

---

## Feature Engineering

A custom engineered feature was created using:

```python
(sepal_length * sepal_width) / (petal_length * petal_width)
```

This demonstrates how new variables can be created from existing measurements to potentially improve predictive analysis.

---

## Regression Analysis

Two simple regression estimators were evaluated for predicting sepal width:

### Estimator 1
- Mean of petal length

### Estimator 2
- Mean of sepal length minus petal width

### Regression Metrics Used
- Mean Error (ME)
- Mean Percentage Error (MPE)
- Mean Absolute Percentage Error (MAPE)
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)

### Results

Estimator 1 performed better overall because it produced lower error values across all evaluation metrics.

---

## Classification Analysis

Two rule-based classifiers were evaluated for predicting flower type using percentile thresholds based on sepal length.

### Classifier 1
- 25th percentile
- 50th percentile

### Classifier 2
- 50th percentile
- 75th percentile

### Classification Metrics Used
- Accuracy
- Precision
- Recall
- F1 Score

### Results

Classifier 2 achieved better classification performance with higher accuracy and F1 scores.

---

## Visualizations

The notebook includes:
- Scatterplots
- Boxplots
- Confusion matrices
- Summary statistics

These visualizations help explore feature relationships and evaluate model performance.

---

## Technologies Used

- Python
- Jupyter Notebook
- pandas
- NumPy
- scikit-learn
- seaborn
- matplotlib

---

## Key Concepts Demonstrated

- Supervised Learning
- Regression
- Classification
- Feature Engineering
- Train/Test Splitting
- Model Evaluation
- Error Metrics
- Performance Interpretation

---

## Future Improvements

Potential improvements include implementing more advanced machine learning algorithms such as:

- Linear Regression
- Logistic Regression
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machines (SVM)

These approaches could improve prediction accuracy by learning more complex patterns from all available features.
