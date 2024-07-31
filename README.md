# Predictive_Maintenance
Implementing Machine Learning Algorithms to detect product breakdown

## Motivation behind the project

Predictive maintenance has emerged as a critical strategy for optimizing asset lifecycles and preventing unplanned downtime across various industries. By leveraging data-driven insights and advanced analytics, organizations can proactively identify potential equipment failures before they occur, leading to significant cost savings and improved operational efficiency.

## Objective

To develop a robust predictive maintenance model capable of accurately predicting equipment failures based on real-time sensor readings.

## Dataset Description

* The dataset consists of 1 categorical feature along with 5 numerical features and 2 target variables.   
* The categorical feature represents the Type of the problem which gives information about the quality about the product.  
* The numerical features contain discrete values representing the properties of the product while the product is actively used.  
* The first target variable represents whether the product is going to fail or not.   
* The second target variable represents the type of failure occurring in the product.

# Methodology

* Data Acquisition:  

  * Dataset Source: https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification

* Data Cleaning:  
  
  * Filling missing values  
  * Eliminating Misleading Data   
  * Eliminating Outliers   

* Data Preprocessing:  
  
  * Feature Encoding  
  * Undersampling  
  * Splitting data into train test sets   
 
* Model Development:
  
  * Choosing the appropriate model.
  * Machine learning is preferred over deep learning Since the data is structured and there are no missing values.
  * For failure prediction, we implemented a binary classification model such as logistic regression and alternatively implemented random forest.
  * For Failure Type Prediction, since it is a multi-class classification problem, we choose to implement XGBoost and LightGBM.
  * Training the model on a portion of the data and evaluating its performance on a separate testing set.

* Evaluation and Analysis:
  
  * Evaluating the model's performance using metrics like accuracy, precision, recall, and F1-score.
  * Analyzing the features with the highest importance scores to understand their role in the classification process.

# Results 

### Failure Prediction
 
Logistic Regression:

![Logistic Regression Classification Report](https://github.com/Shashank-Pericherla/Predictive_Maintenance/blob/main/Results/Logistic%20Regression%20Classification%20Report.png)

Random Forest:

![Random Forest Classification Report](https://github.com/Shashank-Pericherla/Predictive_Maintenance/blob/main/Results/Random%20Forest%20Classification%20Report.png)

ROC Curve of both models:

![AUC-ROC Curve](https://github.com/Shashank-Pericherla/Predictive_Maintenance/blob/main/Results/AUC-ROC%20Curve.png)

### Failure Type Prediction

LightGBM:

![LightGBM Classification Report](https://github.com/Shashank-Pericherla/Predictive_Maintenance/blob/main/Results/LightGBM%20Classification%20Report.png)

XGBoost:

![XGBoost Classification Report](https://github.com/Shashank-Pericherla/Predictive_Maintenance/blob/main/Results/XGBoost%20Classification%20Report.png)


Successfully trained models with great precision, recall and accuracy scores with no signs of overfitting.
