---
layout: post
title:  "Children in the city of Copenhagen"
date:   2025-03-31 15:35:59 +0200
categories: jekyll update
---

<b>
Having children in the city can often be challenging and new families usually seek out to the suburbs or countryside to have more space and let their children be closer to nature. However, Copenhagen proclaims that it is a city that welcomes kids with endless opportunities of playgrounds, abundance of green space and even that the city <a href="https://www.visitcopenhagen.com/copenhagen/activities/copenhagen-with-kids">is designed to match the needs of kids and their parents</a>. Through open source data, this article investigates how recent trends have been regarding families in the capital of Denmark, and weather the city can live up to their claims. 
</b>


<figure id="fig1" style="float: right; margin-left: 10px; margin-bottom: 5px; max-width: 400px;">
  <iframe src="{{ site.baseurl }}/assets/plots/environmental_zones.html" width="400" height="300" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 5px;">
    <strong>Figure 1:</strong> Map of Copenhagen showing environmental zones and air quality measuring stations. <a href="https://www.opendata.dk/city-of-copenhagen/miljozoner">[Data origin]</a>
  </figcaption>
</figure>


<p>
The municipality of Copenhagen has made several initiatives to improve the well-being of their citizens. For example to improve air quality in the city, an <a href="https://miljoezoner.dk/om-mz/om-miljozoner/">environmental zone</a> covering the entire city has been established. This was implemented in 2020 and intends to reduce air pollution from vehicles by permitting access only for vehicles with certain particle filters installed. To monitor the air pollution, Aarhus Universitet has installed three measuring stations in the city, located between the districts of Nørrebro and Østerbro. The environmental zone and measuring stations are mapped out on the right in <ref target="fig1">Figure 1</ref> . Please note that it is possible to zoom-in on the plot the get better insigt to the location of the measuring stations marked as red icon.
</p>

<p>
 A <a href="https://www.unicef.org/tajikistan/press-releases/1-5-infant-deaths-europe-and-central-asia-linked-air-pollution-unicef">UNICEF</a> report shows that for children under 1 out of 5 children mortalities for ages below 1 year are linked air pollution, based on a study from 23 countries and territories across Europe and Central Asia. From the measuring stations, different pollutant are measured and the graph below shows how these varies significantly throughout March. Furthermore it should be noticed that on 2 pollutants, namely NOX and NO2-emissions, are measured at Jagtvej, while the finer particles (PM2.5 and PM10) as well as SO2-emissions are exclusively measured at HC Andersens Boulevard. The graphs can be filtered by clicking on the legend of different pollutants. 
</p>

