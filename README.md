# DSproject2
The purpose of this project is to understand the cause and affects of ocean acidification. Below is documentation for reproducability. 

## Software and Platform
This project used Python programming through Jupyter Notebook on Windows platform.

Required imports and libraries:
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import xarray as xr
import seaborn as sns
from statsmodels.tsa.stattools import adfuller
import pmdarima as pm
from statsmodels.tsa.statespace.sarimax import SARIMAX
from sklearn.preprocessing import StandardScaler
```

## Documentation
- LISCENCE.MD: proper citation for repository
- SCRIPTS folder: source code for project 
- DATA folder: initial data (for pH/CO2, surface temperature, global temperature, plankton population) and final cleaned data
- OUTPUT: figures and tables generated from scripts
- REFERENCES: sources used throughout project

## Reproducing results
SCRIPTS:

1.Tweet_Sentiment_Analysis_&_EDA: Read in Musk tweets dataset imported from Kaggle and perform sentiment analysis and EDA. 

Output = new dataframe (Tweet Sentiment Data.csv), EDA graphs

2.Stock_Price_EDA: Read in Tesla stock prices from yfinance over same period of time as twitter dataset, and perform EDA.

Output = new dataframe (Tesla Stock.csv), EDA graphs

3.Data Analysis: This re-reads in Musk tweets and Tesla stock price dataframes, 1)processes and merges data into 1 dataframe (Merged Data.csv), 2)process merged dataframe for time-series analysis so both sets of data are stationary, and 3)performes multiple statistical analysis' to test relationship between sentiment of Musk's tweets and Tesla stock prices.

Output = new dataframe (Merged Data.csv), and statistical summaries of each test
