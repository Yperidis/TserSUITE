# Overview
The TserSUITE is inteded to be a holistic suite of tools for performing a wide range of time series analysis techniques.

Currently the endeavour consists of three Jupyter notebooks written in Python, two out of which assume an input of keyword-value 
csv files for the series in question. The third (Requests) attempts to lay out the backbone of API calls for data collection purposes.
In brief, the other two files' functionality is as follows:

1. Data_analysis.ipynb: 
* Data processing and wrangling considering of the input csv files. 
* Similarity of like values (items) across the whole
dataset and over the given period. 
* Visualizations of items' overlap via Venn diagrams, various evolution plots of the series (also cumulative) and pie charts. 
* Basic clustering and dimensionality reduction with k-means clustering and k-means neighbours with PCA.

2. G_Causality.ipynb (culminating on the Granger causality test): 
* A preprocessing stage as in Data_analysis.ipynb.
* Normality statistical tests.
* Covariance of the given series. Summarise in matrix and visualise.
* Autocorrelation visualisations with significance intervals and visualization.
* Testing for stationarity and rendering the series static (if the test is negative) by consecutive differencing. Visualize.
* Perform for all given time series the Granger causality test and summarise the results on a matrix. Visualise the latter.
* If all the above is satisfied, attempt to construct a vector autoregression model for forecasting purposes.
* Discrete Fourier analysis of the time series and visualisation.
* Wavelet (Morlet) analysis and visualisation.

The inspiration for the code was drawn by projects of mine while being a postdoc at the US army corps of engineers.

### Dependencies
The code draws heavily from the pandas dataframe, numpy and scikit-learn modules for analysis purposes, 
and matplotlib and seaborn for visualizations.
* Pandas (checked with 0.25.1).
* Numpy (checked with 1.16.5).
* Scipy (checked with 1.3.1).
* Matplotlib (checked with 3.2.0).
* Time.
* Seaborn (checked with 0.9.0).
* Statsmodels (0.10.1).
* Sklearni (0.21.3).
* Mpltoolkits.
* Json (2.0.9).
* Requests (2.22.0).
