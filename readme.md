Geom99lab3
canada map representation bonus: https://jordantishler.github.io/geom99lab3/canada.html

how to upload a file to arcgis online 

step one: add a new ArcGIS online server using this link : https://luna.flemingcollege.ca:6443/arcgis use on the this port when connecting and sign in useing adroot.

Step two make sure the file you are using is in cdrive/gisworkshop/canada and then make sure you have a publisher connectection and can share.

step 3: when sharing add in the map as a map service and anlyze each error 

step4: fix the error turn on numeric ID's and turn off the basemaps register the file folder if needed (it has already been done with canada file bause this same folder was used.

step 5: add tags and a name and a summary

Step 6: manage the amp service and sign in to get the rest url/api

Step 7: delete at this site if you already have one. : https://luna.flemingcollege.ca:6443/arcgis/manager/ sign in normally with adroot in user name 

week 5 examples: https://github.com/shawnmflemingc/geom99/blob/main/arcgisrest.md

use the qurey: https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0/query?where=capital%3D%27Y%27&geometry=%7Bxmin%3A+-104%2C+ymin%3A+35.6%2C+xmax%3A+-94.32%2C+ymax%3A+41%7D&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&outFields=objectid%2Careaname%2Cst&returnGeometry=true&orderByFields=areaname&f=html

Week 5 example 1: https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0/query?where=st%3D%27GA%27&text=&objectIds=&time=&timeRelation=esriTimeRelationOverlaps&geometry=&geometryType=esriGeometryEnvelope&inSR=&spatialRel=esriSpatialRelIntersects&distance=&units=esriSRUnit_Foot&relationParam=&outFields=*&returnGeometry=true&returnTrueCurves=false&maxAllowableOffset=&geometryPrecision=&outSR=&havingClause=&returnIdsOnly=false&returnCountOnly=false&orderByFields=pop2000%27desc%27&groupByFieldsForStatistics=&outStatistics=&returnZ=false&returnM=false&gdbVersion=&historicMoment=&returnDistinctValues=false&resultOffset=&resultRecordCount=&returnExtentOnly=false&sqlFormat=none&datumTransformation=&parameterValues=&rangeValues=&quantizationParameters=&featureEncoding=esriDefault&f=html or https://sampleserver6.arcgisonline.com/arcgis/rest/services/USA/MapServer/0/query?where=st+%3D+%27GA%27&outFields=*&returnGeometry=true&orderByFields=pop2000+desc&f=html
records: 82

Week5 example 2: https://sampleserver6.arcgisonline.com/arcgis/rest/services/Earthquakes_Since1970/MapServer/0/query?where=magnitude+%3E%3D+8.3&outFields=*&returnGeometry=false&f=html 
Bonus:
The question was for the number of earthquakes, and there is a parameter called returnCountOnly=true that would do this and be quicker to respond with only a count of the number of records. Can you just return the count?
yes just use this: https://sampleserver6.arcgisonline.com/arcgis/rest/services/Earthquakes_Since1970/MapServer/0/query?where=magnitude+%3E%3D+8.3&text=&objectIds=&time=&timeRelation=esriTimeRelationOverlaps&geometry=&geometryType=esriGeometryEnvelope&inSR=&spatialRel=esriSpatialRelIntersects&distance=&units=esriSRUnit_Foot&relationParam=&outFields=*&returnGeometry=false&returnTrueCurves=false&maxAllowableOffset=&geometryPrecision=&outSR=&havingClause=&returnIdsOnly=false&returnCountOnly=true&orderByFields=&groupByFieldsForStatistics=&outStatistics=&returnZ=false&returnM=false&gdbVersion=&historicMoment=&returnDistinctValues=false&resultOffset=&resultRecordCount=&returnExtentOnly=false&sqlFormat=none&datumTransformation=&parameterValues=&rangeValues=&quantizationParameters=&featureEncoding=esriDefault&f=html
records: 7

Week5 example 3: https://sampleserver6.arcgisonline.com/arcgis/rest/services/AGP/Hurricanes/MapServer/0/query?where=1%3D1&outFields=EVENTID+&returnGeometry=false&returnDistinctValues=true&f=html

records: 14
