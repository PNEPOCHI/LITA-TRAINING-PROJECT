# LITA-TRAINING-PROJECT

## Table of content

[project overview](#project-overview)

[data source](#data-source)

[tools used](#tools-used)

[data cleaning and preparation](#data-cleaning-and-preparation)

[exploratory data analysis](#exploratory-data-analysis)

[data analysis](#data-analysis)

[findings and results](#findings-and-results)

[recommendation](#recommendation)



### Project Overview 

The aim of this project is to Analyze sales performance of INTERNATIONAL BREWERIES from 2017-2019, in terms of consumer preferences and financial stability.
The project will focus on the performance of different product across five different countries on a yearly basis. The goal is to identify the best performing product in different rejoins of the country as well as the least performing country 


![Screenshot (4)](https://github.com/user-attachments/assets/4dce742a-832d-4262-96e3-748dd040b2c0)
![Screenshot (5)](https://github.com/user-attachments/assets/3b27c350-38be-4699-bb85-e530fce64d68)
![Screenshot (6)](https://github.com/user-attachments/assets/9264019f-e0a0-4587-9cdf-3b784f8b0b38)
![Screenshot (7)](https://github.com/user-attachments/assets/03f39ed7-7854-485b-bc29-997eee4f3124)


### Data source

The primary source of data used here is INTERNATIONAL BREWERIES.CSV. This dataset was given to me by my instructor and similar dataset can also be gotten from any open data source online.

### Tools Used

- Microsoft excel: For data cleaning, analyzing,  data visualization 
- SQL: Data Analysis

### Data cleaning and preparation

In the initial phase of the Data cleaning and preparation, we perform the following action
1	Data loading and inspection
2	Handling missing variables 
3	Data cleaning and formatting

### Exploratory Data Analysis

1. what product is the best seller?
2. what is the overall profit trend in different years
3. What is the overall sales trend in different country 

### Data Analysis

```sql
SELECT*FROM [dbo].[InternationalBreweries]

select sum(profit) as TotalProfit
from  internationalBreweries

select countries,
CASE
   WHEN COUNTRIES in('Nigeria','Ghana') then 'Anglophone'
   Else 'Francophone'
   End as Countriesgroup,
   sum(profit) as Totalprofit from internationalBreweries
   where years in ('2017','2018','2019')
   Group by countries
   order  by 3 desc
```

### Findings and Results

At the end of this data analysis , it was determined that;
. Castle lite is the top selling product
. Senegal has the highest sales
. the best sales were made in 2017

### Recommendation
. more castle lite product should be produced 
. other countries need more marketing strategies to enhance sales

|HEADING1|HEADING2|
|--------|--------|
|CONTENT1|CONTENT2|
|EXCEL|SQL|


😊😊💖💖✨✨🌹🌹


