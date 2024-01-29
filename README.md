# Project-1: US Banks & IShare ETF Financial Analysis
### Group 2: Katie Nieuwhof, Catherine Ding, Sobi Iyver, Justice Bangura

## Motivation & Hypothesis
**Hypothesis**: we believe that certain economic environment impacts the banks financial and market behavior in US free trade market. 

We assume that:

1.	The Top 3 US Banks stock data and their financial report, as well as with iShares S&P U.S. Banks UCITS ETF data can represent the US publicly traded Banks market.
2.	The most important economic environment factors for US banks market can be briefly assessed by fed and treasury bonds interests, inflation forward rate, mortgage rates, cpi and unemployment rate.
   
**The primary question we asked is:**
How did the US publicly traded Banks market behave during the last 5 years (2019-2023) based on the recent economic environment?

We asked this question because we have experienced a special period over the last 5 years due to Covid-19 and huge interest rate changes.

We were able to answer the above question by analyzing the relationship between the bank stock prices, the financial data, the economic data, and the banks index. We chose the top 3 US publicly traded banks - JP Morgan Chase, Bank of America, and Wells Fargo - and analyzed their stock price behaviors, 3 years of their recent financial data from their annual reports, and we compared them to one another. We also compared the data with iShares S&P U.S. Banks UCITS ETF price data and analyzed the economic data (such as fed and treasury bonds interest rates, forward inflation rate, cpi, unemployment rate, fixed mortgage rate) to assess their impacts to the banks stock market.

**The data we used, and where we found it:**
* Stock prices for JPM, BAC, and WFC were found using Google Finance function in excel sheets, and their financial data found using yahoo finance api
* IShare US Bank ETF Index data found by yahoo finance api
* Economic market data found online via New York Stock Exchange

## Findings

### Stock Price Data:

**Question:** How has the bank market fluctuated over the past 5 years (2019-2023), and why?

After calculating the daily returns, we were able to calculate the cumulative returns which is displayed in the plot below. We can see a rapid decline in the cumulative returns for the top 3 US banks as well as the bank index in 2020 with the onset of COVID-19 in 2020. This is likely due to the instability and high volatility the market faced during the pandemic, as well as the drastic increase in unemployment rates which negatively impacts bank profitability. The cumulative returns for the top 3 US banks and the bank index steadily increase and peak in 2022 – likely due to rapid increase of interest rates by feds in 2022. Thereafter, cumulative returns decline over the first half of 2022, then remaining stable through the end of 2023. 

![Cumulative Returns](Figures/cumulative_returns_plot.png)

The plot below displays the rolling standard deviation with a window of 21 days. The largest change in standard deviation occurs in 2020 with the onset of COVID-19. This drastic increase implies a greater fluctuation in bank stock prices indicating a higher volatility and greater risk – which aligns with the cumulative returns plot shown above (rapid decrease in cumulative returns in 2020).

![Rolling Standard Deviation](Figures/rolling_std_plot.png)

**Question:** How are do the 3 top US banks compare to each another and the bank index?

The heatmap below displays the correlation of the top 3 US bank stock prices with the bank index. This heat map demonstrates that JP Morgan Chase and Bank of America are the most correlated amongst the 4, which is not a surprise given they are the top 2 banks in the US. 

![Heat Map](Figures/heatmap.png)

The distribution plot is based off of daily returns, and it appears all 3 banks and the index are relatively normally distributed.

![Distribution](Figures/distrubution_plot.png)

According to the Sharpe ratios shown below, JPMorgan Chase has a more attractive risk reward trade off compared to the other banks and the bank index, indicating a greater return at a lower risk. 

![Sharpe Ratios](Figures/sharpe_ratios_plot.html)

