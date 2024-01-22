![Logo](https://github.com/bycnfz/weather2k/blob/main/logo.png)

# Weather2K: A Multivariate Spatio-Temporal Benchmark Dataset for Meteorological Forecasting Based on Real-Time Observation Data from Ground Weather Stations

【Accepted】by **the 26th International Conference on Artificial Intelligence and Statistics (AISTATS) 2023**

https://aistats.org/aistats2023/accepted.html

This repository provides the dataset used in the paper. We hope that the release of Weather2K can provide a foundation for accelerated research in this area and foster collaboration between atmospheric and data scientists.



## Download the dataset

Google Drive : https://drive.google.com/drive/folders/1rTabWIuAarDfSkUROK2rzEYJEqP338UM?usp=share_link

If you have any quesetions about the data download, please contact wuming@bupt.edu.cn

The data is hosted in the upper links with the following directory structure :

```
.
|-- Weather2K-R
|   `-- data.npy
|-- Weather2K-S
|   |-- 79.csv
|   |-- 114.csv
|   |-- 209.csv
|   |-- 259.csv
|   |-- 532.csv
|   |-- 546.csv
|   |-- 850.csv
|   |-- 852.csv
|   |-- 947.csv
|   |-- 1201.csv
|   |-- 1272.csv
|   |-- 1328.csv
|   |-- 1527.csv
|   |-- 1691.csv
|   `-- 1796.csv
`-- idx2stat.txt
```

The shape of the numpy file of Weather2K-R is (1866, 23, 40896), which means 1,866 groud weather stations,  3 constants for position information and 20 meteorological factors, and 40,896 time steps. 

Weather2K-S contains 15 representative and geographically diverse ground weather stations distributed throughout China. They are csv files named after the index used in the numpy file.

idx2stat.txt shows the correspondence bewteen the numpy index and the original station number.



## Definitions of the variables in the dataset

|  Numpy Index   | **Long Name**                             | **Short Name**         | **Unit** |
| :------------: | :---------------------------------------- | :--------------------- | :------: |
|       0        | Latitude                                  | lat                    |   (°)    |
|       1        | Longitude                                 | lon                    |   (°)    |
|       2        | Altitude                                  | alt                    |   (m)    |
|       3        | Air pressure                              | ap                     |   hpa    |
|       4        | Air Temperature                           | t                      |   (°C)   |
|      5/6       | Maximum / Minimum temperature             | mxt / mnt              |   (°C)   |
|       7        | Dewpoint temperature                      | dt                     |   (°C)   |
|       8        | Relative humidity                         | rh                     |   (%)    |
|       9        | Water vapor pressure                      | wvp                    |   hpa    |
| 10/11/12/13/14 | Precipitation in 1h / 3h / 6h / 12h / 24h | p1 / p2 / p3 / p4 / p5 |   (mm)   |
|       15       | Wind direction                            | wd                     |   (°)    |
|       16       | Wind speed                                | ws                     | (ms<sup>-1</sup>) |
|       17       | Maximum wind direction                    | mwd                    |   (°)    |
|       18       | Maximum wind speed                        | mws                    | (ms<sup>-1</sup>) |
|       19       | Land surface temperature                  | st                     |   (°C)   |
|     20/21      | Horizontal visibility in 1 min / 10 min   | hv1 / hv2              |   (m)    |
|       22       | Vertical visibility                       | vv                     |   (m)    |


## Cite

If you are using this dataset please cite 
> Zhu X, Xiong Y, Wu M, et al. Weather2K: A Multivariate Spatio-Temporal Benchmark Dataset for Meteorological Forecasting Based on Real-Time Observation Data from Ground Weather Stations[C]//International Conference on Artificial Intelligence and Statistics. PMLR, 2023: 2704-2722.
