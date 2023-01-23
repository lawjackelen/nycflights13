# Modeling Late NYC  Flights

## Problem Statement

Inconsistencies in a flight’s scheduled and experienced itinerary can have a butterfly affect on important business travel, vacations, time-sensitive situations, and everything else in its path! User-side, understanding the possibility of a late flight can allow contingencies to be made. Business-side, saving operations costs and headaches as well as maintaining a great customer experience. No matter how you slice it, understanding how and when late flights happen is important.

Given flight dataset detailing flights from New York City airports (JFK, Newark, LaGuardia) from January 2013 until July 2013, create a model for predicting late flights.

## Requirements
This project requires few libraries:
-  pandas
-  numpy
-  matplotlib.pyplot
-  seaborn
-  sklearn

## Project Directory
```
lexisnexis
|__ code
|   |__ 01_EDA.ipynb
|   |__ 02_Preprocessing.ipynb
|   |__ 03_Modeling.ipynb
|__ data
|   |__ flight_history.csv
|   |__ flight_test.csv
|   |__ cleaned_flight_history.csv
|   |__ cleaned_flight_test.csv
|   |__ x_test_ss_processed.csv
|   |__ y_test_processed.csv
|   |__ x_train_ss_processed.csv
|   |__ y_train_processed.csv
|__ presentation.md
|__ README.md
```

## Data Dictionary
|Feature|Description|
|---|---|---|---|
||year|Numeric year for that flight|
|month|Numeric month for that flight|
|day|Numeric day for that flight|
|dep_time|Actual Time of departure (24 hr clock –HHMM,  local timezone)|
|sched_dep_time|Scheduled Time of departure (24 hr clock –HHMM, local timezone)|
|dep_delay|Delay of departure in minutes|
|arr_time|Actual Arrival time of arrival (24 hr clock -HHMM, local timezone)|
|sched_arr_time|Scheduled Time of arrival (24 hr clock – HHMM, local timezone)|
|arr_delay|Delay of arrival in minutes|
|carrier|2 byte carrier code|
|flight|flight number|
|tailnum|tail number of the plane for that flight|
|origin|3 byte origin airport code|
|dest|3 byte destination airport code|
|air_time|length of flight spent in air in minutes|
|distance|distance between origin and dest airports in miles|
|hour|hour of scheduled time of departure|
|minute|minute of scheduled time of departure|
|time_hour|Day and Time of scheduled departure to the hour|
|weekday|Name of Day of week of scheduled departure|
|month_penetration|Day of departure divided by the month of departure's total days|
|weekday|Name of Day of week of scheduled departure|
|carrier_late_rate|Proportion of flights in training set that were late by carrier|
|origin_delayed_rate|Proportion of flights in training set that were delayed by origin|
|origin_late_rate|Proportion of flights in training set that were late by origin|
|dest_delayed_rate|Proportion of flights in training set that were delayed by destination|
|dest_late_rate|Proportion of flights in training set that were late by destination|
|sched_distance_rounded|distance between origin and destination airports in miles, rounded to nearest 100|
