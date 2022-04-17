# Analyzing Portfolio Risk and Return
Quantitative analyst for a FinTech investing platform. This platform aims to offer clients a one-stop online investment solution for their retirement portfolios that’s both inexpensive and high quality. To keep the costs low, the firm uses algorithms to build each client's portfolio. The algorithms choose from various investment styles and options evaluating four new investment options for inclusion in the client portfolios. Legendary fund and hedge-fund managers run all four selections. (People sometimes refer to these managers as **whales**, because of the large amount of money that they manage). 
## Technologies

- Jupyter notebook
- Pandas library for data analysis, and visualizations.
- Pathlib to import the csv file.
- Numpy

### Resources

* read_csv: CSV file that contains bitcoins timestamp informations for the analysis.
---

## Usage:
> To open this file you must have installed in your machine juppyter notebook or jupyter lab or other software. for more info visit https://jupyter.org/

### 1. Performance Analyze
Analyze the data to determine if any of the portfolios outperform the broader stock market, which the S&P 500 represents. 

- Pandas `plot` function to visualize the daily return data of the four fund portfolios and the S&P 500.
- Pandas `cumprod` function to calculate the cumulative returns for the four fund portfolios and the S&P 500.
- Pandas `plot` to visualize the cumulative return values for the four funds and the S&P 500 over time.

---

### 2. Analyze the Volatility
- Pandas `plot` function and the `kind="box"` parameter to visualize the daily return data for each of the four portfolios and for the S&P 500 in a box plot.

---

### 3. Analyze the Risk

Evaluate the risk profile of each portfolio by using the standard deviation and the beta. To do so, complete the following steps:

1. Pandas `std` function to calculate the standard deviation for each of the four portfolios and for the S&P 500. 
2. Calculated the annualized standard deviation for each of the four portfolios and for the S&P 500. 
3. Used the daily returns DataFrame and a 21-day rolling window to plot the rolling standard deviations of the four fund portfolios and of the S&P 500 index.
4. Used the daily returns DataFrame and a 21-day rolling window to plot the rolling standard deviations of only the four fund portfolios. 

---

### 4. Analyze the Risk-Return Profile
To determine the overall risk of an asset or portfolio, quantitative analysts and investment managers consider not only its risk metrics but also its risk-return profile. 

1. Used the daily return DataFrame to calculate the annualized average return data for the four fund portfolios and for the S&P 500. Used 252 for the number of trading days. 
2. Calculated the Sharpe ratios for the four fund portfolios and for the S&P 500. To do that, divide the annualized average return by the annualized standard deviation for each. 
3. Visualized the Sharpe ratios for the four funds and for the S&P 500 in a bar chart. 

---

#### 5. Diversify the Portfolio
How the portfolios react relative to the broader market. Based on the analysis so far,  for that i choose two portfolios that likely to recommend as investment options

1. Use the Pandas `var` function to calculate the variance of the S&P 500 by using a 60-day rolling window. 

2. Next, for each of the two portfolios:

    * Used the 60-day rolling window, the daily return data, and the S&P 500 returns, calculate the covariance.
    * Calculated the beta of the portfolio. To do that, divide the covariance of the portfolio by the variance of the S&P 500.
    * Used the Pandas `mean` function to calculate the average value of the 60-day rolling beta of the portfolio.
    * Ploted the 60-day rolling beta. 

--- 

##  Contributors
Brought to you by Carlos Polanco.

- Email: carlos.polanco0508@gmail.com
- GithubProfile: https://github.com/carlosmpr
- Linkedin: https://www.linkedin.com/in/carlosmpr/

---

## License

MIT

Copyright (c) 2012-2022

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.