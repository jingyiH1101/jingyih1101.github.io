---
name: Homework 6
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/building_inventory_bar1.png
description: This is the homework 6 project created by Jingyi Huang that uses vega-lite and Altair for interactive visualizations.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Homework 6 Jekyll Webpage, Jingyi Huang, jingyi48

## Bar Chart 1: Building Count and Proportion by Agency Name and Status

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inventory_bar1.json" style="width: 100%"></vegachart>

**Description and Design Choices**

This plot visualizes the building count for various agencies, categorized by their building status ("In Use," "In Progress," "Abandon"). It helps users identify which agencies have a large proportion of "Abandon" status buildings, which allows for further analysis of underutilized properties. It also provides insights into the distribution of building usage across agencies.

For this visualization, I used a bar chart with the X-axis representing `Agency Name` and the Y-axis representing `Building Count`. Tooltips showing the proportion of different building statuses are included. For the color scheme, I used the default setting as it is clear enough to differentiate the categories.

**Data Transformation**

The data was grouped by `Agency Name` and `Building Status` to calculate the count of buildings for each combination. Additionally, a `Status Proportion` column was created to show the proportion of each status within each agency.

**Difference from Homework 5**

Although I am using the same dataset, my previous homework focused on plots using `Year Constructed`. In this assignment, I focused on Building Status instead. Thus, while the dataset remains the same, these two assignments explore completely different topics.

**Interactivity**

This plot includes two interactivities. First, the dropdown filter allows users to select a specific agency or view all agencies, enabling them to focus the analysis on a particular organization. Second, the legend selection enables users to toggle building statuses to compare or isolate specific statuses for better clarity and insight.

## Bar Chart 2: Average Square Footage by Building Status

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inventory_bar2.json" style="width: 100%"></vegachart>

**Description and Design Choices**

This plot visualizes the average square footage for buildings categorized by their building status. It allows users to identify which building statuses are associated with larger or smaller average square footage. It provides insight into how building usage correlates with size.

For this visualization, I used a horizontal bar chart with the Y-axis representing `Building Status` and the X-axis representing `Average Square Footage`. I used the default color scheme to represent building statuses (blue for "Abandon," orange for "In Progress," and red for "In Use"), as it is consistent with the first chart.

**Data Transformation**

The data was grouped by `Building Status` to calculate the mean square footage for each category. This aggregation provided the average square footage for buildings in different statuses.

## Search The Data & Methods

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jingyih1101/jingyih1101.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
