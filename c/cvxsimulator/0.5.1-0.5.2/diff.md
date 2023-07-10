# Comparing `tmp/cvxsimulator-0.5.1.tar.gz` & `tmp/cvxsimulator-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.5.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.5.2.tar", max compression
```

## Comparing `cvxsimulator-0.5.1.tar` & `cvxsimulator-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-06-11 21:28:16.366250 cvxsimulator-0.5.1/LICENSE
--rw-r--r--   0        0        0     5051 2023-06-11 21:28:16.366250 cvxsimulator-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    16264 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1209 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1457 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/month.py
--rw-r--r--   0        0        0    19295 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-06-11 21:28:16.458251 cvxsimulator-0.5.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      633 2023-06-11 21:28:52.266601 cvxsimulator-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5643 1970-01-01 00:00:00.000000 cvxsimulator-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-07-10 14:46:35.394627 cvxsimulator-0.5.2/LICENSE
+-rw-r--r--   0        0        0     5166 2023-07-10 14:46:35.394627 cvxsimulator-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    16257 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1209 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1457 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/month.py
+-rw-r--r--   0        0        0    19303 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-07-10 14:46:35.486628 cvxsimulator-0.5.2/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      726 2023-07-10 14:47:10.598803 cvxsimulator-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5784 1970-01-01 00:00:00.000000 cvxsimulator-0.5.2/PKG-INFO
```

### Comparing `cvxsimulator-0.5.1/LICENSE` & `cvxsimulator-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.1/README.md` & `cvxsimulator-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# [cvxsimulator](http://www.cvxgrp.org/simulator/)
+# [cvxsimulator](https://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/cvxgrp/simulator)
+
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
 
 ## Modus operandi
```

### Comparing `cvxsimulator-0.5.1/cvx/simulator/builder.py` & `cvxsimulator-0.5.2/cvx/simulator/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-from dataclasses import dataclass
-from dataclasses import field
+from dataclasses import dataclass, field
 
 import pandas as pd
 
 from cvx.simulator.portfolio import EquityPortfolio
 from cvx.simulator.trading_costs import TradingCostModel
 
 
@@ -313,15 +312,17 @@
         for t in self.index:
             # valuation of the current position
             self._state.prices = self.prices.loc[t]
             yield self.index[self.index <= t], self._state
 
     def __setitem__(self, time, position):
         """
-        The method __setitem__ updates the stock data in the dataframe for a specific time index with the input position. It first checks that position is a valid input, meaning it is a pandas Series object and has its index within the assets of the dataframe.
+        The method __setitem__ updates the stock data in the dataframe for a specific time index
+        with the input position. It first checks that position is a valid input,
+        meaning it is a pandas Series object and has its index within the assets of the dataframe.
         The method takes two input parameters:
 
         time: time index for which to update the stock data
         position: pandas series object containing the updated stock data
 
         Returns: None
```

### Comparing `cvxsimulator-0.5.1/cvx/simulator/grid.py` & `cvxsimulator-0.5.2/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.1/cvx/simulator/metrics.py` & `cvxsimulator-0.5.2/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.1/cvx/simulator/month.py` & `cvxsimulator-0.5.2/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.5.2/cvx/simulator/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,16 @@
         as the stocks dataframe, with NaN values filled with zeros."""
         t = self.stocks.diff()
         t.loc[self.index[0]] = self.stocks.loc[self.index[0]]
         return t.fillna(0.0)
 
     @property
     def trades_currency(self) -> pd.DataFrame:
-        """A property that returns a pandas dataframe representing the trades made in the portfolio in terms of currency.
+        """A property that returns a pandas dataframe representing
+        the trades made in the portfolio in terms of currency.
 
         Returns: pd.DataFrame: A pandas dataframe representing the trades made in the portfolio in terms of currency.
 
         Notes: The function calculates the trades made in currency by multiplying
         the number of shares of each asset bought or sold (as represented in the trades_stocks dataframe)
         with the current prices of each asset (as represented in the prices dataframe).
         Uses pandas ffill() method to forward fill NaN values in the prices dataframe.
```

### Comparing `cvxsimulator-0.5.1/cvx/simulator/trading_costs.py` & `cvxsimulator-0.5.2/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.5.1/PKG-INFO` & `cvxsimulator-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: quantstats
 Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
-# [cvxsimulator](http://www.cvxgrp.org/simulator/)
+# [cvxsimulator](https://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
+[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/cvxgrp/simulator)
+
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
 
 ## Modus operandi
```

