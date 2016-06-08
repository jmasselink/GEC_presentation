

## Managing large-scale wildlife data using *GIS*

Joel Masselink

GIS Developer

![Vulcan Technology](assets/VulcanTechnology-200sq.png "Vulcan Technology")
<!-- .slide: data-background="MintCream" -->
*June 23rd, 2016*



## What is the Great Elephant Census?

## How was GIS used to manage data?<!-- .element: class="fragment" data-fragment-index="1" -->

## Results + impacts of GEC<!-- .element: class="fragment" data-fragment-index="2" -->



## What is the GEC?

####Purpose: *provide accurate + current data regarding African savannah elephant population* <!-- .element: class="fragment" data-fragment-index="0" -->

*spatial data recorded from light aircraft*<!-- .element: class="fragment" data-fragment-index="1" -->

*funded by Paul Allen, cofounder of Microsoft*<!-- .element: class="fragment" data-fragment-index="2" -->


## GEC by the numbers:

- 20 countries<!-- .element: class="fragment" data-fragment-index="0" -->

- 90 scientists<!-- .element: class="fragment" data-fragment-index="1" -->

- 286 crew people<!-- .element: class="fragment" data-fragment-index="2" -->

- 81 airplanes <!-- .element: class="fragment" data-fragment-index="3" -->

- XX # of flights <!-- .element: class="fragment" data-fragment-index="4" -->

- 9700 hours of flight time<!-- .element: class="fragment" data-fragment-index="5" -->


## Spatial data collection

*Flight logger*<!-- .element: class="fragment" data-fragment-index="1" -->

*Aerial photographs*<!-- .element: class="fragment" data-fragment-index="2" -->

*Flight tracklogs*<!-- .element: class="fragment" data-fragment-index="3" -->

*Georeferenced Observations*<!-- .element: class="fragment" data-fragment-index="3" -->


## Project partners

####*Nonprofits*
_Elephants Without Borders_
_Wildlife Conservation Society_
_Frankfurt Zoological Society_

####*Government agencies*
_Tanzania Wildlife Research Institute_
_South Africa_
_20 countries had data collection agreements_

####*Scientists*
_IUCN African Elephant Specialist Group_




###*Distributed networks (Twitter)*<!-- .element: class="fragment" data-fragment-index="5" -->


## Tools used by GEC
_open SQL database backend_<!-- .element: class="fragment" data-fragment-index="0" -->

_Excel template_<!-- .element: class="fragment" data-fragment-index="1" -->

_*discrete geographic features*_<!-- .element: class="fragment" data-fragment-index="3" -->

_Points_<!-- .element: class="fragment" data-fragment-index="4" -->

_Lines_<!-- .element: class="fragment" data-fragment-index="5" -->

_Polygons_<!-- .element: class="fragment" data-fragment-index="6" -->


##*answering questions*:

_WHERE is the largest concentration of elephants in Tanzania?_<!-- .element: class="fragment" data-fragment-index="1" -->

_WHERE is fishing the most intensive and targeting which species?_<!-- .element: class="fragment" data-fragment-index="2" -->

_WHERE are poaching entry points to Lewa?_<!-- .element: class="fragment" data-fragment-index="3" -->


## GIS Tasks
- *compile & process data*<!-- .element: class="fragment" data-fragment-index="1" -->

- *analyze data* <!-- .element: class="fragment" data-fragment-index="2" -->

- *design & visualize results*<!-- .element: class="fragment" data-fragment-index="3" -->



## Trends in the Industry

_Spatial is no longer Special_<!-- .element: class="fragment" data-fragment-index="0" -->

_Powerful databases_<!-- .element: class="fragment" data-fragment-index="1" -->

_Cloud Computing_<!-- .element: class="fragment" data-fragment-index="2" -->

_Open Data_<!-- .element: class="fragment" data-fragment-index="3" -->

