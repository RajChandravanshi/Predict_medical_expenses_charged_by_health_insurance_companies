# Insurance Cost Prediction Model

This project is focused on predicting insurance costs for individuals using a machine learning model. The model uses personal information such as age, sex, BMI (Body Mass Index), number of children, smoking status, and region to predict how much insurance costs for an individual. The dataset used is called "insurance.csv," which contains real-world data on insurance costs.

## What is the Goal of This Project?

The main goal of this project is to predict the cost of insurance (the "expenses" column) based on other personal factors (like age, BMI, smoking status, etc.). We build and train machine learning models to make these predictions as accurately as possible.

## Dataset Overview

The dataset contains **1338 rows** (data entries) and **7 columns** (features). Each row represents data for a different individual. The columns in the dataset are:

1. **age**: Age of the individual (numerical, for example, 25, 30, 40)
2. **sex**: Gender of the individual (categorical, can be either "male" or "female")
3. **bmi**: Body Mass Index (numerical, for example, 22.5, 30.4)
4. **children**: Number of children/dependents (numerical, for example, 0, 1, 2)
5. **smoker**: Whether the person is a smoker or not (categorical, can be either "yes" or "no")
6. **region**: The region where the person lives (categorical, can be one of the following: "northeast", "southeast", "southwest", "northwest")
7. **expenses**: The medical insurance cost for the individual (numerical, target variable that we want to predict)

## Key Steps in This Project

### 1. Exploratory Data Analysis (EDA)
EDA is about understanding the data, looking for patterns, and visualizing the relationships between different features.

- We create **pie charts** to show the distribution of gender, smoking status, and region.
- We create **histograms** and **box plots** to look at the distribution of numerical features like age, BMI, and expenses.
- We use **correlation matrices** to see how strongly different features relate to each other, especially to the target variable "expenses."

### 2. Model Building
After understanding the data, we build several machine learning models to predict the insurance costs. These models are:

- **Linear Regression**: A simple model that tries to find a straight line relationship between features and expenses.
- **Lasso Regression**: A variation of linear regression that adds a penalty for larger coefficients (useful for handling overfitting).
- **Ridge Regression**: Another variation of linear regression that works well for regularizing the model.
- **Decision Tree Regressor**: A decision tree model that splits data into segments based on feature values.
- **Random Forest Regressor**: A collection of decision trees that work together to make a prediction.
- **Gradient Boosting Regressor**: A model that builds trees in a way that improves the prediction by focusing on errors made by previous trees.
- **Stacking Regressor**: Combines the predictions from multiple models to improve accuracy.

### 3. Model Evaluation
We evaluate how well each model performs using **R-squared (R²)**. The R² score tells us how much of the variability in the target variable ("expenses") is explained by the model. A higher R² score means the model is doing a good job of predicting.

### 4. Prediction
Once the models are trained, we can use them to make predictions for new data. For example, we can input the details of a new person (like age, BMI, and whether they smoke) and predict their insurance cost.
