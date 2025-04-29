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

**Indsæt plot**
<figure id="fig2">
 {% include environmental_zones_map.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 2:</strong> Animated map of San Francisco showing the location of each reported crime within the categories from 2018 to 2024.
  </figcaption>
</figure>


<figure id="fig2">
 {% include air_quality_timeseries.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 2:</strong> Animated map of San Francisco showing the location of each reported crime within the categories from 2018 to 2024.
  </figcaption>
</figure>

From these measuring stations it is possible to see that the air pollution varies significantly throughout the month of march, reaching values 

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
Checking that plots are working:
<figure>
  <img src="/plots/polar_subplots.png" width="100%" height="300" alt="Polar Subplots" style="border:none;">
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;"><strong>Figure 1:</strong>
Polar bar chart of each crime type for each hour of the day.
  </figcaption>
</figure>

Checking that html integration is working

<figure id="fig2">
 {% include overlay_crime_by_location.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 2:</strong> Animated map of San Francisco showing the location of each reported crime within the categories from 2018 to 2024.
  </figcaption>
</figure>







# Final Project 


