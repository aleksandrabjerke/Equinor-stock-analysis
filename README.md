# Equinor Stock Analysis

Stocks have never been more unpredictable than in today's political climate. 
Wars, OPEC decisions, and currency fluctuations all move markets in ways that 
are difficult to model. So I tried anyway.

## What is this?
This project investigates whether oil prices can explain and predict Equinor's 
stock price - using linear regression, Ridge/Lasso regularization, and Random 
Forest classification.

## What I found
- Oil prices explain ~30% of Equinor's stock price movements (R² = 0.308)
- The model is stable - similar performance on both training and test data
- Lasso automatically removed currency as a variable, confirming oil price is 
  the dominant factor
- Predicting the direction of tomorrow's price? Barely better than a coin flip (53%)

## Limitations
70% of stock price variation is unexplained - market sentiment, geopolitical 
events, and investor behavior all play a role that simple macro variables 
can't capture. Turns out the market doesn't care much about our models.

## Tech
Python, pandas, scikit-learn, yfinance, matplotlib
