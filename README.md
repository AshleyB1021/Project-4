# Diabetes Prediction Project

## Introduction:
Diabetes affects  over 537 million people around the world , making it the deadliest and the most common non‐communicable disease.  According to the American Diabetes Association (ADA), in 2021, 38.4 million Americans, or 11.6% of the population, had diabetes. Additionally, 1.2 Million Americans are diagnosed with Diabetes every year.


## Overview:
This project aims to develop a machine learning model to predict the likelihood of diabetes based on health indicators from the CDC (Centers for Disease Control and Prevention) dataset. By analyzing various health-related factors, we seek to build a predictive model that can assist healthcare professionals in identifying individuals at higher risk of developing diabetes.


## Data Exploration:
The data exploration process involved analyzing the dataset's structure, contents, and statistical properties. Descriptive statistics, visualizations, and exploratory data analysis techniques were used to gain insights into the dataset and identify relevant variables for predictive modeling.

## Model Development:
In the model development phase, we tested two different machine learning algorithms: linear regression and decision tree. Each model underwent data preprocessing, including standardization and train-test splitting, before training and evaluation. 


## Results:
The trained models achieved promising results, each demonstrating unique strengths and limitations. The linear regression model achieved an accuracy of 86.59%, with an ROC-AUC score of 0.826. However, it exhibited limitations in capturing non-linear relationships, resulting in lower precision and recall for predicting positive cases (diabetes). On the other hand, the decision tree model achieved an accuracy of 79.86%, with an ROC-AUC score of 0.603. While the decision tree model showed improved performance in capturing non-linear relationships, it had lower overall accuracy compared to the linear regression model. 

## References:

### Dataset

https://www.cdc.gov/brfss/annual_data/annual_2014.html

https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset

### (American Diabetes Association)

https://diabetes.org/about-diabetes/statistics/about-diabetes#:~:text=Overall%20numbers,of%20the%20population%2C%20had%20diabetes.&text=Diagnosed%20and%20undiagnosed%3A%20Of%20the,and%208.7%20million%20were%20undiagnosed.
