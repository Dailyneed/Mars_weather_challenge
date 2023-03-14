# Mars_weather_challenge: Web-scraping and data analysis project

## Background
You've learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You decide to use the the knowledge to scrape mars facts from HTML table.

## Objective
The purpose of this project is to use automated browsing with Splinter and HTML parsing with Beautiful Soup to scrape information from HTML table, and use Pandas to analysis the information.

## Technologies
Splinter,
Beautiful Soup,
Pandas,
Python,
Selenium

## Instruction:
### Part 1: Srape Titles and Preview Text from Mars News
In this section, you'll use automated browsing to visit the Mars news site. Inspect the page to identify which elements to scrape.
Create a Beautiful Soup object and use it to extract text elements from the website.
Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

  Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
 
Store all the dictionaries in a Python list.

Print the list in your notebook.

Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)

## Part 2: Scrape and Analyze Mars Weather Data
In this section, use automated browsing to visit the Mars Temperature Data Site. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

Analyze your dataset by using Pandas functions to answer the following questions:
  How many months exist on Mars?
  How many Martian (and not Earth) days worth of data exist in the scraped dataset?
  What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
    Find the average minimum daily temperature for all of the months.
    Plot the results as a bar chart.
    
  Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    Find the average daily atmospheric pressure of all the months.
    Plot the results as a bar chart.
    
  About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    Visually estimate the result by plotting the daily minimum temperature.
    
Export the DataFrame to a CSV file.

# Reference
Jason Lepelmeier,(2023, Mar 09). Class lecture: Data- Collection - Automated Browsing(1.12).pdf. Data Analytics and Visualization Bootcamp. https://umn.bootcampcontent.com/University-of-Minnesota-Boot-Camp/UofM-VIRT-DATA-PT-12-2022-U-LOLC/-/blob/main/11-Data%20-%20Collection/3/Unit%2011.3%20Lesson%20Plan%20Slides%20(1.12).pdf
