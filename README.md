# Claim-prediction-for-Insurance-firm

## Problem Statement:
An Insurance firm providing tour insurance is facing higher claim frequency. The management decides to collect data from the past few years. The task is to make a model which predicts the claim status and provide recommendations to management.

## Approach:
Using CART, Random Forest & Artificial Neural Networks. Comparing the models performances in train and test sets.

## EDA and Data Pre-prossessing:
Exploratory data analysis was done with null value checks and data duplication checks:
Univariate and Bivariate data analysis was performed to understand the correlation and spread of the data.

## Model Building:
Data was split into training and testing sets. Models were trained on Desision tree, Random Forest and Artificial Neural Network algorithms.

## Model Optimization and Hyperparameter tuning:
The trained models were optimized using automated hyperparameter tuning using param grid and grid search techniques.

## Model Evaluation:
Performance of model Predictions on Train and Test sets done using Accuracy, Confusion Matrix, Plot ROC curve and getting ROC_AUC score for each model.

### Decision Tree Classifier performance:
Train Data:
AUC: 81.0%
Accuracy: 78.28%
Sensitivity: 58%
Precision: 66%
f1-Score: 62%

Test Data:
AUC: 81.5%
Accuracy:79.55%
Sensitivity: 58%
Precision: 73%
f1-Score: 64%

Training and Test set results are almost similar, and with the overall measures high, the model is a good model.
Agency Code is the most important variable for predicting Claim Status

### Random Forest Model performance:
Train Data:
AUC: 82.5%
Accuracy: 77.85%
Sensitivity: 51%
Precision: 68%
f1-Score: 58%

Test Data:
AUC: 83.7%
Accuracy:78.66%
Sensitivity: 51%
Precision: 74%
f1-Score: 61%

Training and Test set results are almost similar, and with the overall measures high, the model is a good model.
Agency Code is the most important variable for predicting Claim Status

### Artificial Neural Networks performance:
Train Data:
AUC: 82.0%
Accuracy: 78.38%
Sensitivity: 51%
Precision: 70%
f1-Score: 59%

Test Data:
AUC: 82.9%
Accuracy: 79%
Sensitivity: 52%
Precision: 75%
f1-Score: 61%

Training and Test set results are almost similar, and with the overall measures high, the model is a good model.

## Overall Conclusion:
Out of the 3 models, Artificial Neural Networks has slightly better performance than the CART and Random Forest.

If we consider Recall as an imp factor, decision tree classifier has better results compared to the other two.

Overall all the 3 models are reasonaly stable enough to be used for making any future predictions.
From Cart and Random Forest Model, the variable change is found to be the most useful feature amongst all other features for predicting if a person has diabetes or not. If change is yes, then those patients have more chances of getting diabetes.

## Inference of Analysis:
Inference based on these predictions, these are the business insights and recommendations:

From the Decision Tree and Random Forest predicive models, we found that the variable 'Agency' is contributing the most when it comes to prediction.
So, the company should investigate further and check which are the agencies having higher claim rate.

Sales and the Product name are the other two variables which are important variables in contributing to the predictions.
The company need to investigate the products and find the products from which the claims are higher.

we may recommend to take safety measures and help prevent any loss or damage which would help in reducing the claims.
The feature importance for variables Age, Destination and Channel are almost 0 or negligible.
These variables are not contributing much for the predictions.
We may choose not to consider these variables in our predictions.

### Please check the ipynb file for full code and detailed analysis
