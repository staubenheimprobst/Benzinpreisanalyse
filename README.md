# Benzinpreisanalyse
Get fuel-prices from http://clever-tanken.de and save them for price-development analysis

*written in Python 3*

This Python script uses the website http://clever-tanken.de to get the fuel-price of the stations in your area of choice.
The data is saved into a csv-File for later analysis in an application of your liking.

## Usage
Edit the script and set the Parameters:  

|Variable |Meaning|
|---------|-------|
|path     |*the path where you want to save your results*|
|filename |*the name of the csv-file*                    |
|day      |*day when the scanning starts (default = Sun)*|
|span     |*how many shall the program run (default = 7)*|
|period   |*frequency of the scans (default = 3600 sec = 1hr)*|
|PLZ      |*enter your ZIP-Code*|
|town     |*Enter the name of your town*|
|radius   |*radius of the area scanned (default = 5.0km)*|
|fueltype |*What kind of fuel are you looking for (1=Autogas (LPG), 2=LKW-Diesel, 3=Diesel, 4=Bio-Ethanol, 5=Super E10, 6=Super Plus, 7=Super E5, 8=Erdgas (CNG), 12=Premium-Diesel, 13=AdBlue)*|

Run the program on your server with `python3 Benzinpreis.py`. After the program finished running you can copy the csv file and open it in any application you think appropriate for analysis.

## ToDo
+ adding a GUI
+ adding matplotlib to generate graphs from the gathered data/csv-file
+ adding the data/graphs to a website
