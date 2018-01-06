<span style=display:none; >[You are now in a GitHub source code view - click this link to view Read Me file as a web page]( https://ibpsa2017.github.io/#readme-epw.md "View file as a web page." ) </span>


# [EPW Read Me]( #readme-epw.md )


_2017-09-16 ~ Forked from [ibpsa2-17.github.io]( https://ibpsa2017.github.io/#./pages/readme-epw.md ). Will start updating eventually for this site._


## Concept / The problem we are trying to solve

Weather is a fascinating topic. It's certainly one of the most talked about topics. And every news program has time to tell you the weather.

Perhaps as a result of this frequency of appearances, most methods of visualizing weather are quite old-school.

There are pictures maps with stuff like icons, isolines and arrows written on them. And the maps may show boundaries, radar and satellite imagery. After that you are left with Beaufort wind charts and tables of numbers. In other words it's stuff you've seen before or stuff that's just too tedious to look at.

Yet weather visualization has been disruptable for much of this decade. The technology to view massive amounts of data is readily available. The ongoing issue is readily available data sources.  Yes, there are plenty of places where you can download a file at a time and run it on a program that you purchased and installed on your computer. In other words it's stuff that people who are paid to do this kind of work do. It's a day job for programmers and engineers. But it's not the sort of thing peeps are going to do just for the fun of it.

If we are to disrupt weather viz it will happen when both the tools and the data are readily accessible to artists, designers and hackers.

A typical example is the availability of EnergyPlus Weather (EPW) files. These types of files are used by engineers all over the world to help the calculate the size of furnaces air air conditions need for a construction project. 

> Displaying Design Conditions from "Climate Design Data 2009 ASHRAE Handbook". ASHRAE design conditions are carefully generated from a period of record (typically 30 years) to be representative of that location and to be suitable for use in heating/cooling load calculations


These files contain standard or typical weather data for all 365 x 24 or 8,760 hours per year. These files include op to 26 variables of data including temperature, wind speed. humidity, visibility, solar radiation and more. They are generally under two megabytes in size. There are currently files for about three thousand cities available. 

In order to view the data, typically you go to a site like [EPWMap]( http://www.ladybug.tools/epwmap/ ). You then click around until you find the file you need and then download it to your computer, extract the data from the ZIP file. Then you open a program - or go to a web site like [epwvis]( https://mdahlhausen.github.io/epwvis/ ) and upload the file. Finally you are looking at the data. Repeat three thousand times. If you happen to open the files, you will note the data is in some kind of old-timey format. 


Now just click on this link:

[Buenos Aires, Argentina EPW]( http://www.eco-envolventes.net/data/json/allEPW/ARG/ARG_BUENOS%20AIRES.json )

Bingo, you have data! Courtesy of the nice peeps at Pilota University in Bogata, Columbia who have converted all the EPW files to JSON and made them available for directly opening in a web page.

We need more nice peeps like this and we need the files on freely available places like Wiki Commons and GitHub. Anyway this is a start. I should note that organizations such as weatherunderground have made extensive data available. The issue is that you have to register, and abide by rate limits and there's a learning curve as well and etc. 

But this freely/easily weather data thing is new - and much welcomed.

### Now What

OK, yay, now you have tools and data. Who do you disrupt?

The answer is simple: me and you. 

You have very fixed notions about what the numbers can do. You are stuck on the idea that the numbers for the weather in Albuquerque are stuck to a map of Arizona. You need to let the numbers for the weather of a thousand cities to float freely in space.

You need to think like a cartoonist and let all manner of exaggeration happen.

And most of all you have to leave the simple world of paper where you can only view two or three variables at a time. You have to move into 3D viz - and let a [hundred variables bloom]( https://en.wikipedia.org/wiki/Hundred_Flowers_Campaign ).


### Current Output

#### [EPW JSON Basic]( #epw-json-basic/epw-json-basic-cors-anywhere.html )

Throughout this web site we are doing our best to separate the 3D tools code from the user interface tools. This first experiment is the attempt to provide user interface access to all the JSON data files. This 300 lines of code does exactly this - it helps you find a file and data of interest and it all fits into a narrow space such as a scrollable menu.

One interesting aspect is that the Pilato University web site is not [cross-origin resource sharing]( https://en.wikipedia.org/wiki/Cross-origin_resource_sharing ) enabled and we wanted anybody to be able to run this file without a server. Therefor we are using a free proxy service - https://cors-anywhere.herokuapp.com/ - to gather the data and forward it to your browser.


#### [EPW JSON Three.js]( #epw-json-threejs/README.md )

The file we are currently working on. It attempts to be a rewrite of the eco-envolventes with single dependency on Three.js. It also tries to be entry level cookbook code that any designer or artist with a small ammount of coding knowledge good get started with. The menu is built with the EPW JSON Basic code. The graphics are built with 300 lines of Three.js code.

Generally, it shows that the logic is generally correct and it should serve as a test case or a template for future efforts.

Next steps include:

* Wrapping the numbers around a cylinder instead of being flat
* Opening multiple surfaces displaying multiple variables at the same time
	* playing with sectioning and opacity to highlight the differences
* Adding multiple sliders to control and exaggerate the data


#### [EPW Data Parser]( #epw-parser/README.md )

This demo was built just before hearing about the EPW files from eco-envolventes. It was built around a JSON file created by Matt Dahlhausen with eight variables. The intention is to display in readable and understandably all eight variables simultaneously for all 8,760 hours.

This attempt was a fail. There are likely a good number of fails.


#### [EPW 3D]( #epw-3d/README.md )

This file was created in order to have something lively and amusing to end our workshop at Building Simulation 2017. And it did its job well. The next effort will be to bring make this file usable with all the JSON files along with the buildings, maps and terrain of their location. And the buildings will actually sway in the wind. ;-)


## Links of Interest

There are a number of interesting things related to EPW files. Here are a few of them.


### Google

* [Search EPW Weather Images]( https://www.google.com/search?q=epw+weather&rlz=1C1GCEA_enUS752US752&source=lnms&tbm=isch&sa=X )


### Wikipedia

* [Standard Day]( https://en.wikipedia.org/wiki/Standard_day )
	* The term standard day is used throughout meteorology, aviation, and other sciences and disciplines as a way of defining certain properties of the atmosphere in a manner which allows those who use our atmosphere to effectively calculate and communicate its properties at any given time. 


### [EnergyPlus]( https://energyplus.net/ )
EnergyPlus™ is a whole building energy simulation program that engineers, architects, and researchers use to model both energy consumption—for heating, cooling, ventilation, lighting and plug and process loads—and water use in buildings

EnergyPlus is funded by the U.S. Department of Energy’s (DOE) Building Technologies Office (BTO), and managed by the National Renewable Energy Laboratory (NREL).

EnergyPlus is developed in collaboration with NREL, various DOE National Laboratories, academic institutions, and private firms.

EnergyPlus created and maintain EnergyPlus Weather (EPW) files.

* [Weather Data]( https://energyplus.net/weather )
	* Weather data for more than 2100 locations are now available in EnergyPlus weather format — 1042 locations in the USA, 71 locations in Canada, and more than 1000 locations in 100 other countries throughout the world. The weather data are arranged by World Meteorological Organization region and Country.
* [Weather Data for Simulation]( https://energyplus.net/weather/simulation )
	* Users of energy simulation programs have a wide variety of weather data from which to choose – from locally recorded weather data to preselected 'typical' years –, often a bewildering range of options. Many locations are available on this site – but users may have special needs for different locations. 
* [Weather Data Sources]( https://energyplus.net/weather/sources )
	* The weather data provided in EnergyPlus weather format on this website are derived from 20 sources:


### [onebuilding.org]( http://onebuilding.org/ )

* [climate.onebuilding.org]( http://climate.onebuilding.org/ )
	* Respository for free weather data for building performance simulation
	* [Weather Data Sources]( http://climate.onebuilding.org/sources/default.html )


### [Ladybug Tools]( http://ladybug.tools )

* [EPW Map]( http://www.ladybug.tools/epwmap/ )
	* The goal of the project is to provide a single interface for all the available free .epw weather files. Currently it shows weather files hosted by EnergyPlus Website and One Building. 
* [epwmap]( https://github.com/ladybug-tools/epwmap )
	* epwmap is developed as part of Ladybug Tools. The goal of epwmap is to provide a single interface for all the free available .epw weather files.
* [[FAQ] Where to find .epw weather data?]( http://www.grasshopper3d.com/group/ladybug/forum/topics/faq-where-to-find-epw-weather-data )


### [DOE2.com]( http://www.doe2.com/ )

* [Weather Data & Weather Data Processing Utility Programs]( http://doe2.com/index_wth.html )


### [White Box Technologies]( http://weather.whiteboxtechnologies.com/home )

* Building energy simulations require weather data as an essential input. White Box Technologies provides useful tools to find "typical year" and historical year weather files created from weather reports of over 10,000 official weather stations around the world.


### [WeatherShift]( http://www.weather-shift.com/ )

* Buildings and infrastructure built today will experience significantly different weather patterns over the course of the 21st century due to the impact of climate change.
* The WeatherShift™ tool uses data from global climate change modeling to produce EPW weather files adjusted for changing climate conditions. (EPW files contain hourly values of key weather variables for a typical year and are intended to be used for simulating building energy requirements.) The projected data can be viewed for three future time periods based on the emission scenario selected to the left.


### [Energy Simulation Solutions Limited]( http://cms.ensims.com/ )

* [Compare two EPW files]( http://jess.ensims.com/epw_compare.html )


### [epwvis]( https://mdahlhausen.github.io/epwvis/ )

* An online viewer and analysis tool for EnergyPlus Weather (EPW) files
* Probably the best 2D viewer available today
* By Matthew Dahlhausen


### [andrewmarsh.com]( http://andrewmarsh.com/ )

* [Weather Data]( http://andrewmarsh.com/software/weather-data-web/ )
	* This web app lets you load and display EnergyPlus weather data in a 3D graph with data averaging and animated sectioning. It maps the full range of weather data metrics against day of the year and hour of the day to create an undulating 3D surface plot. You can interactively adjust the displayed metric, the graph size and scale, section planes and data averaging parameters. Simply drag&drop a .EPW file anywhere in the browser windows and you are ready to go.
	* Dr Marsh is one of the gods of simulating complicated things in 3D



### [eco-envolventes]( http://www.eco-envolventes.net/ )

[eco-envolventes]( http://www.eco-envolventes.net/ ) is a research project at the [Universidad de Piloto]( http://www.unipiloto.edu.co/ ), Bogota, Colombia

The group prepared a submission for Workshop at the Design Modelling Symposium 16 - 17 September 2017 Paris 

The submission includes a number of very interesting 2D and 3D visualizations.

Of primary importance is their data set of EPW files converted to JSON.

Pages of great interest include:

* [Prototype Visualisation Tools]( http://www.eco-envolventes.net/tools.html )

	* [3d annual chart]( http://www.eco-envolventes.net/tools/170614a/3dChart1.html )
		* Data is from the EnergyPlus *.epw files collection which represents 68 Countries and 2240 cities. These have been converted to our climaJSON format for use online. Using this format the data can be visualised in 2d, 3d and on a psychrometric chart. The full set of converted *.epw files is available here.
	* [climaJSON]( http://www.eco-envolventes.net/climaschema/ )
		* Schema for a climaJSON object.
		* This format describes an object containing climate data for a single year in a single location. The object stores an unlimited set of fields for monthly and / or hourly values.
		* Author: R Hudson. Updated: 21/5/2017
	* 2D: http://www.eco-envolventes.net/tools/170614/
	* Psychrometric chart: http://www.eco-envolventes.net/tools/170614b/pChart.html
	* Folders with all converted files: http://www.eco-envolventes.net/data/json/allEPW/
	* More visualizations: http://www.eco-envolventes.net/tools/


## Change Log


### 2017-08-21 ~ Theo

* Moany code and text updates

### 2017-08-12 ~ Theo

* First commit
