# Life360 Live Map (OpenStreetMap)Demo

## Overview

This demo uses Life360 API to retrieve the circle member's geolocation (latitude & longitude), and display the location in the map using OpenStreetMap API. (This custom tile does NOT need the Life360 device in either SmartThings nor Hubitat.)


Please note that this is not an official Life360 integration but just to demo the possible integrations can be implemented via Custom Tile.

## Getting Started

### Authorize Life360 (Retrieve Access Token)
Follow the steps below to authorize your Life360 via Life360 OAuth and retrieve the access token:
* Go to "https://geode-pie-thistle.glitch.me/" in the web brower
* Tap "Authorize" button, and sign in using your Life360 credential 
* When the authorization is compeled, tap the blurred token field and copy the access token.
* (Optional) Click on "Get Circles" in the page and verify the retrieved the circle information. Copy the Circle ID from the retrieved data to be used in the Tile Settings.
* (Optional) Click on "View" next to the Members under the retrieved Circle informaiton and copy the desired User ID to be used in the Tile Settings.


### Create Custom Tile
* Tap the link to create the custom tile using this demo source code
* Save the Custom tile.

### Deploy Custom Tile
* Go to the desired dashboard, Edit, and Add Item. Tap "Custom Tile" in the Other section and add this custom tile.

* Edit the tile and fill-in the Life360 access token and the other optional fields.  

* Save


### Done
