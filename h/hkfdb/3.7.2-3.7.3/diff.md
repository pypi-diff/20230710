# Comparing `tmp/hkfdb-3.7.2.tar.gz` & `tmp/hkfdb-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.7.2.tar", last modified: Fri Jul  7 10:49:31 2023, max compression
+gzip compressed data, was "hkfdb-3.7.3.tar", last modified: Mon Jul 10 02:50:02 2023, max compression
```

## Comparing `hkfdb-3.7.2.tar` & `hkfdb-3.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-07 10:49:31.828866 hkfdb-3.7.2/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.2/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-07 10:49:31.828607 hkfdb-3.7.2/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.2/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-07 10:49:31.827005 hkfdb-3.7.2/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   108296 2023-07-07 04:27:05.000000 hkfdb-3.7.2/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.2/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-07 10:49:31.828308 hkfdb-3.7.2/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-07 10:49:31.000000 hkfdb-3.7.2/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-07 10:49:31.000000 hkfdb-3.7.2/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-07 10:49:31.000000 hkfdb-3.7.2/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-07 10:49:31.000000 hkfdb-3.7.2/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-07 10:49:31.000000 hkfdb-3.7.2/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-07 10:49:31.828944 hkfdb-3.7.2/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-07 10:48:33.000000 hkfdb-3.7.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-10 02:50:02.194467 hkfdb-3.7.3/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.3/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-10 02:50:02.194203 hkfdb-3.7.3/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.3/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-10 02:50:02.193163 hkfdb-3.7.3/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   109294 2023-07-09 04:51:35.000000 hkfdb-3.7.3/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.3/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-10 02:50:02.193894 hkfdb-3.7.3/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-10 02:50:02.194517 hkfdb-3.7.3/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-10 02:49:12.000000 hkfdb-3.7.3/setup.py
```

### Comparing `hkfdb-3.7.2/LICENSE` & `hkfdb-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.2/PKG-INFO` & `hkfdb-3.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.2
+Version: 3.7.3
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.2/README.md` & `hkfdb-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.2/hkfdb/Database.py` & `hkfdb-3.7.3/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,14 @@
         if False not in list(check_bool_dict.values()):
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token = str(self.authToken)
             start_date_str = str(start_date)
             end_date_str = str(end_date)
             link_str = f'{link_url}token={token}&database=hk_futures_ohlc&index={index}&freq={freq}&start_date={start_date_str}&end_date={end_date_str}'
-            # print(link_str)
 
             response = requests.get(link_str)
             response_ok = response_check(response)
 
 
             if response_ok == True:
 
@@ -309,14 +308,16 @@
                         df_single['datetime'] = pd.to_datetime(df_single['datetime'])
                         df_single['date'] = pd.to_datetime(df_single['datetime']).dt.strftime('%Y%m%d').astype(int)
                         df_single['time'] = pd.to_datetime(df_single['datetime']).dt.strftime('%H%M%S').astype(int)
                         df_single['RTH'] = df_single.apply(self.apply_RTH_ATH, axis=1)
 
                         if rth_only:
                             df_single = df_single[df_single['RTH'] == True]
+                        else:
+                            df_single = df_single[df_single['RTH'] == False]    # only 1D
 
                         df_all = []
 
                         for current_month in [True, False]:
                             df_current = df_single[df_single['current_month'] == current_month].sort_values(
                                 by=['datetime']).reset_index(drop=True)
                             df = df_current.head(1).copy()
@@ -329,14 +330,21 @@
                                 df['volume'] = df_current['volume'].sum()
 
                                 df_all.append(df.copy())
 
                         if len(df_all) > 0:
                             dfs.append(pd.concat(df_all))
 
+                    if len(dfs) == 0:
+                        column_names = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume',
+                                        'expiry_date', 'roll_diff']
+                        df = pd.DataFrame(columns=column_names)
+
+                        return df
+
                     df = pd.concat(dfs)
                     df['datetime'] = pd.to_datetime(df['datetime'])
 
                     ## Find the valid expiry date to processed , ie within date range
                     expiry_dates = list(df['expiry_date'].unique())
                     expiry_dates.sort()
 
@@ -431,39 +439,46 @@
 
                             df_roll = df[(df['date'] == exact_rolling_date)].copy()
                             df_roll = df_roll[df_roll['time'] == rolling_time].sort_values(by=['expiry_date']).reset_index(drop=True)
 
                             roll_diff_dict[expiry_date] = {}
 
 
-                            if len(df_roll) == 2:
+                            if len(df_roll) == 2: # Got date on exact rolling date and both current and next month present
                                 roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
                                 roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
                                 roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
                                 roll_diff_dict[expiry_date]['rolling_time'] = rolling_time
 
-                            else:
-                                # Cannot find rolling time, assume roll at RTH last trade
+                            else: # length of df_roll is zero
                                 df_roll = df[(df['date'] == exact_rolling_date) & (df['RTH'] == True)].copy()
+                                # last_row = 0
+                                # if not (len(df_roll) == 1): ## something only 1 row, investigate laster
+                                #     # Cannot find rolling time, assume roll at RTH last trade
+                                #     df_roll = df[(df['date'] == exact_rolling_date) & (df['RTH'] == True)].copy()
+                                #     last_row = 1
+
                                 df_roll = df_roll.sort_values(by=['time', 'expiry_date']).reset_index(drop=True)
                                 df_roll = df_roll.tail(2).sort_values(by=['expiry_date']).reset_index(drop=True)
+                                # print(df_roll)
                                 roll_diff = df_roll.at[0, 'close'] - df_roll.at[1, 'close']
                                 roll_diff_dict[expiry_date]['rolling_day'] = exact_rolling_date
                                 roll_diff_dict[expiry_date]['roll_diff'] = roll_diff
                                 roll_diff_dict[expiry_date]['rolling_time'] = df_roll.at[0, 'time']
 
-                        except:
+                        except Exception as e:
+                            roll_diff_dict = {}
                             pass
 
 
                     df = df.reset_index(drop=True)
                     df['roll_diff'] = 0
 
-
                     for expiry_date in roll_diff_dict.keys():
+                        print('Hi')
                         d = roll_diff_dict[expiry_date]['rolling_day']
                         t = roll_diff_dict[expiry_date]['rolling_time']
                         diff = roll_diff_dict[expiry_date]['roll_diff']
 
                         condition = (df['date'] == d) & (df['time'] == t) & (df['current_month'] == False)
                         indices = df[condition].index[0]
                         df.at[indices, 'roll_diff'] = diff
@@ -494,14 +509,15 @@
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
 
+    # # Old fut
     # def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
     #
     #     check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
     #
     #     if False not in list(check_bool_dict.values()):
     #
     #         if freq == '1D':
@@ -747,14 +763,15 @@
     #     else:
     #         err_msg = 'Error in: '
     #         for error in check_bool_dict:
     #             if check_bool_dict[error] == False:
     #                 err_msg += error + ','
     #         print(err_msg)
 
+
     def get_hk_market_cap_hist_by_date(self, start_date, end_date):
 
         check_bool_dict = self.check_start_end_date(start_date, end_date)
 
         if False not in list(check_bool_dict.values()):
             link_url = 'http://www.hkfdb.net/data_api?'
             token_str = 'token=' + str(self.authToken)
```

### Comparing `hkfdb-3.7.2/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.7.3/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.2
+Version: 3.7.3
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.2/setup.py` & `hkfdb-3.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.7.2",
+    version="3.7.3",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

