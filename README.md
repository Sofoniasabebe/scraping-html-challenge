# scraping-html-challenge

This project consists of two technical products/deliverables:

* Deliverable 1: Scrape titles and preview text from Mars news articles.

* Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

### Part 1: Scrape Titles and Preview Text from Mars News

For this section, the following tasks were done:

1. Used automated browsing to visit the Mars news site and inspected the page to identify which elements to scrape.
2. Created a Beautiful Soup object and used it to extract text elements from the website.
3. Extracted the titles and previewed text of the news articles that were scraped. Stored the scraping results in Python data structures and printed the list in the notebook. 
4. Exported the scraped data to a JSON file to ease sharing the data with others. 

### Part 2: Scrape and Analyze Mars Weather Data

For this section, the following steps were followed:

1. Automated browsing was used to visit the Mars Temperature Data site. The page was inspected to identify which elements to scrape. 
2. A Beautiful Soup object was created and used to scrape the data in the HTML table.
3. Assembled the scraped data into a Pandas DataFrame. The columns have the same headings as the table on the website. Here’s an explanation of the column headings:
* id: the identification number of a single transmission from the Curiosity rover
* terrestrial_date: the date on Earth
* sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
* ls: the solar longitude
* month: the Martian month
* min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
* pressure: The atmospheric pressure at Curiosity's location
4. Examined the data types that are associated with each column.
5. Analyzed the dataset by using Pandas functions to answer the following questions:
* How many months exist on Mars?
* How many Martian (and not Earth) days worth of data exist in the scraped dataset?
* What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question, the average minimum daily temperature for all of the months were calculated and the results were plotted in a bar chart.
* Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question, the average daily atmospheric pressure of all the months were calculated and the results were plotted in another bar chart.
* About how many terrestrial (Earth) days exist in a Martian year? To answer this question, I considered how many days elapse on Earth in the time that Mars circles the Sun once, as required. Then, visually estimated the result by plotting the daily minimum temperature of each observation.
6. Expored the DataFrame to a CSV file. 

## Analysis of the Findings

#### Minimum Temperature
The bar chart shows that Month 3 appears to be the coldest month on Mars with tempreatures approaching -80C. The fourth and second month also have cold temperatures indicating that between month 2 and 4 may be Mars' coldest season. 

Months 8,9, and 10, on the other hand, appear to have relatively warmer average minimum temperatures. This also could indicate the interval for Mars' warmer season. 

These indicators concur with NASA's finding that Mars is similar to earth in having distinct seasons due to both having axis of rotation, 25 degrees for Mars and 23.4 degrees for Earth. Also, according to NASA, a year on Mars lasts 669.6 sols, which is the same as 687 Earth days. 
(https://science.nasa.gov/mars/facts/)

#### Atmospheric Pressure
According to the bar chart for Atmospheric Pressure, the highest atmospheric pressure occurs around the 9th and 10th months. Months 5 and 6 show lowest atmospheric pressure. 

In comparison to the temperatures on Mars, atmospheric pressure is highest when temperatures are warmer and pressure decreases as the temperature is colder. Both observations strengthen the idea that there are seasonal variations in Mars. 

#### Year Length
We can see from the plot showing minimum temperature over time that the temperture cycles repeat approximately every 687 Earth days. This is consitent with astronomical data from MARS suggesting that a full Martian year is about 687 days. (https://science.nasa.gov/mars/facts/) 

Although the years are twice as long on Mars, the fact that the cold and warm periods appearing in regular intervals indicate relative predictability with regard to probable seasons on Mars. 

The chart also indicates that the highest minimum temperatures occur around -65C and the lowest minimums peak around -90C. Some of the spikes and dips may be due to 'short-term weather events' like dust storms according to NASA (https://science.nasa.gov/mars/facts/). 

In conclusion, while a year on Earth lasts about 365 days, a year on Mars lasts 687 Earth days. This leads to longer seasons and more extream weather variations on Mars. 

**References**

*The Mars News websiteLinks to an external site. is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars NewsLinks to an external site. website in November 2022. Images are used according to the JPL Image Use PolicyLinks to an external site., courtesy NASA/JPL-Caltech.*

*For analyzing the findings, I consulted the NASA Mars Factsheet website at https://science.nasa.gov/mars/facts/ .* 