***Rats in New York City***

*What I aimed to accomplish*: 
In the street of my accommodation in South Harlem, I often see many rats searching for food in the trash bags left outside when I walk around. I found out that there is a dataset on rat sightings from NYC 311's system. So, I wanted to learn more about the rats in NYC. How big is the rat problem? And where do rats live, or where do they like to stay? Are there any patterns?

*Findings*: 
After analyzing the dataset, cleaning and merging rows and columns to combine population data with rat sightings into a dataframe, I created several graphs. This revealed matching geographic patterns between reported rat sightings, New York's subway lines, and sidewalk trash reports. Additionally, I found that rat sightings in the city have increased significantly since the pandemic began in 2019.

*Data collection*: 
The three main datasets I used are:
  - rat_sightings_20240701.csv: # <a href="https://data.cityofnewyork.us/Social-Services/Rat-Sightings/3q43-55fe/about_data">reported rat sightings to NYC's 311 system</a> from 2010 until the end of june 2024
  - dirty-condition-2023.csv: # <a href="https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9/about_data">reported dirty conditions</a> with descriptor «trash» to NYC's 311 system in 2023
  - population-nyc-2022.csv: # population of nyc in 2020 by zip code/borough from <a href="https://censusreporter.org/data/table/?table=B01003&geo_ids=04000US36,140|04000US36,860|04000US36&primary_geo_id=04000US36#">U.S. census</a>

*Data analysis*: 
I analyzed the datasets using Python and pandas. To create different dataframes, I cleaned, merged, and filtered the data, which provided a quick overview. By plotting the data with simple graphics, I uncovered some interesting patterns. After selecting the data I wanted to visualize, I exported the specific dataframes as CSV or GeoJSON files using Python. Then, I prepared the data in Google Sheets for Datawrapper. For the maps, I imported the GeoJSON files into QGIS for further editing. Finally, I exported the maps from QGIS as SVG files and make them prettier in Illustrator and to add annotations for a scrollytelling piece with ai2html.

*Summary, Challenges, Skills*: 
I struggled with finding a focus and interesting angle for a story. This is probably one of the challenges when you start with a dataset first and then try to find a story. After analyzing the datasets, I created many charts, which I eventually skipped or removed from my story because they no longer fit to the storyline. For example, I made a nice chart showing the rat sightings per 10,000 residents for each zip code in New York City. For this chart, I spent a long time searching for the right population data at the zip code level and had difficulty merging it with the rat sightings data frame in Python. Despite the effort, I discarded the chart in the end. Using a choropleth map and multiple heatmaps for the same story was overwhelming, so I decided to go with the heatmaps because I wanted to practice QGIS and try out a scrollytelling piece. It was a challenge to use the scrollytelling template before we covered it in class. Additionally, there was a bug in Soma's template that prevented it from displaying resized images for mobile devices. Finding the bug in 1,000 lines of code took some time.

With this project, I improved my Python skills for data analysis, learned more about working with QGIS, and successfully created a scrollytelling piece.
