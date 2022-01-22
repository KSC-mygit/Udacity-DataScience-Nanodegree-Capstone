# Udacity_DataScience_Nanodegree_Capstone
Capstone project of Udacity Data Scientist Nanodegree

This Capstone project is completed as part of the curriculum for the Udacity Data Scientist Nanodegree Program. In this project I create a stock price predictor that generates a stock price for given stock or list of stocks as of a given date predicted over a specified forecast interval.

## Libraries used
 * yfinance
 * re
 * numpy
 * pandas
 * sklearn
 * datetime
 * matplotlib
 * seaborn
 * math

## Data
In this analysis I used the yfinace which provides an API to download stock prices from Yahoo Finance. 
Run ```! pip install --upgrade pip``` before running ```! pip install yfinance``` if ```yfinance``` is not installed in your environment.

## Getting Started
1. Run all the in the code in the accompaning jupyter notebook until just before the **USER INTERFACE** section. This initializes all the classes, functions and objects required to proceed further.
2. Follow the steps in the **USER INTERFACE** section of the jupyter notebook to supply the inputs needed to generate your prediction. The following will be requested for input:
    * list of tickers (a list of tickers from the S&P 500 is provided to pick examples from, if you do not already ones in mind)
    * the start date and end date of the training period of your choice based on available data from Yahoo Finance
    * the number of days for the forcast interval
    * and finally, the specific date you wish you generate a prediction for

## Four different regression models were used as follows:
    * Linear Regression
    * Kernel Ridge Regression
    * Stochastic Gradient Descent Linear Regression
    * Linear Support Vector Regression    
    
## Prediction Process:
The following steps will be followed:
1. User inputs one or more ticker symbols
2. Dowload the available historical stock price data from Yahoo Finance
3. User specifies the training period
4. User specifies the forecast interval
5. Train the 4 models indicate above and test them to determine the best one for each ticker - the one with the least root mean squared error (RMSE)
6. User specifies the date the prediction should be generated for from a range of dates in the period that is subsequent to the training period specified in step. 3 above
7. Generate a prediction and compute the error and absolute error relative to the actual observed price and display the results.

## Further Reference
For more information on my analysis please read the accompanying blogpost on Medium which can be found at the following link: https://medium.com/p/af90a9ac4cb0/edit

## Acknowledgements
Special thanks to Yahoo Finance for the free API that allows for easy download of the stock price data used in this analysis

## Contribution
Contibutions to this project are welcome!
