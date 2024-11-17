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



#### This is a plot of bigfoot observations in the United States

<vegachart schema-url="{{ site.baseurl }}/assets/json/bigfoot.json" style="width: 100%"></vegachart>




## Search The Data & Methods

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

