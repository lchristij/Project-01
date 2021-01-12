# Event Driven Robo Advisor Project:
Our project will produce a robo advisor for Individual Investors to predict the impact of News/Announcements in the currency markets. We will analyze various economic events from 2007 to present. Specifically, we are going to measure the high impact news (Central Bank/Interest Rates, GDP, Inflation, Unemployment, etc.) on their respective currencies through the Alpaca & Alpha Vantage APIs. In addition, we will scrape the economic calendar from BabyPips via the beautifulsoup4 library to provide a consensus on upcoming announcements and map the historic impact of those events on the currencies relative to the US Dollar to provide Buy/Sell/Neutral recommendations supported by Monte Carlo simulations for a "crystal ball" prediction for potential returns on recommendations from upcoming announcements.

## Data Sets, Packages and Visualization:
1. https://www.babypips.com/economic-calendar?timezone=America%2FChicago&week=2020-W51 - news events and consensus data related to forex pairs dating back to 2007 in chronological order consisting of 9 columns and several rows. The data is html based and will be scraped from website.
2. https://rapidapi.com/alphavantage/api/alpha-vantage - pricing data provided in multiple formats such as csv, etc. for EUR/USD, GBP/USD, USD/JPY currency pairs from 2001-2021.
3. https://app.alpaca.markets/paper/dashboard/overview - pricing data provided in multiple formats such as json, etc. for the selected currency pairs from 2016-2021.
4. Packages planned for use are: beautifulsoup, numpy, MCForecastTools_fp, datetime, holoviews, panel, hvplot, & pathlib
5. Visualization frequency of plotted monte carlos simulation will be provided for directional strategy on the currency pairs
6. The tool will provide retail forex investors with buy/sell/neutral recommendation for EUR/USD, GPB/USD & USD/JPY

### Based on the economic calendar forecasts that highly impact the currency pair (EUR/USD, GBP/USD, USD/JPY), can we provide Buy/Sell/Neutral recommendations within 4 weeks of upcoming news events?

We establish that economic announcements have a significant impact on currency volatility and the ecomonic calendar available to Individual Retail Investors includes a Forecasted Consensus of the upcoming announcement vs. the Previous Consensus. We successfully perform our fundamental analysis via an algorithm to provide a Buy/Sell/Neutral recommendation based upon any difference (positive or negative) in that Forecast vs. Previous Consenses. The results provide a recommendation for each in which we net the positive and negative recommendations to produce our own summary recommendation for the period. Depending on the current market and economic conditions, this period can either change rapidly (daily/weekly) or maintain its recommendation for an extended period (weeks/months). This is evident in the links to the following graphs and plots:

Historical Precedence via TradingView:
![](https://github.com/lchristij/Project-01/blob/main/images/trading_view_historical.png)

Euro Line Chart:
![](https://github.com/lchristij/Project-01/blob/main/images/euro_graph.png)

Japanese Yen Line Chart:
![](https://github.com/lchristij/Project-01/blob/main/images/jpy_graph.png)

Great Britain Pound Line Chart:
![](https://github.com/lchristij/Project-01/blob/main/images/gbp_graph.png)


### Given an initial investment amount of $10,000 and assuming recurring 8 week holding periods over 5 years, with what confidence can we produce an expected return for the investor over that holding period?

Provided the above assumptions, we were able to produce a confidence interval of the performance of all three currency pairs (EUR/USD, GPB/USD, USD/JPY). This Monte Carlo prediction on the returns that captures both the Long and Short impacts in the 8 week holding periods over 5 years. This was actually a slightly better performance than 4 week holding periods over 5 years. There may be additional peformance improvements for shorter durations such as daily or intraday, but that was beyond the scope of the MVP. The following plots and graphs illustrate our analysis to date:

![](https://github.com/lchristij/Project-01/blob/main/images/MC_lower_upper.png)

![](https://github.com/lchristij/Project-01/blob/main/images/monte_carlo.png)



### Can we iteratively improve the confidence interval of our recommendations through additional Time Series Analysis, NLP, and Machine Learning?
We identified several areas for improvement through our development process. The first was to create a Natural Language Processor to identify which economics news events had a positve vs. a negative directional impact on the specific currency. We also recognized that both time series analysis and machine learning could be utilized to provide our own Forecast consensus numbers prior to having to wait for the Forecasts from Babypips to be published. Finally, we realized the historic volatility could be best captured with specifically timed Long/Short recommendations/actions to maximize profit over the same holding periods. This can be achieved through multiple accounts or a non FIFO based trading account to allow for multidirectional trading at the same time. By implementing all of the above with an additional 2 weeks for development, we could drastically improve our recommendation accuracy to provide significant improvement in overall performance, most likely through an automated algorithmic trading bot. Looking forward to those potential features in Project 2!


