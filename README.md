# superset

In visualizing the time series data using https://superset.apache.org/ for some data sets, the time column  name and its type is not automatically detected at least for v3.8.6.
A column alias _timestamp can be used as a work around.

Example:
Imported the following data with a column ‘TravelDate’ (removed the space)
https://raw.githubusercontent.com/apache-superset/examples-data/master/tutorial_flights.csv
SELECT Datetime as _timestamp, Cost , Distance  from tutorial_flights2;

