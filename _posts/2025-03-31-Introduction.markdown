---
layout: post
title:  "Introduction"
date:   2025-03-31 15:35:59 +0200
categories: jekyll update
---


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


