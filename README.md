# TTC_Headway_Archive_Dec11-Dec18

This repo contains archived NextBus data from Dec11 to Dec 18 of 2016.

To generate your own archive, run `node gen_files.js` to create the folders for all the TTC routes.

Then run `node head.js` to continuously pull data from the restbus API.

Note: you are using their public API (http://restbus.info/). If you plan to be courteous, run their script on your own servers.

The first row of the text file will contain the route's name.
The next row will contain information about the routes in this fashion:
	`routestops: stopid~stopcode~stoptitle~stoplat~stoplon`
Finally, the succeeding lines contain information regarding the busses in the following fashion:
	`vehicleid~directionid~headingid~lat~lon`
Note how the grave symbol `~` is used as a delimiter.

All the files between the dates `Dec11-Dec18`  will be stored in its respective folder.
