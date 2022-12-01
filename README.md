Tutorial OSGEO4W - Cálculo de bandas raster - Índices de vegetação

1- Qgis instalado
2- acessar pasta raiz do Qgis;
3- Copiar a pasta "scripts" em C:\Program Files\QGIS 3.28.1\apps\Python39 para c:/ 
4- Colocar o ortomosaico.tif dentro da pasta c:/scripts
5- Acessar OSGEO4W Shell pelo administrador;
6- No prompt digitar cd c:/scripts +ENTER
7- Digitar: python c:\Scripts\gdal_calc.py -A ortomosaico.tif --A_band=1 -B ortomosaico.tif --B_band=2 -C ortomosaico.tif --C_band=3 --outfile=indice.tif --calc="formula" --NoDataValue=-999 + ENTER
8- O índice de vegetação estará disponível em c:/scripts com o nome de indice.tif
