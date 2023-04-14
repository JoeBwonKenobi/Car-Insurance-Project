# Car Insurance Predictions

The overall Objective of this project is to predict if customers will make a claim on their insurance using data from an insurance company.

# Link to Orignal Data Source:

https://www.kaggle.com/datasets/sagnik1511/car-insurance-data

# Project Overview:

Built Logistic Regression Model, Random Forest Classifier, and KNN models and tuned them using GridsearchCV. I used GridsearchCV because it will systematically search through a specified range of hyperparameters to find the best combination of hyperparameters that optimizes the performance of the model. This ensures I'm getting the best posible version of the model.

# Visualizations of Data:

![download](https://user-images.githubusercontent.com/117705408/231908899-49c9f21b-afce-4b78-ab3b-b6733cb0d1fb.png)

- This visualization shows the number of claims inside the different income levels of the people who are in the dataset.
- The trend that is clearly visable here is that the poverty class has a much larger amount more claims than most of the other income classes.
- This is more than likely because people of this income level are unable to afford the cost of repairs caused by an incident.
- The upper class has the lowest amount of claims overall, likely due to the fact that most of them can afford to repair their vehichle without making a claim.

![download](https://user-images.githubusercontent.com/117705408/231908926-01faf914-e525-4efd-8e51-bea5d1629567.png)

- This shows us the percentage of people in each imcome class who own their own car.
- The people who do not own their own car are most likely easing their vehicle.
- The trend we are clearly able to see here is that the higher income class someone is in, the better chance there is that they own their own car.

![download](https://user-images.githubusercontent.com/117705408/231908963-89790edd-9a4b-4678-ac80-655784637af2.png)

- This shows us the number of people who had Dui's for each possible outcome result(1)DUI or (0)no DUI.
- There is a trend with the people who have no Dui's, they are more prone to make a claim on their insurance. 
- This is most likely because the people who have at least one Dui went to jail and their insurance company more than likely dropped their coverage, or at the least they did not make a claim on their insurance because they don't offer coverage for people who are in an accident under the influence.

# Methods used for Data Preparation:

Before splitting the data I will drop the duplicates and check for any inconsistancies, this will help prepare the data for machine learning. Then I identified the features (X) and the target (y) and performed a validation split. Next, I created a preprocessing object to prepare the dataset for Machine Learning. I imputed missing values using the Simple Imputer after the validation split to minimize the chance of any data leakage.

# Model:
The model I ended up using is a Logistic Regression Model. For this particular model, I used Gridsearch CV to find the best parameters to tune
My best model for predicting car insurance claims was a logistic regression model that had an accuracy of 84%


# Interpretation and Description of Model:
There are many unpredictable factors that come into play when predicting claims for car insurance. Even the best drivers could unexpectedly end up in an accident and have to use their claim. But if this model were put into production, it would do a pretty decent job at being able to predict car insurance claims. At 84% accuracy for the test data, this would be a good choice for the company to use to predict car insurance claims. It should not be used as an extremely reliable model, due to the unpredictable nature of what we are predicting, it should be taken more as a strong suggestion then a solid prediction.
