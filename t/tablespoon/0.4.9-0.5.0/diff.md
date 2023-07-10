# Comparing `tmp/tablespoon-0.4.9.tar.gz` & `tmp/tablespoon-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablespoon-0.4.9.tar", max compression
+gzip compressed data, was "tablespoon-0.5.0.tar", max compression
```

## Comparing `tablespoon-0.4.9.tar` & `tablespoon-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-02-02 15:48:15.619144 tablespoon-0.4.9/LICENSE
--rw-r--r--   0        0        0     8862 2023-02-02 15:48:15.619272 tablespoon-0.4.9/README.md
--rw-r--r--   0        0        0      956 2023-07-07 20:13:42.179744 tablespoon-0.4.9/pyproject.toml
--rw-r--r--   0        0        0       84 2023-02-02 15:48:15.627496 tablespoon-0.4.9/tablespoon/__init__.py
--rw-r--r--   0        0        0   432508 2023-02-02 15:48:15.628400 tablespoon-0.4.9/tablespoon/data.py
--rw-r--r--   0        0        0    12065 2023-02-02 15:48:15.628579 tablespoon-0.4.9/tablespoon/forecasters.py
--rw-r--r--   0        0        0     3428 2023-02-02 15:48:15.628691 tablespoon-0.4.9/tablespoon/model_selection.py
--rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 tablespoon-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-09 12:25:34.922534 tablespoon-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8862 2023-07-09 12:25:34.922534 tablespoon-0.5.0/README.md
+-rw-r--r--   0        0        0      888 2023-07-09 16:57:20.068349 tablespoon-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-07-09 18:14:26.378753 tablespoon-0.5.0/tablespoon/__init__.py
+-rw-r--r--   0        0        0   432508 2023-07-09 12:25:34.930534 tablespoon-0.5.0/tablespoon/data.py
+-rw-r--r--   0        0        0    22258 2023-07-10 04:01:42.966847 tablespoon-0.5.0/tablespoon/forecasters.py
+-rw-r--r--   0        0        0     3428 2023-07-09 12:25:34.930534 tablespoon-0.5.0/tablespoon/model_selection.py
+-rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 tablespoon-0.5.0/PKG-INFO
```

### Comparing `tablespoon-0.4.9/LICENSE` & `tablespoon-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.9/README.md` & `tablespoon-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.9/pyproject.toml` & `tablespoon-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -19,24 +19,20 @@
   "seasonal naive",
   "mean forecast",
 ]
 license = "MIT"
 name = "tablespoon"
 readme = "README.md"
 repository = "https://github.com/alexhallam/tablespoon"
-version = "0.4.9"
+version = "0.5.0"
 
 [tool.poetry.dependencies]
 numpy = "^1.23.0"
 pandas = "^1.3.2"
 pytest = "7.0.0"
 python = ">=3.10"
 scipy = "^1.9.3"
 statsmodels = "^0.14.0"
 
-[tool.poetry.dev-dependencies]
-numpy = "^1.21.2"
-pandas = "^1.3.2"
-
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `tablespoon-0.4.9/tablespoon/data.py` & `tablespoon-0.5.0/tablespoon/data.py`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.9/tablespoon/forecasters.py` & `tablespoon-0.5.0/tablespoon/forecasters.py`

 * *Files 25% similar despite different names*

```diff
@@ -148,14 +148,95 @@
             )
         np_predictions = forecast.transpose().reshape(
             uncertainty_samples * horizon, 1
         )
         df_pred = pd.DataFrame(np_predictions, columns=["y_sim"])
         df_result = pd.concat([df_cross, df_pred], axis=1)
         return df_result
