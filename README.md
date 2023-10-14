# House Prices Prediction

Here in this problem i was trying to predict the selling price of a house based on various factors.

# Description of the dataset

The features in the dataset are as follows 
1. ID: ID of the Record 
2. OverallQual: It represents the overall quality of the house
3. GrLivArea: It represents the living room area in the house
4. YearBuilt: It represents in which year the house is constructed 
5. TotalBsmtSF: It represents the total area of the house
6. FullBath: It represents the number of washrooms
7. HalfBath: It represents the number of semi washrooms
8. GarageCars: It represents how many cars will fit in garage
9. GarageArea: It represents the area of the garage
10. SalePrice: It represents the selling price of the house and it is the target variable 

# Data preprocessing, EDA, Feature Engineering

- Dropped the ID coloumn as it doesnot have any impact on target variable
- Here in the dataset there were neither missing values nor outliers that needs to be handled
- There were no categorical coloumns that are needed to be encoded
- Performed the correlation between all the features to find if there any positive or negative correlation, but there is no correlation
 across all the variables. Even the target variable is not having any correlation with any other variable which doesnot help most of the models to find patterns in the data. So i couldnot perform the feature selection.
- **(Tried various data transformations such as log transformations and exponential transformations to see if it improves the correlation but didnot find any improvement) not included this in the notebook.**
- **As there is no correlation among independent features considering dimensionality reduction is not a choice.**
- Splitted the dataset considering 75% of the data for training and 25% of the data for testing.

# Model Selection and training

- Choosen Random forest regressor and support vector regressor as there is no linear relationship in the data.
- Choosen MSE, RMSE, R square, Adjusted R square for evaluating the model.
- Here both the models failed to predict the testing dataset. out of both SVR has got low Mean Squared Error.

# Hyperparameter tuning

- Considered the above mentioned algorithms with some parameters using GridSearchCV and Cross validation and found out the best parameters
- Using those parameters tried fitting models once again but it didnot improve the results.

# Conclusion

- In this project i tried to build a ML model which is capable of predicting the selling price of a house. 
- But the data seems to be not accurate as any of the features are not showing impact of the output variable.
- Improving the data quality or by adding additional data might help the model to understand the underlying patterns.

# Future Scope

- Will try to re-check if there is any underlying patterns in the data by exploring transformations during feature engineering.
- Will try to implement this use case using Artificial Neural Networks and explore if it improves predictions