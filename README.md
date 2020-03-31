# Big-Mart-Sales-Hackathon
This Hackathon is sponsored by Analytics Vidhya and we are supposed to build a predictive model and find out the sales of each product at a particular store.


We have train (8523) and test (5681) data set, train data set has both input and output variable(s). We need to predict the sales for test data set.

 # Evaluation Metric:

 The Evaluation metric we will use is the Root Mean Square Error value. 

Where,
N: total number of observations
Predicted: the response entered by user
Actual: actual values of sales


# EDA Steps taken

1. Checking the distribution of Train and Test Data.
2. Checking the Statistics for the whole Data.
3. Filling the missing values in the Item_Weight column with mean and Outlet_Size with mode as there are missing values
4. Generating a Profile report on the whole dataset.

# Feature Engineering

1. Replacing the various content values in the Item Fat Content variable 
2. Getting the first two characters of ID to separate them into different categories.
3. Checking the distribution of variables using count plot.
4. Checking the unique items in the train and test set.
5. Mapping the Item_Identifier variable with their respective column names.
6. Label Encoding the train and test dataset.
7. One hot encoding the data to get dummy variables for the train and test data.

# Modelling

1. Linear Regression yielding a RMSE score of 9.18
2. Random Forest Regressor yielding a RMSE score of 39.62
3. Support Vector Machine yielding a RMSE score of 739.68
4. Gradient Boosting Algorithm yielding a RMSE score of 30.42
5. Decision Tree Regressor yielding a RMSE score of 30.02
6. Adaboost Algorithm yielding a RMSE score of 121. 48

After using 6 algorthims on the train data and testing the same on unseen test data we can see that Linear Regression has yielded the lowest RMSE Score of 9.18, since, lower the RMSE value the better, as it is able to explain the variance in the data points in a much better way. And RMSE is defined by how close the predicted values are in terms of the observed data points. Lower values of RMSE indicate better fit. Hence, we will select the Linear Regression RMSE value for the prediction purposes.




