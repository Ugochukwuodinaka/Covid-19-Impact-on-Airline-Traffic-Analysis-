# Covid-19-Impact-on-Airline-Traffic-Analysis-(2020)
![](Covid-19_Impact_on_Airport_Traffic_image.jpg)

## Project Overview
### Introduction:
The outbreak of the Covid-19 pandemic in 2020 led to unprecedented disruptions across various sectors, with the airline industry being one of the hardest-hit. This project aims to analyze the impact of the Covid-19 pandemic on global airline traffic patterns during the year 2020. By leveraging data analysis techniques, we seek to gain insights into how travel restrictions, lockdown measures, and public health concerns affected air travel behavior worldwide.

### Problem Statement:
The outbreak of the Covid-19 pandemic in 2020 has severely impacted the global airline industry, leading to unprecedented disruptions in air travel patterns. As countries implemented various containment measures, including travel restrictions and lockdowns, airline traffic experienced significant fluctuations, with profound implications for airlines, airports, and related stakeholders. However, there remains a critical need to systematically analyze the extent and nature of these disruptions, understand the underlying factors driving changes in airline traffic behavior, and identify actionable insights to inform future strategies and policies. This analysis project focuses on 4 countries which are: The Unuted States of America (USA), Canada, Australia and Chile.

This project seeks to address the following key questions:

- What is the total flight recorded for this analysis?
- What is the total traffic impact?
- What is the average percent of baseline?
- What is the total flights recorded by Country?
- What is the number of Airports, Countries and Cities in this analysis?
- What is the overall traffic impact by Country? Use a chart.
- With the help of a chart, display the flights trend monthly was recorded within the period of this analysis?
- Using a chart, show the contributions of different Airports to the overall traffic impact?
- Using geospatial mapping, showcase the percentage of baseline by Airport, Country, Stae and City?
- What actionable insights can be derived from the analysis to assist stakeholders in the aviation industry and policymakers in adapting strategies and mitigating future risks associated with similar crises?

### Expected Outcomes:

- Total Flight Recorded: The analysis will provide the total number of flights recorded within the specified period, offering a comprehensive view of the scale of air traffic during the time frame under consideration.

- Total Traffic Impact: By comparing pre-pandemic levels of air traffic with those during the pandemic period, the analysis will quantify the total impact on air traffic, providing insights into the severity of disruptions experienced by the airline industry.

- Average Percent of Baseline: Calculating the average percentage of baseline traffic will offer a standardized measure to gauge the overall reduction in air travel activity relative to pre-pandemic levels.

- Total Flights Recorded by Country: This outcome will present a breakdown of the total number of flights recorded for each country, enabling a comparative analysis of the impact across different regions.

- Number of Airports, Countries, and Cities: Providing counts of airports, countries, and cities included in the analysis will offer contextual information about the scope and geographic coverage of the dataset.

- Overall Traffic Impact by Country (Chart): A chart depicting the overall traffic impact by country will visually illustrate the varying degrees of disruption experienced across different countries.

- Monthly Flight Trend (Chart): Visualizing the monthly flight trend will enable stakeholders to identify temporal patterns and fluctuations in air travel activity over the course of the analysis period.

- Contributions of Different Airports (Chart): Displaying the contributions of different airports to the overall traffic impact will highlight the relative importance of various air transportation hubs in shaping the overall traffic patterns.

- Geospatial Mapping of Baseline Percentage: Using geospatial mapping, the analysis will showcase the percentage of baseline traffic by airport, country, state, and city, offering a spatial perspective on the distribution of air traffic disruptions.

- Actionable Insights: Drawing from the analysis results, actionable insights will be derived to assist stakeholders in the aviation industry and policymakers in adapting strategies and mitigating future risks associated with similar crises. These insights may include recommendations for route optimization, capacity planning, health and safety protocols, policy adjustments, and crisis management strategies.

