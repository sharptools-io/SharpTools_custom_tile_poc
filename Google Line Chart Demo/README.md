# Google Chart (Line Chart) + COVID-19 Status Demo

## Overview
This demo uses [DISEASE.SH](https://github.com/disease-sh/api) API to retrieve COVID-19 historical data based on the specified state/county and displays the data in a line chart using Google Charts.

![Quick View](/Google%20Line%20Chart%20Demo/assets/covid_chart_tile.png)

## Getting Started

### Create Custom Tile
* Go to Developer Tools in SharpTools user dropdown
* Create a custom tile
    * Select "HTML" as the Type
    * Add two "Settings" with "STRING" type        
        * `state`
        * `county`
    * Set the default dimensions to 2x3
    ![settings](/Google%20Line%20Chart%20Demo/assets/tile_settings.png)    
    * Copy & paste the **raw** code from [here](/Google%Line%20Chart%20Demo/source.html)

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Expand the 'Other' section and select "Custom Tile", then add this custom tile.

* Edit the tile and fill-in the desired state and county. 

  ![Edit custom tile](/Google%20Line%20Chart%20Demo/assets/tile_editor.png)

* Tap **Save**