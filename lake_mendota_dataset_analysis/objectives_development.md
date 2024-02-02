MAIN FOCUS IS GGPLOT

Scientists have been recording the dates when Lake Mendota first closes with ice (at least half the surface is covered with ice) and opens (more than half the surface is liquid water) since the middle of the 1800s.
In most winters, there is a single uninterrupted period of time from the first time the lake is closed in the winter to the first time it reopens in the spring.
Some winters have multiple intervals of closure
The data set we are using summarizes the raw data with a single row for each winter from 1855–56 through last winter, 2021–22.
The variable year1 is the first year of the given winter.
The variable duration is the total number of days that Lake Mendota was closed by ice in the given winter. (Note: the word “winter” used here specifies a single season spanning two consecutive calendar years and does not use the endpoints from the winter solstice to the spring equinox, for example.)
We will first create graphs to examine the question, “How long does Lake Mendota freeze each winter?” with graphical exploration of the variable duration.
Subsequently, we will examine the question, “How has the duration that Lake Mendota freezes each winter changed over time?” by exploring the relationship between duration and year1.

link: https://bookdown.org/bret_larget/stat-240-case-studies/madison-lakes.html

development-

read data,exploratory data analysis using ggplot2,single variable plots,histogram,boxplots,density plots,side by side plots,bar graphs,facets,Scales,Coloring,Themes,Aesthetics,Geoms


QUESTIONS ASKED

How do the total number of days that Lake Mendota is closed with ice vary over time?

In a typical year, how much does the actual duration for which Lake Mendota is frozen (the surface is at least 50% covered by ice) vary from its predicted value? (How far apart are the black points and the blue curve, typically, in a given year)?

When in the winter does Lake Mendota typically close with ice the first time?


How has the duration that Lake Mendota is closed by ice (at least 50% covered by ice) changed over time?

1. Are there changes to the typical dates that Lake Mendota first freezes in the winter and finally thaws in the spring?

2. Can we predict the thaw date based on the date the lake first freezes?

3. Can we predict the total duration that the lake will be frozen in the upcoming winter?

4. Is the model for the trend appropriate? Would a simpler straight-line model be adequate?

5. Can we characterize the distribution of variation around the trend line?

6. Is the rate of decrease in the total freeze duration larger now than it was between 1850 and 1900?


