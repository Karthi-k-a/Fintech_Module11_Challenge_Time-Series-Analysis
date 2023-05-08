# Fintech_Module11_Challenge_TimeSeriesAnalysis

## Forecasting Net Prophet
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/unit-11-readme-photo.png)

### Overview
Forecasting Net Prophet aims at analysing the company's financial and user data in clever ways to help the company grow in a Jupyter notebook that contains data preparation, analysis, and visualisations for all the time series data that the company needs to understand.<br> 
Files: [forecasting_net_prophet.ipynb](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/forecasting_net_prophet.ipynb), [google_hourly_search_trends.csv](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Resources/google_hourly_search_trends.csv), [mercado_daily_revenue.csv](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Resources/mercado_daily_revenue.csv), [mercado_stock_price.csv](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Resources/mercado_stock_price.csv)

### Steps
- Find unusual patterns in hourly Google search traffic.
- Mine the search traffic data for seasonality.
- Relate the search traffic to stock price patterns.
- Create a time series model by using Prophet.
- (optional): Forecast the revenue by using time series models.

### Analysis and Results
**Do any unusual patterns exist in the month of May 2020?**<br>
From the below plot, it can be seen that the search trend was unusually high at 12 am on 5th and 6th May as compared to the rest of the month.<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/1.png)

**Did the Google search traffic increase during the month that MercadoLibre released its financial results?**<br>
The median monthly search traffic of MercadoLibre is 35172 while the search traffic in May 2020 was 38181 which is 8.5% more than the monthly average. This increase in search traffic in May 2020 was due to the release of financial results.<br>

**Does any day-of-week effect that you observe concentrate in just a few hours of that day?**<br>
From the below plots, it can be observed that the search trend is concentrated between 10 pm and 2 am on all days of week. It can also be seen that the traffic is low between 5 am and 12 pm which could be a result of people being at work/school.<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/2.png)
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/3.png)

**Does the search traffic tend to increase during the winter holiday period (weeks 40 through 52)?**<br>
The search traffic increases from week 42 to 51 with people shopping for holidays and drops rapidly on week 52 reaching year's lowest.<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/4.png)

**Mercado Libre Stock Closing Price**<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/5.png)

**Slice the data to just the first half of 2020 and then use hvPlot to plot the data. Do both time series indicate a common trend that’s consistent with this narrative?**<br>
From the below time series plots, it can be seen clearly that the stock price and search trend have a direct realtionship. In the months of February and March, there is a downward trend in both stock price and search traffic. And, in the month of May where there is a sharp increase in search trend, there is a sharp increse in the stock price as well.<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/6.png)
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/7.png)

**Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns?**<br>
From the correlation matrix, it is seen that lagged search traffic and the stock volatility have a weak negative correlation whereas lagged search traffic and the stock price returns have a weak positive correlation.<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/8.png)
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/corr.png)

**What is the near-term forecast for the popularity of Mercado Libre?**<br>
The forecast indicates that the popularity of MercadoLibre gradually decreases towards the end of 2020.

**MercadoLibre Search Trends Forecast**<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/9.png)

**What time of day exhibits the greatest popularity?**<br>
The time between 10 pm and 2 am exhibits the greatest popularity.

**Which day of week gets the most search traffic?**<br>
Tuesday to Friday have more search traffic compared to the rest of the week with Tuesday having the highest search traffic.

**What's the lowest point for search traffic in the calendar year?**<br>
The lowest point for search traffic in the calendar year seems to be in mid October.

**MercadoLibre Daily Sales in Millions (USD)**<br>
<br>
![](https://github.com/Karthi-k-a/Fintech_Module11_Challenge_TimeSeriesAnalysis/blob/main/Images/10.png)

**Based on the forecast information, produce a sales forecast for the finance division, giving them a number for expected total sales next quarter. Include best and worst case scenarios, to better help the finance team plan.**<br>
Based on the forecast information generated, we can see that the most likely case for the quarter would be roughly 969 million dollars. The best case scenario would be around 1051 million dollars and the worst case scenario would be around 887 million dollars.
