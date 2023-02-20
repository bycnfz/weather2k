![Logo](https://github.com/ai4environment/WeatherBench/blob/master/figures/logo_text_left.png?raw=true)

![](C:\Users\Xiong\Desktop\weather2k.png)

# **Weather2K: A Multivariate Spatio-Temporal Benchmark Dataset for Meteorological Forecasting Based on Real-Time Observation Data from Ground Weather Stations**

If you are using this dataset please cite 
> Stephan Rasp, Peter D. Dueben, Sebastian Scher, Jonathan A. Weyn, Soukayna Mouatadid, and Nils Thuerey, 2020.
> WeatherBench: A benchmark dataset for data-driven weather forecasting.
> arXiv: [https://arxiv.org/abs/2002.00469](https://arxiv.org/abs/2002.00469)

This repository contains all the code for downloding and processing the data as well as code for the baseline models
 in the paper.

描述了数据的下载和说明

---
 balabala....

---

If you have any questions about this dataset, please use the [Github Issue](https://github.com/pangeo-data/WeatherBench/issues) feature on this page! 



## Download the data
The data is hosted below with the following directory structure:

百度云：链接: https://pan.baidu.com/s/1rAOjB20I2kwqtsfDF5j2JQ 提取码: 5uf1

Google Drive：https://drive.google.com/drive/folders/1rTabWIuAarDfSkUROK2rzEYJEqP338UM?usp=share_link

```
.
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
|    -- 1796.csv
|-- Weather2K-R
|   `-- data.npy
|-- idx2stat.txt

```

描述--



## Definitions and physical descriptions of the variables in the Weather2K dataset



| Index          | **Long Name**                             | **Short Name**         | **Unit** | **Physical Description**                                     |
| -------------- | ----------------------------------------- | ---------------------- | -------- | ------------------------------------------------------------ |
| 0              | Latitude                                  | lat                    | (°)      | The latitude of the ground observation station               |
| 1              | Longitude                                 | lon                    | (°)      | The longitude of the ground observation station              |
| 2              | Altitude                                  | alt                    | (m)      | The altitude of the air pressure sensor                      |
| 3              | Air pressure                              | ap                     | hpa      | Instantaneous atmospheric pressure at 2 meters above the ground |
| 4              | Air Temperature                           | t                      | (°C)     | Instantaneous temperature of the air at 2.5 meters above the ground where sheltered from direct solar radiation |
| 5/6            | Maximum / Minimum temperature             | mxt / mnt              | (°C)     | Maximum / Minimum air temperature in the last one hour       |
| 7              | Dewpoint temperature                      | dt                     | (°C)     | Instantaneous temperature at which the water vapor saturates and begins to condense |
| 8              | Relative humidity                         | rh                     | (%)      | Instantaneous humidity relative to saturation at 2.5 meters above the ground |
| 9              | Water vapor pressure                      | wvp                    | hpa      | Instantaneous partial pressure of water vapor in the air     |
| 10/11/12/13/14 | Precipitation in 1h / 3h / 6h / 12h / 24h | p1 / p2 / p3 / p4 / p5 | (mm)     | Cumulative precipitation in the last 1 / 3 / 6 / 12 / 24 hour(s) |
| 15             | Wind direction                            | wd                     | (°)      | The direction of the wind speed. (Wind direction is 0 if wind speed is less than or equal to 0.2) |
| 16             | Wind speed                                | ws                     | (ms*−*1) | The average speed of the wind at 10 meters above the ground in a 10-minute period |
| 17             | Maximum wind direction                    | mwd                    | (°)      | Maximum wind speed’s direction in the last one hour          |
| 18             | Maximum wind speed                        | mws                    | (ms*−*1) | Maximum wind speed in the last one hour                      |
| 19             | Land surface temperature                  | st                     | (°C)     | Instantaneous temperature of bare soil at the ground surface |
| 20/21          | Horizontal visibility in 1 min / 10 min   | hv1 / hv2              | (m)      | 1 / 10 minute(s) mean horizontal visibility at 2.8 meters above the ground |
| 22             | Vertical visibility                       | vv                     | (m)      | Instantaneous vertical visibility                            |

