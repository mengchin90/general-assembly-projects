## Problem Statement
Housing price has been a key concern in many developed countries including the United States. In the project, we are aiming to developed a regression model to help us effectively predict the housing price in the Ames, Iowa.
<br/>
<br/>
With this model, it will be beneficial to both the buyer and seller as it will provide an estimate of the housing price based on the different features identified. It will help the buyer to set a realistic budget for their dream home while preventing any over inflation of price. It will benefit the seller by enabling them to identify key areas that they could target to make improvement so as value add before putting the apartment on sale.
## Executive Summary

### Train_Clean_EDA notebook
- Importing Data and Cleaning
    - Imputing Null Values
    - Converting Ordinal Features to Numeric
- Exploratory Data Analysis
    - Age vs Sale Price
    - Porch vs Sale Price
    - Garage vs Sale Price
    - Living Area vs Sale Price
    - Basement vs Sale Price
    - heteroscedasticity
- Converting Categorical to Numeric
### Test_Clean notebook
### Modeling notebook
- Feature Selection
- Model Selection
    - Linear Regression
    - Lasso Regression
    - Ridge Regression
    - Model Comparision
- Prediction Model
- Conclusion
- Recommendation

## Conclusion
### Predictor for Higher Sale Price
##### Housing Space
- Above Grade Living Area
- 1st Floor Squared Feet
- 2nd Floor Squared Feet
- Garage Cars
- Basement Full Bath
- Screen Porch area

##### House Quality
- Overall Quality
- Overall Condition
- Functional
- Exterior Quality
- Basement Qualilty
- Rating of Basement Finish Type 1
- Heating Quality

It should come at no surprise that the sale price of the apartment have strong positive relationship with the space and quality of the apartment. While age of the apartment plays a big part in bringing down the price.
#### Positive features
- Exterior type - Brick Face
- Single-family Detached
- Hillside - Significant slope from side to side
- Proximity to various conditions(Normal)
- New homes

#### Negative features
- Banked - Quick and significant rise from street grade to building
- Exterior type - Asbestos Shingles

Some of the features of the house that could value add to the apartment and some of the features that should be avoided are shown above
#### Neighborhood
- Stone Brook
- Northridge Heights
- Crawford
- Somerset
- Brookside

It seem that there is a preference in the above neighborhood which drive the housing price in these neighborhood higher. Family who are on a budget can focus on finding an apartment in Edwards instead for a bargain.


#### MS Zoning
- Residential Low Density
- Floating Village Residential

While the above zone are fetching a higher price, housing that are within the Commercial zone seem less ideal.
## Recommendation
This model will be able to help both the buyers and the sellers to provide an estimate of the sale price of the houses. Additionally, it also show the buyers and sellers the features that might affect the sale price. This will allow buyers to set a proper budget based on the features or neighborhood that they are interested in while allowing seller to determine areas that they could worked on to improve their house's value.

However, it could be seen that this model will start to diverge at higher prices. Hence, for future improvement. We could attempt to create a second regression model that would help us to more accurately predict housing price for higher end apartment.
