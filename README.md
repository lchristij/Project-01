# Event Driven Robo Advisor Project:
Our project will produce a robo advisor for Individual Investors to predict the impacts of News/Announcements in the currency markets. We will analyze the impact of various economic events from 2007 to present. Specifically, we are going to measure the impact of the Central Banks and Government actions on their respective currencies (through the Alpaca, Alpha Vantage, and/or Bloomberg APIs). In addition, we will scrape the economic calendar from Forex Factory to provide a consensus on upcoming announcements and map the historic impact of those events on the currencies paired with the US Dollar to provide Long/Short recommendations supported by Monte Carlo simulations for a "crystal ball" prediction for upcoming announcements.

## Data Sets, Packages and Visualization:
1.	https://www.babypips.com/economic-calendar?timezone=America%2FChicago&week=2020-W51 - news events and consensus data related to forex pairs dating back to 2007 in chronological order consisting of 9 columns and several rows. The data is html based and will be scraped from website.
2. https://rapidapi.com/apidojo/api/bloomberg-market-and-financial-news?endpoint=apiendpoint_99774619-7ee2-4cb9-ac1b-cc8ff9857ce2 - news and forex pricing data provided in multiple formats such as json, etc. for various currency pairs.
3. Packages planned for use are: scikit-learn and beautifulsoup4
4. Visualization frequency of plotted monte carlos simulation will be provided for each recommendation
5. The tool will provide retail forex investors with buy/sell recommendation for EUR/USD,GPB/USD & USD/JPY. 