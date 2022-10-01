# World Weather Analysis and Trip Planning:  API Calls to OpenWeatherMaps and Google

## Purpose
An Application Programming Interface, or API, is a type of software interface that allows two, or more, computers to communicate with each other.  As API’s allow for a certain level of control and security, companies or organisations that accumulate large amounts of data often use API’s to make their databases accessible and searchable.  The purpose of this project was to use API calls to determine the closest cities to randomly generated latitude and longitude coordinates and the current weather conditions in those cities and place the information into a data frame.  The resultant data frame was then used to guide an API with Google Maps in the interests of planning a trip between four cities and obtaining information regarding accommodations within those cities.

## Results
After using the numpy module to generate 2000 random latitude, longitude coordinate pairs, the citipy module was used to determine which city, if any was closest to those coordinates and an API call was made to OpenWeatherMaps to determine the current weather conditions in those cities.  The city name and coordinates were then placed along with select information from the API call into a Pandas DataFrame (See Figure 1).

![](https://github.com/Scruffy-Bearie/World_Weather_Analysis/blob/main/DataFrameSample.png)

Following creating, user input was employed to select cities from the above data frame based on current temperature conditions to create a new data frame and an API call was made to Google Maps using existing latitude, longitude coordinate pairs to determine the name of the closest hotel in each city.  After appending the new data frame to include the name of the closest hotel in each city and removing null entries, the information was used to produce a Google Map with markers to indicate the location of all cities with current temperatures inside the range selected and pop up info boxes to display the name of the hotel, city an country along with current weather conditions (See Figure 2).

-	Link to figure 2

Using the map created above four cities in the same country were selected and an API call to Google Maps Directions was used to plot the best travel route between those cities (See Figure 3).  Finally, information acquired in previous steps was used to produce a Google Map with markers to identify selected cities and pop up info boxes to relay the name of the selected hotel, city and country along with current weather conditions (See Figure 4).

-	Link to figures 3 and 4

## Analysis

The results clearly demonstrate that API calls are valuable tools for collecting information and that when combined, through tools like Jupyter notebooks and python, with mapping technology like Google Maps capable of contributing to products with inherent consumer value.
