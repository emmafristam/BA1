# BA
Bachelor Thesis Data Analysis

## ARIMA Model

import pandas as pd
import numpy as np
%matplotlib inline

import warnings
warnings.filterwarnings("ignore")

import statsmodels as sm
from statsmodels.tsa.arima_model import ARMA, ARIMA, ARMAResults, ARIMAResults

from pmdarima import auto_arima

Error: 

---------------------------------------------------------------------------
ImportError                               Traceback (most recent call last)
<ipython-input-56-241dcca81435> in <module>
----> 1 from pmdarima import auto_arima

~/opt/anaconda3/lib/python3.7/site-packages/pmdarima/__init__.py in <module>
     47 
     48     # Stuff we want at top-level
---> 49     from .arima import auto_arima, ARIMA, AutoARIMA, StepwiseContext, decompose
     50     from .utils import acf, autocorr_plot, c, pacf, plot_acf, plot_pacf, \
     51         tsdisplay

~/opt/anaconda3/lib/python3.7/site-packages/pmdarima/arima/__init__.py in <module>
      4 
      5 from .approx import *
----> 6 from .arima import *
      7 from .auto import *
      8 from .utils import *

~/opt/anaconda3/lib/python3.7/site-packages/pmdarima/arima/arima.py in <module>
     11 
     12 from statsmodels.tsa.base.tsa_model import TimeSeriesModelResults
---> 13 from statsmodels import api as sm
     14 
     15 from scipy.stats import gaussian_kde, norm

~/opt/anaconda3/lib/python3.7/site-packages/statsmodels/api.py in <module>
      9 from . import regression
     10 from .regression.linear_model import OLS, GLS, WLS, GLSAR
---> 11 from .regression.recursive_ls import RecursiveLS
     12 from .regression.quantile_regression import QuantReg
     13 from .regression.mixed_linear_model import MixedLM

~/opt/anaconda3/lib/python3.7/site-packages/statsmodels/regression/recursive_ls.py in <module>
      9 import pandas as pd
     10 
---> 11 from statsmodels.compat.pandas import Appender
     12 
     13 from statsmodels.tools.data import _is_using_pandas

ImportError: cannot import name 'Appender' from 'statsmodels.compat.pandas' (/Users/emmafristam/opt/anaconda3/lib/python3.7/site-packages/statsmodels/compat/pandas.py)
