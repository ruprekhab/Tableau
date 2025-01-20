# Citibike System Data Analysis: September 2024 - December 2024

## Overview
The project aims to analyze Citibike usage trends from September to December 2024. The study involves analyzing the following two phenomenon:
   * Identifying usage patterns as seasons change.
   * Analyzing trip patterns and user behavior.

## Data Source 
Citibike System Data (September 2024 - December 2024) as published by Citibike.

## Files and Folders:
   * clean_data: The folder contains the clean csv file used for analysis in this project
   * Resources: Contains the raw data files downloaded from Citibike 
   * citibike.ipynb: A Jupyter notebook containing the script for data cleaning and preprocessing, including handling missing values, and data transformation to prepare the Citi Bike dataset for analysis.

## Data Cleaning Process
   * Data Import: Monthly raw data was read into individual DataFrames.
   * Concatenation: These DataFrames were combined into a single dataset.
   * started_at and ended_at columns were converted to datetime format.
   * Rows with missing values were removed.
   * Data was filtered to include only records between September 1, 2024, and December 31, 2024.
   * Export: The cleaned dataset was exported to CSV for further analysis.
## Tableau Visualizations
### Interactivity: 
Users can hover over the map, bars, or markers to view corresponding values. A dropdown filter in the maps allow month-by-month exploration.
### Dynamic Maps:
**Description:**
   * Two maps were created to visualize start locations and end locations separately.
   * Marker size increases and color darkens based on location popularity.
   * A dropdown filter allows month-by-month exploration.
   * Maps are segmented by zip codes and a layer of per capital income by zip code was created
##### Insights:

   * The most popular stations for starting and ending trips are Hoboken Terminal and Hudson Pl and Grove St Path.
These locations correspond to areas with high per capita income.

The following map shows the markers for all the start stations:
![image alt](https://github.com/ruprekhab/Tableau/blob/709ce6e2d63e1b650bc8eeb099d1d55d5d8615a9/Images/Map_%20Bike%20Start%20Stations.png)

The following map shows the markers for all the end stations:
![image alt](https://github.com/ruprekhab/Tableau/blob/deb6ebff73fc73b125def03a505f46cdf704369b/Images/Map_%20Bike%20End%20Stations.png)
## Analysis:

### Monthly Trends and User Insights: 
The Month filter on top of the dashboard lets select one or multiple months to view dynamic results.
##### Monthly Trends:
The monthly trends in rides, distance covered, and ride duration reveal notable patterns:
   * Distance Covered: October recorded the highest distance covered, while December had the lowest.
   * Average Ride Duration: Members maintained a consistent average ride duration of under 10 minutes across all months. In contrast, casual riders exceeded a 10-minute average ride duration in all months except December.
   * Total Rides: Among members, the highest total rides occurred in October, with the lowest in December. Casual riders experienced peak ridership between September and October, with a sharp decline in December.
     

The observed patterns are likely due to seasonal changes and rider behaviour:
   * October Peak & December Decline: Favourable weather in October boosts cycling, while cold weather and holidays in December reduce ridership.
   * Casual Riders: Longer rides reflect leisure use, with peak ridership during warmer months (September–October).
   * Members: Consistent short rides suggest utilitarian use, though colder months also impact their activity.
   * December Dip: Holidays and reduced outdoor activity further lower ridership and distance covered.

  ![image alt](https://github.com/ruprekhab/Tableau/blob/deb6ebff73fc73b125def03a505f46cdf704369b/Images/Monthly%20Trends%20%26%20User%20Insights.png)
   


### User Analysis:
The analysis of bike usage and ridership trends reveals key patterns:
   * Growth Trends: Ridership grew the most in October (+2.38%) but declined sharply in December (-37.85%).
   * Top stations to start and end a trip are Hoboken Terminal and Hudson Pl and Grove St PATH
**Day-wise Insights:**
   * Saturdays recorded the highest average distance covered, followed by Sundays, while Mondays had the lowest.
   * Peak hours for weekdays are at 8 AM and 5–6 PM, while weekends peak at 12 PM.

The observed patterns can be attributed to the following factors:
   * Top Stations: Hoboken Terminal, Hudson Pl, and Grove St PATH are likely major commuting hubs, as these areas also correspond to zip codes with high per capita income, a population with greater commuting needs.
   * Peak Hours: Weekday peaks at 8 AM and 5–6 PM align with commuting times, while the 12 PM weekend peak reflects leisure activities during midday.
   * Weekly Average Distance: Saturdays and Sundays see higher distances as riders engage in leisure or recreational activities, while Mondays have the lowest distance due to reduced non-essential trips.
   * Growth Trends: Ridership growth in September could result from favourable weather and the end of summer vacations. The sharp decline in December is likely due to colder weather and holiday season disruptions, reducing travel demand.

     ![image alt](https://github.com/ruprekhab/Tableau/blob/deb6ebff73fc73b125def03a505f46cdf704369b/Images/Bike%20User%20Analysis.png)








