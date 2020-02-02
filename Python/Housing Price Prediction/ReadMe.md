The dataset has been taken from Kaggle. It was the first project as part of learning Data Science using Python. The link to the dataset can be found [here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data). 

There are two datasets, one for training and one for testing. The dimensions of the training dataset are 1460 x 81.

The aim of the project was to correctly predict the housing price considering the data. 

Following steps were taken while completing the project:

1. Loading the dataset.

2. Exploratory analysis of the variables to identify if there is any outlier in the dataset. Correlation factor was also validated to filter out features from the dataset.

3. Transformation of the dataset to remove skewness from the dataset. BoxCox Transformation was used for the purpose.

4. Fitting the final dataset. For building a model various models were considered like, Linear Regression, Multiple Linear Regression, Lasso and Ridge Regression. The best model was obtained using Lasso with some hyperparameter tuning.

**Results:**

A rms score of 0.92 was attained for the test dataset. The score was obtained from the kaggle website after submission of the csv.
