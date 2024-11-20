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

This is the write-up of bar chart 1.

## Bar Chart 2: Average Square Footage by Building Status

<vegachart schema-url="{{ site.baseurl }}/assets/json/building_inventory_bar2.json" style="width: 100%"></vegachart>

This is the write-up of bar chart 2.

## Search The Data & Methods

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jingyih1101/jingyih1101.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>
