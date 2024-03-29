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
        <p>There is a rising change from 2006 to 2009 in DRUG/NARCOTIC use, and in 2007 an article was released by SFGate, mentioning an inceases in drug violence. In response the police department increased it's investment into counter crime and increased the number of police patrols, in an attempt to get a control of the rising violence. The increased patrols and invenstment for countering crimes, reflects on the dataset as the incidents for DRUG/NARCOTICS are exploding in those years. There is a big dropoff in incidents after 2009, and the number of incidents at the end of 2017 is less than a thousand, and less than one fith of its peak in 2008.  </p>
    </div>
    <div class="column">
        <iframe src="{{ site.baseurl }}/assets/bokeh_plot.html" width="600" height="400"></iframe>
        <p>The figure is of the District Tenderloin, where it the data has been normalized, to better get an impression of the number of incidents for each focus crime</p>
        <p>On the Bokeh plot, we've illustrated a comprehensive view of the focus crimes within San Francisco's Tenderloin district. Notably, we've highlighted Prostitution and Drug/Narcotics offenses, which exhibit a strong correlation, underscoring the interconnectedness of social issues and criminal behavior.

Despite the apparent decline in these crimes, a phenomenon that might seem contradictory given the context, several factors could contribute to this trend:

Shift in Law Enforcement Priorities: Law enforcement agencies may have redefined their strategic focus or deployed targeted approaches to combat specific types of crime, such as violent offenses or property crimes. Consequently, resources previously allocated to addressing prostitution and drug-related activities might have been reallocated, potentially leading to a decrease in enforcement efforts in these areas.

Misclassification or Underreporting: It's plausible that incidents related to prostitution and drug offenses are being misclassified or underreported.
Additionally, it's worth noting a sharp rise in both highlighted crimes around 2008. This surge is likely attributed to the 2008 financial crisis, which often pushes individuals towards drugs and prostitution due to financial instability and depression stemming from worsening economic conditions.</p>
    </div>
    <div class="column">
        <iframe src="{{ site.baseurl }}/assets/heatmap.html" width="600" height="400"></iframe>
        <p>The figure is a heatmap of all districts in San Fransisco where DRUG/NARCOTIC use is highlighted</p>
        <p>At first glance, the heatmap may reveal dense clusters of drug-related incidents, indicating hotspots where these activities are most prevalent. These areas often coincide with factors such as poverty, homelessness, and lack of access to resources, which can exacerbate drug use and associated criminal behavior.
This can also be seen by the rise of eviction rates highlighted by the Eviction Report indicating large upticks in evictions in the bay area, this is a sign of a declining neighboorhood where residents fail to make rent payments.
It can also be seen that the crimes somewhat focuses at the Tenderloin district over times. Viewing the full map of San franciso it seems Drug/Nacrotic crimes move towards the neighboorhood. 
This is in line with what can be seen in videos of the area, featuring large homeless encampments, open drug use and a stark lack of police intervention.</p>
        <p>Today San Fransisco has done a lot to reduce drug consumption by both decriminalizing drug use, and investing into harm reduction facitilies ensuring free straws and foil for fentanyl use to reduce infection</p>
    </div>
</div>