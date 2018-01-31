<span style=display:none; >[You are now in a GitHub source code view - click this link to view Read Me file as a web page]( https://prediqtiv.github.io/alpha-vantage-cookbook/#ymbol-search/README.md "View file as a web page." ) </span>



# Symbol Search

See this post in the Alpha Vantagw Community Forum:

<https://www.alpha-vantage.community/post/symbol-search-api-9609292?pid=1302943198>


There are multiple aspects to this topic

* Enter symbol, get company name and/or details
* Enter company name, get symbols
* Determine symbol naming format that works with Alpha Vantage
* Determine that data that Alpha Vantage is likely to return for a symbol
* And so on

The following is a preliminary investigation into online symbol search API with data available - just like Alpha Vantage - at no charge. I have no clear idea where this is all headed., but we will get there one day. ;-)

## Open full screen: [OpenFIGI API Front End R2]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html )

* With slide in/out 'hamburger menu
* Updates results with changes to location hash
* Button loads the NSE NIFTY50 symbol set
	* Button for each symbol checks to see is ticker symbol is recognized by OpenFIGI

### NSE NIFTY50 Ticker Symbols Recognized by Open FIGI

I have not checked all the 50 symbols. Most symbols produce no results in OpenFIGI.

Here are some of the symbols - with links - that do have results:
* [BPCL]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html#%7B%22symbol%22:%22BPCL%22%7D )
* [CIPLA]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html#%7B%22symbol%22:%22CIPLA%22%7D )
* [HDFC]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html#%7B%22symbol%22:%22HDFC%22%7D )
* [ITC]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html#%7B%22symbol%22:%22ITC%22%7D )
* [LT]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html#%7B%22symbol%22:%22LT%22%7D )
* [SBIN]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end-r2.html#%7B%22symbol%22:%22SBIN%22%7D )


## Open full screen: [OpenFIGI API Front End]( https://prediqtiv.github.io/alpha-vantage-cookbook/symbol-search/openfigi-api-front-end.html )

* Very preliminary release
* Type in typical symbol name, see the OpenFIGI results

## Coming Soon to 'OpenFIGI API Front End'

* More filters
* Links to symbols from more exchanges


***

## OpenFIGI Links of Interest

<https://openfigi.com/api>


### Stackoverflow help

* <https://stackoverflow.com/questions/45137592/openfigi-api-and-cors>
	* <https://jsfiddle.net/theo/qvq4xLgy/>
* <https://stackoverflow.com/questions/43142087/openfigi-api-curl-to-java-post


## Bloomberg SymbolSearch Links of Interest

<https://www.bloomberg.com/markets/symbolsearch>

https://www.bloomberg.com/markets/symbolsearch?query=rr&commit=Find+Symbols

https://www.bloomberg.com/markets/symbolsearch?query=BDP("ticker","field")

https://www.bloomberg.com/markets/symbolsearch?query=BDP("ESS PW Equity","Name")


## More Links of Interest

<https://permid.org/>

<https://quant.stackexchange.com/questions/7568/mapping-symbols-between-tickers-reuters-rics-and-bloomberg-tickers>

<https://stackoverflow.com/questions/885456/stock-ticker-symbol-lookup-api>

<http://www.nasdaq.com/screening/company-list.aspx>


## Wikipedia

* https://wikimediafoundation.org/wiki/Developer_app_guidelines
* https://en.wikipedia.org/wiki/Wikipedia:Database_download
* https://dumps.wikimedia.org/
* https://en.wikipedia.org/wiki/Special:Export

### SP500

* https://en.wikipedia.org/wiki/List_of_S%26P_500_companies
* https://en.wikipedia.org/wiki/Special:Export/List_of_S%26P_500_companies


***
