# Predictive Modeling for Diabetes
By: Ashley Blake and Rasha Abdalla

![](https://d2jx2rerrg6sh3.cloudfront.net/image-handler/ts/20221215080726/ri/1350/src/images/news/ImageForNews_733883_16711528404605542.jpg)

## Purpose: 
This project aims to develop a machine learning model to predict the likelihood of diabetes based on health indicators from the CDC (Centers for Disease Control and Prevention) dataset. By analyzing various health-related factors, we seek to build a predictive model that can assist healthcare professionals in identifying individuals at higher risk of developing diabetes.

## Introduction and Overview:
Diabetes affects  over 537 million people around the world , making it the deadliest and the most common non‐communicable disease.  According to the American Diabetes Association (ADA), in 2021, 38.4 million Americans, or 11.6% of the population, had diabetes. Additionally, 1.2 Million Americans are diagnosed with Diabetes every year. Early detection plays a pivotal role in managing and mitigating its adverse effects. By employing a robust predictor model, individuals at risk can be identified preemptively, allowing for timely interventions such as lifestyle modifications, dietary adjustments, or medical treatments. Moreover, such a model empowers healthcare providers to prioritize resources efficiently, streamline patient care, and allocate preventive measures to high-risk populations. Furthermore, from a societal perspective, the implementation of a diabetes predictor model can lead to substantial cost savings by reducing healthcare expenses associated with diabetes-related complications and improving overall health outcomes. Therefore, the development and deployment of a diabetes predictor model represent a proactive approach towards promoting public health, enhancing healthcare delivery, and ultimately, fostering a healthier and more resilient population.

## Dataset, Source and Exploration:
We utilized a clean dataset sourced from the UCI Machine Learning Repository, originally compiled from CDC health indicators. The dataset contained 253,680 rows (instances) and 21 columns (features), providing ample data for analysis. Given the dataset's cleanliness and organization, extensive analysis of statistical properties and visualization was not required. Instead, we focused on leveraging the existing dataset to identify pertinent variables for predictive modeling, streamlining the exploratory data analysis process.

* [UCI Machine Learning Repository] (https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)
* [Original CDC Dataset Link] (https://www.cdc.gov/brfss/annual_data/annual_2014.html)


## Model Development:
In the model development phase, we tested three different machine learning algorithms: logistic regression, decision tree, and random forest. Each model underwent data preprocessing, including standardization and train-test splitting, before training and evaluation. Logistic regression was chosen for its simplicity and interpretability, while the decision tree was selected for its ability to handle non-linear relationships. The random forest model was included for its ensemble learning capabilities, which can improve predictive performance by combining multiple decision trees. These models were evaluated based on accuracy, confusion matrix, classification report, and ROC-AUC score to determine their effectiveness in predicting diabetes


## Results:
#### Logistic Regression:

##### Accuracy: Logistic regression achieved an accuracy of 86.59%, indicating that it correctly predicted the likelihood of diabetes in 86.59% of cases.
##### Precision and Recall: It showed a higher precision for the non-diabetic class (precision of 88%) compared to the diabetic class (precision of 55%), indicating that when it predicted an instance as non-diabetic, it was correct 88% of the time. However, the recall (true positive rate) for the diabetic class was low at 17%, indicating that it correctly identified only 17% of the actual diabetic cases. 
##Logistic Regression 
![image](Visualizations/Feature_Importance_LogisticRegression.png)



##### ROC-AUC Score: The ROC-AUC score, which measures the model's ability to distinguish between positive and negative classes, was 0.826, suggesting a good performance.  
![image](Visualizations/LogisticRegression_RocCurve.png) 
##### Mean Squared Error and R-squared: The mean squared error (MSE) was 0.134, and the R-squared (R2) was -0.128, indicating that the model did not fit the data well and had limited predictive power.

#### Confusion Matrix:
![image](Visualizations/Confusion%20Matrix_Decision%20Tree.png)


 
##### Accuracy: The decision tree model achieved an accuracy of 79.86%, which is lower than logistic regression.
##### Precision and Recall: It showed balanced precision and recall scores for both classes, with precision and recall values around 0.30 to 0.34 for the diabetic class and 0.89 to 0.87 for the non-diabetic class.
##### Feature Importance: The decision tree model provided insights into feature importance, indicating which health indicators were most influential in predicting diabetes.
##### Interpretability: Decision trees are interpretable models, allowing for easy understanding of the decision-making process.

## Conclusion:

In conclusion, our analysis of three different machine learning models for predicting diabetes yielded varying levels of performance. The logistic regression model exhibited the highest accuracy at 86.59%, with an ROC-AUC score of 82.64%. However, its performance in correctly identifying individuals with diabetes (precision and recall) was relatively low compared to other models. The decision tree model achieved an accuracy of 79.86% and a ROC-AUC score of 60.28%, indicating moderate predictive capability. On the other hand, the random forest model demonstrated an accuracy of 85.98%, with a slightly lower ROC-AUC score of 80.15%. Although random forest performed better than the decision tree, its precision and recall for identifying diabetes cases were also suboptimal. Overall, while logistic regression showed the highest overall accuracy, it may not be the most effective model for accurately identifying individuals with diabetes. Further refinement and exploration of alternative modeling techniques could enhance the predictive performance of the models and improve diabetes prediction accuracy.
