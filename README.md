
# PREDICTIVE ANALYSIS IN PROPERTY VALUATION
![banner](https://github.com/Bree-009/PREDICTIVE-ANALYSIS-IN-PROPERTY-VALUATION/blob/main/read%20me%20banner.jpg)

## INTRODUCTION
King County is situated in the Northwestern part of the United States and encompasses the city of Seattle, which is a major economic and cultural hub in the region.
With a population of 2,269,675 in the 2020 census,King County is the most populous county in Washington, and the 12th most populous county in the United States. 
The County has a total land area of 2,130 square miles (1,363,200 acres). About 90% of King County's population lives in cities, while about 246,000 residents live in the unincorporated area; [King County.gov](https://kingcounty.gov/en/dept/executive/governance-leadership/performance-strategy-budget/regional-planning/demographics). 

King County experienced an 18% increase in population growth between 2010 and 2020. Due to this, the housing market in King County has experienced significant growth and changes over the years. 
As the region's economy thrived, King County experienced substantial population growth. This influx of residents led to increased demand for housing, both in urban and suburban areas. Seattle, with its iconic skyline, became a sought-after destination for tech professionals and urban enthusiasts.The real estate market in King County is known for its competitiveness.The region's diverse neighborhoods offer a range of housing options, from historic homes in older districts to modern developments in suburban areas.


#### AUTHORS

- [Jonquil Phelan](https://github.com/phelanthropus),  [George Mbugua](https://github.com/georgembugua00), [Vincent Kiplangat](https://github.com/VincentKiplangat), [Kenneth Gakuru](https://github.com/KennethGakuru), [Fanice Andayi](https://github.com/Fanice-Andayi), [Wallace Ouma](https://github.com/WKalawi), [Ian Odhiambo](https://github.com/ian-obotey), [Charles Gaithuma](https://github.com/CKGaithuma), [Brenda Ngigi](https://github.com/Bree-009). 

  
## OVERVIEW
This project is centered on the development of a multiple linear regression model with the primary objective of predicting property prices in the real estate market. The focal point of this analysis is the dependent variable, "price", while the independent variables encompass a comprehensive range of property characteristics. These characteristics include, but are not limited to, the number of bedrooms, year built, number of floors in the home, total living space area in square feet, overall condition of the home, and the geographical location of the property.

## DEPENDENCIES
- python3

- numpy

- pandas

- seaborn

- sklearn

- statsmodels

- matplotlib

- scipy

## NOTEBOOK STRUCTURE 

1. Overview

2. Business Understanding

3. Data Understanding

4. Data Cleaning

5. Statistical Analysis

6. Data Preparation

7. Modelling

8. Regression Results

9. Conclusion - Recommendations,Limitations and Next Steps

## BUSINESS UNDERSTANDING
### *Stakeholders and Their Interests:* ###
The key stakeholders impacted by this project are Real Estate Agencies. Their interest is accurate pricing and having a competitive advantage and the value they seek is Improved decision making and client satisfaction.

**Benefits for Real Estate Agencies:**

- *Informed Decision-Making*: Agencies can provide clients with data-driven insights, enhancing the decision-making process.
- *Tailored Advice*: Customized recommendations based on the unique features of each property.
- *Maximized Returns*: Clients can make decisions that optimize return on investment in the competitive real estate market.

### OBJECTIVES ###
#### - Main Objective: ####
The main objective of this project is to develop a predictive regression model that assists real estate agencies in advising clients on house prices. The model aims to predict the potential variation in property value based on property characteristics, providing valuable insights to guide clients in making informed decisions about their investments.

#### - Specific Objectives ####

i). Identify Key Factors Influencing House Prices in King County, California, to provide valuable insights for precise pricing strategies.

ii). Analyze Model Performance using metrics such as mean squared error, R-squared values, and residual analysis to gauge the model's effectiveness.

iii). Provide Actionable Recommendations to the Real Estate Agency for improving profitability and market presence, leveraging insights from the model.

## DATA UNDERSTANDING 
-The data utilized for this project has been sourced from [Kaggle](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)

### Data Source: ###
The dataset used for this project is the King County House Sales dataset, which is available in the **kc_house_data.csv file**.
The dataset contains information about house sales in King County, providing details such as property features, location, sale prices, and renovation-related variables.

### Data Size: ###
The kc_house_dataset contains *21597 rows* and *21 columns*.
The columns include :
* `id` - Unique identifier for a house
* `date` - Date house was sold
* `price` - Sale price 
* `bedrooms` - Number of bedrooms
* `bathrooms` - Number of bathrooms
* `sqft_living` - Square footage of living space in the home
* `sqft_lot` - Square footage of the lot
* `floors` - Number of floors in house
* `waterfront` - Whether the house is on a waterfront
* `view` - Quality of view from house
* `condition` - How good the overall condition of the house is. Related to maintenance of house.
  
  And several other columns.

