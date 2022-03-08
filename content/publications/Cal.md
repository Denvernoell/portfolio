---
title: "Visualizing California Water Quality With Python"
date: 2022-02-16
pubtype: "Article"
featured: true
description: "Interactive Dissolved Oxygen Level Chart using Publically Available Data"
tags: ["Engineering","Python"]
image: "https://denvernoell.com/_next/image?url=https%3A%2F%2Fcdn.hashnode.com%2Fres%2Fhashnode%2Fimage%2Fupload%2Fv1645068191331%2F9d-bvuAGT.png%3Fw%3D1600%26h%3D840%26fit%3Dcrop%26crop%3Dentropy%26auto%3Dcompress%2Cformat%26format%3Dwebp&w=3840&q=75"
link: "https://denvernoell.com/visualizing-california-water-quality-with-python"
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 400
sitemap:
  priority : 0.8
---

<br><br><br>
<br>
<!-- <br><br><br> -->

## Source Data
[California Open Data Portal](https://data.ca.gov/) provides water quality data available [here](https://data.ca.gov/dataset/water-quality-data). This contains data ranging from 1968 to 2022 and has results for parameters such as dissolved oxygen and chemical levels. In this example, I will be looking at the Dissolved Oxygen Levels in California.

## Figure 

The graphic below shows the monthly Dissolved Oxygen Level for each station. The stations within each county will share the same shape but have a different color.

Notes
- Hovering over a point will show additional information for the point
- Clicking on a station in the legend will highlight points from that station
- Viewing in landscape mode on mobile devices is advised

<iframe src="https://datapane.com/u/denvernoell/reports/E7yq5g7/water/embed/" width="100%" height="800em" style="border: none;">IFrame not supported</iframe>



---
## Python Modules Used
- *[Pandas](https://pandas.pydata.org/)* to select a trimmed dataset from the original data
- *[Altair](https://altair-viz.github.io/index.html)* to create the visualization
- *[Datapane](https://datapane.com/)* to host the visualization

## Source Code
Source code is available [here](https://github.com/Denvernoell/California-Water-Quality).