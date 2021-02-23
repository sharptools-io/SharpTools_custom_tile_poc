# Google Chart (Line Chart) + COVID-19 Status Demo

## Overview
This demo uses [DISEASE.SH](https://github.com/disease-sh/api) API to retrieve COVID-19 historical data based on the specified state and county, and display the data in a line chart using Google Chart.

![Quick View](/Google%20Line%20Chart%20Demo/assets/covid_chart_tile.png)

## Getting Started

### Create Custom Tile
* Go to Developer Tools in SharpTools user dropdown
* Create a custom tile
    * Select "HTML" as Type
    * Add three "Settings" with "string" type        
        * state 
        * county
    * Set the defaul dimensions to 2x3
    ![settings](/Google%20Line%20Chart%20Demo/assets/tile_settings.png)    
    * Copy & paste the code from [here](/Google%Line%20Chart%20Demo/source.html)

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Tap "Custom Tile" in the Other section and add this custom tile.

* Edit the tile and fill-in the Hubitat API token and Google MAP API Key from previous steps. 

  ![Edit custom tile](/Google%20Line%20Chart%20Demo/assets/tile_editor.png)

* Save

### Done