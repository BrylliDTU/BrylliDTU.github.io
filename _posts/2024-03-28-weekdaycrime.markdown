---
layout: post
title:  "Weekday crime analytics for SF"
date:   2024-03-28 22:08:33 +0100
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
# Weekday plot
focus_crimes_data["Weekday"] = crime_data["Date"].dt.day_name()
weekday_counts_focus = focus_crimes_data.groupby(['Category', 'Weekday']).size().reset_index(name='Count')

# Sorting the weekdays to be in the correct time series
weekdays_ordered = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
weekday_counts_focus["Weekday"] = pd.Categorical(weekday_counts_focus["Weekday"], categories=weekdays_ordered, ordered=True)
weekday_counts_focus = weekday_counts_focus.sort_values(by=["Weekday", "Category"])
{% endhighlight %}

Check out the where we got the dataset for the crimes at [Dataset Crimes][jekyll-docs].
for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[crime-data]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
