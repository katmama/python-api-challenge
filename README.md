Unit 6 Homework: What's the Weather Like?

Background
Whether financial, political, or social—data's true power rests in its ability to answer questions definitively. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
Now, we know what you may be thinking: "Duh. It gets hotter ..."
But, if pressed, how would you prove it?

Part 1: WeatherPy
In this section, you'll create a Python script to visualize the weather of 500+ cities of varying distance from the equator. To do so, you'll use a simple Python library, the OpenWeatherMap API, and your problem-solving skills to create a representative model of weather across cities.
The first requirement is to create a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

After each plot, add a sentence or two explaining what the code is analyzing.
The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, explain what the linear regression is modeling. For example, describe any relationships that you notice and any other findings you may have.
Your final notebook must:

Randomly select at least 500 unique (non-repeated) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed, with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.


Part 2: VacationPy
Now, let's use your skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.


Note: Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out Google Maps Platform Billing and Manage your cost of use for more information.


Note: If you are having trouble displaying the maps, run jupyter nbextension enable --py gmaps in your environment and then retry.


To complete this part of the assignment, you will need to do the following:


Create a heat map that displays the humidity for every city from Part 1, as in the following image:



Narrow down the DataFrame to find your ideal weather condition. For example:


A max temperature lower than 80 degrees but higher than 70.


Wind speed less than 10 mph.


Zero cloudiness.


Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.


Note: Feel free to adjust your specifications, but make sure to limit the number of rows returned by your API requests to a reasonable number.




Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.


Plot the hotels on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country, as in the following image:

![image](https://user-images.githubusercontent.com/99552079/166125606-eec0438f-b4a6-471c-ba04-efe6fad21132.png)
