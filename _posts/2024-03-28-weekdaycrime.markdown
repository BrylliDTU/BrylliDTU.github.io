---
layout: post
title:  "Weekday crime analytics for SF"
date:   2024-03-28 22:08:33 +0100
categories: jekyll update
---
Here you can see the weekday counts of each of the focus crimes.


![crime](/asset/images/weekdaycount.png)

Here is how we calculated the weekday values.

{% highlight ruby %}
# Weekday plot
focus_crimes_data["Weekday"] = crime_data["Date"].dt.day_name()
weekday_counts_focus = focus_crimes_data.groupby(['Category', 'Weekday']).size().reset_index(name='Count')

# Sorting the weekdays to be in the correct time series
weekdays_ordered = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
weekday_counts_focus["Weekday"] = pd.Categorical(weekday_counts_focus["Weekday"], categories=weekdays_ordered, ordered=True)
weekday_counts_focus = weekday_counts_focus.sort_values(by=["Weekday", "Category"])
{% endhighlight %}

Check out the where we got the dataset for the crimes at [Dataset Crimes][crime-data].

[crime-data]: https://jekyllrb.com/docs/home

