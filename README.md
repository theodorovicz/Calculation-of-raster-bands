Calculation of raster bands - Vegetation indices

1- Qgis installed;

2- Access Qgis root folder;

3- Copy the "scripts" folder in C:Program FilesQGIS 3.28.1appsPython39 to c:/;

4- Place the orthomosaic.tif inside the c:/scripts folder;

5- Access OSGEO4W Shell by the administrator;

6- In prompt type cd c:/scripts +ENTER;

7- python c:\Scripts\gdal_calc.py -A ortomosaico.tif --A_band=1 -B ortomosaico.tif --B_band=2 -C ortomosaico.tif --C_band=3 --outfile=indice.tif 
--calc="formula" --NoDataValue=-999 + ENTER

8 -The vegetation index will be available in c:/scripts with the name of index.tif.
