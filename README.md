# Challenge 4 Analyzing Portfolio Risk and Return

## Introduction
In this challenge we will further explore Jupyter Notebook and pandas by analyzing performance, volatility, risk, and risk-return of four funds.

## Analysis
We will be comparing four funds and using the S&P 500 to represent the overall market.

```
daily_pct = whale_df.pct_change().dropna()
daily_pct.head()
```
![daily_return](/Images/daily_return.PNG)

Here we convert the data from daily values to the daily change in percentage. To better visualize the information we put it into a graph.

```
daily_pct.plot(figsize=(20,15), title= 'Whale Daily Pct Change')
```

![daily_return_graph](/Images/daily_return_graph.PNG)

## Head to Head Comparison
We finish with comparing Berkshire Hathaway with Paulson & Co, as they were the most and least volatile respectively.  Here we show which funds are most sensitive to the movements of the S&P 500.

![berk_vs_paul](/Images/berk_vs_paul.PNG)