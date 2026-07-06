US Accidents Exploratory Data Analysis

Overview

This project explores the US Accidents dataset from Kaggle — a countrywide car accident dataset covering 49 US states, with data collected from February 2016 to March 2023. The goal is to uncover patterns in when, where, and under what conditions traffic accidents are most likely to occur, with the broader aim of informing accident prevention strategies.

Dataset


Source: Kaggle — US Accidents (2016–2023)
Size: ~7.7 million accident records, 46 columns
Contents: Location (lat/lng, city, state), timestamp, weather conditions, road features (traffic signals, junctions, etc.), and severity


Approach


Data Loading & Cleaning — Loaded the dataset in chunks to handle its large size (~3 GB), inspected column types, and quantified missing data across all fields.
Missing Value Analysis — Visualized the percentage of missing values per column to identify which features are reliable enough to analyze.
Exploratory Analysis — Investigated key dimensions of the data:

City-level distribution of accidents
Time-based patterns (hour of day, day of week, month)
Geospatial distribution using scatter plots and interactive heatmaps (via Folium)


steps to follow : 
<br>
🔍 Select a large real-world dataset from Kaggle
<br>
⚒ Perform data preparation & cleaning using Pandas & Numpy
<br>
🔁 Perform exploratory analysis & visualization using Matplotlib & Seaborn
<br>
🙋‍♂️ Ask & answer questions about the data in a Jupyter notebook
<br>
📝 Summarize inferences & write a conclusion
<br>



Key Insights


📉 Accidents per city follow an exponential (long-tail) distribution — a small number of cities account for a disproportionate share of accidents, while most cities report very few.
<br>
🏙️ Fewer than 5% of cities report over 1,000 accidents/year, meaning the vast majority of locations see relatively low accident volume.
<br>
❓ Over 1,200 cities have exactly one recorded accident — a data quality/coverage anomaly worth further investigation (possible reporting gaps or geocoding issues).
<br>
⏰ Rush hour effect: Accidents peak sharply between 7–9 AM, consistent with morning commute traffic.
<br>
📅 Weekends behave differently: On Sundays, the peak shifts to 12 PM–2 PM, reflecting a different traffic pattern than weekday commuting.
<br>
🗺️ Geospatial clustering: Accident density heatmaps reveal strong clustering around major metropolitan areas and highway corridors.


