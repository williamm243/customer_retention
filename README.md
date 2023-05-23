# Overview

This project uses machine learning algorithms to build a model that can accurately predict customers who will churn based on the information available in the dataset. The dataset has 20 predictor variables mostly about customer usage patterns. There are 3333 records in this dataset, out of which 483 customers are churners and the remaining 2850 are non-churners. The target variable is 'churn'. Since the target variable is a categorical variable, classification algorithms are used to build the predictive model. Recall is used to evaluate the model's performance.

# Business and Data Understanding

The stakeholder for this project is the company itself that aims to reduce churning and increase profits.
using the dataset of churning of customers we aim to buld the best possible classification model to decrease losses through loss of customers.
Data is in csv format it contains 3333 unique rows 

# Modeling
created different machine learning classification model to classify the probability of churn.
among the models created were;
                                - logistic regression model(base model)
                                - k-Nearest-Neighbors
                                - Decision tree classifier
                                - random forest

# Evaluation
for evaluation of our model we used a classification matrix to measure how our different models were performming.
for this project i choose my classification matrix  to  be Recall (Sensitivity or True Positive Rate):

- Recall measures the proportion of actual churned customers that are correctly identified as churned by the model. In this model it is crucial to capture as many churned customers as possible to take appropriate actions. Therefore, maximizing recall is often important to minimize false negatives churned customers classified as non-churned.

- The aim is to maximize recall
 -   In the logistic model, the recall for customers who did not churn is 97%, and 22% for customer who churned
    - this model is performing poorly.
- In the knn model, the recall for customers who did not churn is 99%, and 29% for customer who churned
       - this model is an improvemet of the baseline model but still the recall is low.
- In the Decision tree model, the recall for customers who did not churn is 99%, and 66% for customer who churned
       -  this is a strong model for predicting
- In the Random forest classifier, the recall for customers who did not churn is 99%, and 65% for customer who churned
       -  this model is strong but the model before

# conclusion
From our EDA we notice that the data is imbalanced where 86% of the customers did not churn

- Only 10% of people are subscribed to international plan

- 72% of people are not subscribed to voice mail

- 137 people who were enrolled in international plan churned

- 403 people with no voice mail churned

- all numerical features are normally distributed apart from churn

- There is multicollinearlity between:

 1 - total day charge and total day minutes

 2 - total eve charge and total eve minutes 
            
 3 - total intl charge and total intl minutes 

 4 - total night charge and total night minutes

- the best features are for model building are:
                        *customer service calls
                        * international plan
                        * Total day charge


