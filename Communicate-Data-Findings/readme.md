# (Ford Gobike Data Exploration)
## by (Aditya kumar)

## Dataset

> This project is divided into two major parts. In the first part, you will conduct an exploratory data analysis on a dataset Ford GoBike System Data. I will use Python data science and data visualization libraries to explore the dataset’s variables and understand the data’s structure, oddities, patterns and relationships. The analysis in this part should be structured, going from simple univariate relationships up through multivariate relationships. 


> In the second part, I will take my main findings from my exploration and convey them to others through an explanatory analysis. To this end, I will create a slide deck that leverages polished, explanatory visualizations to communicate my results.

> This document explores a dataset containing the trip data of the ford gobike approximately 183,412 with 16 features (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude ,end_station_longitude, bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip). Most variables are 9 numerical, and others are 2 datetime, 4 object type and 1 is boolean type.

> For clean dataser are the following:
> 1- change the data type for start and end time to be datetime64.
> 2- change the data type for bike_share_for_all_trip to be bool.


## Summary of Findings

> Trip Duration is so dependendable on the age of the member, when the age between 20 to 45, the trip duration is higher than the older ages.
> For the age, duration, and gender, for the others leap at an older age (around 60 years) to got 3000 trip duration.
> For the age, duration, and user type, both Customer and Subscriber are showing similar trends for age and trip duration, but for subscribers the trip duration is higher for older age.

## Key Insights for Presentation

>Distribution of Trip Durations:
Trip Durations in the dataset take on a very large range of values. Number of Trips values first increases starting from around 8000 values to 12500 values at peak around 600 seconds but then starts to fall below at 2000 values.

>Distribution of User Age:
In the case of age, the distribution is more concentrated between 20 to 40 years old.
