# Ford Go Bike Project

## Introduction

This project is the exploration of the individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

### Data Wrangling and Cleaning Process

> - Start and end datetime columns were changed to datetime type.
> - Outliers in duration_sec, and member_birth_year were filtered out.
> - `age` column was created from member_birth_year column.
> - A distance column was created from the longitude and latitude columns, and values within the column were rounded up to 2dp
> - New columns for day of week, and another for time of the day (morning, afternoon, night, Sunday-Saturday) were created
> - A duration minute column was also created.
> - Columns not relevant to the analysis were dropped and rows with missing data were deleted.

### Summary of Findings

> - The main interest of this research was to explore the distance covered by each person, and how this may be closely related with other features such as age, gender, bike id, user type, day of the week.
> - To do this, distance column was created from the longitude and latitude columns, and values within the column were rounded up to 2dp. Also, the duration_sec was closely looked at because distance is often associated with time.
> - It was seen that 99% of the cyclers rode for less than an hour. Also, only 1% of the population cycled for more than 5.05km. The people in this latter group were referred to as the ambitious bikers throughout the analysis.
> - **Concerning a relationship between duration and distance:** It was also observed that the bikers moved at different speeds, they could have ridden for 1000 seconds and traveled 5km, or just 1km. However, Most of the bikers who traveled far, traveled fast.
> - **As it concerns bike version:** Those who rode their bikes for longer seconds were more likely to be using a more modern bike version.
> - **Looking at hours of the day and days of the week:** People who start a bike ride in the early hours of the morning (0hrs - 5hrs), are more likely to ride for a shorter period of time compared tho those who start after 10:00am. The most popular hours for people to start a bike ride are by 8:00 am, and by 5:00pm. Thursday is the day that most people started a bike journey. The weekend (Saturday and Sunday) is less likely to be chosen as a day to start a bike trip.
> - **Regarding Age:** Interestingly, the ambitious bikers are mostly between their mid 20s and 40s. The people who rode the farthest are in their 30s. Unsurprisingly, younger people (20 - 40 years) are more likely to ride a bike for longer minutes than older people.
> - **In terms of Gender:** Across all genders, older people tend to ride for shorter distances. Also, more people from the `Other` gender category cycle for shorter distances. It was interesting to see that there are more ambitious female bikers between the age of 60 - 70, than there are for either of the two other genders.
> - **Comparing Customers to Subscribers:** During the weekend, there are more customer riders than there are subscriber riders.
