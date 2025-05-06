---
layout: post
title:  "Children in the city of Copenhagen"
date:   2025-03-31 15:35:59 +0200
categories: jekyll update
---

<b>
Having children in the city can often be challenging and new families usually seeks out to the suburbs or countryside to have more space and let their children be closer to nature. However, Copenhagen proclaims that it is a city that welcomes kids with endless opportunities of playground, space and even that the city <a href="https://www.visitcopenhagen.com/copenhagen/activities/copenhagen-with-kids">is designed to match the needs of kids and their parents</a>.
</b>

<p>
Through open source data, this article investigate if the city is a good fit for children based on pollution and how the recent trends have been in wether families decide to put children into the world while living in the capital of Denmark. 
</p>


A Study shows that "in 23 countries and territories across Europe and Central Asia died from causes linked to air pollution in 2021, according to a new policy brief published today by UNICEF. Deaths linked to air pollution across the region accounted for 1 in 5 of all deaths of children under one."
https://www.unicef.org/tajikistan/press-releases/1-5-infant-deaths-europe-and-central-asia-linked-air-pollution-unicef


The municipality of Copenhagen has made several initiatives to improve the air quality in the city. One of these initiatives is the establishment of <a href="https://miljoezoner.dk/om-mz/om-miljozoner/">environmental zones </a> implemented in 2020, which are areas where certain vehicles are restricted or banned to reduce air pollution by having a particle filter. This area is mapped out in blue and shows that it covers all of Copenhagen. Furthermore, Aarhus Universitet has set up 3 measuring stations where different polluters are measured, located between the city districs Nørrebro and Østerbro. 
<figure id="fig1">
  <iframe src="_site/assets/plots/environmental_zones.html" width="100%" height="500" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
    <strong>Figure 1:</strong> Map of Copenhagen showing environmental zones and air quality measuring stations.
  </figcaption>
</figure>




From these measuring stations it is possible to see that the air pollution varies significantly throughout the month of march, reaching values 
The timeseries plots show that the concentration of different air polluters vary significantly thoughout March 2025. It also shows that only NOX and NO2 is measured at Jagtvej, and that the finer particle (PM2.5 and PM10) as well as SO2 is only measured at HC Andersens Boulevard. Furthermore, there are missing data at Jagtvej between March 10th to 13th. 

<figure id="fig2">
 {% include air_quality_timeseries.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 2:</strong> Timeseries graph of different polluters at 3 measuring stations througout March.
  </figcaption>
</figure>



The EU has also envoked the problems with high pollution and in xx a directive set limits for different time units indivually for different polluters. THis table shows the limits set for the polutters measured by Alrhus Universitet:

<table>
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead>
<tr class="header">
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">First column **fields**</td>
<td markdown="span">Some descriptive text. This is a markdown link to [Google](http://google.com). Or see [some link][mydoc_tags].</td>
</tr>
<tr>
<td markdown="span">Second column **fields**</td>
<td markdown="span">Some more descriptive text.
</td>
</tr>
</tbody>
</table>


In order to investigate how big the concentrations are during an average day, a polar bar chart is created. 
The polar bar charts shows how much the average emmission measured pr hour vary during a day of 24 hours. The emissions of NOX and NO2 is compared by location, as these are the only measurements that overlap across the locations. 

NOx is a combination of the two gasses NO and NO2, where the NO2 is most harmful, and is emitted into the air from burning fuels, which primarily stems from cars in urban areas. The department for Environment, Food and Rural affairs describes that NO2 "can cause inflammation of the airways and may increase susceptibility to respiratory infections" https://www.gov.uk/government/statistics/air-quality-statistics/ntrogen-dioxide , which is especially critical for childrens lung development and can create asthma. Furthermore, air pollution also affects pregnancies by low birth weight and pre term births. https://www.eea.europa.eu/en/newsroom/news/air-pollution-levels-across-europe. 

<figure id="fig3">
 {% include polar_barchart_NO2.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 3:</strong> Polar chart showing distribution of NO2 emission throughout an average day.
  </figcaption>
</figure>

<figure id="fig4">
 {% include polar_barchart_NOX.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 4:</strong> Polar chart showing distribution of NOX emission throughout an average day.
  </figcaption>
</figure>


The polar bar chart clearly shows that the concentration is highest in the morning between 6-9, which likely is because this is the time very people are driving to work. The limit set by the EU states that NO2 emissions shold not exceed 200 in a 1 hour average https://environment.ec.europa.eu/topics/air/air-quality/eu-air-quality-standards_en which is exceeded in both Jagtvej and H. C Andersen s bourlevard during this time period and also in hour 20 at H. C. Andersens Boulevard. 

Furthermore, the middle of the day show very low concentrations, and increases again at hour 17-18, however, this is below the EU limit. 


The finer particles (PM2.5 and PM10) is similarly plotted, however this is only measures at the H. C. Andersens Boulevard measurement station. This pollutant are much more damaging, and can cause strokes, cancer and respiratory deasises,  https://www.eea.europa.eu/en/newsroom/news/air-pollution-levels-across-europe, and the PM2.5 is so small that it penetrates deep inside the lings and into the bloodstreams https://www.unicef.org/tajikistan/press-releases/1-5-infant-deaths-europe-and-central-asia-linked-air-pollution-unicef

The EU directive states that the yearly average of 20 and 40 µg/m3 should not be exceeded for PM2.5 and PM10, respectively. https://environment.ec.europa.eu/topics/air/air-quality/eu-air-quality-standards_en. However, for the month of March this average is exceeded ibn all hours of the day, indicating that this could be highly problematic, especially for children who grow up there, because it will have long term health issues. 



<figure id="fig5">
 {% include polar_barchart_PM25and10.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Polar chart showing distribution showing particle pollution throughout an average day.
  </figcaption>
</figure>



<figure id="fig6">
 {% include daycare_vs_playgrounds_components.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
    <strong>Figure 6:</strong> Day care something. 
  </figcaption>
</figure>
