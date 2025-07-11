# Online_payment_fraud_detection-Using-ML
This project focuses on detecting fraudulent online payment transactions using machine learning, specifically leveraging a Random Forest Classifier enhanced with SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance.

Key Steps in the Workflow:
Data Loading and Preprocessing:

Dataset is loaded using Pandas.

Categorical feature 'type' is one-hot encoded.

Irrelevant columns like 'nameOrig' and 'nameDest' are dropped.

Missing values are handled using SimpleImputer with mean strategy.

Train-Test Split:

The dataset is split into 70% training and 30% testing data.

Handling Class Imbalance with SMOTE:

SMOTE is applied only on the training data to oversample the fraud class.

Model Training:

A Random Forest Classifier with 100 estimators and entropy criterion is trained on the balanced dataset.

Model Evaluation:

Predictions are made on the test set.

Performance metrics including accuracy, precision, recall, and a confusion matrix are used to evaluate the model.

The confusion matrix is visualized using matplotlib.
