Part 1: WeatherPy

Use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. 

Next, create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed



Compute Linear Regression for each relationship by plotting 

Northern Hemisphere: Temperature vs. Latitude;  Southern Hemisphere: Temperature vs. Latitude

Northern Hemisphere: Humidity vs. Latitude;  Southern Hemisphere: Humidity vs. Latitude

Northern Hemisphere: Cloudiness vs. Latitude;  Southern Hemisphere: Cloudiness vs. Latitude

Northern Hemisphere: Wind Speed vs. Latitude;  Southern Hemisphere: Wind Speed vs. Latitude

Then explain what the linear regression is modeling. 

Describe any relationships that you notice and any other findings you may uncover.







Part 2: VacationPy

Use the weather data skills to plan future vacations. Use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

Create a map that displays a point for every city in the city_data_df DataFrame. The size of the point should be the humidity in each city.
Narrow down the city_data_df DataFrame to find your ideal weather condition. 

For example: 
A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness

Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
Add the hotel name and the country as additional information in the hover message for each city on the map. 
