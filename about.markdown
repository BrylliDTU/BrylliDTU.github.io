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

Please keep in mynd that the analysis here below was built on data from 2000 to 2019.

# Stadiums

First, we'll explore the stadiums and fan engagement for each team to provide a glimpse into the unique atmosphere of each home stadium. Additionally, we'll delve into the weather conditions of the games to cater to the preferences of each new fan.

## Geographical visualizations

<figure>
  <iframe src="/asset/map1.html" width="800" height="600"></iframe>
  <figcaption>Geographical map for NFL stadiums</figcaption>
</figure>

In the map above, the locations of the stadium for each team is displayed. As a new, european fan, locations of the stadiums for each team may not matter as much to you as you don't live in the USA, but knowing in what state the stadium is in might give you some ideas on how the gameday spirit would look like and how many people would show - if you decide to take a quick trip to see a game.

## Stadium Attendance

<figure>
  <img src="/asset/images/total_attend_per_stadium.png" alt="Total Attendance">
  <figcaption>Total attendance per NFL stadium.</figcaption>
</figure>

Let's take a look at the total attendance for each stadium in the years 2000-2019 so you can get a feeling of how many attend each stadium. Let's note that the NYG/NYJ is used for two teams, which explains the high total attendance. This graph will give you an insight into which stadiums have drawn the largest crowds and how attendance can vary significantly from one venue to another.

Key points to consider:
* Dual-Use Stadium: The stadium shared by the New York Giants and New York Jets, referred to in our data as NYG/NYJ, consistently shows higher attendance figures. This is because it serves as the home field for two teams, essentially doubling its exposure to fans throughout the NFL season.
* Stadium Capacity: Attendance figures are influenced by the capacity of each stadium. Larger stadiums can accommodate more fans, and this is often reflected in higher total attendance numbers. For example, venues like the LAC stadium, the home of the Los Angeles Chargers, has much less capacity compared to other stadiums, which reflects as a low total attendance in our graph.

## Weather at the stadiums

<figure>
  <iframe src="/asset/average_weather_per_stadium.html" width="800" height="600"></iframe>
  <figcaption>Average weather per NFL stadium</figcaption>
</figure>

As a fan, whether you're watching a game from your living room or you're cheering in the stands, knowing the weather can help you prepare for the game. For stadium-goers, understanding typical weather patterns can influence everything from apparel choices to tailgating plans. Meanwhile, at-home viewers will find that commentators often discuss weather impacts on the game’s strategy, adding an extra layer of depth to broadcasts.Think of it like this, do you want to travel to go see your new team play a game on their home stadium? Then perhaps the average weather conditions influence you in where you would travel. The graph above shows us the average wind speed as well as the average temperature for each home team stadium. 

# Teams

Next, we'll focus on individual teams by examining their recent success over the past few years and analyzing the scores of each team. This comprehensive approach will help you select your favorite team, taking into account all these factors.

## Weekly Team Attendance

For the first visualization for the individual teams themselves, we can look at the average weekly attendance for each team. The weekly attendance can give you a better idea on how popular the teams really are. Again, we want to emphasize the fact that the team's stadiums have different capacities.

<figure>
  <img src="/asset/images/average_weekly_attend_team.png" alt="ave_attend">
  <figcaption>Average weekly attendance for each team.</figcaption>
</figure>

From this bar chart, we see that the team that has the highest average weekly attendance for their games are the Redskins. That could be due to high capacity of the stadium and popularity. It is interesting to see that the Los Angeles Rams have such high average weekly attendance, while in the total attendance they were pretty low. This might be because of a loyal fanbase that comes to watch them regularly.

## Geographical Historical Team's Success

<figure>
  <iframe src="/asset/home_win_rate_map.html" width="800" height="600"></iframe>
  <figcaption>Win rates for each home team map</figcaption>
</figure>

In this interactive graph, we've displayed the home win rates for each NFL team in their own stadiums. This visualization can capture the spirit of the game and the  edge that teams may gain in their home stadium. As you explore and hover over this graph, you'll see how different teams leverage their home field advantage, which can vary from one team to another based on factors like crowd support, familiar playing conditions, and even weather. Whether you’re a seasoned fan or new to the NFL, this graph offers a valuable insight into the advantage of playing at home. 

