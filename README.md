IFV: 

python c:\Scripts\gdal_calc.py -A ortomosaico.tif --A_band=1 -B ortomosaico.tif --B_band=2 -C ortomosaico.tif --C_band=3 --outfile=resultvifvfina5.tif --calc="(2*B)-A-C/(2*B)+A-C" --NoDataValue=-999

VARI:
python c:\Scripts\gdal_calc.py -A ortomosaico.tif --A_band=1 -B ortomosaico.tif --B_band=2 -C ortomosaico.tif --C_band=3 --outfile=resultvarifina5.tif --calc=" B-A / B+A -C" --NoDataValue=-999
