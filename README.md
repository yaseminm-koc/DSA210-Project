# A Look into How Urbanization Might Influence Global Marriage Trends


## Topic Change
This project originally focused on the relationship between lifestyle factors and sleep quality. However, I had to change the topic because the datasets couldn’t be merged or enriched effectively.


## Objective
The objective of this project is to examine whether countries with higher levels of urbanization tend to have lower marriage rates, and what other factors might be influencing that relationship.


## Motivation
Urbanization great speed has transformed the way people live, work, and connect. As more people move into cities, we see increase in individualism, workforce participation, and changes in social structures. All of which can affect people's approach towards marriage. On one hand, urban environments often encourage independence and career focus, which might lead to declining marriage rates. On the other hand, urban areas provide more opportunities for social interaction, education, and economic stability that are factors that can support relationship formation.

Given these two sides of urbanization, it's not obvious how urbanization really affects marriage rates across different countries. To better understand this, I decided to look at the relationship between urbanization and marriage rates using global data. I also enriched my dataset with variables like life expectancy, human and gender development indices, GDP per capita, average schooling, unemployment rate, working hours, and income inequality (Gini coefficient) to capture the broader social and economic context in which people make decisions about marriage.


## Expected Outcome
This project aims to uncover whether urbanization plays a significant role in global marriage trends, and if so, how that role changes depending on a country's development level and social conditions. The results could help us better understand how modern lifestyles are reshaping personal and social choices around the world. 


## Data Sources
### Core Datasets:
### Share of the population living in urban areas
Source: https://ourworldindata.org/grapher/share-of-population-urban?tab=table

This dataset tracks the percentage of a country's population living in urban areas. 


### Marriage rates
Source: https://ourworldindata.org/grapher/marriage-rate-per-1000-inhabitants?tab=table#all-charts

This dataset provides information on the number of marriages per 1,000 inhabitants in different countries, showing trends in marriage patterns over time.


### Enrichment Datasets:
### Human Development Index
Source: https://ourworldindata.org/grapher/human-development-index?tab=table&time=2001..2015#reuse-this-work

The Human Development Index (HDI) is a composite statistic of life expectancy, education, and per capita income. It is a strong indicator of a country’s overall development and quality of life that might affect the decision of marriage.


### Unemployment rate
Source: https://ourworldindata.org/grapher/unemployment-rate?tab=table

This dataset tracks the percentage of the labor force that is unemployed but actively seeking work. High unemployment may correlate with economic insecurity, which can affect life decisions like marriage.


### GDP per capita
Source: https://ourworldindata.org/grapher/gdp-per-capita-worldbank?tab=table

Gross Domestic Product (GDP) per capita measures the economic output of a country divided by its population. It gives us a view of the economic environment in which marriage decisions are made. A wealthier country may have different marriage trends than a less wealthy one.


### Annual working hours per worker
Source: https://ourworldindata.org/grapher/annual-working-hours-per-worker?tab=table

This dataset shows the average number of hours worked per year by each employed person. It can help analyze work-life balance trends and economic pressures potentially influencing marriage decisions.


### Life expectancy at birth
Source: https://ourworldindata.org/grapher/life-expectancy-hmd-unwpp?tab=table

This dataset tracks the average number of years a person can expect to live at birth. It's a key measure of public health and general living conditions.


### Gender Development Index
Source: https://ourworldindata.org/grapher/gender-development-index?tab=table

The Gender Development Index (GDI) compares male and female human development achievements in a country. Gender equality plays a significant role in marriage decisions. In societies with greater gender equality, marriage rates may behave differently than in societies with significant gender disparities.


### Average years of schooling
Source: https://ourworldindata.org/grapher/average-years-of-schooling?tab=table

his dataset tracks the average number of years of schooling received by people in a country, providing insights into the country's educational system and the citizen's education levels which is often linked to marriage trends. Usually with higher education level comes delayed marriage.


### Gini coefficient, 1963 to 2023
Source: https://ourworldindata.org/explorers/inequality?tab=table&Data=World+Bank+%28Incomes+after+tax+or+consumption%29&Indicator=Gini+coefficient&country=CHL~BRA~ZAF~USA~FRA~CHN

The Gini coefficient measures income inequality within a country. A Gini index of 0 indicates perfect equality, while an index of 1 means maximum inequality. Income inequality can affect social behaviors, including marriage. In countries with higher inequality, marriage patterns may differ from those in more equal societies.


## Data Analysis
The data analysis was carried out in multiple stages. The datasets used were sourced from Our World in Data because I found that the site's datasets were easier to clean and process. I first filtered each dataset to include only the years between 2010 and 2017, because the dataset 'Annual working hours per worker's included most recent year was 2017 and I also wanted to add multiple years to my project. I also standardized country names and handled missing values manually, especially in the Gini coefficient dataset, where missing years were filled using mean imputation and the linear interpolation formula using the other available years' data from that country. 

After handling the merged data, with the final merged data the analysis focused on visualizing and understanding the relationship between urbanization rates and marriage rates, while considering other potentially influential variables like GDP per capita, unemployment, Gini index, working hours, life expectancy, education, HDI, and GDI. 

Also hypothesis testing was applied to our hypothesis: Countries with higher levels of urbanization tend to have lower marriage rates. Which showed that there is no significant relationship between urbanization and marriage rates in the dataset


## Findings
- No significant correlation was found between urbanization rates and marriage rates across the analyzed countries from 2010 to 2017.
- Also the Human Development Index (HDI) showed no statistically significant relationships with marriage rates.
- A significant correlation was found between unemployment rates and marriage rates, suggesting that economic conditions may influence marriage decisions.
- The Random Forest Regressor was the best-performing machine learning model for predicting marriage rates, though its overall accuracy was limited.


## Limitations and Future Work
One of the key limitations of the project was the availability and completeness of data. Many countries had to be excluded due to missing values, particularly in the marriage rates dataset. As a result, the dataset was limited in both size and diversity. Additionally, only socioeconomic variables were considered, which may not fully capture the complex factors that influence marriage behavior.

In future work, expanding the dataset to include more recent years and a broader range of countries could be valuable. Incorporating cultural datas uch as attitudes toward marriage or family structure could also provide a more comprehensive understanding.


## Conclusion
This project set out to explore the potential influence of urbanization on global marriage trends, with a particular focus on whether higher urbanization levels correlate with lower marriage rates. The study involved compiling and cleaning a rich set of global datasets covering a variety of socio-economic indicators from 2010 to 2017. These included marriage rates, urbanization percentages, GDP per capita, unemployment rates, the Human and Gender Development Indices, average schooling years, life expectancy, income inequality (Gini index), and working hours. Despite facing limitations such as missing data and the need for imputation, the datasets were merged into a unified form to facilitate statistical analysis and visualization.

The hypothesis that higher urbanization correlates with lower marriage rates was tested but found to lack statistical significance. Similarly, other expected relationships such as those between marriage rates and Human Development Index did not show strong evidence. Interestingly, unemployment rate emerged as the only variable with a significant correlation, suggesting that economic stability may play a more direct role in marriage decisions than urban living itself.

Machine learning modeling using a Random Forest Regressor provided some predictive capability but was limited by data sparsity and complexity of the phenomenon being modeled.

Overall, while urbanization alone does not appear to significantly affect marriage rates on a global scale, the findings highlight the importance of economic conditions and suggest that cultural and psychological factors could also play substantial roles. Future research could benefit from broader and more recent datasets, as well as the inclusion of cultural indicators to capture the full picture of marriage dynamics in the modern world.
