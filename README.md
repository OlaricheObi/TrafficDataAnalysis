# Tennesse Department of Transportation (TDOT) Traffic Data Analysis
## Table of Contents
* [Motivation](#Motivation)
* [Technologies](#Technologies)
* [Problems & Hurdles](#problems--hurdles)
  * [Getting the Data](#getting-the-Data)
  * [Data Normalization Trouble](#normalizing-the-data)
  * [Hurdles](#Hurdles)
## Motivation
#### Growing up a Nashville/Middle TN native I have always thought it normal that everyone have a car as their main means of transportation. Assuming this southern lifestyle as the basis, I had never questioned the multi-vehicle households nor the lack of a cohesive public transit system for our Greater Nashville community. As I have matured so has Nashville and its surrounding cities. Now more than ever, more people are flooding into the Middle TN community, with Nashville serving as its hub. As I live in Murfreesboro, a large suburb, nearing 200,000 people; I have found the commute has become a most unenjoyable experience taking anywhere between 35 minutes as expected to over an hour, depending on the traffic.

#### It was not until I left southern life behind, and attended university in the city of Chicago that I had my eyes opened to the facility, flexibility, and ease of a unified public transit system. This system, the CTA (Chicago Transit Authority), includes the elevated train system, the bus system, and even individual, specialized shuttles. The CTA resembles that of a water system. If we imagine the ‘Loop’, the central hub where all the trains come together as the river's source, then the routes of the elevated train (‘L’ train), branching outwards in all directions, are branches of the river. The surrounding bus routes are then represented as smaller estuaries of the river’s branches. The ‘L’ train routes provides a web-like network between downtown Chicago, the surrounding North, West, Southern Chicago neighborhoods, and Cook County suburbs; and wherever the ‘L’ train stops, the bus system picks up.

#### The structure of this transit system functions best, as most transit systems do for its ability to identify areas of heavy traffic and alleviate them by putting introducing bus/train routes in those areas.


#### My project therefore attempts to provide a dashboard tool that examines Greater Middle TN traffic commuter pattern data as collected by the Tennessee Department of Transportation (TDOT). With this tool, I hope to offer a helpful step in the direction of progress for Middle TN transit infrastructure as it continues to grow.

## Technologies
#### For the bulk of the project I use Python 3 within a Jupyter Notebook. Some of the data was extracted from the TDOT Transportation Management System found here at https://tdot.public.ms2soft.com/tcds/tsearch.asp?loc=Tdot&mod=TCDS as CSV files and imported into Jupyter for data cleaning.. The other portion of the data was pulled from the same site via web-scraping.

#### For the organization of the cleaned data, Power  BI was used to create a dashboard tool.

## Problems & Hurdles
### Getting the Data
#### As previously stated, the data was obtained one of two ways: 
#### The first and least labor intensive was going to the TDOT TMS page and searching by county to download its CSV file containg what I had deemed the key contributors for analysis that would aid in my analysis to convince the listener that the transit system necessary.. Essentially any point that could help echo my final sentiment. The CSVs conatined data on the traffic station location IDs, their average annual daily traffic (AADT) totals, and their latitudes and longitudes. Three of the most important data points. 
#### The second and more labor intensive included a web-scraping of the same sight to determine the change in AADT of each traffic station point over time. I thought this necessary to show how the counties have grown over time and how their continued growth would benefit from the implentation of transit system. This web-scrape was difficult as it required scraping a web-site that was coded with javascript.
### Normalizing the Data
#### One thing that might become evident in examining the created dashboard tool is that the analysis of the AADT by county is a summation of a particular traffic station's AADT. This means that certain counties, like Davidson and Rutherford, may perhaps have a higher sum AADT than other counties because they have more traffic stations collecting data. I realized a bit to late that this might skew the analysis and therefore the data is left unnormalized. However, I believe that this doesn't greatly alter what is the reality of the high volumes of traffic that those counties do see.
### Hurdles
#### Although I collected data on the change in AADT over time and was able to plot this on a line graph, I was unable to get Power BI's ArcGIS map feature to smoothly run to show a time lapse of the growing volume of traffic over time.

## Link to Dashboard
