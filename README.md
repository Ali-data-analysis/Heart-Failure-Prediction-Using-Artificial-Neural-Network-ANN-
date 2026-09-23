# Heart-Failure-Prediction-Using-Artificial-Neural-Network-ANN-

## Project Overview

Cardiovascular diseases (CVDs) are among the leading causes of death worldwide. Heart failure is a serious cardiovascular condition in which the heart is unable to pump sufficient blood to meet the body's requirements.

This project focuses on developing a Machine Learning / Deep Learning classification model using an Artificial Neural Network (ANN) to predict the occurrence of a death event among patients with heart failure based on clinical characteristics.

The project covers the complete data science workflow, including:

- Data loading and exploration
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Feature analysis
- Artificial Neural Network model development
- Model training and validation
- Performance evaluation
- Confusion matrix analysis

> **Note:** This project is intended for educational and machine-learning demonstration purposes and should not be used as a clinical diagnostic system.

---

## Problem Statement

The objective is to build a binary classification model that predicts whether a patient experienced a death event based on clinical and demographic features.

### Target Variable

`DEATH_EVENT`

- `0` → Patient survived
- `1` → Patient experienced a death event

---

## Dataset

The dataset contains clinical information about patients with heart failure.

Important features used in the analysis include:

- Age
- Creatinine Phosphokinase
- Ejection Fraction
- Platelets
- Serum Creatinine
- Serum Sodium
- Time

### Feature Description

| Feature | Description |
|---|---|
| `age` | Age of the patient |
| `creatinine_phosphokinase` | Level of creatinine phosphokinase in the blood |
| `ejection_fraction` | Percentage of blood leaving the heart during each contraction |
| `platelets` | Platelet count |
| `serum_creatinine` | Serum creatinine level |
| `serum_sodium` | Serum sodium concentration |
| `time` | Follow-up period |
| `DEATH_EVENT` | Target variable |

---

# Project Workflow

## 1. Importing Libraries

The project uses Python libraries for data analysis, visualization, and deep learning.

Main libraries include:

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras

---

## 2. Loading Data

The dataset is loaded using Pandas and inspected to understand:

- Dataset dimensions
- Data types
- Missing values
- Statistical characteristics
- Target distribution

---

## 3. Exploratory Data Analysis

EDA was performed to understand the relationship between clinical features and the target variable.

### Visualizations

The analysis includes:

- Box plots
- Swarm plots
- Feature distributions
- Target-class distributions
- Correlation analysis
- Training and validation accuracy
- Confusion matrix

### Feature Distribution

The box and swarm plots show the distribution of important clinical variables across the two `DEATH_EVENT` classes.

 

---

## 4. Data Preprocessing

The preprocessing stage includes preparing the dataset for neural-network training.

Major steps include:

- Feature selection
- Separating independent and dependent variables
- Train-test splitting
- Feature scaling
- Preparing data for ANN training

Feature scaling is particularly important for neural networks because the input variables have very different numerical ranges.

---

# 5. Artificial Neural Network Model

An Artificial Neural Network was developed for binary classification.

The ANN learns patterns from the clinical features and predicts the probability of a death event.

The model training process includes:

- Input features
- Dense neural-network layers
- Activation functions
- Binary classification output
- Model optimization
- Validation during training

---

# 6. Model Performance

## Training and Validation Accuracy

The training and validation accuracy curves were monitored across epochs to understand model learning behavior.
 

The model reaches approximately the low-to-mid 80% accuracy range during later training epochs, while validation accuracy remains relatively stable.

This indicates that the model is learning useful patterns from the available features, although some variation between training epochs is visible.

---

## Confusion Matrix

The normalized confusion matrix was used to evaluate the classification performance of the ANN.

 

The displayed normalized values are approximately:

| | Predicted 0 | Predicted 1 |
|---|---:|---:|
| Actual 0 | 0.65 | 0.11 |
| Actual 1 | 0.08 | 0.16 |

Where:

- **True Negative (TN):** 0.65
- **False Positive (FP):** 0.11
- **False Negative (FN):** 0.08
- **True Positive (TP):** 0.16

Based on the displayed normalized confusion matrix, the model correctly classifies a substantial proportion of both classes.

---

# 7. Key Observations

The analysis provides several useful observations:

- Clinical features show different distributions between survival classes.
- `ejection_fraction`, `serum_creatinine`, `age`, and `time` show noticeable differences between the two target classes.
- Some features contain outliers and considerable variation.
- Feature scaling is important before ANN training.
- The ANN achieves approximately 80%+ classification accuracy based on the displayed evaluation results.
- The confusion matrix provides a clearer view of correct and incorrect predictions for each class.

---

# 8. Technologies Used

### Programming Language
- Python

### Data Analysis
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn

### Deep Learning
- TensorFlow
- Keras
- Artificial Neural Networks (ANN)
