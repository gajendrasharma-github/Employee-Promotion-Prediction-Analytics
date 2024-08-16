# Employee-Promotion-Prediction-Analytics
## Problem Statement

In an evolving business environment, identifying and promoting the right talent is crucial for organizational growth and employee satisfaction. However, the challenge lies in accurately predicting which employees are most likely to excel and deserve promotion based on their performance, experience, and other attributes. Traditional methods often fail to account for complex patterns in employee data, leading to inefficiencies and missed opportunities for optimal talent management.

## Project Description

The **Employee Promotion Prediction Analytics** project aims to address this challenge by leveraging advanced data analysis and machine learning techniques. By exploring and analyzing employee data, the project seeks to uncover key factors that influence promotion decisions and develop **predictive models** that can accurately forecast which employees are most likely to be promoted. This solution not only **streamlines the promotion process** but also **enhances decision-making**, ensuring that high-potential employees are recognized and advanced appropriately.

## Project Overview

The main objectives of this project are:
- **Data Preprocessing:** Handling missing values, dropping irrelevant columns, and preparing the dataset for analysis.
- **Exploratory Data Analysis (EDA):** Analyzing various features to understand the distribution and relationships in the data.
- **Feature Engineering:** Separating categorical and numerical features for targeted analysis.
- **Predictive Modeling:** Building and tuning machine learning models, such as Decision Trees and XGBoost, to predict employee promotions.

## Data Description

The dataset used in this project includes the following key features:
- **employee_id:** Unique identifier for each employee.
- **department, region, education, gender, recruitment_channel:** Categorical variables describing employee demographics and job-related attributes.
- **age, length_of_service, avg_training_score:** Numerical variables providing information about employee experience and performance.
- **no_of_trainings, previous_year_rating, KPIs_met >80%, awards_won?:** Other relevant features that might impact promotions.
- **is_promoted:** Target variable indicating whether the employee was promoted.

## Key Steps in the Project

1. **Data Loading and Preparation:**
   - The dataset is split into training and test sets and combined for EDA.
   - The `employee_id` column is dropped as it doesn't contribute to the analysis.

2. **Handling Missing Values:**
   - Missing values in the `education` column are imputed using the mode.
   - Missing values in the `previous_year_rating` column are filled based on insights from the `length_of_service` feature.

3. **Exploratory Data Analysis (EDA):**
   - Visualizing the distribution of categorical and numerical features.
   - Analyzing the relationships between key variables to gain insights that inform model building.

4. **Feature Engineering:**
   - Separating categorical and numerical columns to perform specific analyses.
   - Conducting bivariate analysis to explore relationships between features and the target variable.

5. **Predictive Modeling:**
   - Implementing and tuning a Decision Tree model using GridSearchCV to find the best parameters.
   - Building and tuning an XGBoost model to improve prediction accuracy.
   - Evaluating model performance using metrics such as F1-score and classification reports.

6. **Model Evaluation:**
   - The Decision Tree model was visualized, and its depth was analyzed.
   - The final predictions were generated and saved for submission.


## Insights and Conclusion
The EDA provided insights into the distribution and relationships of various features in the dataset. The predictive models were built and tuned, with the Decision Tree and XGBoost models providing the final predictions on employee promotions.

## Future Work
- **Additional Model Tuning:** Further hyperparameter tuning could be done to improve model performance.
- **Feature Importance Analysis:** Analyze which features have the most impact on the prediction of promotions.
