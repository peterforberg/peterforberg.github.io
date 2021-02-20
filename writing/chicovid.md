---
layout: page
permalink: /my-work/chicago-covid/
---
#### COVID-19 Disparity in Chicago

This is part of an ongoing project to track the COVID-19 vaccine rollout in Chicago, and as the pandemic progresses I hope to find the time to do more rigorous statistical and geographical analysis. For now, this exploratory data begins to tell the story of an unequal pandemic.

![Pie Chart](/images/race-vaccine-pie-chart.png)

This pie chart starkly displays the racial division of vaccine distribution in Chicago's 4 geographic regions (the North Side, South Side, West Side, and Loop). The South Side, which holds nearly 75% percent of the city's large Black population, accounts for only 25% of the vaccinated population. Meanwhile, the North Side, which has a mere 12% of the city's Black residents, has 50% of vaccinated residents.

The story is not just one of race. We also find that wealthier ZIP codes have much higher vaccination rates than poorer ZIP codes, which are predominantly Black. Predominantly white neighborhoods with low vaccination rates are, by no coincidence, also the poorest of the white neighborhoods.

![Scatterplot](/images/scatterplot.png)

Where are these wealthy white neighborhoods? A density plot of median income and violin plot of poverty shows us that they are largely confined to the Loop, the downtown areas of Chicago. Trailing behind the Loop is the North Side, which we remember has a disproportionately high percentage of vaccinated residents.

![Income Density Plot](/images/income-density.png)

![Poverty Violin Chart](/images/violin.png)

To put all of these variables into perspective, we can turn to a matrix of COVID vaccination rates plotted against different variables. These graphs take into account geographic location and ZIP code population. What they reveal to us is a pandemic whose vaccine salve bears a high price of race, insurance, and income, less so than important factors such as age and vulnerability.

![Scatterplot Matrix of Vaccination Rates](/images/scatterplotRate.png)

*Notes:*

For the purposes of this research, the North Side is defined as any ZIP code north of North Avenue, while the South Side is any ZIP code south of Cermark, generally speaking. 

These graphics were created in R using ggplot. The data was taken from the Chicago Open Data Portal (up to date as of February 3rd, 2021) and the 2019 5-Year American Community Survey.

