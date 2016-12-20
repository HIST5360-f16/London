#London Maps Tutorial

##Georeferencing Based on Thames Hydrology
Additions by: Justin Jolly

###Introduction
In this tutorial, you will learn how to georeference old maps of London. You will use the Thames River as your chief reference point. The Thames River is the city's oldest landmark.
![18th Century Depiction of the River Thames](http://www.gac.culture.gov.uk/images%5Clarger%5C10862.jpg)

###Getting Started
1. Make a new folder called "London Maps." You will save all files related to this project in this folder.
2. Open QGIS and begin a new project.
3. Download Irfanview from [Irfanview](http://www.irfanview.com/)
4. Go to the [London Datastore](http://data.london.gov.uk/dataset/statistical-gis-boundary-files-london) and download the file marked "statistical-GIS-boundaries-London" to your "London Maps" folder.

![London Data](/LondonDataPic.png)

###Find and Convert London Maps
5. Google "Historical Maps of London" and select two maps that have a distinct representation of the Thames. Its unmistakable.
6. Right click on either map and save them to your folder as JPGs or PNGs, then open them in your Irfanviewer to convert them into TIF files by using the _batchconvert_ option.

![Irfan](/IrfanConvertPic.png)

###Adding Vector Layers
7. Go to your "London Maps" folder and unzip all the zipped files. Make sure the contents save to your "London Maps" folder.
8. Open the file marked "London_Ward_Citymerged.shp" (the shapefile) as a vector layer in QGIS.
9. Set the project CRS to match the London_Ward_Citymerged layer by right clicking on the layer and click "Set Project CRS from layer".
![London CRS](http://i1092.photobucket.com/albums/i405/finbar01/London%20CRS_zpsd5fap1nm.png)
10. Set the color on this file to one that contrasts easily with blue.
11. Open the file marked "LSOA_2011_London_gen_MHW.shp" (again, a shapefile) as a vector layer.
12. Set the color on this file to blue.
13. Now you can clearly see the outline of the Thames.
![Vector Layers](http://i1092.photobucket.com/albums/i405/finbar01/London%20vector%20layers_zpsfrevsmh1.png) 
14. Using the Blue outline of the Thames to provide reference points, you are going to georeference two old maps.
15. Go to the "Raster" option at the top toolbar of QGIS. Select the georeferencer, and then choose the add vector to select one of your TIF file maps.

![Georeferencer](/QGISLondonGeoRef.png)

###Georeferencing Old Maps
16. Click on an identifiable point on the old map, a small window will pop up from which you should select the "from map canvas" option, and then select the corresponding point on your QGIS map. Make sure to select points on both riverbanks. Also be sure to follow these couple of steps precisely because it is easy to lose track of one of your map windows, freezing it behind the "from map canvas" window.
17. Repeat this step three more times, with three new points.
18. Hit the green arrow buttton. A window will appear with some project specs. Make sure the CSR matches the one you set at the beginning of the project, then click "ok" on the prompt.
19. You should now see the map superimposed over your QGIS map. Select an appropriate level of transparency for the old map layer.
20. Repeat steps 14-18 for your other map.
![Georefrenced](http://i1092.photobucket.com/albums/i405/finbar01/London%20Georefrenced_zpse2kvwa2v.png)
###Congratulations!!! You have now georeferenced two maps of London based on the hydrology of the Thames River. Make sure you save your work and close QGIS.
![Fireworks] (https://richmondhillchiropractic.files.wordpress.com/2013/04/celebrating-12000-visits.jpg "Fireworks")