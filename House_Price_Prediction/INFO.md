This project aims to predict house prices using various machine learning algorithms and a set of housing features. Using Python libraries like pandas, scikit-learn, and matplotlib, the project walks through data preprocessing, exploratory data analysis (EDA), and model training and evaluation.

# Project Overview
Accurate house price prediction is essential for buyers, sellers, and real estate agents, aiding in investment decisions and market analysis. This project explores multiple machine learning models to determine the best approach for predicting house prices.

## Models tested include:

- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

## Requirements
To run this project, you will need:

- Python 3.x
- The following Python packages: pandas numpy matplotlib seaborn scikit-learn
  
## Project Steps
Data Loading: Load the Ames Housing dataset from a specified path or URL.

### Exploratory Data Analysis (EDA)

- Visualize feature correlations and distributions to understand relationships.
- Plot target distribution (House Price) and feature distributions.

### Data Preprocessing

- Scale numeric features to improve model performance.
- Implement a preprocessing pipeline using scikit-learn for consistent data handling.

### Model Selection and Training

- Apply several regression models, including Linear Regression, Random Forest, and Gradient Boosting.
- Use cross-validation to get reliable training performance metrics.

### Model Evaluation

- Evaluate each model using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE).
- Compare models to determine the most accurate one.
