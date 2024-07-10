# python-api-challenge

# Overview:
The purpose of this module was to randomly generate a list of over 500 cities, and then create plots that would visualize the relations between latitude and an assortment of weather conditions. The weather conditions include the city's experienced max temperature, cloudiness, humidity, and wind speed. The data for these weather conditions would be gathered through an API call to the OpenWeather API, and then organized into a usable dataframe, which would be exported into a csv. From there, the dataframe would be used to create several baseline scatter plots of latitude versus each weather condition and outputed as a saved .png file. Afterwards, the dataframe would be split into cities existing within either the northern hemisphere or southern hemisphere. The code will then generate several linear regression plots depicting the realtionship between latitude and the listed weather conditions for both of the northern and southern hemisphere cities, allowing us to determine if there is a correlation between a city's latitude and experienced weather conditions. 

Using the csv file generated earlier, a seperate script will read this csv and generate a map of depicting the locations of all of the cities on the randomly generated list. The script will then isolate cities that exist within specified weather parameters, and place them in a new dataframe. This dataframe will then be used in relation to an API call to Geoapify API, to search for the nearest hotel within 10,000 meters of each city's coordinates, and then add the name of the hotels to the dataframe. This updated dataframe will then be used to create a new map depicting the locations of the ideal weather condition cities and the name of the nearest hotel at each city.

## Mainscripts:
The Mainscripts folder contains all of the saved outputs (png and csv files) from the WeatherPy mainscript, as well as the mainscripts for both WeatherPy and VacationPy.

### WeatherPY: [Mainscript](https://github.com/EdGonz44/python-api-challenge/blob/main/MainScripts/WeatherPy.ipynb)
The WeatherPy mainscript conducts the investigation and visualization of the relations between city latitude and weather conditions. This script is responsible for creating the figures used in the linear regression plots, the baseline png files as well as creating the csv file used in the VacationPy script. The script also contains a brief analysis of the r^2 correlation values found through the linear regression lines.

### VacationPy: [Mainscript](https://github.com/EdGonz44/python-api-challenge/blob/main/MainScripts/VacationPy.ipynb)
The VacationPy mainscript utilizes the generated csv file from the WeatherPy mainscript to create the map depiction of the randomly generated city list, and the map showing the names of the hotels on the cities that fall within the ideal weather condition parameters. 


