# 2017:2018 Bay Wheels Ride Data Exploration and Visualization
## by Mai Rezk



## Dataset
> The dataset used for this exploratory analysis consists of monthly individual trip data from January 2017 to December 2018 in CSV format covering the greater San Francisco Bay area, raw data is available . Visualizations below are created from wrangled and cleaned data to facilitate exploration analysis and help discover usage pattern and rider characteristics.

##### Data wrangling process:
- fix multiple fields that are not in the correct dtype, as `start_time`, `end_time` should be datetime type, `user_type` and `member_gender` should be categorical data type, etc
- add new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, day of week and month
- add a new column calculating riders' age from 'member_birth_year'
- filter out outlier ages 
- cast 'member_birth_year' and 'member_age' to integer instead of float type
- cast 'start_dayofweek' to category dtype
- cast 'start_month' to category dtype 
- filter out outlier trip records where the duration was very long


## Summary of Findings

trips numbers peaked around 8 9 and 17-18 during a day, there were more trips on work days (Mon :Fri) compared to weekends. Summar time was the most popular season due to the weather. The  trips tend to be shorter on (Monday : Friday )compared to weekends. It indicates an efficient usage of the bike system on work days, while more casual flexible use on weekends.

Most riders were male subscribers who did not use bike share for all trips. Most members were around 25 to 40 years old, as the age gets older, bike usage dropped significantly.  male riders tend to have shorter trips compared to female rider . Riders who rented the bikes Monday through Friday are slightly older than those who ride on weekends, which supplements the work ride usage that was observed from some of the univariable exploration plots.

There are a lot more subscriber usage than customers overall. The riding pattern varies a lot between subscribers and customers. Subscribers use the bike sharing system for work trips that why  most trips were on work days (Mon :Fri) and especially during rush hours , whereas customers tend to ride for fun in the afternoon or early evenings over weekends. Subscriber usage peaks out on typical rush hours when people go to work in the morning and getting off work in the afternoon Similar pattern was not observed among customers who tend to ride most in the afternoon or early evening for a different purpose than the subscribers.


## Key Insights for Presentation

Different usage pattern between the two type of riders are seen from the exploration. Subscribers use the system heavily on work days  
(Monday Friday ) whereas customers ride a lot on weekends, especially in the afternoon. Many trips concentrated around 8-9 and 17-18 on work days for subscribers, yet customers tend to use more in the late afternoon around 17Monday to Friday. The short period of usage for subscribers  indicating the use is primarily for work trip. The more relaxing the pattern  is of the customer use shows that they are using  the bike sharing system in a different way than the subscribers, heavily over weekends and in the afternoon