### About The Dataset
This dataset shows traffic to and from the Airport as a Percentage of the Traffic volume during the baseline period. The baseline period used for computing this metric is from 1st Feb to 15th March 2020. The dataset gets updated monthly. This data is publicly available from [Geotab](https://www.geotab.com/). The dataset is in .csv file and can be viewed or downloaded [here](covid_impact_on_airport_traffic.csv)

The dataset is made up of 11 columns and 7,248 rows of data. Here is a breakdown of the column details:

- AggregationMethod: This column indicates the method used for aggregating or summarizing the data. Here, the data is aggregated on a daily basis.
  
- Date: This column represents the date for which the data is recorded. It typically follows a standardized date format (e.g., YYYY-MM-DD) and indicates the specific time point or period to which each data entry corresponds.

- Version: This column denotes the version or iteration of the dataset. It may indicate updates, revisions, or modifications made to the dataset over time, allowing users to track changes and ensure data integrity.

- AirportName: This column contains the name or identifier of the airport associated with each data entry. It identifies the specific airport location to which the data pertains, facilitating analysis and interpretation based on geographic context.

- PercentOfBaseline: This column provides a measure of the percentage deviation from a baseline value. In the context of airline traffic data, it represents the percentage of normal or pre-pandemic levels of air traffic for each observation, indicating the extent of disruption or recovery in air travel activity.

- Centroid: This column contain geographical coordinates (latitude and longitude) representing the central point or centroid of the airport location. It enables spatial analysis and visualization, allowing users to map and analyze data based on airport locations.

- City: This column specifies the city or urban area associated with each airport. It provides additional geographic information to complement the airport name, helping users identify the location of airports within specific cities or metropolitan areas.

- State: This column indicates the state or province (if applicable) where the airport is located. It further refines the geographical context of each airport, particularly in countries with administrative divisions such as the United States, Canada, or Australia.

- ISO_3166_2: This column contain the ISO 3166-2 code corresponding to the state or province where the airport is located. ISO 3166-2 is a standardized coding system used to represent country subdivisions, facilitating data interoperability and cross-referencing with other datasets.

- Country: This column specifies the country where the airport is situated. It provides the highest level of geographical context for each data entry, enabling analysis and comparison of data across different countries or regions.

- Geography: This column contain additional geographical information or descriptors related to each airport location. It could include details such as geographical regions, continents, or other spatial attributes that help classify and organize airport locations within a broader geographic framework.

### Tools Used
1. Power Query Editor
    - Was used to:
        1. Extract,
        2. Transform, and
        3. Load all the datasets for this analysis.
           
2. Power BI (Was used to create reports and dashboard for this analysis)
    - The following Power BI Features were incorporated:
        1. DAX,
        2. Quick Measures,
        3. Page Navigation,
        4. Filters,
        5. Tooltips

### ETL Process using the Power Query Editor:
1. Ttranslated all the colume headers in Swedish language to English for easy understanding
2. Duplicated the Centroid column into 2 more columns: "Centroid 1" and "Centroid 2"
3. Split the duplicated Centroid columns by delimeter.
4. Split the duplicated Centroid columns by position.
5. Changed the Centroid 1 and Centroid 2 datra types to 'text'.
6. Changed their column names to Longitude and Latitude.
7. Changed the Date column type to 'date'.
8. Made sure there is no null values or missing data.

**Raw Data**
![](Raw_Data.png)

**Final query editor screenshot**

![](Power_Query_Eitor_1.png)

## Visuals in Power BI:
![](Covid-19_Impact_On_Airport_Traffic_Analysis(2020)_Dashboard.jpg)

#### Analysis:
From the analysis, i made the findings below:
- The Total Flight Record is 7,247.
- The Average Percentage of Baselie is 66.65%.
- The total number of Airports is 28.
- The Total Traffic Impact is 483,000.
- Total Number of Airport Countries in this analysis is 4
- While the Total Number of Airport Cities is 27.
- Looking at the Total flights recorded by the 4 countries in this analysis, USA had the most number of flights which was 4,441, followed by Canada with 2,311 flights, Australia is next with 57 flights, and lastly, Chile with 238 flights. As we can see, there are variations in these numbers by countries. Let's run a more detailed analysis on them:
     1. Both the USA and Canada have larger populations and more extensive aviation industries compared to Australia and Chile. This inherently leads to higher levels of air travel 
        activity in these countries, irrespective of external factors.

     2. International Travel Hubs: Major cities in the USA and Canada, such as New York, Los Angeles, Toronto, and Vancouver, are significant international travel hubs. They attract a 
        large volume of passengers and facilitate numerous flight connections, contributing to higher overall flight numbers.

     3. Economic Activity and Business Travel: The USA and Canada are home to numerous multinational corporations and have strong economies. This results in substantial business travel 
        activity, which translates to higher demand for flights, particularly between major business centers and corporate hubs.

     4. Geopolitical Factors: The geographical proximity of the USA and Canada to other major global destinations, as well as their political and economic ties with various countries, 
        can influence the volume of international flights operating to and from these countries.

     5. However, it's important to note that the significant disparity in flight numbers between the USA and Canada compared to Australia and Chile during the early part of 2020 can 
        also be attributed to the onset of the Covid-19 pandemic. By January 2020, the Covid-19 outbreak had begun to spread globally, leading to widespread travel restrictions, border 
        closures, and a decline in passenger demand for air travel.

     6. As a result, the USA and Canada, being more connected to global travel networks and having larger aviation industries, likely experienced a higher volume of flights in the early 
        part of 2020 compared to Australia and Chile. However, as the severity of the pandemic increased and travel restrictions intensified, all countries would have seen significant 
        reductions in flight numbers compared to previous years.
     7. Generally, compared to the previous years, these 4 countries experienced lesser flight schedules, due flight restrictions that happened in 2020 due to the destructive impact of 
        the covid-19 pandemic not just in these 4 countries in this analysis, but globally.

- In the context of this analysis, the term "overall traffic impact" refers to the net change or deviation in air traffic activity compared to a baseline or reference period. The specific numbers associated with each country represent the magnitude of this impact, measured in some standardized unit (such as flight counts for this analysis) that allows for comparison across different regions or time periods.

     1. USA: With an overall traffic impact of 286,271, this indicates a substantial net change in air traffic activity within the United States during the specified period. The 
        positive value suggests an increase in air traffic relative to the baseline, while a negative value would imply a decrease.

     2. Canada: Similarly, Canada's overall traffic impact of 178,893 reflects the net change in air traffic activity within Canada during the analyzed period. Again, a positive value 
        indicates an increase in air traffic, while a negative value would signify a decrease.

     3. Australia: Australia's overall traffic impact of 9,702 indicates a comparatively smaller net change in air traffic activity within Australia during the specified period.

     4. Chile: Chile's overall traffic impact of 8,157 represents the net change in air traffic activity within Chile during the analyzed period.

     5. These values provide quantitative insights into how the Covid-19 pandemic, or other factors under consideration, affected air traffic patterns in each country. A higher overall 
        traffic impact suggests a more significant deviation from normal or baseline levels of air traffic, while a lower impact indicates a relatively smaller deviation.

- In the Flight Trend by Month linechart, it is evident that there are fluctuations in air travel activity throughout the year, with certain months experiencing higher or lower percentages relative to a baseline reference point. Below is an analysis of these trends:

     1. Initial Impact of Covid-19 Pandemic (March to May): The percentage of baseline in March is 445, indicating a significant decline in air travel activity compared to pre-pandemic 
        levels. This decline likely corresponds to the initial onset of the Covid-19 pandemic, as countries implemented widespread travel restrictions and lockdown measures to contain 
        the spread of the virus. In April and May, although still significantly below baseline levels, there is a gradual increase in the percentage of baseline (825 and 855, 
        respectively), suggesting a partial recovery or stabilization in air travel activity as some restrictions were lifted and travel began to resume cautiously.

     2. Summer Recovery (June to August): From June to August, there is a further increase in the percentage of baseline, indicating a continued recovery in air travel activity during 
        the summer months. The percentages range from 831 to 862, reflecting a gradual return to normalcy as travel restrictions eased, and consumer confidence in air travel began to 
        improve.

     3. Plateau and Fluctuations (September to November): In September and October, the percentage of baseline remains relatively stable, hovering around 835 to 868, suggesting a 
        plateau in air travel activity. However, there may be fluctuations within this period due to factors such as changing travel regulations, economic conditions, and regional 
        outbreaks of Covid-19. By November, there is a slight decrease in the percentage of baseline to 835, indicating a potential stabilization or modest decline in air travel 
        activity compared to the previous months.

     4. Year-End Decline (December): The percentage of baseline drops significantly in December to 56, indicating a sharp decline in air travel activity compared to the rest of the 
        year. This decline may be attributed to various factors, including holiday travel disruptions, increased Covid-19 cases and restrictions, and seasonal trends in air travel 
        demand.

     5. Overall, the analysis of flight trends by month highlights the dynamic nature of air travel activity throughout the year, with fluctuations influenced by external factors such 
        as the Covid-19 pandemic, government policies, economic conditions, and seasonal variations. 










