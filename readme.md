# FordGoBike Trip Data

## by Adham Hussein


## Dataset

>The forgobike trip data are 183,412 rides that happend in Febraury month of  2019 . The dataset is contain 16 columns before I did cleaning. Some attributes duration_sec, start_time, end_time, start_station_id, start_station_name, and member_age. I downloaded the data set from course resources of project details.
I delete all user more than 75 years old because most users are between 18-75 year old . Also I created new columns like  duration_min, start_hourofday,start_dayOfweek and member age. 
After I cleaned my data and craeted new columns the data became 174884  records and 21 columns.

## Summary of Findings

> In my exploration, I found that there are two types of user:

1-Customer
2-Subscriber
I realised the subscriber users have the highset number of trips at 8.AM and 5.PM and that because the going back from  work hours (start and end work). 
Also the rides trips between 12.AM and 5.AM has the lowest number of rides and that it's hours sleep. And on the week day I found the weekday have more trpis per day than weekend day. Unlike customer users.
The customer users the number of trips are start growing from 7.AM to 5.PM (highset) then it's will be decreased. Also they have the highset trips on weekend.
Also I found most ages are between 28 to 40 years old for subscriber users, and the customer users are between 18 to 37 years old.  I found the ages between 21 to 35 years are the highset.

## Key Insights for Presentation

> Different usage pattern/habit between the two type of riders are seen from the exploration. Subscribers use the system heavily on work days i.e. Monday through Friday whereas customers ride a lot on weekends, especially in the afternoon. Many trips concentrated around 8-9am and 17-18pm on work days for subscribers,
 but customers tend to use more in the late afternoon around 17pm Monday to Friday. The efficient/short period of usage for subscribers corresponds to their high concentration on rush hours Monday through Friday, indicating the use is primarily for work commute. 
 The more relaxing and flexible pattern of customer use shows that they're taking advantage of the bike sharing system quite differently from the subscribers, heavily over weekends and in the afternoon.