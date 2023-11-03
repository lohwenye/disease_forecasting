# disease_forecasting
**High-dimensional superensemble disease forecasting**

**Overview**

This work proposes methods to combine a large number of point and probabilistic forecasts to provide quick and complete forward guidance of ED admissions respectively in a general manner. First, a large number of environmental and anthropogenic measurements were accounted for in simple models, using purely statistical and machine learning tools to generate forward point and probabilistic forecasts. Then, weighting schemes were developed to aggregate point and density forecasts, using constrained, high-dimensional regression which can account for a large number of point and probabilistic forecasts. These were then compared to simpler approaches to aggregate forecasts. A detailed analysis of the generalizability of our findings over multiple years, admission causes, and forecast horizons was provided. This work showed overall strong evidence that forecast combinations which appropriately accounted for a large number of forecasting submodels can consistently outperform baseline models, as well as individual submodels, for a large number of ED admission causes.


**Study setting and data**

Utilized data on emergency department admissions across 16 disease categories, temperature (maximum, mean, and minimum), relative and absolute humidity, particulate matter indicator (PMI) PM2.5 and PM10, pollutants O3, NO2, SO2, and CO, and total precipitation. Emergency department admissions data seems to vary with no clear pattern. 
Meteorological variables were also relatively constant with an average value of 304.865K (Fig 1B, Range: 300.979K — 307.458K), 300.982K (Fig 1C, Range: 298.095K — 303.210K), and 298.116K (Fig 1D, Range: 296.107K — 300.773K) for maximum, mean, and minimum temperature; 79.464% (Fig 1E, Range: 63.546% — 91.475%) and 21.330g/m3 (Fig 1F, Range: 17.315g/m3 — 23.463g/m3) for relative and absolute humidity; 24.299μg/m3 (Fig 1I, Range: 10.036μg/m3 — 59.566μg/m3), 23.863μg/m3 (Fig 1J, Range: 10.342μg/m3 — 44.317μg/m3), 10.780μg/m3 (Fig 1K, Range: 2.160μg/m3 — 30.328μg/m3), 0.537μg/m3 (Fig 1L, Range: 0.296μg/m3 — 2.152μg/m3) for pollutants O3, NO2, SO2, and CO; and 0.005m (Fig 1M, Range: 0.000m — 0.035m) for total precipitation respectively. 
Only PM2.5 and PM10 exhibit significant peaks due to seasonal haze pollution with average values of 18.367μg/m3 (Fig 1G, Range: 9.164μg/m3 — 167.028μg/m3) and 29.965μg/m3 (Fig 1H, Range: 16.664μg/m3 — 213.948μg/m3) for PM2.5 and PM10 respectively.  

**Models**

Naive
Linear Regression
Ridge Regression
LASSO
Elastic Net
Random Forest
Gradient Boost
k-Nearest Neighbours
Mean
Median
Weighted-Mean with Expanding Window
Weighted-Mean with Rolling Window
Second-Order Linear Regression
Second-Order Ridge
Second-Order LASSO
Second-Order Elastic Net
Second-Order Random Forest
Second-Order Gradient Boost
Second-Order k-Nearest Neighbours

**Error Metrics**

For point forecasts, primarily assessed errors here using mean-absolute error (MAE), mean-absolute percentage error (MAPE) and mean absolute scaled error (MASE), which respectively illustrates the raw deviation, the percentage deviation of point forecasts to future observations and the relative deviation of point forecasts to naive forecast errors. Additionally, also employed mean-squared error (MSE) to identify presence of large outlier errors and symmetric mean-absolute percentage error (SMAPE) to reduce the effect of small- or zero-value actual observations in the denominator respectively.
