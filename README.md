# Road-Accident-Data
Analysis of Road Accident Data

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)

### Project Overview
This project aims to provide valuable insight into the Road Accident occurance by various vehicle type, different road types and different weather conditions. By analyzing all these aspects of the data, I seek to indentify accident happening over months, and make data driven recommendations.


![image](https://github.com/Harshkumarspatel/Road-Accident-Data/assets/151779392/9c303b15-6ed9-4857-b135-03cdb26951ff)


### Data Sources
The primary dataset used here is the "Road Accident Data.xlsx" file. Which contain detail of each of the Road accident happened in the two years (2021 & 2022). 
The dataset contains more than 300K rows of information.

### Tools
- Excel - for data cleaning
- PowerBI - for data analysis and to create report 

### Data Cleaning
In the initial data preparation phase following tasks were performed:
1. Data loading and Inspection
2. Handling missing values
3. Data cleaning and formatting

### Exploratory Data Analysis
EDA involved exploring the data to answer following questions:
- What is the road surface condition where most accidents occured?
- Which types of vehicle have highest number of accidents?
- What is the weather condition and light condition when accidents happened?

### Data Analysis
For data analysis DAX measures where created in PowerBI, some of them are shown below:

1) PY casualties = CALCULATE(SUM(Data[Number_of_Casualties]),SAMEPERIODLASTYEAR('Calendar'[Date]))
2) CY Casualties = TOTALYTD(SUM(Data[Number_of_Casualties]),'Calendar'[Date])

### Results

1. Car witnessed most number of accidents in both the years, followed by the bike.

![image](https://github.com/Harshkumarspatel/Road-Accident-Data/assets/151779392/83e9c7cf-47df-4bfa-80a4-c972ea467d1b)


2. Number of road accident takes significant drop in the month of december in both years. while overall casualties by accidents got decreased compared to the last year.

![image](https://github.com/Harshkumarspatel/Road-Accident-Data/assets/151779392/0c8900f3-789c-4c2f-9f4f-121a9ef1ba32)


### Recommendations
Based on the analysis, I recommend following actions:
- Analysis showed that accident occured more in urban areas(62%) compared to rural areas(38%), it maybe because urban areas have more number of vehicles. So, the final conclusion should not be based on this.
- It also shows that during fine weather there are more accidents than when conditions are rain or snow, So it's most likely that it happened due to the human error.
- Higher authorities can implement strict laws for drivers and can improve road conditions if required.
