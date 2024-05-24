# Fraud-Detection-and-Insights-Analysis
Data Source : The dataset can be found [here](https://drive.google.com/uc?export=download&confirm=6gh6&id=1VNpyNkGxHdskfdTNRSjjyNa5qC9u0JyV).

## Description

For the fraud detection model, we typically use supervised learning algorithms suited for classification tasks. Here’s an example using a Random Forest Classifier:

Model Choice: Random Forest was chosen due to its robustness and ability to handle imbalanced datasets and its capability of providing feature importance scores.

Data Preparation: The dataset was split into training and validation sets, and SMOTE was used to handle class imbalance.

Feature Engineering: New features were created to capture potential patterns indicative of fraud.

Model Training: The model was trained on the resampled training set.

Evaluation: The model was evaluated using precision, recall, F1-score, and AUC-ROC.

## Model Precision

![image](https://github.com/vansh-py04/Fraud-Detection-and-Insights-Analysis/assets/128248352/14ec23e6-6f46-4bad-9469-5e4ed54d03a5)



## Gained Insights 1:

-> Pattern of Fraudulent Transactions: It has been observed that fraudulent transactions often occur in pairs. Specifically, a fraudulent transfer is followed immediately by a corresponding cash-out transaction.

-> Transaction Consistency: For instance, if there is a transfer transaction (T1) of a certain amount, such as 181, it is immediately followed by a cash-out transaction of the same amount.

## Proposition

-> Timing and Amounts: Monitoring the timing and amounts of transactions can provide further insights. Transactions occurring in quick succession, especially for the same amount, should be flagged for further investigation.

-> Structured Fraud Behavior: The consistent pairing of transfer and cash-out transactions indicates a structured and deliberate pattern of fraud. Fraudsters seem to transfer funds and then quickly withdraw them, aiming to minimize the risk of detection and maximize the speed of asset liquidation.

## Gained Insights 2:

-> Initiation of Fraudulent Transactions: Every fraudulent transaction starts from a customer account, denoted by 'C'. This means that the initial transfer in a fraudulent sequence always originates from a customer account.

-> Recipient Accounts: The recipients of these fraudulent transactions are also customer accounts, denoted by 'C'.

## Proposition

-> Originating Account Type: Knowing that fraudulent transactions always start from customer accounts provides a key focal point for fraud detection systems. Enhanced monitoring and security measures can be implemented specifically for transactions initiated by customer accounts.

-> Uniformity in Recipient Accounts: Since both the initiators and recipients of fraudulent transactions are customer accounts, fraud detection systems can be fine-tuned to monitor customer-to-customer transactions more closely. This uniformity simplifies the detection rules and focuses the analysis on a specific subset of transactions.
