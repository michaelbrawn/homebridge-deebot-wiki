This functionality requires the [Eve App ➚](https://www.evehome.com/en/eve-app) to initially set up.

This will only work if your device supports mapping and different areas within the ECOVACS app.

### Obtain Spot Area IDs

The 'Spot Area IDs' are numbers which ECOVACS uses to determine a specific area on the map. These can be obtained by putting the plugin in debug mode and inspecting the logs. You should see log entries such as:

```
[Deebot] [Device] MapSpotAreaInfo: {"mapID":"125160527","mapSpotAreaID":"13","mapSpotAreaName":"Bedroom","mapSpotAreaConnections":"12,8,","mapSpotAreaBoundaries":"875,2875;875,4825;...","mapSpotAreaSubType":"1"}.
[Deebot] [Device] MapSpotAreaInfo: {"mapID":"125160527","mapSpotAreaID":"11","mapSpotAreaName":"Kitchen","mapSpotAreaConnections":"12,1,","mapSpotAreaBoundaries":"-775,-275;-775,-175;...","mapSpotAreaSubType":"5"}.
[Deebot] [Device] MapSpotAreaInfo: {"mapID":"125160527","mapSpotAreaID":"4","mapSpotAreaName":"Hall","mapSpotAreaConnections":"9,5,","mapSpotAreaBoundaries":"4125,-2825;4125,-2725;...","mapSpotAreaSubType":"3"}.
```

In this example we have:

* Bedroom with Spot Area ID `13`
* Kitchen with Spot Area ID `11`
* Hall with Spot Area ID `4`

### Configure Spot Areas

Use these numbers in the configuration to create the areas for the plugin to use, for example:

![Example config](https://user-images.githubusercontent.com/43026681/126316967-acb601a6-8888-4803-ad50-e7d2c398de12.png)

Here,
* Custom Area 1 relates to the Bedroom (with Spot Area ID 13)
* Custom Area 2 relates to the Kitchen (with Spot Area ID 11)
* Custom Area 3 relates to both the Kitchen and the Hall (with Spot Area IDs 4 and 11)