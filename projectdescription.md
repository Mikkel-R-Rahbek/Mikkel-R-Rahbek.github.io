---
layout: page
title: Project description
permalink: /projectdescription/
---
<html>
<head>
	<title>projectdescription</title>
	<style>
    .centered-image {
    display: block;
    margin: 0 auto;
    }
    h2 {
    margin-bottom: -15px;
    } 
    h3 {
    margin-bottom: -15px;
    } 
    p {
    margin-top: 10px;
    }
  </style>
</head>
<body>
  <h1 class="page-heading">{{ page.title }}</h1>
  <div>
    <h2> Initial idea - Carbon Emissions of buildings in San Francisco </h2>
        <h3> Data </h3>
        <p> 
            The initial idea of the final project in Social Data Analysis and Visualization was to investigate the carbon emissions of buildings in San Francisco based on the data from the San Francisco Energy Benchmarking Ordinance. The data set contains information about the energy use and carbon emissions of buildings in San Francisco, and is available on the <a href="https://data.sfgov.org/Energy-and-Environment/Existing-Buildings-Energy-Performance-Ordinance-Re/j2j3-acqj"> San Francisco Open Data Portal. </a> This dataset presents basic information about energy use and implications (estimated greenhouse gas emissions, gas use, electricity use, and district steam use); and compliance status for private-sector (non-municipal) properties and contain data last updated in February 2023.
        </p>
        <h3> What and how? </h3>
        <p> 
            Based on the data set, the initial idea was to investigate the carbon emissions of buildings in San Francisco, and to investigate whether there is a correlation between the carbon emissions and the age of the buildings. The idea was to visualize the data in a map of San Francisco, where the buildings would be colored according to their carbon emissions. The map would also contain a slider, where the user could choose a specific year, and the map would then show the carbon emissions of the buildings in that year.
            More concretely, we created the project A assignment from this idea, and hence it can be seen described more thoroughly in the video below. (Please excuse the rapid speech, we were trying to fit it into the 1 minute ;) )
        </p>
        </div>
        <p align="center">
        <iframe width="420" height="315"
            src="https://www.youtube.com/embed/R6TtLWJrg6w?controls=0">
        </iframe>
        </p>
        <p> 
            However, we have decided not to follow through on this idea. We identified that the project would eventually lead to the inevitable conclusion that older buildings emit more carbon than newer buildings, and that this would not be a very interesting conclusion. Therefore, we spent time trying to enhance the dataset with additional building information or demographics about the different neighoborhoods in San Francisco. This was possible, but then we identified that the building dataset was very narrowly focused on buildings in the busy neighborhoods of San Francisco, and that the dataset did not contain information about the buildings in the more rural areas of San Francisco. These thoughts and issues ultimately led us to believe that another project would be more challenging and interesting to investigate.
        </p>
  <h2> Project Idea 2.0 - 3-1-1 Cases in San Francisco </h2>
    <h3> Data </h3>
        <p> 
            Instead of the building emissions dataset, we have chosen to focus our attention towards the extremely interesting dataset of 3-1-1 cases in San Francisco. 3-1-1 is an easy-to-remember telephone number that connects customers with highly-trained Customer Service Representatives ready to help you with non-emergency City and County of San Francisco government matters. Based on residents, businesses and tourists' calls to 3-1-1, the City and County of San Francisco has created a dataset of all the 3-1-1 cases in San Francisco. The dataset contains information about the type of case, the date of the case, the neighborhood of the case, the status of the case, and much more. The dataset is available on the <a href="https://data.sfgov.org/City-Infrastructure/311-Cases/vw6y-z8j6"> San Francisco Open Data Portal. </a> The dataset gets updated daily, and contains data from 2008 to the present. At present time (1st of May 2023) the data contain 6.11 million rows and 21 columns, where each row corresponds to a 3-1-1 case.
        </p>
    <h3> Idea for investigation </h3>
        <p>
            Keeping cities clean and safe is one of the most important and essential factors for the well-being of both residents and visitors.  Studies have shown that cleanliness of a city plays a critical role in maintaining the <a href="https://www.epowertrucks.co.uk/news/how-dirty-streets-are-affecting-the-environment-and-property-values-in-your-area/" target="_blank">public health</a> [1], promoting tourism and creating a safe and comfortable environment for everyone. On the other hand, when a city is dirty and filled with trash and waste, it negatively impacts the quality of life for all parties involved.
            <br>
            <br>
            San Francisco is a city that has faced significant challenges regarding the cleanliness of its streets. They are often littered with loose garbage, bulky items, needles and even human faeces, which is both repulsive and unhealthy. Major news outlets in San Francisco, such as <a href="https://abc7news.com/sf-tourism-san-francisco-streets-international-travelers-conventions-in/12227886/" target="_blank"> ABC News</a> [2] and the <a href="https://www.sfchronicle.com/opinion/letterstotheeditor/article/sf-streets-are-not-safer-or-cleaner-17596059.php" target="_blank"> San Francisco Chronicle</a> [3], reported multiple stories around 2018 that highlighted this crucial problem. This has also given rise to Mayor London Breed to incorporate the <a href="https://londonformayor.com/policies/clean-streets-clean-city-2/" target="_blank"> "Clean Streets"-agenda into her main campaign</a> [4].
            <br>
            Given the significant issue of dirtiness in San Francisco and its ongoing discussion and seriousness, this report aims at contributiong to the understanding of the problem by analysing the government of San Francisco’s dataset (<a href="https://data.sfgov.org/City-Infrastructure/311-Cases/vw6y-z8j6" target="_blank">3-1-1 Cases</a>) of cases associated with Street Cleaning requests in the city.
            <br>
            <br>
            <ol type='1'>
                <li>
                    Given the stories reported in 2018, are the dirty streets still a prevalent issue today in San Francisco? And if so what are some of the main reasons for and contributors to this?
                </li>
                <li>
                    News articles often focuses their attention to specific areas of the city. This project, however, also aims at elucidating if the problem is present throughout the city. In this way, we can answer if there are any specific areas that are more affected by the problem than others. And if so, what are the main reasons for this?
                </li>
            </ol>
        </p>
</body>
</html>


