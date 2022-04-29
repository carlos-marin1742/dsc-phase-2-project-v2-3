# To Renovate or not to renovate


## Background
Every Year, Americans renovate their home so when it comes time to sell, they can best the return. I create two multiple linear regression models based on whether they were renovated or not.


## Business Problem
How much does renovating or not renovating your home affect pricing of the home? By creating a multiple linear regression we can see how each coefficient works with pricing. From this we can create an actual formula that can be used to calculate how much your home will sell for once renovated or not renovated


## Data
Using KC data set. The data set is seperated  by renovated and then normalization data processing is done.
Renovated data set has 744 rows
Non renovated data set has 3842 rows.
Both have 5 rows



## Methods
First we create single linear models by coefficient to price
Then we compare and create the multiple linear regression to see how the coefficient changes.
Data is trimmed to increase R squared and the overall model accuracy at the end. 



## Results
Results show lots of variability in data. High RMSE, high MAE. Model score accuracy is low. 
![](./renovated actual vs predicted)
![](./NR actual vs predicted)


## Conclusions
First I evaluated how each coefficient (bedroom, bathroom, square foot living area, square foot above area) when renovated how they affect pricing of a home. While trimming the data did lower R squared, but it is known that the model accuracy score at the end would be significantly lower if not trimmed. The plot would now show a non linear trend at all if not trimmed. Trimming data to remove outliers increased model score accuracy at the end. Possibly more (or less) trimming could be done, to increase the model score accuracy seen at the the end.




## Next Steps 

1) Evaluate methods to increase model accuracy
2) evaluate trimming (decrease/increase trimming) see how this affects R squared and model accuracy score at the end.
3) evluate what causes negative correlation in multiple linear regression