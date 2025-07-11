# Online_payment_fraud_detection-Using-ML
This project focuses on detecting fraudulent online payment transactions using machine learning, specifically leveraging a Random Forest Classifier enhanced with SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance.

*🔑 Key Steps in the Workflow*
*1. 📥 Data Loading and Preprocessing*
The dataset is loaded using Pandas.

Categorical feature 'type' is one-hot encoded to convert it into numeric format.

Irrelevant columns such as 'nameOrig' and 'nameDest' are dropped.

Missing values are handled using SimpleImputer with the mean strategy.

*2. ✂️ Train-Test Split*
The dataset is split into 70% training and 30% testing data using train_test_split.

*3. ⚖️ Handling Class Imbalance with SMOTE*
SMOTE (Synthetic Minority Over-sampling Technique) is applied to the training set only.

It oversamples the minority (fraud) class to balance the dataset.

*4. 🌲 Model Training*
A Random Forest Classifier with:

n_estimators=100

criterion='entropy'

random_state=7

The model is trained on the balanced training data (after applying SMOTE).

*5. 📊 Model Evaluation*
The trained model is used to make predictions on the test set.

Evaluation is performed using:

Accuracy

Precision

Recall

Confusion Matrix

The confusion matrix is displayed using Matplotlib for better visualization
