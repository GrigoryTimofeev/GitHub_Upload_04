# Module-4-Challenge - Analyzing Portfolio Risk and Return

In Module 4 Challenge FinTech Columbia University Boot Camp we created application to analyse 4 whale funds for S&P 500 market data to provide a service of recommendation how a fund to be included for retirees.

![Portfolio](pic.PNG)

---

## The Challenge description

As a quantitative analyst for a FinTech investing platform, you've been tasked with evaluating four new investment options for inclusion in the client portfolios. You’ll need to determine the fund with the most investment potential based on key risk-management metrics: the daily returns, standard deviations, Sharpe ratios, and betas.

This Fintech investing platform aims to offer clients a one-stop online investment solution for their retirement portfolios that’s both inexpensive and high quality. 

---

## The Goals

* The data to be acceptable in csv format  

* Ablility to clean data by:  
    * Improve data set by Removing NaN data items  

* Data Analysis covering:
    * Calculate Volatility: using box plots of daily percent returns information 
    * Calculate Performance: using cumulative daily percent returns information
    * Calculate Risk: using standard deviation / annualized standard deviation with rolling window of 21 days
    * Define Risk/Return: using Sharpe Ratios 
    * Analyse Sensitivity to Market: using Betas with rolling window of 60 days for the fund for the market
    
---

## The Workflow of the application  


* Data Collection - read in the csv data file from **whale_navs.csv**. 

* Data Preparation - 
    * index data by Date/Timestamp
    * show the trade data as daily percent returns using pct_change()
    * improve data set - remove NaN

* Data Analysis -
    * Performance: find a fund which performed better than S&P 500
        * calculate dailiy returns 
        * calculate cumulative returns
    
    * Volatility: find the most & least volatile funds by relative volatility
        * explore box plots
    
    * Risk: compare portfolio risk with the market
        * calculate portfolio standard deviation
        * use a window of 21 days, with and without the market data
    
    * Risk/Return: find a fund offers the best returns
        * Sharpe Ratios 
        * Plot Sharpe Ratios in a Bar plot
    
    * Sensitivity to Market: find the fund sensitivity to S&P 500
        * Calculate Betas in window of 60 days
        
---

## Technologies

Python 3.7.11 with additional libraries:

Install the Fire and Questionary libraries executing following commands:

```python
  pip install fire
  pip install questionary
```
---

## Usage

The following details the instructions on how to run the application.  

### Run the Application

[click here for information on Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/).  

Run **risk_return_analysis.ipynb** file.  

---

## Contributors

Grigory Timofeev

[E-mail](fintech_github_challenge4@unloca.com)

---

## License

The MIT License (MIT)

Copyright (c) 2022 Grigory Timofeev

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.