# Google_Advanced_DA_Capstone_Project

### Introduction:
This repository contains the capstone project from Google Advanced Data Analytics. It provides analysis of the Human Resources (HR) department of Salifort Motors firm. 
I built a predictive model to anticipate employee attrition, a critical concern for organizations. This presentation outlines the model's performance metrics and discusses its potential impact on identifying employees likely to leave.

##### Statistical analysis

I performed Hypothesis tests to find out why employees leave

- Null Hypothesis (H0): There is No significant difference in the means of the variables of employees left the company and employees that did not leave the company.
- Alternative Hypothesis (H1): There is a significant difference in the means of the variables of employees left the company and employees that did not leave the company.
- The significance level was choosen to be 0.05

###### Result summary, based on the t-test results:

Variables like "satisfaction_level," "number_of_project," "average_monthly_hours," and "time_spent_in_company" show statistically significant differences between employees who left and those who stayed.
The "last_evaluation" variable does not show a statistically significant difference between the two groups.

###### Result summary, based on the chi-square test and ANOVA results:

Variables like "work_accident", "promotion_in_last_5years" and "Salary" all show statistically significant differences between employees who left and those who stayed.


##### ML Training and Performance Metrics:
After label Encoding, checking for class imballance, spliting the data into train, test set with stratification, I trainde a Random Forest classsifier model with 10 k-fold cross validation

###### Summary of results
- Accuracy: 98.46%: This metric indicates the overall correctness of predictions. A high accuracy rate suggests that the model is proficient at distinguishing between staying and leaving employees.

- Precision: 97.88%: Precision represents the model's ability to correctly identify leaving employees among those predicted to leave. A high precision score indicates few false positives (incorrectly predicted departures).

- Recall: 92.71%: Recall measures the model's capacity to capture actual departures among all employees who left. A high recall score indicates fewer missed departures (lower false negatives).

- F1 Score: 95.23%: The F1 score is the harmonic mean of precision and recall. It provides a balanced assessment of model performance, favoring neither false positives nor false negatives.

- ROC AUC: 97.99% The Receiver Operating Characteristic Area Under the Curve (ROC AUC) quantifies the model's ability to discriminate between positive and negative cases. A high ROC AUC score confirms the model's discriminative power. Implications for Predicting Employee Attrition:

The model exhibits outstanding performance across various metrics, promising significant benefits for the organization:
