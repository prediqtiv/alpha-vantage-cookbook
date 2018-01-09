# FAQ

### _if for example I make a request for MSFT and 5min bars, do the he timestamps on the intraday data represent the end time or the begin time of the bar?_

The timestamp mentioned indicates the end time or the last refreshed time for the details mentioned within the block. On the other hand for the first bar time stamp is 09:30:00  which indicates prices between 09:25:00 to 09:30:00.

https://www.alpha-vantage.community/post/timestamp-question-9610161?pid=1302811454



## _Is there a list of supported symbols?_

There is no list of symbols provided by Alpha Vantage. If you need the symbol for a stock you may search on [Yahoo Finance]( https://finance.yahoo.com/ ) or [Google Finance]( https://finance.google.com/finance ).



## _Trying to find intraday data on Ether (symbol: ETH). What market code should i use to get the data?_

There are issues with CNY / Chines Yuan.

I just tried:

https://www.alphavantage.co/query?function=DIGITAL_CURRENCY_INTRADAY&symbol=ETH&market=USD&apikey=<apikey>

and got results. ditto with

https://www.alphavantage.co/query?function=DIGITAL_CURRENCY_INTRADAY&symbol=ETH&market=GBP&apikey=<apikey>


## _What is an ETF?_

https://en.wikipedia.org/wiki/Exchange-traded_fund

By the end of 2015, ETFs offered "1,800 different products, covering almost every conceivable market sector, niche and trading strategy".

https://en.wikipedia.org/wiki/List_of_exchange-traded_funds


## _What is an ETN?_

https://en.wikipedia.org/wiki/Exchange-traded_note

As of April 2008, there were 56 ETNs from nine issuers tracking different indexes.

## _How to get data on non-US stocks?_

If you want to get data of Stocks from other exchanges other then US-Stock exchanges then you need to do something like this, If I wanted to get the stock value for TITAN from Indian Exchange NSE, then I need to use this in symbol NSE:TITAN .

<https://github.com/RomelTorres/alpha_vantage/issues/13#issuecomment-344839209>