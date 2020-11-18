# Python API Project - What's the Weather Like?

## Background

Utilized Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"


## Part I - WeatherPy

Created a Python script to visualize the weather of 500+ randomly selected cities across the world of varying distance from the equator. To accomplish this, I utilized a [simple Python library](https://pypi.python.org/pypi/citipy), and the [OpenWeatherMap API](https://openweathermap.org/api), to create a representative model of weather across world cities.


* Randomly selected **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* Performed a weather check on each of the cities using a series of successive API calls.
* Included a print log of each city as it's being processed with the city number and city name.
* Saved a CSV of all retrieved data and a PNG image for each scatter plot.


Then I Create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

I ran linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). I created a function that creates the linear regression plots to speed things along.


### Part II - VacationPy

For this section, I utilized juptyter notebooks and the Google Places API.

* Created a heat map that displays the humidity for every city from the part I of this project.

* Narrowed down the DataFrame to find my ideal weather condition. 

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Dropped any rows that don't contain all three conditions. 

* Using Google Places API I foundd the first hotel for each city located within 5000 meters of your coordinates.

* Plotted the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.


Thank you for visiting my GitHub.

Arlette Varela