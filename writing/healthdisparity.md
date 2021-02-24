---
layout: page
permalink: /my-work/health-disparity/
---
#### Sexual Health Disparities in Chicago's Community Areas

This represents my first attempt at exploratory data analysis 2 years ago. Using the geographical software GeoDa, I combined data from the U.S. Census and Chicago Open Data Portal to investigate sexual health disparities in Chicago.

First, we look at a few variables and see if there appear to be viable statistical overlaps of disparities.

![Maps](/images/quantilemaps.png)

We immediately see clusters of high chlamydia rates, high crime, high poverty, high un-education rates, and high abandoned buildings. These might overlap with where see see more public health clinics, which is a good sign for the health of Chicago. We can step back from the maps for a second and see if there are correlations between these variables using a correlation matrix.

![Scatterplot matrix](/images/scatterplot_matrix.png)

Here we do see a number of correlations, suggesting there may be statistically significant spatial heterogeneity. I then constructed some spatial weights and, after a few more graphs, decided that k-nearest neighbors was the best strategy. Based on those weights, we can start to see if there are signficant overlaps of the variables using both Moran's I and Local Geary.

![High high](/images/highigh.png)

This first graph shows us that there are a number of statistically significant overlaps of these variables, demonstrating areas where there are higher rates of negative socio-economic conditions and also higher rates of chlamydia. Luckily there also appear to be more public health clinics. 

The next graph highlights the areas where there are statistically significant overlaps with low rates of negatives socio-economic conditions and low rates of chlamydia. These places appear to have comparable or lower numbers of public health clinics.

![Low low](/images/lowlow.png)

This brief statistical exploration was based on a hodgepodge of data, but it begins to suggest that the sexual health experiences of Chicagoans are geographically stratified and that resources have been put in place to begin to address these stratifications. Such an exploration sets the groundwork for a deeper look at health clinics in Chicago.