# GISTEMP

Goddard Institute for Space Studies Surface Temperature Analysis ver. 4 (GISTEMP v4)

This repository was created to store and share the Goddard Institute for Space Studies Surface Temperature Analysis (GISTEMP) as a project for LIS 4220: Data Curation at the University of Denver 2021.

GISTEMP v4 is a dataset examining the changing temperature trends on Earth produced through analysis of the National Oceanic and Atmospheric Administration’s (NOAA’s) 4th version of the Global Historical Climatology Network (GHCN v4) and fifth version of Extended Reconstructed Sea Surface Temperature (ERSST v5) datasets for land temperature and ocean temperature respectively. The GISTEMP data reflect temperature anomalies. In the case of this data, temperature anomaly refers to the deviation, in degrees Celsius, from the average temperature measured over the 30 year span from 1951 to 1980. The temporal coverage of this data is constrained by the availability of accurate temperature measurement, 1880-present. Measurements from 1960-present are the most accurate with an uncertainty of +/- 0.05 degrees Celsius, though that uncertainty increases to +/- 0.1 degrees Celsius for seasonal means and +/- 0.17 degrees Celsius for monthly means.

GISTEMP was first initiated in 1979 by Dr. James E. Hansen as he grew concerned about the potential for a rise in temperature due to anthropogenic greenhouse gasses. The basic methodology was to group station data into 80 equal area boxes and assesses the deviance from mean for that area. The current iteration groups these data into 8000 equal area boxes. The GISTEMP project has changed over time as more and better data has become available, but the project remains true to the initial goal of assessing global temperature rise. The project is currently led by Dr. Gavin Schmidt. For more information about the project, visit https://data.giss.nasa.gov/gistemp/ 

To cite this dataset please be sure to update the date accessed and include the most recent scholarly publication from the GISTEMP team:

GISTEMP Team, 2021: GISS Surface Temperature Analysis (GISTEMP), version 4. NASA Goddard Institute for Space Studies. Dataset accessed YYYY-MM-DD at https://data.giss.nasa.gov/gistemp/.
Lenssen, N., G. Schmidt, J. Hansen, M. Menne, A. Persin, R. Ruedy, and D. Zyss. 2019. Improvements in the GISTEMP uncertainty model. J. Geophys. Res. Atmos., 124, no. 12, 6307-6326, doi:10.1029/2018JD029522.


Data are presented in table formats and the source code for the project is also available as a Python program.

Files in this repository:

•	GLB.Ts+dSST
  *	This CSV file contains average annual, monthly, and seasonal temperature anomalies for the entire Earth in degrees Celsius. For monthly mean temperature, the fields are  presented as 3 letter month codes, e.g. Jan for January, Feb for February, etc. The annual means are presented as January to December, J-D, and December to November, D-N. Lastly the seasonal mean temperatures are listed under DJF (December, January, and February) for winter, MAM (March, April, and May) for spring, JJA (June, July, and August) for summer, and SON (September, October, and November) for autumn. 

•	NH.Ts+dSST
  *	This CSV file contains the average annual, monthly, and seasonal temperature anomalies for the entire Northern Hemisphere in degrees Celsius. For monthly mean temperature, the fields presented as 3 letter month codes, e.g. Jan for January, Feb for February, etc. The annual means are presented as January to December, J-D, and December to November, D-N. Lastly the seasonal mean temperatures are listed under DJF (December, January, and February) for winter, MAM (March, April, and May) for spring, JJA (June, July, and August) for summer, and SON (September, October, and November) for autumn. 
 
•	SH.Ts+dSST
  *	This CSV file contains the average annual, monthly, and seasonal temperature anomalies for the entire Southern Hemisphere in degrees Celsius. For monthly mean temperature, the fields are presented as 3 letter month codes, e.g. Jan for January, Feb for February, etc. The annual means are presented as January to December, J-D, and December to November, D-N. Lastly the seasonal mean temperatures are listed under DJF (December, January, and February) for winter, MAM (March, April, and May) for spring, JJA (June, July, and August) for summer, and SON (September, October, and November) for autumn. 
  
•	ZonAnn.Ts+dSST
  *	This CSV file contains the average annual temperature anomalies for latitudinal zones in degrees Celsius. In addition to global (Glob) and hemispherical (NHem & Shem) zones, the zones are listed as ranges in degrees of latitude, e.g. 24N-90N represents the region between the 24th parallel North and the North Pole. 
  
•	GISTEMP4.0.tar
 *	This is the source code for GISTEMP. This python program adapted from the Fortran original requires the GHCN v4 and ERSST v5 datasets from NOAA’s National Centers for Environmental Information (NCEI) to calculate temperature anomalies on Earth as subdivided into 8000 equal-area cells. This produces far more granular data than the tables and can be more readily be applied to maps. This program is designed to run on a Unix-like system. 


