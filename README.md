

# PREDICTIVE ANALYSIS IN PROPERTY VALUATION

## INTRODUCTION
King County is situated in the Northwestern part of the United States and encompasses the city of Seattle, which is a major economic and cultural hub in the region.
With a population of 2,269,675 in the 2020 census,King County is the most populous county in Washington, and the 12th most populous county in the United States. 
The County has a total land area of 2,130 square miles (1,363,200 acres). About 90% of King County's population lives in cities, while about 246,000 residents live in the unincorporated area. [King County.gov](https://kingcounty.gov/en/dept/executive/governance-leadership/performance-strategy-budget/regional-planning/demographics). 

King County experienced an 18% increase in population growth between 2010 and 2020. Due to this, the housing market in King County has experienced significant growth and changes over the years. 
As the region's economy thrived, King County experienced substantial population growth. This influx of residents led to increased demand for housing, both in urban and suburban areas. Seattle, with its iconic skyline, became a sought-after destination for tech professionals and urban enthusiasts.The real estate market in King County is known for its competitiveness.The region's diverse neighborhoods offer a range of housing options, from historic homes in older districts to modern developments in suburban areas.


#### AUTHORS

- [Jonquil Phelan](https://github.com/phelanthropus),  [George Mbugua](https://github.com/georgembugua00), [Vincent Kiplangat](https://github.com/VincentKiplangat), [Kenneth Gakuru](https://github.com/KennethGakuru), [Fanice Andayi](https://github.com/Fanice-Andayi), [Wallace Ouma](https://github.com/WKalawi), [Ian Odhiambo](https://github.com/ian-obotey), [Charles Gaithuma](https://github.com/CKGaithuma), [Brenda Ngigi](https://github.com/Bree-009)

  
## OVERVIEW
This project is centered on the development of a multiple linear regression model with the primary objective of predicting property prices in the real estate market. The focal point of this analysis is the dependent variable, "price," while the independent variables encompass a comprehensive range of property characteristics. These characteristics include, but are not limited to, the number of bedrooms, year built, number of floors in the home, total living space area in square feet, overall condition of the home, and the geographical location of the property.

Real estate agencies play a critical role in assisting homeowners with crucial decisions related to buying, selling, or renting properties. This project introduces a powerful tool for empowering real estate agencies – a regression-based model designed to predict potential increases in property value. This model relies on various features influenced by property characteristics, including the number of bedrooms, year built, number of floors, total living space area in square feet, overall condition of the home, and the location.

## BUSINESS AND DATA UNDERSTANDING

### OBJECTIVES
The primary goal of this project is to provide real estate agencies with a robust predictive tool, enabling them to offer tailored advice to clients. By leveraging regression analysis, the model can estimate potential increases in property value based on key features. This empowers agencies to guide homeowners in making informed decisions that maximize returns on investment in the highly competitive real estate market.

## MODELING


## REGRESSION RESULTS
Model 3 is the preferred model beacuse:
From the evaluation metrics, we can see that the models have close performance in terms of MAE and RMSE. However, Model 3, which includes log transformations has the highest R-squared value and the lowest AIC and BIC values among the models. Therefore, Model 3 is the best model among the ones considered.

- Consider investing in properties with the basement
- The further  from seattle the cheaper the houses
- The more the bedrooms the more expensive the house
- The more space/land a house occupies,the more expensive it is
- Square Footage of Living Space: The square footage of living space has a positive impact on house prices. As the size of the living space increases, the estimated price of the house also increases. This indicates that larger houses are generally priced higher.
- As the age of the house increases, the estimated price also increases. This could be due to factors such as historical significance or architectural value associated with older houses.
## CONCLUSION
**RECOMMENDATIONS**

- Feature Enhancement: Consider enhancing or upgrading the features that positively affect house prices. For example, increasing the square footage of the living area, improving the overall grade of the property, or adding more bathrooms can potentially increase the value of the house.

- Data Collection: Consider collecting additional relevant data that could improve the accuracy of the regression model. This may include variables such as location-specific factors, proximity to amenities, property age, or neighborhood characteristics.

- Market Segmentation: Analyze the relationship between the independent variables and house prices to identify market segments or specific buyer preferences. For instance, if higher-grade houses tend to have higher prices, it may indicate a market segment of luxury or high-end properties.

**LIMITATIONS**

Limited Handling of Non-Linearity:

Issue: If the relationship between predictors and the response is highly non-linear, multiple linear regression may not capture these complexities effectively.
Impact: The model may fail to capture important patterns in the data, leading to inaccurate predictions.

Causation vs. Correlation:

Issue: Correlation between variables does not imply causation. Even if variables are correlated, it does not necessarily mean that changes in one variable cause changes in another.
Impact: The model may identify associations but cannot establish causal relationships.

Assumption of Independence:

Issue: Multiple linear regression assumes that observations are independent of each other.
Impact: Violation of independence assumptions may lead to biased standard errors and affect the validity of statistical tests.

Linearity Assumption:

Issue: Multiple linear regression assumes a linear relationship between the independent variables and the dependent variable. If the true relationship is not linear, the model may not capture the underlying patterns accurately.
Impact: It may lead to biased predictions and inaccurate estimates of the coefficients.

**NEXT STEPS**

Explore Alternative Models:

Consider exploring more complex models that can capture non-linear relationships, interactions, and other complexities in the data. Examples include random forests and neural networks.

Time Trends and Seasonality:

If time trends or seasonality are relevant, explore time series models or include time-related features to better capture temporal patterns.

Regular Monitoring:

Implement regular monitoring and updates to the model. As new data becomes available, retrain the model periodically to ensure it remains relevant and effective.
