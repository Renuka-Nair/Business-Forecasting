# Business Forecasting - Harmonized Index of Consumer Prices: Sugar, Jam, Honey, Chocolate, and Confectionery for Norway

## Introduction
1. This project is to forecast the HICP value for the basket goods mentioned above in Norway by processing the data from 2010 till August 2021. The index tracks the prices of goods such as coffee, tobacco, meat, fruit, household appliances, cars, pharmaceuticals, electricity, clothing and many other widely used products. Thus it is also used as an Inflation Measure in the euro area and forecasting HICP can be used to understand inflation rates in the area.

2. The project forecast could be a Point forecast along with a confidence interval for HICP in the next year (2022).

3. The accuracy of the forecast will be measured using one the below measures : <br />
MAD  Mean Absolute Value <br />
MSE Mean Squared Error <br />
RMSE Root Mean Squared Error <br />
MAPE Mean Absolute Percentage Error <br />
MPE Mean Percentage Error <br />
We are leaning more towards using RMSE as an accuracy measure as we would like an accuracy measure that would penalise us for errors in this particular prediction.

4. The data was obtained from the economic research website FRED. (https://fred.stlouisfed.org/series/CP0118NOM086NEST)
The frequency of the data is monthly starting from 2010 till 2021 August. The Harmonized Index of Consumer Prices category "Sugar, Jam, Honey, Chocolate, and Confectionery (01.1.8)" is a classification of nondurable goods that includes cane or beet sugar, unrefined or refined sugar, powdered sugar, crystallized sugar, or sugar lumps; jams, marmalades, chocolates etc. 

## Team Members 

Nishit Pabari https://github.com/n1sh1t9
William Cardona https://github.com/Wcard625  

## Models 

The project compared various models and below are some of the important ones : <br />
1) Naive <br />
2) ETS <br />
3) Moving Averages <br />
4) Holt-Winters <br />
5) ARIMA <br />

## Conclusion 

At the end of the project, we gained enough insights to conclude that Holt-Winters/ARIMA are the best models for this particular prediction as they gave a decent RMSE value (if not the best) and also gave satisfactory residual analysis. The FRED website now has the most recent HICP values for September, October and November 2021 that were not there previously. If we compare these values to the forecast outputs of ARIMA and Holt-Winters, we can see the predictions are pretty spot on. <br />
 Month         |  Actual HICP   | Holt-Winters  | ARIMA <br />
---------------|----------------|---------------|-------
Sep-21         |      97.6      |    96.7       |  97.2  <br />
Oct-21         |      96.2      |    95.5       |  96.1  <br />
<br />