_Mobile/distributed data collection_<!-- .element: class="fragment" data-fragment-index="4" -->

_Micro-satellites & Drones_<!-- .element: class="fragment" data-fragment-index="5" -->



##Databases w/ spatial extensions

###_SQL integration with PostGIS_

```
SELECT a.name, ST_Distance(c.geom, a.geom, true) * 0.000621371 AS distance_as_miles
FROM geo.cities_ne c
CROSS JOIN transport.airports_ne a
WHERE c.name = 'Seattle'
ORDER BY ST_Distance(c.geom, a.geom, true) ASC
LIMIT 1;
```



##*Software*

###_Open Software_

_Python integrated into GIS software_

_GeoJSON objects_

_R statistical analysis software_


###**QGIS**

_Full-featured desktop software_<!-- .element: class="fragment" data-fragment-index="0" -->

_Free and open-source_<!-- .element: class="fragment" data-fragment-index="1" -->

_Integrates with other Open source software/tools_<!-- .element: class="fragment" data-fragment-index="2" -->

_Robust development and user group_<!-- .element: class="fragment" data-fragment-index="3" -->


###**Mapbox**

_Free and open-source_<!-- .element: class="fragment" data-fragment-index="0" -->

_Design, data visualization for web_<!-- .element: class="fragment" data-fragment-index="1" -->

_Vector Tiles_<!-- .element: class="fragment" data-fragment-index="2" -->

_Raster Tiles_<!-- .element: class="fragment" data-fragment-index="3" -->


###**Esri**<!-- .element: class="fragment" data-fragment-index="0" -->

_Proprietary software_<!-- .element: class="fragment" data-fragment-index="1" -->

_Private company_<!-- .element: class="fragment" data-fragment-index="2" -->

_Huge customer base_<!-- .element: class="fragment" data-fragment-index="3" -->

_Purveyors of the "Shapefile"_<!-- .element: class="fragment" data-fragment-index="4" -->


**Other spatial software:**

_CartoDB_<!-- .element: class="fragment" data-fragment-index="0" -->

_Tableau_<!-- .element: class="fragment" data-fragment-index="1" -->



##Cloud Computing##

_Landsat stored in Amazon S3 buckets_<!-- .element: class="fragment" data-fragment-index="0" -->


_Google Earth Engine_

<iframe width="1080" height="600" src="https://earthengine.google.com/iframes/timelapse_player_embed.html#v=36.13528,-115.03715,10,latLng&t=0.15" frameborder="0"></iframe>


_Live demo_
[Google Earth Engine playground](https://code.earthengine.google.com/3b2621f0a08e7549fd1fcb4234a109e6)



###Open Data & Open Source

_OpenStreetMap (OSM)_<!-- .element: class="fragment" data-fragment-index="0" -->

![_OpenStreetMap (OSM)_](assets/100px-Openstreetmap_logo.svg.png "OSM")<!-- .element: class="fragment" data-fragment-index="0" -->

_OpenDroneMap_<!-- .element: class="fragment" data-fragment-index="1" -->

_OpenAerialMap_<!-- .element: class="fragment" data-fragment-index="2" -->


![HOT](assets/HOT_logo.png "HOT")<!-- .element: class="fragment" data-fragment-index="0" -->

_"applies the principles of open source and open data sharing for humanitarian response and economic development."_<!-- .element: class="fragment" data-fragment-index="1" -->



# Thank you!

Contact: joelm@vulcan.com

[jmasselink.github.io](jmasselink.github.io)


## Thank you!

*Vulcan colleagues*
Kirk Larsen
Kathleen Gobush
Ted Schmitt

_alukach_ of Maptime Calgary for this presentation template

Christy Heaton of Maptime Seattle

Cascadia User Group of Open Source Geo **(CUGOS)**

MapTime Seattle

OpenStreetMap Seattle



and others who have helped me

> Written with [StackEdit](https://stackedit.io/).