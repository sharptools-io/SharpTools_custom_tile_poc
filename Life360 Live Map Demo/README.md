# Life360 Live Map (OpenStreetMap) Demo

![overview](/Life360%20Live%20Map%20Demo/assets/live_map.png)       

## Overview
This demo uses Life360 API to retrieve the members' geolocations from your Life360's circle(s), and display the member(s) in the map using OpenStreetMap API. (This custom tile does NOT need the Life360 device in either SmartThings nor Hubitat.)

This custom tile display all the members from your Life360 circles by default, and you can add the users' emails in the User Filter field to control what users to be disaplyed in the map.

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


### Configure Custom Tile
These steps assume you've already imported the custom tile using the button toward the top of this page.
* Add the tile to your dashboard from Add Item -> Other -> Custom Tile
* Tap the `...` in the top-right corner of the newly added tile and select **Edit**
* Paste the **Life360 Access Token** from the steps above. 
* If you have multiple members in your circle(s) and would like to specify a set of users, you can add their Life360 user emails in the **User Filter* field and separate them by comma.
![tile settings](/Life360%20Live%20Map%20Demo/assets/tile_settings.jpeg)

### Optional Settings
* **Map Source** - customize the map appearance with 'bright', 'light', or 'dark' 
   * See [this post](https://community.sharptools.io/t/life-360-hubitat-map-tile/6596/26?u=josh) for screenshots and further details
* **User Filter** - input the email addresses or ids of the Life360 users from your circles to filter the users to be displayed in the map.
  * The [authorization page](https://smart-life-360.glitch.me/) has a utility under Get Circles -> View Members to confirm email addresses
* **Display User's Name** - check to display the user's first name under the user's avatar or pin image
* **Use Pin Icon** - check to use the pin image to mark the user in the map, instead of using the user's avatar image
![pin markers](/Life360%20Live%20Map%20Demo/assets/pin_markers.jpeg)

### Done
