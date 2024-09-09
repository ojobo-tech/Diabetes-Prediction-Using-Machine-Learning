# Diabetes-Prediction
The project involves the prediction of diabetes in an individual based on their social, demographic and health status. Machine learning models were created to test the classification, and were assessed based on their accuracy, sensitivity and area under curve.

# Dataset
https://drive.google.com/file/d/1R-I9jiGWQMDjUIgOOP8v6g_qfZXTs6H0/view?usp=sharing

# Code Description
  1. Data Loading and Preprocessing: Four CSV files are loaded, combined, and cleaned. This includes handling missing values, normalization, and encoding categorical features.

  2. Data Splitting: The data is split into training, validation, and test sets.

  3. Model Training: Several machine learning models (Logistic Regression, K-Nearest Neighbors, Decision Tree, Random Forest, XGBoost) are trained using GridSearchCV for hyperparameter tuning.

  4. Model Evaluation: The models are evaluated on the test data using metrics such as accuracy, precision, recall, and F1-score.

# Requirements
You should have a programming software like Python, using libraries pandas: numpy, sciki-learn, matplotlib

# Project Findings
The study analyzed data comprising 129,024 individuals, including 21,303 with type 2 diabetes, from the Center for Disease Control, 2014 Behavioral Risk Factor Surveillance System, annotated with variables including BMI, age, exercise frequency, smoking status, sleep duration, socioeconomic status (SES), healthcare access, and geographical factors. The data was split into 80% training and 20% testing sets.

Six Machine Learning models (Logistic Regression, Gaussian Naive Bayes, Random Forest, Gradient Boosting, Neural Network and Decision Trees) were trained, and their performances were compared based on accuracy, sensitivity, specificity, and the Area Under Curve (AUC). Feature importance analysis was conducted to identify the most predictive variables.

The predictive models used achieved a high area under the curve (AUC ranging from 0.69 to 0.81). However, the Gradient Boosting Model (GBM) and Neural Network outperformed others with similar results of accuracy of 0.86 and 0.85 respectively, specificity of 0.99, and AUC of 0.81. The Gaussian Naive Bayes model presented a balanced sensitivity-specificity trade-off (Accuracy: 0.80, Sensitivity: 0.43, Specificity: 0.87, AUC: 0.75) but fell short in overall accuracy and AUC compared to Gradient Boosting and Neural Network. This study highlighted that people who are unable to work (Coef = 0.5649), or who had a Health Care Coverage with the Alaska Native/Indian Health Service (Coef = 0.6096), or who have not had a medical checkup in the last 5 years or more (Coef =-1.0077) have higher risk for type 2 diabetes.

