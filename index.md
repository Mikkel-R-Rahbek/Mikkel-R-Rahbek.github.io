---
layout: default
title: Homepage
---

<div class="container">
    <div class="column">
        <h2>The evolution of the Tenderloin district in San Fransisco </h2>
        <p>The Tenderloin district, originally named after a similar area in New York City, has undergone numerous transformations from the early 19th century to the present day in the 21st century. Throughout its history, the district has served as a focal point for various counterculture movements and activist groups, resulting in a diverse population representing a wide range of cultures.
However, over the years, the district has faced significant economic challenges. The tech boom caused rents to skyrocket, displacing many lower-income residents from their apartments and exacerbating issues such as poverty, homelessness, drug addiction, and crime. Furthermore, the limited investment in the district has contributed to its decline.
Data for visualization purposes is sourced from the San Francisco Police Department, documenting incidents across various crime categories from 2003 to 2017. </p>
        <img src="{{ site.baseurl }}/assets/figure.png" alt="Plot" width="600" height="400">
        <p>The figure is of DRUG/NARCOTIC use in the tenderloin district, highlighting the change in the district over the years</p>
        <p>Between 2006 and 2009, there was a notable uptick in drug/narcotic usage, coinciding with a 2007 article by SFGate highlighting an escalation in drug-related violence. In response, the police department bolstered its efforts to combat crime, intensifying patrols and increasing investment in crime prevention measures to curb the rising violence. This heightened focus on policing is reflected in the dataset, with incidents of drug/narcotic-related offenses surging during those years.
        Following the peak in 2008, there was a significant decline in incidents, with the number dropping to less than a thousand by the end of 2017. This marks a substantial decrease, amounting to less than one-fifth of the peak observed in 2008.</p>
    </div>
    <div class="column">
    <p>In 2013, a report underscored a staggering 127% increase in lease breaches from 2009 to 2013, indicating a significant challenge in maintaining property standards. Additionally, an article from 2018 shed light on the deterioration of streets attributed to increased incidents of public urination between 2015 and 2018. While reported incidents of drug/narcotic crimes have decreased, it's plausible that this decline is not indicative of improved conditions but rather a result of reduced police enforcement in recent years. It's conceivable that drug usage has, in fact, escalated during this period.</p>
        <iframe src="{{ site.baseurl }}/assets/bokeh_plot.html" width="600" height="400"></iframe>
        <p>The figure represents the Tenderloin District, where the data has been normalized to provide a clearer impression of the number of incidents for each focus crime</p>
        <p>On the Bokeh plot, we've depicted a comprehensive overview of the focus crimes within San Francisco's Tenderloin district. Notably, we've emphasized Prostitution and Drug/Narcotics offenses, which demonstrate a strong correlation, highlighting the intertwined nature of social issues and criminal behavior. Despite the apparent decline in these crimes, a trend that may seem paradoxical given the circumstances.

Based on our research, it's evident that drug use and prostitution remain prevalent, if not more so, in the later years of the dataset. This suggests that the decreasing crime rates for these two highlighted offenses may be attributed to underreporting. It's possible that law enforcement authorities are choosing not to arrest offenders, potentially reflecting a shift in policing strategies. This phenomenon could stem from various reasons, such as a perceived inability to address the root causes of these crimes effectively, a strategic decision to prioritize other types of offenses, or a broader containment strategy focusing on restricting such activities to the Tenderloin district.

Furthermore, the consistent number of arrests related to assault indicates that law enforcement agencies may be prioritizing violent crimes over drug and prostitution offenses, or other crimes such as Larceny/theft . This strategic allocation of resources could suggest a deliberate effort to target more immediate threats to public safety while potentially deprioritizing certain non-violent offenses within the district.</p>
    </div>
    <div class="column">
        <iframe src="{{ site.baseurl }}/assets/heatmap.html" width="600" height="400"></iframe>
        <p>The figure is a heatmap of all districts in San Fransisco where DRUG/NARCOTIC use is highlighted</p>
        <p>At first glance, the heatmap may reveal dense clusters of drug-related incidents, indicating hotspots where these activities are most prevalent. These areas often coincide with factors such as poverty, homelessness, and lack of access to resources, which can exacerbate drug use and associated criminal behavior.
This can also be seen by the rise of eviction rates highlighted by the Eviction Report indicating large upticks in evictions in the bay area, this is a sign of a declining neighboorhood where residents fail to make rent payments.
It can also be seen that the crimes somewhat focuses at the Tenderloin district over times. Viewing the full map of San franciso it seems Drug/Nacrotic crimes move towards the neighboorhood. 
This is in line with what can be seen in videos of the area, featuring large homeless encampments, open drug use and a stark lack of police intervention.</p>
        <p>Today San Fransisco has done a lot to reduce drug consumption by both decriminalizing drug use, and investing into harm reduction facitilies ensuring free straws and foil for fentanyl use to reduce infection [NY Times](https://www.nytimes.com/2024/01/31/upshot/san-francisco-drug-crisis.html)</p>
    </div>
</div>