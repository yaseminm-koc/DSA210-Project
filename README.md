# A Look into How Urbanization Might Influence Global Marriage Trends

## Topic Change
This project originally focused on the relationship between lifestyle factors and sleep quality. However, I had to change the topic because the datasets couldn’t be merged or enriched effectively.

## Objective
The objective of this project is to examine whether countries with higher levels of urbanization tend to have lower marriage rates, and what other factors might be influencing that relationship.

## Motivation
Urbanization great speed has transformed the way people live, work, and connect. As more people move into cities, we see increase in individualism, workforce participation, and changes in social structures. All of which can affect people's approach towards marriage. On one hand, urban environments often encourage independence and career focus, which might lead to declining marriage rates. On the other hand, urban areas provide more opportunities for social interaction, education, and economic stability that are factors that can support relationship formation.

Given these two sides of urbanization, it's not obvious how urbanization really affects marriage rates across different countries. To better understand this, I decided to look at the relationship between urbanization and marriage rates using global data. I also enriched my dataset with variables like life expectancy, human and gender development indices, GDP per capita, average schooling, unemployment rate, working hours, and income inequality (Gini coefficient) to capture the broader social and economic context in which people make decisions about marriage.

## Data Sources
### Core Datasets:
### Share of the population living in urban areas
Source: https://ourworldindata.org/grapher/share-of-population-urban?tab=table


### Marriage rates
Source: https://ourworldindata.org/grapher/marriage-rate-per-1000-inhabitants?tab=table#all-charts


### Enrichment Datasets:
### Human Development Index
Source: https://ourworldindata.org/grapher/human-development-index?tab=table&time=2001..2015#reuse-this-work


### Unemployment rate
Source: https://ourworldindata.org/grapher/unemployment-rate?tab=table


### GDP per capita
Source: https://ourworldindata.org/grapher/gdp-per-capita-worldbank?tab=table


### Annual working hours per worker
Source: https://ourworldindata.org/grapher/annual-working-hours-per-worker?tab=table


### Life expectancy at birth
Source: https://ourworldindata.org/grapher/life-expectancy-hmd-unwpp?tab=table


### Gender Development Index
Source: https://ourworldindata.org/grapher/gender-development-index?tab=table


### Average years of schooling
Source: https://ourworldindata.org/grapher/average-years-of-schooling?tab=table


### Gini coefficient, 1963 to 2023
Source: https://ourworldindata.org/explorers/inequality?tab=table&Data=World+Bank+%28Incomes+after+tax+or+consumption%29&Indicator=Gini+coefficient&country=CHL~BRA~ZAF~USA~FRA~CHN


## Data Analysis
The data analysis was carried out in multiple stages. The datasets used were sourced from Our World in Data because I found that the site's datasets were easier to clean and process. I first filtered each dataset to include only the years between 2010 and 2017, because the dataset 'Annual working hours per worker's included most recent year was 2017 and I also wanted to add multiple years to my project. I also standardized country names and handled missing values manually, especially in the Gini coefficient dataset, where missing years were filled using mean imputation and the linear interpolation formula using the other available years from that country. 

Once merged, the analysis focused on visualizing and understanding the relationship between urbanization rates and marriage rates, while considering other potentially influential variables like GDP per capita, unemployment, Gini index, working hours, life expectancy, education, HDI, and GDI. 


## Expected Outcomes
The project aims to uncover lifestyle trends that significantly influence sleep efficiency. I expect to identify key factors such as screen time, caffeine intake, and stress levels as potential contributors to poor sleep quality.
