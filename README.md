# COVID_19

Code One: Viewing continent where values are not null.

===> Select *
From [COVID-19_data]..CovidDeaths$
Where continent is not null 
order by 3,4 <===

Code Info: The provided SQL code retrieves all columns from the table `CovidDeaths$` in the schema `[COVID-19_data]`, where the `continent` column is not null. The result is ordered by the third and fourth columns.

Code result:
![Cap a1](https://github.com/jona00001/Covid-19_Project/assets/108422584/bd293ac1-80d3-425c-a032-205f90cb3325)


Code Two: Viewing continent where values are not null.

===>Select Location, date, total_cases, new_cases, total_deaths, population
From [COVID-19_data]..CovidDeaths$
Where continent is not null 
order by 1,2 <===

Code Info:The given SQL code retrieves data from the table CovidDeaths$ and selects specific columns: Location, date, total_cases, new_cases, total_deaths, and population. The FROM clause specifies the source table [COVID-19_data]..CovidDeaths$.

Code result:![Cap a2](https://github.com/jona00001/Covid-19_Project/assets/108422584/38430f5b-35be-4d3f-bb86-351b0216e5da)









