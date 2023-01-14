# Resident bird species are more responsive to a changing climate
Data used:USGS Breeding Bird Survey; NOAA weather data; AVONET avian morhpological data

Technology used: Analysis: Pandas, statsmodels (Python), Google BigQuery.  
                 Visualization: GeoPandas, Matplotlib, Seaborn, Plotly.  
                 Web-scraping: Beautiful Soup.    

A predicted consequence of rising global temperatures is that species in the northern hemisphere will shift their ranges to higher 
latitudes. By combining millions of bird observations from the USGS Breeding Bird Survey spanning the years 1966-2019, and temperature 
records from the NOAA, I tested this prediction on North American breeding bird species. 


Roughly half of the songbird species examined experineced a northward shift in their mean range. On average, this shift began in the mid-1990s,
and continued through 2019. Data are mean latitudes weighted by the number of birds observed at each site, with 95 percent confidence intervals.
![image](https://user-images.githubusercontent.com/89553765/211092509-9d28b6d5-21d6-4170-bdc7-7b2893849f5d.png)

Temperatures in June have shown a steady increase since the mid-1990s. This timeline matches that of the shift mean latitude of songbird
species. Data are average monthly temperatures for June (background trace), and the overlaid running average with a 5-year window.

![image](https://user-images.githubusercontent.com/89553765/211460410-05c47356-3460-491c-82cd-6dea6b6610a5.png)

Visualizing all observations for the years 1987 and 2019 reveals that some species experience no northward shift, or even a southward shift 
(prothonotary warbler), a modest northward shift (eastern bluebird), or a pronounced northward shift (red-bellied woodpecker). 

![image](https://user-images.githubusercontent.com/89553765/211158795-18c39c09-aa12-4ff2-832a-b437ff3c0983.png)

Plotting the northern 97.5th percentile latitude of observations against time reveals that not only are some species experiencing a shift in
mean latitude, but their ranges are actually expanding northwards.
![image](https://user-images.githubusercontent.com/89553765/211460334-87b071ad-6c07-4b56-b5f3-36bfbb4eaed0.png)


A striking trend, and the most pronounced, was that the pace of the northward shifts tracks with migratory behavior. Species which reside in the US/Canada all year have shifted their ranges northwards at a much faster pace than short-distance migrants, who in turn have shifted their ranges
northwards more quickly than long-distance migrants.

![image](https://user-images.githubusercontent.com/89553765/211112373-4e3a8f08-cbee-413e-a786-d4d55e3430c5.png)

This trend remained statistically significant even after controlling for preferred habitat, and two measures of dispersal ability (hand-wing index
and range size) in a multiple linear regression model. Coefficients are standardized to allow direct comparison.

![image](https://user-images.githubusercontent.com/89553765/211449214-272f12b3-e22a-48d8-a236-4fd2b5dd451d.png))
