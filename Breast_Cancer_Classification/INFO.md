# Breast Cancer Classification

This project aims to classify breast cancer tumors as benign or malignant using the Wisconsin Breast Cancer Dataset (WBCD). The dataset contains various features derived from digitized images of fine needle aspirate (FNA) of breast masses.

## Dataset

The dataset is sourced from the UCI Machine Learning Repository and contains 699 instances with 10 features plus a label indicating the class of the tumor. The classes are:

2: Benign --> Encoded as 0
4: Malignant --> Encoded as 1

The features include measurements of cell characteristics, such as clump thickness, uniformity of cell size and shape, and others.

## Libraries Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- TensorFlow/Keras
- Matplotlib/Seaborn (for data visualization)

## The project includes:

- Data loading and preprocessing
- Exploratory Data Analysis
- Logistic Regression Model for classification
- Neural Network Model for classification
- Evaluation of models with accuracy and classification reports
- Results

After training both the Logistic Regression and Neural Network models, the Neural Network model outperforms the Logistic Regression model.

## Conclusion

This project demonstrates the use of machine learning techniques for breast cancer classification. The results show the effectiveness of using various algorithms for binary classification problems in medical datasets. Further improvements can be made by experimenting with more complex models or incorporating additional features.
