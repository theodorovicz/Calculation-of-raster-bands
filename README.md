## Calculation of raster bands - Vegetation indices ##

Qgis installed;

Access Qgis root folder;

Copy the "scripts" folder in C:Program FilesQGIS 3.28.1appsPython39 to c:/;

Place the orthomosaic.tif inside the c:/scripts folder;

Access OSGEO4W Shell by the administrator;

In prompt type cd c:/scripts +ENTER;
```
python c:\Scripts\gdal_calc.py -A ortomosaico.tif --A_band=1 -B ortomosaico.tif --B_band=2 -C ortomosaico.tif --C_band=3 --outfile=indice.tif 
--calc="formula" --NoDataValue=-999 + ENTER
```
The vegetation index will be available in c:/scripts with the name of index.tif.
