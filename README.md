# **Car Insurance Predictions**

![image](https://github.com/JoeBwonKenobi/Car-Insurance-Project/assets/117705408/710433cc-443f-45ec-b72f-07664df61321)

The overall objective of this project is to predict if customers will make a claim on their insurance using data from an insurance company.

# **Link to Orignal Data Source:**

https://www.kaggle.com/datasets/sagnik1511/car-insurance-data

# **Project Overview:**

I built a Logistic Regression Model, Random Forest Classifier, and KNN models and tuned them using Gridsearch CV. I used GridsearchCV because it systematically searches through a specified range of hyperparameters to find the best combination of hyperparameters that optimize the performance of the model. This ensures that I'm getting the best possible version of the model.

I separated this project into four different notebooks for the four major steps included in the project,They are linked below:

1. Prepose two choices for datasets that meet the requirements of the project.

   https://github.com/JoeBwonKenobi/Car-Insurance-Project/blob/main/Choosing_between_two_datasets.ipynb
 
   
2. Clean the data in the selected dataset from the previous notebook.

   https://github.com/JoeBwonKenobi/Car-Insurance-Project/blob/main/Data_Cleaning_Car_insurance_Data.ipynb

3. Visualize the trends and coorelations within the dataset.

   https://github.com/JoeBwonKenobi/Car-Insurance-Project/blob/main/Visualizing_Trends_and_Coorelations.ipynb
   
 4. Build multiple models, use gridsearchCV and PCA to find the optomized version of the best model used to make predictions.

    https://github.com/JoeBwonKenobi/Car-Insurance-Project/blob/main/Car_Insurance_Prediction_Models.ipynb
   
# **Visualizations of Data:**

![image](https://user-images.githubusercontent.com/117705408/235288525-e42d9266-b5a4-45b1-ad6d-37d6ed45391f.png)


- This visualization shows the number of claims inside the different income levels of the people who are in the dataset.
- The trend that is clearly visible here is that the poverty class has a much larger number of claims than most of the other income classes.
- This is more than likely because people of this income level are unable to afford the cost of repairs caused by an incident.
- The upper class has the lowest number of claims overall, likely due to the fact that most of them can afford to repair their vehicles without making a claim.

![image](https://user-images.githubusercontent.com/117705408/235288620-b20db775-d794-423f-a355-de8a6abcbf58.png)

- This shows us the percentage of people in each income class who own their own car.
- The people who do not own their own car are most likely leasing their vehicle.
- The trend we are clearly able to see here is that the higher income class someone is in, the better chance there is that they own their own car.

![image](https://user-images.githubusercontent.com/117705408/235288673-e73b3dcc-3388-4a79-a9e2-e3c325d6bfdb.png)

- This shows us the number of people who had DUIs for each possible outcome result: (1) DUI or (0) no DUI. 
- There is a trend with the people who have no DUIs; they are more prone to make a claim on their insurance.  
- This is most likely because the people who have at least one DUI went to jail, and their insurance company more than likely dropped their coverage, or at the least, they did not make a claim on their insurance because they don't offer coverage for people who are in an accident under the influence.

# **Methods used for Data Preparation:**

To get the data ready for the machine to learn, I'll make sure there are no duplicates and that everything is consistent. Then I'll separate the data into two groups: one group that shows what we want the machine to learn (the "target" or y) and another group that provides information for the machine to use (the "features" or X).

After that, I'll divide the data into a training set and a validation set, so we can test how well the machine is learning. I'll use a set of tools called a "preprocessing object" to get the data ready for the machine, and one of the things I'll do is fill in any missing information.

To make sure the missing information doesn't interfere with the machine's learning, I'll wait until after the validation split to fill it in. This way, the machine won't be able to use any information from the validation set to learn about the training set.

# **Model:**
The model I ended up using is a Logistic Regression Model. For this particular model, I used GridsearchCV to find the best parameters to tune. My best model for predicting car insurance claims was a logistic regression model that had an accuracy of 84%.


# **Interpretation and Description of Model:**
There are many unpredictable factors that come into play when predicting claims for car insurance. Even the best drivers could unexpectedly end up in an accident and have to use their claim. But if this model were put into production, it would do a pretty decent job at being able to predict car insurance claims. At 84% accuracy for the test data, this would be a good choice for the company to use to predict car insurance claims. It should not be used as an extremely reliable model, due to the unpredictable nature of what we are predicting. It should be taken more as a strong suggestion than a solid prediction

# **Recomendations:**

 The insurance company could use the model as a reference or suggestion for making predictions, but more data would need to be obtained to get a higher accuracy from the model. A wider scope of insurance data would provide a much deeper insight and inturn imorove the accuracy of the model. With more data, it has more opurtunities to learn and make better predictions. Thes insights about income level and number of claims could provide a chance for the sales team to make some changes on advertizing, and for the finaincial executives to look at adjusting prices accordingly.
 
# **Limitations & Next steps:**

The linear regression model's ability to make predictions is only as good as the data I give it allows it to be. Meaning the more data I give it the better accuracy it will obtain. The next steps would be to try and obtain more data from the insurance company and run the new data through the model I've created. Based on my findings so far, there are many insightfull discoveries in the data that was provided. Knowing the trends in income levels, vehichle ownership, and many other categories can give extremely helpful suggestions to corporate executives within the insurance company. These can be used to make a number of different descisions including the pricing of preiums, straegy of advertizement, policy terms, and a number of other very critical parts of running an insurance company.
