## Python API Project (What's the Weather Like?)

        To create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api) and to create a representative model of weather across world cities.

        This includes creation of a series of scatter plots to showcase the relationships and is to run linear regression on each relationship, separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 
        Performed a weather check on each of the cities using a series of successive API calls.


Used jupyter-gmaps and the Google Places API for this part of the project. Created a heat map that displays the humidity for every city from the part I of the project.
Narrowed down the DataFrame to find an ideal weather condition. Dropped rows that didn't contain all three conditions. Used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates. Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country. For max intensity in the heat map, set it to the highest humidity found in the data set.


API Querying (Imported API key from external script and used as variable;  correctly loops over the list of cities; no errors interrupt the API call loop; printed pur the current number and name of the city they are currently retrieving data for)

Data Modeling (a pandas dataframe is created and saved to a .csv from the data retrieved from the API; for part one the dataframe contains 500+ rows in all of the columns: city latitude, city longitude, max temperature, humidity, cloud coverage, wind speed, city country, city datetime; for part two dataframe created for city, country, latitude, longitude, hotel name, shows ten or less rows)

Plot Creation (a plot created with a title, axis labels and saved as a .png file for latitude vs temp, lat vs humidity, lat vs cloudiness, lat vs wind speed; a plot created for linear regression with a title, axis lavel and saved as a .png file for Northern Hemisphere temp vs lat, Southern Hemisphere temp vs lat, Northern Hemisphere hum vs lat, Southern Hemisphere hum vs lat, Northern Hemisphere cloudiness vs lat, Southern Hemisphere cloudiness vs lat, Northern Hemisphere wind speed vs lat, Southern Hemisphere wind speed vs lat)


Data Analysis (conducted analysis that provided sound reasoning to back up why all three trends are occuring; correct description of those observable trends)

Google Maps (created a heatmap, the second map contains pins for all the cities in the dataFrame, pins are clickable to display city, country, and hotel name placed on top of the heatmap)
