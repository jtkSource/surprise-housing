# Surprise Housing Assignment
> You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not


## Table of Contents
* [General Info](#general-information)
* [Objective](#objective)
* [Data](#data)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
A US-based housing company named Surprise Housing has decided to enter the Australian market. 
The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. 
For the same purpose, the company has collected a data set from the sale of houses in Australia.

The company is looking at prospective properties to buy to enter the market. 
You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.
The company wants to know:
 - Which variables are significant in predicting the price of a house, and
 - How well those variables describe the price of a house.
Also, determine the optimal value of lambda for ridge and lasso regression

## Objective

- You are required to model the price of houses with the available independent variables. 
This model will then be used by the management to understand how exactly the prices vary with the variables. 
- They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. 
- Further, the model will be a good way for management to understand the pricing dynamics of a new market.

### Data
Please find the dataset link [here](https://ml-course3-upgrad.s3.amazonaws.com/Assignment_+Advanced+Regression/train.csv)

Files:
- data/data_description.txt
- data/train.csv

## Conclusions

### Optimal Lambda Value
  - Ridge regression: 0.7
  - Lasso regression: 0.0010 

### Significant Variables (Top 10)

#### **Ridge regression**

_Positive Correlation_

- GrLivArea - Above grade (ground) living area square feet
- MSZoning - Identifies the general zoning classification of the sale
  - FV Floating Village Residential
  - RL Residential Low Density
  - RH Residential High Density
  - RM Residential Medium Density

_Negative Correlation_

- HeatingQC - Poor Heating quality and condition
- Exterior1st - Brick Common Exterior covering on house
- Fireplaces - Number of fireplaces 3
- BedroomAbvGr - Number of Bedroom above grade 1
- MSSubClass - Identifies the type of dwelling involved in the sale
  - 160 - 2-STORY PUD - 1946 & NEWER


#### **Lasso regression**

_Positive Correlation_

- GrLivArea - Above grade (ground) living area square feet
- OverallQual - Very Good overall material and finish of the house
- Neighborhood - Crawfor
- Neighborhood - NridgHt
- MSZoning - Identifies the general zoning classification of the sale
  - FV - Floating Village Residential

_Negative Correlation_

- GarageType - No Garage
- OverallCond - Low overall condition of the house
- RemodAdd_Yrs - Number of years since renovation
- MSSubClass - Identifies the type of dwelling involved in the sale
  - 30 - 1-STORY 1945 & OLDER
- OverallQual - Low overall material and finish of the house

As we prefer to use the Lasso regression as we can model on a fewer features.

## Business Recommendation 
> The model suggests that there is a positive co-relation for the 
> Living area of the house as the primary concern followed by the build quality of the house.
> The location of the house also plays a very important role
> 
> There is also a negative correlation for houses with no garage feature and having low overall 
> condition of the house.  Houses that are not renovated for a long time tend to fetch lower prices along with houses that
> are very old 

## Technologies Used
- pandas - 1.4.4
- matplotlib - 5.5.2
- seaborn - 0.11.2
- statsmodels - 0.13.2
- sklearn - 1.1.3

## Acknowledgements
Give credit here.
- As part of the Upgrad Course on ML&AI

## Contact
Created by [@jtkSource] - feel free to contact me!
