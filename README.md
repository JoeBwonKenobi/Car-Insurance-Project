# Car Insurance Predictions

The overall Objective of this project is to predict if customers will make a claim on their insurance using data from an insurance company.

# Link to Orignal Data Source:

https://www.kaggle.com/datasets/sagnik1511/car-insurance-data

# Methods used for Data Preparation:

Before splitting the data I will drop the duplicates and check for any inconsistancies, this will help prepare the data for machine learning. Then I identified the features (X) and the target (y) and performed a validation split. Next, I created a preprocessing object to prepare the dataset for Machine Learning. I imputed missing values using the Simple Imputer after the validation split to minimize the chance of any data leakage.

# Model:
The model I ended up using is a Logistic Regression Model. For this particular model, I used Gridsearch CV to find the best parameters to tune
My best model for predicting car insurance claims was a logistic regression model that had an accuracy of 84%


# Interpretation and Description of Model:
There are many unpredictable factors that come into play when predicting claims for car insurance. Even the best drivers could unexpectedly end up in an accident and have to use their claim. But if this model were put into production, it would do a pretty decent job at being able to predict car insurance claims. At 84% accuracy for the test data, this would be a good choice for the company to use to predict car insurance claims. It should not be used as an extremely reliable model, due to the unpredictable nature of what we are predicting, it should be taken more as a strong suggestion then a solid prediction.
