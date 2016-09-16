# Cuba in QGIS: Adding Vectors and Layers
[originally used on Monday March 28, 2016, altered September 15, 2016]
![Test image](https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Flag_of_Cuba.svg/2000px-Flag_of_Cuba.svg.png)
### This tutorial is designed so you can practice the skills you used in the [Programming Historian QGIS Tutorial about adding layers](http://programminghistorian.org/lessons/qgis-layers "Links to Programming Historian")

1.	Make a folder or directory called "Cuba" on your computer.

2.	Download the following Cuba data sets from DIVA-GIS [Google it] into that directory and unzip them; each should be in its own sub-directory.
    -	Administrative Areas CUB\_adm.ZIP
    -	Roads CUB\_rds.ZIP

3. 	Open QGIS and set up up a new project.

4.	Set up CRS (Coordinate Reference System) so that the project is using the NAD27/Cuba Norte Geographic Coordinate system. Go to "Project Properties" under the File menu. Make sure you are in the CRS tab, and then click "Enable on the fly CRS transformation." You can then search for NAD27/Cuba Norte and apply the change at the bottom of the panel.

![CRS selection](/Screenshots/CRS selection.png)

5.	Build a base map: Open these vectors, then change the way they look using the “properties”
    - CUB\_adm0.shp; change so there is no color fill. Click on fill style and select simple line
    - CUB\_adm1.shp; same as above
    - CUB\_roads.shp; change the color and width of the lines so they are easier to see

![No fill outline](/Screenshots/No fill outline.png)

6.	Look at the attribute table of CUB\_adm1.shp. These show the country’s 14 provinces. Note which one of the columns gives the name of the province. Write down the name of that column. Close the attribute table. Go into the “properties” for CUB\_adm1.shp into “labels”. Change it so that your map shows the names of the provinces in a large font.

7.	Go to Blackboard and from the Cuba tutorial area, download the file named Cuba, island, georif.zip. Unzip it and import the .tif file into QGIS as a raster file.

8.	Go back to CUB\_adm0.shp and CUB\_adm1.shp and change the width of the lines so they are visible.

9.	In the left-hand “layers” panel, drag the raster layer so you can see the parish lines over the historical map.

![Poorly georeferenced island](/Screenshots/Poorly geofrenced island.png)

10.	Go back to Blackboard and download the file named Port of Havana_modified.tif. Import that into QGIS. Drag the raster over your GIS map. You can also adjust the transparency on both of your historical maps in order to see the provincial boundaries.

11.	Save your work. Close QGIS

# Data Sources for this Tutorial
## Country GIS base map data
http://www.diva-gis.org/gdata

## Historical maps
The map "Cuba, Island" can be downloaded [here](http://jcb.lunaimaging.com/luna/servlet/detail/JCBMAPS~1~1~6264~115902445:Cuba-en-Iamaica,-soo-als-die-door-K?sort=normalized_date%2Cfile_name%2Csource_author%2Csource_title&qvq=q:cuba;sort:normalized_date%2Cfile_name%2Csource_author%2Csource_title;lc:JCBMAPS~1~1&mi=52&trs=126)

The map "Port of Havana" can be downloaded [here](http://jcb.lunaimaging.com/luna/servlet/detail/JCBMAPS~1~1~1089~101600001:Port-de-la-Havane-dans-l-Isle-de-Cu?sort=normalized_date%2Cfile_name%2Csource_author%2Csource_title&qvq=q:havana;sort:normalized_date%2Cfile_name%2Csource_author%2Csource_title;lc:JCBMAPS~1~1&mi=21&trs=32)
