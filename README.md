## FACTORS AFFECTING HOUSE PRICES
[Link to presentation](https://docs.google.com/presentation/d/1X5AKUkKfecgnlAMWa0VvOXkWCgYHlhJ2zEQBVspkMUA/edit?usp=sharing)
### Overview
* Building a multiple linear regression model to help identify factors that greatly affect house prices in order to help improve the real estate business conducted by WON Real Estate Limited 
### Business Understanding

WON Real Estate Limited is a real estate company located in the American Northwest that buys and sells houses to its clients.The company would like to know which factors affect house prices the most in order to consider them when buying and selling the houses and make changes to any houses bought,that don't meet these factors.

This project will help identify these factors  by developing a  model that can estimate the house prices based on its features.The performance of the model will also be evaluated.
### Data understanding

The data used in this project was obtained from [kaggle website](https://www.kaggle.com/datasets/shivachandel/kc-house-data).This dataset contains the prices of houses in the American Northwest and their various features such as the number of bathrooms and the number of bedrooms. Being that the company is also situated in the American Northwest  this data will be of great use 


The dataset contains twenty one columns that are the features (characteristics) of the houses.The model developed in this project will also estimate the prices of houses that are contained in the 'price' column.
### Modelling
Four linear regression models were created in this project.`Model_1` was used to come up with the reccomendations and conclusions since it explained 54% of the variance in price. This was the highest compared to the rest of the models. The models were as follows:
 - `Baseline model`: This was a simple linear regression model that was used to evaluate the performance of the multiple linear regression models.
 - `Model_1`: This model had the highest R_squared compared to the rest of the models.It was used to come up with the recommendations and conclusions.
 - `Model_2`: This was a modification of model_1 with the statistically_insignificant features dropped.
 - `Model_3`: This was modification of model_1 with the target as log_price instead of price.
 - `Model_4`: This was a modification of model_1 with the categories in the grade column reduced to 'ABOVE GRADE','BELOW AVERAGE' and 'AVERAGE'. It turned out to be a poor model compared to model_1
### Regression Results
* Model one has the highest R_squared(0.54) compared to the rest of the models. This will be the preferred model (it explains 54% of the variance in price).
* With alpha is set to 0.05 the model is statistically significant with a p_value of 0.00.
* From model_1 it can be stated that the following features greatly impact the price of a house:
    
    - `Number of bathrooms`: An increase in the number of bathrooms by one is associated with an increase in the house price by  about `$13604`.
    - `The living space`: An increase in living space by one square foot is associated with an increase in the house price by about `$61037`. 
    - `The number of floors` : An increase in the number of floors by one is associated with an increase in price by about `$12189`.
    - `The year the house was built` : An increase in the year a house was built corresponds to a decrease in the house price by `$77775`.
     - `The lot size`: An increase in lot size by one square foot is associated with a decrease in the house price by about `$24333`.
    - `Whether kind of view the house has` : When a house has no view compared to houses with no view,there is an associated decrease in the house price by `$12415`.
    - `The condition of the house` : Compared to houses with an average condition,houses with a very good condition have an associated increase in price by about `$11556`.
    - `The grade of the house` i.e. its construction and design : Compared to houses with average grade,houses with a Better condition have an associated increase in price by `$63230`.
    - `Whether the house has a basement or not` : Houses with a basement have an associated decrease in price by about `$9506` compared to those with no basement.
    - `The season the house was sold`: Houses sold during spring have an associated increase in price by about `$11566` compared to those sold during autumn.
    - `Number of bedrooms`: An increase in the number of bedrooms is associated with a decrease in house price by about `$12187`.
    
### Conclusions
* Houses sold during spring go at higher prices.
* Vintage (old) houses are sold at higher prices.
* Houses with a good grade are sold at higher prices.
* Houses with a better condition go at higher prices.
### Recommendations
* The company should sell its houses during the spring season since houses go at higher prices during this season.
* The company should ensure that they buy houses with a good grade in order to sell them at higher prices.
* Older houses go at higher prices the company should focus on buying vintage houses in order to sell them at higher prices to gain more profits.
* To clinch more profits the company might consider buying houses with an average condition and improving the house condition. This will enable the house to be sold at a much higher price hence higher profits.
