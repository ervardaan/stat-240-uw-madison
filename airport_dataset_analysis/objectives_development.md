# usage of tidyr,readr

data provided by the US Customs and Border Protection Agency which tracks time to clear customs at many US airports.
Accessing this data will involve several new concepts.
Reading in data in different formats
More detail on working with dates
Writing functions
Iteration

Downloaded data is as an HTML file for each airport with a single table that is complicated by using three rows for a header and some fields which span multiple columns.
There is a package in the tidyverse called rvest which can read in data from many HTML files, but it does not handle well this example due to the complicated header structure.
Instead, we will use the package XML and a command readHTMLTable() for one of the files.
We will illustrate using readHTMLTable() for data from a single airport and a single HTML file, and then write the results to the more typical CSV file for one example.
For other airports, we will begin from the already cleaned CSV files.

Packages:

tidyverse

lubridate

XML

link:https://bookdown.org/bret_larget/stat-240-case-studies/airport-waiting-times.html

development:reading,importing files,working with plain text files,excel files,working with dates and strings using lubridate,reading data with purr

### Airport Waiting Time Data Analysis

Exploratory Data Analysis,Summarize Key Variables

# questions asked

Is there any missing data?

How many passengers and flights are there at each airport/terminal combination? Create a table with these summary statitics. Add a column total_airport_passengers which includes the total number of passengers in the corresponding airport across all terminals. (Note: this column will repeat values for airports with multiple terminals.) Arrange the table by descending order of this total airport passengers variable and then descending by total passengers per terminal. Then delete the total_airport_passengers column before printing the table.

How many days of data are there for each airport?

Find which date is missing for each data set

Does the all_total variable match the sum of the other columns of passenger counts?

At what time of day and at which airports are these mismatches happening?Create a histogram to show the distribution of the size of these mismatches.

Are some months busier than others?

Are some days of the week busier than others?
Are some times during the day busier than others?
Are some airports more efficient that than others in terms of average wait time?

Are some airports more efficient in the number of people served by hour per available booth?

Are some months busier than others?

Are some days of the week busier than others?

Are some times during the day busier than others?

Are some airports more efficient than others in terms of average wait time?

Do airports differ in the number of passengers processed per booth?

Display the median values in a bar graph

What is the average waiting time at each airport for all passengers?

Are some airports more efficient in the number of people served by hour per available booth?

During times with at least 100 arrivals per hour, what is the average hourly rate of number of passengers served by each booth at various airports?