## Historcal Win rate for each team

The next graph  illustrates the distribution of the home win rate by stadiums to gain another angle. From both of the graphs, we see that the team that has the highest percentage of home wins at their home stadium are the New England Patriots which are located in Boston. While the New Englan Patriots are successfully maintaining their high home winning rate, the Cleveland Browns have the lowest home win rate percentage.

<figure>
  <img src="/asset/images/home_win_rate.png" alt="home_win_rate">
  <figcaption>Win rates for each home team.</figcaption>
</figure>

## First wins

The graph below is an interactive graph made with plotly express to show each teams first win, if you hover over the data-points, you can see the team abbrivation and the date of their first win. This kind of graph can give important information about historical success.

<figure>
  <iframe src="/asset/first_wins.html" width="800" height="600"></iframe>
  <figcaption>First wins for each team</figcaption>
</figure>

For the first win graph above, we have displayed information regarding the first win of each team since the year 2000. Pretty much all of the teams had their first fin at a similar time, except for the Los Angeles Chargers and the Houston Texans. This information is to understand the team's historical success better.

## More data on wins and scores

<figure>
  <iframe src="/asset/wins_per_season.html" width="800" height="600"></iframe>
  <figcaption>Interactive graph for wins per season</figcaption>
</figure>

Here below you can see average wins per season for each team.

<figure>
  <iframe src="/asset/average_wins_per_team.html" width="800" height="600"></iframe>
  <figcaption>Average wins per season for each teamn</figcaption>
</figure>

Here below you can see the high scoring percentage for teams that score over 50 points.

<figure>
  <img src="/asset/images/high_scoring_games.png" alt="high_score">
  <figcaption>Percentage of teams that have had games where they score over 50 points.</figcaption>
</figure>

# Conlusions and Recommendations

As you embark on your journey into the exciting world of American football, armed with insights into team performance, stadium atmospheres, and fan engagement, you're now better equipped to select the perfect NFL team to support. From analyzing historical data to exploring interactive visualizations, our guide has provided valuable insights to help you make an informed decision.

Explore our recommendations below, or simply choose your own team that you particularly like, and enjoy your journey to becoming a devoted fan of the NFL.


## New England Patriots (NE)
If you're seeking to support a well-established franchise that has consistently proven successful and victorious over the years, we recommend rooting for the New England Patriots (NE). They boast the highest winning percentage at their home stadium, lead in average wins among all NFL teams, and have clinched multiple Super Bowl victories. The Patriots also excel in high-scoring games per season, promising an exhilarating viewing experience. Additionally, their stadium is conveniently located just outside of Boston, Massachusetts, a popular tourist destination.

## New Orleans Saints (NO)
If action-packed games with high scores are your preference, then the New Orleans Saints (NO) are the team for you. They lead the league in high-scoring games and are among the top-performing teams, consistently ranking in the upper quartile for average wins per season.

## Los Angeles Rams (LA)
For fans who enjoy good weather, vibrant cities, and iconic locations for game days, we recommend supporting the LA Rams (LA). Situated in Los Angeles, with its array of famous landmarks and favorable year-round weather, the Rams offer a unique game day experience. Despite their favorable location, it's worth noting that the Rams rank among the lower-performing teams in the league, so consider your preferences carefully before making them your NFL team of choice.


# External sources 

Here you can find the source for the [regular season][nflSchedule]

Here you can find the source for the dataset: [NFL game attendance][gameAttend]

Here you can find the source for the dataset: [NFL games][games]

Here you can find the source for the dataset: [NFL Stadium Coordinates][nflStad]

[nflSchedule]: https://operations.nfl.com/gameday/nfl-schedule/creating-the-nfl-schedule/#:~:text=THE%20ANATOMY%20OF%20THE%20NFL%20SCHEDULE&text=Every%20team%20will%20play%2017,games%20in%20the%202023%20season
[gameAttend]: https://www.kaggle.com/datasets/sujaykapadnis/nfl-stadium-attendance-dataset

[games]: https://github.com/nflverse/nfldata/blob/master/data/games.csv

[nflStad]: https://www.kaggle.com/datasets/rusiano/nfl-stadiums





