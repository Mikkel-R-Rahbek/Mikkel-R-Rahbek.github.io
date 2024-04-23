---
layout: page
title: 3-1-1 - Street Cleaning Requests in San Francisco
permalink: /project/
---

<html>
<head>
	<style>
        .page-title {
            color: white;
            font-size: 32px;
        }
        h3 {
            font-size: 14px;
            text-align: center
        }
		.column {
			float: left;
			width: 50%;
			padding: 10px;
			box-sizing: border-box;
            text-align: center;
		}
		.column img {
			display: block; /* make the image a block element */
			max-width: 100%; /* set the maximum width of the image to the width of its parent element */
			height: auto; /* allow the height of the image to adjust proportionally */
			margin: 0 auto; /* center the image horizontally */
		}
		.column p {
			width: 80%; /* set the width of the paragraph text to 80% of the column */
			margin: 0 auto; /* center the paragraph text horizontally */
            text-align: justify
		}
        .border-right {
            border-right: 1px solid black;
        }
		.clearfix::after {
			content: "";
			clear: both;
			display: table;
		}
        div {
            text-align: justify
        }
        .back-gif {
            position: absolute;
            left:0;
            width: 100%;
            height: auto;
            z-index:-1;
            transform: translateY(-80%);
        }
        footer {
            text-align: right;
        }
        .center {
            display: block;
            margin-left: auto;
            margin-right: auto;
            width: 85%;
        }
        iframe {
            display: block;
            border-style:none;
            margin: 0 auto;
        }
	</style>
</head>

