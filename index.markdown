---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Assignment 2 - Social Data | Group 63
---
# Group Information
* Brynjar Karl Ævarsson - s232736@dtu.dk
* Birkir Fanndal Sturluson - s2327XX@dtu.dk
* Védís Sigríður Ingvarsdóttir - s2327XX@dtu.dk

# Introduction

Over the last couple of years, the city of San Francisco has been gathering data on crimes and illegal activity in the Bay Area. This data has been made available to the public and has caught the interest of many, including us. 
We, Birkir Fanndal, Brynjar Karl and Védís Sigríður, want to analyze this massive dataset by visualizing the data with graphs and plots to figure out some trends within the many categories of crime committed in San Francisco.
In this short story we will be focusing on the crime of **prostitution**, where we will analyze the development and the trends of prostitution in San Francisco. We will utilize graphs and maps to identify and analyze the trends over the last couple of years.

# Information about the Dataset

The dataset that we will be using for this project is called **Police Department Incident Reports from 2003 to May 2018**. It includes 2.129.525 datapoints and 37 crime categories. Here you can access the dataset that will be used for this project: [Dataset Crimes][crime-data].

[crime-data]: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry/about_data


# Time series

Here we will show time series

<figure>
  <img src="/asset/images/timeseries2.png" alt="Time Series">
  <figcaption>Times series for weekday, month, hour of day and year.</figcaption>
</figure>

Observing the pattern of daily reported crimes, there's a noticeable trend where incidents gradually increase from Tuesday, peaking on Thursday, before declining again. Contrary to expectations that weekends might see the highest numbers, this midweek peak is quite intriguing. 

When examining monthly crime reports, variations are minimal across the year. However, a slight dip during the summer months might reflect the busier schedules of individuals, while a modest uptick in January could be attributed to increased feelings of depression during the winter months. 

Looking at the data on an hourly basis, reported crimes surge significantly from 8 pm to 1 am. This pattern aligns with expectations, considering the higher demand for prostitution during nighttime hours. 

It's noteworthy that reports of prostitution crimes have been on a decline from 2007 to 2017. This trend may be linked to enhanced police surveillance in areas known for high prostitution activity and reflects a broader shift towards deprioritizing prostitution as a criminal issue by law enforcement. 

# Map visualization

Here we will show heat map 

<figure>
  <iframe src="/asset/map.html" width="800" height="600"></iframe>
  <figcaption>Reported crimes shown on map fer each district</figcaption>
</figure>

The map below displays San Francisco's districts outlined by borders, with yellow dots marking each reported prostitution incident over the years. The districts reporting the highest incidents—Mission and Northern—are notable, with Central and Tenderloin also showing significant activity. These areas' higher population densities and proximity to the city's nightlife offer some context for the higher report rates. 

Capp Street in the Mission district, known for its association with sex work, has seen recent city efforts to deter such activities through physical barriers. 

# Interactive visualization in Bokeh

Here we show an interactive

<figure>
  <iframe src="/asset/Bokeh2.html" width="800" height="600"></iframe>
  <figcaption>Reported crimes for hour of day depending on districts</figcaption>
</figure>

The interactive visualization clearly indicates that the Mission district reports the highest number of prostitution-related crimes, likely influenced by the notorious Capp Street. Additionally, in densely populated districts like Central, Northern, and Tenderloin, there's a noticeable volume of reports, further emphasizing the correlation between nightlife proximity and crime reports. 

# External sources 

Here you can find the source for time series insights [Time Series Insights][time-series].

Here you can find the sources for the map insights [Capp street][capp-street] and [Barriers][barrier]

[time-series]: https://localnewsmatters.org/2023/08/17/sex-work-and-the-city-policing-prostitution-in-san-francisco-reflects-evolving-attitudes/
[capp-street]: https://www.sfgate.com/local/article/san-francisco-sex-workers-mission-17777619.php 
[barrier]: https://www.nbcbayarea.com/news/local/san-francisco-mission-barriers-address-sex-work/3320123/




