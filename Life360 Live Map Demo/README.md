# Life360 Live Map (OpenStreetMap) Demo

## Overview

This demo uses Life360 API to retrieve the circle member's geolocation (latitude & longitude), and display the location in the map using OpenStreetMap API. (This custom tile does NOT need the Life360 device in either SmartThings nor Hubitat.)


Please note that this is not an official Life360 integration but just to demo the possible integrations can be implemented via Custom Tile.

## Getting Started

### Authorize Life360 (Retrieve Access Token)
Follow the steps below to authorize your Life360 via Life360 OAuth and retrieve the access token:
* Go to "https://smart-life-360.glitch.me/" in the web browser
* Tap "Authorize" button, and sign in using your Life360 credential 
* When completed, tap the button to copy the access token to be used in the tile settings later.

### Create Custom Tile
* Tap [here](https://sharptools.io/developer/custom-tiles/import/?url=https%3A%2F%2Fraw.githubusercontent.com%2Fjamesguitar3%2FSharpTools_custom_tile_poc%2Fmain%2FLife360%2520Live%2520Map%2520Demo%2Fsource.html) to create the custom tile using this demo source code
* Save the Custom tile.

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Tap "Custom Tile" in the Other section and add this custom tile.

* Edit the tile and fill-in the Life360 access token and the other optional fields.  

* Save


### Done
