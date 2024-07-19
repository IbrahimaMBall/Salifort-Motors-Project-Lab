# Salifort-Motors-Project-Lab

## PROJECT TITLE: Providing data-driven suggestions for HR

# Project Overview

The HR department at Salifort Motors aims to improve employee satisfaction levels by understanding the factors that contribute to employee attrition. This project involves analyzing the collected data and building a model to predict whether an employee will leave the company. The goal is to identify factors influencing employee turnover and provide data-driven suggestions to enhance employee retention.



# Motivation

Employee attrition is costly and time-consuming for companies, as it involves finding, interviewing, and hiring new employees. By predicting which employees are likely to leave, Salifort Motors can proactively address the underlying issues, improve job satisfaction, and enhance employee retention.

# Dataset


Source: Collected by the HR department at Salifort Motors.

Number of Records: In this dataset, there are 14,999 rows and 10 columns.

Features: The dataset contains the follow variables:

<img width="537" alt="Screen Shot 2024-07-19 at 6 41 20 PM" src="https://github.com/user-attachments/assets/78d9bb4b-17cf-418e-8355-b276877f224a">

# Data Preprocessing

-Renaming and Standardization of column in snake_case
-Handling missing values

-Handling duplicates

-Handle outliers

-Encoding categorical variables

# Exploratory Data Analysis (EDA) Insights

-Employee Attrition Rate: Analysis of employees who left the company and their percentage.

-Work Hours and Projects: Stacked boxplot and histogram visualizations of average_monthly_hours distributions for number_project.

-Attrition Groups: Identification of two groups of employees who left: those who worked less (possibly fired or given notice) and those who worked more (likely quit).

-Project Load: All employees with seven projects left, with high average monthly hours.

-Optimal Project Number: Optimal number of projects for employees to work on appears to be 3-4.

-Overworked Employees: Employees working more than 166.67 hours per month (indicative of being overworked).

-High Attrition Projects: Confirmation that all employees with seven projects left.

-Satisfaction and Hours: Scatterplot insights showing two groups of employees who left: those overworked with low satisfaction and those with normal hours but still dissatisfied.

-Data Quality: Strange shape of distributions indicating possible data manipulation or synthetic data.

-Attrition Categories: Employees who left fall into two general categories: dissatisfied with short tenures and very satisfied with medium-length tenures.

-Four-Year Mark: Investigation of unusually low satisfaction levels at the four-year mark.

-Long Tenure: Longest-tenured employees did not leave, indicating possible higher-ranking, higher-paid employees.

-Satisfaction Scores: Mean and median satisfaction scores of employees who left are lower than those who stayed.

-Salary and Tenure: Examination of salary levels for different tenures.

-Evaluation Scores: Correlation between working long hours and high evaluation scores.

-Promotions: Few employees promoted in the last five years left, and few who worked the most hours were promoted.

-Department Distribution: Distribution of employees who left across departments shows no significant differences.

-Management and Satisfaction: Strong correlations between variables indicating poor management, long working hours, many projects, and lower satisfaction levels.

# Models and Results

In this project, we built and evaluated three different models to predict employee attrition: Logistic Regression, Decision Tree, and Random Forest. Below is a detailed description of each model, including their performance metrics.

## 1. Logistic Regression Model
The logistic regression model is a simple yet powerful linear model for binary classification.

<img width="318" alt="Screen Shot 2024-07-19 at 7 14 54 PM" src="https://github.com/user-attachments/assets/865b44cd-c50c-4073-b496-c879d16abb69">

Performance Metrics:

Precision: 79%

Recall: 82%

F1-Score: 80%

Accuracy: 82%

While the logistic regression model showed decent overall performance, its scores for predicting employees who leave were significantly lower.

## 2. Decision Tree Model
The decision tree model is a non-linear model that splits the data into subsets based on the most significant features.

Cross-Validation Metrics:

Precision: 91.46%

Recall: 91.69%

F1-Score: 91.57%

Accuracy: 97.20%

AUC: 96.98%

The decision tree model performed exceptionally well during cross-validation, indicating strong predictive capabilities.

## 3. Random Forest Model
The random forest model is an ensemble method that combines multiple decision trees to improve predictive performance and control overfitting.

Test Set Metrics:

Precision: 96.42%

Recall: 91.97%

F1-Score: 94.14%

Accuracy: 98.10%

AUC: 95.64%

The random forest model showed excellent performance on the test set, with scores very similar to the validation scores, indicating its robustness and reliability for predicting employee attrition on new, unseen data.

# Conclusion and Recommendations 
<img width="534" alt="Screen Shot 2024-07-19 at 7 21 43 PM" src="https://github.com/user-attachments/assets/1fd796e7-1568-4e4c-80a1-0ebc850965a2">
<img width="501" alt="Screen Shot 2024-07-19 at 7 22 13 PM" src="https://github.com/user-attachments/assets/ae177ace-782f-403a-8e93-512897264046">



Through comprehensive analysis and modeling of employee data at Salifort Motors, we have identified critical factors contributing to employee attrition. Our findings highlight that overworking employees, coupled with unclear policies and inadequate recognition, are major contributors to dissatisfaction and turnover.

The models built—including logistic regression, decision trees, and random forests—confirm that high workloads and a lack of structured support are significant issues. To address these challenges and improve employee retention, the following recommendations have been proposed:

Cap Project Workload: Limit the number of projects employees can handle to prevent burnout and ensure manageable workloads.

Promote and Investigate: Consider promoting employees who have been with the company for at least four years or investigate the reasons behind the dissatisfaction of four-year tenured employees.

Adjust Hour Expectations: Either reward employees for working extended hours or adjust workload expectations to prevent overworking.

Clarify Policies: Ensure employees are aware of overtime pay policies and make workload and time-off expectations explicit.

Enhance Work Culture: Conduct discussions to address and improve work culture both company-wide and within specific teams.

Reward Effort Proportionately: Implement a reward system that acknowledges employee contributions based on effort and impact, rather than solely on long hours.

By implementing these strategies, Salifort Motors can create a more supportive and engaging work environment, leading to improved employee satisfaction and reduced turnover.
