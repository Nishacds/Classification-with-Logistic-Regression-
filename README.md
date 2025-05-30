# Breast Cancer Classification using Logistic Regression with Threshold Tuning and ROC Analysis
This project implements a Logistic Regression model on the Breast Cancer Wisconsin dataset to classify tumors as benign or malignant. Beyond standard model training, it explores threshold tuning for improved performance and uses visual tools like the ROC curve and probability histograms to enhance model understanding.

# Project Highlights
Binary classification using Logistic Regression

Data standardization with StandardScaler

Probability prediction and custom threshold tuning

Evaluation using ROC curve, confusion matrix, precision, and recall

Visualization of predicted probability distributions

# Dataset
We use the Breast Cancer Wisconsin Diagnostic Dataset, available through sklearn.datasets.
Each instance describes characteristics of a cell nucleus derived from digitized images of a fine needle aspirate (FNA) of a breast mass.

Total samples: 569

Features: 30 numeric features (e.g., radius, texture, perimeter, area, smoothness, etc.)

Target classes:

0: Malignant (cancerous)

1: Benign (non-cancerous)

# Libraries Used
scikit-learn
numpy
matplotlib

# Model Workflow
1. Load and Explore Dataset
Load the Breast Cancer dataset using sklearn.datasets.
Check data shape, class distribution.

2. Data Preprocessing
Perform a train-test split (80% train, 20% test) with stratification to preserve class balance.
Standardize features using StandardScaler.

3. Logistic Regression
Train a LogisticRegression model.
Predict class probabilities (predict_proba) on test set.

4. Evaluation
# ROC Curve
Plot ROC curve using roc_curve and roc_auc_score to evaluate classification performance at all thresholds.

# Threshold Tuning
Use custom thresholds (e.g., 0.2, 0.3, 0.5, 0.7) instead of default 0.5 to classify based on predicted probabilities.
Measure:
- Precision
- Recall
- Confusion Matrix
Tune to meet specific business or healthcare priorities (e.g., higher recall to avoid missing malignant cases).

# Probability Distribution Plot
- Histogram showing predicted probability distribution per class.
- Helps visually select an appropriate decision threshold.

# Visualizations Included
ROC Curve
- Displays true positive rate vs false positive rate for various thresholds.

Probability Histogram
- Shows distribution of predicted probabilities.
- Helps understand how confident the model is in its predictions.

Confusion Matrices at Tuned Thresholds
- Display model performance for multiple manually selected thresholds.

# Key Learnings
- Logistic Regression is powerful and interpretable for binary classification tasks.
- Threshold tuning can drastically affect model precision and recall.
- Visual tools like ROC curves and probability distributions aid in informed threshold selection.
- Understanding sigmoid output is key to working with classification probabilities.
