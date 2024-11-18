---
name: Homework 6
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/cars.png
description: This is a homework 6 that uses vega-lite & altair for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework 6 Plots

Data comes from this [link](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv).

This is a homework assignment for [IS 455 - Data Visualization](https://uiuc-ischool-dataviz.github.io/is445_bcubcg_fall2024/).



### This is a plot of bigfoot observations in the United States

<vegachart schema-url="{{ site.baseurl }}/assets/json/bigfoot_interaction.json" style="width: 100%"></vegachart>


#### First Plot Write-up

The first plot on the left illustrates the number of Bigfoot observations. Bigfoot is a large, hairy creature commonly referred to as Sasquatch. I encoded this plot using mark_line with a navy color to show the trend of observations reported to the Bigfoot Field Researchers Organization (BFRO). Based on the visualization, most observations occurred between the late 1990s and early 2010s. To address massive file sizes and the presence of missing values, I sampled the data to reduce file size while retaining the necessary information. This plot does not overlap with Homework 5, as I used a different encoder and dataset for Homework 6.

#### Second Plot Write-up

The second plot illustrates the relationship between the median temperature and dew point recorded during the observations, along with the amount of cloud cover. I encoded this plot using mark_circle to create a scatterplot, which reveals that temperature and dew points are positively correlated — as temperature increases, the dew point also increases. Additionally, the highest cloud cover values were observed when the temperature and dew point were reported at approximately a 1:1 ratio (e.g., 40°F temperature to 40°F dew point). For better visual interpretation, I used the 'sinebow' color scheme to represent cloud cover.

The data was transformed for the same reasons as the first plot. The transformed dataset contains five columns (date, temperature_mid, dew_point, cloud_cover, and year—derived from the date column) with 2,661 samples, while the original dataset consisted of 4,747 samples and 29 columns. Like the first plot, this plot has no overlap with Homework 5, as new encoders and a different dataset were used for Homework 6.

#### Interactivity

The interactivity for this assignment involves a slider that adjusts the year displayed in the scatterplot. By default, the scatterplot shows data for all years. When the user interacts with the slider, the plot updates to display only the data recorded for the selected year.


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/sunghwansyoon/sunghwansyoon.github.io/blob/main/python_notebooks/bigfoot.ipynb" text="The Analysis" %}
</div>

