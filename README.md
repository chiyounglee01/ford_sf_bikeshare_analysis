# Ford GoBike Bikeshare Data Exploration

## Dataset

183412 bike rentals from the Ford GoBike bikeshare service in the San Francisco Bay area. The dataset contained 183412 entries and the data was collected from 02/01/2019 to 03/01/2019. The information includes duration of rentals, user type, date, gender, start station id and end station id. It can be found [here](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv),  with feature documentation available [here](http://ggplot2.tidyverse.org/reference/diamonds.html).


## Summary of Findings

In the exploration, I was mainly interested in what affects
bikeshare usage and bike rental duration time.

I found that 90.5 percent of bikeshare users were subscribers and
only 9.5 percent were customers. The bikeshare users were overwhelmingly
male, with males three times more likely to rent bikes than females or other combined.
Most bike users were between the ages of 20 and 40. More bikes were rented on weekdays
than weekends. Also, alot of the bikes seem to be rented for commute as 8:00 and 17:00
military time had the most rentals.


I found that there was no correlation between age and 
bike rental duration time. But customers had an average of 5 minutes
longer bike rental duration than subscribers.

## Key Insights for Presentation

For the presentation, I first focus on the factors that influence bikeshare
usage. I first show the ratio of subscribers and customers with a pie chart.
I then compare the number of bike rents made by male, female and other gender
by using a countplot. Then I show the distribution of Bike Rent Counts by Age
using a histogram. I then show the bike rent count by day of week using a countplot.
I use another countplot to show the bike rent count by hour of day.

Afterwards, I make a scatterplot between duration and age to see if there
is a correlation between those two factors. I found there were extreme outliers
through the scatterplot, so I filtered out 700 entries with duration of 100 minutes
or more to make the next plot. For the final plot I compare average duration between
User Type and Gender by using a barplot with the gender as hue.
