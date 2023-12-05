<h1>GROUP 5 MIST 4610 Group Project 2</h1>

<h2>TEAM NAME:</h2>
29704 Group 5

<h2>Team Members:</h2>

1. Michael Hearnes [@michaelhearnes](https://github.com/mh101410)

2. Elton Hsieh [@eltonhsieh](https://github.com/ehsieh1)

3. Aidan Kane [@aidankane](https://github.com/aidanpatrickkane)

4. Mandy Larsen [@mandylarsen](https://github.com/awl25)

5. Zhengze Li [@Hwyqlzz](https://github.com/Hwyqlzz)

6. Nabeel Mohammed [@nabeelmohammed](https://github.com/nabeelmohd56)

<h2>Dataset Description:</h2>

The dataset we have chosen for analysis is the Motor Vehicle Collisions in New York City, found at the following link: https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes. Each row in the dataset details a crash reported to the NYPD using MV-104AN forms filed surrounding the crash. These forms are used for those collisions in which either major injuries/death occur or $1,000 in vehicle damage is done. The data dimensions collected in these forms include the date in mm/dd/yyyy and time in hh:mm of the crash, the borough of the crash (i.e. Brooklyn, Manhattan, etc.), zip code, latitude/longitude, the street on which the crash occurred, the cross street/off street (where applicable), number of injuries/deaths by category (number of pedestrians injured, number of cyclists killed, etc.), contributing factors to the crash, collision id (primary key), and the vehicle code (4 door sedan, truck, etc.). With regards to data types; boroughs, streets, vehicle code, location (latitude, longitude), and contributing factors are all of string data type; collision ID and number of deaths by category are int types, and zip code (int) and latitude/longitude (decimal) are loaded into Tableau assuming their respective geographic roles. One key thing to note about the original data is that there can be multiple categories of injuries/deaths, contributing factors, and vehicle codes (up to 5 each).

<h2>Question One:</h2>

**1. In 2022, How do the different numbers of traffic incidents and resulting deaths vary across different boroughs (Bronx, Brooklyn, Manhattan, Queens, Staten Island) in NYC during rush hours (9 AM and 5 PM), as visualized on a Tableau Coordinate Map?**
<h3>Importance & Relevance:</h3>

**Safety Insights:** This Tableau coordinate map helps determine which NYC boroughs are most impacted by vehicle-related deaths. By using the coordinate map to find trends within different areas of the city, public health programs and safety measures can be specifically targeted to areas in the most need. For example, Queens had the most deaths at 3.

**Guiding Policy Decisions:** This coordinate map can help NYC policymakers identify which locations and Burroughs need targeted traffic rules or better road safety infrastructure by providing a visual representation of the overall distribution of traffic incidents and fatalities in the most recently completed calendar year.

**Resource Allocation:** Reducing response times in high-risk locations may be achieved by strategically placing emergency response services, emergency rooms, and other traffic resources with the use of insights regarding the geographic distribution of vehicular accidents and related fatalities.

**Community Awareness:** The results may be utilized to change driving behavior in high-risk areas and to raise community awareness and overall knowledge about the value of traffic safety measures.

**Traffic Safety Measures Testing:** The information may prove useful in evaluating the performance of current traffic safety initiatives in various boroughs and pinpointing opportunities for enhancement.
<h3>Tie to the Dataset:</h3>

The dataset we chose is located at (https://catalog.data.gov/dataset/motor-vehicle-collisions-crashes) and is perfect for this kind of geographical analysis since it contains a thorough record of traffic accidents and deaths along with latitude and longitude coordinates. 

These incidents described- we displayed on a coordinate map, to highlight significant regional patterns and trends.

By filtering by different boroughs, our group can provide which areas of NYC need the most allocation of time and resources.

<h2>Question Two:</h2>

**2. What are the patterns in cyclist injuries in Brooklyn over different hours of the day?**

<h3>Importance and Relevance:</h3>

**Cycling Safety Assessment:** By finding the times of day when riders are most likely to get in an accident, this question aims to improve bike safety in Brooklyn. This information is essential for creating focused safety initiatives and marketing, by understanding key points in the data when riders are most at risk.

**Urban Planning:** Knowing when cyclists are most susceptible to crashes will help the future design of infrastructure, bike lanes, and riding routes that will be safer, particularly during hours of high-injury traffic.

**Public Awareness Campaigns:** By educating everyday bikers and drivers about the riskiest times to ride, the analysis can encourage safer and more cautious behavior.

**Policy Making:** The results of this analysis can help NYC’s  government design policies and enforcement laws and regulations that target periods of the day when cycling injuries are more common.

**Sustainable Transport Culture:** The analysis can support cycling as a sustainable means of transportation in urban environments like NYC by addressing safety concerns and improving safer riding conditions.

**Safety Insights:**  When relating to the objective of why the data was collected (Vision Zero), and the goal to eliminate all kinds of traffic accidents, when no filter is applied it shows that Brooklyn has the highest number of cyclists injured.  Although it can be chalked up to Brooklyn having the highest population, when compared to a borough of a similar size (Queens) it is obvious that Brooklyn is the biggest area of focus on improving bike-lane (which also brings into question pedestrian safety) safety.

**Guiding Policy Decisions:**  This line graph helps exemplify the need for safer structures for biking and walkability, mostly in Brooklyn, by showing the number of accidents, in which the injury frequency is also correlated with the frequency of traffic during the time of day.

**Resource Allocation:**  Re-paving lanes that cyclists use (bike lane, sidewalk), or widening them, will help reduce the number of incidents greatly.

**Community Awareness:**  The results can be used to help the communities of NYC decide which times are the most dangerous and to avoid or be more cautious during certain hours of the day.

**Traffic Safety Measures Testing:** The information may prove useful to help bring more emphasis on safety and spatial awareness, based on location and time of day.

<h3>Tie to the Dataset:</h3>

The dataset we chose is located is perfect for this kind of pattern recognition as it contains types of people injured/killed in which boroughs. 

To show off each pattern, we have a line graph showing how many cyclists are injured in which hour (so hour 6 would include 6:00:00 - 6:59:59) throughout the day.

By having a filter, although we are only highlighting Brooklyn, it helps show other boroughs in comparison to help emphasize that Brooklyn is the biggest contributor to this issue.

Analyzing the trends of cycling-related incidents is made possible by the time-stamped (by hour) data on rider injuries in the dataset. 

The analysis of different vehicles and hazards that bicycle riders in Brooklyn encounter during the day necessitates the availability of this comprehensive temporal data.


<h2>Manipulations of the Data Set:</h2>

One manipulation we made on the dataset was excluding those rows in which the time reported for the crash was exactly midnight (i.e. 12:00 AM or 0:00 in 24-hour time). The timing of these reports is likely the result of the police not listing the actual time of the crash and just the date. As a result, there was an excessively high number of reports all at midnight, which greatly skewed the data. Because our analysis focuses on trends of crashes based on the time of day, we decided it would be best to exclude these reports altogether from our analysis. To remove these from our analysis, we created a filter for exclusion. Additionally, we created filters based on the questions we created for analysis. For instance, our first question focuses on crashes in 2022 during specific times of the day (9 am-5 pm). Additionally, our second question focuses only on cyclist data coming out of the Brooklyn borough.

Another manipulation we made was excluding the rows in which the "Borough" column held a null value from Question 2's figures. The occurrence of null values in these cases likely was the result of police offers not listing the borough in their report, and since the borough comparisons were critical to our second question, there would be little value in retaining rows in which borough information was not present.

<h2>Analysis and Results:</h2>

**1. In 2022, How do the different numbers of traffic incidents and resulting deaths vary across different boroughs (Bronx, Brooklyn, Manhattan, Queens, Staten Island) in NYC during rush hours (9 AM and 5 PM), as visualized on a Tableau Coordinate Map?**

<img width="724" alt="Screenshot 2023-12-04 at 11 57 25" src="https://github.com/mh101410/29704Group5/assets/148079593/02e5c77b-d305-42e3-bd5c-65d881482a3c">

Manhattan Red - 1043 accidents / 1 killed

Bronx Blue - 1132 / 1 killed 

Queens Teal 1567 / 3 killed 

Brooklyn Yellow 2198 / 2 killed

Staten Island 280 / 0 killed

Manipulations: only 9 AM and 5 PM were included, all NULL values were excluded 

The only included crash times are 9 AM and 5 PM which are designated rush hours. 
The borough of Manhattan is home to around 1.5 million people. It is primarily known for its dense population and job market, which attracts many commuters. However, when cross-referencing this knowledge with the data, one would expect that Manhattan would carry one of the highest rates of deaths and collisions. This is quite the opposite. According to our data, Manhattan has the second lowest collision rate and a death rate of about .000959. This is potentially due to the extensive public transportation available in Manhattan. Even though Manhattan has a high number of civilians, only “22% of households own a car” (“New Yorkers and Their Cars.” New Yorkers and Their Cars | NYCEDC). Since a majority of households do not own a car, this could explain their low number of collisions despite the high population. 

Comparatively, the Bronx has a similar number of collisions sitting at around 1,132 and 1 death. While the Bronx is double the size of Manhattan, another explanation for its higher accident count is the possibility of a more complex city layout. On top of that, the Bronx car ownership rate is close to double that of Manhattan, at about 40%. So, a bigger, more complex city layout coupled with a higher presence of cars will lead to a higher collision rate. 

Queens is a unique data cluster as it has the second-highest collision rate, yet it possesses the highest death rate at around .0020. This is 2.08 times higher than that of Manhattan. The reason behind this could be a variety of reasons. When looking at speed limit maps of both areas, one will find that Queens has many more 50+ MPH zones than Manhattan, which can lead to more fatal accidents. Not only that, but Queens is the biggest borough of the five, and around 62% of households own a vehicle. Combining higher speeds and more cars will raise collisions and deaths. 

Brooklyn has the highest collision number out of all 5 boroughs and has 2 deaths for those. While the death rate is lower, the collision count is nearly double that of Manhattan and Bronx. This could be due to Brooklyn having the largest population of about 2.3 million people. Its similar car ownership to the Bronx, of around 44% is negated due to its huge population. 

The last Borough of Staten Island had around 280 collisions and 0 deaths. Staten Island is about 58 square miles and boasts a population of 378,000. This large borough with a comparatively small population is a formula for minimal accidents. While car ownership skyrockets to 83%, the thinly distributed characteristic of its population negates any increased chance of collision.

**2. What are the patterns in cyclist injuries in Brooklyn over different hours of the day compared to the other boroughs?**

<center>
    <img src="https://github.com/mh101410/29704Group5/blob/main/E703056E-6B04-4BA9-9656-E0E28BA22644.jpeg?raw=true" width="50%" height="50%">
</center>

<center>
    <img src="https://github.com/mh101410/29704Group5/blob/main/FE992263-6F35-41CE-A579-E5ED2C6517E5.jpeg?raw=true" width="50%" height="50%">
</center>

<center>
    <img src="https://github.com/mh101410/29704Group5/blob/main/DC9D15B5-B518-468C-84C6-419283413B6C.jpeg?raw=true" width="50%" height="50%">
</center>

Analysis: 

**Figure 1** shows a clear pattern of Brooklyn's cycling-related injuries over 24 hours. Each point represents the number of injuries occurring in the data within that hour, for example, the 671 cyclists injured at 8:00 AM represent all those hurt between 8:00 and 8:59 AM from our dataset. Early in the morning, from midnight until about 4:00 AM, cyclist injuries continually decline, which makes sense given that the majority of the borough’s population will be at home asleep. Then, the number of injuries bottoms out at 4:00 AM when the morning rush hour begins, prompting a sudden spike that endures until 6:00 PM when the number of cyclist injuries peaks at 1,460. This implies that the afternoon is the riskiest period for bicycles in Brooklyn, likely encompassing the lunch hour and the first part of the evening rush. The data then reveals a sharp fall in injuries after peak, which could be a sign of fewer cyclists as the evening wears on.

This injury count that jumps at 4:00 AM and falls at 6:00 PM is rigidly in line with the traditional work schedule. With the expected high traffic around the city explained by New Yorkers’ commutes, it’s certainly the case that the higher number of employee traffic explains the stark increase in injuries. A key insight we gleaned from the data is that, despite Queens and Brooklyn having similar populations throughout the range of data, Brooklyn has significantly more injuries throughout the data period than Brooklyn as shown in **figure 2**. Figure 3 shows that the total number of injured cyclists in the data was 8,238 in Queens and nearly double in Brooklyn at 16,586. So, despite Brooklyn and Queens having similar populations, there is a confirmed discrepancy in the former borough’s handling of bikers’ safety, highlighting the need for them to learn from how the latter has more effectively protected its residents.

Manipulations: Rows where Time 12:00:00 AM and where borough value = null are excluded

<h2>Tableau Packaged Workbook:</h2>

The Tableau Packaged Workbook has been uploaded to the eLC dropbox.
