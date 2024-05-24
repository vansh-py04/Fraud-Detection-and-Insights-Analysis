# Fraud-Detection-and-Insights-Analysis
Data Source: The dataset can be found [here](https://drive.google.com/uc?export=download&confirm=6gh6&id=1VNpyNkGxHdskfdTNRSjjyNa5qC9u0JyV).

## Description

For the fraud detection model, we typically use supervised learning algorithms suited for classification tasks. Here’s an example using a Random Forest Classifier:

Model Choice: Random Forest was chosen due to its robustness and ability to handle imbalanced datasets and its capability of providing feature importance scores.

Data Preparation: The dataset was split into training and validation sets, and SMOTE was used to handle class imbalance.

Feature Engineering: New features were created to capture potential patterns indicative of fraud.

Model Training: The model was trained on the resampled training set.

Evaluation: The model was evaluated using precision, recall, F1-score, and AUC-ROC.

Model Precision : 

![image](https://github.com/vansh-py04/Fraud-Detection-and-Insights-Analysis/assets/128248352/a5d2b330-98a5-4aec-ab9f-4f74eb356531)
