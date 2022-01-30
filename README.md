# PyBer Ride Sharing Analysis
## Overview
The purpose of this paper is to analyse data from PyBer, a ride sharing company, in order to determine the rides, drivers and fares collected by city type, in order to determine business proposals that may benefit the company.
The analysis presented here was made using Python v. 3.7.6, Pandas Lybrary, Matplotlib and Jupyter Notebook interface.

## Results
After importing the csv files containing the information pertaining to the data per city and rides, which were provided by the company, the information was reviewed. All the data was readable, with no empty values, so both data sets were merged in a single data frame containing the city name, the time stamp for each ride, the fare collected on each ride, the ride id number, the driver count and the city type in which the ride was made.

![Merged data frame](https://user-images.githubusercontent.com/95982833/151723120-1c9d2ebb-0d3c-47ce-beb4-90251b58935e.png)

After merging all the data into a single data frame, code script was written, taking advantage of the groupby function in pandas, in order to determine the following parameters:

 - Total rides for each city type.
 - Total drivers for each city type.
 - The sum of all fares for each city type.
 - Average fare per ride for each city type.
 - Average fare per driver for each city type.

Then, all this information was summarized in the Data frame shown below.

![summary_df](https://user-images.githubusercontent.com/95982833/151723126-4da7b86e-7520-4be4-9980-042a254b9c23.png)

After the summary was made, all the rides from January to April 2019 were added, divided by week and plotted in the following chart.

![Pyber_fare_summary](https://user-images.githubusercontent.com/95982833/151723134-16d0148d-7a9d-4b4c-bf27-002b63fc00bb.png)

## Summary

As it can be noted in the analysis made, there is a significant difference in total rides, total drivers and total fares collected, when grouped by city type. As it is expected, urban cities have the most rides, drivers and fares collected, as the urban areas have more demand for ride sharing services.

However, the average fare per ride is greater in rural cities, then in suburban cities, and the cheapest are the urban cities. This difference may be explained because usually in rural areas the distances traveled are greater than in the suburbs or in urban areas. This also correlates with the average fare collected pare driver, being almost three times greater in rural cities than in urban cities.

When analysing the income by week per city type, from january to april 2019, it is clear that the income generated in rural cities, does not come in any way close to the income generated in the suburbs or in the urban cities, with an almost three-fold difference between the worst week in urban cities ($1661.68) and the best performing week in rural cities ($501.24).

Three recommendations can be made based on this analysis:
1. Rural cities may not be the best market for a ride-sharing service, taking into account that is the least profitable for the company, with a demand for rides of less than ten percent of the demand for rides in urban cities (125 rides in rural cities vs. 1,625 rides in urban cities). These results may be explained by the needs and baseline charachteristics of rural cities, in terms of population, population density and economic activities in each type of city.

2. The company may benefit from increasing it's presence in the suburbs, as there is almost five times more rides in these cities, but with an average fare per ride almost as expensive as a rural ride, and with an average fare per driver more than double the average fare for an urban ride per driver. This may be an incentive for the drivers to focus un subruban areas, as they can make a similar income with less rides ( 1.2 rides per driver in the subrubs).

3. Although urban cities represent the most profitable cities for the company, there is almost 50% more drivers than rides made, with the lowest fares per ride and per driver. Usually in urban cities the rides are shorter, and there are alternative means of transportation to the car. If the number of drivers were to decrease, increasing the cost per ride, this may cause the riders to think of alternative means of transportation, so no changes should be made in this type of cities. As it is now, this remains the most profitable market, making on its own, more than the suburban and rural cities combined.
