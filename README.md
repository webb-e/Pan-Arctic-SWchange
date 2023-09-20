# Pan-Arctic-SWchange
Code used to analyze pan-Arctic surface water trends 

This is the companion code to:
Webb, E.E., Liljedahl, A.K., Cordeiro, J.A. et al. Permafrost thaw drives surface water decline across lake-rich regions of the Arctic. Nat. Clim. Chang. 12, 841–846 (2022). https://doi.org/10.1038/s41558-022-01455-w

Yearly July surface water datasets and the trend in July surface water is available here https://arcticdata.io/catalog/view/doi%3A10.18739%2FA2NK3665N

Most of the files here are written in Java Script to be executed in the Google Earth Engine web interface. They calculate the trend in climate variables over time or the trend in surface water (as measured by the Superfine Water Index; SWI) over time. Here, trend is defined as the Sen's slope of the variable regressed against year (2000-2021). Climate variables are calculated over the entire pan-Arctic (land north of 50N) and the surface water index is calculated only in the study region of the Webb et al., paper (see code or the paper for details on the study region). The climate variables are taken from the ERA5-land-hourly dataset and the SWI is calculated from MODIS NBAR reflectance data.

The file called SW_archived.ipnyb is the code used to run the machine learning analysis that identified the drivers of surface water change. The pixel-wise 12km data (surface water trends, climate trends, landscape variables, etc.) used in analysis is too large to be stored on github but is available upon request from the author.

#################################################

SWI citation: Sharma, R. C., Tateishi, R., Hara, K. & Nguyen, L. V. Developing Superfine Water Index (SWI) for global water cover mapping using MODIS data. Remote Sensing 7, 13807–13841 (2015).

ERA-5 Land hourly citation: Muñoz Sabater, J. ERA5-Land hourly data from 1981 to present. (2019) doi:doi:10.24381/cds.e2161bac

MODIS NBAR citation: Schaaf, C., Z. W. MCD43A4 MODIS/Terra+Aqua BRDF/Albedo Nadir BRDF Adjusted Ref Daily L3 Global - 500m V006. (2015) doi:https://doi.org/10.5067/MODIS/MCD43A4.006
