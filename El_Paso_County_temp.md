---
layout: default
---

# El Paso County Temperature Analysis

### How is Climate Change impacting Colorado, and El Paso County? 
- Longer, hotter summers and extreme heat events (https://climatechange.colostate.edu/)
- Increased wildfire appearance and scale of impact of the fires (https://www.colorado.edu/today/2026/07/23/wildfires-are-moving-faster-heres-what-means-colorado)
- Lower water levels and increased drought (Udall, 2017, https://doi.org/10.1002/2016WR019638 Digital Object Identifier (DOI))

---

## Map of El Paso County, Colorado (Area of Interest)

<div style="display: flex; justify-content: center;">
  <div style="max-width: 100%; width: 600px;">
    <iframe src="./img/elpaso_map.html" width="100%" height="600" frameborder="0" style="display: block;"></iframe>
  </div>
</div>

El Paso County is one of the largest counties in Colorado, situated in southern Colorado directly east of the southern Front Range of the Colorado Rockies. It is home to eight municipalities as well as rural/subrural expanses. The area has seen large-scale development over the last 40 years and has one of the fastest-growing populations in the state. The county is historically susceptible to wildfires and seasonal temperature extremes due to its mountain proximity and high desert environment. 

---

## Yearly Average Temperature

<div style="display: flex;">
  <div style="max-width: 100%; width: 420px;">
    <iframe src="./img/ElPaso_yearly_avg_temp.html" width="800" height="400" frameborder="0" style="display: block;"></iframe>
  </div>
</div>


This interactive graph allows the user to locate minimums and maximums of the data by hovering their cursor over points of interest. As well as giving a general visualization of trends in annual temperature in El Paso County throughout time.
- The minimum mean annual temp is 16.778 Celsius in 1915.
- The maximum mean annual temp is 21.883 Celsius in 1937.
- The data shows clear multi-year fluctuation patterns, likely due to El Niño-Southern Oscillation (ENSO) fluctuations (ocean current-driven weather patterns, El Niño, La Niña)

--- 

## Temperature Visualizations

### Assumptions and potential caveats with our analysis:
- **Random error:**
Though we assume that all error beyond climate change is random, as mentioned above, there are other factors that may directly influence temperature change, such as shifting teleconnections (seasonal weather patterns).
- **Stationarity:**
Fanning patterns across time within El Paso County annual temperature data seem to shift in ~40-year periods. 1900-1940 shows high variability and minima-maxima extremes, characteristic of temperature trends in the state during that period (Ie: Boulder annual temperature data). After 1940, data seem to have an inward-fanning trend; however, around 1990, variability between minima and maxima extremes increases. This may be due to factors outside of the assumed generalized climate change effect, such as increased large-scale development and loss of green space. 
- **Linearity:**
There is a clear trend of warming seen from 1900-2023. However, extreme shifts in ~1930 disrupt the linear trend and influence the regression, potentially leading to a less steep trendline slope than what would be present without those extreme cold periods.
- **Gaussian Distribution:**
Data seems to be normally distributed, though with a slight skew towards the warmer extreme values.  

<div style="text-align: center;">
  <img src="./img/ElPaso_ann_temp.jpeg" height="600" width="700" alt="Annual Temperature" style="margin: 10px;">
  <img src="./img/ElPaso_ann_temp_1980_2023.jpeg" height="600" width="700" alt="Annual Temperature 1980-2023" style="margin: 10px;">
</div>

### Annual Temperature in El Paso County, CO (1900-2023) shows a clear trend of warming throughout time, despite El Niño-Southern Oscillation (ENSO) fluctuations. 

A consistent warming trend is shown through analysis of temperature data time series. An OLS regression analysis exhibits a slope of 0.007832732420920455, which indicates a warming trend of degrees per year.

When doing the same regression analysis over 1980-2023, we can see the warming trend is even greater, with a trendline slope of 0.0323349776838149, which indicates a warming trend of 0.0323349776838149 degrees Celsius per year. 

This is likely due to the omission of cold extremes seen before 1980, which led to the dampening of the trendline slope in the longer time series analysis. 
