# Democratizing Financial Data with IEX
This project consists of a collection of functions written in Python to request and capture financial data in a structured fashion from IEX developer's application programming interface (API). These functions obtain historical, fundamental, and alternative data for more than 9,000 assets and 5,000 publicly traded common stocks with a maximum range of 5 years.

## What is IEX?
The IEX Group, Inc. operates the Investors Exchange (IEX), a stock exchange regulated by the Security and Exchange Commission (SEC). The IEX group is on a mission to build fairer markets by fighting against questionable trading practices. IEX offers a free API containing minute by minute and historical data for U.S. Equities and other alternative assets. 

This link goes to IEX's official website: https://iextrading.com/
This link goes to IEX's API website: https://iextrading.com/developer/

## IEX's API Data
IEX's API offers a wide variety of data, categorized by reference data, market data, statistics, and markets. The source contains data for 8,740 securities, including:

Common Stock (cs): 5422 securities.
Exchange Traded Funds (et): 917 securities.
Cryptocurrencies (crypto): 18 securities.
Preferred Stock (ps): 534 securities.
Other (N/A): 1749 securities.
Su: 92
Bo: 9

For this use-case, we will focus only on common stock, given it is the subcategory that contains the most amount of securities and therefore the most amount of specific data. 

The API offers an incredible amount of current and historical market data for each common stock. The following explains some of the categories that we will be dealing with 

Company: returns Symbol (ticker), company name, market exchange, industry and sector.
Financials: returns non-consolidated statement of Income, balance sheet, and some cashflow information.

Key stats: returns current market capitalization, dividend information, earnings, and some profitability ratios. 

News: returns up till the last 50 news covering a single security with datetime, headline, summary, and source. 
Peers: returns a list of peer companies defined by IEX for the selected security. 

## Data Structures
Given we will be dealing with a high amount of data, we will require efficient data structures to capture the most amount of data with the less amount of separate data structures. Our goal is to capture data for every single security in the common stock category through efficient computational methods. We will be using Arrays, Dataframes, Lists, and Dictionaries powered by external libraries like Numpy and Pandas. 





