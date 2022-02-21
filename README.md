# World_Weather_Analysis

## Overview: 
The purpose of this project was to design an app that would allow the beta tester to identify potential travel destinations, hotels, and travel routes based off of their weather preferences. 

Project Folders: [Weather_DataBase](https://github.com/Lan-kdl/World_Weather_Analysis/tree/main/Challenge/Weather_Database) 
[Vacation_Search](https://github.com/Lan-kdl/World_Weather_Analysis/tree/main/Challenge/Vacation_Search) 
[Vacation_Itinerary](https://github.com/Lan-kdl/World_Weather_Analysis/tree/main/Challenge/Vacation_Itinerary)

Python: [Weather_DataBase](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Weather_Database/Weather_Database.ipynb) 
[Vacation_Search](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Vacation_Search/Vacation_Search.ipynb) 
[Vacation_Itinerary](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Vacation_Itinerary/Vacation_Itinerary.ipynb)

## Project Steps 
First, I generated a list of 2000 random longitudes and latitudes which I then assigned to 735 of the nearest cities. From there, using openweathermap, I collected the information for each city pertaining to temperature, humidity, cloudiness, wind speed, weather description, and country. I compiled this information into a dataframe which was then exported as a [csv file](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Weather_Database/Weather_Database/WeatherPy_Database.csv). 

![Untitled](https://user-images.githubusercontent.com/95589611/154873664-4efe97b2-4ad8-499d-af91-08bbd1e86631.png)

It is at this point that the beta tester would be asked to input their prefered min and max temperatures from which a new datafram which would contain only those cities within that parameter. 

![which](https://user-images.githubusercontent.com/95589611/154873760-aa14c322-8cdc-4f93-b439-bc22ffa0b06a.png)

The relevent hotels for each city were then pulled from google and added to the dataframe. This dataframe was used to create a [marker map](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Vacation_Search/Vacation_Search/WeatherPy_vacation_map.png) that displayed each city's information. From this marker map the beta tester could choose any number of cities displayed on the map (for testing purposes, we chose 4 cities in Australia). Using gmaps, I created a [direction layer map](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Vacation_Itinerary/WeatherPy_travel_map.png) which displayed the Driving routes to each city, starting and ending with Port Hedland. I also created a [marker layer map](https://github.com/Lan-kdl/World_Weather_Analysis/blob/main/Challenge/Vacation_Itinerary/WeatherPy_travel_map_markers.png) which displayed the city information such as weather description, country, and max temp. 

## Example maps that can be created by the app
![WeatherPy_vacation_map](https://user-images.githubusercontent.com/95589611/154872731-a97d1c0d-da30-4b51-8b9e-7375c4820bbb.png)
![WeatherPy_travel_map](https://user-images.githubusercontent.com/95589611/154872750-b673f54c-e9e1-4e81-a644-a09572249361.png)
![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/95589611/154872756-7144da3c-76b9-410d-be3e-30f326ed8468.png)
