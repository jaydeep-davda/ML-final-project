Food Nutrition Analysis and Caloric Value Prediction Using Machine Learning
Abstract

This project investigates the application of machine learning techniques to predict the caloric value of food items based on their nutritional composition. Using a comprehensive food nutrition dataset, multiple regression models were developed and evaluated to analyze the relationship between macronutrients and total caloric content. The study follows a systematic machine learning workflow including data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, and performance evaluation. The results demonstrate that both linear and non-linear models are effective in calorie prediction, with neural network and ensemble-based methods achieving superior performance.

1. Introduction

Accurate estimation of caloric values plays a critical role in dietary planning, nutrition analysis, and health monitoring. Traditional calorie calculation methods rely on fixed nutritional rules, which may not capture complex interactions between nutrients. Machine learning provides an effective alternative by learning patterns directly from data.
This project aims to design and evaluate machine learning models capable of predicting caloric values from food nutrition data, while also providing comparative insights into different modeling approaches.

2. Dataset Description

The dataset used in this study was obtained from Kaggle’s Food Nutrition Dataset, comprising approximately 2,400 food items and 37 nutritional attributes.
The dataset includes macronutrients (protein, fats, carbohydrates), micronutrients (vitamins and minerals), and other dietary components.

Target Variable: Caloric Value

Input Features: Nutritional attributes such as fat, carbohydrates, protein, sugars, and fiber

Multiple CSV files were merged to form a unified dataset.

3. Data Preprocessing

The following preprocessing steps were applied:

Removal of redundant index columns

Handling of missing values

Verification and correction of data types

Scaling of numerical features using Min-Max and Standard scaling techniques

These steps ensured data consistency and suitability for machine learning algorithms.

4. Exploratory Data Analysis (EDA)

Exploratory analysis was conducted to understand data distributions and relationships:

Distribution analysis of caloric values

Correlation heatmaps among nutritional attributes

Scatter plots examining relationships between calories and macronutrients

Boxplots for outlier detection

EDA results revealed strong correlations between caloric value and macronutrients, particularly fat and carbohydrates, supporting their selection as primary predictors.

5. Feature Selection and Engineering

Initial feature selection focused on the primary macronutrients:

Protein

Fat

Carbohydrates

An extended feature set was later incorporated, including saturated fats, sugars, dietary fiber, sodium, and water content.
Feature scaling was applied to improve model convergence and performance.

6. Methodology and Models

A comparative modeling strategy was adopted, beginning with a baseline model and progressing to more complex approaches:

Baseline Model

Linear Regression

Advanced Models

Random Forest Regressor (with hyperparameter tuning)

Support Vector Regressor (SVR)

Multi-Layer Perceptron (Neural Network)

Light Gradient Boosting Machine (LightGBM)

This approach enabled evaluation of both linear and non-linear relationships within the data.

7. Model Evaluation

Model performance was assessed using:

R² Score

Mean Squared Error (MSE)

Results indicated:

Linear Regression performed strongly due to the inherent linear relationship between macronutrients and caloric values

Neural Network and Random Forest models achieved the highest predictive accuracy

SVR showed comparatively lower performance, highlighting sensitivity to feature scaling and hyperparameter selection

8. System Implementation

To demonstrate practical applicability, a Streamlit-based web application was developed.
The application allows users to:

Select food items

View corresponding nutritional values

Visualize macronutrient distributions

The deployment serves as a proof-of-concept interface for nutritional analysis.

9. Technologies Used

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

LightGBM

Streamlit

10. Project Structure
├── app.py                    # Streamlit application
├── MLfinal.ipynb             # Data analysis and model development
├── requirements.txt          # Dependency list
├── README.md                 # Project documentation

11. Academic Context

Course: Machine Learning

Program: Master of Science in Data Science

University: University of Europe for Applied Sciences

12. Conclusion

This project demonstrates the effectiveness of machine learning techniques in predicting caloric values from nutritional data. The comparative analysis highlights the strengths of both linear and ensemble-based models, while emphasizing the importance of data preprocessing and feature selection. The study confirms that machine learning can serve as a reliable tool for nutritional analysis and decision support systems in health-related applications.

13. Future Work

Integration of trained machine learning models into the deployment layer

Inclusion of food image recognition for automated input

Expansion of prediction targets to include micronutrients

Advanced hyperparameter optimization and model interpretability techniques

Author

Jaydeep Davda
MSc Data Science
University of Europe for Applied Sciences
