Bike Sharing Analysis

## Overview of the data

We have 10 csv file include all the ford gobike system data from 2017-1 to 2018-10. There are 1916465 rows and 16 columns in the 10 dataset. Some columns are user_type, gender, birth year, start and end station information and the date time of each trip. 

The motivation of this project is to generate insights about demographic of users as well as use pattern, for example, the peak time of using the bike or where would be a good location for us to build more stations or arrange more bikes.




## Packages
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- re
- folium


## Get started

### Data wrangling

I loaded all 10 csv file under a folder and merge them into one dataset. Then I did some assessing steps to uncover the data issues, some key findings are like: 

- There are multiple missing value in member_gender, member_birth year columns.
- The data type for start_time and end_time are wrong.
- Duration in seconds is not understandable and need to be converted into minute.
- There are some outliers in duration_sec and member_birth_year, for example, we have a 1840 birth year for a user which is definitely unmeaningful and need to be processed.


### Data exploration

I developed a lot of visualization to figure out the descriptive statistics about the data set:

- Demographic of user: 74.2% of users are male, 24.3% of users are female. More than 50% of users belong to the 18~35 age group, 30% of user are from 36~55 years old group, other users are from 56~74 age group.
- The duration distribution are mainly fall into the range from 1 to 20 mins, 5~10 mins is the most frequent durations for each trip. The median duration for female is 
about 10 mins higher than 8 mins for male users.
- In this dataset, we can read the most users are subscribers. 




### Data explanatory analysis

I explored some interesting insights through this analysis, for example:

- I found generally the customer would spend more time for each trip, the median duration of subscriber is around 8 mins whereas median duration of customer is around 14 mins. We can see a 6 mins gap here.

- 7:00 ~ 9:00 and 16:00 ~ 18:00 are the peak time to use bike sharing, and it aligns with the morning rush hour so I can assume most frequent use cases is to commute. 

- The bikes get the highest usage during weekday, which is again, prove that the most frequent use case is for people to commute for work.

- With plotting map about start station location and end station location, I found that the trip start station are centrated on San Francisco, Oakland and San Jose areas. That makes sense since the density of office buildings in these 3 area is very high.


### Conclusion and Recommendation

Given the insight we generated from the analysis, I think we can have some improvement about the marketing strategy and operations.

- In the San Francisco, Berkely, Oakland and San Jose area we can build more bike stations and put more bikes there for make sure we provide enough amount of bikes.

- Especially during weekday morning and evening, we need to make sure the enough supply for people since the most frequent use cases for user is to commute for work.

- Since male users account for a large amount of our users, we can put more marketing budget and resources focus to the male customer.








