---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

# Introduction

Over the last couple of years, the city of San Francisco has been gathering data on crimes and illegal activity in the Bay Area. This data has been made available to the public and has caught the interest of many, including us. 
We, Birkir Fanndal, Brynjar Karl and Védís Sigríður, want to analyze this massive dataset by visualizing the data with graphs and plots to figure out some trends within the many categories of crime committed in San Francisco.
The Crimes we want to focus on are .........

Fill in text

# Information about the Dataset

The dataset that we will be using for this project is called **Police Department Incident Reports from 2003 to May 2018**. It includes 2.129.525 datapoints and 37 crime categories. Here you can access the dataset that will be used for this project: [Dataset Crimes][crime-data].

[crime-data]: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry/about_data




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
