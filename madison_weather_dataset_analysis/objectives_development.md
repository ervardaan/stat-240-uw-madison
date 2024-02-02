## dplyr usage

merging datasets,adding new columns,selecting columns,filtering rows,creating summary rows,arranging rows,columns,piping

We will be working with data set containing weather data on Madison collect over a number of years from different weather stations.
In addition to investigating different scientific questions on the data, we will also be learning about the dplyr package from tidyverse which is “a grammar of data manipulation.”
Overview of Madison Weather Data
The source of the data for this week is from the National Oceanic and Atmospheric Administration (NOAA) of the United States.

link:https://bookdown.org/bret_larget/stat-240-case-studies/madison-weather.html

The data file is madison-weather-1869-2022.csv, and the variable descriptions are provided below.

STATION: unique code for the weather station
NAME: station name
LATITUDE: station latitude
LONGITUDE: station longitude
ELEVATION: station elevation (feet above sea level)
DATE: date of observations
PRCP: precipitation (inches, water)
SNOW: snow fall (inches)
SNWD: snow depth (inches)
TAVG: daily average air temperature (degrees Fahrenheit)
TMAX: maximum air temperature (degrees Fahrenheit)
TMIN: minimum air temperature (degrees Fahrenheit)

development:

load and read dataset, transform data, solve problem of missing values, write to files

## questions asked

Create a summary table of the data with the average temperature per year. Then, make an effective plot of this data to show patterns over time and variation around the main pattern.

Meteorologists often determine weather norms by averaging over a 30-year period. Create a variable which partitions the data into 30-year periods from 1871-1900, 1901-1930, and so on. Ignore the years before 1871 and 2021.

Find the daily maximum and minimum temperatures for each day of the year in different data frames
Record the year and the temperature for each record
If there are ties, have a separate row for each year

On what date did Madison have the highest recorded temperature? What was the this temperature and how many different times was it achieved?

Which dates have the most ties for the highest temperature?

What is the record latest date in the first six months of the year where the daily minimum temperature was below 32 degrees Fahrenheit? In which years did this occur?

Make a summary table of the number of days for each 30-year period and month with the proportion of days with precipitation
