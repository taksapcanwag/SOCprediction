# An LSTM approach for predicting soil organic carbon content using Landsat-8/9 and Sentinel-1 data

## Table of Contents

- [About](#about)
- [Contributing](#contributing)
- [License](#license)

## About

Soil organic carbon (SOC) is a key substance for tackling current challenges including climate change, food security and biodiversity loss, making it important to develop strong methods for SOC predictions. Recently-developed satellite remote sensing and deep learning have given us potential powerful tools for accurate predictions of SOC. Thus, the objective of this study is to explore the potential of an LSTM approach using Landsat and Sentinel-1 time-series data. First, the Landsat 8/9, Sentinel-1, topography and climate data were collected and sorted into tabular datasets. These datasets consist of different kinds of timescales: 1, 2, 4 and 5 years in order to investigate the optimum time periods to consider for SOC predictions. Next, for each time scale, the LSTM and baseline RF models were constructed, trained and tested with the above-created tabular datasets. Lastly, the model performance was assessed with R2 and RMSE scores and variable importance based on SHAP values. The experimental results demonstrated the outperformance of LSTM models in R2 in all the datasets, indicating the importance of temporal dependencies and advanced non-linear learning. Moreover, 2-year and 4-year datasets gave better metric scores than 1-year and 5-year ones, suggesting the past temporal patterns of 2 to 4 years length are optimum for predicting SOC. Looking at the variable importance, Sentinel-1 bands are the least important for LSTM predictions and they can be replaced with other useful features. On the other hand, some Landsat variables contributed the most to the LSTM outputs, which is different from the RF model, showing the complex learning ability of the LSTM models to utilize the raw Landsat data. Meanwhile, the topography and climate data made substantial contributions in both LSTM and RF due to their broad relevance with SOC-related factors, such as land use and management, soil moisture and temperature, water flow and soil processes. Based on the key findings of this research, future research is expected to further explore different experimental settings of models, feature combinations and temporal frequencies and lengths.

## Contributors

Shoyo Nakamura, Tor-Gunnar Vagen (International Centre for Research in Agroforestry)

## License

Apache License 2.0
