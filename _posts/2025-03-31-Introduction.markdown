---
layout: post
title:  "Children in the city of Copenhagen"
date:   2025-03-31 15:35:59 +0200
categories: jekyll update
---

<b>
Having children in the city can often be challenging and new families usually seek out the suburbs or countryside to have more space and let their children be closer to nature. However, Copenhagen proclaims that it is a city that welcomes kids with endless opportunities of playgrounds, space and even that the city <a href="https://www.visitcopenhagen.com/copenhagen/activities/copenhagen-with-kids">is designed to match the needs of kids and their parents</a>.
</b>

<p>
Through open source data, this article investigates if the city is a good fit for children based on pollution and how the recent trends have been in whether families decide to raise children while living in the capital of Denmark. 
</p>

A study shows that "in 23 countries and territories across Europe and Central Asia, children died from causes linked to air pollution in 2021, according to a new policy brief published today by UNICEF. Deaths linked to air pollution across the region accounted for 1 in 5 of all deaths of children under one."
https://www.unicef.org/tajikistan/press-releases/1-5-infant-deaths-europe-and-central-asia-linked-air-pollution-unicef

The municipality of Copenhagen has made several initiatives to improve air quality. One is the establishment of <a href="https://miljoezoner.dk/om-mz/om-miljozoner/">environmental zones</a> implemented in 2020, where certain vehicles are restricted or banned to reduce air pollution via particle filters. This area covers all of Copenhagen. Aarhus Universitet has also set up three measuring stations in the city, located between the districts of Nørrebro and Østerbro.


<figure id="fig1">
  <iframe src="{{ site.baseurl }}/assets/plots/environmental_zones.html" width="100%" height="500" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
    <strong>Figure 1:</strong> Map of Copenhagen showing environmental zones and air quality measuring stations.
  </figcaption>
</figure>



From these stations, it is possible to see that air pollution varies significantly throughout March. Only NOX and NO2 are measured at Jagtvej, and finer particles (PM2.5 and PM10) as well as SO2 are only measured at HC Andersens Boulevard. There are missing data at Jagtvej between March 10th to 13th.

<figure id="fig2">
 {% include air_quality_timeseries.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 2:</strong> Timeseries graph of different pollutants at 3 measuring stations throughout March.
  </figcaption>
</figure>
The EU has also raised concerns about high pollution levels. In [XX], a directive set limits for various pollutants over different time frames. This table shows the limits for the pollutants measured by Aarhus Universitet:


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
<td markdown="span">Some more descriptive text.</td>
</tr>
</tbody>
</table>


In order to investigate how big the concentrations are during an average day, a polar bar chart is created. These charts show how the average emissions vary per hour across a day. NOX and NO2 are compared by location, as they are the only shared measurements across sites.

NOx is a mix of NO and NO2, where NO2 is most harmful. It comes from fuel combustion, especially from cars. According to the UK Department for Environment, Food and Rural Affairs, NO2 "can cause inflammation of the airways and may increase susceptibility to respiratory infections" — especially concerning for children. (https://www.gov.uk/government/statistics/air-quality-statistics/ntrogen-dioxide)

Air pollution also affects pregnancies through low birth weight and pre-term births. (https://www.eea.europa.eu/en/newsroom/news/air-pollution-levels-across-europe)


<figure id="fig3">
 {% include NO2_emissions.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 3:</strong> Polar chart showing distribution of NO2 emissions throughout an average day.
  </figcaption>
</figure>

<figure id="fig4">
 {% include NOX_emissions.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 4:</strong> Polar chart showing distribution of NOX emissions throughout an average day.
  </figcaption>
</figure>


The charts clearly show peaks in the morning between 6–9 AM, likely due to rush hour. According to the EU, NO2 should not exceed 200 µg/m³ in a 1-hour average (https://environment.ec.europa.eu/topics/air/air-quality/eu-air-quality-standards_en), which is exceeded in Jagtvej and HC Andersens Boulevard at those times — and also around 8 PM at the latter.

Midday concentrations are lower but rise again around 5–6 PM, though still under the EU limit.

The finer particles (PM2.5 and PM10) are only measured at HC Andersens Boulevard. These are especially dangerous — they can cause strokes, cancer, and respiratory diseases (https://www.eea.europa.eu/en/newsroom/news/air-pollution-levels-across-europe). PM2.5 is small enough to enter the lungs and bloodstream (https://www.unicef.org/tajikistan/press-releases/1-5-infant-deaths-europe-and-central-asia-linked-air-pollution-unicef).

EU directives say that yearly averages of 20 µg/m³ for PM2.5 and 40 µg/m³ for PM10 should not be exceeded (https://environment.ec.europa.eu/topics/air/air-quality/eu-air-quality-standards_en). But in March, these averages were exceeded during all hours of the day, raising serious long-term health concerns for children growing up in the area.


<figure id="fig5">
 {% include PM_emissions.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Polar chart showing particle pollution throughout an average day.
  </figcaption>
</figure>
{% comment %}
<figure id="fig6">
 {% include daycare_vs_playgrounds_components.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
    <strong>Figure 6:</strong> Day care vs. playground access.
  </figcaption>
</figure>
{% endcomment %}



<figure id="fig5">
 {% include families_evolution_plot.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Polar chart showing particle pollution throughout an average day.
  </figcaption>
</figure>


<figure id="fig5">
 {% include families_population_plot.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Polar chart showing particle pollution throughout an average day.
  </figcaption>
</figure>

<figure id="fig5">
 {% include playgrounds_green_areas_plot.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Polar chart showing particle pollution throughout an average day.
  </figcaption>
</figure>

<figure id="fig5">
 {% include traffic_noise_plot.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Polar chart showing particle pollution throughout an average day.
  </figcaption>
</figure>

<figure id="fig1">
  <iframe src="{{ site.baseurl }}/assets/plots/daycare_vs_playgrounds_dual_axis.html" width="100%" height="500" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
    <strong>Figure 1:</strong> Map of Copenhagen showing environmental zones and air quality measuring stations.
  </figcaption>
</figure>
