# Home Price Prediction Data Analysis
## Overview

This project aims to analyze the factors influencing home prices in the United States using data science techniques. We explore various economic indicators such as the Consumer Price Index (CPI), median household income, unemployment rate, interest rate, and housing starts to understand their impact on home prices over the past two decades. We build and evaluate predictive models using linear regression and random forest regression algorithms to forecast home prices based on these factors.


## Data Sources

The primary data sources used in this analysis are:

S&P Case-Shiller Home Price Index (CSUSHPISA) from Federal Reserve Economic Data (FRED)

30-Year Fixed Mortgage Rate (MORTGAGE30US) from FRED

Unemployment Rate (UNRATE) from FRED

Median Household Income (MEHOINUSA672N) from FRED

Housing Starts (HOUST) from FRED

Consumer Price Index (CPIAUCSL) from FRED

## Methodology

1. Data Collection: Fetch data from FRED API for each economic indicator.

2. Data Preprocessing:
Resample all datasets to monthly frequency.
Forward-fill missing values to ensure uniform time series data.
Merge all datasets into a single DataFrame.
Drop any remaining NaN values.

3. Model Building:
Split the data into training and testing sets.
Train linear regression and random forest regression models using the training data.

4. Model Evaluation:
Calculate Mean Squared Error (MSE) for each model to assess predictive accuracy.
Calculate R-squared to measure the goodness of fit of the models.

5. Feature Importance Analysis:
Determine the importance of each feature in predicting home prices using the random forest model.

### Results

1. Linear Regression MSE: 131.88
2. Random Forest MSE: 2.29
3. Linear Regression R-squared: 0.85
4. Random Forest R-squared: 0.98

The random forest model outperforms the linear regression model with significantly lower MSE and higher R-squared values, indicating better predictive accuracy and model fit.

## Conclusion

The analysis reveals that economic indicators such as CPI, median household income, and unemployment rate have a significant impact on home prices. Policymakers, real estate professionals, and investors can leverage these insights to make informed decisions regarding housing market trends, investment strategies, and economic forecasts.
    