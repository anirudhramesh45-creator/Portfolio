# Capital Bikeshare: Member vs Casual Rider Analysis

## Project Overview

This project analyzes Capital Bikeshare trip data to understand differences in bike rental patterns between **member riders** and **casual riders**.

The main research question is:

> **How do bike rental patterns differ between member and casual riders with respect to time, place, and ride duration?**

Three Capital Bikeshare datasets were downloaded and combined into a single dataset for the analysis.

## Analysis Objectives

The analysis focuses on:

* **Time:** Compare riding patterns by hour of day, day of week, weekday vs. weekend, and month.



Additional analysis includes bike type preferences and rider activity by day and hour.

## Dataset

The project uses publicly available trip data from **Capital Bikeshare**.

The dataset includes information such as:

* Ride ID
* Bike type
* Start date and time
* End date and time
* Start station
* End station
* Station latitude and longitude
* Rider type (`member` or `casual`)

## Tools and Libraries

The analysis was completed in a Jupyter Notebook using Python.

Main Python libraries:

```text
pandas
numpy
matplotlib
seaborn
```

## Data Preparation

Before analysis, the following steps were performed:

1. Combined three Capital Bikeshare data files.
2. Converted start and end timestamps to datetime format.
3. Calculated ride duration in minutes.
4. Created hour, day, month, and weekday/weekend variables.
5. Checked missing values and duplicate records.
6. Removed invalid ride durations.

## Exploratory Data Analysis

The notebook examines:

* Total rides by rider type
* Member vs. casual ride percentages
* Hourly bike rental patterns
* Day-of-week patterns
* Weekday vs. weekend usage


Seaborn and Matplotlib are used to visualize the patterns.


## Data Source

Capital Bikeshare System Data:

[https://capitalbikeshare.com/system-data](https://capitalbikeshare.com/system-data)

## Summary

This project demonstrates how Python data analysis and visualization can be used to identify behavioral patterns in bike-sharing data and compare the usage characteristics of member and casual riders.

For a student GitHub project, this level of README is sufficient; after you run the analysis, 

**Key Findings**
- The dataset was audited for missing values and duplicates, calculating both "Missing_Count" and "Missing_Percent" using sum(), isnull(), len(), and round(). An if statement was used to check for the presence of the ride_id column and print the total count of duplicate ride IDs found.

- Ride duration was calculated in minutes along with time components including start, end, duration, hour, day of the week, month, and date.
- The dataset was filtered to retain only ride durations between 0 and 1,440 minutes, outputting the row count before and after cleaning.

- A bar graph of total rides revealed that members accounted for 69.9% of rentals while casual riders made up 30.1%.
- Analysis of member versus casual ride counts showed that casual ride volume was twice as large as member ride volume.
- A comparison of overall rider percentages indicated that the casual rider segment was 40% larger than the member segment.
- Hourly rental patterns showed overall ride volume plotted against time of day, with casual rider usage reaching its peak between 7:00 AM and 8:00 AM.
- Analysis of rental timing demonstrated higher total ride volume on weekends compared to weekdays.
