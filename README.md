#Map Your Farmer’s Market

##Goal

To create an accurate map of a Farmer's Market (suitable for submission to USDA) that can also be used on the web for visitors to find vendors, amenities, parking, etc.

##Current Software

- QGIS
- LibreCAD

##Current Website Sources

- http://viewer.nationalmap.gov/viewer/

##Current Process
(rough outline - details coming soon)

1. using national map viewer, locate area of market and download 1-foot resolution aerial imagery
2. place imagery in QGIS
3. zoom into market area and create line layer indicating boundaries of market, areas where stalls are, etc. (use local state/plane projection)
4. export line layer as DXF format
5. open DXF format in LibreCAD and auto-zoom to market area
6. measure angle of market space (in case space is not perfectly north aligned)
7. create outlines of stalls and other amenities (if necessary, rotate outlines by angle determined in previous step)
8. hatch solid fill the outlines (these will appear as polygons when opened in QGIS)
9. save DXF
10. open DXF in QGIS
11. save layer as shapefile to make editable
12. modify new layer to fill in attributes appropriate for market stalls and amenities (stall numbers, descriptions, etc.)
