# Project 2: Ames, Iowa Housing Price Analysis


### Problem Statement

The purpose of this analysis of housing prices in Ames, Iowa is to understand the key factors that influence the housing prices in the area and to develop a model that can accurately predict the value of a given property based on its features. This analysis will help developers better understand the local market and make informed decisions about buying, selling, or investing in properties in Ames, Iowa.

At the end of this report, I will provide recommendations based on the analysis undertaken, as determined by the the success of the model. This success will be determined by a number of statistical factors, including Root Mean Squared Error and R2 value, as they both provide a human interpretable comparison between our two data sets.

My goal is to provide the board with a model that is more accurate that the null model. This information will inform the board's direction as they aim to improve available housing for the residents of Ames.

### Conclusion

The dataset was imperfect and needed a significant amount of cleaning to make it usable for the stated purpose. Null values were handled accordingly as stated in the data dictionary. The type of data that the null represented dictated what type of action was taken. These null values created a limitation in the data and created outliers that were difficult to handle without creating issues within our model

Additional data regarding the surrounding features would further improve the model, as most of the features pertained to the homes themselves, rather than the auxillary features of the region (flood levels, natural disaster propensity, proximity to critical facilities, etc.). Within my analysis, I identified several features that are valuable in predicting the price of a home in the area. Those features are, but not limited to:

 - Neighborhoods: Green hills, StoneBrook, and Northridge
 - 2.5 storey homes (finished)
 - Wood shingle Roofs
 
 Features that show a negative correlation with price:
 
 - Elevators (Misc. Feature)
 - Composite shingle roofs
 - Homes in the Meadow Valley neighborhood
 
 
### Recommendations

* As stated in the conclusion, more data regarding regional features would likely improve the model, all things equal
* This model is unlikely to provide useful analysis for areas outside of Ames. This is due to the significant impact the Neighborhood features had in the results
* This model will predict home values more precisely within a given neighborhood, rather than generalized throughout the city


### Data Dictionary

Below is a summary and dictionary of the data I analyzed

https://jse.amstat.org/v19n3/decock/DataDocumentation.txt


### Ames, Iowa Data

| Feature | Type | Dataset | Description |
| --- | --- | --- | --- |
| SalePrice | Numeric | Ames Housing Dataset | The property's sale price in US dollars |
| LotArea | Numeric | Ames Housing Dataset | The size of the lot in square feet |
| OverallQual | Categorical/Ordinal | Ames Housing Dataset | Overall material and finish quality of the house on a scale of 1-10, with 10 being the best |
| OverallCond | Categorical/Ordinal | Ames Housing Dataset | Overall condition rating of the house on a scale of 1-10, with 10 being the best |
| YearBuilt | Numeric | Ames Housing Dataset | The year the house was built |
| YearRemodAdd | Numeric | Ames Housing Dataset | The year the house was remodeled or had additions made |
| MasVnrArea | Numeric | Ames Housing Dataset | Masonry veneer area in square feet |
| TotalBsmtSF | Numeric | Ames Housing Dataset | Total square footage of basement area |
| 1stFlrSF | Numeric | Ames Housing Dataset | Total square footage of first floor area |
| 2ndFlrSF | Numeric | Ames Housing Dataset | Total square footage of second floor area |
| GrLivArea | Numeric | Ames Housing Dataset | Above grade (ground) living area square footage |
| FullBath | Numeric | Ames Housing Dataset | Number of full bathrooms in the house |
| HalfBath | Numeric | Ames Housing Dataset | Number of half bathrooms in the house |
| BedroomAbvGr | Numeric | Ames Housing Dataset | Number of bedrooms above ground |
| KitchenAbvGr | Numeric | Ames Housing Dataset | Number of kitchens above ground |
| TotRmsAbvGrd | Numeric | Ames Housing Dataset | Total rooms above ground, excluding bathrooms |
| Fireplaces | Numeric | Ames Housing Dataset | Number of fireplaces in the house |
| GarageCars | Numeric | Ames Housing Dataset | Size of garage in car capacity |
| GarageArea | Numeric | Ames Housing Dataset | Size of garage in square feet |
| MoSold | Categorical/Nominal | Ames Housing Dataset | Month of sale |
| YrSold | Numeric | Ames Housing Dataset | Year of sale |
| Neighborhood | Categorical/Nominal | Ames Housing Dataset | Physical locations within Ames city limits |
| MSSubClass | Categorical/Nominal | Ames Housing Dataset | The building class |
| HouseStyle | Categorical/Nominal | Ames Housing Dataset | Style of dwelling |
| ExterQual | Categorical/Ordinal | Ames Housing Dataset | Evaluates the quality of the material on the exterior of the house on a scale of Excellent, Good, Average/Typical, Fair, Poor |
| ExterCond | Categorical/Ordinal | Ames Housing Dataset | Evaluates the present condition of the material on the exterior of the house on a scale of Excellent, Good, Average/Typical, Fair, Poor |
| HeatingQC | Categorical/Ordinal | Ames Housing Dataset | Heating quality and condition |
| CentralAir | Categorical/Nominal | Ames Housing Dataset | Central air conditioning |
| Electrical | Categorical/Nominal | Ames Housing Dataset | Electrical system |
| BsmtQual | Categorical/Ordinal | Ames Housing Dataset | Evaluates the height of the basement on a scale of Excellent (100+ inches), Good (90-99 inches), Typical (80-89 inches), Fair (70-79 inches), Poor (<70 inches), No Basement |


#### References

1. ScienceDirect article: "Real estate appraisal by hybrid model for outlier detection and feature selection: A comparative analysis"
2. Medium article: "Data Modeling: Building a House Price Prediction Model"
3. Towards Data Science article: "Create a Model to Predict House Prices using Python"
