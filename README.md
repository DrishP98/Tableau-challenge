# Tableau-challenge - New York City Citibike Analysis for Jan 2014-Sept 2014

## Link to project:
https://public.tableau.com/app/profile/drishti.patel/viz/Module18_17121366279200/Story1

## Project Description
Congratulations on your new job! As the new lead analyst for the New York Citi BikeLinks to an external site. program, you are now responsible for overseeing the largest bike-sharing program in the United States. In your new role, you will be expected to generate regular reports for city officials looking to publicise and improve the city program. Since 2013, the Citi Bike program has implemented a robust infrastructure for collecting data on the program's utilisation. Each month, bike data is collected, organised, and made public on the Citi Bike DataLinks to an external site. webpage. However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have questions about the program, so your first task on the job is to build a set of data reports to provide the answers.
## Instructions
1. Your task in this assignment is to aggregate the data found in the Citi Bike Trip History Logs and find two unexpected phenomena. Design 2–5 visualisations for each discovered phenomenon (4–10 total). You may work with a timespan of your choosing. Optionally, you can also merge multiple datasets from different periods.
2. Use your visualisations (not necessarily all of them) to design a dashboard for each phenomenon. The dashboards should be accompanied by an analysis explaining why the phenomenon may be occurring.
3. Create a static map that plots all bike stations with a visual indication of the most popular locations to start and end a journey, with zip code data overlaid on top.
4. Create your final presentation:Create a Tableau story that brings together the visualisations, requested maps, and dashboards. Ensure your presentation is professional, logical, and visually appealing.

## Analysis
1. I have chosen to go with Citibike Data from NYC for the period Jan 2014-September 2014. Data was downloaded as CSV files from the website https://citibikenyc.com/system-data.
2. The reason I have chosen this period is largely because a lot of the larger files were difficult to download, manipulate and add to Tableau.
3. Data cleaning: I have concatenated the CSV files using Jupyter Notebook. I have filled all nulls with 'unknown'. I have also changed all birth year to integers and trip duration to datetime. The files were too large to upload to Github.
4. Questions explored:
* Birth Year with highest number of bike riders?  1983 with 312521 riders. The age range would be around 30 and likely explains mature aged workers with stable jobs and regular bike riding.
* Trip duration trend? Average trip durations were longer during the older birth years from 1899-1952 and then stayed relatively consistent from 1952 onwards. The large fluctuaions in the early birth years are likely due to older age and varying fitness/health levels compared to the younger population.
* Is there a gender discrepancy between riders? Yes, as seen in the bar chart there are approximately 4 million more male riders than female. More investigation would be needed to understand why there is such a large gap in both genders.
* Monthly trends: There are a total of 8081216 trips recorded during this time period. In general the number of bikers have increased over the months of January to September which would likely be due to improved weather/summer months. Both user types have an increase but annual subscribers have a more exponential growth compared to short-term customer type. Average trip duration is higher for customer type than subscriber, with February having the highest duration. Annual subscibers are likely everyday bikers that commute to work and this explains why they have significantly larger numbers than the customer types. It also makes sense for everyday commuters to have shorter trip duration as it's likely an everyday trip compared to short-term customers who might be making varying trips and of longer duration if it's not regular practice.
* Most and least popular start stations: Most popular start station is 8 Ave & W 31 St which makes sense as it's the main intercity railroad station in NYC. Least popular start station is 7 Ave & Farragut St which is very far away from the central area.
* Most and least popular end stations: Most popular end station is E 17 St & Broadway which is near Union Square Manhattan, another very busy intersection. Least popular end station is Montangue St & Clinton St which could possibly be due to the high crime area in the Brooklyn district. 

## References:
Data source: https://citibikenyc.com/system-data. Thi project is completed as part of the UWA Data Analytics and Visualisation Bootcamp and is intended for educational purpose only.
