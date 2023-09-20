# OpenStreetMap + Hubitat Maker API (Life360) Demo


>🛑 <strong>Warning:</strong>  
> Use the new version at https://community.sharptools.io/t/life360-live-map/7135
>
> The new version talks *directly* to Life360, so it isn't dependent on Hubitat or a custom driver. 


## Overview

This demo uses Hubitat Maker API to retrieve the device's geolocation (latitude & longitude), and display the location in the map using OpenStreetMap API.

![Quick View](/Google%20Map%20Demo/assets/live_map_tile.png)

Please note that this is using a Hubitat community developed smartapp and device driver to access Life360 geolocation info. For SmartThings users, the community developed device driver needs to be updated with the new Custom Capability before the new SmartThings REST API can retrieve these custom attributes. Or the alternative option is to access Life360 API directly to get the latitude and longitude info. See below for the detailed information and these implementation are not the "official" connection on either platform.

* [Hubitat Community Developed Life360 Smartapp & Device Driver - by bptworld](https://github.com/bptworld/Hubitat/tree/master/Ported)

* [SmartThings Community Developed Life360 Smartapp - by tmleafs](https://github.com/tmleafs/life360-smartthings-refresh/tree/master/smartapps/tmleafs/life360-connect.src).


## Getting Started

### Enable Hubitat Maker API 
Follow the steps below to enable Maker API in Hubitat admin page.
[Maker API](https://docs.hubitat.com/index.php?title=Maker_API)
* Select the devices that can be controled using this Maker API
* Enable "Allow Access via Remote/Cloud"
* Add "https://run.sharptools.app" in the **Allowed Hosts (for CORS)** field
* Scroll down and copy the Access Token generated

### Create Custom Tile
* Go to Developer Tools in SharpTools user dropdown
* Create a custom tile
    * Select "HTML" as Type
    * Create four settings (String type)
    ![settings](/Google%20Map%20Demo/assets/custom_tile_settings.png)        
        * Sample Maker API URL: can be found in the Hubitat Maker API page.
          ![smaple_url](/Google%20Map%20Demo/assets/sample_cloud_url.png)
        * Life360 Device Id: Hubitat device id for Life360. Can be found by going to [SharpTools User Page](https://sharptools.io/user), tap `...` next to the Hubitat location in the Authorized Locations section, select the Life360 device, and toggle the Advanced option in the device page.
          ![settings](/Google%20Map%20Demo/assets/find_device_id.png)
        * Avatar Image Url (optional): the image you want to display in the map
        * Map Source (optional): four different map styles - default, bright, light, and dark.
        
    * Set default dimensons to 2x2
    * Copy & paste the code from [here](/Google%20Map%20Demo/source.html)

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Tap "Custom Tile" in the Other section and add this custom tile.

* Edit the tile and fill-in the Hubitat Maker API sample URL and Life360 device id.

  ![Edit custom tile](/Google%20Map%20Demo/assets/tile_editor.png)

* Save


### Done
