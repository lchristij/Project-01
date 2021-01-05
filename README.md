# Event Driven Robo Advisor Project:
Our project will produce a robo advisor for Individual Investors to predict the impacts of News/Announcements in the currency markets. We will analyze the impact of various economic events from 2007 to present. Specifically, we are going to measure the high impact news (Central Bank, GDP, Inflation, Unemployment, etc.) on their respective currencies through the Alpaca & Alpha Vantage APIs. In addition, we will scrape the economic calendar from BabyPips via beautifulsoup4 library to provide a consensus on upcoming announcements and map the historic impact of those events on the currencies relative to the US Dollar to provide Buy/Sell/Neutral recommendations supported by Monte Carlo simulations for a "crystal ball" prediction for upcoming announcements.

## Data Sets, Packages and Visualization:
1. https://www.babypips.com/economic-calendar?timezone=America%2FChicago&week=2020-W51 - news events and consensus data related to forex pairs dating back to 2007 in chronological order consisting of 9 columns and several rows. The data is html based and will be scraped from website.
2. https://rapidapi.com/alphavantage/api/alpha-vantage - pricing data provided in multiple formats such as csv, etc. for EUR/USD, GBP/USD, USD/JPY currency pairs (2011 - 2021)
3. https://app.alpaca.markets/paper/dashboard/overview - pricing data provided in multiple formats such as json, etc. for FXE, FXY, FXG ETFs.
4. Packages planned for use are: beautifulsoup4, numpy, mc forecast***
5. Visualization frequency of plotted monte carlos simulation will be provided for direcational strategy on ETFs (assuming Long positions only for initial analysis)
6. The tool will provide retail forex investors with buy/sell/neutral recommendation for EUR/USD, GPB/USD & USD/JPY

### Based on the economic calendar forecasts that highly impact the currency pair (EUR/USD, GBP/USD, USD/JPY), can we provide Buy/Sell/Neutral recommendations within 4 weeks of upcoming news events?
Short Description + Relevant Plots/Graphs

#### Given an initial investment amount of $10,000 and assuming recurring 8 week holding periods over 5 years, with what confidence can we produce an expected return for the investor over that holding period?
Short Description + Relevant Plots/Graphs

##### Can we iteratively improve the confidence interval of our recommendations through additional Time Series Analysis, NLP, and Machine Learning?
Short Description + Relevant Plots/Graphs
