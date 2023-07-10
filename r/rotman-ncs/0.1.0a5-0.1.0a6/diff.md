# Comparing `tmp/rotman_ncs-0.1.0a5-py3-none-any.whl.zip` & `tmp/rotman_ncs-0.1.0a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,16 @@
-Zip file size: 620086 bytes, number of entries: 20
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 19:17 call_strategy/__init__.py
--rw-r--r--  2.0 unx   274806 b- defN 23-Jul-09 19:17 call_strategy/random_action.csv
--rw-r--r--  2.0 unx    76695 b- defN 23-Jul-09 19:17 call_strategy/random_strategy_portfolio.parquet
--rw-r--r--  2.0 unx   149006 b- defN 23-Jul-09 19:17 call_strategy/random_strategy_portfolio_10d.parquet
--rw-r--r--  2.0 unx    16686 b- defN 23-Jul-09 19:17 call_strategy/random_strategy_portfolio_1d.parquet
--rw-r--r--  2.0 unx    76219 b- defN 23-Jul-09 19:17 call_strategy/random_strategy_portfolio_5d.parquet
--rw-r--r--  2.0 unx   279457 b- defN 23-Jul-09 19:17 call_strategy/spy_action.csv
--rw-r--r--  2.0 unx    12797 b- defN 23-Jul-09 19:17 call_strategy/spy_strategy_portfolio.parquet
--rw-r--r--  2.0 unx    12418 b- defN 23-Jul-09 19:17 call_strategy/strategy.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Jul-09 19:17 data/__init__.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Jul-09 19:17 data/downloader.py
--rw-r--r--  2.0 unx       76 b- defN 23-Jul-09 19:17 model/__init__.py
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-09 19:17 model/config.py
--rw-r--r--  2.0 unx     2855 b- defN 23-Jul-09 19:17 model/inference.py
--rw-r--r--  2.0 unx     6278 b- defN 23-Jul-09 19:17 model/train.py
--rw-r--r--  2.0 unx    11355 b- defN 23-Jul-09 19:19 rotman_ncs-0.1.0a5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4205 b- defN 23-Jul-09 19:19 rotman_ncs-0.1.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 19:19 rotman_ncs-0.1.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-09 19:19 rotman_ncs-0.1.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1721 b- defN 23-Jul-09 19:19 rotman_ncs-0.1.0a5.dist-info/RECORD
-20 files, 927650 bytes uncompressed, 617278 bytes compressed:  33.5%
+Zip file size: 17838 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      281 b- defN 23-Jul-09 23:58 ncs/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-09 23:58 ncs/call_strategy/__init__.py
+-rw-r--r--  2.0 unx    13714 b- defN 23-Jul-09 23:58 ncs/call_strategy/strategy.py
+-rw-r--r--  2.0 unx     2804 b- defN 23-Jul-09 23:58 ncs/data/__init__.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jul-09 23:58 ncs/data/downloader.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-09 23:58 ncs/model/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-09 23:58 ncs/model/config.py
+-rw-r--r--  2.0 unx     2822 b- defN 23-Jul-09 23:58 ncs/model/inference.py
+-rw-r--r--  2.0 unx     7183 b- defN 23-Jul-09 23:58 ncs/model/train.py
+-rw-r--r--  2.0 unx    11355 b- defN 23-Jul-09 23:59 rotman_ncs-0.1.0a6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6876 b- defN 23-Jul-09 23:59 rotman_ncs-0.1.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 23:59 rotman_ncs-0.1.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-09 23:59 rotman_ncs-0.1.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1114 b- defN 23-Jul-09 23:59 rotman_ncs-0.1.0a6.dist-info/RECORD
+14 files, 47891 bytes uncompressed, 15994 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,61 +1,43 @@
-Filename: call_strategy/__init__.py
+Filename: ncs/__init__.py
 Comment: 
 
-Filename: call_strategy/random_action.csv
+Filename: ncs/call_strategy/__init__.py
 Comment: 
 
-Filename: call_strategy/random_strategy_portfolio.parquet
+Filename: ncs/call_strategy/strategy.py
 Comment: 
 
-Filename: call_strategy/random_strategy_portfolio_10d.parquet
+Filename: ncs/data/__init__.py
 Comment: 
 
-Filename: call_strategy/random_strategy_portfolio_1d.parquet
+Filename: ncs/data/downloader.py
 Comment: 
 
-Filename: call_strategy/random_strategy_portfolio_5d.parquet
+Filename: ncs/model/__init__.py
 Comment: 
 
-Filename: call_strategy/spy_action.csv
+Filename: ncs/model/config.py
 Comment: 
 
-Filename: call_strategy/spy_strategy_portfolio.parquet
+Filename: ncs/model/inference.py
 Comment: 
 
-Filename: call_strategy/strategy.py
+Filename: ncs/model/train.py
 Comment: 
 
-Filename: data/__init__.py
+Filename: rotman_ncs-0.1.0a6.dist-info/LICENSE
 Comment: 
 
-Filename: data/downloader.py
+Filename: rotman_ncs-0.1.0a6.dist-info/METADATA
 Comment: 
 
