---
name: Final Project
tools: [Python, HTML, vega-lite, Altair]
image: assets/pngs/Banner.png
description: In final project IS445, we are using Netflix dataset to present the story of the dataset. Click here for more...
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Final Project - Group 13 - Chien Nguyen - Hongyu Yan

The idea of this analysis is telling the story about the dataset of Netflix from 1920 to 2022
## Figure 1

```python
  "Method" : Heat Map and Bar Chart
  "Scheme" : yellowgreen
  "Columns" : Rating, Country and Realease Year
  "Encoding type" : Norminal and Ordinal
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard1.json" style="width: 80%"></vegachart>
 <center> Figure 1</center>

<br />
In figure 1, we want to show the relationship between rate, country, and release years. Since the first data in 'release year' is 1925, but there are only several data in first thirty years. in this case, we filtered the release year between 1990-2020. The second filter we applied is drop movie or ty shows which have more than one country in the 'country' cloumn. Thus, we have the dashboard showing above. It is based on altair, so users will need to draw a rectangle anywhere on the left component. After drawing the rectangle, it will remain on there and users can drag around. The rectangle's size can also be changed by using scroll on mouse, or two fingers swipe up and down on touchpad. In different place, the right component will show relevant release year.

## Figure 2

```python
  "Method" : Heat Map and Bar Chart
  "Columns" : Rating, Type and Realease Year
  "Scheme" : yellowgreen
  "Encoding type" : Norminal and Ordinal
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard2.json" style="width: 100%"></vegachart>
 <center> Figure 2</center>
<br />

In the figure 2, By applying same filters, the dashboard 2 showing relationships between 'rate', 'type', and 'release year'. It is based on altair, so users will need to draw a rectangle anywhere on the left component. After drawing the rectangle, it will remain on there and users can drag around. The rectangle's size can also be changed by using scroll on mouse, or two fingers swipe up and down on touchpad. In different place, the right component will show relevant release year.


## Figure 3

```python
  "Method" : Heat Map and Bar Chart
  "Columns" : Type, Country and Realease Year
  "Scheme" : yellowgreen
  "Encoding type" : Norminal and Ordinal
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboard3.json" style="width: 100%"></vegachart>
<center> Figure 3</center>
<br />
By applying same filters, the figure 3 showing relationships between 'country', 'type', and 'release year'. It is based on altair, so users will need to draw a rectangle anywhere on the left component. After drawing the rectangle, it will remain on there and users can drag around. The rectangle's size can also be changed by using scroll on mouse, or two fingers swipe up and down on touchpad. In different place, the right component will show relevant release year.


### Additional informations, click the buttons bellow to see the dataset and my code. Thanks for reading.

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/cnguyen1411/cnguyen1411.github.io/blob/main/python_notebooks/HW10-Altair-Analysis.ipynb" text="The Analysis" %}
</div>

