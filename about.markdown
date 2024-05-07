---
layout: default
title: NFL Fan Starter Guide
description: Embark on your journey into the exhilarating realm of American football with our comprehensive guide tailored for new fans seeking to navigate the dynamic world of the NFL!
permalink: /finalproject/
---
# Project Assignment B | Final Project 

# Group 36
* Brynjar Karl Ævarsson - s232736@dtu.dk
* Birkir Fanndal Sturluson - s232729@dtu.dk
* Védís Sigríður Ingvarsdóttir - s232719@dtu.dk

# Introduction

American football is the biggest sport in the United States of America, with the National Football League (NFL) being the big stage where 32 teams compete each season to win the much coveted Superbowl. The anatomy of the NFL can be quite confusing for those not familiar with how it works. The 32 teams are split into two conferences - the American Football Conference (AFC) and the National Football Conference (NFC). The 16 teams in each conference are split into 4 divisions; East, North, South and West divisions, with all divisions having 4 teams. Each regular season spans 18 weeks and each team plays 17 games over those weeks. Those 17 games consist of 6 games against divisional opponents, 4 games against teams from a division within its conference, 4 games against teams from a division in the other conference and 2 games against teams from the two remaining divisions in its conference. Then each team plays an additional game against a non-conference team that they are not scheduled to play.  

For you as a reader, all this information can be quite overwhelming for a new NFL viewer and when it comes to picking a team to support there are a lot of options to pick from. Some people have a favorite player and root for the team that said player plays for and some people root for their local team, or the team from their respective state or city. However, if you are an audience outside of the USA, you may not have such ties to any teams in the NFL and would therefore rather support a team that has been doing good over the last few years or maybe a team that has been successful in the past. We want to analyze the performance of all 32 teams for the last 20 seasons to potentially give a you, as new NFL-fan, an idea of what team to support.




# Stadiums

First, we'll explore the stadiums and fan engagement for each team to provide a glimpse into the unique atmosphere of each home stadium. Additionally, we'll delve into the weather conditions of the games to cater to the preferences of each new fan.

<figure>
  <iframe src="/asset/map1.html" width="800" height="600"></iframe>
  <figcaption>Reported crimes shown on map fer each district</figcaption>
</figure>

# Teams

Next, we'll focus on individual teams by examining their recent success over the past few years and analyzing the scores of each team. This comprehensive approach will help you select your favorite team, taking into account all these factors.


## Wins


## Score



# Conlusions and preferences



# Time series

Observing the pattern of daily reported crimes, there's a noticeable trend where incidents gradually increase from Tuesday, peaking on Thursday, before declining again. Contrary to expectations that weekends might see the highest numbers, this midweek peak is quite intriguing. The reason could be that other crimes are increasing during the weekend, which makes prostitution low priority to get arrests for on the weekends. 

When examining monthly crime reports, variations are minimal across the year. However, a slight dip during the summer months might reflect the busier schedules of individuals, while a modest uptick in January could be attributed to increased feelings of depression during the winter months. 

Looking at the data on an hourly basis, reported crimes surge significantly from 8 pm to 1 am. This pattern aligns with expectations, considering the higher demand for prostitution during nighttime hours. 

It's noteworthy that reports of prostitution crimes have been on a decline from 2007 to 2017. This trend may be linked to enhanced police surveillance in areas known for high prostitution activity and reflects a broader shift towards deprioritizing prostitution as a criminal issue by law enforcement according to this article: [Time Series Insights][time-series].

<figure>
  <img src="/asset/images/timeseries3.png" alt="Time Series">
  <figcaption>Times series for weekday, month, hour of day and year.</figcaption>
</figure>



# Map visualization

The map below displays San Francisco's districts outlined by borders, with yellow dots marking each reported prostitution incident over the years. The districts reporting the highest incidents are Mission and Northern, with Central and Tenderloin also showing significant activity. These areas' higher population densities and proximity to the city's nightlife offer some context for the higher report rates, see this article: [Capp street][capp-street].

Northern's’ Polk Street has been reported as a street associated with sex work and the area around it, which includes Larkin Street in the Tenderloin district. That could explain why Tenderloin also shows a significant amount of prostitution activity. See this article: [Polk Street][polk]

Capp Street in the Mission district, known for its association with sex work, has seen recent city efforts to deter such activities through physical barriers according to this article: [Barriers][barrier]. An overwhelming number of all prostitution related crimes in 2003 occurred in the area around Shotwell Street and Capp Street in the Mission district alone. Residents of Shotwell Street claim that the police patrol the area quite infrequently and that prostitution matters are simply low in priority for the police according to this article: [Mission 2003][M2003].

<figure>
  <iframe src="/asset/map2.html" width="800" height="600"></iframe>
  <figcaption>Reported crimes shown on map fer each district</figcaption>
</figure>



# Interactive visualization in Bokeh

The interactive visualization clearly indicates that the Mission district reports the highest number of prostitution-related crimes, likely influenced by the notorious Capp Street, which is known for alleged sex work, violence and crime. See the following article: [Capp Street alleged crimes][Cap2]

The Mission district is a densely populated district, which is likely a significant reason for the high number of prostitution crimes in the district. Looking at some of the other densely populated areas, such as Central district, Northern district, Southern district and Tenderloin district, we can see that they have a relatively higher number of prostitution crimes in comparison to some of the more sparsely populated areas, such as Ingleside and Bayview. It is also interesting that in the district of Taraval the peak of prostitution crimes is around noon. 

<figure>
  <iframe src="/asset/Bokeh3.html" width="800" height="600"></iframe>
  <figcaption>Reported crimes for hour of day depending on districts</figcaption>
</figure>


# External sources 

Here you can find the source for the [regular season][nflSchedule]

Here you can find the source for the dataset: [NFL game attendance][gameAttend]

Here you can find the source for the dataset: [NFL games][games]

Here you can find the source for the dataset: [NFL Stadium Coordinates][nflStad]

[nflSchedule]: https://operations.nfl.com/gameday/nfl-schedule/creating-the-nfl-schedule/#:~:text=THE%20ANATOMY%20OF%20THE%20NFL%20SCHEDULE&text=Every%20team%20will%20play%2017,games%20in%20the%202023%20season
[gameAttend]: https://www.kaggle.com/datasets/sujaykapadnis/nfl-stadium-attendance-dataset

[games]: https://github.com/nflverse/nfldata/blob/master/data/games.csv

[nflStad]: https://www.kaggle.com/datasets/rusiano/nfl-stadiums