-Filename: model/__init__.py
+Filename: rotman_ncs-0.1.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: model/config.py
+Filename: rotman_ncs-0.1.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: model/inference.py
-Comment: 
-
-Filename: model/train.py
-Comment: 
-
-Filename: rotman_ncs-0.1.0a5.dist-info/LICENSE
-Comment: 
-
-Filename: rotman_ncs-0.1.0a5.dist-info/METADATA
-Comment: 
-
-Filename: rotman_ncs-0.1.0a5.dist-info/WHEEL
-Comment: 
-
-Filename: rotman_ncs-0.1.0a5.dist-info/top_level.txt
-Comment: 
-
-Filename: rotman_ncs-0.1.0a5.dist-info/RECORD
+Filename: rotman_ncs-0.1.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `call_strategy/strategy.py` & `ncs/call_strategy/strategy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ncs.data import *
+from ..data import *
 import pandas as pd
 import numpy as np
 import plotly.express as px
 from IPython.display import display, HTML
 
 import os
 import argparse
@@ -215,14 +215,26 @@
 
 
 def run_strategy(
         action_file=f'{cur_dir}/benchmark_action.csv',
         holding_period=5,
         log_file='',
         save_portfolio_path='./portfolio.parquet',):
+    """
+    Run strategy using the provided action file, holding period, log file, and save portfolio path.
+
+    Parameters:
+        action_file (str): Path to the action file containing the buy / no action / sell actions, (default: './benchmark_action.csv').
+        holding_period (int): Holding period for the strategy (1-day, 5-days, or 10-days) (default: 5).
+        log_file (str): Path to the log file (default: '').
+        save_portfolio_path (str): Path to save the portfolio file containing the portfolio values (default: './portfolio.parquet').
+
+    Returns:
+        None
+    """
     # set log_file and terminal output
     logging.basicConfig(
         level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
         handlers=[logging.StreamHandler()] +
         [] if log_file == '' else [logging.FileHandler(log_file)],
         datefmt='%Y-%m-%d %H:%M:%S'
     )
@@ -238,14 +250,30 @@
     return
 
 
 def report_strategy_analysis(actions,
                              portfolio,
                              holding_period,
                              model_name='Strategy Portfolio Values'):
+    """
+    Generate a report of the strategy analysis for a given set of actions and portfolio.
+    The report contains
+    1. Portfolio performance metrics
+    2. Trade performance metrics
+    3. Portfolio value plot    
+
+    Parameters:
+        actions (str): Path to the CSV file containing the actions.
+        portfolio (str): Path to the Parquet file containing the portfolio values generated by run_strategy function.
+        holding_period (int): The holding period of the strategy (1, 5, or 10 days).
+        model_name (str, optional): The name of the model used for plotting title. Defaults to 'Strategy Portfolio Values'.
+
+    Returns:
+        None
+    """
     actions = pd.read_csv(actions)
     portfolio = pd.read_parquet(portfolio)
     plot(portfolio, model_name=model_name)
     # display dataframe in html
     display(HTML(calc_performance(portfolio).to_html()))
     display(HTML(trade_analysis(actions, holding_period).to_html()))
 
@@ -254,15 +282,15 @@
     """Run benchmark strategy.
 
     Parameters
     ----------
     strategy : str
         Strategy name. 'spy' or 'random'.
     holding_period : int
-        Holding period (1, 5, 10 days). Default is 5.
+        Holding period (1, 5, 10 days) only used when strategy is 'random'. Default is 5.
 
     Returns
     -------
     None
     """
     report_strategy_analysis(
         f'{cur_dir}/{strategy}_action.csv',
```

## Comparing `data/downloader.py` & `ncs/data/downloader.py`

 * *Files identical despite different names*

## Comparing `model/inference.py` & `ncs/model/inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Run evaluation on the test set
 '''
-from ncs.model.config import default_role_weights, default_section_weights, default_statement_type_weights, default_holding_period
+from .config import default_role_weights, default_section_weights, default_statement_type_weights
 import pandas as pd
 import os
 import pickle
 import warnings
 warnings.filterwarnings('ignore')
```

## Comparing `model/train.py` & `ncs/model/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ncs.data import load_stock_returns_on_calls, load_call_statements
-from ncs.model.config import default_role_weights, default_section_weights, default_statement_type_weights, default_holding_period
+from ..data import load_stock_returns_on_calls, load_call_statements
+from .config import default_role_weights, default_section_weights, default_statement_type_weights, default_holding_period
 import pandas as pd
 from sklearn.metrics import classification_report
 from sklearn.model_selection import train_test_split
 from sklearn.model_selection import GridSearchCV
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.linear_model import LogisticRegression
 from sklearn.neural_network import MLPClassifier
@@ -23,14 +23,31 @@
           section_weights=default_section_weights,
           statement_type_weights=default_statement_type_weights,
           sell_quantile=0.35,
           buy_quantile=0.65,
           holding_period=default_holding_period,
           classifier='logistic_regression',
           save_model='model.pkl'):
+    """
+    Train a model using the provided feature files and parameters.
+
+    Parameters:
+        - feature_files: A list of paths to feature files.
+        - role_weights: A dictionary of weights for different presentor roles.
+        - section_weights: A dictionary of weights for different sections.
+        - statement_type_weights: A dictionary of weights for different statement types.
+        - sell_quantile: The quantile value for determining the sell threshold. Defaults to 0.35.
+        - buy_quantile: The quantile value for determining the buy threshold. Defaults to 0.65.
+        - holding_period: The holding period for the stock return data.
+        - classifier: The type of classifier to use for training ('logistic_regression', 'random_forest', or 'neural_network'). Defaults to 'logistic_regression'.
+        - save_model: The path to save the trained model.
+
+    Returns:
+        None
+    """
     # load features
     feature_df = call_statement_data[[
         'statement_uid', 'call_uid', 'presentor_role', 'section', 'statement_type']].set_index('statement_uid')
 
     feature_cols = []
     for feature_file in feature_files:
         feature_data = pd.read_parquet(feature_file)
```

## Comparing `rotman_ncs-0.1.0a5.dist-info/LICENSE` & `rotman_ncs-0.1.0a6.dist-info/LICENSE`

 * *Files identical despite different names*

