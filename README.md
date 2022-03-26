# World Weather Analysis 

## Overview
### Purpose
This purpose of this project was to create a pseudo-app that assimilated current weather analysis for locations for users to filter by temperature preference to view ideal travel locations with hotel recommendations in a dataframe and map. The user then would be able to select cities and create personalized travel itinerary by visualizing directions map. 

### Resources
**Data retrieval:** [OpenWeatherMap.Org](https://openweathermap.org/), [Google Maps](https://mapsplatform.google.com/)

**Tools:** Python, Jupyter Notebook, GMaps, [Citipy](https://github.com/wingchen/citipy), Requests Library, OpenWeather API, PANDAS, Matplotlib, Numpy, Statistics
<br>

### Current Weather
Using API requests of [Open Weather Map](https://openweathermap.org/), the current weather: maximum temperature, percent cloudiness, percent humidity, wind speed, and current description were determined for a list of cities generated with citipy script using random latitude and longitude values. 

In [Weather_Database Folder](/Weather_Database/), the dataframe for current weather statistics was created from a random list of cities and exported as a csv file. 
<br>
<br>**Table 1.** Current Weather Database
<br>![Table 1 image](/Weather_Database/Weather_Database_Sample.png)
<br>Table 1 is a sample of the dataframe created from random list of cities and the current weather.


### Hotel Map
With data from the [Table 1](Weather_Database/WeatherPy_Database.csv), an API requests of [Google Maps Places](https://developers.google.com/maps/documentation/places/web-service) was used to create a map with markers denoting hotels for travel locations that matched user specified temperature ranges. User input for preferred temperature range was used to generate the map of cities.
<br>
<br>**Image 1.** Vacation Search Map
<br>![Image of Map](/Vacation_Search/WeatherPy_vacation_map.png)
<br>Image 1. shows a screenshot of the vacation search map with markers detailing hotels, city, country, and current weather.

### Travel Map
Using the user-specified data from previous section ([User-filtered data](/Vacation_Search/WeatherPy_vacation.csv)), four cities were selected and travel itinerary created using [Google Maps Directions](https://developers.google.com/maps/documentation/directions/web-service).
<br>
<br>**Image 2.** Vacation Travel Map
<br>![Image of Travel Map](/Vacation_Itinerary/WeatherPy_travel_map.png)
<br>Image 2 shows a screenshot of travel map created in [/Vacation_Itinerary/ Folder](/Vacation_Itinerary/) from user traveling from Natal, Brazil to desired stops: Cabedelo, Brazil; Pitimbu, Brazil; and Olinda, Brazil.
<br>
<br>**Image 3.** Vacation Hotel Marker Map
<br>![Image 3 of Hotel Travel Map](/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
<br>Image 3 shows the screenshot of map with the selected cities with markers with hotel information. 


