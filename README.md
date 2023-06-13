# Income-prediction
A short data science project for predicting income using various factors 
Project Title: Income Evaluation and Prediction

Objective:
The objective of this project is to build a model that predicts whether a person's income exceeds a certain threshold (e.g., <=50K or >50K) based on various features. This prediction model will help identify the factors that contribute to higher incomes.

Data Set Description:
The dataset used for this project contains the following features:

- Age: The age of an employee.
- Work-class: Profession category.
- Final_census: Census (population of the country).
- Education: Type of last (max) education.
- Education_num: Years spent on studies.
- Marital Status: Person married or not.
- Occupation: Person's occupation.
- Relationship: Bounded by any relation or dependent.
- Race: Ethnicity to which the employee belongs.
- Gender: Gender of the employee.
- Capital-gain: Capital gain earned from selling assets.
- Capital-loss: Capital loss incurred from selling assets.
- Hours/week: Number of working hours in a week.
- Country: Country of residence.

Target Variable:
The target variable is the income threshold, categorized into two ranges: <=50K and >50K.

Model Evaluation:
Three machine learning models were selected and evaluated for their performance in predicting income:

1. XGBoost (F1 score = 0.90)
2. Random Forest (F1 score = 0.89)
3. Gradient Boosting (F1 score = 0.86)

Cross-validation using K-fold suggested no overfitting.

Hyperparameter Tuning:
Hyperparameter tuning was applied to the XGBoost model. However, it did not yield significant improvement since the model already achieved high accuracy.

Model Evaluation Results:
The XGBoost model achieved an average accuracy of 0.9044 on cross-validation. The classification report shows precision, recall, and F1-score for each class. The weighted average F1-score was 0.90.

Feature Importance:
The importance of features in predicting income was determined using the XGBoost model. The top five important features are:

1. Feature relationship
2. Feature capital-gain
3. Feature Education-num
4. Feature marital-status
5. Feature capital-loss

Conclusion:
In conclusion, tree-based models, particularly XGBoost, performed well in predicting income based on the provided features. However, further exploration is needed to better understand the relationships between features. The feature importance analysis indicates that some features, such as race, may have been overlooked in the prediction model.

