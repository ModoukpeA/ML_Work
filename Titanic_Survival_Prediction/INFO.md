# Titanic Survival Prediction

## Project Overview
This project predicts the survival of passengers on the Titanic using attributes like age, gender, and passenger class. 

## Dataset
The dataset is from the [Titanic Kaggle competition](https://www.kaggle.com/c/titanic). 

## Steps
1. **Data Exploration**: Inspected data, handled missing values.
2. **Feature Engineering**: Encoded categorical variables.
3. **Model Training**: Trained Logistic Regression and Random Forest models.
4. **Evaluation**: Compared models using accuracy, confusion matrix, and classification report.

## Results
Random Forest achieved the highest accuracy, making it the best model for this project.

## How to Run
Clone this repository and execute `titanic_survival_prediction.ipynb` to see the results.

## Additional Notes
- Try tuning hyperparameters with GridSearchCV or RandomizedSearchCV to improve model performance.
- Experiment by adding or removing features to observe the effect on model performance.
- Use joblib or pickle to save the best-performing model for future use.
