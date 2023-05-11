# COVID_19

Code One: Viewing continent where values are not null.

===> Select *
From [COVID-19_data]..CovidDeaths$
Where continent is not null 
order by 3,4 <===

Code Info:
The provided SQL code retrieves all columns from the table `CovidDeaths$` in the schema `[COVID-19_data]`, where the `continent` column is not null. The result is ordered by the third and fourth columns.

Code result:
![Cap a1](https://github.com/jona00001/Covid-19_Project/assets/108422584/bd293ac1-80d3-425c-a032-205f90cb3325)


Code Two:Viewing continent in relation to Location, date, total_cases, new_cases, total_deaths, population.

===>Select Location, date, total_cases, new_cases, total_deaths, population
From [COVID-19_data]..CovidDeaths$
Where continent is not null 
order by 1,2 <===

Code Info:
The given SQL code retrieves data from the table CovidDeaths$ and selects specific columns: Location, date, total_cases, new_cases, total_deaths, and population. The FROM clause specifies the source table [COVID-19_data]..CovidDeaths$.

Code result:![Cap a2](https://github.com/jona00001/Covid-19_Project/assets/108422584/38430f5b-35be-4d3f-bb86-351b0216e5da)

Code Three:

===>Select Location, date, total_cases,total_deaths, (total_deaths/total_cases)*100 as DeathPercentage
From [COVID-19_data]..CovidDeaths$
Where location like '%states%'
and continent is not null 
order by 1,2 <===

Code Info: 
The given SQL code retrieves data from the table [COVID-19_data]..CovidDeaths$ and calculates the death percentage for each location and date.

Code result:![cap a-Code three](https://github.com/jona00001/Covid-19_Project/assets/108422584/a71a5bf2-887a-4edf-922b-dec72519cc3c)



Code Four:

===>Select Location, date, Population, total_cases,  (total_cases/population)*100 as PercentPopulationInfected
From [COVID-19_data]..CovidDeaths$
--Where location like '%states%'
order by 1,2 <===

Code Info: 
The given SQL code retrieves data from the table CovidDeaths$ in the schema [COVID-19_data]. It selects the columns Location, date, Population, and total_cases from the table. Additionally, it calculates the percentage of the population infected by dividing total_cases by population and multiplying by 100. The result of this calculation is aliased as PercentPopulationInfected.

Code result:![Cap a4](https://github.com/jona00001/Covid-19_Project/assets/108422584/83bad828-f9de-4105-a3ae-824fd9894a8d)







