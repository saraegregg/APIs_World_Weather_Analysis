# World_Weather_Analysis


## Overview
For the new modifications to the PlanMyTrip app, add more cities' data to the database, make it so that customers can filter the results based on their preferred temperature range and know the weather in the cities when they click on a pop-up marker. Finally, facilitate clients' hotel choice by providing them an option at each destination. 

After modifying the PlanMyTrip app, make a sample itinerary with a map showing the route one might take from city to city, as well as a map with a logings option, city name, country, and current weather conditions.

## Resources
- Jupyter Notebook 6.4.5
- Python 3.9.7
  - APIs:
      - OpenWeatherMap
      - Google Places
      - Google Maps JavaScript
      - Google Directions

## Process
### CitiPy and OpenWeather API
After creating a list of 2000 random latitudes and longitudes, citipy was used to locate the nearest city. Next the OpenWeather API provided weather data for the cities, which was gathered and formatted the information into a DataFrame.

![city_data_df](https://github.com/saraegregg/Mod6_World_Weather_Analysis/blob/main/city_data_df.png)

### Google API 
At this point, PlanMyTrip asks the user to input their desired temperature range in the form of min and max values. A new DataFrame is created  that includes cities whose weather fell into the client's ideal temperature range.  After inserting a new column, "Hotel Name" into the DataFrame, the Google 'nearbysearch' endpoint API populated a hotel for each city in the DataFrame, which all was displayed to the cusomer using an interactive map with markers. (see below)

### Create a travel itinerary map
The app allows a user to narrow down travel destinations based on their preferred weather, and, to illustrate, I created an itinerary with four cities in Australia in the 75-90 degree temperature range. I was able to create a route between each city and see where to stay on each marker, displayed on the maps below:

![WeatherPy_vacation_map](https://github.com/saraegregg/Mod6_World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

![WeatherPy_travel_map](https://github.com/saraegregg/Mod6_World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)


