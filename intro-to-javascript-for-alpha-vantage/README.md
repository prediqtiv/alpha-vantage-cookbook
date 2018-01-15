
# Introduction to JavaScript for Alpha Vantage

Five simple and basic scripts to get you started with coding the calls to Alpha Vantage that suit your specific needs.

Click any of the file names to run the script.

##	[01-alpha-vantage-get-data-basic.html]( #intro-to-javascript-for-alpha-vantage/01-alpha-vantage-get-data-basic.html )

A 'hello world' script. The script makes an Ajax / XMLHttpRequest call to load and display the basic Alpha Vantage demo file.
The call is identical to the first link in the Alpha Vantage documentation. After a few seconds, the requested data will appear on screen replacing the existing text.

Tip: the API call in this script uses the [same symbol and API key]( https://github.com/prediqtiv/alpha-vantage-cookbook/blob/master/intro-to-javascript-for-alpha-vantage/01-alpha-vantage-get-data-basic.html#L43 ) as the [Alpha Vanatage documentation]( https://www.alphavantage.co/documentation/ ), therefore it may access the Alpha Vantage data without error.

Things to do: edit the API key and the symbol to make a new and different call for data


## [02-alpha-vantage-get-data-interactive.html]( #intro-to-javascript-for-alpha-vantage/02-alpha-vantage-get-data-interactive.html )

This script adds two input elements. The first is where you enter your API key. The second enables you to call for data for any symbol.

Once the data has been entered, you may click the get data button to make the call.

Things to do: Edit the default values for the two input boxes.


## [03-alpha-vantage-get-data-local-storage.html]( #intro-to-javascript-for-alpha-vantage/03-alpha-vantage-get-data-local-storage.html )

Entering your API key  becomes tedious very quickly. This script adds storing the key in the browser's [localStorage]( https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage ).

Things to do: Add local storage for your favorite symbol.


## [04-alpha-vantage-get-data-save-to-file.html]( #intro-to-javascript-for-alpha-vantage/04-alpha-vantage-get-data-save-to-file.html )

Once you have the data, it's nice to be able to save the data to a local file. This script adds a 'save data to file button'.

Things to do: Add a date to the suggested file name. Save the data to a JSON file.


## [05-alpha-vantage-get-data-select-parameters.html](#intro-to-javascript-for-alpha-vantage/05-alpha-vantage-get-data-select-parameters.html )

Alpha Vantage API calls support a variety of parameters. This script shows you how to set parameters using dropdown menus.

Things to do: Set alternative choices as the defaults. Translate the text to another language.

***

# <center><a href=javascript:window.scrollTo(0,0); style=text-decoration:none; > ❦ </a></center>

