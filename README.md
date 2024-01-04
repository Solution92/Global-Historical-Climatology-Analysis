# Global-Historical-Climatology-Analysis
Global Historical Climatology Network-Monthly (GHCN-M)

### Project Overview

The Global Historical Climatology Network (GHCN) is an integrated database of climate summaries from land surface stations across the globe. This data set contains gridded mean temperature anomalies, or departures from a reference value or long-term average, from the Global Historical Climatology Network-Monthly (GHCN-M) version 3.2.1 temperature data set. The gridded anomalies were produced from GHCN-M bias-corrected data. Each month of data consists of 2,592 gridded data points produced on a 5° by 5° basis for the entire globe (72 longitude by 36 latitude grid boxes).
•	Frequency: Monthly
•	Period: 1880 to 2016

Gridded data for every month from January 1880 to the most recent month is available. The data are temperature anomalies in degrees Celsius. Each gridded value was multiplied by 100 and written to the file as an integer. Missing values are represented by the value -9999.
The data are formatted by year, month, latitude, and longitude. There are 72 longitude grid values per line -- each grid is labeled as a concatenation of "long", "w" or "e", then the degree. The latitude is captured in the "lat" field where the value indicates the lower bound of a grid cell (e.g. 85 indicates 85-90N whereas -90 indicates 85-90S). Longitude values are written from 180°W to 180°E, and latitude values from 90°N to 90°S.
This dataset permits the quantification of changes in the mean monthly temperature and precipitation for the earth's surface. Changes in the observing system itself have been carefully removed to allow for the true climate variability at the earth's surface to be represented in the data.

### Objectives

This granular dataset permits extensive historical analysis of the earth’s climate to answer questions about climate change:

- Do Spatial and Temporal Climate Change Analysis
- Conduct a Temporal Variation (Monthly Climate Change) Analysis
- What is the Longitudinal Segmentation of Climate Behavior?
- What are the Potential Climate (Yearly) Trends?

### Tools Used

- **MS Excel** is Used For Data Cleaning and Transformation.
- **Tableau** is used for Analysis and Creating Reports.

### Data Source

You can download the dataset [here](https://www.kaggle.com/datasets/noaa/global-historical-climatology-network)

### Data Cleaning and Preparation

There was not much cleaning in the dataset as it was stated that Missing values are represented by the value -9999.

![Climate Data](https://github.com/Solution92/Global-Historical-Climatology-Analysis/assets/144762124/bfbc16e7-54ca-44d6-abe2-43e1cd1a61ab)

### Data Analysis

To enhance the analysis, I did the average of all longitude East and West in Tableau.
~~~
AVG([lon 10 15E]+[lon 10 15W]+[lon 100 105E]+[lon 100 105W]+[lon 105 110E]+[lon 105 110W]+[lon 105 110E]+[lon 105 110W]+[lon 110 115E]+[lon 110 115W]+[lon 115 120E]+[lon 115 120W]+[lon 120 125E]+[lon 120 125W]+[lon 125 130E]+[lon 125 130W]+[lon 130 135E]+[lon 130 135W]+[lon 135 140E]+[lon 135 140W]+[lon 140 145E]+[lon 140 145W]+[lon 15 20E]+[lon 15 20W]+[lon 150 155E]+[lon 150 155W]+[lon 155 160E]+[lon 155 160W]+[lon 160 165E]+[lon 160 165W]+[lon 165 170E]+[lon 165 170W]+[lon 170 175E]+[lon 170 175W]+[lon 175 180E]+[lon 175 180W]+[lon 20 25E]+[lon 20 25W]+[lon 25 30E]+[lon 25 30W]+[lon 30 35E]+[lon 30 35W]+[lon 35 40E]+[lon 35 40W]+[lon 40 45E]+[lon 40 45W]+[lon 45 50E]+[lon 45 50W]+[lon 5 10E]+[lon 5 10W]+[lon 50 55E]+[lon 50 55W]+[lon 55 60E]+[lon 55 60W]+[lon 60 65E]+[lon 60 65W]+[lon 65 70E]+[lon 65 70W]+[lon 70 75E]+[lon 70 75W]+[lon 75 80E]+[lon 75 80W]+[lon 80 85E]+[lon 80 85W]+[lon 85 90E]+[lon 85 90W]+[lon 90 95E]+[lon 90 95W]+[lon 95 100E]+[lon 95 100W])
~~~

### Dashboards

![CLimate chge 1](https://github.com/Solution92/Global-Historical-Climatology-Analysis/assets/144762124/f4c316ac-e287-48b0-a884-54b043701fdd)


[Here is the link to the Dashboard on the tableau public](https://public.tableau.com/app/profile/emmanuel.ashiedu/viz/GlobalHistoricalClimatologyAnalysis/Dashboard1?publish=yes)


### Result and Findings

- Spatial and Temporal Climate Change

![Spacial Clmt chge](https://github.com/Solution92/Global-Historical-Climatology-Analysis/assets/144762124/f53c5ac5-da43-4b1b-a4d4-622843ef2160)

The bar chart represents the spatial and temporal coverage of climate change, categorized by latitude. The chart shows the average longitude (calculated) on the x-axis and different latitude ranges on the y-axis. The bars represent values from +699,930 to -241,575. The color intensity appears to correlate with these values; darker shades indicate higher positive values 1.

- Temporal Variation (Monthly Climate Change) Analysis

![Monthly Climate](https://github.com/Solution92/Global-Historical-Climatology-Analysis/assets/144762124/c5763475-5228-434a-ba2b-5d376f3085d4)

The line graph above depicts a trend where the value decreases over time, reaching its lowest point around the 6th month, and then slightly increases towards the 13th month.
The x-axis represents months, ranging from 0 to 13. The y-axis represents value, with markers at intervals of 20K from 0K to -240K. There are two sets of data represented on the graph:
One set of data points is plotted along the top of the graph with values ranging from approximately -3,145 to -3,485. These points are labeled with their exact values.
Another set of data points is plotted along the bottom of the graph with values ranging from approximately -221,273 to -227,955. These points are also labeled with their exact values.
A blue line connects each point in both sets of data showing a downward trend for both until around month six where it begins to rise slightly.

- Longitude Segmentation Analysis

![Longitude Seg Ana](https://github.com/Solution92/Global-Historical-Climatology-Analysis/assets/144762124/a5ae2d15-7a96-476e-9b8a-73e5d59c4c7c)

One data point is positioned at approximately 0 on the x-axis and 59,223 on the y-axis. Another data point is located at about -231,406 on the x-axis and -240k on the y-axis

- Potential Climate (Yearly) Trends

![Yearly Chge](https://github.com/Solution92/Global-Historical-Climatology-Analysis/assets/144762124/29ef2d5b-0bfc-4319-b949-3e58d5dbe4ff)

There is a trend of increasing negative values over the years, indicating a decline in the AQG/AVG Longitude. This could potentially be related to climate change or other environmental factors. My recommendation would be to investigate the underlying causes of this trend and implement strategies to mitigate negative impacts.

### Recommendation

Based on the analysis of the Global Historical Climatology data, it is crucial to prioritize investigations into the factors contributing to the declining AQG/AVG Longitude, especially the increasing negative values over the years. This trend suggests potential adverse effects on the climate, necessitating a comprehensive study of environmental factors influencing this shift.

Implementing proactive strategies and policies to address and mitigate these negative impacts is essential for long-term climate resilience and sustainability. Further research should focus on identifying specific drivers behind the observed trends to inform targeted interventions and adaptation measures.




















