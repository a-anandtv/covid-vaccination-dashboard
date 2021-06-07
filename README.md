# Covid Vaccination Dashboard
An analytic dashboard for the world covid vaccination data collected from the ourworldindata.com database. The data is then hosted in a postgreSQL database and used in Tableau to design the dashboard. 

### Dashboard design
The design for the dashboard was influenced by the impfdashboard.de design.

<p align="center">
  <img src="https://github.com/a-anandtv/covid-vaccination-dashboard/blob/main/resources/vaccination_progress.png" >
</p>

#### Concepts used in the dashboard:
* Aggregate Measures
* Ranked Measures
* Measures matching with a calculated aggregate field
* Bar charts, Line Charts and Area charts
* Map with dynamic refresh based on filters
* Dynamic texts
* Common filters that apply to the entire dashboard workspace
* Cascading and relevant filters
* Ranking filters to display only top vaccinated countries
* Null value checks, data consistency checks and other data cleanses done with Tableau

### Data Architecture
Data was initially downloaded in a single csv file with all the data as columns.
This was then split into two staging files, with each file holding data corresponding to one particular relevent subject: vaccinations and cases/deaths respectively.
Data from the staging tables were then cleaned, transformed and then loaded into an analytical database with a star shaped model.

### SQL/Data engineering
SQL was used to further clean and organize the data. And also to calculate aggregate measures, which were then collected into views to be used in Tableu for the dashboard.

#### SQL skills used
Constraints, Joins, Unions, CTEs, Window functions, Inner queries, Sub queries, Aggregates functions, Analytical functions, Text conversions, Date extractions, Data type conversions, temp tables and Creating Views.
