# WeatherPy and VacationPy

This project leverages various APIs and data analysis techniques to explore weather patterns and identify ideal vacation spots based on specific weather criteria. It is divided into two parts: **WeatherPy** and **VacationPy**.

## Part 1: WeatherPy

### Objective
Utilize the OpenWeatherMap API to retrieve and analyze weather data for various cities across the globe. Perform a series of analyses to examine how geographical latitude correlates with various weather factors.

### Key Analyses
1. **Weather Data Collection**:  
   Using the OpenWeatherMap API, weather data (temperature, humidity, cloudiness, and wind speed) is retrieved for a randomly generated list of cities.

2. **Scatter Plots**:
   - Latitude vs. Temperature
   - Latitude vs. Humidity
   - Latitude vs. Cloudiness
   - Latitude vs. Wind Speed

3. **Linear Regression Analysis**:  
   Compute linear regressions to investigate potential relationships between weather parameters and latitude for both the Northern and Southern Hemispheres:
   - Northern Hemisphere: Temperature vs. Latitude
   - Southern Hemisphere: Temperature vs. Latitude
   - Northern Hemisphere: Humidity vs. Latitude
   - Southern Hemisphere: Humidity vs. Latitude
   - Northern Hemisphere: Cloudiness vs. Latitude
   - Southern Hemisphere: Cloudiness vs. Latitude
   - Northern Hemisphere: Wind Speed vs. Latitude
   - Southern Hemisphere: Wind Speed vs. Latitude

4. **Findings**:  
   Explore and interpret the linear regression models to determine if any notable relationships exist between the variables. Provide insights based on the scatter plots and regression results.

### Tools and Libraries
- **APIs**: OpenWeatherMap
- **Python Libraries**: Pandas, Matplotlib, Seaborn, SciPy

---

## Part 2: VacationPy

### Objective
Using the weather data analysis skills developed in WeatherPy, plan ideal vacation spots based on specific weather preferences.

### Steps:
1. **Mapping Cities**:  
   Create a map to visualize all cities in the dataset, with each point's size representing the humidity level in that city. Utilize geoViews and the Geoapify API for mapping.

2. **Filtering for Ideal Conditions**:  
   Filter the dataset (`city_data_df`) to match specific weather conditions:
   - Maximum temperature lower than 27°C but higher than 21°C
   - Wind speed less than 4.5 m/s
   - Zero cloudiness

3. **Finding Hotels**:  
   For each filtered city, use the Geoapify API to find the nearest hotel within 10,000 meters of the city's coordinates. Store information on the city, country, coordinates, and humidity, along with the name of the nearest hotel.

4. **Displaying on a Map**:  
   Create an interactive map to display the filtered cities and their associated hotels. Hovering over a point will show additional information such as the hotel name, city, country, and weather details.

### Tools and Libraries
- **APIs**: Geoapify, OpenWeatherMap
- **Python Libraries**: Pandas, geoViews, Matplotlib, Jupyter Notebooks
- **Mapping**: geoViews, Geoapify API

---

## Results and Insights
- In **WeatherPy**, we identified correlations between latitude and various weather parameters, such as temperature being higher in equatorial regions and lower toward the poles.
- In **VacationPy**, the combination of weather data and mapping allowed us to filter and visualize ideal vacation spots based on specific weather preferences, making it easier to plan vacations based on preferred conditions.

---
