# Bangalore_Metro_Accessibility_Qgis

This Qgis Project tries to calculate the percentage population of Bangalore living close to metro stations (ie in 1 Km radius of every metro station) thus trying to give an indication of accessabilty of metro in Bangalore.


Data sources use : 

1) Population count : wordpop.org (https://www.worldpop.org/geodata/summary?id=49992)
2) Metro stations location : Overpass API (API accessed using Quick OSM in Qgis)
3) Bangalore map : spatialthoughts.com (https://docs.google.com/forms/d/e/1FAIpQLSdwB5I9PdheF8V4yOSeoGSkmEdBZoe4R9CyFQVzlFH-pTl6FQ/viewform)


Important Steps:
1) Under-construction and unconnected metro stations are filtered out using QGIS tools
2) A buffer zone of 1Km radius is created around metro stations by temporarly reprojecting the metro data layer to the Datum :EPSG:32643 - WGS 84 UTM
3) Calculating the population residing in bangalore and 'Areas near metro stations' by apllying the QGis tool 'Zonal Statistics'

