# Rivercane Project [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14496874.svg)](https://doi.org/10.5281/zenodo.14496874)
### This project for [the Earth Analytics Data Science Bootcamp-Geog 4463/5463-course](https://earthlab.colorado.edu/earth-data-analytics-professional-graduate-certificate?utm_source=earthdatascience&utm_medium=website&utm_campaign=certificate-2022&utm_id=certificate-2022) from Univ. of Colorado Boulder is a work in progress.
<img src="/pics/rivercane_image.jpg" alt="Rivercane along creek in Great Smoky Mountains National Park" width="50%"/> 
Native Rivercane - <i>Arundinaria gigantea</i> - is native to 22 states in the US and has been reduced to 2% of it's original range (Sharma, 2003). 

## This project will explore habitats that might be suitable for restoration efforts in the future based upon two different climate predictions. It is intended for conservationist and others who would like to start a restoration project. Once this project is completed, anyone should be able to edit the code with a county of their choice and get information on elevation, soil composition and precipitation which will help locate appropriate areas with the best habitat for Rivercane.

### Habitat suitability will be compared between two counties in the United States; specifically, Cherokee County, Oklahoma and Jackson County, North Carolina. These areas were chosen because they are inhabited by Cherokee people who use native Rivercane for a variety of cultural purposes. For each location, soil data and elevation will be analyzed and two climate models will be used to look at different predictions for precipitation at the end of the century (2096-2099). The two models chosen were:
1. The Model for Interdisciplinary Research on Climate version 5, which was developed by the Center for Climate System Research (CCSR) at the University of Tokyo, Japan. 
2. The Geophysical Fluid Dynamics Laboratory (GFDL) Earth System Model GFDL-ESM2M (GFDL-ESM2M)  developed by  of the National Oceanic and Atmospheric Administration (NOAA).

### At this point - December 2024 - I have been able to download most of the data and crop it to fit Cherokee County Oklahoma and Jackson County North Carolina. It is my intention to complete the modeling at a later date. In these notebooks, I provide an outline of what those next steps will be to provide a tool for others to use. What I can show to date is a difference in elevation between the two locations. Rivercane grows best in locations below 2,000 ft or 609.6 m.
## Figure 1: In Cherokee County OK, there are no areas which do not meet the elevation requirements of rivercane.
<img src="/pics/ok_elevation.png" alt="color plot of elevation within Cherokee County OK" width="50%"/>

## Figure 2: In Jackson County NC, there are many areas which exceed the elevation requirements of rivercane and are therefore not suitable for restoration
<img src="/pics/nc_elevation.png" alt="color plot of elevation within Cherokee County OK" width="50%"/>

## Sources
* Sharma, Sanjeev. 2023, "PROPAGATION, PHYSIOLOGY, AND BIOMASS OF GIANT CANE (ARUNDINARIA
GIGANTEA) FOR CONSERVATION AND RESTORATION", A Master’s Thesis Presented to The Graduate College of Missouri State University. [accessed online] (https://bearworks.missouristate.edu/cgi/viewcontent.cgi?article=4887&context=theses)
* US Census, 2024 "TIGER/Line Shapefiles" accessed online: https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html
* POLARIS: A 30-meter probabilistic soil series map of the contiguous United States
By: Nathaniel W. Chaney, Eric F Wood, Alexander B McBratney, Jonathan W Hempel, Travis W. Nauman, Colby W. Brungard, and Nathan P Odgers
https://doi.org/10.1016/j.geoderma.2016.03.025
* earthaccess python library available online at: https://earthaccess.readthedocs.io/en/latest/
* The Climate Model Intercomparison Project, available online at: http://thredds.northwestknowledge.net:8080/thredds/reacch_climate_CMIP5_macav2_catalog2.html

## Software Installation 
* Python is the programming language
* Bash is used to conda install <package_name>
* Packages include: Earthaccess, GeoPandas, Glob, Math, Mathplotlib, Pandas, Rasterio, Requests, Rioxarray, Xarray, Xrspatial, Zipfile

## Other Considerations
Input Data:
* County level shapefiles are extracted from the U.S. Census website: "https://www2.census.gov/geo/tiger/TIGER2023/COUNTY/tl_2023_us_county.zip"
* Soil data is extracted from the Polaris website: "http://hydrology.cee.duke.edu/POLARIS/PROPERTIES/v1.0/"
* The Earthaccess website is used for elevation data. See this guide for setting up an account and using this resource: "https://earthaccess.readthedocs.io/en/latest/"

Output Data:
* Shapefiles which contain geospatial vector information for U.S. Counties
* Data arrays for soil composition, pH and elevation

Contributing Guidelines: 
* Create a new branch for your contribution
* Be respectful and constructive in all communication
* When creating an issue, provide a clear and concise description which includes: a brief and descriptive title, detailed steps to reproduce the issue, what should happen vs what actually happens and any relevant log or screenshot.

Disclosure: Google Gemini was used in a variety of ways to learn and enhance this project.
