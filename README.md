WeatherPy

In this project we use weather data take a look at the latitude of over 500 citites and seeing if there is a correlation between the temperature, humidity, cloudiness, and wind speed of each city.

Using the data, we create scatter plots and linear regression lines to determine the strength of each correlation based on the hemisphere.

When observing temperature we can see that the latitude does have a strong correlation on the temperature in each city. From the data we can see that as the latitiude moves further from the equator the temperature tends to decrease in both hemispheres.

Humidity, Cloudiness, wind speed on the other hand all showed little to no correlation when compared to the latitude.


VacationPy

In this project, we show how weather data can be used to plan future vacations using the Geoapify API and the geoViews Python library.

We start by crating a map that displays a point for every city in the city_data_df DataFrame where the size of the point indicates the humidity in each city.

We continue by narrowing down the city_data_df DataFrame to find ideal weather condition. using this requirements:
A max temperature lower than 27 degrees but higher than 21
Cloudiness less than 20%
Humidity less than 70%

The main objective is to limit the dataframe down to about 20 rows

Finally we create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, we use the Geoapify API to find the first hotel located within 10,000 metres of your coordinates and add the hotel name and the country as additional information in the hover message for each city in the map as in the following image:
