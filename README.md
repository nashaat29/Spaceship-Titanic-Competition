# From Data to Predictions: Building a Model for Spaceship Titanic Survival

Welcome to the **Spaceship Titanic Survival Prediction** project repository! This project focuses on utilizing machine learning techniques to predict whether a passenger aboard the Spaceship Titanic was transported to an alternate dimension during a spacetime anomaly. The goal is to build a reliable and interpretable model for survival prediction based on passenger data.

![Cover](https://github.com/user-attachments/assets/6e960c9d-4475-4dbe-8588-3eb7b65f3862)

---

## Project Overview

**Objective**: Develop a machine learning model to predict passenger survival on the Spaceship Titanic.  
**Features**: Passenger information such as Age, CryoSleep status, Spending habits (RoomService, FoodCourt, ShoppingMall, Spa, VRDeck), HomePlanet, Destination, and more.  
**Dataset**: Contains information about passengers aboard the Spaceship Titanic, including whether they were transported (`Transported`).  
**Methodology**: Extensive data exploration, preprocessing, feature engineering, and model evaluation using machine learning algorithms.

---

## Key Steps

### 1. Data Exploration
In the data exploration phase, i analyzed the dataset to understand its structure and identify patterns. Key tasks included:
- **Dataset Overview**: Examining the size, structure, and basic statistics of the dataset.
- **Feature Analysis**: Investigating the distribution of each feature and identifying missing values or anomalies.
- **Target Variable Exploration**: Analyzing the distribution of the target variable (`Transported`) to understand the balance between transported and non-transported passengers.

### 2. Preprocessing
Effective preprocessing was crucial for preparing the dataset for modeling. Key steps included:
- **Remove Useless Columns**
- **Convert Columns Data Types**
- **Handle Missing Data and Duplicated Records**
- **Feature Engineering**
- **Handle Categorical Columns**

### 3. Modeling
I experimented with various machine learning algorithms to identify the best-performing model for survival prediction. Key steps included:
- **Algorithm Selection**: Tried multiple algorithms such as Logistic Regression, Random Forest, XGBoost, K-Nearest Neighbors (KNN), and Naive Bayes.
- **Cross-Validation**: Used 5-fold cross-validation to evaluate model performance and ensure robustness.
- **Hyperparameter Tuning**: Optimized hyperparameters using `GridSearchCV` to improve model accuracy.

### 4. Evaluation
Model evaluation was performed to assess the effectiveness of each algorithm. Key metrics included:
- **Accuracy**: Overall correctness of the predictions.
- **ROC-AUC Score**: Area under the ROC curve, measuring the model's ability to distinguish between classes.

### 5. Feature Selection
Feature selection was performed to enhance the model's efficiency by focusing on the most relevant features. Key steps included:
- **Correlation Analysis**: Identifying correlated features to reduce multicollinearity.
- **Feature Importance**: Using techniques like feature importance to select the most influential features.

---

## Selected Model

After a comprehensive evaluation, the **Logistic Regression** model emerged as the top performer, achieving an impressive accuracy of **76.86%**. This model was selected for its interpretability and reliability in predicting passenger survival.

---

## Results

The table below summarizes the performance of each algorithm, showcasing the highest accuracies across folds:

| Algorithm              | Accuracy         |
|------------------------|------------------|
| Logistic Regression    | 76.39            |
| Random Forest          | 74.07            |
| XGBoost                | 75.29            |
| KNN                    | 70.62            |
| Naive Bayes            | 66.36            |

---

## Kaggle Notebook

You can explore the full implementation of this project on Kaggle:  
Kaggle Notebook: https://www.kaggle.com/code/mohammednashat/building-a-model-for-spaceship-titanic-survival
