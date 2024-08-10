# Cyclistic Case Study

Case study: How does a bike-share navigate speedy success?

## Introduction

In this case study, you work for a
fictional company, Cyclistic, along with some key team members. In order to answer the
business questions, follow the steps of the data analysis process: Ask, Prepare, Process,
Analyze, Share, and Act.

Data : https://divvy-tripdata.s3.amazonaws.com/index.html

This study was conducted using [Google Colaboratory](https://colab.research.google.com/)

## Scenario

You are a junior data analyst working on the marketing analyst team at Cyclistic, a bike-share
company in Chicago. The director of marketing believes the company’s future success
depends on maximizing the number of annual memberships. Therefore, your team wants to
understand how casual riders and annual members use Cyclistic bikes differently. From these
insights, your team will design a new marketing strategy to convert casual riders into annual
members. But first, Cyclistic executives must approve your recommendations, so they must be
backed up with compelling data insights and professional data visualizations.

## Ask

Three questions will guide the future marketing program:

1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

## Prepare

Data that will be used are from June 2023 to May 2024.
The data has been made available by
Motivate International Inc. under this [license](https://divvybikes.com/data-license-agreement)

There are 12 csv files with each file containing data for one month. each file has the same column

## Process

### Combining the Data

The data is combined and created a new dataframe with 5.743.278 rows

### Data Exploration

1. Check the data type

![alt text](image-1.png)

2. Check for null values

![alt text](image-2.png)

3. Check for duplicates

![alt text](image-3.png)

### Data Cleaning

1. Delete Rows that have null values in it

![alt text](image-4.png)

2. Create 4 more column for duration of the rent (duration), day of the rent (day_start), hour of the rent (hour_start) and year-month of the rent (year_month).

![alt text](image-6.png)

![alt text](image-8.png)

3. Delete row with Anomalous Durations

![alt text](image-5.png)

## Analyze and Share

The question is: How do annual members and casual riders use Cyclistic bikes differently?

First we will see the precentage of member and casual

![alt text](image-9.png)

There are more Member than Casual

Then we will see the distribution of the rideable type for member and casual

![alt text](image-10.png)

Most people used classic bike followed by the electric bike. Docked bikes are used the least and only by casual riders.

Next, we will see the distribution of trips across months, days of the week, and hours of the day.

![alt text](image-11.png)

Member start renting in the morning and afternoon, while casual rentals are primarily higher in the afternoon.

![alt text](image-12.png)

Member rentals are higher on Monday, Tuesday, and Wednesday (weekdays), while casual rentals are higher on Friday and Saturday (weekends).

![alt text](image-13.png)

Besides July and August, we can see that the monthly trend is quite similar for both members and casual users. Summer and spring see an increase in rentals, while winter and autumn experience a decrease.

Ride duration of the trips are compared to find the differences in the behavior of casual and member riders.

![alt text](image-14.png)

Casual tend to rent longer compare to members do on average.

We can infer from the previous observations that member may be using bikes for commuting to and from the work in the week days while casual riders are using bikes throughout the day, more frequently over the weekends for leisure purposes. Both are most active in summer and spring.
These findings lead to the conclusion that casual commuters travel longer (approximately 2x more) but less frequently than members. They make longer journeys on weekends and during the day outside of commuting hours and in spring and summer season, so they might be doing so for recreation purposes.

Next, we will see the station where the members and casual tend to start and end their rent.

![alt text](image-15.png)

![alt text](image-16.png)

we will visualize with the map for easier understanding\
_note: green is the starting station and red is the ending station_

Member
![alt text](image-17.png)

Casual
![alt text](image-18.png)

Members usually start and end their rent inside the city while casual started and end their rent in park, lake, beach, or harbor.

### Summary

- People tend to prefer renting classic bikes, followed by electric bikes, with docked bikes being rented only by casual users.
- Rental activity increases during the summer and spring and decreases in the winter and autumn.

**Member**

- Rent bikes on weekdays in the morning and afternoon
- They are more often rent a bike but only in a short time
- Members predominantly rent bikes within the city. Probably for work or school

**Casual**

- Rent bikes on weekends in the afternoon
- They are less often rent a bike but rent it for a long time
- Casual riders tend to rent bikes in locations outside the city, such as parks or lakes. Probably in their free time for vacation

## Act

1. Marketing efforts should be concentrated during the Summer and Spring seasons, as well as on weekends, particularly in recreational areas where casual renters are more prevalent.
2. Consider introducing a membership plan tailored for individuals who primarily rent on weekends. This membership could offer bonuses or discounts for extended rental durations.
3. Implement seasonal discounts during Autumn and Winter to encourage increased rentals during these lower-demand periods.
