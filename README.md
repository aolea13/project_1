## Project 1: Home Value Patterns Due to COVID-19

By: Jason Sheridan, Anna Sours, Jenni Davis, Austin Olea, & Mark Blankenship


### Hypothesis: Where COVID-19 cases are higher in counties with major cities, home values will increase in the surrounding counties.

#### Guiding Questions:
* How are people migrating throughout the US since COVID 19 began?
* Has this impacted home values? 
* Is there a relationship between cases and the housing market? 

### Data Sources:
#### COVID-19 Cases: 
* NY Times US states & counties
* Texts files with state, county, date, cases, etc. 
* US census data
  * Shapefiles 
* API calls
  * Coordinates
* New dependencies for mapping
  * geopandas
  * folium 

#### Home values:
* Zillow Home Value Index (ZHVI) from zillow.com
  * CSV files updated monthly
  * ZHVI values for Metro & U.S. 
  * Monthly values from 1/31/1996 - 12/31/2020

### COVID-19 Data Exploration
#### Analysis 1: 
##### NY Times US states & counties
  * Q: What states have the highest count of COVID-19 cases? And of those states, which counties had the highest  count of COVID-19 cases? 


##### Exploration & Data Wrangling: 
* NY Times data
  *US states & counties data - date, state, county, cases, etc.

    * Methods: 
      * Filtering
      * Grouping
      * Stats
      * Dropping values
      * Sorting values
      * Horizontal bar chart

#### Analysis 2: 
##### API calls, US census data & geopandas
  * Q: Can we take the NYTimes data and layer it onto a map of the United States and have it display state name and maximum case counts?

##### Exploration & Data Wrangling: 
* API calls
  *Coordinates
* US census data
  *Shapefiles 
*  Geopandas


  *Methods: 
    * API calls 
    * Shapefiles
    * Export/Import csv files
    * More: filtering, grouping, dropping
    * Adding/renaming columns
    * Merging

![USmapColorbar.png](Image/USmapColorbar.png?raw=true "Title")

* States determined for further analysis:
  * California
  * Texas
  * Florida
  
  
#### Analysis 3: 
##### More mapping…?
  * Q: Can we use heat maps and markers to better highlight the counties with maximum cases and their surrounding counties?

##### Exploration & Data Wrangling: 
* Folium
  * Mapping library 

  * Methods: 
    * Gmaps 
    * Heatmaps
    * Folium
    * Lists...
    * Lists of coordinates...
    * Lists of cities...
    * LISTS!

### Home Values of Counties with high COVID-19 Cases
#### California
![tri_county_zhvi.png](output/tri_county_zhvi.png?raw=true "Title")

#### Florida
![highest_covid_counties_fl.png](output_data/highest_covid_counties_fl.png?raw=true "Title")

#### Texas
![county_lines.png](county_lines.png?raw=true "Title")

### Percent Change in Home Values 

#### California
![los_angles_metro.png](output_data/los_angles_metro.png?raw=true "Title")

#### Florida
![miami_metro_county.png](output_data/miami_metro_county.png?raw=true "Title")

#### Texas
![dfwmetro2.png](dfwmetro2.png?raw=true "Title")

![houstonmetro2.png](houstonmetro2.png?raw=true "Title")
