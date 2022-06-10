
# Ford GoBike Data Exploration
## by Bukunmi Adebanjo


## Dataset

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. Contained within the dataset is total of 16 variables(dependent and non-dependent) before cleaning and over 180,000 bike trip records:

        Variable                Data_ Type
    1. duration_sec                 int64
    2. start_time                  object
    3. end_time                    object
    4. start_station_id           float64
    5. start_station_name          object
    6. start_station_latitude     float64
    7. start_station_longitude    float64
    8. end_station_id             float64
    9. end_station_name            object
    10. end_station_latitude      float64
    11. end_station_longitude     float64
    12. bike_id                     int64
    13. user_type                  object
    14. member_birth_year         float64
    15. member_gender              object
    16. bike_share_for_all_trip    object

The dataset was provided by Udacity and can be found [here](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv), with feature documentation found [here](https://docs.google.com/document/d/e/2PACX-1vQmkX4iOT6Rcrin42vslquX2_wQCjIa_hbwD0xmxrERPSOJYDtpNc_3wwK_p9_KpOsfA6QVyEHdxxq7/pub).

## Summary of Findings

Average trip duration for the entire dataset hovers around 10 minutes. Most people start their trips for the day at 8am while evening trips are mostly started at 5pm. A percentage of 75 male gender type dominate the data set and majority (95%) of the bike riders are Subscriber category user types. Over 50% of the Subscriber category users travel less than a total of 10 minutes while the Customer user types record more minutes during bike trips. Users of age range 32 to 35 ride bikes the most and average age across all categories is below 40yrs.
A surprising outcome is that the Other gender category kept some stations busier than every other gender category. in other words, they took longer trips despite being of the lowest percentage of gender type present in the dataset. 


## Key Insights for Presentation
For this presentation I focus on exploring variables of interest such as gender, start_station, end_station,start_time, user types and trip duration. Particularly, how trip duration varies amongst different gender groups,user types and hours of the day. Also, using trip durations as a metric to determine the busiest Start and End bike stations and what gender groups engages these busy stations the most.                    
Inspecting the duration variable will start the presentation while I gradually indtroduce other variables to show the possibles relationships and correlations that exist amongst them. In other words a flow from Univariate to Bivariate and Multivariate plots will be deployed for this presentation to better communicate necessary insights. Bar plots to explore distribution of the duration variable. As this is a key variable in my analysis. It is important I understand and modify its distribution plot if necessary. Another bar representaion plot will explore the distribution of the start and end time for bike rides across the data set.The busiest start and end stations too are worth understanding with via a Bar plot representation. Subsequently investigation into relationship amongst variables will commence by plotting the start time vs the duration to better understand the association between longer and shorter ride duration with various start times, a scatter plot more suitable represents this relationship. Finally, I deployed an adapted plot to see gender performance with regards to the top five busiest station in terms of trip duration across gender categories.