### Data Types: ###
The data types include categorical and numerical variables.
Columns with categorical variables include, date, waterfront, view, condition, grade and sqft_basement while columns with numerical variables include id, price, bedrooms, bathrooms, sqft_living, sqft_lot, floors, yr_built, yr_renovated, zipcode, lat, long, sqft_above, sqft_living15 and sqft_lot15.

### Data Cleaning and Pre-Processing ###
Data was cleaned to address issues related to the quality of the dataset. 
The following outlines data cleaning and preparation methods implemented during the project:
- Handling Missing Values.

- Handling Duplicates.

- Dealing with placeholders.

- Transforming data.

- Handling Outliers.


## MODELING
**Model Performance:**
Model with Log-Transformed Target - MSE: The model's predictions have an MSE of approximately 35.1 billion.
Model with Log-Transformed Target - R-squared: 0.761
The R-squared value gauges how well the model explains the variance in the target variable. A value of 0.761 indicates that approximately 76.1% of the variability in the target variable (price) is accounted for by the model.

**Model Coefficients:**
- sqft_living: The coefficient is 0.000222.
For each one-unit increase in sqft_living, the predicted log-transformed price increases by 0.000222.
bedrooms: The coefficient is -0.0272.
Each additional bedroom correlates with a decrease of approximately 0.0272 in the predicted log-transformed price.
- bathrooms: The coefficient is 0.0012.
The small and statistically insignificant (high p-value) coefficient suggests that the number of bathrooms might not significantly impact the log-transformed price in this model.
- grade: The coefficient is 0.1985.
For each one-unit increase in the grade, the predicted log-transformed price increases by 0.1985.
-condition: The coefficient is 0.1041.
Each one-unit increase in condition corresponds to a predicted log-transformed price increase of 0.1041.

**OLS Regression Results:**
R-squared: 0.761
The R-squared value remains consistent with the model's R-squared, indicating similar performance in both log-transformed and original scale.
F-statistic: 4637 with a low p-value.
The overall model is statistically significant.
Interpretation:
The log transformation of the target variable has notably improved the model's performance, evident in the lower MSE and higher R-squared compared to the model without log transformation. This transformation appears to have effectively captured underlying data patterns, enhancing the model's predictive accuracy.

## REGRESSION RESULTS

Model 3 is the preferred model beacuse:
From the evaluation metrics, we can see that the models have close performance in terms of MAE and RMSE. However, Model 3, which includes log transformations has the highest R-squared value and the lowest AIC and BIC values among the models. 

- Consider investing in properties with the basement
- The further  from seattle the cheaper the houses
- The more the bedrooms the more expensive the house
- The more space/land a house occupies,the more expensive it is
- Square Footage of Living Space: The square footage of living space has a positive impact on house prices. As the size of the living space increases, the estimated price of the house also increases. This indicates that larger houses are generally priced higher.
- As the age of the house increases, the estimated price also increases. This could be due to factors such as historical significance or architectural value associated with older houses.

## CONCLUSION
### RECOMMENDATIONS 

- Feature Enhancement: Consider enhancing or upgrading the features that positively affect house prices. For example, increasing the square footage of the living area, improving the overall grade of the property, or adding more bathrooms can potentially increase the value of the house.

- Data Collection: Consider collecting additional relevant data that could improve the accuracy of the regression model. This may include variables such as location-specific factors, proximity to amenities, property age, or neighborhood characteristics.

- Market Segmentation: Analyze the relationship between the independent variables and house prices to identify market segments or specific buyer preferences. For instance, if higher-grade houses tend to have higher prices, it may indicate a market segment of luxury or high-end properties.

### LIMITATIONS

**- Limited Handling of Non-Linearity:**

Issue: If the relationship between predictors and the response is highly non-linear, multiple linear regression may not capture these complexities effectively.
Impact: The model may fail to capture important patterns in the data, leading to inaccurate predictions.

**- Causation vs. Correlation:**

Issue: Correlation between variables does not imply causation. Even if variables are correlated, it does not necessarily mean that changes in one variable cause changes in another.
Impact: The model may identify associations but cannot establish causal relationships.

**- Assumption of Independence:**

Issue: Multiple linear regression assumes that observations are independent of each other.
Impact: Violation of independence assumptions may lead to biased standard errors and affect the validity of statistical tests.

**- Linearity Assumption:**

Issue: Multiple linear regression assumes a linear relationship between the independent variables and the dependent variable. If the true relationship is not linear, the model may not capture the underlying patterns accurately.
Impact: It may lead to biased predictions and inaccurate estimates of the coefficients.

### NEXT STEPS

1. Consider exploring more complex models that can capture non-linear relationships, interactions, and other complexities in the data. Examples include random forests and neural networks.

2. If time trends or seasonality are relevant, explore time series models or include time-related features to better capture temporal patterns.

3. Implement regular monitoring and updates to the model. As new data becomes available, retrain the model periodically to ensure it remains relevant and effective.



