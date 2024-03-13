# classification-challenge
Module 13 Challenge

## Overview ##
Develop a supervised machine learning (ML) model that will accurately detect spam emails so that an ISP can filter them out of its customers' inboxes. ISP has provided a dataset that contains information about emails, with two possible classifications: spam and not spam. We will create two classification models to fit the provided data, and evaluate which model is more accurate at detecting spam. The two classification models are:
1. Logistic Regression
2. Random Forest

### Detail ###
The following subtasks are executed to get the result
1. Split the data into training and testing sets.
   - Read the data nto a Pandas DataFrame.
   - Create the labels set (y) from the “spam” column, and then create the features (X) DataFrame from the remaining columns.
   - Check the balance of the labels variable (y) by using the value_counts function.
   - Split the data into training and testing datasets by using train_test_split.
     
2. Scale the features.
   - Create an instance of StandardScaler.
   - Fit the Standard Scaler with the training data.
   - Scale the training and testing features DataFrames using the transform function.
     
3. Create a logistic regression model.
   - Fit a logistic regression model by using the scaled training data (X_train_scaled and y_train). Set the random_state argument to 1.
   - Save the predictions on the testing data labels by using the testing feature data (X_test_scaled) and the fitted model.
   - Evaluate the model’s performance by calculating the accuracy score of the model.
     
4. Create a random forest model.
   - Fit a random forest classifier model by using the scaled training data (X_train_scaled and y_train).
   - Save the predictions on the testing data labels by using the testing feature data (X_test_scaled) and the fitted model.
   - Evaluate the model’s performance by calculating the accuracy score of the model.
     
6. Evaluate the models.
   - Determine which model performed better