+    
+    def fitted_params(
+        self,
+        df_historical,
+        horizon=30,
+        frequency=None,
+        lag=1,
+        uncertainty_samples=5000,
+        include_history=False,
+    ):
+        """Fitted Parameters - forecast method
+
+        Args:
+            df_historical (pd.DataFrame): A date sorted dataframe with the columns `ds` and `y`
+            horizon (int, optional): Forecast horizon. Defaults to 30.
+            frequency (int, optional): number of rows that make a seasonal period. Defaults to None.
+            lag (int, optional): number of rows that make a seasonal period. Defaults to 1.
+            uncertainty_samples (int, optional): number of uncertainty samples to draw. Defaults to 5000.
+            include_history (bool, optional): include history. Defaults to False.
+            chain_ids (str, optional): identifiers for chain ids. Defaults to None.
+            verbose (bool, optional): verbose. Defaults to False.
+
+        Returns:
+            pd.DataFrame: A dataframe of predictions as `y_sim`
+
+        Example:
+            ```py
+            import pandas as pd
+            import tablespoon as tbsp
+            from tablespoon.data import APPL
+            df_APPLE = APPL
+            df_APPLE = df_APPLE.assign(ds = lambda df: pd.to_datetime(df.ds))
+            naive = tbsp.Naive()
+            df_f = (naive.predict(df_APPLE, horizon=7*4, frequency="D", lag = 1, uncertainty_samples = 500).assign(model = 'naive'))
+            df_f.head(10)
+            ```
+        """
+        if frequency is None:
+            send_helpful_frequency_error()
+        self.y = df_historical["y"]
+        self.history_dates = get_sorted_dates(df_historical)
+        last_date = self.history_dates.max()
+        min_date = self.history_dates.min()
+        check_historical_dates_are_contiguous(
+            self.history_dates, min_date, last_date, frequency
+        )
+        dates = pd.date_range(
+            start=last_date, periods=horizon + 1, freq=frequency
+        )  # An extra in case we include start  # 'M','D', etc.
+        dates = dates[dates > last_date]  # Drop start if equals last_date
+        dates = dates[:horizon]  # Return correct number of periods
+        if include_history:
+            dates = np.concatenate((np.array(self.history_dates), dates))
+        df_dates = pd.DataFrame({"ds": dates})
+        df_samples = pd.DataFrame({"rep": np.arange(uncertainty_samples)})
+        df_cross = df_dates.merge(df_samples, how="cross")
+        # fit
+        t = lag + 1
+        t_lag = t - lag
+        y = self.y.to_numpy()
+        end = len(y) - lag
+        yt = y[t:]
+        yt_lag = y[t_lag:end]
+        y_last = y.take(-1)
+        mod = sm.GLM(yt, yt_lag, family=sm.families.Gaussian())
+        sigma = np.sqrt(mod.fit().scale)
+        rng = np.random.default_rng()
+        forecast = np.empty([uncertainty_samples, horizon])
+        # fitted params
+        params_list = []
+        for h in range(0, horizon):
+            params_dict = {}
+            # make dictionary of parameters
+            params_dict["ds"] = dates[h]
+            params_dict["mu"] = np.round(y_last, 2)
+            params_dict["sigma"] = np.round(sigma * np.sqrt(h + 1),2)
+            mu = params_dict["mu"]; sd = params_dict["sigma"];
+            params_dict['dist'] = f"N({mu}, {sd})"
+            params_list.append(params_dict)
+        return pd.DataFrame(params_list)
+
 
 
 class Mean(object):
     """
     Mean Forecaster
     """
 
@@ -233,14 +314,95 @@
             )
         np_predictions = forecast.transpose().reshape(
             uncertainty_samples * horizon, 1
         )
         df_pred = pd.DataFrame(np_predictions, columns=["y_sim"])
         df_result = pd.concat([df_cross, df_pred], axis=1)
         return df_result
