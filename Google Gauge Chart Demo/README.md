# Google Chart (Gauge) + Hubitat Make API Demo

## Overview
This demo uses Hubitat Maker API to retrieve the device's battery reading, and display the value in a gauge using Google Chart.

![Quick View](/Google%20Gauge%20Chart%20Demo/assets/gauge_tile.png)

## Getting Started

### Enable Hubitat Maker API 
Follow the steps below to enable Maker API in Hubitat admin page.
[Maker API](https://docs.hubitat.com/index.php?title=Maker_API)
* Select the devices that can be controlled using this Maker API
* Enable "Allow Access via Remote/Cloud"
* Add "https://run.sharptools.app" in the **Allowed Hosts (for CORS)** field
* Scroll down and copy one of the example cloud endpoints
* Make sure to press "Done" to save your changes!

### Create Custom Tile
* Go to Developer Tools in SharpTools user dropdown
* Create a custom tile
    * Select "HTML" as Type
    * Copy & paste the code from [here](/Google%20Gauge%20Chart%20Demo/source.html)
    * Tap out of the code editor and accept the new settings

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Tap "Custom Tile" in the Other section and add this custom tile.

* Edit the tile and fill-in the settings:
  * Hubitat Maker API example - use one of the Hubitat Maker API Cloud endpoints
  * Device ID -  enter the ID of a device with a battery attribute

  ![Edit custom tile](/Google%20Gauge%20Chart%20Demo/assets/tile_editor.png)

* Save