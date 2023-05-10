# Data-Professional-Survey

## Introduction
This dashboard is inspired by the portfolio project done by AlexTheAnalyst and uses the data he captured surveying data professionals. 

### Aim for this project is to analyze the following:
* What are the average salary for different data job titles?
* Which language is most preferred by job professionals?
* What are the most common educational qualifications?
* How the survey takers respond to the questions asked to them on scale of 1-10?

## Data Cleaning
#### Before we started with the dashboard creation we needed clean up and transform the data as per the requirement for which I used Power Query
* Removed coloums which were not relevant for the analysis like Browser, OS, city etc.
* Column for preferred programming language had many values under "Others" category as shown below:
![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/7824975e-286a-4a29-a2b0-56599f8c7e6f)

From this I wanted to group everything under Others but keep "SQL" as standalone value similar to Python or R. I used split by, replace and conditional functionalities to achieve the below mentioned list:

![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/3544d301-36d1-422c-a9bc-e2db9c967ae6)

* Salary column had ranges provided in it that too in text format as shown below:

![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/7bf7607e-8ef5-4017-9d7e-83bd60204825)

I needed a numerical value for our analysis so firstly I used th range given to create 2 numerical columns with lower and upper value in each. Then I calculated the average column using the M coding to achieve the below results:
![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/d2c518ad-62b2-4e0e-a58f-7478a26e3186)

## Data Visualizations
For the dashboard I decided to go with 2 sheets; 1st sheet is used to display generic demographics of survey takers while 2nd sheet would contain actual survey questions with their respective scores. Complete dashboard along with PDF with both the sheets are placed in the same repository.

### Key Insights I got from this dashboard
1. There were total of 630 respondants to the survey with average age of 30 and average salary of 54K (Used cards)
![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/45f78c9d-7913-4c76-8631-31c519812f87)

2. Data Scientists have highest average salary followed by Data Engineer and Data Architect respectively (Used Stacked bar chart)

 ![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/a9493730-7304-4609-bf74-61336d750307)

3. Python is the most preferred language amongst the respondants (Used Stacked column chart)

 ![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/89f36736-cae0-41f5-9907-2e8516f22132)

4. Majority of the respondants were from US followed by India, UK, Canada and Nigeria (Used Treemap for this)
![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/b3872848-b350-4400-8828-98bc5c7d23b7)

5. People have rated 5.61/10 on the learning opportunites provided to them and 5.74/10 on the work/life balance they have in their current positions (Used Gauge meters)

![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/3556edc7-620d-416e-89cb-904f1151c5b5)
![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/19cf3051-fea5-4096-a013-7a28a20c6d21)


6. On the salary side people have rated just 4.27/10 and on upward mobility opportunities 4.76/10 (Used Gauge meters)
![image](https://github.com/akshaykumar17288/Data-Professional-Survey/assets/133111241/888569bd-4940-4e67-85d9-817564a3e447)

