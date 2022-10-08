###### Landsat. Sentinel. Flood & indices

# **Building indices and flood areas** <img src="https://w7.pngwing.com/pngs/281/213/png-transparent-satellite-logo-communications-satellite-logo-ground-station-satellite-radio-angle-text-computer-icons.png" width="20"><br> **based on Landsat-8/9, and Sentinel-2 imagery**

##  <p align="justify"> [NDVI](https://en.wikipedia.org/wiki/Normalized_difference_vegetation_index),  [NDWI](https://en.wikipedia.org/wiki/Normalized_difference_water_index), [SAVI](https://en.wikipedia.org/wiki/Soil-adjusted_vegetation_index), [VARI](https://pro.arcgis.com/en/pro-app/latest/arcpy/spatial-analyst/vari.htm), [MNDWI](https://www.space4water.org/taxonomy/term/1246), [NDMI](https://pro.arcgis.com/en/pro-app/latest/arcpy/spatial-analyst/ndmi.htm), [Clay Minerals](https://www.space4water.org/taxonomy/term/1250), [Ferrous Minerals](https://pro.arcgis.com/en/pro-app/2.6/arcpy/image-analyst/ferrousminerals.htm)</p> 
 
### Introduction

<p align="justify">There is a large number of spectral indices that can analyze various aspects such as vegetation, water resources, snow, soil, fire, among others. The satellites better known as Landsat and Sentinel offer the opportunity to perform various operations with their bands, the result can be converted into a spectral index.

The two main sensors for Landsat 8/9 are the <i>Operational Land Imager (OLI)</i> and <i>Thermal Infrared Sensor (TIRS)</i>. The Operational Land Imager (OLI) produces 9 spectral bands (Band 1 to 9) at 15, 30, and 60 m spatial resolution. Then, the Thermal Infrared Sensor (TIRS) consists of 2 thermal bands with a spatial resolution of 100 m.

Sentinel-2 carries an optical instrument payload that samples 13 spectral bands: four bands at 10 m, six bands at 20 m and three bands at 60 m spatial resolution.</p> 


### Normalized Difference Vegetation Index (NDVI)
<p align="justify">The normalized difference vegetation index (NDVI) is a simple graphical indicator that can be used to analyze remote sensing measurements, often from a space platform, assessing whether or not the target being observed contains live green vegetation.

> <i> NDVI = (NIR – Red) / (NIR + Red)</i></p> 

### Normalized Difference Water Index (NDWI). Formula 1
<p align="justify">Normalized Difference Water Index (NDWI) may refer to one of at least two remote sensing-derived indexes related to liquid water.
One is used to monitor changes in water content of leaves, using near-infrared (NIR) and short-wave infrared (SWIR) wavelengths:

> <i>NDWI = (NIR – SWIR) / (NIR + SWIR), proposed by Gao in 1996 </i></p> 

### Normalized Difference Water Index (NDWI). Formula 2
<p align="justify"> Another is used to monitor changes related to water content in water bodies, using green and NIR wavelengths:

> <i>NDWI = (Green – NIR) / (Green + NIR), defined by McFeeters in 1996 </i></p> 

### Soil-Adjusted Vegetation Index (SAVI)
<p align="justify"> Landsat Soil Adjusted Vegetation Index (SAVI) is used to correct Normalized Difference Vegetation Index (NDVI) for the influence of soil brightness in areas where vegetative cover is low.

> <i>SAVI = ((NIR - Red) / (NIR + Red + L)) x (1 + L)</i>

* NIR = pixel values from the near infrared band
* Red = pixel values from the near red band
* L = amount of green vegetation cover.</p>

### Visible Atmospherically Resistant Index (VARI)
<p align="justify"> The Visible Atmospherically Resistant Index (VARI) is designed to emphasize vegetation in the visible portion of the spectrum while mitigating illumination differences and atmospheric effects. It is ideal for RGB or color images; it utilizes all three color bands.

> <i>VARI = (Green - Red)/ (Green + Red - Blue)</i></p>

### Modified Normalized Difference Water Index (MNDWI)
<p align="justify"> The Modified Normalized Difference Water Index (MNDWI) uses green and SWIR bands for the enhancement of open water features. It also diminishes built-up area features that are often correlated with open water in other indices.

> <i> MNDWI = (Green - SWIR) / (Green + SWIR)</i></p>

###  Normalized Difference Moisture Index (NDMI)
<p align="justify">  The Normalized Difference Moisture Index (NDMI) is sensitive to the moisture levels in vegetation. It is used to monitor droughts as well as monitor fuel levels in fire-prone areas. It uses NIR and SWIR bands to create a ratio designed to mitigate illumination and atmospheric effects.

> <i> NDMI = (NIR - SWIR1)/(NIR + SWIR1)</i></p>

### Clay Minerals
<p align="justify"> The clay ratio is a ratio of the SWIR1 and SWIR2 bands. This ratio leverages the fact that hydrous minerals such as clays, alunite absorb radiation in the 2.0–2.3 micron portion of the spectrum. This index mitigates illumination changes due to terrain since it is a ratio.

> <i>Clay Minerals Ratio = SWIR1 / SWIR2</i></p>

###  Ferrous Minerals
<p align="justify"> The ferrous minerals ratio highlights iron-bearing materials.

> <i>Ferrous Minerals Ratio = SWIR / NIR</i></p>

### Repository content
```shell
│   Landsat 8-9. Image Analysis. USA.ipynb
│   Landsat 8. Flood monitoring. Madagascar.ipynb
│   Landsat 8_9 imagery analysis and building indices. NY (the USA).ipynb
│   Sentinel 2 imagery analysis and building indices. Russia. RGB+NIR.ipynb
│   Sentinel 2 imagery analysis. Russia. All bands.ipynb
│   Sentinel 2. Image Analysis. Sundarbans.ipynb
│
└───files
        landsat8_9.jpg
        Sentinel-2.png
```
