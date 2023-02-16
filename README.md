# SQLPortfolioProject

# Covid 19 Data Exploration 

This is an analysis that shows information about covid total number of cases, number of deaths and number of people vaccinated in the world.

Skills used: Joins, Converting Data Types, CTE's, Temp Tables, Windows Functions, Aggregate Functions, Creating Views, 

# Project Overview

The dataset used for this analysis was obtained from:

Coronavirus Pandemic (COVID-19)
Research and data: Edouard Mathieu, Hannah Ritchie, Lucas Rodés-Guirao, Cameron Appel, Daniel Gavrilov, Charlie Giattino, Joe Hasell, Bobbie Macdonald, Saloni Dattani, Diana Beltekian, Esteban Ortiz-Ospina, and Max Roser
which can be accessed here "https://ourworldindata.org/coronavirus"

The data is in an excel sheet

# Data Cleaning
The data set were split into two files:

1. Named CovidDeaths contained the data as regards the cases detected and the reported death counts per day
- Some columns from the original dataset that were not necessary to the covid death analysis were removed

2. Named CovidVaccinations contained the data as regards the number of people vaccinated per day
- Some columns from the original dataset that were notnecessary t the covid vaccination analysis were also excluded.

# Data Processing

The cleaned dataset were imported to SQL for further analysis. The SQL script is uploaded in this repo.

[screenshot.docx](https://github.com/FolakeFadare/SQLPortfolioProject/files/10758989/screenshot.docx)

# Data Exploration and Analysis

For CovidDeaths had dataset with 170,342 rows but when the columns with continents as 'null' were removed, we have 162,120 rows which were used for further analysis.
For CovidVaccinations had dataset with 85,171,rows while we worked wih 81,060 rows after excluding the the column continents with null values and were also used for further analysis

* Exploring the total number of cases, total number of deaths and the death rates at specific dates for specific countries
  ### At the end of 2020
      In Nigeria, the total number of cases was 87 607 with total deaths being 1 289 which was 1.47% Death rate.
      In  United States, the total number of cases  was 20 099 363 with a death rate of 1.75 which was 352 093 deaths.

  ### On the 30th of April, 2021:
      In Nigeria, the total_cases was 165,110 while the total_deaths was 2,063 while Death_rate was 1.25.
      In United States the total_cases was 32,346,971 while total_deaths was 576,232 with a death_Rate of 1.78.

* The top 10 countries in the world with the highest infected population are:
      1. Andorra (17.15%)
      2. Montenegro (15.5%)
      3. Czechia (15.22%)
      4. San Marino (14.9%)
      5. Slovenia (11.55%)
      6. Luxembourg (10.7%)
      7. Bahrain (10.3%)
      8. Serbia (10.13%)
      9. United States (9.77%)
      10. Israel (9.68%)

* The top 5 countries with the highest death count:
1. United States 576,232
2. Brazil 403,781
3. Mexico 216,907
4. India 211,853
5. United Kingdom 127,775

* Grouping the death counts according to continents revealed Europe as the highest followed by North America



