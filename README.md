# Surprise Housing Analysis using Regularisation
> To understand the factors affecting the house prices like which features are significant in predicting the price of a house and how well those variables describe the price of a house.


## Table of Contents
* [Project Info](#project-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## Project Information

### 1. Business Problem Statement

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.The company is looking at prospective properties to buy to enter the market. They need a good model that can be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. 

We will to build a regression model using regularisation in order to predict the actual value of the prospective properties and determine the optimal value of lambda for ridge and lasso regression and then decide whether to invest in them or not. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

### 2. Dataset

The following categorical features have one level NA

  Alley : NA = No alley access
  <br/>BsmtQual, BsmtCond, BsmtExposure, BsmtFinType1, BsmtFinType2 : NA = No Basement
  <br/>FireplaceQu : NA = No Fireplace
  <br/>GarageType, GarageFinish, GarageQual, GarageCond : NA = No Garage
  <br/>PoolQC : NA = No Pool
  <br/>Fence : NA = No Fence
  <br/>MiscFeature : NA = None

So, please prevent the auto consideration of missing value when reading the dataset.

## Technologies Used
- numpy - 1.23.5v
- pandas - 1.5.3v
- matplotlib.pyplot - 3.7.0v
- seaborn - 0.12.2v
- sklearn - 1.2.1v
- statsmodels - 0.13.5v
- python - 3.10.12v

## Conclusions
1. We can observe that the values of R2 Score, RSS, MSE and RMSE values of both Ridge and Lasso Regression are similar for both train & test datasets.
2. The optimal value of lambda for Ridge Regression is 1
3. The optimal value of lambda for Lasso Regression is 0.0001
4. The top features that are significant in predicting the price of a house are :
 - For Ridge Regression:
   - OverallQual_9
   - OverallQual_10
   - OverallQual_8
   - OverallCond_9
   - OverallCond_8
 - For Lasso Regression:
   - OverallQual_9
   - OverallQual_10
   - OverallQual_8
   - OverallCond_9
   - OverallQual_7

So it is recommended to consider these significant features in predicting the price of a house.

5. These top features describe the price of a house in the following way:
   - OverallQual_10, OverallQual_9, OverallQual_8 & OverallQual_7:
     If the overall material and finish of the house is Good, Very Good or Excellent, the price of house will increase by 1.13 to 1.54 times
   - OverallCond_9, OverallCond_8 & OverallCond_7:
     If the overall condition of the house is Good, Very Good or Excellent, the price of house will increase by 1.04 to 1.10 times
   - GrLivArea:
     As we increase 1 area square feet, the price of house will increase by 1.07 times
   - MSSubClass_70: If the type of dwelling involved in the sale is 2-STORY 1945 & OLDER, the price of house will increase by 1.07 times
   So now, we can check how well each feature describes the price of a house in a similar way.


## Acknowledgements

- I would like to thank [Anjali Rajvanshi](https://www.linkedin.com/in/anjalirajvanshi/) for her explanation on Advanced Regression.
- References for seaborn plots are taken form [Tutorials Point](https://www.tutorialspoint.com/seaborn/seaborn_tutorial.pdf)
- References for regularizations are taken from [Analytics Vidhya](https://www.analyticsvidhya.com/blog/2022/08/regularization-in-machine-learning/)).


## Contact
Created by [@gnyana_teja](https://www.linkedin.com/in/somanchi-gnyana-teja/) 

Feel free to contact me 👍
