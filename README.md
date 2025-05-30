# Classification-with-Logistic-Regression

Breast Cancer Classification using Logistic Regression
Overview
This project aims to classify breast cancer tumors as malignant or benign using logistic regression. The dataset used for this analysis is the Breast Cancer Wisconsin (Diagnostic) dataset, which contains various features computed from digitized images of fine needle aspirates (FNA) of breast masses. The goal is to build a predictive model that can accurately distinguish between malignant and benign tumors based on these features.

Dataset
The dataset consists of 30 features, including measurements such as radius, texture, perimeter, area, and smoothness of the tumors. The target variable indicates whether a tumor is malignant (1) or benign (0).

Methodology
-Data Loading: The dataset is loaded from a CSV file into a Pandas DataFrame for analysis.
-Data Exploration: Initial exploration of the dataset is performed to understand its structure, including the features and target variable.
-Feature Selection: Specific features are selected for model training, focusing on those that are most relevant to the classification task.
-Data Preprocessing:
  The target variable is encoded if necessary.
  The dataset is split into training and testing sets to evaluate model performance.
  Features are standardized to ensure they have a mean of 0 and a standard deviation of 1.
-Model Training: A logistic regression model is trained on the training dataset.
-Model Evaluation:
  Predictions are made on the test set.
A confusion matrix is generated to assess the model's performance.
Precision and recall metrics are calculated to evaluate the model's effectiveness in identifying malignant tumors.
The ROC-AUC score is computed to measure the model's ability to distinguish between classes.
The ROC curve is plotted to visualize the trade-off between true positive and false positive rates.
Threshold Tuning: The classification threshold is adjusted to optimize precision and recall based on the specific needs of the application.
Results
The results of the model evaluation, including the confusion matrix, precision, recall, and ROC-AUC score, are presented. The ROC curve is also plotted to provide a visual representation of the model's performance.

Conclusion
This project demonstrates the application of logistic regression for binary classification tasks in the medical domain. The findings highlight the importance of feature selection, data preprocessing, and model evaluation in building effective predictive models. Future work may include exploring other classification algorithms, hyperparameter tuning, and implementing cross-validation techniques to enhance model performance.
