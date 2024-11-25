# KNN
# Cancer Diagnosis Prediction Using Machine Learning
This project uses various machine learning techniques to classify cancer diagnoses as malignant or benign based on a comprehensive dataset. The goal is to identify the most effective machine learning model for accurate and reliable predictions, making strides toward early detection and improved outcomes in cancer diagnostics.

### Table of Contents
1. Overview
2. Dataset
3. Data Preprocessing
4. Exploratory Data Analysis (EDA)
5. Modeling
6. Evaluation
7. Technologies Used

### Overview
Early detection of cancer is critical to patient survival and treatment success. This project applies machine learning algorithms to classify tumors based on a range of diagnostic measurements. It evaluates models such as K-Nearest Neighbors (KNN), Naive Bayes, and Support Vector Machines (SVM) to determine the most effective classifier.

### Key Goals:

Build a robust and scalable pipeline for data preprocessing, training, and evaluation.
Leverage cross-validation to enhance model reliability.
Visualize data relationships and identify correlations between features.

### Dataset
The dataset used in this project was obtained from Kaggle:
Cancer Data

 Features:

Numerical measurements of tumor properties (e.g., radius, texture, perimeter).
A categorical target variable: diagnosis (M for malignant, B for benign).

### Data Preprocessing
Loading and Cleaning Data:

 Removed unnecessary columns (Unnamed: 32 and id).
Addressed missing or null values (if applicable).
Feature Selection:

Retained only numerical columns for analysis.
Extracted the target column (diagnosis) for classification.
Train-Test Split:

Data split into 80% training and 20% testing subsets.

### Exploratory Data Analysis
Correlation Heatmap:
Visualized feature correlations using a heatmap to identify the most relevant predictors for diagnosis.

### Modeling
Models Implemented:
K-Nearest Neighbors (KNN):

Parameters: n_neighbors=5, weights='uniform'.
Achieved a mean accuracy of 96.04%.
Naive Bayes (GaussianNB):

Integrated with a standardized pipeline.
Achieved a mean accuracy of 93.41%.
Support Vector Machine (SVM):

Parameters: C=0.9, kernel='poly', degree=5, class_weight='balanced'.
Achieved a mean accuracy of 95.82%.

### Evaluation
Cross-validation was used to ensure robust model performance across multiple folds. KNN emerged as the most accurate model, demonstrating its effectiveness for this dataset.

Model	Mean Accuracy (%)
K-Nearest Neighbors (KNN)	96.04
Naive Bayes (GaussianNB)	93.41
Support Vector Machine (SVM)	95.82

### Technologies Used
Programming Language: Python
Libraries:
pandas, numpy for data manipulation
matplotlib, seaborn for visualization
scikit-learn for machine learning
