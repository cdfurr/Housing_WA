# Housing in Washington State

# Business Understanding
Daniel's Inc. is a residential real estate investment company that operates nationally. They would like to pierce the housing market in King County which is located in Washington State. They want to select houses that are rent ready and will gain a great return on investment in the distant future.

# Data Understainding
The data was gathered from info.kingcounty.gov focusing on the years of 1900-2015.

The csv has 21 columns and 21,597 rows.

It contains the following features:

id
date
price
bedrooms
bathrooms
sqft_living
sqft_lot
floor
waterfront
view
condition
grade
sqft_above
sqft_basement
yr_built
yr_renovated
zipcode
lat
long
sqft_living15
sqft_lot15

# Business Problem
## Inital questions
- Is there a yr_built in which a house should not be bought?
- What is the relationship between sqft_living and price?
- what is the relationship between sqft_above and price?
- How do the variables listed in the data understanding section affect the recommendations presented?

# Baseline Model
Two baseline models were created to try and understand the correlation between sqft living and price, and sqft living above and price. 

# Final Model
The final showed:
- R2: 78.2% of the variance in the y variable is described by the x variables.
- P-Value: there are a few features in the model that have a pvalue greater than alpha which make them not statitically significant with majority being located in the cities.
- Coefficients: there are coefficients that have a negative impact of the y-variable with a unit increase.e.g. "long", "population", "bedrooms".

With the final model we were able to graph the significance of a neighborhoods average sale price.

![](Images/pic1.png)

Also, the significance of a neigborhoods average grade on house quality.

![](Images/pic2.png)

Finally, the average sqft of the top fifteen neighborhoods.

![](Images/pic3.png)

# Conclusion
Throughout this housing data modeling process, we ran two baseline models with the two highest correlating X variables to the Y variable and two kitchen sink models that showed promise. In the first kitchen sink model we were accounting for living space in two columns and individual zipcodes which skewed the data. In the second kitchen sink model we drop these three columns and got a better depicition of the data. We can see that location, size of the living space, grade and year built or recently renovated has a positive impact on the price of the house. All of these reasons support why this model would be beneficial to our investors and their real estate investment endeavor.