<body>
    <div class="city_life">
        <img src="/SocialDataFinalProject/site_content/SF.gif" class="back-gif" alt="Messy">
    </div>
    <h1 class="page-title">{{ page.title }}</h1>
    <p style="color:white">A deep dive into the defilement of San Francisco</p>
    <br>
    <br>
    <h2>Introduction</h2>
    <div>
        <p>
            For the outside world San Francisco is a city that is known for its beautiful scenery, iconic landmarks and its unique Victorian architecture. The Golden Gate Bridge, Alcatraz Island, the Painted Ladies and the cable cars are just some of the many attractions that the city has to offer.
        </p>
    </div>
    <div class="column">
        <h4 align="center"> The Golden Gate Bridge </h4>
        <img src="/SocialDataFinalProject/site_content/goldengate.jpg" alt="bridge" width="425" height="200">
    </div>
    <div class="column">
        <h4 align="center"> The Painted Ladies (Alamo Square) </h4>
        <img src="/SocialDataFinalProject/site_content/postcardRow.png" alt="houses" width="360" height="200">
        <br>
    </div>
    <div> 
    <p>
        However, underneath the surface San Francisco is a city that has been facing significant challenges in recent years. One of the most significant issues is the cleanliness of its streets. Keeping cities clean and safe is one of the most important and essential factors for the well-being of both residents and visitors.  Studies have shown that cleanliness of a city plays a critical role in maintaining the <a href="https://www.epowertrucks.co.uk/news/how-dirty-streets-are-affecting-the-environment-and-property-values-in-your-area/" target="_blank">public health</a> [1], promoting tourism and creating a safe and comfortable environment for everyone. On the other hand, when a city is dirty and filled with trash and waste, it negatively impacts the quality of life for all parties involved.
        San Francisco is a city that has faced significant challenges regarding the cleanliness of its streets. They are often littered with loose garbage, bulky items, needles and even human faeces, which is both repulsive and unhealthy. Major news outlets in San Francisco, such as <a href="https://abc7news.com/sf-tourism-san-francisco-streets-international-travelers-conventions-in/12227886/" target="_blank"> ABC News</a> [2] and the <a href="https://www.sfchronicle.com/opinion/letterstotheeditor/article/sf-streets-are-not-safer-or-cleaner-17596059.php" target="_blank"> San Francisco Chronicle</a> [3], reported multiple stories around 2018 that highlighted this crucial problem. This has also given rise to Mayor London Breed to incorporate the "Clean Streets"-agenda into her <a href="https://londonformayor.com/policies/clean-streets-clean-city-2/" target="_blank">main campaign</a> [4].
        Given the significant issue of dirtiness in San Francisco and its ongoing discussion and seriousness, this report aims at contributing to the understanding of the problem by analysing the government of San Francisco’s dataset (<a href="https://data.sfgov.org/City-Infrastructure/311-Cases/vw6y-z8j6" target="_blank">3-1-1 Cases</a>) of cases associated with Street Cleaning requests in the city.
        <br>
        In this way, we hypothesize that our report sheds light on especially two main issues: 
        <ol type='1'>
            <li>
                Given the stories reported in 2018, are the dirty streets still a prevalent issue today in San Francisco? And if so what are some of the main reasons for and contributors to this?
            </li>
            <li>
                News articles often focuses their attention to specific areas of the city. This project, however, also aims at elucidating if the problem is present throughout the city. In this way, we can answer if there are any specific areas that are more affected by the problem than others. And if so, what are the main reasons for this?
            </li>
        </ol>
    </p>
    <h2>Our Dataset</h2>
    <p>
        The dataset used for this project is the 311 Cases dataset made publicly available by the city's 311 Customer Service Center. The dataset contains non-emergency requests for service made by residents and visitors of San Francisco to the 311 Customer Service Center via  <a href="https://sf311.org/" target="_blank">phone calls, online submissions</a> [5] or mobile apps. The request types cover a wide range of issues, such as street and sidewalk cleaning, graffiti, abandoned vehicles and noise complaints. The dataset contains detailed information about each request, such as the date and time it was made, the location, the nature of the problem, and the status of the problem. The dataset is regularly updated to include the newest requests made, however we do not consider request made after the 30th of April. 
        <br>
        <br>
        The full dataset contains over 6 million requests made from 2008 to 2023, but since we focus on the Street and Sidewalk cleaning requests the actual dataset of interest contains approximately 2 million requests. Due to the significant size of the dataset, we only include requests with a latitude and longitude position within the boundaries of San Francisco. Moreover, we made sure that request types are not duplicated, but instead sum up similar types to get a more accurate representation of the severeness of the type. This means that for example, we accumulate the request types "Human or Animal Waste" and "Human Waste" to get a more accurate representation of the number of requests regarding human waste. Lastly, we direct focus towards the 10 most frequent request types, which are hence also the types we deem most relevant for our analysis. We will refer to these as the main request types, and we will not consider tendencies in the other request types.
        <br>
        <br>
        For a more hands-on inspection of the creation of this report, we have composed all findings in an explainer notebook, that can be found <a href="https://nbviewer.org/github/notaiax/SocialDataFinalProject/blob/master/coding/explainer_notebook.ipynb" target="_blank">here</a>.
    </p>
    <h2>The Dirtier Side of San Francisco: Increasing Demand for Street Cleaning</h2>
    <p>
        In 2018, <a href="https://www.youtube.com/watch?v=VEOkX9dp85I&ab_channel=NBCBayArea" target="_blank">NBC Bay Area</a> [6] conducted a thorough analysis about the cleanliness of San Francisco’s streets. They concluded that the cleanliness of San Francisco’s streets had deteriorated over time, and especially more severe issues like needles and animal waste were contributing to an image of San Francisco comparable to slums in developing countries. In this section, we start by attempting to track the number of cleaning requests in San Francisco to see if San Francisco's dirtiness has improved or worsened over the years. Given the possibility through the vast amount of data, we will attempt to track the number of cleaning requests per year, and see if there is a trend in the number of requests, and why that might be the case.
        <br>
        <br>
        In Figure 1, we show the total number of street cleaning requests from 2008 to 2022. From the figure, one recognizes that the number of cleaning requests is clearly increasing over time. Observing increasing numbers year by year contributes to a trend that is troubling for the city. Just in 15 years the number of requests has increased by more than tenfold to nearly 300,000. This is a significant increase, and it is therefore interesting to investigate why this could be the case.
    </p>
    <div>
        <h3>Figure 1: San Francisco Street & Sidewalk Cleaning Requests</h3>
        <div class="center">
        <iframe src="/SocialDataFinalProject/assets/images/BarChartV2.html" width="100%" height="500"></iframe>
        </div>
    </div>
    <p>
        While we observe a significant increase in street cleaning requests from the citizens of San Francisco we must be wary in concluding that this can be solely attributed to the streets getting more and more dirty. The increase in requests is of course the principal proxy for dirty streets, but other factors such as the population growth of San Francisco might also affect the tendency. However, The San Francisco Standard recently reported a decline in the population from 2020 to 2022, which we would expect to observe in Figure 1, if the contribution of population estimates was significant <a href="https://sfstandard.com/research-data/san-francisco-bay-area-california-population-decline-census-pandemic-covid/" target="_blank">[7]</a>. Nonetheless, factors such as technology adoption, 311 service awareness, and many others must also be considered as contributing factors to the trend. 
        <br>
        In particular, it is interesting to reflect on the fact that in 2008 the iPhone was introduced only 6 months earlier, and the first Android phone was not released until 2009. Fast-forward to today where almost every citizen has a smartphone, and it is much easier to report issues to the 311 Customer Service Center <a href="https://www.statista.com/statistics/201182/forecast-of-smartphone-users-in-the-us/" target="_blank">[8]</a>. This could be a contributing factor to the increase in requests, but it is difficult to quantify the effect of this. This and many other factors as mentioned above are interesting to investigate. Nevertheless, by visually inspecting request tickets we can still get a good idea of the severity of the problem. 
        <br>
        <br>
        We do this in Figure 2, where we show a slideshow of images depicting some of the reported cases. This demonstrates that not all cases are frivolous, and implies that San Francisco does indeed face a severe problem with dirty streets. One could for example imagine the rareness of such occurences in a city such as Copenhagen, which has a very efficient waste management system.
    </p>
    <div>
        <h3>Figure 2: Examples of Requested Cleaning</h3>
        <embed 
            type="text/html" 
            src="/SocialDataFinalProject/site_content/slideshow.html"
            width="1050"
            height="520"
            >
    </div>
    <h2>From Needles to Christmas Trees: Decoding San Francisco's Dirty Secrets</h2>
    <p>
        So, we now know that the defilement of San Francisco has increased steadily every year from 2008 to the present time, which shows an unpleasant trend of a city in trouble. Nevertheless, just having an increase in citizen requests can not explain the whole story. As explained above multiple factors are contributing to the increase, but looking into how this increase takes place is another point of analysis that is extremely interesting. What types of requests are most significant, and how do the specific tendencies for each of these look? Are parts of the city more affected by the increase than others, and if so which and why? By answering questions like these it is possible to notice specific patterns that might explain how the City of San Francisco are handling the increase, and maybe catch sight of efforts to decrease specific categories.
        <br>
        <br>
        In Figure 3 below, tendency shows that the larger categories have been a growing issue at least since 2008, when data started being collected. A pattern that stands out is that of the Christmas trees, that only get requested after Christmas - logically making sense. However, this pattern contrasts with Loose Garbage and Debris which has a decrease in its common pattern that matches the christmas tree category. This might be due to the fact that the request type Christmas Trees was first introduced here, and hence the requests about christmas trees on the streets that were earlier categorized as Loose Garbage and Debris are now categorized as Christmas Trees.
        <br>
        <br>
        Another interesting insight we gain from Figure 3 is related to the Human or Animal Waste and Needles categories. Right around 2018 where NBC Bay Area and other news outlets drew attention to the issue of dirty streets, we see a break and decrease in the requests related to these categories. This observation coincides with the reportings of specific measures being taken into action regarding the clean up of specifically these two somewhat more unpleasant categories <a href="https://www.sfchronicle.com/bayarea/article/SF-to-get-team-dedicated-to-clearing-used-needles-12858548.php" target="_blank">[9]</a><a href="https://www.sfaf.org/collections/status/getting-syringes-off-san-francisco-streets/" target="_blank">[10]</a>. This is a positive sign that the city is taking action to improve the situation, and it is interesting to see if this trend continues in the future.
    </p>
    <div>
        <h3>Figure 3: Trends in San Francisco Street Cleaning Requests by Category (2008-2023)</h3>
        <embed 
            type="text/html" 
            src="/SocialDataFinalProject/assets/images/timeSeriesPlot.html"
            width="1025"
            height="550"
            >
    </div>
    <p>
        In a majority of the stories covering the dirty streets of San Francisco news outlets tend to focus their attention to only a few districts. In particular the Tenderloin district is often mentioned as a district with a severe problem. Nevertheless, as mentioned in the introduction this project aims at achieving a more general understanding of the problem, and therefore we will look at the problem from a complete district-level perspective. 
        <br>
        <br>
        In Figure 4, we show the number of requests per district per year. From this figure, we quickly observe that throughout practically all years the Mission district stands out. This is not surprising as the Mission district is both one of the most populated districts and also one of the districts with the highest homeless population. 
        <br>
        <br>
        On the other hand, a suprising insight is that the Tenderloin and South of Market districts seem to be catching up with the dirty streets. In the years from approximately 2008 to 2019 these districts get as severe a number of requests as the Mission district. However, this has not been the case since 2019. This is contrary to what we would expect, as the Tenderloin and South of Market districts are often mentioned in the stories referenced among the most problematic districts. At first glance a positive sign, but a possible explanation could be that during the COVID-19 pandemic reportings in these areas have been less frequent as it coincides with the time where the pandemic hit the hardest. Nevertheless, this is just a hypothesis that could be investigated further, but is outside the scope of this report. On the other hand, another possible explanation is that the notable increase in the number of requests in the Mission district during the same period suggests a significant shift of requests towards that area. In other words, this implies that the problem may not have been resolved but rather relocated.
    </p>
    <div>
        <h3>Figure 4: A Yearly District-Level Perspective on Street Cleaning Requests</h3>
        <embed 
            type="text/html" 
            src="/SocialDataFinalProject/assets/images/SF_mapYearlyV2.html"
            width="1050"
            height="725"
            >
    </div>
    <h2>Mission, South of Market and Tenderloin: A Trifecta of Trouble</h2>
    <p>
        Even though Figure 4 showed signs of a Tenderloin and South of Market in progress, it is still interesting to look at the three districts in more detail as the three districts are often the center of attention for many negative stories about the city. Recently (February 2023) <a href="https://www.cbsnews.com/sanfrancisco/news/surging-crime-dirty-streets-local-residents-say-san-franciscos-mission-district-is-in-crisis/" target="_blank">CBS News</a> [11] reported a story about a business owner in the Mission district debating the surging crimes and dirty streets. While in 2022 <a href="https://www.sfchronicle.com/bayarea/article/sf-mission-tents-17037918.php" target="_blank">San Francisco Chronicle</a> [12] ran a story about how Mission is turning into a worse version of the notorious Tenderloin. It is therefore of interest to look more into these districts, and see if we can find any patterns that might explain why these districts are often mentioned, and more importantly whether the districts are in fact rightfully considered a trifecta of trouble.
        <br>
        <br>
        To answer this, we employ a second dataset that we can use to support the analysis. This dataset is the San Francisco Police Department Incident Reports dataset, which contains information about all the incidents reported to the San Francisco Police Department from 2003 to present. The dataset contains information about the type of incident, the district, the date and time of the incident, and the location of the incident <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry" target="_blank">[13]</a><a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783" target="_blank">[14]</a>. By utilizing this dataset we can get a better understanding of the incidents that occur in the three districts, and see if there are any patterns that might explain why these districts are often mentioned. We therefore show a similar figure as Figure 4, but instead of showing the number of street cleaning requests, we show the number of crime incidents reported to the San Francisco Police Department in Figure 5.
        <br>
        <br>
        From Figure 5, we observe that the Mission district is still the district with the most incidents reported to the San Francisco Police Department. Moreover, we also observe that the Tenderloin and South of Market districts are not far behind. Hence, it seems that the three districts are indeed a trifecta of trouble, when we consider crime and street cleaning data. It is interesting to see that the correlation between crime incidents and street cleaning request is so strong. It shows a worrying sign that such populated and central areas of a city like San Francisco are the home of such a high number of crime incidents and street cleaning requests. Yet, it is well known that crime and poverty are closely related, and the three districts are also among the poorest districts in San Francisco, so the correlation between the two datasets might not be that surprising. But why is this the case? And what measures should the city take to solve the problem? Answering questions like these requires a more in-depth analysis that also includes social data about the demographics of the districts and other related factors that can help explain the problem. As mentioned related to Figure 4, the Mission district is widely known for its high homeless population, and this might be a factor that can help explain the problem. However, getting a more detailed answer to these questions is outside the scope of this report, but is definitely something that could be investigated further.
    </p>
    <div>
        <h3>Figure 5: A Yearly District-Level Perspective on Crimes in San Francisco</h3>
        <embed 
            type="text/html" 
            src="/SocialDataFinalProject/assets/images/SF_CrimemapYearlyV2.html"
            width="1050"
            height="725"
            >
    </div>
    <h2>Concluding Thoughts</h2>
    <p>
        From our comprehensive analysis of street cleanliness in San Francisco, several key takeaways emerge. Firstly, it is evident that San Francisco has been grappling with cleanliness issues over the years, with the number of cleaning requests increasing significantly from 2008 to 2023. This upward trend suggests that San Francisco's streets are becoming progressively dirtier, affecting the city's image and quality of life for its residents. Hence, confirming that the analysis put out by the NBC Bay Area is still valid, as well as our first hypothesis.
        <br>
        Nevertheless, the rise in street cleaning requests may not entirely indicate an increase in dirtiness. Other factors such as technological advancements, population growth, and awareness of the 311 service could also contribute to this surge. While San Francisco's grimy streets are a pressing issue, it is essential to consider these underlying factors when interpreting the data.
        <br>
        <br>
        The dirty streets are still a prevalent issue today in San Francisco. However, when examining the types of cleanliness complaints, we notice a decrease in requests related to "Human or Animal Waste" and "Needles" around 2018, coinciding with the city's efforts to tackle these specific problems. This positive trend might suggest the city's actions are yielding results and should be sustained.
        <br>
        The data also reveals a geographically uneven distribution of cleanliness issues, with districts like Mission, Tenderloin, and South of Market being most affected. Yet, there seems to be a shift in cleanliness complaints from Tenderloin and South of Market to the Mission district in recent years, suggesting that the problem might be moving rather than resolving.
        <br>
        <br>
        We also observe that a strong correlation exists between areas with high cleaning requests and crime incidents. Mission, Tenderloin, and South of Market, often highlighted as problematic areas, indeed exhibit a high number of both cleaning requests and crime incidents. This correlation, although not surprising considering these areas' socioeconomic status, deserves deeper investigation. Nonetheless, this also confirms the second hypothesis that the city's cleanliness is very much focused on a specific area of the city.
        <br>
        Looking forward, the findings from this report offer several potential directions for further research and action. One clear area is to delve deeper into the reasons behind the geographical shift of cleanliness complaints. Another is to investigate the strong correlation between cleaning requests and crime incidents and the potential underlying socioeconomic factors. Understanding these aspects could provide valuable insights into formulating effective strategies to improve the cleanliness of San Francisco's streets. A potential solution may lie in studying and adopting strategies from cities like Los Angeles, known for its more efficient trash collection programs in terms of money spent per collected trash.
        <br>
        <br>
        As the city grapples with these challenges, it is crucial for residents and visitors to be mindful of the situation, especially when navigating the "trifecta of trouble". Until comprehensive solutions are implemented, the people must be vigilant and proactive in maintaining cleanliness in their neighborhoods.
    </p>
    <a id="references" style="color:inherit; text-decoration: none !important;"><h2>References</h2></a>
    <ol type="1">
        <li>
            <a href="https://www.epowertrucks.co.uk/news/how-dirty-streets-are-affecting-the-environment-and-property-values-in-your-area/" target="_blank"> How Dirty Streets Are Affecting The Environment And Property Values In Your Area </a>
        </li>
        <li>
            <a href="https://abc7news.com/sf-tourism-san-francisco-streets-international-travelers-conventions-in/12227886/" target="_blank"> ABC News article: SF's "dirty streets" hurting international tourism as conventions struggle to come back </a>
        </li>
        <li>
            <a href="https://www.sfchronicle.com/opinion/letterstotheeditor/article/sf-streets-are-not-safer-or-cleaner-17596059.php" target="_blank"> SF Chronicle: Letters: Why Mayor Breed’s efforts aren’t making S.F. streets safer or cleaner </a>
        </li>
        <li>
            <a href="https://londonformayor.com/policies/clean-streets-clean-city-2/" target="_blank"> Mayor Breed: Clean Streets, Clean City </a>
        </li>
        <li>
            <a href="https://sf311.org/" target="_blank"> SF 311 </a>
        </li>
        <li>
            <a href="https://www.youtube.com/watch?v=VEOkX9dp85I&ab_channel=NBCBayArea" target="_blank">NBC Bay Area: Behind the Story: Walking San Francisco's Dirty Streets</a>
        </li>
        <li>
            <a href="https://sfstandard.com/research-data/san-francisco-bay-area-california-population-decline-census-pandemic-covid/" target="_blank">The SF Standard: It’s Official: A Quarter Million People Fled the Bay Area Since Covid</a>
        </li>
        <li>
            <a href="https://www.statista.com/statistics/201182/forecast-of-smartphone-users-in-the-us/" target="_blank">US Smartphone Users 2009-2040</a>
        </li>
        <li>
            <a href="https://www.sfchronicle.com/bayarea/article/SF-to-get-team-dedicated-to-clearing-used-needles-12858548.php" target="_blank">SF Chronicle: SF to get team dedicated to clearing used needles from city’s streets</a>
        </li>
        <li>
            <a href="https://www.sfaf.org/collections/status/getting-syringes-off-san-francisco-streets/" target="_blank">SF Aids Foundation: Getting syringes off San Francisco streets</a>
        </li>
        <li>
            <a href="https://www.cbsnews.com/sanfrancisco/news/surging-crime-dirty-streets-local-residents-say-san-franciscos-mission-district-is-in-crisis/" target="_blank">CBS News: Surging crime, dirty streets; Local residents say San Francisco's Mission District is in crisis</a>
        </li>
        <li>
            <a href="https://www.sfchronicle.com/bayarea/article/sf-mission-tents-17037918.php" target="_blank">SF Chronicle: ‘A neighborhood in chaos’: Is the Mission following in the Tenderloin’s footsteps?</a>
        </li>
        <li>
            <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry" target="_blank">San Francisco Police Department Crime Incident Report from 2003-2018</a>
        </li>
        <li>
            <a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783" target="_blank">San Francisco Police Department Crime Incident Report from 2018 to present</a>
        </li>
    </ol>
    <footer>
        <p>
            Click the link below to get a walkthrough of our data processing.
            <br>
            <a href="https://nbviewer.org/github/notaiax/SocialDataFinalProject/blob/master/coding/explainer_notebook.ipynb" target="_blank">NBViewer</a>
            <br>
            <a href="https://github.com/GustavHansen99/SocialDataFinalProject/" target="_blank">Github Repository</a>
        </p>
    </footer>