**PREDICTING PRICES OF BOSTON DATASET**

1. This notebook refers to predicting median average house prices of **BOSTON** (dataset downloaded from kaggle in csv format)
   
2. Dataset contains 13 predictive and 1 target variables(all variables are numeric).

**LOADING DATASET**

1. Imported all the necessary libraries and loaded the csv file using pandas.

2. Splitted dataframe into features and target.

3. Splitted the features and target into train and test.

**PREPROCESSING**

1. Scaled all the predictive variables using standard scaler.

**PIPELINE**

1. built a pipeline that will scale the data and will use transformed target regressor to predict the prices.

1a. Transformed target regressor is a transformer that automatically transformed my target variable to normal distribution and performed inverse transform at the end for interpretability.

1b. Inside tranformed target regressor was, the ridge estimator that predicted the target.

**PREDICTION**

1. Fitted the pipeline on train data and finally got predictions.

**EVALUATION**

1. Used mean squared error for model evaluation.

**RESULTS**

Got mean squared error of 4.16 on test data.
