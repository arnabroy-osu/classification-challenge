## Title
Module 13 Challenge - Email Spam Detector

## Source Data
Data is sourced from the UCI Machine Learning Library. The data is located at [https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv]. The dataset contains 57 features and 1 target variable (spam), which is the last column in the dataset.

## Desired Outcome of the exercise
The goal of this exercise is to create and fit two Machine Learning models (Logistic Regression & Random Forest Classifier) to predict whether an email is spam or not. We will then compare the performance of the two models and determine which model is the best fit for the data based on the accuracy score.

## Data Preparation & Analysis
Data preparation is pretty straight forward. We will load the data from CSV file (UCI Machine Learning Library) into a DataFrame and then separate the features and target variable into 2 separate DataFrames. We then split the data into training and testing datasets using the train_test_split method & apply the StandardScaler to scale the features data. Finally, we create and fit the Logistic Regression and Random Forest Classifier models to the training data and then make predictions on the testing data.

## Conclusion
The Logistic Regression model had an accuracy score of 0.91, whereas the Random Forests model had an accuracy score of 0.96. We already preicted at the beginning of creating & fitting the 2 models, that Random Forests would perform better than Logistic Regression, and our prediction was correct. This is because Random Forests are better suited for high-dimensional data, and this dataset has 57 features.