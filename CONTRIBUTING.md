This repository is to help you to contribute a new map to [White Cargo Van](http://www.whitecargovan.com). All maps are 
stored in [GeoJson](http://geojson.org/) format with the following caveats/conventions:
 1. All maps have the name of the race (Camel Case) prefixed with the year that they were valid. Not all races update their maps, but this should help track things down.
 2. Please do the exchange points (plus finish line) as a `FeatureCollection` of `Feature` with `"type":"Point"`.
 3. Each point should have the additional `properties` of `leg`, `miles`, and `name` if possible.
 4. The finish line should have a terminator `properties` of `"miles": 0.0, "name": "Finish"` to aid in automatically marking it in the online widgets and tools.