+    
+    def fitted_params(
+        self,
+        df_historical,
+        horizon=30,
+        frequency=None,
+        uncertainty_samples=5000,
+        include_history=False,
+    ):
+        """Fitted Parameters
+
+        Args:
+            df_historical (pd.DataFrame): A date sorted dataframe with the columns `ds` and `y`
+            horizon (int, optional): Forecast horizon. Defaults to 30.
+            frequency (int, optional): number of rows that make a seasonal period. Defaults to None.
+            lag (int, optional): number of rows that make a seasonal period. Defaults to 1.
+            uncertainty_samples (int, optional): number of uncertainty samples to draw. Defaults to 5000.
+            include_history (bool, optional): include history. Defaults to False.
+            chain_ids (str, optional): identifiers for chain ids. Defaults to None.
+            verbose (bool, optional): verbose. Defaults to False.
+
+        Returns:
+            pd.DataFrame: A dataframe of predictions as `y_sim`
+
+        Example:
+            ```py
+            import pandas as pd
+            import tablespoon as tbsp
+            from tablespoon.data import APPL
+            df_APPLE = APPL
+            df_APPLE = df_APPLE.assign(ds = lambda df: pd.to_datetime(df.ds))
+            mean = tbsp.Mean()
+            df_f = (n.predict(df_APPLE, horizon=7*4, frequency="D", lag = 1, uncertainty_samples = 500).assign(model = 'mean'))
+            df_f.head(10)
+            ```
+        """
+        self.y = df_historical["y"]
+        self.history_dates = get_sorted_dates(df_historical)
+        last_date = self.history_dates.max()
+        min_date = self.history_dates.min()
+        check_historical_dates_are_contiguous(
+            self.history_dates, min_date, last_date, frequency
+        )
+        dates = pd.date_range(
+            start=last_date, periods=horizon + 1, freq=frequency
+        )  # An extra in case we include start  # 'M','D', etc.
+        dates = dates[dates > last_date]  # Drop start if equals last_date
+        dates = dates[:horizon]  # Return correct number of periods
+        if include_history:
+            dates = np.concatenate((np.array(self.history_dates), dates))
+        df_dates = pd.DataFrame({"ds": dates})
+        df_samples = pd.DataFrame({"rep": np.arange(uncertainty_samples)})
+        df_cross = df_dates.merge(df_samples, how="cross")
+        # fit
+        y = self.y
+        T = len(y)
+        deg_freedom = T - 1
+        mu, sigma = norm.fit(y)
+        rng = np.random.default_rng()
+        forecast = np.empty([uncertainty_samples, horizon])
+        for h in range(0, horizon):
+            forecast[:, h] = mu + sigma * np.sqrt(1 + (1 / T)) * rng.standard_t(
+                df=deg_freedom, size=uncertainty_samples
+            )
+        np_predictions = forecast.transpose().reshape(
+            uncertainty_samples * horizon, 1
+        )
+        df_pred = pd.DataFrame(np_predictions, columns=["y_sim"])
+        df_result = pd.concat([df_cross, df_pred], axis=1)
+        ## fitted params
+        params_list = []
+        for h in range(0, horizon):
+            params_dict = {}
+            # make dictionary of parameters
+            params_dict["ds"] = dates[h]
+            params_dict["mu"] = np.round(mu, 2)
+            params_dict["sigma"] = np.round(sigma * np.sqrt(1 + (1 / T)),2)
+            mu = params_dict["mu"]; sd = params_dict["sigma"];
+            params_dict['dist'] = f"N({mu}, {sd})"
+            params_list.append(params_dict)
+        return pd.DataFrame(params_list)
 
 
 class Snaive(object):
     """
     Seasonal Naive Forecaster
     """
 
@@ -307,18 +469,89 @@
         # fit
         y = self.y.to_numpy()
         last_start = len(y) - lag
         last_end = len(y)
         yt = y[lag:last_end]
         yt_lag = y[0:last_start]
         mod = sm.GLM(yt, yt_lag, family=sm.families.Gaussian())
-        sigma = np.sqrt(mod.fit().scale)
+        sigma = np.sqrt(mod.fit().scale) # attempt to use glm to get sigma
         rng = np.random.default_rng()
         forecast = np.empty([uncertainty_samples, horizon])
         for h in range(0, horizon):
             forecast[:, h] = y[(len(y)) - (lag - ((h) % lag))] + sigma * np.sqrt(np.trunc(((h) * 1) / (lag)) + 1) * rng.standard_normal(uncertainty_samples)
         np_predictions = forecast.transpose().reshape(
             uncertainty_samples * horizon, 1
         )
         df_pred = pd.DataFrame(np_predictions, columns=["y_sim"])
         df_result = pd.concat([df_cross, df_pred], axis=1)
         return df_result
