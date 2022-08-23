# **python-api-challenge :  What's the Weather Like?**
## **Background**
Whether financial, political, or social—data's true power rests in its ability to answer questions definitively. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
Now, we know what you may be thinking: "Duh. It gets hotter ..."
But, if pressed, how would you prove it?

## **Before You Begin**


1. Create a new repository for this project called python-api-challenge and be sure to select a .gitignore template for Python.  Do not add this homework to an existing repository.


2. Clone the new repository to your computer.


3. Use Visual Studio Code to open this new repo and then edit the .gitignore file to add the following the top of the file.

    # Adding file to hold API keys. 
    api_keys.py

Note: the entry above can really appear anywhere in your .gitignore file, but directing everyone to put it at the top of the file makes these instructions easier to follow. Also note that if you choose to use a different file to hold your api keys, for example config.py, then you'll have to add this different filename to your .gitignore file (instead of what's listed above).


4. Create new files called WeatherPy.ipynb and VacationPy.ipynb. These will be the main scripts to run for each analysis.


5. Use Git to add, commit, and push the above changes to GitHub.

## **Part 1: WeatherPy**

The first requirement is to create a series of scatter plots to showcase the following relationships:

 * Temperature (F) vs. Latitude

 * Humidity (%) vs. Latitude

 * Cloudiness (%) vs. Latitude

 * Wind Speed (mph) vs. Latitude

After each plot, add a sentence or two explaining what the code is analyzing.
The second requirement is to compute the linear regression for each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

 * Northern Hemisphere - Temperature (F) vs. Latitude

 * Southern Hemisphere - Temperature (F) vs. Latitude

 * Northern Hemisphere - Humidity (%) vs. Latitude

 * Southern Hemisphere - Humidity (%) vs. Latitude

 * Northern Hemisphere - Cloudiness (%) vs. Latitude

 * Southern Hemisphere - Cloudiness (%) vs. Latitude

 * Northern Hemisphere - Wind Speed (mph) vs. Latitude

 * Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, explain what the linear regression is modeling. For example, describe any relationships that you notice and any other findings you may have.

Your final notebook must:

 * Perform a weather check on each of the cities using a series of successive API calls.

 * Include a print log of each city as it's being processed, with the city number and city name.

 * Save a CSV of all retrieved data and a PNG image for each scatter plot.

## **Part 2: VacationPy**

Now, let's use your skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.


**Note**: Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out Google Maps Platform Billing and Manage your cost of use for more information.

To complete this part of the assignment, you will need to do the following:


1. Create a heat map that displays the humidity for every city from Part 1.


2. Narrow down the DataFrame to find your ideal weather condition. For example:

 * A max temperature lower than 80 degrees but higher than 70.


 * Wind speed less than 10 mph.


 * Zero cloudiness.


 * Drop any rows that don't satisfy all three conditions. You want to be sure the weather is ideal.


**Note**: Feel free to adjust your specifications, but make sure to limit the number of rows returned by your API requests to a reasonable number.




3. Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.


4. Plot the hotels on top of the humidity heatmap, with each pin containing the Hotel Name, City, and Country.


## **What to submit:**

 * You must complete your analysis using a Jupyter notebook.

 * You must use the Matplotlib or Pandas plotting libraries.

 * For Part 1, you must include a written description of three observable trends based on the data.

 * For Part 2, you must take a screenshot of the heatmap that you create and include it in your submission.

 * Your plots must include labeling aspects like plot title (with date of analysis) and axis labels.

 * For max intensity in the heatmap, try setting it to the highest humidity found in the dataset.
