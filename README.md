# House Prices Prediction

Here in this problem i was trying to predict the selling price of a house based on various factors.

# Description of the dataset

The features in the dataset are as follows 
1. ID: ID of the Record 
2. OverallQual: It represents the overall quality of the house
3. GrLivArea: It represents the living room area in the house
4. YearBuilt: It represents in which year the house is constructed 
5. TotalBsmtSF: It represents the total area of the house
6. FullBath: It represents the number of bathrooms
7. HalfBath: It represents the number of semi bathrooms
8. GarageCars: It represents how many cars will fit in garage
9. GarageArea: It represents the area of the garage
10. SalePrice: It represents the selling price of the house and it is the target variable 

# Data preprocessing, EDA, Feature Engineering

- Dropped the ID coloumn as it doesnot have any impact on target variable
- Here in the dataset there were neither missing values nor outliers that needs to be handled
- There were no categorical coloumns that are needed to be encoded
- Performed the correlation between all the features to find if there any positive or negative correlation, but there is no correlation
 across all the variables. Even the target variable is not having any correlation with any other variable which doesnot help most of the models to find patterns in the data.
- (Tried various data transformations such as log transformations and exponential transformations to see if it improves the correlation but didnot find any improvement) not included this in the notebook.
- As there is no correlation among independent features considering dimensionality reduction is not a choice.

# Splitting the Dataset
