# Exploratory Data Analysis on Travel Insurance
### Background
Travel insurance is a plan you purchase that protects you from certain financial risks and losses that can occur while traveling, either internationally or domestically. These losses can be minor, like a delayed suitcase, or significant, like a last-minute trip cancellation or a medical emergency overseas.

This dataset is obtained from a third-party Singapore-based travel insurance services company. It contains 63,326 rows and 11 attributes about travel insurance products had been sold and the amount of net sales with claim status. The dataset was obtained from the website of [Kaggle]. 

## Table Content
* [Problem Statement](#problem-statement)
* [Technologies](#technologies)
* [Features](#features)
* [Problem Description](#problem-description)
* [Summary](#summary)
* [Conclusion](#conclusion)

## Problem Statement
The project objective is to understand which risk profile are more likely to have high claim rate of travel insurance and determine the price for the particular plans to be adjusted based on the age, duration and country that is most travelled.

## Technologies
Project is created with: 
* Python

## Features
The feature of the dataset have as per below: 
1.	Name of agency (Agency)
2.	Type of travel insurance agencies (Agency Type)
3.	Distribution channel of travel insurance agencies (Distribution Channel)
4.	Name of the travel insurance products (Product Name)
5.	Claim Status (Claim)
6.	Duration of travel (Duration)
7.	Destination of travel (Destination)
8.	Amount of sales of travel insurance policies (Net Sales)
9.	Commission received for travel insurance agency (Commission)
10.	Gender of insured (Gender)
11.	Age of insured (Age)

## Problem Description 
Before starting actual analysis, a lot of cleaning needs to be done on the data. 
* Data Cleaning
1. Drop the column gender as the feature is blank more than 70%. 
2. Replacing the age more than 100 years old by the average age of individual product. 
	- [Current oldest people living is 114 years old.]("https://en.wikipedia.org/wiki/Oldest_people") 
* Data Quality Assurance 
1. Drop the negative value from Duration and replace zero by average.
	- Highly right skewed for the "Duration"
	- This is not practically possible that duration is negative values because a trip must have a duration greater than 0. 

## Summary 
 - Online transactions are more than offline, this is due to more convenient to do online and people are more IT savvy now.
 - An imbalanced claim status as there is only 1.5% claimed from the whole dataset.
 - The variances between the most highest frequency and the second highest frequency is huge.
 - Commission and Net Sales have the stronger relationship among the other variables. It could be due to the commission paid out is higher hence adviser will be more driven to close the sales on the particular product. 

## Conclusion
- In general, travel insurance premium is mostly based on destination and duration for the coverage.
- Airline agencies should focus more on acquiring customers who opt for airline insurance together with a package at a lower price to attract the customer to purchase from them.
- Provider may consider to drop their low performing products which generates lesser revenue.
- Airline agencies should invest on how to increase their sales via online mode(e-commerce).
- Intelligently divide the resources in proportion to the revenue that they generate from different countries.



This project was done as part of DS102 & DS104 project requirement of Applied Data Science with Machine Learning in MAGES of Institute of Excellence - 2021. 


[Kaggle]:https://www.kaggle.com/mhdzahier/travel-insurance
