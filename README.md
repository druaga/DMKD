# Analysing data from Uber for New York City.

## Introduction
New York City (NYC) is the most populous city in the United States. It is also the most
densely populated major city in the United States. Situated on one of the world's largest
natural harbors, New York City consists of five boroughs. The five boroughs: Brooklyn, Queens,
Manhattan, Bronx, and Staten Island { were consolidated into a single city in 1898.

This project was done as a part of my coursework for 'Data Mining & Knowledge Discovery'subject 
included in the second semester of my Master's Degree. This is not a very detailed work for the topic
but more of a data understanding phase.

The objective of this project is to understand the traffic in different boroughs of New York
City and to try and categorise the various zones within various boroughs as being: office
destinations, residential destination, popular brunch destination or party destination according
to it's popularity given the time-range and the day of the week.

I have used data generated by Uber, an online transportation network company. This data
is available at Kaggle under the heading: 'Uber Pickups in New York City', provided by user:
'FiveThirtyEight' who obtained the data from the NYC Taxi Limousine Commission (TLC)
by submitting a Freedom of Information Law request on July 20, 2015.

The directory downloaded contains data on over 4.5 million Uber pickups in New York City
from April to September 2014, and 14.3 million more Uber pickups from January to June 2015.
I have used R to extract knowledge and mine the dataset.

## Data
The dataset downloaded contains, roughly, four groups of files:
1. Uber trip data from 2014 (April - September), separated by month, with location infor-
mation (longitude - latitude values)
2. Uber trip data from 2015 (January - June), with less fine-grained location information
3. Non-Uber FHV (For-Hire Vehicle) trips. The trip information varies by company, but
can include day of trip, time of trip, pickup location, driver's for-hire license number, and
vehicle's for-hire license number.
4. Aggregate ride and vehicle statistics for all FHV companies (and, occasionally, for taxi
companies)

However this project used two groups of files that was generated by Uber:
* Uber trip data from 2014 (April - September)
* Uber trip data from 2015 (January - June)

### Uber trip data from 2014
There are six files of raw data on Uber pickups in New York City from April to September
2014 (uber-raw-data-xyz14.csv). The files are separated by month and each has the following
columns:
* Date/Time : The date and time of the Uber pickup
* Lat : The latitude of the Uber pickup
* Lon : The longitude of the Uber pickup
* Base : The TLC base company code affiliated with the Uber pickup

### Uber trip data from 2015
Also included is the file uber-raw-data-janjune-15.csv This file has the following columns:
* Dispatching base num : The TLC base company code of the base that dispatched the
Uber
* Pickup date : The date and time of the Uber pickup
* Affiliated base num : The TLC base company code affiliated with the Uber pickup
* locationID : The pickup location ID affiliated with the Uber pickup

### Data for NYC Zone lookup
For coarse-grained location information from the pickups in 2015, the file taxi-zone-lookup.csv
shows the taxi Zone (essentially, neighborhood) and Borough for each locationID contained in
the Uber trip data from 2015.

## Implementation, Evaluation and Results
Please consult the report 'SejalJ_UberData_Report for further details. 
