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

The model created with Lasso regression, selected features that gave an r2 score:
- r2 for training data: 0.86
- r2 for test data: 0.85
  72 features where selected as a result using the Lasso Regression with a hyperparameter of 250
The coefficient sign explain whether the independent variables are positively correlated, 
i.e. The  with increase in variable value there is an increase in Sales price
or negatively correlated i.e. with the increase in the variable value there is a decrease in Sales Price

**Positive correlation**

    - BedroomAbvGr 3/4 Bedrooms above grade 3 and 4
    - BsmtExposure Gd - Good Basement Exposure
    - BsmtFinType1 BLQ/GLQ - Below Average / Good Living Quarters
    - BsmtFullBath 1 - 1 basement full bathrooms
    - Exterior1st BrkFace/Plywood - Exterior covering on house
    - FireplaceQu Gd/ TA - Good to Average Fireplace quality
    - Fireplaces 2 - Number of fireplaces
    - Foundation PConc - Type of foundation Poured Concrete
    - FullBath 3 Full bathrooms above grade
    - GarageCars 3 Size of garage in car capacity
    - GarageType Attchd Garage location Attached to home
    - GrLivArea: Above grade (ground) living area square feet
    - HouseStyle 1Story	Style of dwelling One story
    - LotConfig CulDSac Lot configuration
    - LotShape IR2	Moderately Irregular shape of property
    - MSSubClass 60 Identifies the type of dwelling involved in the sale
    - MSZoning FV/RL - Identifies the general zoning classification of the sale.
        - Floating Village Residential
        - Residential Low Density
    - Neighborhood Brookside/Crawford/Northridge/Northridge Heights/Stone Brook - Physical locations within Ames city limits
    - OverallQual (8-10) Rates the overall material and finish of the house
        - Very Good to Excellent
    - RoofStyle_Hip Type of roof
    - TotRmsAbvGrd 10 Total rooms above grade (does not include bathrooms)
    - WoodDeckSF Wood deck area in square feet


**Negative correlation**


    - BsmtExposure No / NA  - when there is no basement exposure
    - BsmtFinType1 Unf / NA - when unfinished basement or no basement
    - BsmtQual Fa/Gd/NA/TA - when basement Fair/Good/TA or not available
    - Built_Yrs - year of construction
    - ExterQual TA - Average quality of the material used for the exterior
    - Exterior1st HdBoard - Exterior covering on house is Hard Board
    - Exterior2nd Stucco/Wd Sdng (Wood Siding) - Exterior covering on house (if more than one material)
    - FireplaceQu NA - No Fireplace quality
    - FullBath 1 - Full bathrooms above grade
    - GarageCars 1 - Size of garage in car capacity
    - GarageFinish NA/RFn/Unf - Interior finish of the garage NA/Rough Finished/ Unfinished
    - GarageType NA - No Garage
    - HeatingQC Fa/Gd/TA - Fair/Good/Average Heating quality and condition
    - KitchenQual Fa/Gd/TA - Fair/Good/Average Kitchen quality
    - LotConfig Inside - Lot Configuration
    - LotShape Reg	- Regular	shape of property
    - MSSubClass - Identifies the type of dwelling involved in the sale
        - 1-STORY PUD (Planned Unit Development) - 1946 & NEWER
        - 2-STORY PUD - 1946 & NEWER
        - DUPLEX - ALL STYLES AND AGES
        - 1-STORY 1945 & OLDER
    - MSZoning RM - Identifies the general zoning classification of the sale
        - Residential Medium Density
    - Neighborhood Edwards/NAmes/OldTown - Physical locations within Ames city limits
    - OverallCond (1-4) Rates the overall condition of the house
        - Very Poor to Below Average
    - OverallQual (1-4) Rates the overall material and finish of the house
        - Very Poor to Below Average
    - RemodAdd_Yrs years since Remodel date
    - RoofStyle Gable - Type of roof
    - TotRmsAbvGrd 5 - Total rooms above grade (does not include bathrooms)



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
