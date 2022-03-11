# Hawaii Weather Analysis

# Overview of Analysis

In this analysis, my overall goal was to summarize the weather on the island of Oahu. Using the sqlalchemy library in python, I accessed a sqlite database holding daily Oahu weather data covering the years 2010-2017. To get a baseline description for the weather, I ran two queries: The first query gathered all of the temperatures from all of the nine temperature stations on Oahu for days in the month of June. The second query did the same thing for days in the month of December.  I stored both of the queries in lists and then transformed each list to a pandas dataframe. Lastly, I observed statistics for the temperatures in both months by using the pandas describe function. By observing temperature data from two opposite sides of the calendar, I'm able to get a feel for the overall weather for the full year.

# Results

## June Temperature Statistics

![June temps](https://user-images.githubusercontent.com/95651156/156652366-9b1d5281-5183-476e-b793-8ce92fbc90d2.png)

## December Temperature Statistics

![December temps](https://user-images.githubusercontent.com/95651156/156652684-29adc424-67c3-42bb-b819-cb60a640cd11.png)

### Key Takeaways from Results

* The average temperature in Oahu for the month of June (74.94 degrees farenheit) is nearly four degrees higher than that of the month of December (71.04 degrees farenheit)
* The highest temperature recorded in Oahu for the month of June (85) is just two degrees higher than the highest temperature for the month of December (83)
* The lowest temperature recorded in Oahu for the month of December (56) is eight degrees lower than the lowest temperature for the month of June (56)
* Temperatures in Oahu for the month of December varied slighlty more (standard deviation of 3.75 degrees) than temperatures for the month of June (standard deviation of 3.26 degrees)

# Summary

From looking at the temperatures and temperature statistics for the months of June and December, it's clear that the temperature patterns in Oahu for the months of June and December are actually quite similar. Because the average, maximum and minimum temperatures are so close to each other in two months that are in opposite "seasons" of the year, I can be relatively certain that the weather is relatively steady (and warm) throughout the year. 

To get an even better feel for the weather during these two months, I have decided to run the two queries from before, but with temperatures replaced by precipitation levels. After storing the query results in two lists and transitioning the lists to pandas dataframes, I used the describe function to get the following two tables:

## June Rainfall Statistics

![June Rainfall](https://user-images.githubusercontent.com/95651156/156684771-8496c12f-2767-4a80-8f79-e5fc1d1a5fcd.png)

## December Rainfall Statistics

![December Rainfall](https://user-images.githubusercontent.com/95651156/156684817-736f3ab5-ae23-4140-9284-6e7017907455.png)

I see that the average daily rainfall in Oahu for the month of December is about .08 points higher than the month of June, which I would argue is a bigger gap on a relative scale than the difference we saw in temperatures for the two months. Overall, while these charts show that Oahu receives substantial rain (sometimes in large amounts), it does not rain nearly enough to spoil the ideal moderate temperatures felt throughout the year.



