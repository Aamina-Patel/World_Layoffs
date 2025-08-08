# World_Layoffs


## Introduction
In this project, I cleaned the world layoffs dataset in MySQL and developed an interactive dashboard in Tableau to identify layoff trends by country, stage and industry.


## About the Dataset
The dataset contains information from layoffs around the world, from 2020 to 2023, structured into one table:
- layoffs - contains details of layoffs including company, location, industry, total_laid_off, percentage_laid_off, date, stage, country and funds_raised_millions


## Problem Statement
The dataset contains data from 2020 to 2023 which covers the covid period where many people were made redundant as companies were cutting back costs to reduce the losses caused by lockdowns.
My goal as a data analyst is to perform data cleaning, an initial data exploration and create a report that analyses the impact of covid on layoffs using the layoffs dataset.


## My Approach and Tools Used
To clean the dataset and perform an initial data exploration I used MySQL, ensuring accuracy.
To create this dashboard I used Excel and Tableau, ensuring interactivity.


### Data Cleaning

#### 1. Remove duplicates: 
- Firstly, I checked for duplicates in the tables using a windows function and a CTE. I created a staging table before removing the duplicates so that I had a copy of the raw dataset

#### 2. Standardise the data: 
- I found and corrected data entry errors in the table. For example, spaces before company names, changing date format from string to date etc

#### 3. Null or blank values: 
- Populated null or blank values using joins. Some nulls remain as further information is required to calculate these

#### 4. Remove unwanted column/rows: 
- Removed row_num column created to identify and remove duplicates and removed rows where both total_laid_off and percentage_laid_off were blank as I don't know if they have laid any employees off


### Data Analysis

#### 1. Initial exploratory data analysis: 
- I performed an initial exploratory data analysis in MySQL to see some trends which would allow me to better plan my dashboard, and then I exported the cleaned dataset to import into tableau

#### 2. Create a layout: 
- Used excel to create a layout for my tableau dashboard

#### 3. Graphs: 
- Loaded data into tableau and created graphs for dashboard

#### 3. Dashboard creation: 
- Inserted image of dashboard layout and then used horizontal and vertical floating containers to bring in graphs

### Final Dashboard

<img width="1352" height="757" alt="World Layoffs Dashboard" src="https://github.com/user-attachments/assets/84777292-9a09-459f-b1e7-2c4eab9cb46a" />


## Insights from the Dashboard
The dashboard provides a comprehensive breakdown of layoff trends by country, stage and industry. Key insights include:

#### 1. KPI's
- Total Laid Off: 192,900
- Average % Laid Off: 26%
- Total Funds Raised: 428,626 M
- Total Companies Affected: 826

2022 saw the highest total laid off at 80,400 employees. 
  
#### 2. Layoffs by Country
- Country with the Highest Layoffs: US had the highest total laid off at 130,300 employees

#### 3. Layoffs by Industry - Top 10
- Retail industy saw the highest layoffs at 30,500 employees laid off and 69 companies affected
- Real Estate industry saw the 10th highest layoffs at 9,100 employees laid off and 35 companies affected

#### 4. Layoffs by Company - Top 10
- Amazon had the highest layoffs at 18,200 employess laid off
- IBM industry saw the 10th highest layoffs at 3,900 employees laid off


## 
- Created by: Aamina Patel
- Built with: MySQL, Microsoft Excel, Tableau
- Data Source: [AlexTheAnalyst](https://github.com/AlexTheAnalyst/MySQL-YouTube-Series/blob/main/layoffs.csv)
