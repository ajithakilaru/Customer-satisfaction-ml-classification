# Customer Satisfaction Prediction using Machine Learning

## Overview

This project analyses customer satisfaction in road transport and builds
machine-learning models to predict whether a traveller is satisfied or
dissatisfied.

The project covers the complete machine-learning workflow including data
cleaning, exploratory data analysis, feature engineering, preprocessing,
model training and model evaluation.

## Objectives

- Analyse factors influencing traveller satisfaction
- Explore relationships between service ratings, travel characteristics
  and delays
- Handle missing values and outliers
- Engineer meaningful features
- Train and compare multiple classification algorithms
- Identify the best-performing model

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Scikit-learn
- Jupyter Notebook

## Data Analysis

The analysis included:

- Gender and satisfaction analysis
- Age distribution
- Travel category and distance analysis
- Seat comfort and food-rating comparison
- Departure and arrival delay analysis
- Correlation analysis
- Outlier detection

Statistical tests such as Chi-square tests and Welch's t-tests were also
used where appropriate.

## Data Preprocessing

Missing numerical values were handled using median imputation, while
categorical missing values were handled using the mode.

Categorical variables were transformed using one-hot encoding.

Numerical features were standardised using StandardScaler where required.

## Feature Engineering

Several new features were created:

- **Total Delay** – combination of departure and arrival delay
- **Average Service Rating** – combined measure of service-quality ratings
- **Comfort Interaction** – interaction between seat comfort and leg room
- **Distance Category** – journey distances grouped into Short, Medium,
  Long and Very Long categories

## Machine Learning Models

Four classification algorithms were trained and evaluated:

1. Decision Tree
2. Random Forest
3. K-Nearest Neighbors (KNN)
4. Logistic Regression

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|------|------:|------:|------:|------:|
| Decision Tree | 84.08% | 80.89% | 81.43% | 81.16% |
| Random Forest | **89.19%** | **89.27%** | **84.48%** | **86.81%** |
| KNN | 86.47% | 86.39% | 80.56% | 83.38% |
| Logistic Regression | 81.88% | 78.99% | 77.61% | 78.29% |

## Best Model

**Random Forest** achieved the best overall performance with:

- Accuracy: **89.19%**
- Precision: **89.27%**
- Recall: **84.48%**
- F1-score: **86.81%**

Random Forest provided the strongest balance between predictive accuracy,
precision and recall.

## Key Findings

Customer satisfaction is influenced by a combination of service quality,
travel characteristics and delays.

Comfort-related and service-quality features showed positive relationships
with satisfaction, while longer departure and arrival delays were
associated with lower satisfaction.

The engineered **Comfort Interaction** and **Average Service Rating**
features also showed meaningful relationships with satisfaction.

## Future Improvements

Possible improvements include:

- Cross-validation
- Hyperparameter tuning
- Random Forest feature-importance analysis
- Testing additional ensemble models
- Testing the model on completely unseen data

## Notebook

The complete analysis is available in:

`customer_satisfaction_classification.ipynb`