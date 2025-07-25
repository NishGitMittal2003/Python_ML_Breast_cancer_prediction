# Breast Cancer Prediction using Machine Learning

This project focuses on building a predictive model for breast cancer classification using a dataset of features extracted from digitized images of fine needle aspirate (FNA) of breast masses. The goal is to classify tumors as **Malignant (M)** or **Benign (B)** using machine learning algorithms.

## Dataset Overview

The dataset consists of **569 samples** with **30 numeric features** that describe characteristics of the cell nuclei present in the image. It includes measurements like:

- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Symmetry
- Fractal Dimension

The target variable is the **diagnosis** (`M` = malignant, `B` = benign).

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Data Preprocessing

- Removed unnecessary columns (`id`, `Unnamed: 32`)
- Verified and handled missing values (none present)
- Exploratory Data Analysis (EDA) with bar plots, heatmaps, and correlation matrices
- Feature-target separation for training and testing

## Models Implemented

### 1. Decision Tree Classifier
- Trained using `sklearn.tree.DecisionTreeClassifier`
- Accuracy: **93.5%**

### 2. Logistic Regression
- Trained using `sklearn.linear_model.LogisticRegression`
- Accuracy: **97.0%**
- Logistic Regression outperformed Decision Tree based on recall and generalization

## Evaluation Metrics

- Accuracy
- Confusion Matrix (not shown but implied)
- Precision, Recall (focus on recall for medical diagnosis)
- Model comparison based on actual vs. predicted values

## Conclusion

While both models performed well, **Logistic Regression** achieved higher accuracy and recall, making it a more reliable choice for early detection and diagnosis of breast cancer.


