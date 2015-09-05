# d3 US Map of Favorite Pizza joints from ["Steve Kinney's Pizza Repo"](https://github.com/stevekinney/pizza)

![alt text](https://github.com/cluhring/us_pizza_d3_map/blob/master/pizza_usa.png)

Create an updated us.json file, if the pizza_map.geojson file changes, using the the below command in your terminal:

topojson -o us.json --id-property STATE_NAME --properties name=NAME --id-property SU_A3 --properties name=NAME --id-property pizzeria --properties name=NAME -- states.json subunits.json pizza_map.geojson

Created by following the Mike Bostock ["Lets Make a Map Tutorial"](http://bost.ocks.org/mike/map/)
with assistance from QGIS concepts learned from ["Gretchen Peterson's GIS Tutorial."](https://github.com/PetersonGIS/Maptime-Boulder-Pub-Map) as well as other d3 sites, including but not limited to: 1) Label hover helpers - ["tooltips"]("http://bl.ocks.org/Caged/6476579") & ["d3.tip"]("https://github.com/Caged/d3-tip"), 2) ["Zoom to Bounding Box II"]("http://bl.ocks.org/mbostock/9656675"), 3) topojson formatting helpers - ["Topojson Command Line Tools / GDAL"]("https://github.com/mbostock/topojson/wiki/Command-Line-Reference") & ["Topojson point"]("http://bl.ocks.org/mbostock/4408297")

start http-server by running "http-server -p 8008 &"

stop http-server by finding the Server PID# "lsof -i tcp:8008"
then "kill -9 INSERTPID#HERE"
