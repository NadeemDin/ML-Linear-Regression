# ML-Linear-Regression-Project:

Building a Linear Regression model to predict housing sale price using the features of the AMES housing dataset.

## Description:

The data set contains housing sale prices and the descriptive features of each house.
Upon initial inspection we can see that some features are more correlated with the 'SalePrice' than others, features such as Overall Quality of the house, Gr living area, Garage Area etc. This is to be expected. 

Very early on we can see that these three features have siginificant importance when aiming to predict the SalePrice.

Before building the model, appropriate data exploration and transformation was conducted to isolate outliers and remove or populate missing data (using domain knowledge and logical assumptions). dummy variables were also created for the more categorical columns.

## Building the Linear Model:

Beginning by spliting the data into 90% training data and 10% test data using Sklearns train_test_split, then scaling using StandardScaler I was able to prep the training and test data appropriately for use in the chosen linear model (ElasticNet).

A GridSearch was also implimented to find the 'best' parameters for the model.

## Results:

Upon building the model, aimed to predict the y values (SalePrice) of the X_test (10% test data) and using simple metrics such as MAS and RMSE to measure performance. 

The model was fairly basic and with an MAE of ~$14195 and RMSE of ~$20558
where the mean SalePrice is ~$180796.

So the results werent bad but with a different or more complex model I could aim to reduce the metrics further and thus increase the performance of the model.








