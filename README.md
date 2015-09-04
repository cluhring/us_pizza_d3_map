# d3 Map of the USA

mapping data points from ["Steve Kinney's Pizza Repo"]https://github.com/stevekinney/pizza

![alt text](https://github.com/cluhring/us_pizza_d3_map/blob/master/pizza_usa.png)

Create an updated us.json file, if the pizza_map.geojson file changes.

topojson -o us.json --id-property STATE_NAME --properties name=NAME --id-property SU_A3 --properties name=NAME --id-property pizzeria --properties name=NAME -- states.json subunits.json pizza_map.geojson

start http-server by running "http-server -p 8008 &"
stop http-server by finding the Server PID# "lsof -i tcp:8008"
then "kill -9 INSERTPID#HERE"

Created by following the Mike Bostock ["Lets Make a Map Tutorial"](http://bost.ocks.org/mike/map/)
with assistance from QGIS concepts learned from ["Gretchen Peterson's GIS Tutorial"](https://github.com/PetersonGIS/Maptime-Boulder-Pub-Map)
