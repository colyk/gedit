
```
import gedit as gd
bbox = gd.geotypes.Bbox(min_lat=51.1, min_lon=22.2, max_lat=51.2, max_lon=22.3)
geojson = gd.fetch(bbox=bbox, type=”pedestrian_way”).to_geojson()
graph = gd.graph.from_geojson(geojson)
graph.show()
```
