#PREDICTING PRICES OF BOSTON DATASET
This notebook refers to predicting median average house prices of **BOSTON** (dataset downloaded from kaggle in csv format).
Dataset contains 13 predictive and 1 target variables(all variables are numeric).
##LOADING DATASET
Imported all the necessary libraries and loaded the csv file using pandas.
Splitted dataframe into features and target.
Splitted the features and target into train and test.
##PREPROCESSING
Scaled all the predictive variables using standard scaler.
##PIPELINE
built a pipeline that will scale the data and will use transformed target regressor to predict the prices.
Transformed target regressor is a transformer that automatically transformed my target variable to normal distribution and performed inverse transform at the end for interpretability.
Inside tranformed target regressor was, the ridge estimator that predicted the target.
##PREDICTION
Fitted the pipeline on train data and finally got predictions.
##EVALUATION
Used mean squared error for model evaluation.
##RESULTS
Got mean squared error of 4.16 on test data.
