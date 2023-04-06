## Summary of Module 6 WeatherPy/VacationPy challenge for UC Berkeley's Data Analytics Bootcamp

## Part 1 WeatherPy

* This Python code randomly selects a group of 500+ cities across the world. Then, the code collects data from the OpenWeatherMap API to create a representatitve model of weather across world cities. The API data is used to graph the following relationships:
    * Temperature (F) vs. Latitude
    * Humidity (%) vs. Latitude
    * Cloudiness (%) vs. Latitude
    * Wind Speed (mph) vs. Latitude
* From the analysis, the following conclusions can be drawn:
    * Temperature seems to have a clear correlation with latitude
    * As expected, the weather becomes significantly warmer as one approaches the equator (0 Deg. Latitude). The southern hemisphere tends to be warmer this time of year than the northern hemisphere
    * There is no strong relationship between latitude and cloudiness. However, it is interesting to see that a strong band of cities near 0, 80, and 90% cloudiness
    * There is no strong relationship between latitude and wind speed. However, in northern hemispheres there is a flurry of cities with over 20 mph of wind
    * Wind speed tends to generally be betweeen 0 and 15 mph regardless of latitude
    * There is no strong relationship between latitude and humidity. however there is a slightly larger cluster of northern hemisphere cities with high humidity (above 60% humidity)
    
## Part 2 VacationPy
* This deliverable uses the weather data skills from Part 1 to plan future vacations using Jupyter notebooks, the geoViews Python library, and the Geoapify API: 
   * A map was created that displays a point for every city in the city_data_df DataFrame, where the size of the point relates to the humidity level in each city. 
   * The city_data_df DataFrame was narrowed down to find the ideal weather condition. 
   * A new DataFrame called hotel_df was created to store the city, country, coordinates, and humidity. 
   * For each city, the Geoapify API was used to find the first hotel located within 10,000 meters of the coordinates in hotel_df. 
   * Lastly, the hotel name and the country was added as additional information in the hover message for each city on the map.

## Files
* The analysis includes the following files:
    * A "WeatherPy.ipynb" Jupyter Notebook that contains the Python code for the analysis
    * An "api_keys.py" Python file that contains the OpenWeatherMap API and Geoapify keys used in the analysis. (note: if downloading this analysis, the user must put her or his OpenWeatherMap API Key and/or Geoapify Key into this file in order for the "WeatherPy.ipynb" Jupyter Notebook to work properly)
    * A "cities.csv" CSV file in the "output_data" folder that contains the CSV version of the DataFrame created in the Jupyter Notebook
    * Four PNG files in the "Figures" folder. Each of the four files is a graph created in the analysis
