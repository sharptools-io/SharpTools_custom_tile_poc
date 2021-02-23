# Google Chart (Gauge) + Hubitat Make API Demo

## Overview
This demo uses Hubitat Maker API to retrieve the device's battery reading, and display the value in a gauge using Google Chart.

![Quick View](/Google%20Gauge%20Chart%20Demo/assets/gauge_tile.png)

## Getting Started

### Enable Hubitat Maker API 
Follow the steps below to enable Maker API in Hubitat admin page.
[Maker API](https://docs.hubitat.com/index.php?title=Maker_API)
* Select the devices that can be controled using this Maker API
* Enable "Allow Access via Remote/Cloud"
* Add "https://api.sharptools.io" in the **Allowed Hosts (for CORS)** field (to be updated)
* Scroll down and copy the Access Token generated

### Create Custom Tile
* Go to Developer Tools in SharpTools user dropdown
* Create a custom tile
    * Select "HTML" as Type
    * Add three "Settings" with "string" type        
        * token (Hubitat Maker API token created in the previous step)        
    ![settings](/Google%20Gauge%20Chart%20Demo/assets/tile_settings.png)    
    * Copy & paste the code from [here](/Google%20Gauge%20Chart%20Demo/source.html)

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Tap "Custom Tile" in the Other section and add this custom tile.

* Edit the tile and fill-in the Hubitat API token and Google MAP API Key from previous steps. 

  ![Edit custom tile](/Google%20Gauge%20Chart%20Demo/assets/tile_editor.png)

* Save

### Done