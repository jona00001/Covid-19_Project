# COVID_19

Code One: Viewing continent where values are not null.

===> Select *
From [COVID-19_data]..CovidDeaths$
Where continent is not null 
order by 3,4 <===

Code Info: The provided SQL code retrieves all columns from the table `CovidDeaths$` in the schema `[COVID-19_data]`, where the `continent` column is not null. The result is ordered by the third and fourth columns.

Code result:
![Cap a1](https://github.com/jona00001/Covid-19_Project/assets/108422584/bd293ac1-80d3-425c-a032-205f90cb3325)


Code Two: Viewing continent in relation to Location, date, total_cases, new_cases, total_deaths, population.

===>Select Location, date, total_cases, new_cases, total_deaths, population
From [COVID-19_data]..CovidDeaths$
Where continent is not null 
order by 1,2 <===

Code Info:The given SQL code retrieves data from the table CovidDeaths$ and selects specific columns: Location, date, total_cases, new_cases, total_deaths, and population. The FROM clause specifies the source table [COVID-19_data]..CovidDeaths$.

Code result:![Cap a2](https://github.com/jona00001/Covid-19_Project/assets/108422584/38430f5b-35be-4d3f-bb86-351b0216e5da)

Code Three:

===>Select Location, date, total_cases,total_deaths, (total_deaths/total_cases)*100 as DeathPercentage
From [COVID-19_data]..CovidDeaths$
Where location like '%states%'
and continent is not null 
order by 1,2 <===

Code Info: The given SQL code retrieves data from the table [COVID-19_data]..CovidDeaths$ and calculates the death percentage for each location and date.

Code result:![Cap a3](https://github.com/jona00001/Covid-19_Project/assets/108422584/6c2874c0-814c-4876-901b-7b9cf3479e2b)











