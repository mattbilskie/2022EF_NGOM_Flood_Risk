[![DOI](https://zenodo.org/badge/450105833.svg)](https://zenodo.org/badge/latestdoi/450105833)

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg


When using this dataset, please cite the following:
1. M.V. Bilskie, D. Del Angel, D. Yoskowitz, S.C. Hagen (2022), Future Flood Risk Exacerbated by the Dynamic Impacts of Sea Level Rise Along the Northern Gulf of Mexico, **Earth's Future**, Revised & Resubmit.
2. DOI for this data.


# Metadata
## GIS
### Building_damage_output.gdb

This geodatabase contains building damage loss for residential buildings, displaced people, and people requiring shelter at the census block level under a present day sea level and a low (0.2 m), intermediate-low (0.5 m), intermediate-high (1.2 m), and high (2.0 m) rise in sea level (baseline year of 1992) [[1]](#1).

The filenames are organized as follows:

Building damage - Region_ReturnPeriod_SLRScenario_BldDamLoss_RES

Region 1 = Wakulla, Frankling, and Gulf Counties, FL

Region 2FL = Bay, Walton, Okaloosa, Santa Rosa, and Escambia Counties, FL

Region 2AL = Baldwin and Mobile Counites, AL

Region 3 = Jackson, Harrison, and Hancock Counties, MS

Displaced people at the census block level - Displaced_People_ReturnPeriod_SLRScenario

Displaced people at at the county level - Region_Displaced_ReturnPeriod

Displaced People requring shelter at the census block level - Displaced_Shelter_People_ReturnPeriod_SLRScenario

Return Period

100 yr (1% annual exceedance probability)

500 yr (0.2% annual exceedance probability)

SLR Scenario

P = Present

L = Low (0.2 m)

IL = Intermediate-Low (0.5 m)

IH = Intermediate-High (1.2 m)

H = High (2.0 m)

### GIS_layers.gdb

NGOM_Counties - county layer

ms_al_fl_coastal_cb - census blocks for the study region.

## RDS

This directory contains R data files. These files are based on the GIS layers described above.

Displaced_People_ReturnPeriod.rds - Number of displaced individuals at the census block level for each SLR scenario for a given return period.

Displaced_Shelter_People_ReturnPeriod.rds - Number of displaced individuals requring shelter at the census block level for each SLR scenario for a given return period.

Region_res_ReturnPeriod_county - Number of buildings substantially damaged (> 50% damage) for each county in the region for each SLR scenario. The dataset also contains the number of buildings damaged in bins of 10%.

## References
<a id="1">[1]</a> 
AP Parris et al. (2012). 
Global Sea Level Rise Scenarios for the United States National Climate Assessment
NOAA technical report OAR CPO ; 1;
https://repository.library.noaa.gov/view/noaa/11124