+
+    def fitted_params(
+        self,
+        df_historical,
+        horizon=30,
+        frequency=None,
+        lag=7,
+        uncertainty_samples=5000,
+        include_history=False,
+    ):
+        """Fitted Parameters - Normal(mu, sigma)
+
+        Args:
+            df_historical (pd.DataFrame): A date sorted dataframe with the columns `ds` and `y`
+            horizon (int, optional): Forecast horizon. Defaults to 30.
+            frequency (int, optional): number of rows that make a seasonal period. Defaults to None.
+            lag (int, optional): number of rows that make a seasonal period. Defaults to 7 (7 days of a week).
+            uncertainty_samples (int, optional): number of uncertainty samples to draw. Defaults to 5000.
+            include_history (bool, optional): include history. Defaults to False.
+            chain_ids (str, optional): identifiers for chain ids. Defaults to None.
+            verbose (bool, optional): verbose. Defaults to False.
+
+        Returns:
+            dictionary: A dictionary of fitted parameters as `ds`, `mu`, and `sigma`
+
+        Example:
+            ```py
+            import tablespoon as tbsp
+            from tablespoon.data import SEAS
+            sn = tbsp.Snaive()
+            df_f = sn.fitted_params(SEAS, horizon=7 * 4, frequency="D", lag=7, uncertainty_samples=800).assign(model="snaive")
+            df_f.head(10)
+            ```
+        """
+        self.y = df_historical["y"]
+        self.history_dates = get_sorted_dates(df_historical)
+        last_date = self.history_dates.max()
+        min_date = self.history_dates.min()
+        check_historical_dates_are_contiguous(
+            self.history_dates, min_date, last_date, frequency
+        )
+        dates = pd.date_range(
+            start=last_date, periods=horizon + 1, freq=frequency
+        )  # An extra in case we include start  # 'M','D', etc.
+        dates = dates[dates > last_date]  # Drop start if equals last_date
+        dates = dates[:horizon]  # Return correct number of periods
+        if include_history:
+            dates = np.concatenate((np.array(self.history_dates), dates))
+        df_dates = pd.DataFrame({"ds": dates})
+        df_samples = pd.DataFrame({"rep": np.arange(uncertainty_samples)})
+        df_cross = df_dates.merge(df_samples, how="cross")
+        # fit
+        y = self.y.to_numpy()
+        last_start = len(y) - lag
+        last_end = len(y)
+        yt = y[lag:last_end]
+        yt_lag = y[0:last_start]
+        mod = sm.GLM(yt, yt_lag, family=sm.families.Gaussian())
+        # the variable sigma represents the estimated standard deviation of the residuals from the generalized linear model (GLM) fit.
+        sigma = np.sqrt(mod.fit().scale)
+        params_list = []
+        for h in range(0, horizon):
+            params_dict = {}
+            # make dictionary of parameters
+            params_dict["ds"] = dates[h]
+            params_dict["mu"] = y[(len(y)) - (lag - ((h) % lag))]
+            params_dict["sigma"] = np.round(sigma * np.sqrt(np.trunc(((h) * 1) / (lag)) + 1),2)
+            mu = params_dict["mu"]; sd = params_dict["sigma"];
+            params_dict['dist'] = f"N({mu}, {sd})"
+            params_list.append(params_dict)
+        return pd.DataFrame(params_list)
```

### Comparing `tablespoon-0.4.9/tablespoon/model_selection.py` & `tablespoon-0.5.0/tablespoon/model_selection.py`

 * *Files identical despite different names*

### Comparing `tablespoon-0.4.9/PKG-INFO` & `tablespoon-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablespoon
-Version: 0.4.9
+Version: 0.5.0
 Summary: Simple probabilistic time series benchmark models
 Home-page: https://alexhallam.github.io/tablespoon/
 License: MIT
 Keywords: forecasting,forecast,probabilistic,naive,benchmark,seasonal naive,mean forecast
 Author: Alex Hallam
 Author-email: alexhallam6.28@gmail.com
 Requires-Python: >=3.10
```

