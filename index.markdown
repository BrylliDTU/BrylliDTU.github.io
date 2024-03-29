---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

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

[time-series]: https://localnewsmatters.org/2023/08/17/sex-work-and-the-city-policing-prostitution-in-san-francisco-reflects-evolving-attitudes/



figure {
  /* Add some space around the figure */
  margin: 20px 0;
  /* Center the content */
  text-align: center;
}

figcaption {
  /* Style for the caption text */
  margin-top: 10px;
  font-style: italic;
  color: #555;
}



Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Weekday count crimes 
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





# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
