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
        <p>There is a rising change from 2006 to 2009 in DRUG/NARCOTIC use, and in 2007 an article was released by SFGate, mentioning an inceases in drug violence. In response the police department increased it's investment into counter crime and increased the number of police patrols, in an attempt to get a control of the rising violence. The increased patrols and invenstment for countering crimes, reflects on the dataset as the incidents for DRUG/NARCOTICS are exploding in those years. There is a big dropoff in incidents after 2009, and the number of incidents at the end of 2017 is less than a thousand, and less than one fith of its peak in 2008.</p>
    </div>
    <div class="column">
    </p>In 2013 a report highlighted lease breaches was increased by 127% from 2009 to 2013, and an article from 2018 highlighted the Deterioration of the streets due to urination between 2015 and 2018. The data itself is therefore not good representation of the situation in the Tenderloin district, as even though the DRUG/NARTOOTIC crime has decreased, it is most likely due to the police force no longer enforcing the crime, and the drug use has rather risen in those years</p>
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
        <p>Today San Fransisco has done a lot to reduce drug consumption by both decriminalizing drug use, and investing into harm reduction facitilies ensuring free straws and foil for fentanyl use to reduce infection</p>
    </div>
</div>