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
from functools import reduce
import seaborn as sns
from scipy.stats import shapiro
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
from sklearn.linear_model import LinearRegression
import statsmodels.api as sm
```

## Documentation
- LISCENCE.MD: proper citation for repository
- SCRIPTS folder: source code for project 
- DATA folder: initial data (for pH/CO2, surface temperature, global temperature, plankton population) and final cleaned data
- OUTPUT: figures and tables generated from scripts
- REFERENCES: sources used throughout project

## Reproducing results
SCRIPTS: The script provided is the final script to clean the data, perform an EDA, and analyze the time series through ARIMAX. 

CLEAN DATA & EDA: date time and average dataframe by year if needed. Plot each variable and visualize correlation matrix.

ANALYSIS: prep ARIMAX by differencing data if they're non-stationary. 
1. Forecast future pH using historical CO2, sea surface temp, global temperature, and number of eruptions, then perform statistical tests.
2. Forecast future plankton populations using historical pH measurements, and perform statistical tests.  

Output =  EDA graphs, new dataframe (Final Clean Data.csv), statistical summaries of each test

