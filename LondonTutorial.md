#London Maps Tutorial

##Georeferencing Based on Thames Hydrology
Additions by: Justin Jolly

In this tutorial, you will learn how to georeference old maps of London to the Thames River, its oldest landmark.
![18th Century Depiction of the River Thames](http://www.gac.culture.gov.uk/images%5Clarger%5C10862.jpg)
1. Make a new folder entitled "London Maps."
2. Open QGIS and begin a new project.
3. Download Irfanview from [Irfanview](http://www.irfanview.com/)
4. Go to the [London Datastore](http://data.london.gov.uk/dataset/statistical-gis-boundary-files-london) and download the file marked "statistical-GIS-boundaries-London" to your "London Maps" folder.

![London Data](/LondonDataPic.png)

5. Google "Historical Maps of London" and select two that have a distinct representation of the Thames. Its unmistakable.
6. Right click on either map and save them as pictures, then use your Irfanviewer to convert them into TIF files by using the _batchconvert_ option.

![Irfan](/IrfanConvertPic.png)

7. Go to your "London Maps" folder and extract all the zipped files.
8. Open the file marked "London_Ward_Citymerged.shp" (the shapefile) as a vector layer in QGIS.
9. Set the project CRS to match the London_Ward_Citymerged layer by right clicking on the layer and click "Set Project CRS from layer".
![London CRS](http://i1092.photobucket.com/albums/i405/finbar01/London%20CRS_zpsd5fap1nm.png)
9. Set the color on this file to one that contrast easily with blue.
10. Open the file marked "LSOA_2011_London_gen_MHW.shp" (again, a shapefile) as a vector layer.
11. Set the color on this file to blue.
12. Now you can clearly see the hydrology of the Thames.
![Vector Layers](http://i1092.photobucket.com/albums/i405/finbar01/London%20vector%20layers_zpsfrevsmh1.png) 
13. Using the Blue outline of the Thames to provide reference points, you are going to georeference two old maps.
14. Go to the "Raster" option at the top toolbar of QGIS. Select the georeferencer, and then choose the add vector button to select one of your TIF file maps.

![Georeferencer](/QGISLondonGeoRef.png)

15. Click on a discernable point on the old map, select the "from map canvas" option, and then select the corresponding point on your QGIS map. Make sure to select points on both riverbanks.
16. Repeat this step three more times, with three new points.
17. Hit the green arrow buttton. The coordinates are not necessary to add (they were in the shapefile), so just click "ok" on the prompt.
18. You should now see the map superimposed over your QGIS map. Select an appropriate level of transparency for the old map layer.
19. Repeat steps 14-18 for your other map.
![Georefrenced](http://i1092.photobucket.com/albums/i405/finbar01/London%20Georefrenced_zpse2kvwa2v.png)
20. Congratulations, you have georeferenced two maps of London based on the hydrology of the Thames. Save your work and close QGIS.
