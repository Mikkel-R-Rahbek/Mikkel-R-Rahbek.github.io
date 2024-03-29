---
layout: default
title: Homepage
---

<div class="container">
    <div class="column">
        <h2>The evolution of the Tenderloin district in San Fransisco </h2>
        <p>The Tenderloin district was originally named after a similar district in New York city, and have been through multiple changes throughout the early 19th century until today in the 21st century. The district has often been a focul point for various counterculture movements and various activist groups, and therefore have been home to a wide range of cultures and people. However during the years it has also felt economic challenges, the tech boom made rent skyrocket and pushed the lower-class out of their apartmens which has led to higher rates of poverty, increased homelessness, drug addiction and crime. Limited invenstment in the district has furthered the district's demise. The data used for visualization is from the police department in San Fransisco, where each crime in various categories have been logged between 2003 and 2017.  </p>
        <img src="{{ site.baseurl }}/assets/figure.png" alt="Plot" width="600" height="400">
        <p>The figure is of DRUG/NARCOTIC use in the tenderloin district, highlighting the change in the district over the years</p>
    </div>
    <div class="column">
        <p>This is the content for column 2.</p>
        <iframe src="{{ site.baseurl }}/assets/bokeh_plot.html" width="600" height="400"></iframe>
        <p>The figure is of the District Tenderloin, where it the data has been normalized, to better get an impression of the number of incidents for each focus crime</p>
        <p>Tasdasdasdsa.</p>
    </div>
    <div class="column">
        <p>This is the content for column 3.</p>
        <iframe src="{{ site.baseurl }}/assets/heatmap.html" width="600" height="400"></iframe>
        <p>The figure is a heatmap of all districts in San Fransisco where DRUG/NARCOTIC use is highlighted</p>
        <p>At first glance, the heatmap may reveal dense clusters of drug-related incidents, indicating hotspots where these activities are most prevalent. These areas often coincide with factors such as poverty, homelessness, and lack of access to resources, which can exacerbate drug use and associated criminal behavior.
This can also be seen by the rise of eviction rates highlighted by the Eviction Report indicating large upticks in evictions in the bay area, this is a sign of a declining neighboorhood where residents fail to make rent payments.
It can also be seen that the crimes somewhat focuses at the Tenderloin district over times. Viewing the full map of San franciso it seems Drug/Nacrotic crimes move towards the neighboorhood. 
This is in line with what can be seen in videos of the area, featuring large homeless encampments, open drug use and a stark lack of police intervention.</p>
    </div>
</div>