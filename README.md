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

![image](https://github.com/user-attachments/assets/1f7fce77-1e73-4324-9966-2032c20ddcd6)

2. Check for null values

![image](https://github.com/user-attachments/assets/baf22bfb-b25b-4992-b1f1-4f8b4005a2f3)


3. Check for duplicates

![image](https://github.com/user-attachments/assets/d42d4107-b7b4-4fed-92ab-6302c5e620dd)


### Data Cleaning

1. Delete Rows that have null values in it

![image](https://github.com/user-attachments/assets/5c523c3d-0a05-41aa-a6ee-5d812b78f854)


2. Create 4 more column for duration of the rent (duration), day of the rent (day_start), hour of the rent (hour_start) and year-month of the rent (year_month).

![image](https://github.com/user-attachments/assets/d0babed7-51fa-43dc-9204-dabe1e405dca)


![image](https://github.com/user-attachments/assets/18e3af91-a096-4ec6-a0aa-e3edc8221629)


3. Delete row with Anomalous Durations

![image](https://github.com/user-attachments/assets/5dd12cab-6e06-4cf2-a7fd-115f44c3734c)


## Analyze and Share

The question is: How do annual members and casual riders use Cyclistic bikes differently?

First we will see the precentage of member and casual

![image](https://github.com/user-attachments/assets/593063b7-d341-41bc-8ae1-b7d5c23c2f12)


There are more Member than Casual

Then we will see the distribution of the rideable type for member and casual

![image](https://github.com/user-attachments/assets/51eec182-b090-4073-948d-07b658ce9049)


Most people used classic bike followed by the electric bike. Docked bikes are used the least and only by casual riders.

Next, we will see the distribution of trips across months, days of the week, and hours of the day.

![image](https://github.com/user-attachments/assets/42641f14-ccf5-4b34-96ab-4f8e356213a5)


Member start renting in the morning and afternoon, while casual rentals are primarily higher in the afternoon.

![image](https://github.com/user-attachments/assets/07610394-575a-478d-94d1-a0bd2a0fd4ff)


Member rentals are higher on Monday, Tuesday, and Wednesday (weekdays), while casual rentals are higher on Friday and Saturday (weekends).

![image](https://github.com/user-attachments/assets/d3cbe8e6-58f7-4ee8-9429-40eeb80c70a9)


Besides July and August, we can see that the monthly trend is quite similar for both members and casual users. Summer and spring see an increase in rentals, while winter and autumn experience a decrease.

Ride duration of the trips are compared to find the differences in the behavior of casual and member riders.

![image](https://github.com/user-attachments/assets/7533cf44-2838-4eb8-afe4-0c9de8f3b017)


Casual tend to rent longer compare to members do on average.

Next, we will see the station where the members and casual tend to start and end their rent.

![image](https://github.com/user-attachments/assets/9a5a17a2-3fb8-4fb7-977d-97ca50c27836)


![image](https://github.com/user-attachments/assets/43994bf0-eb56-491a-a867-370b95e9c56a)


we will visualize with the map for easier understanding\
_note: green is the starting station and red is the ending station_

Member
![image](https://github.com/user-attachments/assets/39335de3-8101-48bb-a64e-8643570e30b1)


Casual
![image](https://github.com/user-attachments/assets/19f91625-1893-4fb6-88a2-1980c4712e09)


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
