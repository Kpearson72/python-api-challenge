# Python API Homework - What's the Weather Like?

![Equator](Images%20/equatorsign.png)


## Part I - WeatherPyImages 


The task was to create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 

The first requirement was to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
![lat v. temp](WeatherPy/output_data/lat_vs_Temp.png)
* Humidity (%) vs. Latitude
![lat v. humidity](WeatherPy/output_data/lat_vs_humidity.png)
* Cloudiness (%) vs. Latitude
![lat v. cloudiness](WeatherPy/output_data/lat_vs_cloudiness.png)
* Wind Speed (mph) vs. Latitude
![lat v. windspeed](WeatherPy/output_data/lat_vs_windspeed.png)

The second requirement was to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
![N hemisphere temp v. lat](WeatherPy/output_data/N_hemisphere_maxtemp.png)

* Southern Hemisphere - Temperature (F) vs. Latitude
![S hemisphere temp v. lat](WeatherPy/output_data/S_hemisphere_maxtemp.png)
  
* Northern Hemisphere - Humidity (%) vs. Latitude
![N hemisphere humidity v. lat](WeatherPy/output_data/N_hemisphere_humidity.png)

* Southern Hemisphere - Humidity (%) vs. Latitude
![S hemisphere humidity v. lat](WeatherPy/output_data/S_hemisphere_humidity.png)
  
* Northern Hemisphere - Cloudiness (%) vs. Latitude
![N hemisphere cloudiness v. lat](WeatherPy/output_data/N_hemisphere_cloudiness.png)

* Southern Hemisphere - Cloudiness (%) vs. Latitude
![S hemisphere cloudiness v. lat](WeatherPy/output_data/S_hemisphere_cloudiness.png)

* Northern Hemisphere - Wind Speed (mph) vs. Latitude
![N hemisphere windspeed v. lat](WeatherPy/output_data/N_hemisphere_windspeed.png)

* Southern Hemisphere - Wind Speed (mph) vs. Latitude
![S hemisphere windspeed v. lat](WeatherPy/output_data/S_hemisphere_windspeed.png)

My final [jupyter notebook](https://github.com/Kpearson72/python-api-challenge/blob/main/WeatherPy/WeatherPy.ipynb) included:

* Randomly selected cities (at least 500) based on latitude and longitude.
* A weather check on each of the cities using a series of successive API calls.
* A print log of each city as it's being processed with the city number and city name.
* A saved [CSV](https://github.com/Kpearson72/python-api-challenge/blob/main/WeatherPy/output_data/city_df.csv) file of all retrieved data and a PNG image for each scatter plot.

### Part II - VacationPy

![hotel_map](Images%20/hotel_image.png)

**Planning a future vacation**

I used jupyter-gmaps and Google Places API for this part of the assignment.

Tasks for this part of the project consisted of:

* Creating a heat map that displays the humidity for every city from Part I - WeatherPy

![heatmap](VacationPy/images/Screen%20Shot%202020-12-13%20at%206.42.29%20PM.png)

* Narrowing down the DataFrame to find my ideal weather condition. It had to have:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Dropped any rows that don't contain all three conditions. You want to be sure the weather is ideal.

* Using Google Places API to find the first hotel for each city located within 5000 meters of the cities coordinates.

* Plotting the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

![heatmap with pinned hotels](VacationPy/images/Screen%20Shot%202020-12-13%20at%206.42.19%20PM.png)

As a final consideration:

I completed my analysis using a Jupyter notebook. 
* [WeatherPy Notebook link](https://github.com/Kpearson72/python-api-challenge/blob/main/WeatherPy/WeatherPy.ipynb)
* [VacationPy Notebook link](https://github.com/Kpearson72/python-api-challenge/blob/main/VacationPy/VacationPy.ipynb)



