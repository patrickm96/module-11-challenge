# module-11-challenge

The following resources were referenced in order to complete this challenge:

1. Extract all the text elements - TA Paveen clarified which class to display.
2. Extract titles and previews - Instructor Eli provided sample code.
3. How to loop through table - Instructor Eli provided sample code.
4. How to sort bars in increasing order - https://www.tutorialspoint.com/how-to-sort-bars-in-increasing-order-in-a-bar-chart-in-matplotlib
5. Change fig width - https://www.geeksforgeeks.org/change-plot-size-in-matplotlib-python/
6. Add grid lines to a plot - https://www.w3schools.com/python/matplotlib_grid.asp#:~:text=Add%20Grid%20Lines%20to%20a,grid%20lines%20to%20the%20plot.
7. How to group data in a DataFrame - https://www.geeksforgeeks.org/python-pandas-dataframe-groupby/
8. Save DataFrame as a csv file - https://www.geeksforgeeks.org/saving-a-pandas-dataframe-as-a-csv/

## Instructions
### Part 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.

Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.

Create a Beautiful Soup object and use it to extract text elements from the website.

Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

![image](https://github.com/patrickm96/module-11-challenge/assets/135382512/d6c02566-1062-4799-9d6a-86768efab2a7)

Store all the dictionaries in a Python list.

Print the list in your notebook.

Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)

### Part 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site.. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

- id: the identification number of a single transmission from the Curiosity rover
- terrestrial_date: the date on Earth
- sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
- ls: the solar longitude
- month: the Martian month
- min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
- pressure: The atmospheric pressure at Curiosity's location

Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

Analyze your dataset by using Pandas functions to answer the following questions:

- How many months exist on Mars?
- How many Martian (and not Earth) days worth of data exist in the scraped dataset?
- What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
- Find the average minimum daily temperature for all of the months.
- Plot the results as a bar chart.
- Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
- Find the average daily atmospheric pressure of all the months.
- Plot the results as a bar chart.
- About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
- Consider how many days elapse on Earth in the time that Mars circles the Sun once.
- Visually estimate the result by plotting the daily minimum temperature.

Export the DataFrame to a CSV file.
