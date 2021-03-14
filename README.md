# python-api-challenge

## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how would you **prove** it?

![Equator](Images/equatorsign.png)

## WeatherPy

Objective was to write a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a the citipy Python library(https://pypi.python.org/pypi/citipy), the OpenWeatherMap API(https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

To do this a series of scatter plots were built to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The final notebook:

* Randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save both a CSV of all data retrieved and png images for each scatter plot.


Observable Trends
1. Max temperature increases as latitude approaches 0, or as latitude approaches the equator. However, temperature does max out at around 20 degress latitude not right at the equator. 
2. The plots for humidity and cloudiness don't appear to showing any discernable trend or pattern. The data points appear to be pretty randomly distributed over the graphs. More analysis is needed to determine the drivers of humidity and cloudiness. 
3. Wind speeds don't seem to be fluctuating or changing very much based on latitude as the data points are pretty evenly spread over the latitude measurements. However, the highest wind speed readings are coming from points further away from the equator. 