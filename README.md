# PyBer_Analysis

## Overview of Analysis

The purpose of this analysis is to first create a summary DataFrame by combining data from two seperate CSV files. The summary DataFrame will collect the following data:
- Total Rides
- Total Drivers
- Total Fares
- Average Fares per Ride
- Average Fares per Driver

We will be using these paramaters to analyze how PyBer data varies by city type. 

Second, we will be using the summary DataFrame to create a multi line chart to visualize. 

## Results

### The Summary DataFrame

In order to get the picture below, the groupby() function is used to combine the data from the two seperate CSV's. To find the average fares per ride and average fares per driver, total fares was divided by total rides and total drivers, respectively. Additional formatting is applied using a format map to display the data correctly. 

![Pic1](https://github.com/cbrooks718/PyBer_Analysis/blob/main/analysis/Data_Frame_Summary.png)

From this table we can see that:
- Rural cities have the lowest total fares but have the highest average fares
- Urban cities have the highest total fares but have the lowest average fares
- Suburban cities as a result score right in the middle for both total and average fares

### The visualization

In order to generate this line graph, the groupby() function is used again in order to rearrange the data into a pivot table. After the data is placed in a pivot table, the resample() function is used in order to get the total fares for each week so that we can create the visualization below.

![Pic2](https://github.com/cbrooks718/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

A couple of findings that can be observed are:
- Total fares for all city types peaks somewhere toward the end of February
- There are no distinct patterns for any of the 3 city types; therefore, further analysis or more data is needed to identify trends over time

## Summary/Reccomendations

1. One reason for why total fares for urban cities is higher than the rest is due to a higher population density. Given that the average fare is low and there are more total rides, it's safe to assume that much shorter trips are being conducted at a higher rate. Conversely, the low population density of rural areas explains why the average fare is higher given that there are much less trips and trips are likely longer. Further analysis is needed to see how drivers compensated depending on where they are driving (city type). 

2. Given that total drivers is greater than total rides in urban areas, it could be safe to question if drivers need to be more evenly dispersed in order to cover more suburban/rural areas. This could indicate that some drivers in urban areas are not being compensated enough which could lead to high employee turnover. 

3. As stated earlier, fares seemed to have peaked sometime in the latter half in the month of Februrary. If an advertising/marketing campaign were to be conducted, that would be the best time to promote PyBer and spend advertising $. 