<figure id="fig2">
 {% include air_quality_timeseries.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 2:</strong> Timeseries graph of different pollutants at the 3 measuring stations throughout March. <a href="https://www.opendata.dk/city-of-copenhagen/luftforurening">[Data origin]</a>
  </figcaption>
</figure>


<p>
The EU has also raised concerns about high air pollution levels in cities and has invoked the directive: <a href="https://environment.ec.europa.eu/topics/air/air-quality/eu-air-quality-standards_en">EU air quality standards</a>, that defines standards with limits for different pollutants averaged over different timeperiods. A snippet of the relevant pollutants are listed below in the table:
</p>
<table style="border-collapse: collapse; width: 60%; margin: 0 auto; font-family: 'Arial', sans-serif; text-align: left; font-size: 14px;">
  <colgroup>
    <col style="width: 15%;" />
    <col style="width: 20%;" />
    <col style="width: 25%;" />
  </colgroup>
  <thead>
    <tr style="background-color: #f4f4f4; color: #333; font-weight: bold; border-bottom: 2px solid #ddd;">
      <th style="padding: 8px; text-transform: uppercase; text-align: center;">Pollutant</th>
      <th style="padding: 8px; text-transform: uppercase; text-align: center;">Concentration</th>
      <th style="padding: 8px; text-transform: uppercase; text-align: center;">Averaging period</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 6px; text-align: center;">NO2</td>
      <td style="padding: 6px; text-align: center;">200 µg/m³</td>
      <td style="padding: 6px; text-align: center;">1 hour</td>
    </tr>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 6px; text-align: center;">PM2.5</td>
      <td style="padding: 6px; text-align: center;">20 µg/m³</td>
      <td style="padding: 6px; text-align: center;">1 year</td>
    </tr>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 6px; text-align: center;">PM10</td>
      <td style="padding: 6px; text-align: center;">40 µg/m³</td>
      <td style="padding: 6px; text-align: center;">1 year</td>
    </tr>
    <tr>
      <td style="padding: 6px; text-align: center;">SO2</td>
      <td style="padding: 6px; text-align: center;">350 µg/m³</td>
      <td style="padding: 6px; text-align: center;">1 hour</td>
    </tr>
  </tbody>
</table>
<br>
<p>
NOX is a mix of NO and NO2, where NO2 is causing the most harm and is emmitted from fuel combustion, especially from cars in urban areas. According to the <a href="https://www.gov.uk/government/statistics/air-quality-statistics/ntrogen-dioxide">UK Department for Environment, Food and Rural Affairs</a>, NO2 can cause short term inflammation in the airways and may increase susceptibility to respiratory infections, which is especially critical for childrens lung development and can create asthma. Looking at <ref target="fig2">Figure 2</ref> the NO2 emissions exceeds the limits of 200 µg/m³ many times throughout March, however the EU directive also sets these limits based on averaged values across different time periods. In order to investigate how big the concentrations are during an average day, a polar bar chart in <ref target="fig3">Figure 3</ref> presents how the emissions of this specific pollutant average across hours during the days in March, which is more comparable to the EU standards. 
</p>

<figure id="fig3">
 {% include NO2_emissions.png %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 3:</strong> Polar chart showing average hourly distribution of NO2 emissions throughout March.
  </figcaption>
</figure>


<p>
The charts clearly show peaks of NO2 emission in the morning between 6–9 AM, likely due to rush hour when people are driving to work. The midday concentrations are lower but increase again in the afternoon and evening hours. However, the limit of 200 µg/m³ is exceeded at H. C. Andersens Boulevard and Jatvej during the peak hours, which can be verified by hovering over the plot. This is problematic as Denmark is obliged to obey EU directives. 
</p>

<p>
Air pollution also affects pregnancies through low birth weight and pre-term births and the finer particles called PM2.5 and PM10 can cause more long term harm including strokes, cancer, and respiratory <a href="https://www.eea.europa.eu/en/newsroom/news/air-pollution-levels-across-europe">diseases</a>. The PM2.5 particles are even so small, that they can to enter the lungs and  <a href="https://www.unicef.org/tajikistan/press-releases/1-5-infant-deaths-europe-and-central-asia-linked-air-pollution-unicef">bloodstream</a>. The finer particles (PM2.5 and PM10) are only measured at H. C. Andersens Boulevard, and a similar polar chart shown in <ref target="fig4">Figure 4</ref> for this data indicates that the EU limits of 20 µg/m³ and 40 µg/m³ for PM2.5 and PM10, respectively, is exceeded in all hours of the day:
</p>
<figure id="fig4" style="float: right; margin-left: 10px; margin-bottom: 5px; width: 100%; max-width: 100%;">
  <iframe src="{{ site.baseurl }}/assets/plots/PM_emissions.html" 
          width="100%" 
          height="500" 
          frameborder="0" 
          style="margin-bottom: 0;"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 0;">
    <strong>Figure 4:</strong> Polar chart showing particle pollution throughout March.
  </figcaption>
</figure>

<p>
And even though the EU directive states that this limit is set for a 1 year averaging period, the results indicate that Copenhagen might not also be living up to these standard. This should raise concerns about prolonged exposure to these very harmful particles, especially for children in their developing years. 
</p>
<p>
Despite the risk of exposing children to harmful emission, the number of families in Copenhagen has seen a growth in recent years, where the city districts Amager Vest, Valby and Kgs. Enghave has had quite an increase in the last 10 year. This is shown in the interactive graph below, which can be filtered by clicking on the legends to examine the trend for specific city districts.
</p>
<figure id="fig5">
 {% include families_evolution_plot.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Evolution of nr. of families in different city districts in Copenhagen. <a href="https://kk.statistikbank.dk/statbank5a/Graphics/mapanalyser.asp?maintable=KKFAM1&lang=0">[Family data origin]</a>
  </figcaption>
</figure>


<figure id="fig1" style="float: right; margin-left: 10px; margin-bottom: 5px; max-width: 400px;">
  <iframe src="{{ site.baseurl }}/assets/plots/families_population_plot.html" width="400" height="350" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 5px;">
    <strong>Figure 1:</strong> Family growth and share of families in Copenhagen. 
  </figcaption>
</figure>

<p>
<br>
<br>
<br>
  The plots on the right shows that, even though there seem to be an overall trend of families in Copenhagen, it could be correlated to the fact that overall the population in Copenhagen has been increasing in recent years. The red graph shows that the relative share of families compared to the total population growth in Copenhagen is in fact decreasing, indicating that families are not choosing Copenhagen as their primary base, controversely to the overall urbanization. 
</p>
<br>

<p>
  Still, this does not change the fact that Amager, Valby and Kgs. Enghave has had an increase in families compared to other city districts, which could be due to the many green areas located in those city districts. The map below in <ref target="fig7">Figure 7</ref> shows where green areas are located in Copenhagen, with Amager standing out, primarily because of the protected natural area <a href="https://www.kk.dk/brug-byen/byens-groenne-oaser/parker-og-groenne-omraader/amager-faelled">Amagerfælled</a> located in the western part of Amager.
</p>

<p>
  Studies show that children who have access to green areas, and are exposed to them on a regular basis, show a reduced risk of mental health disorders and improved <a href="https://www.nih.gov/news-events/nih-research-matters/green-space-may-improve-young-children-s-mental-health">mood</a>, which could have had an impact on parents' decisions to settle their families down in Amager.
</p>

<figure id="fig8" style="float: right; margin-left: 10px; margin-bottom: 5px; width: 100%; max-width: 100%; ">
  <iframe src="{{ site.baseurl }}/assets/plots/playgrounds_green_areas_plot.html" width="100%" height="500" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 5px;">
    <strong>Figure 8:</strong> Map of green areas and playground in Copenhagen. <a href="https://www.opendata.dk/city-of-copenhagen/legepladser1">[Playground data origin]</a> <a href="https://www.opendata.dk/city-of-copenhagen/gronne-omrader">[Green areas data origin]</a>
  </figcaption>
</figure>
<p>
In the map above, playgrounds located around Copenhagen is also pinpointed, where it is possible to hover over the points to get the exact names of the playgrounds. Having access to playground has a positive influence on the both physical and social development of children in all ages and will help children <a href="https://www.nih.gov/news-events/nih-research-matters/green-space-may-improve-young-children-s-mental-health">"engage, change and impact the world around them"</a>. 
</p>

<p>
To investigate this further, the interactive bar chart below show two key indicators of how the access to day care and playgrounds is distributed in different city district in Copenhagen. When clicking on the red legend ("Playground per 1000 Kids"), the number of playground per 1000 children in ages 0-4 years per city district. This clearly shows that Indre By has many more playground compared to the number of youngster living in Indre By, compared to other city districts. This could be due to the space limitations in this more densely populated area in Copenhagen, which may result in the playground not being able to accommodate as many children. However, the sizes of the playgrounds are not taken into consideration. Further, due to a limited access to green areas, it could also be that the municipality of Copenhagen has prioritized investing in playgrounds Indre By, as a way to provide children with accessible recreational spaces to improve the quality of life for families and children, specifically. This argument is supported by those city district pointed out ealier as having high acess to green areas, only has between 2-4 playground per 1000 kids. This suggests that the municipality of Copenhagen might have taken access to green areas into concideration, when distributing playgrounds in city districts. 
</p>


<figure id="fig9">
  <iframe src="{{ site.baseurl }}/assets/plots/daycare_vs_playgrounds_dual_axis.html" width="100%" height="600" frameborder="0"></iframe>
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
    <strong>Figure 9:</strong> Daycare Coverage vs Playgrounds per 1000 Kids. ***indsæt link***
  </figcaption>
</figure>

By clicking on the blue legend ("Daycare coverage(%)") it is possible to see how good access parents have to putting their children in day care. Many parents in Copenhagen has found it a struggle to find day care for their children, due to long waitlists and overcrowded institutions. And an article from  <a href="https://cphpost.dk/2012-04-23/general/daycare-woes-continue-for-copenhagen-parents/">"The Copenhagen Post"</a> descibed these challenges in 2012, where the Mayor of Copenhagen Frank Jensen stated that by 2014 "there will be daycare for everyone within four kilometres of their home." So based on a baseline assuming that the share of children in ages 0-4 years to daycare institutions in the entirety of Copenhagen relates to 100%, the distribution in each city district is found. This analysis reveals that Østerbro, Amager, and Vanløse have the lowest share of daycare institutions, while Indre By stands out with an exceptionally high concentration of daycare facilities. Similar to the playgrounds, this could again be due to the limited access in the central part of Copenhagen, leading to smaller daycare institutions that are unable to accommodate a large number of children. 

The same trend is seen for the share of Daycare. Likely this is because due to Indre By being the most densely populated, causing the playgrounds and daycare centers to fit less children. 



However indre By has a lot of playgrounds however the noise pollution levels are also very high in the city center, where children are playing on playground outside. 

<figure id="fig5">
 {% include traffic_noise_plot.html %}
  <figcaption style="text-align: center; font-style: italic; margin-top: 10px;">
   <strong>Figure 5:</strong> Noise pollution in Copenhagen XXX.
  </figcaption>
</figure>

All in all, the municipality of Copenhagen has taken action in making city-living for families manageable, however 

Concluding on wether copenhagen is a good city to settle down as a family?
