# Machine-Learning-Model
Machine Learning Model for Car Price Prediction
## Model Implementation
1) Linear Regression
2) Decision Tree Regressor
3) Random Forest Regressor
4) Gradient Boosting Regressor
5) Support Vector Regressor
## Model Evaluation
we train and evaluate all the models Implemented on the test set and calculated the R-squared Score ,Mean Squared Error,Mean Absolute Error

 R-squared: This metric tells us how well the model fits the data. The higher the R-squared value, the better the model explains the variance in the target variable.
 
 Mean Squared Error: MSE is the average squared difference between predicted and actual values. The smaller the value, the better the model.
 
 Mean Absolute Error: MAE measures the average absolute difference between predicted and actual values. Lower is better again.

After Checking Each Model We Got the Best Model as Random Forest Regressor,because it has the Higher R-square value.

Random Forest Regressor has a higher R-squared value,it explains more variance in the target variable, that is, car prices. The higher the R-squared value, the better the model fits in describing the relationship of the independent features with the dependent variable (car price).

Random Forest Regressor has the lowest MSE among all the models. The lower MSE means that the model's predictions are closer to the true values, meaning fewer errors in predicting the car prices.
The MAE for the Random Forest model is also the lowest, showing that on average, its predictions are better than those of other models. Lower MAE shows fewer average errors in prediction.

Random Forest Regressor is the best performer with respect to predicting the prices of cars from the dataset provided, CarPrice_Assignment, because of its high R-squared, low MSE, and low MAE. It captures the complex relations among car features and price fairly well, making it a robust model and reliable for car price predictions. Its ensemble approach and capacity to model non-linear relations and feature importance analysis makes it an ideal choice for this task.

Similarly, the Gradient Boosting Regressor is also got higher R-squared value closer to R-squared value got for the Random Forest Regressor

## Feature Importance Analysis
It is essential to Find the Feature that affect the Car Price here we use SelectKBest to find the features.the important features that Affect the car price are:- 
  carlength,carwidth,curbweight,enginesize,horsepower,highwaympg

## Hyperparameter Tuning 
Hyperparameter tuning is an essential step in optimizing machine learning models. It involves finding the optimal combination of hyperparameters, which are parameters that control the learning process of the model but aren't learned from the data itself.
Using GridSearchCV, we done hyperparameter tuning and got a more optimum output than the previous by testing the model after tuning hyperparameters with an unseen data and checked the value of R-square, Mean Squared Error, and Mean Absolute Error.
## Saving the Best Model
Saved the best Model Using Joblib.By saving the best model is efficient, consistent, and convenient because it saves the model without needing further retraining, which also allows for easier deployment and better integration into production pipelines or easier sharing with others.
