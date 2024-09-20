# Credit-Card-Fraud-Detection

1. Project Overview
The project focuses on detecting fraudulent credit card transactions using machine learning. Credit card fraud detection is a critical issue for financial institutions, as fraudulent transactions cause significant financial loss and damage to customer trust. The project aims to develop a model that effectively distinguishes between legitimate and fraudulent transactions, considering the severe class imbalance inherent in the data.

      2.    Business Understanding   
The primary objective is to accurately detect fraud transactions in a dataset where the number of fraudulent transactions is much smaller than the number of legitimate ones. Key business questions include:
- What time do credit card frauds usually occur?
- What are the general trends of transaction amounts for fraudulent transactions?
- How can the data be balanced to prevent the model from overfitting on legitimate transactions?

     3.    Data Understanding   
The dataset used is sourced from Kaggle's Credit Card Fraud Detection dataset. The key points about the data are:
- It includes 32 features, from V1 to V28, along with `Time`, `Amount`, and `Class`.
- Features V1-V28 are anonymized for confidentiality.
- The target variable is `Class`, with values:
  - `0`: Legitimate Transaction
  - `1`: Fraud Transaction
- The dataset does not contain missing values and consists of purely numerical features.

     4.    Data Preprocessing   
-    Scaling:    Data features were standardized using scaling techniques to ensure all features are on a comparable scale, enhancing the performance of machine learning algorithms.
-    Balancing Data:    Due to the imbalanced nature of the dataset, techniques like Synthetic Minority Over-sampling Technique (SMOTE) were used to balance the class distribution and prevent the model from being biased towards legitimate transactions.

     5.    Model Development   
Several machine learning models were developed and evaluated:
-    Logistic Regression   
-    Support Vector Machine (SVM)   
-    K-Nearest Neighbors (KNN)   
-    Decision Tree Classifier   
-    Random Forest Classifier   
-    Stochastic Gradient Descent (SGD) Classifier   

These models were evaluated based on various performance metrics, including precision, recall, F1-score, and ROC-AUC score.

     6.    Model Evaluation and Selection   
-    Cross-Validation:    Techniques like K-Fold and Stratified K-Fold cross-validation were used to ensure robust model evaluation.
-    Metrics:    The models were primarily evaluated using the Matthews Correlation Coefficient (MCC), precision, recall, and F1-score to account for the imbalance in the data.
-    Hyperparameter Tuning:    Grid Search CV was employed for hyperparameter optimization to improve model performance.

     7.    Results and Conclusions   
- The best-performing model was selected based on evaluation metrics, balancing accuracy, and the ability to correctly identify fraud without overwhelming false positives.
- The report concludes with recommendations for deploying the model and strategies for continuous monitoring to adapt to evolving fraud patterns.
