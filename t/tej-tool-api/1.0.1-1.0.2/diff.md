# Comparing `tmp/tej-tool-api-1.0.1.tar.gz` & `tmp/tej-tool-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tej-tool-api-1.0.1.tar", last modified: Wed Jun 28 03:40:59 2023, max compression
+gzip compressed data, was "tej-tool-api-1.0.2.tar", last modified: Mon Jul 10 09:24:30 2023, max compression
```

## Comparing `tej-tool-api-1.0.1.tar` & `tej-tool-api-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 03:40:59.384963 tej-tool-api-1.0.1/
--rw-rw-rw-   0        0        0     5553 2023-06-28 03:40:59.383965 tej-tool-api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5143 2023-06-08 06:00:16.000000 tej-tool-api-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 03:40:59.372905 tej-tool-api-1.0.1/TejTOolAPI/
--rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.1/TejTOolAPI/Error.py
--rw-rw-rw-   0        0        0    15389 2023-06-12 05:47:06.000000 tej-tool-api-1.0.1/TejTOolAPI/Map_Dask_API.py
--rw-rw-rw-   0        0        0    10547 2023-06-12 05:47:06.000000 tej-tool-api-1.0.1/TejTOolAPI/TejToolAPI.py
--rw-rw-rw-   0        0        0     1542 2023-06-12 05:47:06.000000 tej-tool-api-1.0.1/TejTOolAPI/parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-28 03:40:59.365927 tej-tool-api-1.0.1/TejTOolAPI/tables/
--rw-rw-rw-   0        0        0    38911 2023-06-05 09:52:31.000000 tej-tool-api-1.0.1/TejTOolAPI/tables/columns_group.xlsx
--rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.1/TejTOolAPI/tables/mktboard.csv
--rw-rw-rw-   0        0        0       42 2023-06-28 03:40:59.384963 tej-tool-api-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1490 2023-06-28 03:40:19.000000 tej-tool-api-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 03:40:59.380973 tej-tool-api-1.0.1/tej_tool_api.egg-info/
--rw-rw-rw-   0        0        0     5553 2023-06-28 03:40:58.000000 tej-tool-api-1.0.1/tej_tool_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-28 03:40:59.000000 tej-tool-api-1.0.1/tej_tool_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 03:40:58.000000 tej-tool-api-1.0.1/tej_tool_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-28 03:40:58.000000 tej-tool-api-1.0.1/tej_tool_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-28 03:40:58.000000 tej-tool-api-1.0.1/tej_tool_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/
+-rw-rw-rw-   0        0        0     5553 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5143 2023-06-08 06:00:16.000000 tej-tool-api-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.468400 tej-tool-api-1.0.2/TejTOolAPI/
+-rw-rw-rw-   0        0        0      197 2023-05-19 07:13:38.000000 tej-tool-api-1.0.2/TejTOolAPI/Error.py
+-rw-rw-rw-   0        0        0    17148 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/Map_Dask_API.py
+-rw-rw-rw-   0        0        0    11098 2023-07-07 05:58:29.000000 tej-tool-api-1.0.2/TejTOolAPI/TejToolAPI.py
+-rw-rw-rw-   0        0        0      582 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/exchange_calendar.py
+-rw-rw-rw-   0        0        0     1381 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.468400 tej-tool-api-1.0.2/TejTOolAPI/tables/
+-rw-rw-rw-   0        0        0    38860 2023-07-10 09:13:18.000000 tej-tool-api-1.0.2/TejTOolAPI/tables/columns_group.xlsx
+-rw-rw-rw-   0        0        0   137941 2023-05-19 07:13:38.000000 tej-tool-api-1.0.2/TejTOolAPI/tables/mktboard.csv
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2023-07-04 07:26:09.000000 tej-tool-api-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:24:30.484022 tej-tool-api-1.0.2/tej_tool_api.egg-info/
+-rw-rw-rw-   0        0        0     5553 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-10 09:24:30.000000 tej-tool-api-1.0.2/tej_tool_api.egg-info/top_level.txt
```

### Comparing `tej-tool-api-1.0.1/PKG-INFO` & `tej-tool-api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

### Comparing `tej-tool-api-1.0.1/README.md` & `tej-tool-api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.1/TejTOolAPI/Map_Dask_API.py` & `tej-tool-api-1.0.2/TejTOolAPI/Map_Dask_API.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,55 @@
+# import os
+import tejapi
+# tejapi.ApiConfig.ignoretz = True
+# tejapi.ApiConfig.page_limit=10000
+# tejapi.ApiConfig.api_base = os.environ.get('TEJAPI_BASE')
+# tejapi.ApiConfig.api_key = os.environ.get('TEJAPI_KEY')
+
 import pandas as pd
 import datetime
-import tejapi 
-tejapi.ApiConfig.ignoretz = True
 import numpy as np
 import dask.dataframe as dd
-import dask 
-import multiprocessing
+import dask
 import gc
+from . import parameters as para
 
-npartitions_local = multiprocessing.cpu_count()
-
-default_start = '2013-01-01'
-default_end = datetime.datetime.now().date().strftime('%Y-%m-%d')
 
 def get_fin_data(table, tickers, columns=[], **kwargs):
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
     fin_type = kwargs.get('fin_type', ['A', 'Q', 'TTM'])
     # transfer_to_chinese = False
-    npartitions = kwargs.get('npartitions', npartitions_local)
+    npartitions = kwargs.get('npartitions', para.npartitions_local)
     
     # 將需要的 column 選出
     columns += ['coid', 'mdate', 'annd', 'no', 'key3']
     columns = list(set(columns))
 
     # get all data
     def get_data(table, tickers, columns, start, end, fin_type):
         data_sets = tejapi.get(table,
                         coid=tickers,
+                        key3 = fin_type,
                         paginate=True,
                         chinese_column_name=False,
                         mdate={'gte': start, 'lte': end},
-                        opts={'columns': columns, 'sort':{'coid.desc', 'mdate.asc', 'annd.asc', 'no.asc'}})
+                        opts={'columns': columns, 'sort':{'coid.asc', 'mdate.asc', 'annd.asc', 'no.asc'}})
         
         # 
         if len(data_sets) < 1:
             return pd.DataFrame({'coid': pd.Series(dtype='object'),
                                   'mdate': pd.Series(dtype='datetime64[ns]'),
                                   'key3': pd.Series(dtype='object'),
                                   'no': pd.Series(dtype='object'),
                                   'annd':pd.Series(dtype='datetime64[ns]')
                                     })
 
         # select certain fin_type
-        data_sets = get_certain_fin_type(data_sets, fin_type)
+        # data_sets = get_certain_fin_type(data_sets, fin_type)
 
         # parallel fin_type to columns 
         data_sets = fin_pivot(data_sets, remain_keys=['coid', 'mdate', 'no', 'annd'])
 
         return data_sets
     
     # Define the meta of the dataframe
@@ -76,29 +78,29 @@
     data = data.drop_duplicates(subset = subset, keep = keep_mothod)
 
     return data
 
 
 def get_trading_data(table, tickers, columns = [], **kwargs):
     # Setting default value of the corresponding parameters
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
-    npartitions = kwargs.get('npartitions',  npartitions_local)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
+    npartitions = kwargs.get('npartitions',  para.npartitions_local)
 
     # 自動補上 coid, mdate
     columns += ['coid', 'mdate']
     columns = list(set(columns))
 
     def get_data(table, tickers, columns, start, end):
         data = tejapi.get(table,
                         coid = tickers,
                         paginate = True,
                         chinese_column_name=False,
                         mdate = {'gte':start,'lte':end},
-                        opts = {'columns':columns, 'sort':{'coid.desc', 'mdate.asc'}})
+                        opts = {'columns':columns, 'sort':{'coid.asc', 'mdate.asc'}})
         return data
     
     # Define the meta of the dataframe
     meta = get_data(table = table, tickers = '2330', columns=columns, start = start, end =end)
 
     # Calculate the number of tickers in each partition.
     ticker_partitions = get_partition_group(tickers=tickers, npartitions=npartitions)
@@ -111,162 +113,202 @@
         data_sets = data_sets.repartition(npartitions=npartitions)
 
     data_sets = data_sets.drop_duplicates(subset=['coid', 'mdate'], keep = 'last')
 
     return data_sets
 
 def get_alternative_data(table, tickers=[], columns = [], **kwargs):
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
     # transfer_to_chinese = False
-    npartitions = kwargs.get('npartitions', npartitions_local)
+    npartitions = kwargs.get('npartitions', para.npartitions_local)
 
     # 自動補上 coid, mdate, 發布日
     if table == 'TWN/APISALE':
         # 月營收
+        annd = 'annd_s'
         columns += ['coid', 'mdate','annd_s']
         columns = list(set(columns))
     else:
         # 集保資料 
+        annd = 'edate1'
         columns += ['coid','mdate','edate1']
         columns = list(set(columns))
     # 營業日
-    days = generate_multicalendars(tickers, start = start, end = end)
+    # days = generate_multicalendars(tickers, start = start, end = end)
+    days = para.exc.calendar
+    days = days.rename(columns = {'zdate':'all_dates'})
 
     # alternative data
     data_sets = tejapi.get(table,
                     coid = tickers,
                     paginate = True,
                     chinese_column_name=False,
                     mdate = {'gte':start,'lte':end},
-                    opts = {'columns':columns, 'sort':{'coid.desc', 'mdate.desc'}})
+                    opts = {'columns':columns, 'sort':{'coid.asc', 'mdate.asc'}})
+    # 創建一個向量化的函數
+    vectorized_annd_adjusted = np.vectorize(annd_adjusted)
+
+    # 所有不同的發布日
+    uni_dates = pd.to_datetime(data_sets[annd].unique())
+
+    # 傳入 ExchangeCalendar 物件
+    result = vectorized_annd_adjusted(para.exc, uni_dates)
+
+    # Create a mapping dictionary
+    dict_map = {uni_dates[i]:result[i] for i in range(len(result))}
+
+    # Adjust non-trading announce date to next trading date.
+    data_sets[annd] = data_sets[annd].map(dict_map)
+    
     data_sets = data_sets.drop(columns=['mdate'])
 
     if table == 'TWN/APISALE':
-        data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates', 'coid'], right_on=['annd_s', 'coid'])
+        # data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates', 'coid'], right_on=['annd_s', 'coid'])
+        data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates'], right_on=['annd_s'])
     else:
-        data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates', 'coid'], right_on=['edate1', 'coid'])
-    
+        # data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates', 'coid'], right_on=['edate1', 'coid'])
+        data_sets = dd.merge(days, data_sets, how='left', left_on = ['all_dates'], right_on=['edate1'])
+
     del days
     gc.collect()
 
-    data_sets = data_sets.groupby('coid', group_keys = False).apply(fillna_multicolumns, meta = data_sets)
+    data_sets = data_sets.groupby('coid', group_keys = False).apply(fillna_multicolumns)
 
     return data_sets
 
 
 def get_fin_auditor(table, tickers, columns=[], **kwargs):
     # Setting defualt value of the parameters
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
     fin_type = kwargs.get('fin_type', ['A', 'Q', 'TTM'])
     # transfer_to_chinese = False
-    npartitions = kwargs.get('npartitions', npartitions_local)
+    npartitions = kwargs.get('npartitions', para.npartitions_local)
 
     # 自動補上 coid, mdate
     columns += ['coid', 'mdate','key3','no','annd']
     columns = list(set(columns))
 
     # get fin data
     def _get_data(table, tickers, columns, start, end, fin_type):
+        # try:
+        columns.remove('annd')
         data_sets = tejapi.get(table,
                             coid = tickers,
+                            key3 = fin_type, 
                             paginate = True,
                             chinese_column_name=False,
                             mdate = {'gte':start,'lte':end},
-                            opts= {'pivot':True, 'sort':{'coid.desc', 'mdate.asc', 'key3.asc', 'no.asc'}})
+                            opts= {'columns':columns, 'sort':{'coid.asc', 'mdate.asc', 'key3.asc', 'no.asc'}, 'pivot':True})
         
+        columns.append('annd')
+
         if len(data_sets) < 1:
             return pd.DataFrame({'coid': pd.Series(dtype='object'),
-                                  'mdate': pd.Series(dtype='datetime64[ns]'),
-                                  'key3': pd.Series(dtype='object'),
-                                  'no': pd.Series(dtype='object')
+                                'mdate': pd.Series(dtype='datetime64[ns]'),
+                                'key3': pd.Series(dtype='object'),
+                                'no': pd.Series(dtype='object')
                                     })
         
         # modify the name of the columns from upper case to lower case.
         lower_columns = {i:i.lower() for i in data_sets.columns}
         data_sets = data_sets.rename(columns=lower_columns)
 
-        # select certain fin_type
-        data_sets = get_certain_fin_type(data_sets, fin_type)
-
         # get most recent announce date of the company
-        fin_date = get_announce_date(tickers, start = start, end = end)
-        fin_date = get_certain_fin_type(fin_date, fin_type)
-        data_sets = fin_date.merge(data_sets, how = 'left', on = ['coid', 'mdate', 'key3','no'])
+        fin_date = get_announce_date(tickers, start = start, end = end, fin_type = fin_type)
+        data_sets = fin_date.merge(data_sets, how = 'left', on = ['coid', 'mdate', 'key3', 'no'])
+
         del fin_date
         gc.collect()
         
-        # select columns
+        # Select columns
         try:
             data_sets = data_sets.loc[:,columns]
         
         except:
-             # Check selected columns exist in the columns of dataframe
-            selected_columns = []
-            for i in columns:
-                if i in data_sets.columns:
-                    selected_columns.append(i)
+            # Check selected columns exist in the columns of dataframe
+            selected_columns = [i for i in columns if i in data_sets.columns]
             
-            # Drop duplicates
+            # Ensure `data_sets` does not have duplicate rows.
             selected_columns = list(set(selected_columns))
             
             # Select columns again
             data_sets = data_sets.loc[:,selected_columns]
 
-        # parallel fin_type to columns 
+        # Parallel fin_type (key3) to columns 
         data_sets = fin_pivot(data_sets, remain_keys=['coid','mdate','no','annd'])
         
         # Cut off the duplicate rows
-        data_sets = data_sets.sort_values(['coid','mdate', 'annd'])
-        data_sets = data_sets.drop_duplicates(subset=['coid', 'annd'], keep = 'last')
+        # data_sets = data_sets.sort_values(['coid','mdate', 'annd'])
+        # data_sets = data_sets.drop_duplicates(subset=['coid','annd'], keep = 'last')
         
         return data_sets
+        
+        # except: 
+        #     print(tickers, columns)
     
     # Define the meta of the dataframe
     meta = _get_data(table = table, tickers = '2330', columns = columns, start = start, end =end, fin_type= fin_type)
 
     # 
     ticker_partitions = get_partition_group(tickers=tickers, npartitions=npartitions)
     
     # Submit jobs to the parallel cores
     data_sets = dd.from_delayed([dask.delayed(_get_data)(table=table, tickers = tickers[(i-1)*npartitions:i*npartitions]+['2330'], columns = columns, start = start, end = end, fin_type = fin_type) for i in range(1, ticker_partitions)], meta = meta)
     
     # If ticker smaller than defaulted partitions, then transform it into defaulted partitions
     if data_sets.npartitions < npartitions:
         data_sets = data_sets.repartition(npartitions=npartitions)
 
-    data_sets = data_sets.drop_duplicates(subset=['coid', 'annd'], keep = 'last')
+    data_sets = data_sets.drop_duplicates(subset=['coid','annd'], keep = 'last')
 
     return data_sets
 
 
 def get_announce_date(tickers, **kwargs):
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
+    fin_type = kwargs.get('fin_type', ['A', 'Q', 'TTM'])
+
     data = tejapi.get('TWN/AINVFINQA',
                     coid = tickers,
                     paginate = True,
+                    key3 = fin_type,
                     chinese_column_name=False, 
                     mdate = {'gte':start, 'lte':end},
-                    opts = {'sort':{'coid.asc', 'mdate.asc', 'annd.asc'}})
-    
-    return data
+                    opts = {'sort':{'coid.asc', 'mdate.asc', 'key3.asc', 'no.asc','annd.asc'}})
 
-def get_certain_fin_type(data, fin_type):
-    if type(fin_type) is str:
-        # data = data.query(f'key3 == "{fin_type}"')
-        data = data.loc[data['key3']==fin_type,:]
+    # 創建一個向量化的函數
+    vectorized_annd_adjusted = np.vectorize(annd_adjusted)
+
+    # 所有不同的發布日
+    uni_dates = pd.to_datetime(data['annd'].unique())
+
+    # 傳入 ExchangeCalendar 物件
+    result = vectorized_annd_adjusted(para.exc, uni_dates)
+
+    # Create a mapping dictionary
+    dict_map = {uni_dates[i]:result[i] for i in range(len(result))}
+
+    # Adjust non-trading announce date to next trading date.
+    data['annd'] = data['annd'].map(dict_map)
+
+    # Keep the last row when there are multiple rows with the same keys
+    # The last row represents the data with the greatest mdate
+    data = data.drop_duplicates(subset=['coid', 'key3','annd'], keep='last')
 
-    else:
-        # data = data.query(f'key3.isin({fin_type})')
-        data = data.loc[data['key3'].isin(fin_type),:]
-    
     return data
 
+def annd_adjusted(ExchangeCalendar, date):
+        if ExchangeCalendar.is_session(date):
+            return date
+        
+        return ExchangeCalendar.next_open(date)
+
 def fin_pivot(df, remain_keys):
     # for loop execute pviot function
     uni = df['key3'].dropna().unique()
     data = pivot(df, remain_keys, uni[0])
 
     for i in range(1, len(uni)):
         temp = pivot(df, remain_keys, uni[i])
@@ -289,17 +331,17 @@
         raise ValueError('請使用 get_announce_date 檢查該檔股票的財務數據發布日是否為空值。')
     
     return data
 
 
 def generate_multicalendars(tickers, **kwargs):
     # Setting defualt value of the parameters
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
-    npartitions = kwargs.get('npartitions', npartitions_local)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
+    npartitions = kwargs.get('npartitions', para.npartitions_local)
 
     def get_daily_calendar(tickers:list):
         def get_data(ticker):
             cal = pd.date_range(start=start, end=end, freq='D')
             coid = [str(ticker)]*len(cal)
             return pd.DataFrame({'coid':coid, 'all_dates': cal})
         
@@ -322,24 +364,24 @@
     # Calculate the number of tickers in each partition. 
     ticker_partitions = get_partition_group(tickers=tickers, npartitions=npartitions)
     
     # Submit jobs to the parallel cores
     fin_calendar = dd.from_delayed([dask.delayed(get_daily_calendar)(tickers[(i-1)*npartitions:i*npartitions]) for i in range(1, ticker_partitions)], meta = meta)
     
     # If ticker smaller than defaulted partitions, then transform it into defaulted partitions
-    if fin_calendar.npartitions < npartitions_local:
+    if fin_calendar.npartitions < para.npartitions_local:
         fin_calendar = fin_calendar.repartition(npartitions=npartitions)
 
     return fin_calendar
 
 def generate_multicalendars_dask(tickers, **kwargs):
     # Setting defualt value of the parameters
-    start = kwargs.get('start', default_start)
-    end = kwargs.get('end', default_end)
-    npartitions = kwargs.get('npartitions', npartitions_local)
+    start = kwargs.get('start', para.default_start)
+    end = kwargs.get('end', para.default_end)
+    npartitions = kwargs.get('npartitions', para.npartitions_local)
 
 
     def get_daily_calendar(tickers:list):
         def get_data(ticker):
             cal = pd.date_range(start=start, end=end, freq='D')
             coid = [str(ticker)]*len(cal)
             return pd.DataFrame({'coid':coid, 'all_dates': cal})
@@ -373,8 +415,11 @@
     return fin_calendar
 
 
 def fillna_multicolumns(df):
     return df.fillna(method = 'ffill')
 
 def get_partition_group(tickers:list, npartitions):
-    return (len(tickers)//npartitions) + 1 if len(tickers)%npartitions ==0 else (len(tickers)//npartitions) + 2
+    return (len(tickers)//npartitions) + 1 if len(tickers)%npartitions ==0 else (len(tickers)//npartitions) + 2
+
+
+
```

### Comparing `tej-tool-api-1.0.1/TejTOolAPI/TejToolAPI.py` & `tej-tool-api-1.0.2/TejTOolAPI/TejToolAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,89 @@
-import tejapi 
-tejapi.ApiConfig.ignoretz = True
-tejapi.ApiConfig.page_limit=10000
+import tejapi
+# tejapi.ApiConfig.ignoretz = True
+# tejapi.ApiConfig.page_limit=10000
 import dask.dataframe as dd
 import pandas as pd
 import gc
 from . import parameters as para
+from . import Map_Dask_API as dask_api
 import dask
-import dask.dataframe as dd
 
 
+# 映射函數 (dask_version)
+funct_map = {
+    'A0001':dask_api.get_trading_data,
+    'A0002':dask_api.get_fin_data,
+    'A0003':dask_api.get_alternative_data,
+    'A0004':dask_api.get_fin_auditor
+}
 
-def get_history_data(tickers:list, columns:list = [], fin_type:list = ['A','Q','TTM'], include_self_acc:str = 'N', **kwargs):
+def get_history_data(ticker:list, columns:list = [], fin_type:list = ['A','Q','TTM'], include_self_acc:str = 'N', **kwargs):
     # Setting default value of the corresponding parameters
     start = kwargs.get('start', para.default_start)
     end = kwargs.get('end', para.default_end)
     transfer_to_chinese = kwargs.get('transfer_to_chinese', False)
     npartitions = kwargs.get('npartitions',  para.npartitions_local)
-    all_tables = triggers(ticker = tickers, columns= columns, start= start, end= end, fin_type= fin_type, include_self_acc= include_self_acc, npartitions = npartitions)
+    all_tables = triggers(ticker = ticker, columns= columns, start= start, end= end, fin_type= fin_type, include_self_acc= include_self_acc, npartitions = npartitions)
 
     def process_fin_data(all_tables, variable, tickers, start, end):
         # transfer to daily basis
-        days = para.dask_mpf.generate_multicalendars(tickers, start = start, end = end)
-        all_tables[variable] = dd.merge(days, all_tables[variable], left_on=['coid','all_dates'], right_on=['coid', 'annd'], how='left')
+        # days = para.dask_mpf.generate_multicalendars(tickers, start = start, end = end)
+        # all_tables[variable] = dd.merge(days, all_tables[variable], left_on=['coid','all_dates'], right_on=['coid', 'annd'], how='left')
+
+        days = para.exc.calendar
+        days = days.rename(columns = {'zdate':'all_dates'})
+        all_tables[variable] = dd.merge(days, all_tables[variable], left_on=['all_dates'], right_on=['annd'], how='left')
         
         # Drop mdate column
         all_tables[variable] = all_tables[variable].drop(columns = 'mdate')
 
         # Delete the redundant dataframe to release memory space
         del days
         gc.collect()
 
         # Filling NaN with the precending value
-        all_tables[variable] = all_tables[variable].groupby('coid', group_keys = False).apply(para.dask_mpf.fillna_multicolumns, meta = all_tables[variable])
+        # all_tables[variable] = all_tables[variable].groupby('coid', as_index = False).apply(para.dask_mpf.fillna_multicolumns, meta = all_tables[variable])
         
         return all_tables[variable]
     
        
     # 針對自結損益和財簽資料作處理
     try:
         # Concate fin_self_acc with fin_auditor
         data_concat = dd.concat([all_tables['fin_self_acc'], all_tables['fin_auditor']]).reset_index(drop=True)
         all_tables['fin_auditor'] = data_concat.drop_duplicates(subset=['coid','mdate','annd'], keep='last')
 
         # Process two fin dataframe
-        all_tables['fin_auditor'] = process_fin_data(all_tables=all_tables, variable='fin_auditor', tickers=tickers, start=start, end= end)
+        all_tables['fin_auditor'] = process_fin_data(all_tables=all_tables, variable='fin_auditor', tickers=ticker, start=start, end= end)
         
         del all_tables['fin_self_acc']
         # return all_tables
 
     except:
         if 'fin_auditor' in all_tables.keys():
-            all_tables['fin_auditor'] = process_fin_data(all_tables=all_tables, variable='fin_auditor', tickers=tickers, start=start, end= end)
+            all_tables['fin_auditor'] = process_fin_data(all_tables=all_tables, variable='fin_auditor', tickers=ticker, start=start, end= end)
 
         elif 'fin_self_acc' in all_tables.keys():
-            all_tables['fin_self_acc'] = process_fin_data(all_tables=all_tables, variable='fin_self_acc', tickers=tickers, start=start, end= end)
+            all_tables['fin_self_acc'] = process_fin_data(all_tables=all_tables, variable='fin_self_acc', tickers=ticker, start=start, end= end)
         
         else:
             pass
 
     # 搜尋觸發到那些 table
     trigger_tables = [i for i in all_tables.keys() if i in para.fin_invest_tables['TABLE_NAMES'].unique().tolist()]
 
     # 根據 OD 進行排序
     trigger_tables.sort(key = lambda x: para.map_table.loc[para.map_table['TABLE_NAMES']==x, 'OD'].item())
 
     # tables 兩兩合併
     history_data = consecutive_merge(all_tables,  trigger_tables)
     history_data = history_data.drop(columns=[i for i in history_data.columns if i in para.drop_keys])
     history_data = history_data.drop_duplicates(subset=['coid', 'mdate'], keep='last').repartition(npartitions=npartitions)
+    history_data = history_data.groupby('coid', group_keys = False).apply(dask_api.fillna_multicolumns, meta = history_data)
 
     if transfer_to_chinese is False:
         # transfer to Chinese version
         lang_map = transfer_language_columns(history_data.columns, isEnglish=True)
         history_data = history_data.rename(columns= lang_map)
 
     elif transfer_to_chinese is True:
@@ -160,18 +172,18 @@
     for table_name in trigger_tables['TABLE_NAMES'].unique():
         # print(table_name)
         selected_columns = trigger_tables.loc[trigger_tables['TABLE_NAMES']==table_name, 'COLUMNS'].tolist()
         api_code = para.table_API.loc[para.table_API['TABLE_NAMES']==table_name, 'API_CODE'].item()
         api_table = para.fin_invest_tables.loc[para.fin_invest_tables['TABLE_NAMES']==table_name,'API_TABLE'].item()
 
         if api_code == 'A0002' or api_code == 'A0004':
-            exec(f'{table_name} = para.funct_map[api_code](api_table, ticker, selected_columns, start = start,  end = end, fin_type = fin_type, npartitions = npartitions)')
+            exec(f'{table_name} = funct_map[api_code](api_table, ticker, selected_columns, start = start,  end = end, fin_type = fin_type, npartitions = npartitions)')
         
         else:
-            exec(f'{table_name} = para.funct_map[api_code](api_table, ticker, selected_columns, start = start,  end = end, npartitions = npartitions)')
+            exec(f'{table_name} = funct_map[api_code](api_table, ticker, selected_columns, start = start,  end = end, npartitions = npartitions)')
 
     return locals()
 
 def get_internal_code(fields:list):
     columns = []
     for c in ['ENG_COLUMN_NAMES', 'CHN_COLUMN_NAMES', 'COLUMNS']:
         temp = para.transfer_language_table.loc[para.transfer_language_table[c].isin(fields), 'COLUMNS'].tolist()
@@ -223,15 +235,15 @@
         else:
             return pd.DataFrame({'coid': pd.Series(dtype='object'), 'mdate': pd.Series(dtype='datetime64[ns]')})
     
     # Define the meta of the dataframe
     meta = pd.DataFrame({'coid': pd.Series(dtype='object'), 'mdate': pd.Series(dtype='datetime64[ns]')})
 
     # Calculate the number of tickers in each partition. 
-    ticker_partitions = para.dask_mpf.get_partition_group(tickers = tickers, npartitions= npartitions)
+    ticker_partitions = dask_api.get_partition_group(tickers = tickers, npartitions= npartitions)
 
     # Submit jobs to the parallel cores
     trading_calendar = dd.from_delayed([dask.delayed(get_data)(tickers[(i-1)*npartitions:i*npartitions]) for i in range(1, ticker_partitions)], meta = meta)
 
     # If ticker smaller than defaulted partitions, then transform it into defaulted partitions
     if trading_calendar.npartitions < 12:
         trading_calendar = trading_calendar.repartition(npartitions=npartitions)
```

### Comparing `tej-tool-api-1.0.1/TejTOolAPI/tables/columns_group.xlsx` & `tej-tool-api-1.0.2/TejTOolAPI/tables/columns_group.xlsx`

 * *Files 23% similar despite different names*

```diff
@@ -105,80 +105,80 @@
 00000680: a0ea 93cf 9b7f d796 a6e9 0d3f 8839 4cec  ...........?.9L.
 00000690: d299 15c8 7362 67d9 ae7c c86c 21f5 f91a  ....sbg..|.l!...
 000006a0: 5553 6839 69b0 629e 723a 2279 5f64 6cc0  USh9i.b.r:"y_dl.
 000006b0: f344 9bbf 13fd 7c2d 4e9c c852 2234 12f8  .D....|-N..R"4..
 000006c0: 32cf 47c7 25a0 f57f 5ab4 34f1 cb9d 79c4  2.G.%...Z.4...y.
 000006d0: 3709 c3ab c8f0 c982 8b1f a8de 0100 00ff  7...............
 000006e0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000006f0: 0088 e8eb 39b1 0300 00f5 0800 000f 0000  ....9...........
+000006f0: 0054 bbc2 17b6 0300 00f1 0800 000f 0000  .T..............
 00000700: 0078 6c2f 776f 726b 626f 6f6b 2e78 6d6c  .xl/workbook.xml
-00000710: ac56 518f e236 107e afd4 ff90 46fb 9a4d  .VQ..6.~....F..M
-00000720: 6c42 6023 e004 1b56 45da 56e8 8ebb 932a  lB`#...VE.V....*
-00000730: a4c8 2486 b824 76ce 7680 d5e9 fe7b c709  ..$..$v.v....{..
-00000740: b001 fab0 dd6b 0476 9cb1 3f7f 33f3 7992  .....k.v..?.3.y.
-00000750: c187 4391 5b3b 2a15 137c 68a3 7bcf b628  ..C.[;*..|h.{..(
-00000760: 4f44 caf8 6668 7f5e 3c39 7ddb 529a f094  OD..fh.^<9}.R...
-00000770: e482 d3a1 fd42 95fd 61f4 eb2f 83bd 90db  .....B..a../....
-00000780: 9510 5b0b 00b8 1ada 99d6 65e8 ba2a c968  ..[.......e..*.h
-00000790: 41d4 bd28 2907 cb5a c882 6818 ca8d ab4a  A..()..Z..h....J
-000007a0: 4949 aa32 4a75 91bb d8f3 02b7 208c db0d  II.2Ju...... ...
-000007b0: 4228 df82 21d6 6b96 d048 2455 41b9 6e40  B(..!.k..H$UA.n@
-000007c0: 24cd 8906 fa2a 63a5 3aa1 15c9 5be0 0a22  $....*c.:...[.."
-000007d0: b755 e924 a228 0162 c572 a65f 6a50 db2a  .U.$.(.b.r._jP.*
-000007e0: 9270 b6e1 4292 550e 6e1f 50d7 3a48 f805  .p..B.U.n.P.:H..
-000007f0: f047 1e34 f8b4 1398 6eb6 2a58 2285 126b  .G.4....n.*X"..k
-00000800: 7d0f d06e 43fa c67f e4b9 085d 84e0 701b  }..nC......]..p.
-00000810: 83b7 21f9 aea4 3b66 7278 6625 8377 b20a  ..!...;frxf%.w..
-00000820: ce58 c12b 18f2 7e1a 0d81 b46a ad84 10bc  .X.+..~....j....
-00000830: 77a2 75cf dcb0 3d1a ac59 4ebf 34d2 b548  w.u...=..YN.4..H
-00000840: 59fe 490a 93a9 dcb6 72a2 f434 659a a643  Y.I.....r..4e..C
-00000850: bb07 43b1 a717 0f64 554e 2a96 8315 071d  ..C....dUN*.....
-00000860: dcb3 ddd1 59ce 7309 03c8 fd38 d754 72a2  ....Y.s....8.Tr.
-00000870: e9a3 e01a a476 a4fe b3b2 aab1 1f33 0122  .....v.......3."
-00000880: b63e d26f 1593 14ce 0e48 08dc 8196 2421  .>.o.....H....$!
-00000890: 59a9 39d1 9955 c97c 683f 86cb cf0a 3c5c  Y.9..U.|h?....<\
-000008a0: 620f 630f a19e 8797 1155 5b2d cae5 3315  b.c......U[-..3.
-000008b0: cbbf 5899 334e 4f7d acbf 5584 ebe5 82fe  ..X.3NO}..U.....
-000008c0: bd10 221f cf67 4b6d f4ab 962d b192 db93  .."..gKm...-....
-000008d0: f11f e44a 1213 2d17 22d4 78d1 dc5f 470b  ...J..-.".x.._G.
-000008e0: 9c91 e149 9273 2d2d b89f 45cf 9096 4f64  ...I.s--..E...Od
-000008f0: 0749 0229 a4c7 333c 832c a04e cc13 19a2  .I.)..3<.,.N....
-00000900: f8fb c443 d3fe 741c 3963 8cfb 8edf 89e0  ...C..t.9c......
-00000910: 6e82 b133 9df8 4f5e f701 05a8 d3ff 01ce  n..3..O^........
-00000920: c820 4c04 a974 76cc bf81 1eda 3e24 fbc6  . L..tv.....>$..
-00000930: f407 399c 2cc8 0b2b 96be d2f8 ee1d 2fc7  ..9.,..+....../.
-00000940: f457 cdc9 f6c3 386c 2add 1746 f7ea 5529  .W....8l*..F..U)
-00000950: 6668 1dbe 329e 8afd d076 1006 a75e 2e87  fh..2....v...^..
-00000960: fbda f895 a53a 03a9 3d78 3e4c 699e fd4e  .....:..=x>Li..N
-00000970: d926 03c6 a8db 370f 49a2 d98e 2ec8 0a9e  .&....7.I.......
-00000980: 1817 b0e1 39b4 2ff8 450d bf27 b81c d35c  ....9./.E..'...\
-00000990: f073 5b04 eb0a 0b44 ebde e2f5 a9a8 6510  .s[....D......e.
-000009a0: 2722 af0a 0e35 b236 d591 b72d 199a ade4  '"...5.6...-....
-000009b0: 2c45 c6d1 8b45 9270 b5a6 32ce 09df 5464  ,E...E.p..2...Td
-000009c0: 435b 0b21 d2e7 85f8 7a21 08af 3515 2ae5  C[.!....z!..5.*.
-000009d0: 796a e77a ea9a f198 f11d 9ccf b891 6a6b  yj.z..........jk
-000009e0: 21d4 9ff3 42ff 869c 1176 2cd2 d6fc 4e6b  !...B....v,...Nk
-000009f0: 7ef7 7a7e 41e5 86c6 5bfa d276 df6f ad08  ~.z~A...[..v.o..
-00000a00: 6a61 9f82 9752 6046 5353 5320 94ad d131  ja...R`FSSS ...1
-00000a10: a0f1 21e7 c57d fcc4 4c9d 8808 7027 0ae2  ..!..}..L...p'..
-00000a20: 938b 84e4 9fcc 2bce 4417 329b b134 a5e6  ......+.D.2..4..
-00000a30: cd6a 8f2e 72f0 dbdd f80e 8577 93bb 4e10  .j..r......w..N.
-00000a40: 0cdc 16fe bb37 03e1 b437 bbce dd71 c3e8  .....7...7...q..
-00000a50: 5f36 6c6f 0fce 8207 c95c 5aa6 ab25 d2c5  _6lo.....\Z..%..
-00000a60: 5d54 6b83 1ef4 b3d2 a301 f450 9e18 e813  ]Tk........P....
-00000a70: f9de b8e7 3df8 8e37 ed74 1dbf ff80 9dbe  ....=..7.t......
-00000a80: dfc1 cea3 1fe1 69b7 378d a693 ae39 aee6  ......i.7....9..
-00000a90: 1321 fc3f 5e94 7595 0c4f df1e 8665 46a4  .!.?^.u..O...eF.
-00000aa0: 5e48 926c e18b e523 5d4f 200d 26da a648  ^H.l...#]O .&..H
-00000ab0: 01cf a6ad 59bb a755 a37f 0000 00ff ff03  ....Y..U........
-00000ac0: 0050 4b03 0414 0006 0008 0000 0021 000e  .PK..........!..
-00000ad0: 1564 c916 0100 007b 0500 001a 0008 0178  .d.....{.......x
-00000ae0: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
-00000af0: 2e78 6d6c 2e72 656c 7320 a204 0128 a000  .xml.rels ...(..
-00000b00: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000710: ac56 5d8f 9b38 147d 5f69 ff03 8bf2 ca80  .V]..8.}_i......
+00000720: 2140 8292 54f9 1a6d a4e9 2a6a a7ed 0b12  !@..T..m..*j....
+00000730: 72c0 096e c066 6d93 64b6 ea7f df6b f231  r..n.fm.d....k.1
+00000740: 2479 999d 2e4a 6c8c ede3 73ef 3df7 c2e0  $y...Jl...s.=...
+00000750: c3a1 2c8c 1d11 9272 3634 d183 631a 84a5  ..,....r64..c...
+00000760: 3ca3 6c33 34bf 3c3f 5a3d d390 0ab3 0c17  <.l34.<?Z=......
+00000770: 9c91 a1f9 42a4 f961 f4fb 6f83 3d17 db15  ....B..a..o.=...
+00000780: e75b 0300 981c 9ab9 5255 64db 32cd 4989  .[......RUd.2.I.
+00000790: e503 af08 8399 3517 2556 3014 1b5b 5682  ......5.%V0..[V.
+000007a0: e04c e684 a8b2 b05d c709 ec12 5366 1e11  .L.....]....Sf..
+000007b0: 22f1 160c be5e d394 cc78 5a97 84a9 2388  "....^...xZ...#.
+000007c0: 2005 5640 5fe6 b492 67b4 327d 0b5c 89c5   .V@_...g.2}.\..
+000007d0: b6ae ac94 9715 40ac 6841 d54b 036a 1a65  ......@.hA.K.j.e
+000007e0: 1a2d 368c 0bbc 2ac0 ec03 f28d 8380 5f00  .-6...*......._.
+000007f0: 7fe4 40e3 9e4f 82a9 bba3 4a9a 0a2e f95a  ..@..O....J....Z
+00000800: 3d00 b47d 247d 673f 726c 84ae 5c70 b8f7  =..}$}g?rl..\p..
+00000810: c1db 90ba b620 3baa 6378 6125 8277 b20a  ..... ;.cxa%.w..
+00000820: 2e58 c12b 1872 7e19 0d81 b41a ad44 e0bc  .X.+.r~......D..
+00000830: 77a2 f917 6eae 391a ac69 41be 1ea5 6be0  w...n.9..iA...k.
+00000840: aafa 0b97 3a52 8569 1458 aa79 4615 c986  ....:R.i.X.yF...
+00000850: 6608 43be 2757 0f44 5d4d 6a5a c0ac 1bf8  f.C.'W.D]MjZ....
+00000860: 6edf b447 1739 2f05 0c20 f6e3 4211 c1b0  n..G.9/.. ..B...
+00000870: 2253 ce14 48ed 44fd 5765 d560 4f73 0e22  "S..H.D.We.`Os."
+00000880: 363e 91bf 6b2a 08e4 0e48 08cc 8116 a711  6>..k*...H......
+00000890: 5ec9 2556 b951 8b62 684e a3f8 8b04 0b63  ^.%V.Q.bhN.....c
+000008a0: d771 5d07 a1d0 71e3 31c3 2987 7cf4 62c2  .q]...q.1.).|.b.
+000008b0: 7632 fe87 5605 65c4 52e4 7bfc 4457 b104  v2..V.e.R.{.DW..
+000008c0: b3ad 0aa7 5bbc 2132 7e26 df9f 392f c6cb  ....[.!2~&..9/..
+000008d0: 45ac b492 65dc 922d becf 91ff 205c 9c6a  E...e..-.... \.j
+000008e0: bfd9 e0ab a33d c7fb 5bbf 8159 223a 8b73  .....=..[..Y":.s
+000008f0: a984 01f7 8bd9 1304 e833 de41 b840 14d9  .........3.A.@..
+00000900: 299b 1710 0fe4 252c 1511 4a7e f4c3 eecc  ).....%,..J~....
+00000910: 0d27 a135 9df6 90d5 1df7 7ad6 241c fb96  .'.5......z.$...
+00000920: e33d f6fb 939e 330e c3c9 4f30 4604 51ca  .=....3...O0F.Q.
+00000930: 71ad f293 1234 f4d0 ec42 d8ef a63e e2c3  q....4...B...>..
+00000940: 7906 3951 4db3 571a 3f9c d365 e9fe a639  y.9QM.W.?..e...9
+00000950: cffd d406 eb9a f795 92bd 7cd5 8c1e 1a87  ..........|.....
+00000960: 6f94 657c 0f92 eafb 3db0 eae5 3c0e f568  o.e|....=...<..h
+00000970: df4c 7ea3 99ca 6105 0a9c cbb3 3f09 dde4  .L~...a.....?...
+00000980: c018 21af e76b d2ae 6636 34af 18cd 8e8c  ..!..k..f64.....
+00000990: 1ee1 b274 73c5 c86e 516a aa2b 506b 7a83  ...ts..nQj.+Pkz.
+000009a0: 3519 d104 3e49 7951 970c ea63 33d5 f8da  5...>IyQ...c3...
+000009b0: 3444 a48f 128b 0c69 d3ae 3609 cce4 9a88  4D.....i..6.....
+000009c0: a4c0 6c53 8396 5a1b c1b7 978d eeed 4690  ..lS..Z.......F.
+000009d0: 5a6b 2954 c9cb 52ef 76e9 9ab2 84b2 1de4  Zk)T..R.v.......
+000009e0: 6672 1467 6b23 d49e cbc6 ee1d 392d e584  fr.gk#......9-..
+000009f0: 67ad f55e 6bbd 7fbb be24 6243 922d 7969  g..^k....$bC.-yi
+00000a00: 9bdf 6ded 081a 299f 9d97 1160 4632 5d4f  ..m...)....`F2]O
+00000a10: c095 add1 c9a1 c9a1 60e5 43f2 4875 8d98  ........`.C.Hu..
+00000a20: 61e0 8e25 f8a7 e029 2e3e ebd7 9bf6 2e04  a..%...).>......
+00000a30: 38a7 5946 f45b d51c 5dc5 e08f ceb8 83a2  8.YF.[..].......
+00000a40: cea4 e3f9 e1c0 6ee1 bffb 3074 7dd8 6dec  ......n...0t}.m.
+00000a50: 4e07 ce3a 5e10 dc1c d83e 1e8c 050b d2a5  N..:^....>......
+00000a60: 3074 d748 c477 7dd4 6883 1cd4 9354 a301  0t.H.w}.h....T..
+00000a70: f450 9a28 e813 7521 079d 7ed7 72e6 9e6f  .P.(..u!..~.r..o
+00000a80: 757b 7dd7 ea75 3dd7 9a42 dece fd70 3e9b  u{}..u=..B...p>.
+00000a90: 4f7c 9da0 faf3 20fa 3f5e 924d 858c cedf  O|.... .?^.M....
+00000aa0: 1d9a 658e 857a 1650 ebe0 6be5 1359 4f20  ..e..z.P..k..YO 
+00000ab0: 0cda dbba 2c01 cf63 dbb0 b6cf bb46 ff02  ....,..c.....F..
+00000ac0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00000ad0: 0000 2100 0e15 64c9 1601 0000 7b05 0000  ..!...d.....{...
+00000ae0: 1a00 0801 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
+00000af0: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 20a2  kbook.xml.rels .
+00000b00: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -186,2247 +186,2244 @@
 00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c00: 00bc 944d 6ac3 3010 85f7 85de 4168 5fcb  ...Mj.0.....Ah_.
-00000c10: 7612 372d 91b3 0985 6c5b f700 c21e ff10  v.7-....l[......
-00000c20: 5b32 9a49 5bdf bec2 a58d 0341 dd18 6f04  [2.I[......A..o.
-00000c30: 3383 defb 3482 b7db 7f75 2dfb 008b 8dd1  3...4....u-.....
-00000c40: 9247 41c8 19e8 dc14 8dae 247f cf5e 1eb6  .GA.......$..^..
-00000c50: 9c21 295d a8d6 6890 7c00 e4fb f4fe 6ef7  .!)]..h.|.....n.
-00000c60: 0aad 2277 09eb a647 e654 344a 5e13 f5cf  .."w...G.T4J^...
-00000c70: 4260 5e43 a730 303d 6837 298d ed14 b9d2  B`^C.00=h7).....
-00000c80: 56a2 57f9 4955 20e2 304c 849d 6af0 f44a  V.W.IU .0L..j..J
-00000c90: 931d 0bc9 edb1 70fe d9d0 3be7 ffb5 4d59  ......p...;...MY
-00000ca0: 3639 1c4c 7eee 40d3 0d0b 8134 b4ee 012c  69.L~.@....4...,
-00000cb0: 53b6 0292 fca7 0e1c 2317 b7ed 5773 da7f  S.......#...Ws..
-00000cc0: 1a7b c21a 802e 047f 2d14 e364 e583 799c  .{......-..d..y.
-00000cd0: 1386 dc1f c105 642c c578 463e 8678 e185  ......d,.xF>.x..
-00000ce0: c43e 9868 6118 ef66 9285 6112 df66 360b  .>.ha..f..a..f6.
-00000cf0: c36c 7c30 eb85 61d6 3e98 a759 03a5 5616  .l|0..a.>..Y..V.
-00000d00: 8a37 b22e 2fa7 b932 6dff c288 abc8 4cbf  .7../..2m.....L.
-00000d10: 0100 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00000d20: 0000 0021 00cf ec59 b839 1500 0057 bc00  ...!...Y.9...W..
-00000d30: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00000d40: 7473 2f73 6865 6574 312e 786d 6c9c 934b  ts/sheet1.xml..K
-00000d50: 8fdb 2010 c7ef 95fa 1d10 f718 dbd9 b81b  .. .............
-00000d60: 2bce aaed 2aea deaa aa8f 33c1 e318 058c  +...*.....3.....
-00000d70: 0b38 0f55 fdee 1d70 1e2b e5d0 682d 9b01  .8.U...p.+..h-..
-00000d80: 46f3 9b19 f367 f174 d08a ecc0 3a69 ba8a  F....g.t....:i..
-00000d90: 6649 4a09 74c2 d4b2 db54 f4c7 f7d5 e491  fIJ.t....T......
-00000da0: 12e7 7957 7365 3aa8 e811 1c7d 5abe 7fb7  ..yWse:....}Z...
-00000db0: d81b bb75 2d80 2748 e85c 455b effb 9231  ...u-.'H.\E[...1
-00000dc0: 275a d0dc 25a6 870e 3d8d b19a 7b5c da0d  'Z..%...=...{\..
-00000dd0: 73bd 055e c720 ad58 9ea6 05d3 5c76 7424  s..^. .X....\vt$
-00000de0: 94f6 1e86 691a 29e0 d988 4143 e747 8805  ....i.)...AC.G..
-00000df0: c53d d6ef 5ad9 bb33 4d8b 7b70 9adb edd0  .=..Z..3M.{p....
-00000e00: 4f84 d13d 22d6 5249 7f8c 504a b428 5f36  O..=".RI..PJ.(_6
-00000e10: 9db1 7cad b0ef 43f6 c005 3958 7c73 fca6  ..|...C...9X|s..
-00000e20: e734 71ff 2693 96c2 1a67 1a9f 2099 8d35  .4q.&....g.. ..5
-00000e30: dfb6 3f67 73c6 c585 74db ff5d 98ec 8159  ..?gs...t..]...Y
-00000e40: d8c9 7080 5754 feb6 92b2 d985 955f 61d3  ..p.WT......._a.
-00000e50: 37c2 8a0b 2cfc 2e5b 0eb2 aee8 9ff4 f44c  7...,..[.......L
-00000e60: d066 6148 afc3 d9f7 972e 17b5 c413 0e5d  .faH...........]
-00000e70: 110b 4d45 3f66 e5a7 6951 50b6 5c44 05fd  ..ME?f..iQP.\D..
-00000e80: 94b0 77af e624 0872 6dcc 3638 5e30 518a  ..w..$.rm.68^0Q.
-00000e90: 0c07 0a44 9006 e168 76f0 1994 aae8 2a7b  ...D...hv.....*{
-00000ea0: 9ca3 aa7f 476e 5c20 945d a8af e7e7 0cab  ....Gn\ .]......
-00000eb0: 28e3 af96 d4d0 f041 f96f 66ff 05e4 a6f5  (......A.of.....
-00000ec0: 7867 8a64 86ed 057d 94f5 f119 9c40 6162  xg.d...}.....@ab
-00000ed0: fa24 9f85 6285 5108 c191 6819 6e18 0a8b  .$..b.Q...h.n...
-00000ee0: 1fa2 ddcb dab7 15cd b3e4 0302 d6e0 fc4a  ...............J
-00000ef0: 061e 2562 70de e85f a33f 3b51 c678 3c96  ..%bp.._.?;Q.x<.
-00000f00: 188f f614 8ff9 334c f51f 008b 75fc 0300  ......3L....u...
-00000f10: 00ff ff00 0000 ffff 949d edae dc46 9244  .............F.D
-00000f20: 5fc5 d003 acbb aafa 7320 0bd8 815f 44f0  _.......s ..._D.
-00000f30: 0a98 5fb3 8b91 e0d9 7dfb cd5b 6d48 b733  .._.....}..[mH.3
-00000f40: 4e08 8c7f 966f a033 bb48 1e16 c93a cd8f  N....o.3.H...:..
-00000f50: 5fff f1e5 cbb7 df3f 7ffb fce9 e3bf fefb  _......?........
-00000f60: dfbf fceb b70f e3c3 2f5f ffe7 f33f bfd6  ......../_...?..
-00000f70: 7ffd 6d7e f8e5 7fc7 f9f3 1f7f fbaf fffb  ..m~............
-00000f80: fdcb d73f befc f3db 6f1f 4eff 312f 1f3e  ...?....o.N.1/.>
-00000f90: 7dfc e32d fb9f 15ae fff5 b5fe fde7 a7f1  }..-............
-00000fa0: b87e fcf5 cf4f 1f7f fde3 afbf fefd f5af  .~...O..........
-00000fb0: b7ef 7ffd b54a 7daf 5735 8ed7 7b0b ef16  .....J}.W5..{...
-00000fc0: bf57 ed35 3561 eaae a4ee 5bf8 b5ee bd7d  .W.55a....[....}
-00000fd0: 574d 98ba e7a4 ee5b f8b5 eea3 d5d5 84a9  WM.....[........
-00000fe0: 7b49 eabe 855f eb8e 532b ac11 53f8 9a14  {I..._..S+..S...
-00000ff0: 7e0b b7c2 a315 d688 297c 4b0a bf85 5be1  ~.......)|K...[.
-00001000: d90a 6bc4 14be 2785 dfc2 adf0 6a85 3562  ..k...'.....j.5b
-00001010: 0a3f 92c2 6fe1 56f8 dc0a 6bc4 141e a7a4  .?..o.V...k.....
-00001020: f24e b7d2 97ce 8eb7 4f7c cdb8 da19 b1de  .N......O|......
-00001030: d2ad b670 4b33 ae76 44af a170 1a3f 3e78  ...pK3.vD..p.?>x
-00001040: 13f5 ef90 71b5 2382 0d05 d4e8 0c83 8cab  ....q.#.........
-00001050: 1d51 6c28 a446 e718 645c ed88 6443 3935  .Ql(.F..d\..dC95
-00001060: 3bca 20e3 6a47 301b 8aaa d969 0619 573b  ;. .jG0....i..W;
-00001070: e2d9 505a cd0e 34c8 b8da 11d2 8602 6b76  ..PZ..4.......kv
-00001080: a641 c6d5 8ea8 3694 59b3 630d 32a6 f68c  .A....6.Y.c.2...
-00001090: b8b6 d3af 6c99 9d6b 9071 b523 ae4d 65d6  ....l..k.q.#.Me.
-000010a0: 94b9 d161 aecd 6c56 a65c 9b9d 6bfb 130f  ...a..lV.\..k...
-000010b0: f17c 465c dbe9 36e6 9d6b 9071 631e 716d  .|F\..6..k.qc.qm
-000010c0: 2ad7 66e7 1a64 5ced 886b 3509 efe7 b1d5  *.f..d\..k5.....
-000010d0: b906 1957 3be2 da54 aead ce35 c8b8 da11  ...W;..T...5....
-000010e0: d7a6 726d 75ae 41c6 d58e b836 956b 7288  ..rmu.A....6.kr.
-000010f0: 6964 fdc0 cfeb 854f c4b5 a95c 93dd 5c23  id.....O...\..\#
-00001100: aef6 8ab8 b6d3 afc7 d8ea 5ca3 8cf9 e22b  ..........\....+
-00001110: 02db 4eb7 e27d d429 e38a 4764 5b4a b6d5  ..N..}.)..Gd[J..
-00001120: c946 1957 3cbb e8d4 29db 92cb 4ec8 b8e2  .F.W<...)...N...
-00001130: 11db 96b2 6d75 b651 c615 8fe0 b614 6ee7  ....mu.Q......n.
-00001140: 0e37 c8d8 bd3d a2db 52ba 9d3b dd20 638b  .7...=..R..;. c.
-00001150: 4778 5b8a b773 c71b 646c f188 6f4b e175  Gx[..s..dl..oK.u
-00001160: eef3 36c8 d8e2 11e0 96d2 ebdc 276e 9071  ..6.........'n.q
-00001170: c5cf 11e1 76fa 1532 e74e 38c8 d8e2 11e1  ....v..2.N8.....
-00001180: ce3a 2d3b 77c2 41c6 168f 0877 56c2 9d3b  .:-;w.A....wV..;
-00001190: e120 638b 4784 3b2b bdce 9d70 90b1 c5b3  . c.G.;+...p....
-000011a0: 7b6b 4ab8 b3dc 5d03 0a1a c29d 23c2 edf4  {kJ...].....#...
-000011b0: eb0e 77e9 8483 8cfd e611 e1ce 4ab8 4b27  ..w.........J.K'
-000011c0: 1c64 6cf1 8870 6725 dca5 130e 32b6 7844  .dl..pg%....2.xD
-000011d0: b8b3 12ee d209 0719 5b3c 22dc 5909 77e9  ........[<".Y.w.
-000011e0: 8483 8c2b 7e89 08b7 d36d 87eb 8483 8c2d  ...+~....m.....-
-000011f0: 1e11 eea2 84bb 74c2 41c6 168f 0877 51c2  ......t.A....wQ.
-00001200: 5d3a e120 638b 4784 bb54 fafb b38a c74d  ]:. c.G..T.....M
-00001210: bef4 f1e9 db25 82db 5bfa 5d5d f9be c7b9  .....%..[.]]....
-00001220: 76c9 1e1c 54fa 5ddd 0ef3 fd61 6d32 6f78  v...T.]....am2ox
-00001230: 7a89 90b6 d3af 1f2c 630d d4fb d1df cba5  z......,c.......
-00001240: d925 22da 4ebf d696 ef0d d073 b523 a05d  .%".N......s.#.]
-00001250: 0068 fd24 4619 573c 02da 4581 7695 c744  .h.$F.W<..E.v..D
-00001260: 003d 53fc 1a01 6da7 db16 9747 45fa 10e1  .=S...m....GE...
-00001270: e28a 4740 bb2a d0ae fd24 0619 5b3c 02da  ..G@.*...$..[<..
-00001280: 159e 82f6 9318 646c f108 6857 25d6 b59f  ......dl..hW%...
-00001290: c420 638b 4754 bb2a b6ae fd24 0619 5b3c  . c.GT.*...$..[<
-000012a0: 42db 552f 4aaf 9d31 90b1 c5b3 e7a2 0aaf  B.U/J..1........
-000012b0: 6b87 faf5 38e0 ae11 e076 ba1d 6a9d 7090  k...8....v..j.p.
-000012c0: b1df 3c22 dc15 6eba 75c2 41c6 168f 0877  ..<"..n.u.A....w
-000012d0: 8527 a09d 7090 71c5 6f11 e176 badd 32ef  .'..p.q.o..v..2.
-000012e0: 8483 8c2d 1e11 ee06 cf0a e481 384c eb0c  ...-........8L..
-000012f0: 5e6f 11e1 76ba 7df3 4e38 c8d8 6f1e 11ee  ^o..v.}.N8..o...
-00001300: 064b 393a e120 638b 4784 bbc1 7a8e 4e38  .K9:. c.G...z.N8
-00001310: c8d8 e211 e16e b0a6 a313 0e32 b678 44b8  .....n.....2.xD.
-00001320: 1bac ebe8 8483 8c2d 9ead fe80 b51d 9d70  .......-.......p
-00001330: b7e3 73b8 5b44 b89d 6e7b 7b27 1c64 ec37  ..s.[D..n{{'.d.7
-00001340: 8f08 7783 e70a 9d70 9071 c5ef 11e1 76ba  ..w....p.q....v.
-00001350: cd9c 3be1 2063 8b47 84bb 2bbd ee9d 7090  ..;. c.G..+...p.
-00001360: b1c5 23c2 dd75 0e77 9765 3f70 e16a f07a  ..#..u.w.e?p.j.z
-00001370: 8f08 b7d3 6dd8 3be1 2063 bf79 44b8 bb12  ....m.;. c.yD...
-00001380: eede 0907 195b 3c22 dc5d 0977 ef84 838c  .....[<".].w....
-00001390: 2d1e 11ee ae84 bb77 c241 c616 8f08 7757  -......w.A....wW
-000013a0: 7add 3be1 2063 8b47 84bb eb1c eede 0907  z.;. c.G........
-000013b0: 195b 3c22 dc1d ae52 fb02 3b8d 3c7e 40f0  .[<"...R..;.<~@.
-000013c0: e5d6 c023 02dc 4eff fcd6 0044 6ced 886f  ...#..N....Dl..o
-000013d0: 0fe5 9b3c b585 8c2d 1ef1 eda1 ec7a 74b2  ...<...-.....zt.
-000013e0: 53c6 8d7a c4b7 87ce e01e 9dec 9471 c523  S..z.........q.#
-000013f0: be3d 946f 8f4e 76ca b8e2 11df 1eca b787  .=.o.Nv.........
-00001400: 2cea 848c 2b1e f1ed a17c 7b74 b253 c615  ,...+....|{t.S..
-00001410: 8ff8 f650 bec9 7a74 cab8 e211 df1e cab7  ...P..zt........
-00001420: 4727 3b65 5cf1 886f 0f80 5727 3b65 4cf1  G';e\..o..W';eL.
-00001430: 710a d7f2 ea3d b687 2cee dc9f f9ca 41c7  q....=..,.....A.
-00001440: 9971 8a28 f78c bf7e 747d 0559 4dac 30f4  .q.(...~t}.YM.0.
-00001450: 0d44 a41b 2745 5d35 250d 0010 ed16 8868  .D..'E]5%......h
-00001460: 374e 8abb 6a4a 1a00 28da 0622 e28d 9322  7N..jJ..(.."..."
-00001470: af9a 9206 008c b681 887a e3a4 48ab a6a4  .........z..H...
-00001480: 81e3 e01b a788 7ccf 78df 0975 493b 00d2  ......|.x..uI;..
-00001490: 8e40 44bf 7152 fc55 5332 0200 49db 4044  .@D.qR.US2..I.@D
-000014a0: c071 5204 5653 d200 80d2 3610 5170 9c14  .qR.VS....6.Qp..
-000014b0: 83d5 9434 707c a637 42a9 81ac 8693 9010  ...4p|.7B.......
-000014c0: 5216 4423 23e1 8eb7 9d50 b49d 0129 df40  R.D##....P...).@
-000014d0: 4642 f21b 8690 1052 be81 8c84 2439 0c21  FB.....R....$9.!
-000014e0: 21a4 7c03 1909 c974 1842 4248 f906 3212  !.|....t.BBH..2.
-000014f0: 82ca 3086 9010 52be 818c 84e0 338c 2124  ..0...R.....3.!$
-00001500: 8494 6f20 2321 480d 63a8 e113 9070 ab0a  ..o #!H.c....p..
-00001510: c795 4830 1b86 6a3e 90f2 2390 9110 f486  ..H0..j>..#.....
-00001520: a1ae 0fa4 6c03 9906 31c0 7118 2afc 40ca  ....l...1.q.*.@.
-00001530: 3790 9110 6488 6aaa 9f0b 20e5 1bc8 4808  7...d.j... ...H.
-00001540: b6c3 50f5 0752 be81 8c84 a03c 0cf5 7f20  ..P..R.....<... 
-00001550: e51b c848 08de c350 0908 52be 818c 8420  ...H...P..R.... 
-00001560: 3f0c 3581 20e5 1bc8 4808 06c4 101d 6840  ?.5. ...H.....h@
-00001570: ca37 9091 1034 882a 2747 4140 c22d 401c  .7...4.*'GA@.-@.
-00001580: 2721 f812 43c4 a001 293f 0219 0941 9aa8  '!..C...)?...A..
-00001590: 7232 02c1 9c30 1327 0658 1143 1421 4ad9  r2...0.'.X.C.!J.
-000015a0: 11c8 e489 0166 4495 eb23 0029 df40 4642  .....fD..#.).@FB
-000015b0: b023 aa29 6920 b83a 5e19 0977 bccd 8ac5  .#.)i .:^..w....
-000015c0: 181a 90f2 2390 9110 2c89 2a27 2310 5c1d  ....#...,.*'#.\.
-000015d0: 6ff5 e1f8 6108 a6c4 78b7 baf1 2fef 1852  o...a...x.../..R
-000015e0: 7e04 3212 822d 31e4 56f4 8094 6f20 2321  ~.2..-1.V...o #!
-000015f0: 1813 554e 3641 40c2 ad41 049b 00ae 8e45  ..UN6A@..A.....E
-00001600: 241a e056 f811 c848 08e6 4495 9311 0848  $..V...H..D....H
-00001610: 9809 1603 ec89 2142 11a5 ec08 6c25 e2f8  ......!B....l%..
-00001620: 2600 83a2 caf5 1180 946f 2023 2158 1443  &........o #!X.C
-00001630: c4a2 0129 df40 4642 3029 aa9c 8c40 709f  ...).@FB0)...@p.
-00001640: f09c 9170 c71b 8a45 301a 90f2 2390 cd09  ...p...E0...#...
-00001650: c1a8 a872 3202 c17d c2ad 4904 3ba1 de01  ...r2..}..I.;...
-00001660: 1c22 1a0d 702f fc08 6424 04b3 a2ca c908  ."..p/..d$......
-00001670: 0424 dcba 4430 0240 4211 8e06 3818 7e04  .$..D0.@B...8.~.
-00001680: 3212 8261 51e5 6404 0212 6622 c600 cb62  2..aQ.d...f"...b
-00001690: 8878 4429 3b02 5b9d 38be 09c0 b490 3d00  .xD);.[.8.....=.
-000016a0: 32d5 d2f7 517a 7924 3eb6 3d11 d487 b52f  2...Qzy$>.=..../
-000016b0: 7dfc 41c8 f849 fd8c 836f 4e46 fb09 189d  }.A..I...oNF....
-000016c0: 8d40 e827 0d64 1cdc 2a47 e3a0 0858 0353  .@.'.d..*G...X.S
-000016d0: 7613 6420 040f a3b6 a26c 0478 ace2 7782  v.d .....l.x..w.
-000016e0: 6c4e 08c2 c610 156b 60ca 8e41 8642 d036  lN.....k`..A.B.6
-000016f0: 6acc 650c e0c1 8a1f 83ec 9909 8819 e322  j.e............"
-00001700: f74a 3165 c720 8321 181c 35e6 3206 f068  .J1e. .!..5.2..h
-00001710: c58e 4166 710c d038 86e8 599c 7263 b0c5  ..Afq..8..Y.rc..
-00001720: 8be3 3802 4f63 bc5b 79f4 d7e5 11a6 6c07  ..8.Oc.[y.....l.
-00001730: d9cc 1064 8d71 9127 4798 b21d 6448 0463  ...d.q.'G...dH.c
-00001740: a3c6 bcef 0794 f2fb 41c6 44d0 36c6 557f  ........A.D.6.U.
-00001750: 2c09 9e34 fb0e 3226 82bb 3144 ea19 94f2  ,..4..2&..1D....
-00001760: 1d64 4c04 8163 5ce5 4e01 a57c 0719 13c1  .dL..c\.N..|....
-00001770: e218 a2f7 0c4a f90e 3226 82ca 5163 2e7b  .....J..2&..Qc.{
-00001780: 22cc 227d 0719 13c1 e718 22fa 0c4a d90e  "."}......"..J..
-00001790: 32ef 6380 d451 63de c780 52be 83ec 010a  2.c..Qc...R.....
-000017a0: d81f e32a 9364 4af9 0e32 2682 de51 632e  ...*.dJ..2&..Qc.
-000017b0: 6300 6b6f 7c07 1913 c1f1 a82d 231d c0e2  c.ko|......-#...
-000017c0: 1bdf 41c6 4410 3dc6 4d98 4829 df41 c644  ..A.D.=.M.H).A.D
-000017d0: b03d c64d 7f46 2e99 276e 87e3 f8d9 1994  .=.M.F..'n......
-000017e0: 0f99 9f40 66dc 7e70 f3f5 6265 6b1c 417d  ...@f.~p..bek.A}
-000017f0: 9dff e971 0073 445f 3fe3 2189 1ffa 0803  ...q.sD_?.!.....
-00001800: 523f 1981 8c87 647f e823 0448 f90e 324b  R?....d..#.H..2K
-00001810: 6480 02a2 176c 10fa 4903 190e 4103 1937  d....l..I...A..7
-00001820: b954 c094 db0d b700 727c 3704 5f64 dce4  .T......r|7._d..
-00001830: b488 29db 4186 4310 4286 fc9e c1c0 94ed  ..).A.C.B.......
-00001840: 20c3 2158 21e3 26a7 454c d90e 321c 821a   .!X!.&.EL..2...
-00001850: 326e 8203 4cd9 0eb2 2922 f821 e326 a745  2n..L...)".!.&.E
-00001860: 4cd9 0eb2 2922 4822 7580 f6d3 22a5 2c12  L...)"H"u...".,.
-00001870: b7fa 111c 0b30 f9bb cb69 117c 929f f020  .....0...i.|... 
-00001880: 4322 2825 43dc b141 293b 0699 5732 c01a  C"(%C..A);..W2..
-00001890: a963 af6f 054a f90e 3226 823a 32ee c244  .c.o.J..2&.:2..D
-000018a0: 4af9 0eb2 2922 f823 4354 b241 29df 41c6  J...)".#CT.A).A.
-000018b0: 4490 4886 f864 8352 be83 8c89 6092 0c91  D.H..d.R....`...
-000018c0: ca06 a57c 0719 1341 3919 6296 0d4a f90e  ...|...A9.b..J..
-000018d0: 3226 8253 52c7 9e1c 0bf0 e8c5 7790 3111  2&.SR.......w.1.
-000018e0: c492 3a42 a583 649a b875 91e3 4c04 bb64  ..:B..d..u..L..d
-000018f0: eaa2 4348 bd5b 89f0 3a4f deca 48d0 80de  ..CH.[..:O..H...
-00001900: 239c bae8 103c 14d7 c0cc 3c94 67fc f5a6  #....<....<.g...
-00001910: fa94 4587 94f2 0d44 409c db5b 690d c8a2  ..E....D@..[i...
-00001920: 434a f906 221e 4e10 51a6 2c3a a494 6f20  CJ..".N.Q.,:..o 
-00001930: c2e1 0411 65ca a243 4af9 0622 1a4e 1051  ....e..CJ..".N.Q
-00001940: a62c 3aa4 946f 2082 e104 1165 caa2 434a  .,:..o ....e..CJ
-00001950: f906 2216 ceed adf4 9d50 7f83 5c59 e81b  .."......P..\Y..
-00001960: 8850 3841 4479 8882 4829 df40 74c1 3c41  .P8ADy..H).@t.<A
-00001970: 4499 fa4b e890 f20d 4493 c309 22ca d49f  D..K....D..."...
-00001980: 4387 946d 2013 5126 2826 536e 1950 ca37  C..m .Q&(&Sn.P.7
-00001990: 9091 1014 93a9 3f8c 0e29 df40 4642 524c  ......?..).@FBRL
-000019a0: 44c8 9c90 f20d 6424 04c5 64ea cfb3 43ca  D.....d$..d...C.
-000019b0: 3790 9110 1493 a9bf d10e 29df 4046 427a  7.........).@FBz
-000019c0: ef86 fe50 3ba4 7c03 1909 e9e5 1bef 3efb  ...P;.|.......>.
-000019d0: f958 6f42 ca37 9091 90de c021 cb2e 6b92  .XoB.7.....!..k.
-000019e0: a68b 11cc 957a cda7 92b7 ec3c e3ed 5c20  .....z.....<..\ 
-000019f0: f7cd 28e5 4720 2321 bd8b 4396 5dd6 24ed  ..(.G #!..C.].$.
-00001a00: f808 84ef e3a0 1772 c8b2 cb09 293b 02db  .......r....);..
-00001a10: 1939 3c2b aee9 977c b729 cb2e 29e5 1bc8  .9<+...|.)..)...
-00001a20: 4808 8ac9 9465 9735 490b 3641 4642 7a3f  H....e.5I.6AFBz?
-00001a30: 872c bbac 495a d040 4642 7a49 872c bbac  .,..IZ.@FBzI.,..
-00001a40: 495a d040 4642 504c a62c bb9c f43e 0fc7  IZ.@FBPL.,...>..
-00001a50: 81ed 8c04 3ba1 cef6 a62c bbac 3952 3002  ....;....,..9R0.
-00001a60: 1909 4144 99b2 ecb2 e648 4103 1909 4131  ..AD.....HA...A1
-00001a70: 99b2 ecb2 e648 4103 1909 4144 99b2 ecb2  .....HA...AD....
-00001a80: e648 c71b c844 949a 7c28 8864 d925 a52c  .H...D..|(.d.%.,
-00001a90: 8832 11a5 261f d040 bf75 4e29 df40 4642  .2..&..@.uN).@FB
-00001aa0: 1051 a62c bb9c f432 0f77 1866 22ca 04c5  .Q.,...2.w.f"...
-00001ab0: 64be 7b4e fbd7 8404 527e 0432 1282 8832  d.{N....R~.2...2
-00001ac0: 65d9 e1a4 977a d811 c848 088a c994 5587  e....z...H....U.
-00001ad0: 935e ec61 1bc8 e684 a098 4c59 7438 e9e5  .^.a......LYt8..
-00001ae0: 1eb6 818c 8420 a24c 5973 38e9 051f b681  ..... .LYs8.....
-00001af0: 8c84 a098 4c59 7258 5394 0044 1909 4144  ....LYrXS..D..AD
-00001b00: 99b2 e2b0 a628 c71b c844 9409 22ca 9405  .....(...D.."...
-00001b10: 8794 b287 6126 a24c 504c a6ac 37a4 946f  ....a&.LPL..7..o
-00001b20: 2023 2128 2653 961b d614 25d8 04d9 9c10   #!(&S....%.....
-00001b30: 4494 29ab 0d6b 8a12 3490 9110 1493 298b  D.)..k..4.....).
-00001b40: 0d6b 8a12 3490 9110 4494 296b 0d6b 8a12  .k..4...D.)k.k..
-00001b50: 3490 9110 1493 294b 0d6b 8a12 3490 9110  4.....)K.k..4...
-00001b60: 4494 292b 0d27 bd08 c491 3013 5126 2826  D.)+.'....0.Q&(&
-00001b70: 5316 1a52 ca1f 8619 0941 4499 b2ce b0a6  S..R.....AD.....
-00001b80: 28c7 3741 26a2 d4e4 43a7 64b2 cc90 5276  (.7A&...C.d...Rv
-00001b90: 0432 11a5 261f d280 fc52 0785 7cfd 0c84  .2..&....R..|...
-00001ba0: 2099 4c59 e558 3394 600b 6420 04c9 64ca   .LY.X3.`.d ..d.
-00001bb0: 22c7 9aa1 040d 6420 04c7 64ca 1ac7 9aa1  ".....d ..d.....
-00001bc0: 040d 6420 0411 65ca 12c7 9aa1 040d 6420  ..d ..e.......d 
-00001bd0: 04c3 64ca 0ac7 9aa1 040d 6420 040d 65be  ..d.......d ..e.
-00001be0: 7b2e fdd7 6501 a4fc 5190 4d09 c92f 39c9  {...e...Q.M../9.
-00001bf0: ef46 d514 2518 828c 8460 a14c 595e 5753  .F..%....`.LY^WS
-00001c00: 94e3 0d64 124a 4d3e 9484 b2ba 8e52 761b  ...d.JM>.....Rv.
-00001c10: 640e 4a4d 3ea0 81be ce95 52be 810c 8520  d.JM>.....R.... 
-00001c20: 974c 595b 5753 9460 1364 2824 b7e4 243f  .LY[WS.`.d($..$?
-00001c30: 9d55 7394 a083 8c85 60a0 4c59 dc57 7394  .Us.....`.LY.Ws.
-00001c40: a081 8c85 a096 4c59 db57 7394 a081 8c85  ......LY.Ws.....
-00001c50: 6496 9cf4 8c0c 31bf 1b66 3024 b3e4 a4ab  d.....1..f0$....
-00001c60: 3820 e63b c868 08fe c994 e58d 354b 0836  8 .;.h......5K.6
-00001c70: 4206 4310 4ba6 ac6e ac59 c2f1 0632 fba4  B.C.K..n.Y...2..
-00001c80: ceff 3a2b 3be9 320e 88d9 6db0 4591 e337  ..:+;.2...m.E..7
-00001c90: acc9 2b39 e99b d421 e63b c870 08f6 c994  ..+9...!.;.p....
-00001ca0: 059e 354f 0836 4286 4390 4fa6 acef ac79  ..5O.6B.C.O....y
-00001cb0: 42d0 4046 43b2 4a4e ba8a 0062 7e1b 6438  B.@FC.JN...b~.d8
-00001cc0: 04f7 64ca 02d3 0929 df40 8643 d24a e48e  ..d....).@.C.J..
-00001cd0: 3584 7cfd 0c86 f0c2 1145 2184 7cfd 0c85  5.|......E!.|...
-00001ce0: 2095 e87a 3608 f9fa 1909 4129 d1e5 6c10   ..z6.....A)..l.
-00001cf0: b2f5 33ed a4b0 af93 b2be c49a 42be 7eb6  ..3.........B.~.
-00001d00: 8c06 7c92 29eb 9beb dc70 9c01 9974 52c4  ..|.)....p...tR.
-00001d10: d333 41f7 2d28 e407 2083 20c8 2453 9657  .3A.-(.. . .$S.W
-00001d20: 1716 8301 c820 082e c994 d5d5 05a5 a081  ..... ..........
-00001d30: 8c81 a092 4c59 5c5d 3b45 d040 c640 3049  ....LY\];E.@.@0I
-00001d40: a6ac adae 8d12 3490 4110 4492 294b ab6b  ......4.A.D.)K.k
-00001d50: a304 0d64 1404 8f64 caab 2c6a a304 0d64  ...d...d..,j...d
-00001d60: 1804 8d64 caeb 2c6a a31c 6f20 734d 6ab8  ...d..,j..o sMj.
-00001d70: 9583 f24a 0b4a 590e 6c2b e4f8 7c10 2492  ...J.JY.l+..|.$.
-00001d80: a96b 4ae9 7d27 ee5e f196 4282 0614 8453  .kJ.}'.^..B....S
-00001d90: 5e6d 511b 25d8 0419 0941 2199 f27a 8b09  ^mQ.%....A!..z..
-00001da0: 29bf 0932 1282 4132 7545 25a4 7c03 1909  )..2..A2uE%.|...
-00001db0: 4120 990f 998d 41ca 3790 9110 2c93 292f  A ....A.7...,.)/
-00001dc0: baa8 8d12 ec03 1909 4132 59f2 a28b da28  ........A2Y....(
-00001dd0: 4103 1909 c91e 9117 5dd4 4609 1ac8 4848  A.......].F...HH
-00001de0: f688 bce8 a236 cae1 066a fc2a 7b98 03cf  .....6...j.*{...
-00001df0: f8eb 8aca 252f bac0 9401 d1ca 5e76 f28c  ....%/......^v..
-00001e00: f706 ba74 8729 db40 7461 bcc0 3159 a7ee  ...t.).@ta..1Y..
-00001e10: 1760 ca36 1091 b086 5bb7 aebc e802 53b6  .`.6....[.....S.
-00001e20: 8188 840b 1c93 252f bac0 946d 2022 610d  ......%/...m "a.
-00001e30: 378c 4027 21a6 6c03 1109 1738 264b 5e74  7.@'!.l....8&K^t
-00001e40: 8129 db40 44c2 1a6e 1d01 7960 8129 db40  .).@D..n..y`.).@
-00001e50: 44c2 45f6 88bc e802 53b6 8188 8435 dc30  D.E.....S....5.0
-00001e60: 02fd 7739 30e5 1ac8 1c93 058e c992 bbf5  ..w90...........
-00001e70: 98b2 0d44 17c7 8bec 1179 d105 a66c 0319  ...D.....y...l..
-00001e80: 09c9 1e91 175d acc0 31a9 f18b 4e46 648f  .....]..1...NFd.
-00001e90: c8cd fae7 87b6 3386 1d81 8c84 648f 8873  ......3.....d..s
-00001ea0: ba02 c764 6d1d e4f8 e998 ec11 714e 9f1f  ...dm.......qN..
-00001eb0: 7a74 0432 1292 3d22 b7e8 56e0 98ac ad83  zt.2..="..V.....
-00001ec0: 0423 0024 947b 74cf 0f3d 3a02 1909 e135  .#.$.{t..=:....5
-00001ed0: 264b 6ed2 2d4a d99d 3023 21d9 23f2 b062  &Kn.-J..0#!.#..b
-00001ee0: 058e c9ca 1c93 67bc 0dae 38a7 9872 2390  ......g...8..r#.
-00001ef0: 3926 35dc 7a2e 10e7 1453 b681 8c84 648f  9&5.z....S....d.
-00001f00: c8d3 9a15 3826 6beb 20c7 8f02 b247 44f9  ....8&k. ....GD.
-00001f10: 7c7e e8c1 a360 eb20 4103 7007 5094 cf15  |~...`. A.p.P...
-00001f20: 3826 6beb 2041 033a 2794 a5e5 cfcf 3c3a  8&k. A.:'.....<:
-00001f30: 0019 0849 1e91 8745 2b50 4cd6 b641 8201  ...I...E+PL..A..
-00001f40: 2010 f6df 8078 7ee8 d111 c840 88f2 48ff   ....x~....@..H.
-00001f50: 0988 1528 266b db20 c108 d065 6fff 559c  ...(&k. ...eo.U.
-00001f60: e787 1e1c 814c 3159 a898 b4df c0a0 90bb  .....L1Y........
-00001f70: 41b3 32c3 e419 6fba a35c 9982 86e2 eb67  A.2...o..\.....g
-00001f80: 1824 c1a4 2fe1 5981 5fb2 32bf e419 6fdf  .$../.Y._.2...o.
-00001f90: bf3f ada1 90ff fed9 7410 c511 b926 09f4  .?......t....&..
-00001fa0: 9295 bde7 e419 effb f68f 73dc 7325 1da7  ..........s.s%..
-00001fb0: f887 cdd7 3641 8e1f 82a4 97c8 8579 6097  ....6A.......y`.
-00001fc0: ac2d 8204 f515 82a2 dd3f 3ff3 2801 3206  .-.......??.(.2.
-00001fd0: 9236 2208 0cdc 92b5 3590 e0fb d355 b110  .6".....5....U..
-00001fe0: 28b8 3d98 a925 0bd4 1251 de31 e426 6299  (.=..%...Q.1.&b.
-00001ff0: 59b2 c02c 5962 9c73 ca1c 005b 0239 be01  Y..,Yb.s...[.9..
-00002000: d019 1106 0766 c9da 1248 d000 3d0b 1608  .....f...H..=...
-00002010: 0766 c9ca 5e71 f28c f7a3 4b28 1c98 256b  .f..^q....K(..%k
-00002020: 4b20 c108 d0b3 6081 5060 96ac ec15 27cf  K ....`.P`....'.
-00002030: 781f 0199 8905 66c9 da12 4830 0230 1514  x.....f...H0.0..
-00002040: e3fc f9a1 0731 9899 250b cc92 3ae8 3a87  .....1..%...:.:.
-00002050: 2865 3990 5d13 9333 22c6 f90a cc92 9599  (e9.]..3".......
-00002060: 25cf 781b 5c31 ce31 e546 2033 4b16 9825  %.x.\1.1.F 3K..%
-00002070: 7568 f64d 4029 db40 3619 2469 448c f315  uh.M@).@6.$iD...
-00002080: a825 6b5b 20c7 8f02 9246 c438 7f7e e8c1  .%k[ ....F.8.~..
-00002090: a360 5b20 4103 704d 2cc6 f90a d492 b52d  .`[ A.pM,......-
-000020a0: 90a0 0120 a1bc e8e7 f9a1 4747 20bb 2826  ... ......GG .(&
-000020b0: 6944 8cf3 15a8 256b 5b20 c108 0009 f5b6  iD....%k[ ......
-000020c0: 40a0 96ac 2d81 040d c0b3 6031 ce9f 1f7a  @...-.....`1...z
-000020d0: 7413 6424 2467 448c f315 9825 2b33 4b9e  t.d$$gD....%+3K.
-000020e0: f1f6 ddc4 38c7 9403 5166 962c 304b eaa0  ....8...Qf.,0K..
-000020f0: eb24 a494 6d20 2321 3923 629c afc0 2c59  .$..m #!9#b...,Y
-00002100: db01 39be 13be c5bf fdf6 e1eb 874f 1fff  ..9..........O..
-00002110: fc54 879b 7cf7 e3eb 07d7 b63f 82d2 c5c0  .T..|......?....
-00002120: efa5 f5ae 74e0 92ac ad7d 0495 0b7e efbe  ....t....}...~..
-00002130: b4cc 4003 8b64 6ddf 2328 5d94 7c57 5ae6  ..@..dm.#(].|WZ.
-00002140: 9e47 f491 5fbf fee3 cb97 6fbf 7ffe f6f9  .G.._.....o.....
-00002150: d3ff 0300 00ff ff00 0000 ffff 4451 db4e  ............DQ.N
-00002160: c330 0cfd 95c8 ef2c 5d27 36a8 d649 5c84  .0.....,]'6..I\.
-00002170: b407 24a4 7d41 68dd 25a2 8d23 c783 31c4  ..$.}Ah.%..#..1.
-00002180: bfe3 eec2 f2e0 f838 f239 f6c9 d2ed 845e  .......8.9.....^
-00002190: 422f c886 b1ab e161 5a3d cee6 7330 7bae  B/.....aZ=..s0{.
-000021a0: 76a1 ade1 a738 9f1b bdef c750 5cc3 e5ed  v....8.....P\...
-000021b0: 17ec 6a99 8965 234e f0ca 74a7 3c43 1f73  ..j..e#N..t.<C.s
-000021c0: b5ef b92d 6bf0 22a9 b236 371e 0797 2743  ...-k."..67...'C
-000021d0: 6898 3275 3269 68b0 d475 a141 9b13 a36b  h.2u2ih..u.A...k
-000021e0: b347 94a1 b765 315d 580e 8d6f 9db8 124e  .G...e1]X..o...N
-000021f0: 2a4f 14db 2081 e259 a91c e5ed bffe 6a99  *O.. ..Y......j.
-00002200: 3c45 94d0 bcb1 e928 ca5a f798 8291 ef84  <E.....(.Z......
-00002210: 3544 d2f6 4fe4 acfd 635f 725b 7c75 bc0d  5D..O...c_r[|u..
-00002220: 319b 1e3b a9a1 982c c070 d8fa 4b2e 948e  1..;...,.p..K...
-00002230: d55b 30ef 2442 c305 799d 1479 4433 5025  .[0.$B..y..yD3P%
-00002240: 521b 4fe0 ccbb 41d9 2593 5c42 de84 838a  R.O...A.%.\B....
-00002250: df83 210e 18d5 2695 af21 a967 ec82 80f1  ..!...&..!.g....
-00002260: 5a3f e8ac ae7f 4e41 49c0 e88c bac2 1573  Z?....NAI......s
-00002270: 35fe 07af dbe9 71dd 2fe2 8fa3 4bab 3f00  5.....q./...K.?.
-00002280: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00002290: 0000 2100 1162 deb5 f824 0000 3618 0100  ..!..b...$..6...
-000022a0: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-000022b0: 732f 7368 6565 7432 2e78 6d6c 9c93 4d8f  s/sheet2.xml..M.
-000022c0: db20 1086 ef95 fa1f 10f7 18db 499c ae15  . ..........I...
-000022d0: 67b5 6a14 756f 553f cf04 8f63 1430 2e90  g.j.uoU?...c.0..
-000022e0: 2f55 fdef 1d6c 271b 2917 6b91 cd60 609e  /U...l'.).k..``.
-000022f0: 7706 c6cb e7b3 56e4 08d6 49d3 1434 8962  w.....V...I..4.b
-00002300: 4aa0 11a6 94cd aea0 3f7f 6c26 9f28 719e  J.......?.l&.(q.
-00002310: 3725 57a6 8182 5ec0 d1e7 d5c7 0fcb 93b1  7%W...^.........
-00002320: 7b57 0378 8284 c615 b4f6 becd 1973 a206  {W.x.........s..
-00002330: cd5d 645a 6870 a532 5673 8f9f 76c7 5c6b  .]dZhp.2Vs..v.\k
-00002340: 8197 9d93 562c 8de3 8c69 2e1b da13 723b  ....V,...i....r;
-00002350: 8661 aa4a 0a58 1b71 d0d0 f81e 6241 718f  .a.J.X.q....bAq.
-00002360: f1bb 5ab6 ee4a d362 0c4e 73bb 3fb4 1361  ..Z..J.b.Ns.?..a
-00002370: 748b 88ad 54d2 5f3a 2825 5ae4 afbb c658  t...T._:(%Z....X
-00002380: be55 98f7 3999 7141 ce16 9f14 dfe9 55a6  .U..9.qA......U.
-00002390: 9b7f 50d2 5258 e34c e523 24b3 3ee6 c7f4  ..P.RX.L.#$.>...
-000023a0: 9fd8 13e3 e246 7acc 7f14 2699 310b 4719  .....Fz...&.1.G.
-000023b0: 2ef0 0d95 be2f a464 7e63 a56f b0e9 3b61  ...../.d~c.o..;a
-000023c0: d90d 168e cbe6 0759 16f4 6f3c b409 da24  .......Y..o<...$
-000023d0: 74f1 244e 4277 d7fe d1d5 b294 78c3 212b  t.$NBw......x.!+
-000023e0: 62a1 2ae8 4b92 afa7 5946 d96a d955 d02f  b.*.K...YF.j.U./
-000023f0: 0927 7737 269e 6fbf 8302 e101 5512 4a42  .'w7&.o.....U.JB
-00002400: 816e 8dd9 878d af38 1523 d375 1b02 930b  .n.....8.#.u....
-00002410: 2f8f f019 940a e805 06e8 fe0c 3a8b 69fe  /...........:.i.
-00002420: 923c cd82 12bb 49dd 8faf b29b aeb6 bf5a  .<....I........Z
-00002430: 5242 c50f ca7f 33a7 2f20 77b5 47fd 2c9a  RB....3./ w.G.,.
-00002440: 63ce a168 f2f2 b206 27b0 5a31 8628 9d07  c..h....'.Z1.(..
-00002450: ae30 0a21 d813 2dc3 6f87 d5c6 cf7d d4b2  .0.!..-.o....}..
-00002460: f435 8e92 e0bf 05e7 3732 e028 1107 e78d  .5......72.(....
-00002470: fe3d 2c0f 90de 1daf aa73 477b ead7 d32c  .=,......sG{...,
-00002480: 4a50 692c 00b3 ef00 6807 4096 468b f1fe  JPi,....h.@.F...
-00002490: b3c1 1fed e08f f98f 0880 75e7 f01f 0000  ..........u.....
-000024a0: ffff 0000 00ff ff94 5ded aee5 3672 7c95  ........]...6r|.
-000024b0: c53c 407c 49ea 835a d803 e448 2f62 3806  .<@|I..Z...H/b8.
-000024c0: f6d7 26d8 319c e4ed d394 8339 ecaa eab9  ..&.1......9....
-000024d0: ea7f 33b7 eb50 dde2 47b5 a866 e9e7 6fff  ..3..P..G..f..o.
-000024e0: f8fd f73f ae5f fff8 f5eb cfff facf fffe  ...?._..........
-000024f0: dbbf 7ef9 52be fced db7f fdfa cf6f f6af  ..~.R........o..
-00002500: bf2f 5ffe f63f 65f9 f5b7 bfff c7ff 5ebf  ./_..?e.......^.
-00002510: 7ffb edf7 7ffe f1cb 978f 7fab eb97 af3f  ...............?
-00002520: ff36 b0ff 6e60 fbd3 37fb ff9f 5f8f faf1  .6..n`..7..._...
-00002530: f34f 7f7e fdf9 a7df fedf faf2 d6e2 ada7  .O.~............
-00002540: b756 6fbd bcb5 7db7 fe64 6e7e f7b5 667c  .Vo...}..dn~..f|
-00002550: 1de0 3bbc ef1e 6fe0 2f23 da7a 80d7 9fb6  ..;...o./#.z....
-00002560: 7231 62d7 deb7 8cf7 03ec bdef e03d 23da  r1b..........=#.
-00002570: 063d 727e daca c588 c07b 1b1b cfc7 c900  .=r~.....{......
-00002580: 7bef e1be be3e 459c 9f22 2e46 04be af19  {....>E..".F....
-00002590: df07 d8fb 5e70 a033 a4e3 6438 3f6f e662  ....^p.3..d8?o.b
-000025a0: 48e0 ff96 f17f 80c1 7f98 8a2f 86f4 8ad3  H........../....
-000025b0: f5f3 662e 8604 feef 19ff 0718 fc87 c5e2  ..f.............
-000025c0: f539 e4fc 1c72 3124 70bf 67dc 1f60 70ff  .9...r1$p.g..`p.
-000025d0: bd9a ddab e88b 21bd 4288 e7e7 cd5c 0c09  ......!.B....\..
-000025e0: fc3f 32fe 0f30 f8bf c0ca c390 5e21 c6f3  .?2..0......^!..
-000025f0: f366 2e86 04fe 978f 4c00 371a 2258 91a9  .f......L.7."X..
-00002600: 468b b0bc 5608 f37c d0d0 2530 5110 39a2  F...V..|..%0Q.9.
-00002610: 1d68 0802 e9ab 30a6 6dc4 ba0a 44e4 cba0  .h....0.m...D...
-00002620: 288a 1405 17e6 c6f2 6ef8 afc9 2030 6dc3  (.......n... 0m.
-00002630: d124 41d0 5f97 0045 51a4 a8b8 3047 1624  .$A._..EQ...0G.$
-00002640: 6381 691b 8cba 5382 a057 2f01 8aa2 4851  c.i...S..W/...HQ
-00002650: 7261 b62c 48ca 02d3 36e8 b053 82e0 7e5c  ra.,H...6..S..~\
-00002660: 0214 4591 22e7 c29c c969 2863 da86 799d  ..E."....i(c..y.
-00002670: 68a8 edc0 f397 0045 51a4 28ba 3073 22ff  h......EQ.(.0s".
-00002680: be04 a6ed 34bb b9a1 b6d3 ec7e ccd3 2545  ....4......~..%E
-00002690: d437 daaf 5148 632f 8169 3bcd 6e66 e2b6  .7..QHc/.i;.nf..
-000026a0: d3ec 7e4c d725 c5d7 371a a240 c216 98b6  ..~L.%..7..@....
-000026b0: d3ec 663e 6e3b cdee c7a4 5d52 ac7d a321  ..f>n;....]R.}.!
-000026c0: 0aa4 6d81 693b cd6e 66e5 b6d3 ec7e 4cdd  ..m.i;.nf....~L.
-000026d0: 3545 dd37 1aa2 40ea 1698 b6d3 531b f37b  5E.7..@.....S..{
-000026e0: eb38 bb45 4bc1 ecae 29ee bed1 1005 3d7a  .8.EK...).....=z
-000026f0: 0a5a ee38 bb45 43ad e3ec 16a0 288a dce3  .Z.8.EC.....(...
-00002700: 3373 7745 eeae e209 bae3 ec96 209c dd02  3swE........ ...
-00002710: 1445 91e2 eeca dc5d 91bb 05a6 759c dd12  .E.....]....u...
-00002720: 84b3 5b80 a228 52dc 5d99 bb2b 72b7 c0b4  ..[..(R.]..+r...
-00002730: 8eb3 5b82 7076 0b50 1445 8abb 6d1f 0973  ..[.pv.P.E..m..s
-00002740: da86 4fd6 0ad3 6976 8b86 0e9a dd8f 9fae  ..O...iv........
-00002750: 6b8a bb6f b49f dd0d 9faf 15e6 a0d9 2db8  k..o..........-.
-00002760: fba0 d9fd 98bb 6b8a bb6f 3444 814f d90a  ......k..o4D.O..
-00002770: 73d0 ec16 dc7d d0ec 7ecc dd35 c5dd 37da  s....}..~..5..7.
-00002780: 4741 0bad 6065 dee4 6310 4d6d d1ce 3b4c  GA..`e..c.Mm..;L
-00002790: bf4b 9962 ee2a 9ea6 719f 5270 326d f57d  .K.b.*..q.Rp2m.}
-000027a0: dece 2520 2d88 a1a5 78fb 46c3 6842 de56  ..% -...x.F.hB.V
-000027b0: 9803 5759 013a 565c 9f54 4b51 1829 e26e  ..WY.:V\.TKQ.).n
-000027c0: ea59 1977 5d05 e680 c172 8a86 7a85 582f  .Y.w]....r..z.X/
-000027d0: 75b5 288c 1473 37c1 cac8 dc0a 7320 5b08  u.(..s7.....s [.
-000027e0: 50af 3831 544b 5118 b91d 70b1 c14d 7be0  P.81TKQ...p..M{.
-000027f0: 0273 00e8 6c62 171c 5399 4b80 c2b9 91e2  .s..lb..S.K.....
-00002800: eec6 dcdd 90bb 2506 594f 803a e632 976a  ......%.YO.:.2.j
-00002810: 29ea 8d14 7937 a6d3 05c9 5b62 e895 0437  )...y7....[b...7
-00002820: 74e0 d3f9 255a 0a7b 23c5 de8d f974 41f6  t...%Z.{#....tA.
-00002830: 5698 0f64 6f01 ea8d a6b8 a0f8 a837 52f4  V..do........7R.
-00002840: dd98 5017 a46f 85f9 c06d 6601 ea98 5a5e  ..P..o...mf...Z^
-00002850: 0214 f646 8abf 1b93 ea82 cfde 0af3 8159  ...F...........Y
-00002860: 8800 75cc 2d2f 010a c348 5178 637e 5ef0  ..u.-/...HQxc~^.
-00002870: e15b 613e 70c7 5980 7aa3 0557 6403 c1a0  .[a>p.Y.z..Wd...
-00002880: 5a52 2c7e a33d 8b2f c8e2 0af3 812c 2e40  ZR,~.=./.....,.@
-00002890: bd01 b95c 0214 f5c6 9262 f11b 0d61 6056  ...\.....b...a`V
-000028a0: a830 1fc8 e202 d41b 2623 0214 8691 62f1  .0......&#....b.
-000028b0: 8559 7c41 1657 980f 6471 01ea f8c4 7209  .Y|A.W..dq....r.
-000028c0: 5018 468a c517 26df 0559 5c61 3e90 c505  P.F...&..Y\a>...
-000028d0: a823 915e 0214 8691 7ba1 cd2c bed0 2b6d  .#.^....{..,..+m
-000028e0: 81f9 4016 5f18 d41b 3ef5 0950 1846 8ac5  ..@._...>..P.F..
-000028f0: 1726 df15 595c 6016 7c03 7e0a 50c7 7ce0  .&..Y\`.|.~.P.|.
-00002900: 12a0 308c 148b 2fcc ab2b b2b8 c02c 0559  ..0.../..+...,.Y
-00002910: 5c80 3ae6 0397 0085 61a4 587c 6116 5f91  \.:.....a.X|a._.
-00002920: c505 6629 c8e2 02d4 311f b804 280c 23c5  ..f)....1...(.#.
-00002930: e20b b3f8 8a2c 2e30 4b41 1617 a08e f9c0  .....,.0KA......
-00002940: 2540 6118 2916 5f98 5757 6471 8159 0ab2  %@a.)._.WWdq.Y..
-00002950: b800 f506 b15e 0214 85b1 a658 fc46 7bfa  .....^.....X.F{.
-00002960: 5b91 c505 6629 c8e2 02d4 2717 efb7 b797  [...f)....'.....
-00002970: 0085 61a4 587c e5e7 ec15 595c 6096 822c  ..a.X|....Y\`..,
-00002980: 2e40 1db3 b34b 80c2 3052 2cbe 328b afc8  .@...K..0R,.2...
-00002990: e202 b3e0 6bf2 5380 3a66 6797 0085 61a4  ....k.S.:fg...a.
-000029a0: 587c 6516 a7ce 108f e2b4 d1f6 793b 9780  X|e.........y;..
-000029b0: 4c3b 406e a36d 4d51 f88d 869a 0fd8 dc11  L;@n.mMQ........
-000029c0: 10ae a9fb bc9d 4b40 c218 52fc bd0a fec6  ......K@..R.....
-000029d0: 3444 6098 311e 3474 29cc 3b2b f33d 91a2  4D`.1.4t).;+.=..
-000029e0: ef95 e91b b733 5f02 b360 d5c5 2940 0796  .....3_..`..)@..
-000029f0: f15c 0214 7646 8abe 57a6 6f2c bf79 09cc  .\..vF..W.o,.y..
-00002a00: 8265 17a7 001d b45d 2840 6118 29fa 5ec5  .e.....](@a.).^.
-00002a10: e637 6621 02b3 70c5 2337 74d0 76a1 6829  .7f!..p.#7t.v.h)
-00002a20: 0c23 45df 2bd3 3796 11bd 0466 a1c2 4701  .#E.+.7....f..G.
-00002a30: 3a68 bb50 80a2 30b6 147d df68 78a5 8159  :h.P..0..}.hx..Y
-00002a40: 88c0 2c54 4028 4007 6d17 0a50 1846 8abe  ..,T@(@.m..P.F..
-00002a50: 37a6 6f2c 877a 09cc 4275 8402 74d0 0695  7.o,.z..Bu..t...
-00002a60: 0085 61a4 e87b 13e5 df48 7c02 b350 2da1  ..a..{...H|..P-.
-00002a70: 001d b441 2540 6118 29fa de04 7d63 1622  ...A%@a.)...}c."
-00002a80: 300b 2e42 a700 1db4 9720 4061 1829 06df  0..B..... @a.)..
-00002a90: f8d9 79c3 bd04 8159 7011 3a05 e8a0 8770  ..y....Yp.:....p
-00002aa0: 010a c348 91f8 c624 8e1b e02f 8159 7011  ...H...$.../.Yp.
-00002ab0: 3a05 e8a0 070d 010a c348 b1f8 265e 4de3  :........H..&^M.
-00002ac0: 5e82 c02c b808 9d02 74d0 8386 0085 61a4  ^..,....t.....a.
-00002ad0: 587c 13ef a6a9 5e5e 6db7 e3ce 8e68 e8a0  X|....^^m....h..
-00002ae0: 3702 0214 8691 62f1 4d14 9621 8b0b cc82  7.....b.M..!....
-00002af0: 8bd0 2940 07ed 410b 5018 468a c537 5159  ..)@..A.P.F..7QY
-00002b00: 867b 0902 b3e0 2274 0ad0 417b d002 1485  .{...."t..A{....
-00002b10: b1a7 58fc 467b 16c7 82c6 97c0 2cb8 089d  ..X.F{......,...
-00002b20: 0274 d01e b400 8561 a458 7c17 75e1 b897  .t.....a.X|.u...
-00002b30: 2030 0b2e 42a7 001d b479 2b40 6118 2916   0..B....y+@a.).
-00002b40: dfc5 112d 6471 8159 7011 3a05 e8a0 5d4f  ...-dq.Yp.:...]O
-00002b50: 010a c348 b1f8 ce2c 8ee5 9b2f 8159 7011  ...H...,.../.Yp.
-00002b60: 3a05 e8a0 5d4f 010a c348 b1f8 2e8e 6d21  :...]O...H....m!
-00002b70: 8b0b cc82 8bd0 2940 07ed 7a0a 5018 468a  ......)@..z.P.F.
-00002b80: c577 515f 868f e202 b3e0 2274 0ad0 41bb  .wQ_......"t..A.
-00002b90: 9e02 1486 9162 f19d 591c 0b65 5f02 b3e0  .....b..Y..e_...
-00002ba0: 2274 0ad0 41fb 6c02 1486 9162 f19d 191a  "t..A.l....b....
-00002bb0: cb69 5f02 b3e0 2274 0ad0 41fb 6c02 1486  .i_..."t..A.l...
-00002bc0: 9162 f19d 591c 0b7e 5f02 b3e0 2274 0ad0  .b..Y..~_..."t..
-00002bd0: b1e0 9b64 010a c348 b1f8 2e6a da90 c505  ...d...H...j....
-00002be0: 66c1 45e8 14a0 03df 825e 0214 85d1 532c  f.E......^....S,
-00002bf0: 7ea3 61c7 109f c505 66c1 45e8 14a0 03df  ~.a.....f.E.....
-00002c00: 825e 0214 8691 62f1 ce2c 8ee5 cd2f 81e1  .^....b..,.../..
-00002c10: 977e 0274 50dd ad00 8561 a458 bc33 8b77  .~.tP....a.X.3.w
-00002c20: 6471 8159 702d 3d05 e8c0 97b9 9700 8561  dq.Yp-=........a
-00002c30: a458 bc8b 6a34 7c16 1798 05d7 d253 800e  .X..j4|......S..
-00002c40: 7c99 7b09 5018 468a c5bb 788f 8d2c 2e30  |.{.P.F...x..,.0
-00002c50: 0bae a5a7 001d f832 f712 a030 8c14 8b77  .......2...0...w
-00002c60: 6671 2c37 7f09 cc82 6be9 2940 07be ccbd  fq,7....k.)@....
-00002c70: 0428 0c23 c5e2 5dec a8c3 bb0d 0161 b583  .(.#..]......a..
-00002c80: cfdb b904 645a 03dc 5b81 9ea2 f01b fde3  ....dZ..[.......
-00002c90: f733 02c2 ef67 3e6f e712 9030 8614 7f77  .3...g>o...0...w
-00002ca0: 556d 8e1d 2130 5408 2d1a 3af0 94d3 a540  Um..!0T.-.:....@
-00002cb0: ef1d 18df 1529 feee ccdf 787c e125 300b  .....)....x|.%0.
-00002cc0: 52f3 2940 9dd2 1075 b520 8c23 c5df 37da  R.)@...u. .#..7.
-00002cd0: 8f28 3c60 f112 9805 a9f9 14a0 4e69 88ba  .(<`........Ni..
-00002ce0: 5a14 468a bf0f e66f 3c86 f112 9805 39ed  Z.F....o<.....9.
-00002cf0: 540d 61a5 c6a5 4051 1829 fe3e 98bf f1a0  T.a...@Q.).>....
-00002d00: c84b 6016 e4b4 5380 3a65 53ea 6a51 1829  .K`...S.:eS.jQ.)
-00002d10: fe3e 98bf 71f6 be04 6641 4e3b 05a8 531a  .>..q...fAN;..S.
-00002d20: a2ae 1685 91e2 ef83 f91b 8f31 bc04 6641  ...........1..fA
-00002d30: 4e3b 5543 5837 7329 5014 468a bf0f 514d  N;UCX7s)P.F...QM
-00002d40: 8ed9 94c0 2c38 ec4f 01ea 944d a9ab 4561  ....,8.O...M..Ea
-00002d50: a4f8 fb60 fec6 630c 2f81 59f0 469f 02d4  ...`..c./.Y.F...
-00002d60: 299b 5257 8bc2 4851 f8c1 4fe1 07ee 8908  ).RW..HQ..O.....
-00002d70: cc82 054a a700 75ca a6d4 d5a2 3052 2c7e  ...J..u.....0R,~
-00002d80: 3043 970f 7cb5 2140 0b56 289d 0274 d039  0C..|.!@.V(..t.9
-00002d90: 6405 8ae2 48d1 f8c1 345e f020 c34b 8016  d...H...4^. .K..
-00002da0: 2c51 3a05 a833 7388 ac21 88c3 6e67 4ed2  ,Q:..3s..!..ngN.
-00002db0: 85cf 7317 3ccb f0fa ab51 2c60 c73a 6285  ..s.<....Q,`.:b.
-00002dc0: eab4 6029 5494 22da 3dcd 05c3 7c5e f044  ..`)T.".=...|^.D
-00002dd0: 8305 c3a8 85ea a914 eac0 d964 2235 2283  ...........d"5".
-00002de0: 087b 2645 ead6 0b42 2e0b 3749 146a a113  .{&E...B..7I.j..
-00002df0: 8c0a d545 3022 8f08 8349 51bb f582 0886  ...E0"...IQ.....
-00002e00: b583 4449 3beb ee88 b63a ae0f d633 229b  ..DI;....:...3".
-00002e10: 0883 4911 7cf9 6086 2f78 c6c1 8699 285a  ..I.|.`./x....(Z
-00002e20: dfb0 be58 a13a 2e12 168c c829 c260 5234  ...X.:.....).`R4
-00002e30: 5f3e 98e7 0b9e 74b0 60c4 2135 d612 12a8  _>....t.`.!5....
-00002e40: 0337 8b2d 1891 5984 c1a4 c8de 7a41 0c33  .7.-..Y.....zA.3
-00002e50: 5214 12a8 65c3 5a63 d556 9ff6 14fe aad2  R...e.Zc.V......
-00002e60: 55a8 7835 4b51 bef5 8208 8684 8504 6a61  U.x5KQ........ja
-00002e70: 7d24 81ea b8e6 59cf 882c 23ec 9914 f197  }$....Y..,#.....
-00002e80: 0fc1 fca4 fea7 50cb 8675 c70a 7590 7a87  ......P..u..u.z.
-00002e90: 4485 c1a4 d8bf 7c08 fac7 1310 3667 18b5  D.....|.....6g..
-00002ea0: b0e6 9340 755c c0ad 6712 1940 52d4 4d89  ...@u\..g..@R.M.
-00002eb0: b1e1 3988 5711 a805 4b84 4e85 eab8 805f  ..9.W...K.N...._
-00002ec0: 0a15 ce99 5b8a edb9 8aaa 506e 2b78 1ac2  ....[.....Pn+x..
-00002ed0: 8211 1900 eb58 09d4 811a 2c16 4c22 03b8  .....X....,.L"..
-00002ee0: 75d4 12c1 880c 00cf 4458 30ea 381b e4d4  u.......DX0.8...
-00002ef0: d633 6a8f 9fd5 ea12 19c0 2da7 9608 4664  .3j.......-...Fd
-00002f00: 0078 32c2 8211 1900 6b73 0954 4736 b29e  .x2.....ks.TG6..
-00002f10: 4964 00b7 aa5a 2218 9101 e0f9 080b 4664  Id...Z".......Fd
-00002f20: 00a8 2166 3d23 b89d d319 858a 56b3 5b5c  ..!f=#......V.[\
-00002f30: 2d11 8cc8 0058 4c50 28b6 2dac 3726 501d  -....XLP(.-.7&P.
-00002f40: a9d5 7a26 9101 dc6a 6d89 6044 06c0 9a82  ..z&...jm.`D....
-00002f50: 4202 6ec1 3222 eb19 f106 1fa9 d582 113b  B.n.2".........;
-00002f60: 0c61 cfe4 3200 a1f1 5658 5a50 a016 d650  .a..2...VXZP...P
-00002f70: 13a8 8ed4 6ac1 2432 80a4 1a9c 907a 2bac  ....j.$2.....z+.
-00002f80: 3028 500b 6abd 59cf 8882 f80e 199c 0523  0(P.j.Y........#
-00002f90: 5061 cfe4 3200 a1f8 5658 6850 a016 d685  Pa..2...VXhP....
-00002fa0: 13a8 8e79 8205 93c8 0072 da70 d60b 4218  ...y.....r.p..B.
-00002fb0: 184b 1c15 6a41 fdba 53a1 3ae6 09a6 27ca  .K..jA..S.:...'.
-00002fc0: 570c 3380 9c44 9cf5 8208 8664 0705 6a21  W.3..D.....d..j!
-00002fd0: ad3b d5d6 812f f82d 9844 0670 abb1 3d5f  .;.../.-.D.p..=_
-00002fe0: cd84 785b c10a f857 11a8 05f7 c2ac 6754  ..x[...W......gT
-00002ff0: 0600 8f13 164c 2203 b845 d912 c188 0c00  .....L"..E......
-00003000: ebe0 2d18 9101 907e 9f42 7516 1915 6dc5  ..-....~.Bu...m.
-00003010: c32c b707 20a4 dc0a 56c3 5b30 2203 c027  .,.. ...V.[0"..'
-00003020: 15eb 19f1 c61f 931e eb99 c41e c02d f696  .............-..
-00003030: e819 9101 9024 6111 0a72 0b69 122a d481  .....$a..r.i.*..
-00003040: d524 164c 2203 c8a9 c859 2f88 0580 f600  .$.L"....Y/.....
-00003050: 046a 4106 b19e 1119 00ab c00a 543c cc72  .jA.........T<.r
-00003060: 1980 508a 2b24 5058 046a 219d 4585 ea98  ..P.+$PX.j!.E...
-00003070: c159 cf24 3280 9ca6 5c11 a272 8574 0a15  .Y.$2...\..r.t..
-00003080: 6ac1 0164 3d23 eaf9 58d9 56a0 e29e c965  j..d=#..X.V....e
-00003090: 0042 f2ad 905c a1f5 150d c685 b423 15ea  .B...\.......#..
-000030a0: 4094 f54c 2203 c8a9 cc59 2ff0 9cc1 8af9  @..L"....Y/.....
-000030b0: 9742 2d9d de02 88b6 3aa6 a3a6 c59d c800  .B-.....:.......
-000030c0: 6e3d b7e7 ab99 907f 2b58 376f c188 3d00  n=......+X7o..=.
-000030d0: d2c3 54a8 ced2 c3a2 ad70 98dd aa6e 8960  ..T......p...n.`
-000030e0: c41e 0056 cf5b 3062 0f00 eb07 4d24 5d64  ...V.[0b....M$]d
-000030f0: 0098 8e5a cf24 3280 5bdb 2d11 8cc8 00b0  ...Z.$2.[.-.....
-00003100: 86de 8211 1900 697c 2a54 6739 65d1 56dc  ......i|*Tg9e.V.
-00003110: 33b9 0c40 08c2 15ac a4b7 6044 0680 a532  3..@......`D...2
-00003120: d633 82db 7166 59cf 2432 805b e72d d133  .3..qfY.$2.[.-.3
-00003130: 2203 c07a 7a0b 46bc 0520 dd52 85ea 5461  "..zz.F.. .R..Ta
-00003140: a550 71cf e4de 0208 05b9 8255 f516 0c73  .Pq........U...s
-00003150: fb82 6533 d633 2203 a0f7 cc0a 1507 93cb  ..e3.3".........
-00003160: 0084 445c 2199 c3a2 24e9 a8f4 4da1 3abf  ..D\!...$...M.:.
-00003170: 9f11 6dc5 c1e4 de02 08a1 b842 6287 d657  ..m........Bb..W
-00003180: 4c9a a404 aa50 9ddf 0288 b6e2 6072 1980  L....P......`r..
-00003190: d094 2b24 7968 7d25 8241 2531 85ea bcd7  ..+$yh}%.A%1....
-000031a0: 2cda 0a83 c929 d459 2f70 0640 c287 0ab5  ,....).Y/p.@....
-000031b0: 902a a842 75de 9d11 578c 83c9 d501 08e9  .*.Bu...W.......
-000031c0: b842 f287 d657 a267 e86b 1602 7560 9e60  .B...W.g.k..u`.`
-000031d0: 1fe5 48ec 01dc 8a70 cf97 6621 2057 4804  ..H....p..f! WH.
-000031e0: b108 d48a 9535 f681 1191 01f0 8686 40c5  .....5........@.
-000031f0: 3d93 ab03 1032 7285 a410 adaf a867 56d2  =....2r......gV.
-00003200: 0955 a8ce 4f9a a2ad 3898 5c06 20c4 e40a  .U..O...8.\. ...
-00003210: d6e0 beac af44 3054 07a0 d4eb f811 40a0  .....D0T......@.
-00003220: e260 7275 0042 52ae 902c a2f5 9508 86be  .`ru.BR..,......
-00003230: 3aa2 34ec 389d 11a8 3898 5c06 2084 e50a  :.4.8...8.\. ...
-00003240: 8923 5a5f 8960 a80e 4029 d989 0520 f116  .#Z_.`..@)... ..
-00003250: e0d6 8b4b 2c00 a20e 8024 12ad af44 30f4  ...K,....$...D0.
-00003260: 2515 a567 870f 0ab6 9a25 f600 6ed5 b844  %..g.....%..n..D
-00003270: 30cc ed78 d4c8 7a8a 42e1 0315 0a85 c7f0  0..x..z.B.......
-00003280: 14a6 4cb5 a7ae 90bf dcc2 7189 4898 d869  ..L.......q.H..i
-00003290: 9749 69d1 7175 9692 b5c3 8f78 0a4c 1c49  .Ii.qu.....x.L.I
-000032a0: 4ed7 ceda 11f7 1bbf eba6 409c 610a 149f  N.........@.a...
-000032b0: ae50 17fc 4130 39ee 1782 7385 242c ed2f  .P..A09...s.$,./
-000032c0: 62b6 50a1 c993 b6ec 5356 e28d 4338 c86e  b.P.....SV..C8.n
-000032d0: 21b9 e783 4ce8 ce15 52b2 b4bf 8868 28c7  !...L...R....h(.
-000032e0: 5442 77f8 5c6d d188 0d87 389a 1cfb 0b05  TBw.\m....8.....
-000032f0: ba42 8296 f617 110d 6d33 0954 a78f 7ca8  .B......m3.T..|.
-00003300: b67e 30d2 72f4 2fb4 e80a e95a da5f 4434  .~0.r./....Z._D4
-00003310: fccd 3451 50c0 a5b3 f28a d11b cd5b 642e  ..4QP........[d.
-00003320: 31d2 c40e 00c9 5b16 a55c 4712 b60a d571  1.....[..\G....q
-00003330: 9fc0 469a ba62 184d 2e01 10d2 7485 542e  ..F..b.M....t.T.
-00003340: ed2f dc37 a464 ab50 9d3e c4a2 503f 1869  ./.7.d.P.>..P?.i
-00003350: b93d 00a1 5057 48ec d2fe 22a2 a144 53a0  .=..PWH..."..DS.
-00003360: 3aae e3d6 3722 e788 5781 dc26 8010 aa2b  :...7"..W..&...+
-00003370: 5858 f9b2 bf88 6828 d314 a88e 5b05 168d  XX....h(....[...
-00003380: 283e 8ca3 c9ed 0208 bdba 8295 9516 0d27  (>.............'
-00003390: 0b2b c9db 2a54 c76f 8758 34a2 fa30 8c26  .+..*T.o.X4..0.&
-000033a0: a791 5784 6c9d fd0d 7301 256e 472a b7aa  ..W.l...s.%nG*..
-000033b0: ad8e 9b05 97bc 621c 4d2e 1710 ea75 8584  ......b.M....u..
-000033c0: 24ed 2f62 a451 2e20 501d 8fe0 5834 995c  $./b.Q. P...X4.\
-000033d0: e056 a57b be42 0b11 bb82 05e5 f671 4b91  .V.{.B.......qK.
-000033e0: 0b90 e6ad 421d b85d 60d1 6472 815b 9c2e  ....B..]`.dr.[..
-000033f0: 118d 7817 40b2 9245 29de 9158 a942 1db8  ..x.@..E)..X.B..
-00003400: 5f60 d188 2bc6 232d 970b 0849 bb82 756f  _`..+.#-...I..uo
-00003410: d637 2217 20cd 5285 3af0 488e 45a3 3286  .7". .R.:.H.E.2.
-00003420: 883d 6fa9 ba44 df08 6626 91c9 a2f4 ef48  .=o..D..f&.....H
-00003430: ba54 a10e 3c93 63d1 6472 815b b12e 118d  .T..<.c.dr.[....
-00003440: 2808 c0ca 37eb 1b91 0b90 82a9 421d f8b1  (...7.......B...
-00003450: 118b 465c 311e 69b9 5c40 e8dc 15ac 16b3  ..F\1.i.\@......
-00003460: 6844 2e40 42a6 0a75 e037 472c 9a4c 2e70  hD.@B..u.7G,.L.p
-00003470: ebd7 25fa 4630 3329 4f16 258a 477a a60a  ..%.F03)O.%.Gz..
-00003480: 75e0 b11c 8b26 930b dc32 7689 6804 3393  u....&...2v.h.3.
-00003490: 0065 51da 78fc 8974 25b3 87e7 722c 9a4c  .eQ.x..t%...r,.L
-000034a0: 2e90 53da 2b42 fcce fe86 b980 92c8 2375  ..S.+B........#u
-000034b0: 53d5 d681 1f22 b9e4 15c3 7973 8bda 3def  S...."....ys..=.
-000034c0: 1ba1 8157 b0c8 ca3e aa2c 7201 1239 55a8  ...W...>.,r..9U.
-000034d0: 03bf 4762 d164 7281 5bdb 2e11 8d60 662c  ..Gb.dr.[....`f,
-000034e0: 4cb2 6844 2e40 5aa7 0a75 e033 9d45 93c9  L.hD.@Z..u.3.E..
-000034f0: 056e 89bb 4434 cccc b429 2854 f3c4 a6a0  .n..D4...)(T....
-00003500: 40d1 a6a0 c094 a90e ca6f 0ade 2a77 8948  @........o..*w.H
-00003510: 4429 1fcd 18c6 b0d6 4a11 f27a f885 2485  D)......J..z..$.
-00003520: f941 24b9 f701 4a17 8f3e f05b 248a 7637  .A$...J..>.[$.v7
-00003530: 9410 1f57 380b d40f a2c9 ed07 2879 3c2e  ...W8.......(y<.
-00003540: 3d93 28fa 32bc d2e3 e312 6781 fa41 34b9  =.(.2.....g..A4.
-00003550: 1c40 a8e4 7119 8d02 f186 ad52 e5e3 538e  .@..q......R..S.
-00003560: 02f5 8360 72db 0142 2bcf 0636 4d1a b11d  ...`r..B+..6M...
-00003570: 409a ae45 89f3 f131 4779 c5f7 d602 2c00  @..E...1Gy....,.
-00003580: b9ed 0021 9967 9384 a211 db01 24ed 5a94  ...!.g......$.Z.
-00003590: 461f 1f0d 9457 8ca2 c9c9 f415 a19c 57b0  F....W........W.
-000035a0: fced a550 2b29 bc2a d4c1 6703 e515 c368  ...P+).*..g....h
-000035b0: 72db 0142 40af 90ce 6b51 327b 24f4 aa50  r..B@...kQ2{$..P
-000035c0: 076e 1d5e 0a15 cf9b 5b18 ef39 d508 1d3d  .n.^....[..9...=
-000035d0: 1bff 38d2 94da 1ee9 bd16 25dc 8767 402d  ..8.......%..g@-
-000035e0: 1a95 7484 7d93 7b35 20e4 f46c fc53 34e2  ..t.}.{5 ..l.S4.
-000035f0: d500 c9be 16a5 df87 8740 2d1a b11d 10a6  .........@-.....
-00003600: 01b7 4c5e a26f c4c3 3989 bf16 a5bd 47ea  ..L^.o..9.....G.
-00003610: af0a 75e0 d6a1 4523 ae18 4793 4b05 84b8  ..u...E#..G.K...
-00003620: 9e8d 6cea 1b51 1a40 22b0 45a9 f9e1 d6a1  ..l..Q.@".E.....
-00003630: 4523 b603 e268 72a9 8090 d9b3 914d d188  E#...hr......M..
-00003640: ed00 d282 2d4a b20f b7e4 2c1a b11d 1047  ....-J....,....G
-00003650: 934b 0584 e09e 8d6c 8a46 6c07 9024 6c51  .K.....l.Fl..$lQ
-00003660: e27d 7cac 565d 318e 2697 0b08 dd3d 1bd9  .}|.V]1.&....=..
-00003670: 148d c805 4819 b628 0d3f 3ca3 6b7d 23b6  ....H..(.?<.k}#.
-00003680: 03e2 6872 b980 90df b391 4dd1 885c 8094  ..hr......M..\..
-00003690: 558b 140e c42f bf2a 54cc 3739 c9bf 2254  U..../.*T.79.."T
-000036a0: f86c 6463 3402 b592 c0aa 6aeb e063 c2ea  .ldc4.....j..c..
-000036b0: 8a61 dfdc ea7a cf57 6821 c667 e39f a211  .a...z.Wh!.g....
-000036c0: db01 a4b3 5a94 b01f 6e52 5f0a f583 be19  ....Z...nR_.....
-000036d0: 549b 8846 3033 165c bd8a 50ee 5b49 6e55  T..F03.\..P.[InU
-000036e0: a10e dca4 b668 32b9 c0ad b597 8846 3033  .....h2......F03
-000036f0: 69c7 1621 e0b7 924c a642 1d7c 865b b4f5  i..!...L.B.|.[..
-00003700: 83be c9bd 1a10 0a7d 36fe 69a4 8957 03a4  .......}6.i..W..
-00003710: 9659 a4b6 206d 70a8 2bc6 f326 970b 0ca1  .Y.. mp.+..&....
-00003720: be3f 7ef9 f2ed cbd7 9fff fc7a f0b3 00d8  .?~........z....
-00003730: 4987 02ec 9045 d8b8 62e6 8f3e b458 6eb5  I....E..b..>.Xn.
-00003740: bdc4 b032 1a9e 5ce7 c9ee edf4 e67c 5c6e  ...2..\......|\n
-00003750: fa3d 7e77 f42f 77bc 485a ec7a 8ee5 8720  .=~w./w.HZ.z... 
-00003760: df74 69ca f2c1 4e35 8c60 070e b2bb cef9  .ti...N5.`......
-00003770: 41ec 7a8e d287 06df 77d7 2beb 4a38 fb4a  A.z.....w.+.J8.J
-00003780: caaa c5d9 0fae 5772 f6e9 19da 3fc5 df32  ......Wr....?..2
-00003790: 7b89 a162 9c3c 39cd f77b b6af a4a3 5ac6  {..b.<9..{....Z.
-000037a0: e5de fdc5 6549 ce1e 395d 7352 7e37 7c72  ....eI..9]sR~7|r
-000037b0: 1a1f 9ebc 7d25 d554 b4a3 388c b7c7 4ea7  ....}%.T..8...N.
-000037c0: 9ec9 eb10 d07b 3b4d 7a10 debe 92b8 a8b7  .....{;Mz.......
-000037d0: 1f54 64e4 edb1 d329 baad 439a 6f72 1a1f  .Td....)..C.or..
-000037e0: 85bc 7d25 2951 b4e3 74f4 f6d8 e9d4 1376  ..}%)Q..t......v
-000037f0: 1d82 7893 d3f8 c4e3 ed2b 096e a21d 734f  ..x......+.n..sO
-00003800: 6f8f 9d4e 9167 1dc2 7793 d3f8 60e3 ed2b  o..N.g..w...`..+
-00003810: 6e5c 9e68 47b9 036f 8f9d 4e71 641d 0277  n\.hG..o..Nqd..w
-00003820: 93d3 f8fc e2ed 2bd5 03a3 1d39 d2db 63a7  ......+....9..c.
-00003830: 538f c575 88e2 4d4e e363 8ab7 af24 6488  S..u..MN.c...$d.
-00003840: 7664 476f 8f9d 4ef1 621d 8275 d33a cb77  vdGo..N.b..u.:.w
-00003850: dadb b11c 1e7f 8f99 94b7 c74e a718 b10e  ...........N....
-00003860: 29bc e94e e323 94b7 af24 4c88 765e 3de6  )..N.#...$L.v^=.
-00003870: f663 a753 cfb2 7508 d04d 4e63 f2e4 ed2b  .c.S..u..MNc...+
-00003880: 69f6 a19d 578f b9fd d0e9 9cb4 5d1d f0c9  i...W.......]...
-00003890: 69a4 716f 5f49 ce0e edb4 7ab8 f663 a773  i.qo_I....z..c.s
-000038a0: 8c38 04e5 26a7 89c6 9d7d c517 f267 053b  .8..&....}...g.;
-000038b0: ad1e ce1e 3b9d 63c4 212f 374d 441a 1e60  ....;.c.!/7MD..`
-000038c0: c76a ee0a 76be d373 fbb1 d339 461c 0271  .j..v..s...9F..q
-000038d0: ef3b 4daf 03ab b3af a4dc 8676 5af2 dcef  .;M........vZ...
-000038e0: 63a7 738c 3884 e026 a729 f770 f695 44cd  c.s.8..&.).p..D.
-000038f0: 2ad8 69f5 70f6 d8e9 1c23 0ec1 b7c9 69ca  *.i.p....#....i.
-00003900: 3d9c 7d25 bdaf 0a76 5a3d 9c3d 763a c788  =.}%...vZ=.=v:..
-00003910: 43d8 6d72 9a72 0f67 5f49 0aab 829d c7f4  C.mr.r.g_I......
-00003920: dc7e ec74 8e11 8780 dbe4 3431 a2b3 afa4  .~.t......41....
-00003930: 1265 0f68 d3ef 573a 1cee edb1 d339 461c  .e.h..W:.....9F.
-00003940: 426d 93d3 947b 38fb 4a02 4ad5 d94d 601c  Bm...{8.J.J..M`.
-00003950: 761d 2e0f 88bd ce51 e250 649b bc26 1e77  v......Q.Pd..&.w
-00003960: f695 9492 2ad8 51be cedb 43a7 735a 6f75  ....*.Q...C.sZou
-00003970: c027 a769 a176 f695 4484 fcef 573a 6eeb  .'.i.v..D...W:n.
-00003980: edb1 d339 4a1c 0a6b 93d3 c4e3 cebe 92be  ...9J..k........
-00003990: 4e75 761b 1fc4 890e 107b 9de3 c421 a536  Nuv......{...!.6
-000039a0: 794d 44ee ec2b 09e9 5467 37af e981 dc01  yMD..+..Tg7.....
-000039b0: 62af 73a4 3834 d3de 5e93 3843 75f6 9514  b.s.84..^.8Cu...
-000039c0: 73c0 4e67 4bbd 3d76 3a47 8a43 1b6d 729a  s.NgK.=v:G.C.mr.
-000039d0: 48d1 d957 1293 a960 e73b 3db7 1f3b 9d23  H..W...`.;=..;.#
-000039e0: c5a1 8136 394d a4e8 ec2b e9ac 54b0 d3fa  ...69M...+..T...
-000039f0: e1ec b1d3 3952 1c5a 6793 d344 8ace be52  ....9R.Zg..D...R
-00003a00: bd51 7576 1bd4 9434 3940 ec75 8e15 87a8  .Quv...49@.u....
-00003a10: d9e4 35b1 a2b3 afa4 3552 9ddd bce6 7b3d  ..5.....5R....{=
-00003a20: 5f20 f63a 478b 43bd 6cf2 9a68 d1d9 573c  _ .:G.C.l..h..W<
-00003a30: 2874 5667 37af 29d7 7380 d8eb 1c2d 0e99  (tVg7.).s....-..
-00003a40: b2c9 6ba2 4567 5f49 3da4 3abb 794d 0fe5  ..k.Eg_I=.:.yM..
-00003a50: 0e10 7a9d 5340 ab03 3e79 4dbc e8ec 2b1e  ..z.S@..>yM...+.
-00003a60: fc39 fdef cd6b 4a51 5d03 b1d7 3962 1cc2  .9...kJQ]...9b..
-00003a70: 6393 d744 8cce be91 1e48 053b f1a2 b3c7  c..D.....H.;....
-00003a80: 4ee7 7871 088c 4d4e 132f 3afb 86b4 67b7  N.xq..MN./:...g.
-00003a90: 7afe fdc6 2b88 b3c7 4ee7 6871 0889 bd9d  z...+...N.hq....
-00003aa0: c61d ff57 75f6 0d17 0873 7afe fdc6 53d1  ...Wu....sz...S.
-00003ab0: d963 a773 b438 04c3 26a7 8916 9d7d c399  .c.s.8..&....}..
-00003ac0: 664e cfbf dfc4 987e 448b 3929 b23a e093  fN.....~D.9).:..
-00003ad0: d344 8bce bee1 2102 737a fefd 4665 f9de  .D....!.sz..Fe..
-00003ae0: 1edf e91c 2d0e 99b0 c969 a245 67df e8c4  ....-....i.Eg...
-00003af0: 7475 765b 3eb0 d4db 0362 af73 b438 94be  tuv[>....b.s.8..
-00003b00: 26af 8916 9d7d a393 d115 ec94 3639 7bec  &....}......69{.
-00003b10: 748e 1587 a2d7 e434 b1a2 b36f 58f7 67e3  t......4...oX.g.
-00003b20: 63fe fd46 9574 de1e 3b9d 23c5 a1dc 3539  c..F.t..;.#...59
-00003b30: 4da4 e8ec 1b9d a5ad ce6e e383 3613 1c20  M........n..6.. 
-00003b40: f43a 270a 5607 7cf2 9a48 d1d9 372c ae3a  .:'.V.|..H..7,.:
-00003b50: fdef 377c f77b 797b ec74 8e13 8714 d7e4  ..7|.{y{.t......
-00003b60: 3471 a2b3 6f74 98b4 829d eeb4 b3c7 4ee7  4q..ot........N.
-00003b70: 3871 486e 4d4e 1327 3afb 46a7 2c2b d889  8qHnMN.':.F.,+..
-00003b80: c89d 3d76 3ac7 8943 5aeb ed34 1d13 afce  ..=v:..CZ..4....
-00003b90: bed1 f143 b4d3 a380 fb7d ec74 8e13 8784  ...C.....}.t....
-00003ba0: d6e4 3471 a2b3 6f74 2eaf 829d 726a 678f  ..4q..ot....rjg.
-00003bb0: 9dce 3d2a 0ea9 acc9 69e2 4467 dfe8 c05a  ..=*....i.Dg...Z
-00003bc0: 053b 25a7 ce1e 3b9d e3c4 219c 3539 4d9c  .;%...;...!.59M.
-00003bd0: e8ec 1b9e 2db2 d563 fefd 86aa d7b6 7a3c  ....-..c......z<
-00003be0: da3f cd89 6dd5 019f 9c26 4a74 f60d df19  .?..m....&Jt....
-00003bf0: 98d3 f3ef 3714 8436 a71f 3d28 e644 b5ea  ....7..6..=(.D..
-00003c00: 804f 4e13 253a fb46 c766 fcef b7a9 ffff  .ON.%:.F.f......
-00003c10: fac8 99b7 c7c3 2347 8943 d16a 729a 28d1  ......#G.C.jr.(.
-00003c20: d937 3a4f 52c1 ce13 f1d1 1bc5 9c54 561d  .7:OR........TV.
-00003c30: f0c9 6962 4467 dfe8 a085 fffd 8647 172e  ..ibDg.......G..
-00003c40: 6f0f eff4 ad38 f5b8 9aa9 0ef8 77a7 e933  o....8......w..3
-00003c50: 45de dce8 7b8b 68a7 2ccf 351f fb9c 23c4  E...{.h.,.5...#.
-00003c60: 2143 35dd 6862 7167 dfe8 d444 053b b1b8  !C5.hbqg...D.;..
-00003c70: b3c7 4ee7 0871 6852 4d4e 138b 3bfb 46c7  ..N..qhRMN..;.F.
-00003c80: 092a d889 c59d 3d76 3a47 8843 54ea ed34  .*....=v:G.CT..4
-00003c90: 1df0 aece be51 9d3d da89 c5dd ef63 a773  .....Q.=.....c.s
-00003ca0: 8438 b4a3 26a7 89c5 9d7d a302 f40a 765a  .8..&....}....vZ
-00003cb0: 3c9c 3d76 3a47 8843 6e6a 729a 58dc d937  <.=v:G.Cnjr.X..7
-00003cc0: aacc ae60 2716 77f6 d8e9 dc33 e250 829a  ...`'.w....3.P..
-00003cd0: 9c26 1677 f68d 4a96 2bd8 7922 3e22 c45b  .&.w..J.+.y">".[
-00003ce0: c129 b1e2 cd84 681f e9c5 72eb 3ada 7b2f  .)....h...r.:.{/
-00003cf0: 891f fc68 8b00 5ef5 1e55 d9dc 5a4d 09bf  ...h..^..U..ZM..
-00003d00: 1d27 d229 d83a 9afb eef6 4675 a768 e705  .'.).:....Fu.h..
-00003d10: e411 27e6 34a3 ea80 4f23 84b2 0f67 dfe8  ..'.4...O#...g..
-00003d20: 33f7 fef7 1b7d fcda dbc3 617d 2b2f 3dbf  3....}....a}+/=.
-00003d30: d303 3e39 4dd9 87b3 6f5c c209 765a 409c  ..>9M...o\..vZ@.
-00003d40: 3d76 3a47 8a43 8f69 729a b20f 67df b884  =v:G.C.ir...g...
-00003d50: 13ec b480 387b ec74 8e14 87ec d23c d568  ....8{.t.....<.h
-00003d60: 0541 0056 af57 04f0 cd9e 2f11 fb9d e3c5  .A.V.W..../.....
-00003d70: 21b0 34dd 6cca 409c 7de3 d253 b0d3 c2e7  !.4.l.@.}..S....
-00003d80: ecb1 d339 5e1c 3a4a 93d3 9481 38fb c6a5  ...9^.:J....8...
-00003d90: a760 a705 c4d9 63a7 73bc 38e4 92e6 11c2  .`....c.s.8.....
-00003da0: 9311 0030 70cf 8a2d d0f6 a903 c47e e7a8  ...0p..-.....~..
-00003db0: 7108 23cd 7ef3 ddf6 00de b681 1650 6fea  q.#.~........Po.
-00003dc0: aa0e 10fb 9ddb 411d 1248 ef41 42e7 92ab  ......A..H.AB...
-00003dd0: b36f 5cea 0b76 caf8 9c3d 763a f7b8 3894  .o\..v...=v:..8.
-00003de0: 8e26 a729 e373 f68d ab66 c1ce 6bc8 236a  .&.).s...f..k.#j
-00003df0: cc49 28d5 019f 4608 6e81 bd08 00f7 f224  .I(...F.n......$
-00003e00: 00bd 7976 9708 6f76 4e2c a90e f8ec 3771  ..yv..ovN,....7q
-00003e10: 3a02 502e 915a 20ae 712d c47e e708 7288  :.P..Z .q-.~..r.
-00003e20: 144d 8384 326c 67df b84a 19ec ecf4 a332  .M..2lg..J.....2
-00003e30: d49c fa51 1df0 c969 e247 67df b84a 19ec  ...Q...i.Gg..J..
-00003e40: 4434 ce1e dfe9 1c3b 0e79 a279 8410 3d22  D4.....;.y.y..="
-00003e50: 00dc b291 ed5b c0ad b4cb 0362 bf73 0439  .....[.....b.s.9
-00003e60: 4486 a69b 4dfb 7bce be71 75b5 b397 0fde  D...M.{..qu.....
-00003e70: e073 80d8 eb1c 430e 31a1 f7dd e67b ed76  .s....C.1....{.v
-00003e80: 42f1 78ab dd6a 6fa7 8a0a 6f7f 0f40 7786  B.x..jo...o..@w.
-00003e90: aede 2240 cf33 ec01 7ffb 4cdc e8cc 0dd5  .."@.3....L.....
-00003ea0: a0cc 67f7 5c48 fa4a 600f 7dce 31e3 5006  ..g.\H.J`.}.1.P.
-00003eb0: 7a8f 0e7a 6a74 e646 5f8c afde 4edf 2305  z..zjt.F_...N.#.
-00003ec0: 7be8 738e 1887 fecf db67 e245 676e f42d  {.s......g.Egn.-
-00003ed0: f50a 767a cef5 f6c8 e79c ae50 1df0 b7cf  ..vz.......P....
-00003ee0: b4e2 3973 a36f 59fb 9f37 fa1e 1fd8 439f  ..9s.oY..7....C.
-00003ef0: 73ef 1587 2ed0 b472 1025 3afb c637 1aec  s......r.%:..7..
-00003f00: 74a3 9d3d 5c38 7222 4175 c0df 9390 1e18  t..=\8r"Au......
-00003f10: 9db9 a1d6 c7e9 7fde 48a1 01ec e18d ce3d  ........H......=
-00003f20: 300e 619e e946 d3d3 80b3 6ff4 0dfa 0a76  0.a..F....o....v
-00003f30: ca98 9c3d bed1 393e 1cfa 3b93 d37c a75d  ...=..9>..;..|.]
-00003f40: 298d 18d2 de4e 4bb4 6b3f 763a 4786 4366  )....NK.k?v:G.Cf
-00003f50: 6772 9a78 c5d9 37fa 7279 053b 3d75 397b  gr.x..7.ry.;=u9{
-00003f60: ec74 8e0b 879a cee4 3411 8bb3 6ff4 51ef  .t......4...o.Q.
-00003f70: eaed f42d 3f6f 8f9d ce3d 2a0e d19c b7d3  ...-?o...=*.....
-00003f80: 24ff 509d 7da3 ef5d a39d 178f 47bb a8b7  $.P.}..]....G...
-00003f90: d8cd 7306 1ff0 c969 a216 67df f880 03d8  ..s....i..g.....
-00003fa0: 7922 3eda 42bd 956f 124e 3b3a c4a3 f7af  y">.B..o.N;:....
-00003fb0: 3a9a fb1e d4c6 071c c0ce 13f1 d173 624e  :............sbN
-00003fc0: 5ba7 0ef8 74a7 8910 9d7d e303 0e60 a789  [...t....}...`..
-00003fd0: e8ec e198 ce49 e8d4 019f 9ca6 54da d937  .....I......T..7
-00003fe0: 3e29 e0ed 7c52 c0d9 63a7 734f 8843 b766  >)..|R..c.sO.C.f
-00003ff0: 729a 58dc d937 3e29 0076 9a88 ce1e 3b9d  r.X..7>).v....;.
-00004000: 63c4 214f 3339 4d8c e8ec 1b9f 1400 3b4d  c.!O39M.......;M
-00004010: 4467 8f9d ce31 e250 a199 9c26 4674 f68d  Dg...1.P...&Ft..
-00004020: 4f0a 809d 26a2 b3c7 4ee7 18d1 c9d3 542c  O...&...N.....T,
-00004030: 4e7f 5567 dfb8 e41e ec3c 1167 c68d 9dce  N.Ug.....<.g....
-00004040: 31a2 13a6 a958 9b6e 4ebb 421a ae5d 77f6  1....X.nN.B..]w.
-00004050: 9d4f cf39 7bec 748e 119d 244d c38b 9ad3  .O.9{.t...$M....
-00004060: 33a3 edf4 f547 b4f3 447c c488 433d e6b9  3....G..D|..C=..
-00004070: ce96 0d88 694c 3774 ca9c 9eed 3b96 a69f  ....iL7t....;...
-00004080: 68e7 89f8 8811 7362 3636 209c d3b4 29e6  h.....sb66 ...).
-00004090: ec3b 96a6 9bd3 f3ef 773e 8ff1 48cc c67a  .;......w>..H..z
-000040a0: 3873 a76f f8f7 d5a3 e19d 7c79 fb8e a5e9  8s.o......|y....
-000040b0: 27da 7122 42fb c193 8bf5 70ce e999 111b  '.q"B.....p.....
-000040c0: 1e02 30a7 67fb 8e45 bce6 b4b3 9306 bbb7  ..0.g..E........
-000040d0: 4713 b10d 759a e763 fa86 4f77 1a19 d1db  G...u..c..Ow....
-000040e0: 777a 538e 769c 88d0 7e78 a753 8c68 03c2  wzS.v...~x.S.h..
-000040f0: 8d69 6444 6fdf a908 1ced 3811 a1fd d0e9  .idDo.....8.....
-00004100: 1423 da80 704e 2323 7afb 4e45 e068 4746  .#..pN##z.NE.hGF
-00004110: 84f6 43a7 538c d89c 984d c383 0936 a667  ..C.S....M...6.g
-00004120: 46db e94b 4368 e789 f884 11db 50a7 c98c  F..KCh......P...
-00004130: 69b7 e189 13cd 9c9e ed3b 7d82 07ec f8de  i........;}.....
-00004140: eef2 f678 22a6 18b1 3931 9b46 352b debe  ...x"...91.F5+..
-00004150: d3b7 69d0 ce13 f109 235a 0fe7 eeb4 632c  ..i.....#Z....c,
-00004160: 5c1d ec4e 3b46 a48f b6a0 9d27 e213 466c  \..N;F.....'..Fl
-00004170: 439d 2633 3c1c 23a2 d0b5 39ed 188f be66  C.&3<.#...9....f
-00004180: 8276 9e88 4f9e 11ad 8753 4e7b b119 5cd2  .v..O....SN{..\.
-00004190: 5e77 73df d7f1 9d3e f381 769a 888f c46c  ^ws....>..v....l
-000041a0: da50 8f49 dc69 2f36 8387 6dcc 69c7 7858  .P.I.i/6..m.i.xX
-000041b0: e37d 829d de11 797b 3811 87ba 4cc6 69f7  .}....y{8...L.i.
-000041c0: 960f d761 737a b6ef f80a c89c f676 9a88  ...asz.......v..
-000041d0: ce1e 3b9d 6344 2f36 4355 becd d9f7 e9aa  ..;.cD/6CU......
-000041e0: 778d b739 3d33 ea8e e5d6 97b7 c74e e718  w..9=3.......N..
-000041f0: d18b cd90 3864 73f6 9d54 f8d1 4e13 f191  ....8ds..T..N...
-00004200: 984d 1bea 3199 e1e1 180b 0f10 d9f0 708c  .M..1.........p.
-00004210: 48f2 f468 e789 f888 1187 ba4c c669 c788  H..h.......L.i..
-00004220: c878 e6b4 6344 d26d 073b 962e dbf0 70ed  .x..cD.m.;....p.
-00004230: 47b9 c750 97c9 38ed 188b c421 9b13 abd9  G..P..8....!....
-00004240: 49d0 1ced 3c11 1f31 e250 97c9 38ed 180b  I...<..1.P..8...
-00004250: 69da eeb4 6344 52fa 463b 31a2 fb7d 3c11  i...cDR.F;1..}<.
-00004260: 738c e8b4 681a d5a9 3467 df49 021b ed3c  s...h...4g.I...<
-00004270: 111f 3162 4ecb a639 ad9a 86b9 c5cb db77  ..1bN..9.......w
-00004280: d286 463b 4d44 df7e 34a6 8776 4c62 7878  ..F;MD.~4..vLbxx
-00004290: a919 3c5f 664e 3b46 243d 5cb0 6309 f0e5  ..<_fN;F$=\.c...
-000042a0: ede1 f018 d231 19a7 1d23 6242 644e 3bc6  .....1...#bBdN;.
-000042b0: 2369 59b4 d344 7ca4 6463 3d9c 73da 3d23  #iY..D|.dc=.s.=#
-000042c0: e2a1 3873 da31 1e49 cba2 9d26 a2fb 7d7c  ..8s.1.I...&..}|
-000042d0: a773 8ce8 9468 1a66 71e6 f4fc 0cb9 e307  .s...h.fq.......
-000042e0: ba4f b4d3 44f4 ed87 633a c788 5e89 06cb  .O..D...c:..^...
-000042f0: 269a 33ef f8e1 6af3 d911 267d 7dca dbe3  &.3...j...&}}...
-00004300: 1b9d 2344 af33 435f 366b cebe e347 a4cc  ..#D.3C_6k...G..
-00004310: 6947 98f4 5926 6f8f 9dce 11a2 d3a1 6998  iG..Y&o.......i.
-00004320: 2edb e870 9ba6 7494 0bed 3c0f 1f11 e290  ...p..t...<.....
-00004330: 8dc9 2c1e fe11 8e87 8723 442a 4268 4ea5  ..,......#D*BhN.
-00004340: 66a7 2204 6f8f ef74 8e10 4164 06df 7dda  f.".o..t..Ad..}.
-00004350: bd9f f672 762a b942 3bcf c347 8498 13b1  ...rv*.B;..G....
-00004360: 6920 6203 df18 f0e6 46af f3d1 4e7c f848  i b.....F...N|.H
-00004370: c2a6 0dcd 98c4 e8f0 1236 b4fb e815 68e8  .........6....h.
-00004380: 6dfe 7db5 f7ee 25bd cd07 7bb4 de0d c998  m.}...%...{.....
-00004390: 8ccf ee25 226d 3e7a 011a 7a99 dfc0 4eb3  ...%"m>z..z...N.
-000043a0: f091 804d 1b8a 3119 9fdd 3b44 da7b f4fa  ...M..1...;D.{..
-000043b0: 33f4 2eff beda 749f 890c 1fe9 d7b4 2128  3.....t.......!(
-000043c0: 93f1 d96d 98e2 b9e5 d7dd dc7b cb83 6a08  ...m.......{..j.
-000043d0: d1ce 03da b7ff 7dbe b8ba c796 d3af b9e1  ......}.........
-000043e0: ef3b 850f dae6 b463 3b2a 2204 3b15 1162  .;.....c;*".;..b
-000043f0: fb91 d339 36f4 fa35 5808 d49c b951 d104  ...96..5X....Q..
-00004400: da69 b5f3 bf0f 6761 8e0c bd7a 0dd6 0135  .i....ga...z...5
-00004410: 2f3e 4335 1368 e7c1 f188 0b87 9a4c 6644  />C5.h.......LfD
-00004420: fb17 88b4 423b 3395 4c34 a75d d3a8 6402  ....B;3.L4.]..d.
-00004430: ece1 7dce 51a1 9796 2126 f466 aa98 6860  ..}.Q...!&.f..h`
-00004440: e7d5 ee11 13e6 946b 9a53 a6e1 85c3 9ba9  .......k.S......
-00004450: 6002 7e7e d06a e77f 1fdd e7a1 1493 181b  `.~~.j..........
-00004460: 202c 83f5 34cd d977 2a30 453b dde8 47c2   ,..4..w*0E;..G.
-00004470: 356d 28c5 649c f627 2288 bf9d f0cc 4ec5  5m(.d..'".....N.
-00004480: 9af7 e5de 4b38 9e78 bdbc 3d4c ee86 524c  ....K8.x..=L..RL
-00004490: c669 7f5e 9008 dc09 cfec 54ac d9c0 4ecb  .i.^......T...N.
-000044a0: dd23 e19a 3694 6232 4e7b b222 0677 c233  .#..6.b2N{.".w.3
-000044b0: 3b67 7760 a7f5 ee91 704d 1b4a 3119 a7fd  ;gw`....pM.J1...
-000044c0: 5e26 118b 139e d939 bdf3 764e ef1e 09d7  ^&.....9..vN....
-000044d0: b4a1 1493 71da ef65 12b3 38e1 999d f33b  ....q..e..8....;
-000044e0: b0f3 447c b457 9a13 ae69 5e58 8674 7bbd  ..D|.W...i^X.t{.
-000044f0: 7de7 04cf fd7e c78f 2eda 447c 4487 39e1  }....~....D|D.9.
-00004500: 9ae6 8469 6c01 433e 74f6 9df3 0eb0 f344  ...il.C>t......D
-00004510: 7cf4 f670 28c9 6486 8723 2c14 c478 3527  |..p(.d..#,..x5'
-00004520: 4cb3 73e2 0176 9e88 8f08 3127 5cd3 9c30  L.s..v....1'\..0
-00004530: 8d2d 6078 a79d 7de7 ccc3 d90f dcc3 b9a0  .-`x..}.........
-00004540: fd88 1173 c235 cd2b cba0 8ac7 cbdb 774c  ...s.5.+......wL
-00004550: 874e b4e3 6966 683f 743a c788 5e59 06b7  .N..ifh?t:..^Y..
-00004560: cacd 69b7 578a 05ca e6b4 b743 4fd9 9df6  ..i.W......CO...
-00004570: 8c1b e4ff 432a 2631 a6bd b20c 4a8f 98d3  ....C*&1....J...
-00004580: 6eaf 1413 2273 dadb f174 adb7 8734 3ea4  n..."s...t...4>.
-00004590: 6232 4e3b 46c4 fd7d 73da ed95 92aa 33da  b2N;F..}s.....3.
-000045a0: f1b4 a7b7 c74e e718 d12b cba0 5e8a 39ed  .....N...+..^.9.
-000045b0: 1e0f 491e 19ed 78da d3db 63a7 738c e895  ..I...x...c.s...
-000045c0: 65f0 a584 393d 335a 279d 61b4 f344 7cc4  e...9=3Z'.a..D|.
-000045d0: 8843 4a26 333c 1c63 9164 6f73 ca34 9d74  .CJ&3<.c.dos.4.t
-000045e0: 86d1 ce13 f111 23e6 946b 9ad3 9db1 058a  ......#..k......
-000045f0: d6e9 99d1 3ae9 0cfb df77 d219 86f6 c325  ....:....w.....%
-00004600: 2fc7 884e 96c6 1628 727a 66b4 4e3a c3cd  /..N...(rzf.N:..
-00004610: fdbe 93ce b0b7 8763 3a27 5bd3 9c2c 8d2d  .......c:'[..,.-
-00004620: 50e8 b4b3 77d2 19f6 bfef a4c8 0aed 4777  P...w.........Gw
-00004630: 3a27 5b63 ea6c 7309 21ca d2bc bcbd 93ce  :'[c.ls.!.......
-00004640: 30da 6922 3e92 ad69 4327 2631 11bd ac0c  0.i">..iC'&1....
-00004650: beb3 32a7 6746 eb58 8e75 a29d 26e2 23d9  ..2.gF.X.u..&.#.
-00004660: 1a3b dd98 73da 3d23 a296 8e39 3ddb 3b56  .;..s.=#...9=.;V
-00004670: 3699 d3de 4e8c e8ec f198 ce31 a2d7 aca1  6...N......1....
-00004680: 79e8 2567 f861 1cec b4ed f148 b2a6 0d8d  y.%g.a.....H....
-00004690: 98cc e870 8f88 9859 da8d 9eed 9d44 86d1  ...p...Y.....D..
-000046a0: 4e2c fe48 b2a6 0d81 988c d38e b0f0 95a5  N,.H............
-000046b0: 39ed 0891 4486 d14e 2cfe 63bd 9a9f befd  9...D..N,.c.....
-000046c0: e3f7 dfff b87e fde3 d7af ff07 0000 ffff  .....~..........
-000046d0: 0000 00ff ff4c 906f 4b03 310c c6bf 4ac8  .....L.oK.1...J.
-000046e0: fbb9 2bc3 89c7 3a10 87b0 1782 b04f 50bd  ..+...:......OP.
-000046f0: dcb5 7836 2597 f3cf c4ef 6e3a 1d9a 1769  ..x6%.....n:...i
-00004700: 9fd0 e6f9 259b 302b dfa5 5149 40a8 f778  ....%.0+..QI@..x
-00004710: e3da dd6a bd46 7897 764e 9dc7 cfe6 3716  ...j.Fx.vN....7.
-00004720: 76ba 9a9a 45e3 6afa 175f b8dc 6e4a e44c  v...E.j.._..nJ.L
-00004730: 9a9e 1e04 7ace bab7 cf0e 413f 0a79 cc7c  ....z.....A?.y.|
-00004740: cbf9 9564 4a9c 4f6f c340 f741 8694 2718  ...dJ.Oo.@.A..'.
-00004750: a957 8fcd c515 82a4 219e efca e554 bd44  .W......!....T.D
-00004760: 7864 557e 39ab 48a1 23a9 6a85 e6c4 c6fe  xdU~9.H.#.j.....
-00004770: 232a 83f5 3d90 ce05 4a28 2487 7434 f36b  #*..=...J($.t4.k
-00004780: 0496 4459 839a bdc7 c2a2 1292 2244 ab1f  ..DY........"D..
-00004790: 8d35 8cbb 92ac 0982 31da 087f 5ada ba04  .5......1...Z...
-000047a0: d977 ae62 2fdf 589e a748 a4db 6f00 0000  .w.b/.X..H..o...
-000047b0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-000047c0: 2100 0161 920c 3f03 0000 2b08 0000 1800  !..a..?...+.....
-000047d0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000047e0: 7368 6565 7433 2e78 6d6c 9c93 4d4f e330  sheet3.xml..MO.0
-000047f0: 1086 ef2b ed7f b07c 6f9c 045a 41d4 14ed  ...+...|o..ZA...
-00004800: 822a b8a0 d50a d8b3 eb4c 1aab fe08 b6d3  .*.......L......
-00004810: 0f21 fefb 8e5d 5a90 7aa9 8812 cf24 633f  .!...]Z.z....$c?
-00004820: 3313 bf9e de6c b522 6b70 5e5a 53d3 22cb  3....l."kp^ZS.".
-00004830: 2901 236c 23cd b2a6 cf4f f3d1 1525 3e70  ).#l#....O...%>p
-00004840: d370 650d d474 079e decc 7efe 986e ac5b  .pe..t....~..n.[
-00004850: f90e 2010 2418 5fd3 2e84 be62 cc8b 0e34  .. .$._....b...4
-00004860: f799 edc1 60a4 b54e f380 af6e c97c ef80  ....`..N...n.|..
-00004870: 3769 9156 accc f309 d35c 1aba 2754 ee1c  7i.V.....\..'T..
-00004880: 866d 5b29 e0ce 8a41 8309 7b88 03c5 03d6  .m[)...A..{.....
-00004890: ef3b d9fb 034d 8b73 709a bbd5 d08f 84d5  .;...M.sp.......
-000048a0: 3d22 1652 c9b0 4b50 4ab4 a81e 96c6 3abe  =".R..KPJ.....:.
-000048b0: 50d8 f7b6 b8e4 826c 1dde 253e 1787 34e9  P......l..%>..4.
-000048c0: fb49 262d 85b3 deb6 2143 32db d77c dafe  .I&-....!C2..|..
-000048d0: 35bb 665c 1c49 a7fd 9f85 292e 9983 b58c  5.f\.I....).....
-000048e0: 1bf8 892a bf57 5231 3eb2 ca4f d8c5 3761  ...*.WR1>..O..7a
-000048f0: 9323 2cfe 2e57 0db2 a9e9 5bfe 718d d016  .#,..W....[.q...
-00004900: 71c8 4739 6a21 7987 d83b 9d4d 1b89 3b1c  q.G9j!y..;.M..;.
-00004910: bb22 0eda 9afe 2aaa df57 94cd a649 3f2f  ."....*..W...I?/
-00004920: 1236 fe8b 4fa2 1c17 d6ae 62e0 01d3 e448  .6..O.....b....H
-00004930: f0a0 4044 6110 8e66 0db7 a054 4d1f 0bd4  ..@Da..f...TM...
-00004940: b87f 4dd0 e823 921d 995f fd03 7f9e 24fc  ..M..#..._....$.
-00004950: c791 065a 3ea8 f0d7 6eee 412e bb80 e765  ...Z>...n.A....e
-00004960: 928d b1b5 a88d aad9 dd81 1728 4a4c 9e95  ...........(JL..
-00004970: e3c8 1556 2104 47a2 653c 5d28 2abe 4d76  ...V!.G.e<](*.Mv
-00004980: 239b d0a5 f505 4e25 0bf0 612e 2390 1231  #.....N%..a.#..1
-00004990: f860 f5bf 8f09 a9bc c4f9 0f00 00ff ff00  .`..............
-000049a0: 0000 ffff 94d3 d10e 8220 1406 e057 713c  ......... ...Wq<
-000049b0: 4078 5054 1ab2 e57c 1146 6e5d 5913 67f5  @xPT...|.Fn]Y.g.
-000049c0: f69d 5a03 24dd e24e fdff f979 7650 dacb  ..Z.$..N...yvP..
-000049d0: 30cc bd9e b592 d3f5 9e4d 2d01 92d9 9b1e  0........M-.....
-000049e0: 2d5e 1d19 c91e 506a 733c 3ffb c19a 619c  -^....Pjs<?...a.
-000049f0: 5b92 1f18 274a 9a77 f784 657c 64f1 7e51  [...'J.w..e|d.~Q
-00004a00: 201a 4917 25a9 f9a6 5d98 b2bc 7629 45ca   .I.%...]...v)E.
-00004a10: 7968 fcef 61d9 79fe 7d9f 6fe9 c20c 04db  yh..a.y.}.o.....
-00004a20: d68a 140d cb4e 2b8a 68b8 3064 506d 7365  .....N+.h.0dPmse
-00004a30: 0a87 65cf 9511 1786 2060 9be3 291c 961d  ..e..... `..)...
-00004a40: c7e3 d585 2108 3ffb 6a75 550a 8765 c789  ....!.?.juU..e..
-00004a50: 3c9a 2e0c 77a7 ab53 382c fb93 c963 6f95  <...w..S8,...co.
-00004a60: ee8d d7a4 7858 f65e 1d1f 9655 fab3 3dea  ....xX.^...U..=.
-00004a70: ffc2 1700 0000 ffff 0000 00ff ff44 8fcd  .............D..
-00004a80: 0e01 510c 855f a5e9 03f8 8988 1063 c366  ..Q.._.......c.f
-00004a90: 1612 8927 b84c cd6d 70db 748a f0f4 4a4c  ...'.L.mp.t...JL
-00004aa0: ecce 7716 e767 a959 0a39 1f77 0627 295e  ..w..g.Y.9.w.')^
-00004ab0: 3715 8e11 fca9 5461 91b5 943b 59c7 5270  7.....Ta...;Y.Rp
-00004ac0: b85a 6a6a 699b ace5 d2c1 854e 5ee1 6830  .Zjji......N^.h0
-00004ad0: 4330 6e73 af5d f4eb 4e11 0ee2 2ed7 9e32  C0ns.]..N......2
-00004ae0: a586 ec43 138c 26f1 1e7e b97b f29b 8226  ...C..&..~.{...&
-00004af0: 25db f32b cae7 0862 4cc5 9347 7d85 2ae6  %..+...bL..G}.*.
-00004b00: 96d8 1172 f8af d89a 2e1b e548 4488 8d71  ...r.......HD..q
-00004b10: e1cf b6e0 f861 7533 fecc 1e3e c4ce 5d26  .....au3...>..]&
-00004b20: f2d5 1b00 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00004b30: 0008 0000 0021 00be 1d90 1e7e 0300 009b  .....!.....~....
-00004b40: 0900 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
-00004b50: 6565 7473 2f73 6865 6574 342e 786d 6c9c  eets/sheet4.xml.
-00004b60: 934b 8fda 3010 c7ef 95fa 1d2c dfc1 49d8  .K..0......,..I.
-00004b70: a54b 4458 558b 50f7 5655 7d9c 8d33 2116  .KDXU.P.VU}..3!.
-00004b80: 7ea4 b6c3 4355 bf7b c766 0948 1c8a d64a  ~...CU.{.f.H...J
-00004b90: 3c4e 9cf9 cd4c e6ef f9f3 412b b203 e7a5  <N...L....A+....
-00004ba0: 3515 cdc7 1925 6084 ada5 d954 f4c7 f7d5  5....%`....T....
-00004bb0: e889 121f b8a9 b9b2 062a 7a04 4f9f 171f  .........*z.O...
-00004bc0: 3fcc f7d6 6d7d 0b10 0812 8caf 681b 4257  ?...m}......h.BW
-00004bd0: 32e6 450b 9afb b1ed c0e0 4e63 9de6 011f  2.E.......Nc....
-00004be0: dd86 f9ce 01af 9393 56ac c8b2 29d3 5c1a  ........V...).\.
-00004bf0: 7a22 94ee 1e86 6d1a 2960 6945 afc1 8413  z"....m.)`iE....
-00004c00: c481 e201 f3f7 adec fc99 a6c5 3d38 cddd  ............=8..
-00004c10: b6ef 46c2 ea0e 116b a964 3826 2825 5a94  ..F....k.d8&(%Z.
-00004c20: af1b 631d 5f2b acfb 903f 7041 0e0e af02  ..c._+...?pA....
-00004c30: efc9 394c 7a7f 1349 4be1 acb7 4d18 2399  ..9Lz..IK...M.#.
-00004c40: 9d72 be2d 7fc6 668c 8b81 745b ff5d 98fc  .r.-..f...t[.]..
-00004c50: 8139 d8c9 d8c0 0baa 785f 4af9 e3c0 2a2e  .9......x_J...*.
-00004c60: b0c9 3b61 d301 167f 972b 7b59 57f4 4ff6  ..;a.....+{YW.O.
-00004c70: 3646 68f3 3865 a36c 12a7 abf1 972e e6b5  6Fh.8e.l........
-00004c80: c40e c7aa 8883 a6a2 9ff3 f2e5 89b2 c53c  ...............<
-00004c90: e9e7 a784 bdbf 5a93 28c7 b5b5 dbb8 f18a  ......Z.(.......
-00004ca0: 6132 2478 5020 a230 0847 b383 1750 aaa2  a2$xP .0.G...P..
-00004cb0: cbe2 1125 fd3b 41e3 1a91 6c60 5eaf cffc  ...%.;A...l`^...
-00004cc0: 5592 f057 476a 6878 afc2 37bb ff02 72d3  U..WGjhx..7...r.
-00004cd0: 063c 2fd3 31c2 9206 cafa b804 2f50 9418  .</.1......./P..
-00004ce0: 7c7c e20a ab10 8233 d132 9e2e 1415 3f24  ||.....3.2....?$
-00004cf0: bb97 7568 937f 1ed3 5983 0f2b 1981 9488  ..uh....Y..+....
-00004d00: de07 ab7f bd7d 10d3 1b00 d893 0440 7b06  .....}.......@{.
-00004d10: cc62 a87b fdb1 0dc9 1fed 2581 4fff f567  .b.{......%.O..g
-00004d20: a98e 7f00 0000 ffff 0000 00ff ff94 d451  ...............Q
-00004d30: 6ec2 300c c6f1 ab54 39c0 6abb 0da5 2854  n.0....T9.j...(T
-00004d40: 1ae5 2255 5769 4f6c 2255 81db e309 14c7  .."UWiOl"U......
-00004d50: 7e5a de80 ff87 f453 1a08 f17b 59d6 f3b4  ~Z.....S...{Y...
-00004d60: 4e43 b8fe dcaa ebd1 a1ab e2ef 7489 fcea  NC..........t...
-00004d70: d0b8 ea8e ed34 1fbe 1ee7 25ce cb65 3d3a  .....4....%..e=:
-00004d80: f820 ef86 30ff 6d3f 79cc 1f45 7ebf 0dd8  . ..0.m?y..E~...
-00004d90: ef43 bd0d a19e dff5 a46b afeb 9857 02f9  .C.......k...W..
-00004da0: 6ecd 90a4 a112 0d8f 93a6 3396 bc11 80b1  n.........3.....
-00004db0: e82a 5265 e1d3 f8ff c9f0 3859 9ac6 60f2  .*Re......8Y..`.
-00004dc0: 4880 06a3 2a0a 5561 da12 0c8f 05d3 1a4c  H...*.Ua.......L
-00004dd0: 1e09 c860 5445 a12a 8c2f c1f0 3861 bcbd  ...`TE.*./..8a..
-00004de0: 3279 2430 e736 aa8a 4255 985d 0986 c709  2y$0.6..BU.]....
-00004df0: d39b 5b71 ca23 8139 b751 5514 aac2 7425  ..[q.#.9.QU...t%
-00004e00: 181e cbaf c95b 4d5e 09bc 794e aaa2 5895  .....[M^..yN..X.
-00004e10: 665f a2e1 b168 3a7b 85f3 4ab0 331a 5551  f_...h:{..J.3.UQ
-00004e20: ac2f 4d2d ff3a 4f00 0000 ffff 0000 00ff  ./M-.:O.........
-00004e30: ff44 8fcd 0e01 510c 855f a5e9 03f8 8988  .D....Q.._......
-00004e40: 1063 c366 1612 8927 b84c cd6d 70db 748a  .c.f...'.L.mp.t.
-00004e50: f0f4 4a4c ecce 7716 e767 a959 0a39 1f77  ..JL..w..g.Y.9.w
-00004e60: 0627 295e 3715 8e11 fca9 5461 91b5 943b  .')^7.....Ta...;
-00004e70: 59c7 5270 b85a 6a6a 699b ace5 d2c1 854e  Y.Rp.Zjji......N
-00004e80: 5ee1 6830 4330 6e73 af5d f4eb 4e11 0ee2  ^.h0C0ns.]..N...
-00004e90: 2ed7 9e32 a586 ec43 138c 26f1 1e7e b97b  ...2...C..&..~.{
-00004ea0: f29b 8226 25db f32b cae7 0862 4cc5 9347  ...&%..+...bL..G
-00004eb0: 7d85 2ae6 96d8 1172 f8af d89a 2e1b e548  }.*....r.......H
-00004ec0: 4488 8d71 e1cf b6e0 f861 7533 fecc 1e3e  D..q.....au3...>
-00004ed0: c4ce 5d26 f2d5 1b00 00ff ff03 0050 4b03  ..]&.........PK.
-00004ee0: 0414 0006 0008 0000 0021 0047 4b9f 3742  .........!.GK.7B
-00004ef0: 0300 0032 0800 0018 0000 0078 6c2f 776f  ...2.......xl/wo
-00004f00: 726b 7368 6565 7473 2f73 6865 6574 352e  rksheets/sheet5.
-00004f10: 786d 6c9c 934b 8f9b 3010 c7ef 95fa 1d2c  xml..K..0......,
-00004f20: df83 8190 7483 4256 6d57 51b7 a76a d5c7  ....t.BVmWQ..j..
-00004f30: d931 43b0 e207 b54d 1eaa fadd 3b26 8f8d  .1C....M....;&..
-00004f40: 9443 a3b5 c033 60fc 9b19 e6ef f9e3 5e2b  .C...3`.......^+
-00004f50: b205 e7a5 3515 cd92 9412 30c2 d6d2 ac2b  ....5.....0....+
-00004f60: fae3 fb72 f440 890f dcd4 5c59 0315 3d80  ...r.@....\Y..=.
-00004f70: a78f 8bf7 efe6 3beb 36be 0508 0409 c657  ......;.6......W
-00004f80: b40d a12b 19f3 a205 cd7d 623b 30b8 d258  ...+.....}b;0..X
-00004f90: a779 c047 b766 be73 c0eb 6193 562c 4fd3  .y.G.f.s..a.V,O.
-00004fa0: 29d3 5c1a 7a24 94ee 1e86 6d1a 29e0 c98a  ).\.z$....m.)...
-00004fb0: 5e83 0947 8803 c503 e6ef 5bd9 f933 4d8b  ^..G......[..3M.
-00004fc0: 7b70 9abb 4ddf 8d84 d51d 2256 52c9 7018  {p..M....."VR.p.
-00004fd0: a094 6851 3eaf 8d75 7ca5 b0ee 7d56 7041  ..hQ>..u|...}VpA
-00004fe0: f60e af1c eff1 39cc f0fe 2692 96c2 596f  ......9...&...Yo
-00004ff0: 9b90 2099 1d73 be2d 7fc6 668c 8b0b e9b6  .. ..s.-..f.....
-00005000: febb 3059 c11c 6c65 6ce0 2b2a 7f5b 4ad9  ..0Y..lel.+*.[J.
-00005010: e4c2 ca5f 61e3 37c2 a617 58fc 5dae ec65  ..._a.7...X.]..e
-00005020: 5dd1 3fe9 698c d066 714a 4769 11a7 abf1  ].?.i..fqJGi....
-00005030: 972e e6b5 c40e c7aa 8883 a6a2 1fb3 f2d3  ................
-00005040: 0365 8bf9 a09f 9f12 76fe ca27 518e 2b6b  .e......v..'Q.+k
-00005050: 3771 e119 c3a4 48f0 a040 4461 108e 660b  7q....H..@Da..f.
-00005060: 9f41 a98a 7ecd 6628 e9df 0334 fa88 6417  .A..~.f(...4..d.
-00005070: e6b5 7fe6 2f07 097f 73a4 8686 f72a bcd8  ..../...s....*..
-00005080: dd17 90eb 36e0 7999 2613 2c2d 6aa3 ac0f  ....6.y.&.,-j...
-00005090: 4fe0 058a 1283 27f9 2472 8555 08c1 9968  O.....'.$r.U...h
-000050a0: 194f 178a 8aef 07bb 9375 68d1 2b92 f107  .O.......uh.+...
-000050b0: 24ac c087 a58c 404a 44ef 83d5 bf4e 1f9c  $.....@JD....N..
-000050c0: 3047 00f6 6400 a03d 018a 18e9 3fdb d990  0G..d..=....?...
-000050d0: c63f 0000 00ff ff00 0000 ffff 94d3 ed0a  .?..............
-000050e0: 8230 1406 e05b 915d 40d3 7d38 8d39 28bc  .0...[.]@.}8.9(.
-000050f0: 91b1 06fd b270 6275 f71d 2b36 3a98 b47f  .....pbu..+6:...
-00005100: ea79 e1f1 3d4e 1dce de4f bd9d acd1 e3e5  .y..=N...O......
-00005110: 568c 1da9 4811 ae76 0870 b567 a4b8 57c2  V...H..v.p.g..W.
-00005120: bafd e9d1 fbe0 fc30 75a4 dc31 498c 764b  .......0u..1I.vK
-00005130: f600 6178 14e0 7e36 552b 349d 8da6 ee33  ..ax..~6U+4....3
-00005140: 3d7e 4f65 9c52 a0a2 07c6 ff1e 84a3 a790  =~Oe.R..........
-00005150: c65e 6fc1 d615 9ea3 4038 2a9c 2386 6f31  .^o.....@8*.#.o1
-00005160: 2287 8170 62f0 eec4 7ba7 eb6d 640e 03e1  "..pb...{..md...
-00005170: c8c8 06b5 593e e56c 7e2c adce 6120 1c99  ....Y>.l~,..a ..
-00005180: b644 4cbd d546 e530 104e 274e 6247 6dd5  .DL..F.0.N'NbGm.
-00005190: 6972 1c08 2747 e143 d0ac f6a1 e96f 7a02  ir..'G.C.....oz.
-000051a0: 0000 ffff 0000 00ff ff44 8fcd 0e01 510c  .........D....Q.
-000051b0: 855f a5e9 03f8 8988 1063 c366 1612 8927  ._.......c.f...'
-000051c0: b84c cd6d 70db 748a f0f4 4a4c ecce 7716  .L.mp.t...JL..w.
-000051d0: e767 a959 0a39 1f77 0627 295e 3715 8e11  .g.Y.9.w.')^7...
-000051e0: fca9 5461 91b5 943b 59c7 5270 b85a 6a6a  ..Ta...;Y.Rp.Zjj
-000051f0: 699b ace5 d2c1 854e 5ee1 6830 4330 6e73  i......N^.h0C0ns
-00005200: af5d f4eb 4e11 0ee2 2ed7 9e32 a586 ec43  .]..N......2...C
-00005210: 138c 26f1 1e7e b97b f29b 8226 25db f32b  ..&..~.{...&%..+
-00005220: cae7 0862 4cc5 9347 7d85 2ae6 96d8 1172  ...bL..G}.*....r
-00005230: f8af d89a 2e1b e548 4488 8d71 e1cf b6e0  .......HD..q....
-00005240: f861 7533 fecc 1e3e c4ce 5d26 f2d5 1b00  .au3...>..]&....
-00005250: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00005260: 0021 0039 6a59 f5ae 0200 0008 0600 0018  .!.9jY..........
-00005270: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00005280: 2f73 6865 6574 362e 786d 6c9c 93c9 4ec3  /sheet6.xml...N.
-00005290: 3010 86ef 48bc 83e5 7be3 245d 44a3 a615  0...H...{.$]D...
-000052a0: 8b10 dc10 02ee ae33 69ac 7a09 b6bb 09f1  .......3i.z.....
-000052b0: ee8c 535a 2af5 5261 39f6 c456 be99 dffe  ..SZ*.Ra9..V....
-000052c0: 3399 6db5 226b 705e 5a53 d22c 4929 0123  3.m."kp^ZS.,I).#
-000052d0: 6c25 cda2 a4ef 6f8f bd1b 4a7c e0a6 e2ca  l%....o...J|....
-000052e0: 1a28 e90e 3c9d 4daf af26 1beb 96be 0108  .(..<.M..&......
-000052f0: 0409 c697 b409 a12d 18f3 a201 cd7d 625b  .......-.....}b[
-00005300: 30b8 535b a779 c057 b760 be75 c0ab ee23  0.S[.y.W.`.u...#
-00005310: ad58 9ea6 23a6 b934 744f 28dc 250c 5bd7  .X..#..4tO(.%.[.
-00005320: 52c0 8315 2b0d 26ec 210e 140f 58bf 6f64  R...+.&.!...X.od
-00005330: eb0f 342d 2ec1 69ee 96ab b627 ac6e 1131  ..4-..i....'.n.1
-00005340: 974a 865d 07a5 448b e279 61ac e373 85ba  .J.]..D..ya..s..
-00005350: b7d9 800b b275 d873 7cfa 8734 ddfa 5926  .....u.s|..4..Y&
-00005360: 2d85 b3de d621 4132 dbd7 7c2e 7fcc c68c  -....!A2..|.....
-00005370: 8b23 e95c ff45 986c c01c ac65 bcc0 3f54  .#.\.E.l...e..?T
-00005380: febf 92b2 e191 95ff c1fa ff84 8d8e b078  ...............x
-00005390: 5cae 58c9 aaa4 5fe9 6feb e19c c521 eda5  \.X..._.o....!..
-000053a0: c338 9cb4 6f3a 9d54 126f 38aa 220e ea92  .8..o:.T.o8."...
-000053b0: de66 c5dd 90b2 e9a4 f3cf 8784 8d3f 8949  .f...........?.I
-000053c0: b4e3 dcda 65dc 78c6 3429 123c 2810 d118  ....e.x.4).<(...
-000053d0: 84e3 b486 7b50 aaa4 4f7d 94e6 3f3b 688c  ....{P..O}..?;h.
-000053e0: 11c9 8ecc d3f8 c07f ec2c fce2 4805 355f  .........,..H.5_
-000053f0: a9f0 6a37 4f20 174d c0ff 6594 0c51 5af4  ..j7O .M..e..QZ.
-00005400: 4651 ed1e c00b 3425 264f f258 ea0f 0000  FQ....4%&O.X....
-00005410: 00ff ff00 0000 ffff 94d2 4b0a c320 1006  ..........K.. ..
-00005420: e0ab 8807 a8f1 b509 4668 c845 c40a 5da5  ........Fh.E..].
-00005430: 258a 6d6f df89 2d63 092e ea4e 9de1 ff46  %.mo..-c...N...F
-00005440: d4c4 6b08 6971 c959 b3dd 1e64 9b28 a724  ..k.iq.Y...d.(.$
-00005450: dedd 1a61 350a 4a9e 5c39 3f5e 5e4b 883e  ...a5.J.\9?^^K.>
-00005460: ac69 a2c3 4968 6a8d df7b cfd0 0c47 11f6  .i..Ihj..{...G..
-00005470: d90e 8665 6b98 ffd6 e6df 1ac7 1a03 062d  ...ek..........-
-00005480: c8ff df12 45a9 4965 8219 2270 02d1 5664  ....E.Ie.."p..Vd
-00005490: 8f22 9b0a 44a0 22db 8aea 5154 51ea bc9f  ."..D."...QTQ...
-000054a0: bb40 042a aaad e81e 657f a76c 8f0a 44a0  .@.*....e..l..D.
-000054b0: a20f 0aab ffe1 0d00 00ff ff00 0000 ffff  ................
-000054c0: 34cd c10a c230 1004 d05f 09fb 0156 11e9  4....0..._...V..
-000054d0: a5e9 c593 07a1 bf10 db6d 12d4 9db0 5914  .........m....Y.
-000054e0: ffde 2ae4 366f 0e33 4349 10b6 3c4f ea56  ..*.6o.3CI..<O.V
-000054f0: 885d 164f 0772 f629 ec49 7086 bc58 6b86  .].O.r.).Ip..Xk.
-00005500: 5037 0e25 44be 068d 59aa 7bf0 6a9e f6bb  P7.%D...Y.{.j...
-00005510: 9e9c e698 5a36 947f 7b22 7783 199e 4d89  ....Z6..{"w...M.
-00005520: c3c2 fad3 91b6 2758 c3b6 dbbd a1f7 9a98  ......'X........
-00005530: 6dfc 0200 00ff ff03 0050 4b03 0414 0006  m........PK.....
-00005540: 0008 0000 0021 00a2 2df2 5aa6 0600 0095  .....!..-.Z.....
-00005550: 1a00 0013 0000 0078 6c2f 7468 656d 652f  .......xl/theme/
-00005560: 7468 656d 6531 2e78 6d6c ec59 5b8b 1b37  theme1.xml.Y[..7
-00005570: 147e 2ff4 3f0c f3ee f836 e3cb 126f b0c7  .~/.?....6...o..
-00005580: 76d2 6637 0959 2725 8f5a 5bf6 28ab 1999  v.f7.Y'%.Z[.(...
-00005590: 91bc 1b13 0225 7929 b414 4ad3 d23e 14da  .....%y)..J..>..
-000055a0: a73e 9436 8104 5a68 f26b 364d 495b c85f  .>.6..Zh.k6MI[._
-000055b0: e891 66ec 91d6 7237 4937 9096 ac61 99d1  ..f...r7I7...a..
-000055c0: 7c3a fa74 ced1 a7db e933 3722 eaec e384  |:.t.....37"....
-000055d0: 1316 b7dc f2a9 92eb e078 c846 249e b4dc  .........x.F$...
-000055e0: 2b83 7ea1 e13a 5ca0 7884 288b 71cb 9d63  +.~..:\.x.(.q..c
-000055f0: ee9e d97c f79d d368 4384 38c2 0ed4 8ff9  ...|...hC.8.....
-00005600: 066a b9a1 10d3 8d62 910f a118 f153 6c8a  .j.....b.....Sl.
-00005610: 63f8 3666 4984 04bc 2693 e228 4107 6037  c.6fI...&..(A.`7
-00005620: a2c5 4aa9 542b 4688 c4ae 13a3 08cc 5e1c  ..J.T+F.......^.
-00005630: 8fc9 103b 4f1e 7ff4 f4eb 7b4f 7ef9 f5d9  ...;O.....{O~...
-00005640: 779f b89b 8b36 7a14 1a8a 0597 0543 9aec  w....6z......C..
-00005650: c816 b051 5161 477b 6589 e073 1ed0 c4d9  ...QQaG{e..s....
-00005660: 47b4 e542 7323 7630 c037 84eb 50c4 057c  G..Bs#v0.7..P..|
-00005670: 68b9 25f5 e716 374f 17d1 4656 898a 3575  h.%...7O..FV..5u
-00005680: b57a 7df5 97d5 cb2a 8cf6 2aaa cd64 b2bb  .z}....*..*..d..
-00005690: 6cd4 f37c afd6 5eda 5700 2a56 71bd 7aaf  l..|..^.W.*Vq.z.
-000056a0: d6ab 2ded 2900 1a0e a1a7 2917 dda6 df69  ..-.).....)....i
-000056b0: 76ba 7e86 d540 e9a3 c576 b7de ad96 0dbc  v.~..@...v......
-000056c0: 66bf bac2 b9ed cb9f 8157 a0d4 beb7 82ef  f........W......
-000056d0: f703 f0a2 8157 a014 ef5b 7c52 af04 9e81  .....W...[|R....
-000056e0: 57a0 145f 5bc1 d74b edae 5737 f00a 1452  W.._[..K..W7...R
-000056f0: 12ef ada0 4b7e ad1a 2c7a bb84 8c19 3d67  ....K~..,z....=g
-00005700: 8537 7daf 5faf 64c6 7314 64c3 32bb 6413  .7}._.d.s.d.2.d.
-00005710: 6316 8b75 b916 a1eb 2ce9 0340 0229 1224  c..u....,..@.).$
-00005720: 76c4 7c8a c768 08c9 1c20 4a76 13e2 6c91  v.|..h... Jv..l.
-00005730: 4908 8937 4531 e350 5caa 94fa a52a fc97  I..7E1.P\....*..
-00005740: 3f4f 3d29 8fa0 0d8c b4da 9217 30e1 2b45  ?O=)........0.+E
-00005750: 928f c387 0999 8a96 fb3e 5875 35c8 f347  .........>Xu5..G
-00005760: 3f3e 7ff4 c079 fee8 fee1 ed87 87b7 7f3e  ?>...y.........>
-00005770: bc73 e7f0 f6bd d496 51f1 1c8a 277a c53f  .s......Q...'z.?
-00005780: bfff ecaf 6f3e 74fe 78f0 ed9f 77bf b0e3  ....o>t.x...w...
-00005790: b98e ffed a78f 9f3c fedc 0e84 cee6 5e78  .......<......^x
-000057a0: fae5 fddf 1fde 7ffa d5a7 cf7e b86b 81b7  ...........~.k..
-000057b0: 13b4 abc3 0724 c2dc b980 0f9c cb2c 82be  .....$.......,..
-000057c0: 292f 98cc f16e f272 3506 2122 460d 1482  )/...n.r5.!"F...
-000057d0: 6d8b e99e 080d e085 39a2 365c 079b cebb  m.......9.6\....
-000057e0: 9a80 c0d8 8067 67d7 0dae 3b61 3213 c4d2  .....gg...;a2...
-000057f0: f2f9 3032 80db 8cd1 0e4b ac0e 382f dbd2  ..02.....K..8/..
-00005800: 3c3c 98c5 137b e3c9 4cc7 5d46 68df d676  <<...{..L.]Fh..v
-00005810: 8062 23b4 bdd9 1494 95d8 4c06 2136 685e  .b#.......L.!6h^
-00005820: a228 1668 8263 2c1c f98d ed61 6ce9 dd35  .(.h.c,....al..5
-00005830: 420c bf6e 9361 c238 1b0b e71a 713a 8858  B..n.a.8....q:.X
-00005840: 5d32 20bb 4622 e595 ce91 08e2 32b7 1184  ]2 .F"......2...
-00005850: 501b bed9 beea 7418 b5f5 ba8b f74d 240c  P.....t......M$.
-00005860: 0844 2de4 0798 1a6e 3c8b 6602 4536 9303  .D-....n<.f.E6..
-00005870: 1451 dde1 5b48 8436 923b f364 a8e3 7a5c  .Q..[H.6.;.d..z\
-00005880: 40a4 2798 32a7 37c2 9cdb ea5c 4ca0 bf5a  @.'.2.7....\L..Z
-00005890: d0cf 83b8 d8c3 be4d e791 894c 04d9 b3d9  .......M...L....
-000058a0: dc42 8ce9 c82e db0b 4214 4dad 9c49 1cea  .B......B.M..I..
-000058b0: d8f7 f81e a428 722e 3161 836f 3373 84c8  .....(r.1a.o3s..
-000058c0: 7788 038a d786 fb2a c146 b88f 1782 2ba0  w......*.F....+.
-000058d0: ab3a a53c 41e4 9759 6289 e559 cccc f138  .:.<A..Yb..Y...8
-000058e0: a763 8495 ca80 ec1b 6a1e 91f8 5869 3f22  .c......j...Xi?"
-000058f0: eafe 5b51 4f67 a5a3 a2de 4e88 7568 9d3b  ..[QOg....N.uh.;
-00005900: 22e5 eb70 ff41 01ef a259 7c09 c398 599d  "..p.A...Y|...Y.
-00005910: c0de eaf7 5bfd 76ff f7fa bd6e 2c9f bc6a  ....[.v....n,..j
-00005920: e742 0d1a 9eaf d6d5 da3d 5abb 741f 134a  .B.......=Z.t..J
-00005930: 77c4 9ce2 2dae 56ef 1ca6 a751 1f0a d5b6  w...-.V....Q....
-00005940: 42ed 2d97 5bb9 6908 8fd9 46c1 c04d 12a4  B.-.[.i...F..M..
-00005950: ea38 0913 1f10 11ee 8468 0a4b fcb2 da88  .8.......h.K....
-00005960: 4e78 667a c29d 29e3 b0f2 57c5 6a67 8c8f  Nxfz..)...W.jg..
-00005970: d856 fb87 59b4 cd46 e98e b55c 96bb d354  .V..Y..F...\...T
-00005980: 3c38 1279 79c9 5f96 c36e 43a4 e85a 3ddf  <8.yy._..nC..Z=.
-00005990: 852d cdab 7ded 44ed 9617 0464 dd97 21a1  .-..}.D....d..!.
-000059a0: 3566 92a8 5a48 d417 8510 857f 22a1 7a76  5f..ZH......".zv
-000059b0: 222c 9a16 160d 697e 11aa 4514 97ae 006a  ",....i~..E....j
-000059c0: cba8 c0fa c981 5557 cbf5 bdf4 2400 3655  ......UW....$.6U
-000059d0: 88e2 918c 537a 28b0 88ae 0cce 8946 7a9d  ....Sz(......Fz.
-000059e0: 33a9 9e01 b098 5864 401e e9a6 e4ba b67b  3.....Xd@......{
-000059f0: b277 69aa bd40 a40d 125a ba99 24b4 340c  .wi..@...Z..$.4.
-00005a00: d108 67d9 a91f 9d9c 64ac 9b79 480d 7ad2  ..g.....d..yH.z.
-00005a10: 158b d190 d3a8 375e 47ac a588 1cd1 061a  ......7^G.......
-00005a20: eb4a 4163 e7a0 e5d6 aa3e 1c92 0dd1 b4e5  .JAc.....>......
-00005a30: 8e61 e70f 8fd1 1472 87cb 752f a213 3845  .a.....r..u/..8E
-00005a40: 1b8a 241d f0af a22c d384 8b2e e261 ea70  ..$....,.....a.p
-00005a50: 253a a91a 4444 e0c4 a124 6ab9 b2fb cb6c  %:..DD...$j....l
-00005a60: a0b1 d210 c5ad 5c01 4178 63c9 3541 56de  ......\.Axc.5AV.
-00005a70: 3472 1074 33c8 783c c643 a187 5d2b 919e  4r.t3.x<.C..]+..
-00005a80: 4e5f 41e1 53ad b07e 55d5 5f1d 2c6b b219  N_A.S..~U._.,k..
-00005a90: 847b 271c 1d38 bb74 965c 4690 627e bd2c  .{'..8.t.\F.b~.,
-00005aa0: 1d38 221c 0e80 caa9 3747 044e 3497 4296  .8".....7G.N4.B.
-00005ab0: e7df 9189 2993 5dfd 4851 e550 5a8e e834  ....).].HQ.PZ..4
-00005ac0: 44d9 8ca2 8b79 0a57 22ba a4a3 de96 3ed0  D....y.W".....>.
-00005ad0: deb2 3e83 4357 5db8 3b91 13ec bf9e 758f  ..>.CW].;.....u.
-00005ae0: 9faa a5e7 34d1 cce7 4c43 55e4 ac69 17d3  ....4...LCU..i..
-00005af0: d737 c96b acf2 49d4 6095 4ab7 da36 f05c  .7.k..I.`.J..6.\
-00005b00: eb9a 0bad 8344 b5ce 12c7 ccba 2f30 2168  .....D....../0!h
-00005b10: d4f2 c60c 6a92 f1aa 0c4b cdce 4a4d 6a27  ....j....K..JMj'
-00005b20: b820 d03c 515b e3b7 e51c 61f5 c4ab cefc  . .<Q[....a.....
-00005b30: 50ef 68d6 ca09 62b1 ae54 89af 6e40 f4db  P.h...b..T..n@..
-00005b40: 09b6 7b1d c4a3 0be7 c033 2ab8 0a25 dc3d  ..{......3*..%.=
-00005b50: 2408 167d e949 722a 1b30 446e 886c 8d08  $..}.Ir*.0Dn.l..
-00005b60: 4fce 2c21 2df7 66c9 6f7b 41c5 0f0a a586  O.,!-.f.o{A.....
-00005b70: df2b 7855 af54 68f8 ed6a a1ed fbd5 72cf  .+xU.Th..j....r.
-00005b80: 2f97 ba9d ca2d 9858 4418 95fd f4f6 a50f  /....-.XD.......
-00005b90: e751 749e ddc1 a8f2 957b 9868 71e4 766a  .Qt......{.hq.vj
-00005ba0: c8a2 2253 f72c 4545 5cdd c394 2bb6 7b98  .."S.,EE\...+.{.
-00005bb0: 81bc 6171 1d02 a273 b356 e937 abcd 4ead  ..aq...s.V.7..N.
-00005bc0: d0ac b6fb 05af db69 149a 41ad 53e8 d682  .......i..A.S...
-00005bd0: 7ab7 df0d fc46 b37f cb75 f615 d86b 5703  z....F...u...kW.
-00005be0: afd6 6b14 6ae5 2028 78b5 92a4 df68 16ea  ..k.j. (x....h..
-00005bf0: 5ea5 d2f6 eaed 46cf 6bdf ca96 31d0 f354  ^.....F.k...1..T
-00005c00: 3e32 5f80 7b15 afcd bf01 0000 ffff 0300  >2_.{...........
-00005c10: 504b 0304 1400 0600 0800 0000 2100 2044  PK..........!. D
-00005c20: 56f6 0503 0000 6e07 0000 0d00 0000 786c  V.....n.......xl
-00005c30: 2f73 7479 6c65 732e 786d 6cb4 55cd 6ed3  /styles.xml.U.n.
-00005c40: 4010 be23 f10e abbd bbfe 491c 92c8 76d5  @..#......I...v.
-00005c50: 34b5 54a9 4848 2d12 d78d bd4e 56dd 1f6b  4.T.HH-....NV..k
-00005c60: bd29 0e08 8923 274e 08f1 0e70 e881 030f  .)...#'N...p....
-00005c70: 840a bc05 b3b6 d3b8 aa04 b415 9778 7776  .............xwv
-00005c80: f79b 6fe6 9b99 44fb b5e0 e882 ea8a 2919  ..o...D.......).
-00005c90: 637f cfc3 88ca 4ce5 4c2e 63fc fc2c 75c6  c.....L.L.c..,u.
-00005ca0: 1855 86c8 9c70 2569 8c37 b4c2 fbc9 e347  .U...p%i.7.....G
-00005cb0: 5165 369c 9eae 2835 0820 6415 e395 31e5  Qe6...(5. d...1.
-00005cc0: d475 ab6c 4505 a9f6 5449 259c 144a 0b62  .u.lE...TI%..J.b
-00005cd0: 60ab 976e 556a 4af2 ca3e 12dc 0d3c 6fe4  `..nUjJ..>...<o.
-00005ce0: 0ac2 246e 11a6 22fb 1710 41f4 f9ba 7432  ..$n.."...A...t2
-00005cf0: 254a 62d8 8271 6636 0d16 4622 9b1e 2fa5  %Jb..qf6..F"../.
-00005d00: d264 c181 6aed 0f49 866a 7fa4 0354 ebad  .d..j..I.j...T..
-00005d10: 93c6 7acb 8f60 9956 952a cc1e e0ba aa28  ..z..`.V.*.....(
-00005d20: 5846 6fd3 9db8 1397 643b 2440 be1f 921f  XFo.....d;$@....
-00005d30: ba5e 7023 f65a df13 69e8 6a7a c1ac 7c38  .^p#.Z..i.jz..|8
-00005d40: 890a 254d 8532 b596 26c6 0110 b529 989e  ..%M.2..&....)..
-00005d50: 4bf5 52a6 f608 14ee 6e25 51f5 0a5d 100e  K.R.....n%Q..]..
-00005d60: 9600 bb49 9429 ae34 3220 1d64 ceb7 1649  ...I.).42 .d...I
-00005d70: 046d 6f5c 7dbc fcf1 f5f2 ead3 fb5f 9f3f  .mo\}........_.?
-00005d80: d893 8208 c637 ed59 fb78 4574 0585 d0e2  .....7.Y.xEt....
-00005d90: 0d46 f652 5306 1d80 6020 8a35 ba96 604b  .F.RS...` .5..`K
-00005da0: 7347 60f2 9fbd 354e 2bf0 ca38 ef25 a735  sG`...5N+..8.%.5
-00005db0: 2411 5491 a15a a670 8aba f5d9 a684 2c48  $.T..Z.p......,H
-00005dc0: 28f8 9634 1cfd f5f6 5293 8d1f 84bd 076e  (..4....R......n
-00005dd0: e330 8916 4ae7 d060 5b59 ac02 ad29 8938  .0..J..`[Y...).8
-00005de0: 2d0c a445 b3e5 ca7e 8d2a e177 a18c 8122  -..E...~.*.w..."
-00005df0: 4ca2 9c91 a592 84db c46d 5f74 0b08 27a3  L........m_t..'.
-00005e00: 9c9f da26 7c51 dcc0 ae0b 24d7 2215 e638  ...&|Q....$."..8
-00005e10: 8f31 b4b3 4df9 7609 8174 cb16 afdd 2411  .1..M.v..t....$.
-00005e20: e16c 2905 9520 21d5 8665 b62e 32d8 d256  .l).. !..e..2..V
-00005e30: b5ba 0006 7d7f adf7 9ee3 0082 babb 6354  ....}.........cT
-00005e40: 1777 60f0 007c 44ca 926f 0eb6 5176 15de  .w`..|D..o..Qv..
-00005e50: 8404 41f4 7279 2393 d711 23db 0b31 fefe  ..A.ry#...#..1..
-00005e60: eded cf77 5fa0 ab3a d668 b166 dc30 d9c6  ...w_..:.h.f.0..
-00005e70: 6055 ba7e 0198 79bd d3c5 b365 61ec 586a  `U.~..y....ea.Xj
-00005e80: 14bb f602 f2e4 b420 6b6e ceae 0f63 bc5b  ....... kn...c.[
-00005e90: 3fa5 395b 0b68 e4ee d633 76a1 4c03 11e3  ?.9[.h...3v.L...
-00005ea0: ddfa c496 8fdf 741d adcd 4905 1d06 5fb4  ......t...I..._.
-00005eb0: d62c c6af 8f66 4f26 f3a3 3470 c6de 6cec  .,...fO&..4p..l.
-00005ec0: 0c07 3474 26e1 6cee 84c3 c3d9 7c9e 4ebc  ..4t&.l.....|.N.
-00005ed0: c03b 7cd3 1b8e 0f18 8dcd 2c87 3af0 87d3  .;|.......,.:...
-00005ee0: 8ac3 00d5 5db0 1df9 d39d 2dc6 bd4d 4bbf  ....].....-..MK.
-00005ef0: 691c a0dd e73e 0946 de41 e87b 4e3a f07c  i....>.F.A.{N:.|
-00005f00: 6738 2263 673c 1a84 4e1a fac1 7c34 9c1d  g8"cg<..N...|4..
-00005f10: 8569 d8e3 1ede 7384 7aae efb7 c3d8 920f  .i....s.z.......
-00005f20: a786 09ca 99dc 6ab5 55a8 6f05 9160 fb87  ......j.U.o..`..
-00005f30: 20dc ad12 eeee 8f32 f90d 0000 ffff 0300   ......2........
-00005f40: 504b 0304 1400 0600 0800 0000 2100 3968  PK..........!.9h
-00005f50: e2c5 171d 0000 a886 0000 1400 0000 786c  ..............xl
-00005f60: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
-00005f70: 6d6c c45d 5b53 1cc7 927e df88 fd0f 0411  ml.][S...~......
-00005f80: 1b71 f6c1 4780 00db 1bb2 4e00 4236 e770  .q..G.....N.B6.p
-00005f90: b3c0 76f8 a9a3 a7a7 07fa 6866 7a3c dd83  ..v.......hfz<..
-00005fa0: c43e e962 0c42 c892 f708 2c59 e866 49e7  .>.b.B....,Y.fI.
-00005fb0: 605b 080b d912 baff 197a 2e4f fb17 f6ab  `[.......z.O....
-00005fc0: aa9e 99a6 33ab 6710 8ed8 b799 aaac acac  ....3.g.........
-00005fd0: ccac acac acac ea23 7f39 9dcb 76cc d945  .......#.9..v..E
-00005fe0: cf71 f31f 7576 ffb9 abb3 c3ce 5b6e dac9  .q..uv......[n..
-00005ff0: cf7c d4f9 d9f4 f1f7 3ee8 ecf0 7c33 9f36  .|......>...|3.6
-00006000: b36e defe a873 def6 3aff 72f4 dfff ed88  .n...s..:.r.....
-00006010: e7f9 1d68 9bf7 3eea 9cf5 fdc2 7f1d 3ae4  ...h..>.......:.
-00006020: 59b3 76ce f4fe ec16 ec3c 6a32 6e31 67fa  Y.v......<j2n1g.
-00006030: f85b 9c39 e415 8ab6 99f6 666d dbcf 650f  .[.9......fm..e.
-00006040: f574 75f5 1fca 994e beb3 c372 4b79 ffa3  .tu....N...rKy..
-00006050: ce9e 9ebe eece 8e52 def9 aa64 0fa9 a2ee  .......R...d....
-00006060: aec3 3d9d 478f 78ce d123 fed1 8963 470e  ..=.G.x..#...cG.
-00006070: f947 8f14 6641 83ef 5893 c58e 8c9b f747  .G..fA..X......G
-00006080: d2a0 b8b3 c39f 2f80 b0bc 3be4 e6c3 8174  ....../...;....t
-00006090: 1e3a 7ae4 9068 a95a ff6d f8cb a983 b4b7  .:z..h.Z.m......
-000060a0: 5c27 7d90 f6b9 b4e9 dbff 9f04 98d9 ac21  \'}............!
-000060b0: 68f0 fe10 2222 9ccd 3879 c3b3 b319 c3b4  h...""..8y......
-000060c0: 2c89 3b52 d71c 75a4 f0a4 3d7f 380e 9877  ,.;R..u...=.8..w
-000060d0: e325 9e9d 8b17 899e 84a0 e3e5 56a9 588c  .%..........V.X.
-000060e0: 9799 f9bc 9257 8c52 8716 3b85 ee9e 78f3  .....W.R..;...x.
-000060f0: 19d2 b9e3 b94e 1cca f19c 944f 0bf3 0c60  .....N.....O...`
-00006100: de29 c401 8b87 bbfa e365 7641 c927 4275  .).......evA.'Bu
-00006110: b1bb ab8f 34ed a64d 01f7 3e03 f701 29eb  ....4..M..>...).
-00006120: edea 66ca 080b 8abd 5d44 4c28 eb65 da12  ..f.....]DL(.e..
-00006130: fa84 a4cc 52da f15d 2218 cf3f 6914 8a8e  ....R..]"..?i...
-00006140: 45a4 983b 4958 29ac 8841 c438 ebcc ccd2  E..;IX)..A.8....
-00006150: d2ac 7b8a 165a 59d7 b369 b199 fe7b c624  ..{..ZY..i...{.$
-00006160: ca3a e766 8916 e508 4d7e 311f 874a 85a6  .:.f....M~1..J..
-00006170: 2122 3437 93b1 a94e cecd 148a a4db 22d5  !"47...N......".
-00006180: abd9 5cb6 60d1 9e4b c5bc 0beb 4666 caac  ..\.`..K....Ff..
-00006190: 590c a775 74ea 9df4 2d93 e81c 988c 5283  Y..ut...-.....R.
-000061a0: c16e e67c aeb8 40fb 2ba4 0809 6967 ce98  .n.|..@.+...ig..
-000061b0: a75c b034 e539 18ee 59c3 33b3 946c 316f  .\.4.9..Y.3..l1o
-000061c0: 0d32 07d2 5d5d 5469 4521 d15a 5148 d456  .2..]]TiE!.ZQH.V
-000061d0: 1412 bd15 8544 7145 2199 94a2 904c 2db3  .....DqE!....L-.
-000061e0: 3767 9e9e 250a 234a 89c6 4a58 96e9 bd39  7g..%.#J..JX...9
-000061f0: 27cf 2161 cc14 9060 5671 92eb 9dcd cc50  '.!a...`Vq.....P
-00006200: 42e6 b9c2 1c2d f4b2 8694 471c 83ff 0163  B....-....G....c
-00006210: 5050 d84d ad47 3731 3280 3b4c c420 0aa9  PP.M.G712.;L. ..
-00006220: f9e8 a1d6 ad87 88a0 d8d3 6fc6 0984 5868  ..........o...Xh
-00006230: 5b51 c809 b087 b18d 1f12 5346 a152 6671  [Q........SF.Rfq
-00006240: 065e ca8c 61cd 3ad4 367f 9571 1c23 559a  .^..a.:.6..q.#U.
-00006250: 8f23 92e5 5814 8941 9115 f669 163e 8529  .#..X..A...i.>.)
-00006260: c823 d255 d8a7 7535 8c9a 644a 9859 0cad  .#.U..u5..dJ.Y..
-00006270: b29c a355 5650 5a15 1ea6 6385 4857 c1d2  ...UVPZ...c.HW..
-00006280: 9a49 730a 9dce 160b 1ca5 b29c a354 5650  .Is..........TVP
-00006290: 4a15 1e86 2085 4857 c152 8a26 b31a 9a60  J... .HW.R.&...`
-000062a0: c918 49cb 062c 4dc0 c377 2d4c 2255 8110  ..I..,M..w-L"U..
-000062b0: 115f c3b1 cf77 7d8e 5251 cc11 2aca 299d  ._...w}.RQ..*.).
-000062c0: 1209 d3a7 c4a2 2967 1907 8d33 c834 1074  ......)g...3.4.t
-000062d0: d052 ec2e 660c 3205 5429 99fd 96e9 cd32  .R..f.2.T).....2
-000062e0: 289c 9ce3 d362 4104 5954 2411 b474 d62d  (....bA.YT$..t.-
-000062f0: fa94 0a4f 1513 320a 2683 392b a9a0 a88d  ...O..2.&.9+....
-00006300: 2c27 2ff8 0a9e ed1b 6451 0dcb 4997 62dd  ,'/.....dQ..I.b.
-00006310: 3452 c40a 87c5 04bc 68fb 701c 0831 29b7  4R......h.p..1).
-00006320: 5834 7c82 252c 2658 d490 68af d91c f547  X4|.%,&X..h....G
-00006330: 6891 4f8b e06d 1969 226c 554a dc16 4fb8  h.O..m.i"lUJ..O.
-00006340: 3846 daf1 fca2 932a f9d8 a7c6 0da5 2df6  8F.....*......-.
-00006350: 3664 3419 8b8a bd90 b5d3 33b4 5822 20ee  6d4.......3.X" .
-00006360: 8437 5bcc 19a5 deae 2eea 7415 3d5d 4541  .7[.......t.=]EA
-00006370: 5791 335c 1d2a 4d45 41d7 2267 f41a 649d  W.3\.*MEA."g..d.
-00006380: 03b5 9ea6 bca0 29cf 19fd 0659 bd25 1ebe  ......)....Y.%..
-00006390: bca0 81cf 191f 18dd 3c97 3415 055d 0b70  ........<.4..].p
-000063a0: a91b 1e17 cb71 5d0d f8c4 b6c1 66c3 f47d  .....q].....f..}
-000063b0: a2a2 7083 8d14 71d3 e074 95a0 61f3 06f1  ..p...q..t..a...
-000063c0: d11b 3564 d702 ecd8 a350 af0a ba5a 608a  ..5d.....P...Z`.
-000063d0: 73d6 2c76 3fa4 67af c442 674a 3093 14b7  s.,v?.g..BgJ0...
-000063e0: 9a8b 6cb9 cb80 7b29 33ed 33e5 4efa b4e1  ..l...{)3.3.N...
-000063f0: 9fca f711 4e8b 8a9c 67d1 5d2c ca5d dfe2  ....N...g.],.]..
-00006400: 1ba0 0231 9db8 d004 aa59 ec02 b8f2 1cb3  ...1.....Y......
-00006410: 3f19 6838 faef 18e7 1108 d42c 3e00 02e5  ?.h8.......,>...
-00006420: b9be 2382 e981 c1d1 6163 7c60 6c78 4a8e  ..#.....ac|`lxJ.
-00006430: fa1d d11c 2cdc 3534 31fa d9d8 f881 08f8  ....,.541.......
-00006440: 83c6 f107 a119 981c 3124 aa83 f074 fa8b  ........1$...t..
-00006450: f143 03c7 87a7 a6c7 c84a 21ab 46c6 3f3f  .C.......J!.F.??
-00006460: 3e32 fe69 5c59 65dd e4c8 e489 a163 07ee  >2.i\Ye......c..
-00006470: 7d72 646a 6074 58d3 c3d4 2727 0686 a613  }rdj`tX...''....
-00006480: 2bbf d0d5 4eff 6d60 7afa 44bc 56b0 6d68  +...N.m`z.D.V.mh
-00006490: e298 eaf0 1d35 71e8 93f1 83ab 7375 fb6e  .....5q.....su.n
-000064a0: 70f1 fa7b d5c5 9f2b bf5f 29af ee1c 8491  p..{...+._).....
-000064b0: 755c db77 2bbf be3e 10a2 7377 2b0f 36ca  u\.w+..>..sw+.6.
-000064c0: df3f a83e 592c af5d afde dd38 08b6 f2fa  .?.>Y,.]...8....
-000064d0: 5265 f176 f9ea d383 20a9 3c5e a9fc f84a  Re.v.... .<^...J
-000064e0: d173 103c b51b dfec bebd 7970 3c55 c9a2  .s.<......yp<U..
-000064f0: e0f1 c3f2 997f 1d1c 9bb0 ce2a 02f0 8eba  ...........*....
-00006500: 982a d0f0 03ca 88df 962a f450 d7b6 d0c3  .*.......*.P....
-00006510: c01d 66e0 7a99 b23e ae8c c1d7 47c2 1ea9  ..f.z..>....G...
-00006520: 423f d3b6 9f69 dbcf b525 1193 54e1 7d06  B?...i...%..T.}.
-00006530: dffb 0cbe 0f89 8798 2a7c 4802 2128 231e  ........*|H.!(#.
-00006540: 20ca 4874 2435 c7f0 7e8e e1fd 5c37 1dc7   .Ht$5..~...\7..
-00006550: 5c37 1dc7 1c23 a339 461e 738c 3ce6 7ae9  \7...#.9F.s.<.z.
-00006560: 7833 0c7d 1986 be0c d36f 86d1 8d0c 434b  x3.}.....o....CK
-00006570: 86a1 25c3 d1d2 4b79 90e9 a53c c8f4 92f0  ..%...Ky...<....
-00006580: 572a c3f0 deb3 c896 2ce5 e5b9 429f 01b4  W*......,...B...
-00006590: c80e 5c34 660a 7da6 cc23 4e6f cacb d2c2  ..\4f.}..#No....
-000065a0: b44d cf42 be2a 39d6 c9f8 9a54 a027 3826  .M.B.*9....T.'8&
-000065b0: f1d0 7128 4394 dc61 2635 ca88 2238 052a  ..q(C..a&5.."8.*
-000065c0: 38a7 4005 8732 a62d 151c e088 909c 0235  8.@..2.-.......5
-000065d0: 080e 3369 5046 2697 c34c 2487 990c 2823  ..3iPF&..L$...(#
-000065e0: 0ae3 3013 c461 2688 c34c 0687 5168 6c53  ..0..a&..L..QhlS
-000065f0: 3cb2 1d71 0bc4 f7cf 1749 112d c933 0ded  <..q.....I.-.3..
-00006600: 9443 76f9 1623 2094 1161 588e 47cf d22c  .Cv..# ..aX.G..,
-00006610: 4e0d 4421 d39c eb87 d304 34a7 aa60 718b  N.D!......4..`q.
-00006620: 080a a972 a190 6a17 0aa9 dd17 8594 4e14  ...r..j.......N.
-00006630: 126b 2120 89f4 2d46 eb2c 469b 5046 7b61  .k! ..-F.,F.PF{a
-00006640: 34cc 9a63 b8c6 6898 35c7 0887 d13a 8bd1  4..c..h.5....:..
-00006650: 3a94 515a 1813 6c31 da69 31e6 d6f2 a965  :.QZ..l1.i1....e
-00006660: b07c 6ad2 2de4 2290 6311 cb4b 59e4 bc05  .|j.-.".c..KY...
-00006670: 9019 72fe 2c0a 89ca 8bc2 4cdc 9e59 9e4d  ..r.,.....L..Y.M
-00006680: 71e2 dccc a351 aa53 e61c 21c9 374f 17eb  q....Q.S..!.7O..
-00006690: b901 7b8f 7de9 5949 7737 7358 c21c e776  ..{.}.YIw7sX...v
-000066a0: 5396 e3e8 963b 0aa6 6720 bd34 8c53 eca3  S....;..g .4.S..
-000066b0: 076d 2823 06ba d8c3 1c55 f771 65dd f438  .m(#.....U.qe..8
-000066c0: a68f a1b9 af8b d2d7 cf8c a3bf 9b9e 18f5  ................
-000066d0: 33e3 e867 8ec8 fba9 b752 ec67 68e9 e768  3..g.....R.gh..h
-000066e0: a15e 0dda 52be f433 723b ccd0 7298 395e  .^..R..3r;..r.9^
-000066f0: 3fcc f0ef 3033 de0f e8d9 9a72 de77 5fde  ?...03.....r.w_.
-00006700: c396 22ae b5d8 f594 d76f c74b c506 e6c1  .."......o.K....
-00006710: 6665 e735 b631 c1c2 03b2 d974 7d33 6b4c  fe.5.1.....t}3kL
-00006720: 40b9 4d5f 1c8a 8d20 4d28 47dc 83f2 d68d  @.M_... M(G.....
-00006730: 60e9 a778 db8f 8bae e719 9345 3783 08fd  `..x.......E7...
-00006740: a8f8 9d29 bab9 3a32 9746 a815 2dc0 547e  ...)..:2.F..-.T~
-00006750: 7d3f 8eac 4982 4218 af57 ad30 8eda dd4b  }?..I.B..W.0...K
-00006760: f1ba 9084 411b d949 b631 6d92 d3b8 f2b3  ....A..I.1m.....
-00006770: 0dbe d771 84e9 d590 e500 084b b72e 050b  ...q.......K....
-00006780: 0f83 cb3b 0a41 bc3a d27a 0031 4911 c836  ...;.A.:.z.1I..6
-00006790: 5308 e5fb ae31 89f0 769e 2c93 e5ad cb42  S....1..v.,....B
-000067a0: 821b 0bc1 854b 4059 b9b1 4c87 2207 5027  .....K@Y..L.".P'
-000067b0: 6ad2 2e1a 5322 54ae a74c a1bc b154 bb7f  j...S"T..L...T..
-000067c0: 2d0e 3468 7a8e 650c 9bc5 3c44 0b49 e990  -.4hz.e...<D.I..
-000067d0: 29b9 2821 57be 5de4 e53c 8673 531c 579f  ).(!W.]..<.sS.W.
-000067e0: 8065 33a0 2e16 33bc 867c 3130 064f 5ccb  .e3...3..|10.O\.
-000067f0: 9271 d599 04c1 31b8 2695 a0eb 7c4a a40a  .q....1.&...|J..
-00006800: 98de ac28 0932 9822 426c 35b6 ab4f cb4b  ...(.2."Bl5..O.K
-00006810: 576a abcf 182c 5322 f5c1 c08c 3885 3c08  Wj...,S"....8.<.
-00006820: 8187 9f87 8ac7 5a2c 6a46 859c 6e89 4c70  ......Z,jF..n.Lp
-00006830: e6c6 b216 1961 7712 c208 b7b5 0863 3c6f  .....aw......c<o
-00006840: 81ae ce72 2dba 08e3 1350 053b e782 3bbf  ...r-....P.;..;.
-00006850: 054b c472 d5d6 2e56 6edc 0fce 3f27 5363  .K.r...Vn...?'Sc
-00006860: fd4c ed97 6b7c c5ee eb6f b98a ab4f 7954  .L..k|...o...OyT
-00006870: d59f df96 577f db7d 7bae 1edf 8a2c e718  ....W..}{....,..
-00006880: d7ee 8bfb b5c5 cb46 70e9 3c66 3521 23ac  .......Fp.<f5!#.
-00006890: ff0e 06cb 0816 cef3 f595 cd6f 38dc eb67  ...........o8..g
-000068a0: 84ca 5ede acdc 7f51 dd7e c68f a509 f1e4  ..^....Q.~......
-000068b0: 1e03 5159 7d8a 1521 b8b9 c8d4 0577 1ed7  ..QY}..!.....w..
-000068c0: 161e 326a 0cc6 2916 05cf 1e11 0bfc dd46  ..2j..)........F
-000068d0: f5f5 05a6 51f9 f7b3 b533 3f04 eb1b c1fd  ....Q....3?.....
-000068e0: 3530 02e3 d1b0 2438 7311 f542 a267 5e71  50....$8s..B.g^q
-000068f0: 2c51 35e5 adab b545 62e3 ebec 16ec d440  ,Q5....Eb......@
-00006900: ac3f 14d3 61eb 6a9c 70d1 e7f9 e7c2 009c  .?..a.j.p.......
-00006910: 79a5 a9c6 92f4 688d b734 95cb 6f6a 8bdf  y.....h..4..oj..
-00006920: 091c ac21 0ad6 1e35 c284 62d8 8ca4 836f  ...!...5..b....o
-00006930: 5f06 cf7f 6b07 3082 ab31 6dfe f7d5 0291  _...k.0..1m.....
-00006940: 4404 aeba b4b8 bbb3 0c12 3032 06b4 f2db  D.........02....
-00006950: 5675 238c 6226 92d7 0660 1424 89bc f2e6  Vu#.b&...`.$....
-00006960: b3e0 f276 594d c3d6 ecd1 833f ff0d e322  ...vYM.....?..."
-00006970: d25c 5ad4 b500 0bfe 834c b33a 3142 aff7  .\Z......L.:1B..
-00006980: 410c 016f 494c ac05 474c 70e1 f7f2 daaf  A..oIL..GLp.....
-00006990: 9864 8700 4ca4 1aad 34aa 6fbf dbdd 3903  .d..L...4.o...9.
-000069a0: bd49 060b aeac 28d9 575f 110b 83de 3ac6  .I....(.W_....:.
-000069b0: 45ad b64b 74d2 dd23 d4b7 5d2d d947 030e  E..Kt..#..]-.G..
-000069c0: 3449 6b00 df71 789f b4b4 db00 b8e3 a85b  4Ik..qx........[
-000069d0: 9012 076f 31cd 980e aa8f 9683 8bab 3097  ...o1.........0.
-000069e0: da09 1c7a 83f2 8481 3387 4a2a ada0 ea7c  ...z....3.J*...|
-000069f0: 6e03 4eb2 ab15 9c30 e24f 16b1 ead4 ce6c  n.N....0.O.....l
-00006a00: 07af 7e67 56a7 1002 abce e28b 4488 ed67  ..~gV.......D..g
-00006a10: d527 f7aa 4f17 5a00 a123 5858 cd32 19ed  .'..O.Z..#XX.2..
-00006a20: ac25 54bd c356 80e5 95b3 c20f a7ae 6e79  .%T..V........ny
-00006a30: 7975 f7ed dda4 c187 1009 836f e048 1a7c  yu.........o.H.|
-00006a40: b423 3db5 d1ce 5a42 b51e bc42 a71d bc38  .#=...ZB...B...8
-00006a50: ca5b bc1d ac7e 131d bf81 d2ea dd15 6285  .[...~........b.
-00006a60: 1bb0 114e 24c2 0269 9421 2df1 4a05 0c07  ...N$..i.!-.J...
-00006a70: dd16 0d6d c036 6868 136f 6412 18b5 b36f  ...m.6hh.od....o
-00006a80: 6b3f fcdc 1e1f 9260 e37c 6885 37ca 87b6  k?.....`.|h.7...
-00006a90: 6808 c7d6 160d 6dc0 421f b41a 135c 5982  h.....m.B....\Y.
-00006aa0: 7791 682b 1444 92ad a8e3 48b4 1591 8e12  w.h+.D....H.....
-00006ab0: 2677 a4b3 9650 ada7 4bf5 d6a5 8625 2472  &w...P..K....%$r
-00006ac0: 5775 725c 7c1d f6e3 4ca8 42e1 5475 accd  Wur\|...L.B.Tu..
-00006ad0: 97de 66f0 f5ed dab9 af35 78af 5fe1 f106  ..f......5x._...
-00006ae0: 4b3b 4a12 4c3b 51a7 a315 755a 5a1b 751a  K;J.L;Q...uZZ.u.
-00006af0: 5a51 afa5 55b4 e569 7db2 883a ce13 9715  ZQ..U..i}..:....
-00006b00: bb2f fea7 bcfc 3b19 44a4 8edd 3b9c b9ad  ./....;.D...;...
-00006b10: 1d64 10a9 6307 22b7 4ae0 3830 1077 4bb6  .d..c.".J.80.wK.
-00006b20: e519 a4f0 ea85 a9ea 83cb 5bbb afdf 56ae  ..........[...V.
-00006b30: 6e40 6cc1 8b7f f252 ad3c ddc4 2c63 5624  n@l....R.<..,cV$
-00006b40: 280c a8d2 5663 7b5a 5e7a aaad 169b c0ed  (...Vc{Z^z......
-00006b50: 35b5 774a dc9a 2940 659b 824b 7718 e1a8  5.wJ..)@e..Kw...
-00006b60: fc83 caf5 57c1 ce79 6c2c e3c3 50d5 c18b  ....W..yl,..P...
-00006b70: 5f82 cd6b 893d 5537 36ab 4f7e 4ede 2722  _..k.=U76.O~N.'"
-00006b80: e6f6 dd32 3af9 5398 f480 4de5 c3e5 ff24  ...2:.S...M....$
-00006b90: aefd facf e597 6f91 7f09 ff42 01ee be78  ......o....B...x
-00006ba0: c1ee a6e3 70bc 4352 26f8 784e c0a3 a99d  ....p.CR&.xN....
-00006bb0: fdb6 75bf 148e ef97 8163 2580 1edf eb6f  ..u......c%....o
-00006bc0: 39da 3814 df27 8162 7b44 6fef 7dd0 b2c7  9.8..'.b{Do.}...
-00006bd0: 3814 df23 8162 7b44 6fef 89bc cf16 2225  8..#.b{Do....."%
-00006be0: 607c 9f14 8ced 5409 a08d 6e19 c024 91ee  `|....T...n..$..
-00006bf0: c1c8 eb12 2ecf f905 9a9e 5add bc20 66fd  ..........Z.. f.
-00006c00: c6a3 dadd 5b7f dadd d924 baaf da91 28e3  ....[....$....(.
-00006c10: 9e76 d58b 8fe9 9cb9 f936 b8bb cc84 d32a  .v.......6.....*
-00006c20: 577f c439 012a 0c74 575e 2341 e066 3dd0  W..9.*.tW^#A.f=.
-00006c30: 32f5 e56b 5bc1 957f 56ce bd28 3fd9 287f  2..k[...V..(?.(.
-00006c40: 2dc3 dc0f 54f2 5534 6656 07aa 5e5f adbc  -...T.U4fV..^_..
-00006c50: 7ea4 4e33 88c5 5dfa 06d1 b8da da3f 6a3f  ~.N3..]......?j?
-00006c60: 5c2d 5f3f 871f 64e2 4b34 e51f 7e09 ceae  \-_?..d.K4..~...
-00006c70: 2306 57be a681 0816 84cd 0544 7061 9be0  #.W........Dpa..
-00006c80: 78b5 5d7d b602 04d5 8d97 d50d 123a 57c3  x.]}.........:W.
-00006c90: 0963 8c97 9e94 ebd0 048d 2442 59cf 6061  .c........$BY.`a
-00006ca0: 492c b26f 5684 194d c00a 2655 175f 54ce  I,.oV..M..&U._T.
-00006cb0: deeb eb82 650e 96be e1a2 8775 4e8d 4d0d  ....e......uN.M.
-00006cc0: 8db4 860a b656 cabf 9c6f 079f 8244 626f  .....V...o...Dbo
-00006cd0: 6ba4 8853 0833 7d76 abbc b208 b3aa 1af0  k..S.3}v........
-00006ce0: b2c0 90a0 36c1 ad8b 5079 2d62 1549 0b2e  ....6...Py-b.I..
-00006cf0: 2f57 7efb 1a1c 537f 89f4 37af 95af be11  /W~...S...7.....
-00006d00: 618d 079b a4af c50b e214 6be7 49f9 e19b  a.........k.I...
-00006d10: 78dd 8025 6f9d 7bc6 09db b29d 3971 0e43  x..%o.{.....9q.C
-00006d20: 96a8 d567 3820 2b4b 240c 06b1 706d 1395  ...g8 +K$...pm..
-00006d30: 1dc1 f5f3 3c6e bd3a f466 2330 edbe bcd6  ....<n.:.f#0....
-00006d40: 829c 4973 9ea3 25b8 f122 78f4 03dc 4bcc  ..Is..%.."x...K.
-00006d50: ab38 9dc7 9dd3 76da 18f0 7087 845c f2a8  .8....v...p..\..
-00006d60: 5cbd 5db9 f013 df6e d499 1347 789a 865f  \.]....n...Gx.._
-00006d70: df0d 5eff c837 1cc9 e32d 8019 471c 5df1  ..^..7...-..G.].
-00006d80: 8d6b 77ae 60a4 0ccf 7024 80fb 3239 7088  .kw.`...p$..29p.
-00006d90: 501a 2c3c dd7d b9a6 e5f6 843f 8be3 a8a6  P.,<.}.....?....
-00006da0: b048 7bf4 0961 a34f 03f1 6544 5288 c0d3  .H{..a.O..eDR...
-00006db0: 7366 dec2 a18b c451 f03d 6308 b7c6 9953  sf.....Q.=c....S
-00006dc0: a906 21fc 1014 210d f5d1 c9eb cd82 8876  ..!...!........v
-00006dd0: 5c7d 54bb 794b d1c3 b372 dccd 1be2 f63a  \}T.yK...r.....:
-00006de0: e808 7969 0c65 4dcf 7332 0e64 6a7a c627  ..yi.eM.s2.djz.'
-00006df0: 7636 6de0 9cd2 1027 4644 f9eb bd28 e495  v6m....'FD...(..
-00006e00: 1b3b b5ef d7ab db77 8273 c41f 1e75 cc94  .;.....w.s...u..
-00006e10: 9375 7ce8 a538 04cb 96d2 c08f f3b9 63c8  .u|..8........c.
-00006e20: ff71 7173 489c 4595 0a60 ca3e 7a97 1243  .qqsH.E..`.>z..C
-00006e30: 08a0 76f6 62d2 1815 c742 6e6b 3446 315d  ..v.b....Bnk4F1]
-00006e40: e16a c132 858e 328e 3087 92c7 7266 2f79  .j.2..2.0...rf/y
-00006e50: 113e 2521 6cd2 c8e2 1427 0072 c727 9641  .>%!l....'.r.'.A
-00006e60: 561d 2771 c92c e366 1dd7 7033 0dc9 f30a  V.'q.,.f..p3....
-00006e70: 1922 931d b581 2c2a 698d 8a47 c96b 8c84  ."....,*i..G.k..
-00006e80: 983f 3506 d9ad 16a8 b2b9 5659 7d80 d460  .?5.......VY}..`
-00006e90: c48a a084 711c c3c8 fff3 e78d 31db 9f75  ....q.......1..u
-00006ea0: d3d0 bb39 dbf3 c5ec 2796 5ab6 069a dd9d  ...9....'.Z.....
-00006eb0: 4b22 0a4a 8d1c ceec 718a 0c5c 4d24 c404  K".J....q..\M$..
-00006ec0: 8000 31b2 ed1d 445f 3556 e0b8 9387 1550  ..1...D_5V.....P
-00006ed0: c7db 4577 ce11 b340 c3a4 3dd8 5a70 093b  ..Ew...@..=.Zp.;
-00006ee0: 37bd e551 dc0e 41f4 886e deda 03c8 4b1a  7..Q..A..n....K.
-00006ef0: cddb 4357 5e5a 2baf 5fe0 6d01 de48 11c9  ..CW^Z+._.m..H..
-00006f00: 1bc2 e624 a87b f9fa 231c d361 4517 8bfa  ...$.{..#..aE...
-00006f10: fac3 b8c8 86dc 1c6e 8d1b 53be 6b9d e424  .......n..S.k..$
-00006f20: 8126 c885 a8fc 444e e686 cc82 2392 484e  .&....DN....#.HN
-00006f30: d89e 5d84 42c4 1123 6bbd b27a bdc2 6628  ..].B..#k..z..f(
-00006f40: 4ccb f493 13b6 8f1b d990 5c3d 5521 8ea2  L.........\=U!..
-00006f50: 72e1 393c 532d e958 85f0 3843 1108 78ea  r.9<S-.X..8C..x.
-00006f60: 858c befd 57b0 84d5 6499 c9b9 0817 08b6  ....W...d.......
-00006f70: 4e11 a84c 4aa8 fc58 2d6d 3ccf 4075 5eda  N..LJ..X-m<.@u^.
-00006f80: 0565 b955 602c 3e0c 852c d970 c68c 258f  .e.U`,>..,.p..%.
-00006f90: 285c 1e76 5e23 fac6 77c2 afe3 a155 9726  (\.v^#..w....U.&
-00006fa0: a01d 1213 b429 6630 93b0 454d 7b02 46a5  .....)f0..EM{.F.
-00006fb0: db7c 868f e25c 5263 e8f4 cdc7 4abe 40a1  .|...\Rc....J.@.
-00006fc0: e58b 9261 9c67 aa6b 78a6 626a b483 266a  ...a.g.kx.bj..&j
-00006fd0: 93f1 8c92 c1a3 15a9 22b7 37e1 732a 5b11  ........".7.s*[.
-00006fe0: ef75 1017 76dd 53c2 7611 538d a0d3 4561  .u..v.S.v.S...Ea
-00006ff0: 7f19 c3f9 a9c8 c0d6 7b87 b84a 8308 4b70  ........{..J..Kp
-00007000: ee3a af17 49be 6583 5ce5 b4b5 ed67 d70d  .:..I.e.\....g..
-00007010: ae21 3821 84ad 31c0 619a 119b 87d6 2a03  .!8!..1.a.....*.
-00007020: 2d6c bb74 85b1 5ccd b643 2e9d 96cd 0438  -l.t..\..C.....8
-00007030: b671 38c1 1b09 707a 14d5 ed97 08e2 f16c  .q8...pz.......l
-00007040: 6d92 307c 1a4f dc78 d40a 62c7 2b76 7a52  m.0|.O.x..b.+vzR
-00007050: a4e5 2b97 1833 f431 6ca0 01c7 b099 49d7  ..+..3.1l.....I.
-00007060: f0e5 1a2e 0571 6122 db88 f2ce 0d20 8e43  .....qa"..... .C
-00007070: 8ce4 0aa6 5314 6bb4 427c c216 cf69 c15c  ....S.k.B|...i.\
-00007080: 434e 8d35 7832 6ba2 beae c805 6e45 8f6e  CN.5x2k.....nE.n
-00007090: 3cf6 dfd3 a0e3 66dd 19c7 42bf adb7 27ed  <.....f...B...'.
-000070a0: a107 fd2d f72d e50b c8a3 f91e f976 842b  ...-.-.......v.+
-000070b0: 32cd 51a4 0a1a a1c0 0867 a3de 262b 2fb5  2.Q......g..&+/.
-000070c0: 2844 a5c6 e350 4944 b53b 8488 70e7 91fe  (D...PID.;..p...
-000070d0: 3bee 284b 018d f876 8eee a356 b682 8595  ;.(K...v...V....
-000070e0: 7655 66f8 b435 8bbd 1c0d 0cfd b42a 7260  vUf..5.......*r`
-000070f0: 5a2b 1ed8 fab9 992d 211b 14bf f47a a736  Z+.....-!....z.6
-00007100: 77ca cb6b 0ba9 2bf7 7b09 ce5e e879 2a94  w..k..+.{..^.y*.
-00007110: 722d 2e3f 59e5 096e 6231 14fb 334a b7f7  r-.?Y..nb1..3J..
-00007120: 78a7 4418 c8f1 4128 2321 0bb6 beb0 6b92  x.D...A(#!....k.
-00007130: 6045 06a9 40b0 858d 20d5 27e5 13e8 b429  `E..@... .'....)
-00007140: e681 f0c3 dae3 e59c dd8a f711 f372 b0d3  .............r..
-00007150: 13ee 6e3e 4d63 0432 e557 6507 c691 88a4  ..n>Mc.2.We.....
-00007160: 3b92 1828 2c0e 5982 6ede 0a76 762a 2f56  ;..(,.Y.n..vv*/V
-00007170: e0c4 6b50 4141 b0f7 c61e 4744 1d9a d97c  ..kPAA....GD...|
-00007180: 84f1 c968 da41 01f6 4573 4bc9 a040 49cb  ...h.A..EsK..@I.
-00007190: 0544 6538 9edd 52a9 b74c 3a73 234f 36cc  .De8..R..L:s#O6.
-000071a0: 236e a883 b08b 4c52 b1b2 e8b0 8bda 2517  #n....LR......%.
-000071b0: f6d5 b2ed 7498 171d b5e6 6a19 1688 5bda  ....t.....j...[.
-000071c0: b0ea 9357 8827 2676 532a 62d2 e359 344c  ...W.'&vS*b..Y4L
-000071d0: d77d 206e 2445 1b43 c739 3589 e445 3310  .} n$E.C.95..E3.
-000071e0: e5cb 885c 7e1f 7cf7 0ddc 8478 ebe6 1a83  ...\~.|....x....
-000071f0: ad70 16ef b889 408d 0c7a 1c73 4b29 1f8f  .p....@..z.sK)..
-00007200: 2018 c770 b78c 9a3a 1981 1361 d9f3 cf81   ..p...:...a....
-00007210: b9fc 720b 1325 b8ff b83d fcf5 48dd bc31  ..r..%...=..H..1
-00007220: 91f2 5ca4 e322 4599 3e4a 575e be56 5d5a  ..\.."E.>JW^.V]Z
-00007230: 86ab 57be 7a1f 6388 a33e 66e3 514b cb51  ..W.z.c..>f.QK.Q
-00007240: e64f c867 2087 8dbd e3c9 8238 30d5 0035  .O.g ......80..5
-00007250: b119 76b5 b3b8 33cd a262 0f7d 07b9 ca33  ..v...3..b.}...3
-00007260: a0ef bad0 73b2 8dc4 5983 1f6f 613d a66c  ....s...Y..oa=.l
-00007270: b2f0 f627 540e 4aa2 7ec0 7751 3134 3c58  ...'T.J.~.wQ14<X
-00007280: a20f c1aa 18eb 3e70 b619 7ee5 3136 883b  ......>p..~.16.;
-00007290: 66c7 a944 b850 13e9 6bc4 3af7 4165 fb61  f..D.P..k.:.Ae.a
-000072a0: d07d 206d 3f42 ba9f d1c7 a3a6 bccf a242  .} m?B.........B
-000072b0: db08 81ec 0375 9b81 d488 5fc5 9f00 10b7  .....u...._.....
-000072c0: 287a ab44 c4b7 2d1f 2b9f 087c c669 c7da  (z.D..-.+..|.i..
-000072d0: 2c62 bcd2 85e0 710f 8937 a620 78e9 6ec1  ,b....q..7. x.n.
-000072e0: 5c26 44b0 e028 dcb8 9584 4b6f dd13 b0ae  \&D..(....Ko....
-000072f0: fd0a 8eb6 08b2 4922 8f8b e72f e5c8 072c  ......I".../...,
-00007300: 04dd 3c0c 5839 64ed 86e0 42e3 941c cf8b  ..<.X9d...B.....
-00007310: ae49 6d23 8e44 e514 9745 5881 5e2d 92c3  .Im#.D...EX.^-..
-00007320: 18c9 671a 0361 6275 c4a2 b2b8 a9bf 2571  ..g..abu......%q
-00007330: 4f94 fc7d 210f e33c 09ea c1ab 5ec4 ddd4  O..}!..<....^...
-00007340: eb9e dae2 27f1 236a 2ac5 f247 3cae 735f  ....'.#j*..G<.s_
-00007350: 63c2 3531 d051 8b56 30ae 69db ced9 e48a  c.51.Q.V0.i.....
-00007360: 2f76 97b5 854b 2a4f 5d04 0be5 5c50 3eab  /v...K*O]...\P>.
-00007370: d65b 9d34 e913 9f61 0c45 e621 f182 ddab  .[.4...a.E.!....
-00007380: f8f5 f01f 31b6 bc65 09c3 e812 7d1c 8267  ....1..e....}..g
-00007390: 7f43 6d12 667e b0b2 85dc 99e0 f5e3 da6d  .Cm.f~.........m
-000073a0: dcd8 2049 3cc3 78bc d5f2 857f 54df 1fa9  .. I<.x.....T...
-000073b0: bb47 4372 afe4 89bd b0d4 28b1 e0cb 1f62  .GCr......(....b
-000073c0: 2ecc e180 467b aea5 ed2a 3c7d 1076 2682  ....F{...*<}.v&.
-000073d0: a4b9 4ed6 97a2 f8d8 43b9 e392 c28f b782  ..N.....C.......
-000073e0: e53b 4c8a 17bb 9ab5 4db6 8842 2ddd 6c1e  .;L.....M..B-.l.
-000073f0: c122 c1e0 fc73 1c25 c20b 64fa d2a2 3506  ."...s.%..d...5.
-00007400: 6ddc 0213 f7c9 c800 e4b9 1102 5622 5250  m...........V"RP
-00007410: d71e 5c8f 89c3 c5ac 5bd3 6f4f b0eb 6aca  ..\.....[.oO..j.
-00007420: ee17 b59a b7f2 4854 bb64 344e 75f6 4775  ......HT.d4Nu.Gu
-00007430: 3b3a 29ce 9ad7 7f39 38c7 87f3 e2dd 7632  ;:)....98.....v2
-00007440: 9bfe 7137 78f6 804f 781a 2fe5 5238 5c15  ..q7x..Ox./.R8\.
-00007450: ea9e 2b64 dd79 9b59 2a25 712a 0b8b 4828  ..+d.y.Y*%q*..H(
-00007460: 7212 a06e 1fe2 88d1 f34a 88af 4fcf ba25  r..n.....J..O..%
-00007470: 4fcc 1279 2991 3af0 cb77 603e 82e7 4f70  O..y).:..w`>..Op
-00007480: ed88 c7fd 858d b79e 7d71 bc8d 3094 3963  ........}q..0.9c
-00007490: 1b30 e2f2 257a 2126 85b4 d109 d1b0 8d05  .0..%z!&........
-000074a0: 2641 0e3b 33ee b6b5 dabc 9e98 188e 63c1  &A.;3.........c.
-000074b0: 6103 5e4f 54f3 1ff3 3e5c f506 7477 1aeb  a.^OT...>\..tw..
-000074c0: 7806 3478 8042 8510 555c cbd0 2252 1b58  x.4x.B..U\.."R.X
-000074d0: 1544 4cbc 1c59 8f20 0a12 1d72 8b5d 24e9  .DL..Y. ...r.]$.
-000074e0: dc87 757f 0a03 afb9 cd28 42b0 e270 2d7a  ..u......(B..p-z
-000074f0: a397 4716 6e29 7497 1af7 0c2c e18e 5e78  ..G.n)t....,..^x
-00007500: b52a 194d c8e8 a4ab 7ed1 60a6 0e59 7d83  .*.M....~.`..Y}.
-00007510: 2692 15a2 c1ec a4bb 9735 194e 474e 23c3  &........5.NGN#.
-00007520: b001 cb81 5a6b 8f73 f846 f523 1c56 4251  ....Zk.s.F.#.VBQ
-00007530: e3a7 692e 5687 a683 d734 812c 3e75 38c1  ..i.V....4.,>u8.
-00007540: 638a 9e43 b08d a341 2b66 f48d 1847 a874  c..C...A+f...G.t
-00007550: 8957 7215 2e1c e7d5 7e58 0fce 5c62 d6d9  .Wr.....~X..\b..
-00007560: 6927 27d3 11ea c130 dc3c 661c 1579 b6ba  i''....0.<f..y..
-00007570: fbe6 2636 834c 3e6c f4f0 a176 e631 7fe5  ..&6.L>l...v.1..
-00007580: 90c9 f631 a635 afa9 47d3 745a 230c 7785  ...1.5..G.tZ#.w.
-00007590: 5a6c 6a07 abc5 d30c 42e8 c811 a753 f214  Zlj.....B....S..
-000075a0: 408b 63cf b4d3 8e4a 5e67 d4e2 0867 9bae  @.c....J^g...g..
-000075b0: 7534 fd48 8b23 32bd f4cc 95eb 88ca ca0a  u4.H.#2.........
-000075c0: eeff c4e8 c431 733e 1a11 f0a2 169f 6ce0  .....1s>......l.
-000075d0: 2436 9554 9580 2d94 511b a890 b083 9cae  $6.T..-.Q.......
-000075e0: 0454 91a0 5173 2122 64e1 aabe 8ca9 8255  .T..Qs!"d......U
-000075f0: cc13 0b7b 63aa 43f3 164d ec51 97ae 949d  ...{c.C..M.Q....
-00007600: 8c63 1f74 dd93 32e6 6e37 6fe8 1b64 b969  .c.t..2.n7o..d.i
-00007610: 5edb 7ab0 c907 b1d5 15f4 8417 0364 5266  ^.z..........dRf
-00007620: 426c 98c4 855b e18a 5cac 8f0f 2a72 b93b  Bl...[..\...*r.;
-00007630: 090b fc97 c80b 7b91 4cd1 e660 ea2e 0cf1  ......{.L..`....
-00007640: 062e 2c31 6781 c1e6 3dc6 a604 cfef 7129  ..,1g...=.....q)
-00007650: afba 5cf6 46ae 2bd9 a0e0 6c2f 5ef6 091c  ..\.F.+...l/^...
-00007660: 9a78 d9a8 7b8a 3855 e2c3 15f1 4271 d262  .x..{.8U....Bq.b
-00007670: 1bc7 dc6c d62c 1267 6aba 68e6 3d13 9e2b  ...l.,.gj.h.=..+
-00007680: 7d75 e6c4 c448 1c95 6ea6 4f0e 9f30 a6bf  }u...H..n.O..0..
-00007690: 9822 6ed0 e420 5ffe b99b 2de5 6cbc fcdb  ."n.. _...-.l...
-000076a0: d5a5 71f2 464d cf37 06e9 c651 964f 709f  ..q.FM.7...Q.Op.
-000076b0: c9a8 fb7a 1851 1a4a ce7d 2b44 7011 8738  ...z.Q.J.}+Dp..8
-000076c0: a770 aa41 dfe3 91ce 67dd 3b4c a00c 0f27  .p.A....g.;L...'
-000076d0: 9cc4 f906 76a4 3a9e 4620 a096 e20d 0bf8  ....v.:.F ......
-000076e0: a084 9592 4c25 1b3d 54fd f8c5 f8d2 1129  ....L%.=T......)
-000076f0: 7d1c 8fe5 5627 0e37 fcd7 787f 9f8a 6f0e  }...V'.7..x...o.
-00007700: 0ce2 4173 f09e ad9b 128f abeb 2a45 c301  ..As........*E..
-00007710: fac8 bc44 2a1b 6a2b 45a6 8ff1 899b 15db  ...D*.j+E.......
-00007720: 0b63 927e 9ee4 b8f8 be80 862e 59a7 a3ab  .c.~........Y...
-00007730: d190 e9ba d950 5bd9 8aae 6336 76e6 4579  .....P[...c6v.Ey
-00007740: 7a8d b45c dfc4 fbce 1a2a 1948 1dcd 1aa4  z..\.....*.H....
-00007750: 0c91 3aa4 7ad0 4ff0 3eb9 dd82 4605 d382  ..:.z.O.>...F...
-00007760: ba26 a256 9de9 241f 122f f3a4 9264 af7c  .&.V..$../...d.|
-00007770: 100d 5b55 a58e d666 5386 c848 53a6 367c  ..[U...fS..HS.6|
-00007780: f964 323c d08a 4f86 b09a cb9c 0dab 064d  .d2<..O........M
-00007790: 6432 e0ac 8999 2c72 328a e059 aec0 99d4  d2....,r2..Y....
-000077a0: 10c1 a725 64a4 e9fa 955f 0c18 125f ec11  ...%d...._..._..
-000077b0: e976 8950 0984 d447 21b1 d5e1 f4cc 50a2  .v.P...G!.....P.
-000077c0: 9284 27d0 3d25 b125 510f 3fcc 1006 584c  ..'.=%.%Q.?...XL
-000077d0: 7686 3d21 5551 2886 a6a9 c151 d861 f13d  v.=!UQ(....Q.a.=
-000077e0: 05b5 4033 88e2 2089 58d4 66dc e308 6ae2  ..@3.. .X.f...j.
-000077f0: 49e0 6513 2869 e863 c8ac c1a3 ee52 33d8  I.e.(i.c.....R3.
-00007800: 5dd2 1e91 b484 0e37 1f46 4bc0 18cb 5bac  ]......7.FK...[.
-00007810: ab51 68c6 1ad7 9307 3d1f dff1 13a9 8ef2  .Qh.....=.......
-00007820: 2351 6aa1 1e75 e961 eaa4 f82a 423d 25b2  #Qj..u.a...*B=%.
-00007830: 25f4 1072 5014 decf f269 1857 dc0f c372  %..rP....i.W...r
-00007840: 8c53 32d5 ad58 2590 3644 9c9a e456 1c59  .S2..X%.6D...V.Y
-00007850: da8e 9821 3761 47f1 f814 a89a 46bc 76df  ...!7aG.....F.v.
-00007860: a425 b44d 2690 6d98 4ca6 e0d8 a0ed 9fb2  .%.M&.m.L.......
-00007870: f109 01c1 425c 7a6b 9783 92db 7cdb 1664  ....B\zk....|..d
-00007880: 729d b64f a620 11f7 e4de 89cc bd6d f741  r..O. .......m.A
-00007890: 66bd 61fb 640a 12a5 ebd7 a642 ee61 67ac  f.a.d......B.ag.
-000078a0: f13e 086d b44c a4f4 639c 8123 e6a1 f453  .>.m.L..c..#...S
-000078b0: 52b9 9fb9 93d8 3a99 564d 5386 583c 5007  R.....:.VMS.X<P.
-000078c0: 6f57 9c21 aa05 e538 59bf d459 a03a 67d4  oW.!...8Y..Y.:g.
-000078d0: c18c 993e 3e9b 25dc 45bb e8b8 e40c 6a0a  ...>>.%.E.....j.
-000078e0: 5fbd 4046 9208 1487 2b8d 0ed1 71f1 218c  _.@F....+...q.!.
-000078f0: 6376 d6c1 623a af25 49e1 135f 3115 c16c  cv..b:.%I.._1..l
-00007900: e9e9 6604 9fa3 a692 0e04 99ec 057c 5214  ..f..........|R.
-00007910: 198d aa77 34c5 83ff 7d5d 467b a093 c3a7  ...w4...}]F{....
-00007920: f703 8bab 741c e283 7fae 41bc d2af befa  ....t.....A.....
-00007930: 70f0 c7fa 87c7 3ffe c370 fd41 df7f 500e  p.....?..p.A..P.
-00007940: c498 f870 6096 7c6e 6d4f a521 7696 5fda  ...p`.|nmO.!v._.
-00007950: f449 e92f dd2f 8d10 81f2 4788 4be6 8e25  .I././....G.K..%
-00007960: 03a8 7eb0 a097 72a5 2ca6 30d5 68f9 ae9f  ..~...r.,.0.h...
-00007970: 0048 a442 0248 645c 7800 d1e5 6432 c4ee  .H.B.Hd\x...d2..
-00007980: 9700 195f 8ed1 f188 cf2c 2aa2 8596 e361  ..._.....,*....a
-00007990: 484c 35d7 90bb 67c9 89b0 72cc 256d b1b9  HL5...g...r.%m..
-000079a0: 6e49 0707 b30f 32a2 cdf5 84d4 073b 2152  nI....2......;!R
-000079b0: 9d25 4dc8 1133 44e8 58c7 bb26 e448 dee8  .%M..3D.X..&.H..
-000079c0: ee21 43a3 18a7 4cc4 3024 4328 4edf e818  .!C...L.0$C(N...
-000079d0: b74f 299e 0173 8788 3a00 6fc7 b86a 409c  .O)..s..:.o..j@.
-000079e0: 9ca6 8e70 7def ad95 4a62 e874 5568 8982  ...p}...Jb.tUh..
-000079f0: 6706 1141 7498 8c70 4f65 9b9a 6850 3450  g..At..pOe..hP4P
-00007a00: 0b91 a555 0a85 4301 3e75 3f4d 0688 0519  ...U..C.>u?M....
-00007a10: 8d29 2c06 3889 6159 1d87 153d c7c5 c1c1  .),.8.aY...=....
-00007a20: e8d9 dc08 252a 2219 fa45 2845 8490 b4e1  ....%*"..E(E....
-00007a30: 1259 a90b 3de8 2ac3 5db3 da7e eb81 909d  .Y..=.*.]..~....
-00007a40: 11c6 dd75 bb0c 84a7 986d a308 5a0d ba26  ...u.....m..Z..&
-00007a50: fd8a d448 f8fd aa78 9b7a b931 4cb7 a1a3  ...H...x.z.1L...
-00007a60: f253 759f e1fb 5958 27dd 5324 5e19 af17  .Su...YX'.S$^...
-00007a70: 9746 11f9 1547 faed 2d90 e246 3a16 54a3  .F...G..-..F:.T.
-00007a80: a3ad e554 9aa6 460c acad 2663 4e1a 213c  ...T..F...&cN.!<
-00007a90: b851 5c17 5322 e358 dc41 9cc6 77a3 8d21  .Q\.S".X.A..w..!
-00007aa0: 3823 b876 46b4 6a0f 1098 9475 3c12 a41d  8#.vF.j....u<...
-00007ab0: 9089 f7c6 7184 58e9 478d 115a 568f 491a  ....q.X.G..ZV.I.
-00007ac0: d334 6027 63aa b438 f6ce 24db 5244 5d75  .4`'c..8..$.RD]u
-00007ad0: 2d55 241c 077d 6ccb 29b6 258e 790d dffe  -U$..}l.).%.y...
-00007ae0: 7b9c 01f8 a22f 5bec b1c5 2a2a 2a71 bce3  {..../[...***q..
-00007af0: 575c 6454 4f37 ef98 80d9 7e41 5b85 bb74  W\dTO7....~A[..t
-00007b00: f8d4 66a1 8d5a 7dfc a58d 084d 3320 a289  ..f..Z}....M3 ..
-00007b10: 09d5 71b0 6641 c430 3a54 50a5 23a1 3326  ..q.fA.0:TP.#.3&
-00007b20: 5122 2114 ae4b e089 1388 e374 17b9 8522  Q"!..K.....t..."
-00007b30: 0ddd 2ea6 ccfc 4943 8892 ac81 a3e2 439e  ......IC......C.
-00007b40: d336 3e9d d8c6 3b0b a942 1f79 e8be bcfd  .6>...;..B.y....
-00007b50: bcfc eb3d fe46 db84 9395 778f 3ec6 f578  ...=.F....w.>..x
-00007b60: fe76 10be 9cd0 17a7 bcf9 3e80 f60a ee00  .v........>.....
-00007b70: 7922 20e1 765a f31a 7afd 743f e1ba 2177  y" .vZ..z.t?..!w
-00007b80: db3b 01f7 1ef0 e899 7d42 1bee 6673 02b8  .;......}B..fs..
-00007b90: 5220 29a2 e6bd 4264 48c8 ebd1 b876 3592  R )...BdH....v5.
-00007ba0: f77c c797 5fda 4c90 eebe 9bf2 dd0a 3a0f  .|.._.L.......:.
-00007bb0: d075 fbcd 2543 b085 28e2 084d 2c60 babb  .u..%C..(..M,`..
-00007bc0: b9ca 0e44 d8a7 5134 7c35 2451 75f7 7ff3  ...D..Q4|5$Qu...
-00007bd0: adb5 72e3 8332 e4db 09b8 4ebb fb1a 6fc5  ..r..2....N...o.
-00007be0: 3e57 3f1a 7756 9887 f3e5 cd82 e69d c1a9  >W?.wV..........
-00007bf0: 52ca 73d2 8e38 1409 9fc5 4fa9 67f1 7149  R.s..8....O.g.qI
-00007c00: 1cb7 221c f155 55b2 cbc1 7769 c817 3df0  .."..UU...wi..=.
-00007c10: 3c89 b8ee b48f 2b5e 2a5f 2072 8baa fe3a  <.....+^*_ r...:
-00007c20: 0051 38f4 7738 3e9f 45ba dcc3 e576 efb9  .Q8.w8>.E....v..
-00007c30: 1d2f 218b 0bb9 2622 176d 4206 f499 4ee8  ./!...&".mB...N.
-00007c40: 274e a297 cc54 8274 7b57 e2da c993 e608  'N...T.t{W......
-00007c50: 20a3 dc43 c0bb dec9 d365 6a53 0a98 afb2   ..C.....ejS....
-00007c60: c006 8bab fc2b e2b9 6bed 7db6 30a9 d7f9  .....+..k.}.0...
-00007c70: 6fec 2f75 732a e1eb 07ad a7e5 21cf f38f  o./us*......!...
-00007c80: fe1f 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00007c90: 0008 0000 0021 003b 6d32 4bc1 0000 0042  .....!.;m2K....B
-00007ca0: 0100 0023 0000 0078 6c2f 776f 726b 7368  ...#...xl/worksh
-00007cb0: 6565 7473 2f5f 7265 6c73 2f73 6865 6574  eets/_rels/sheet
-00007cc0: 312e 786d 6c2e 7265 6c73 848f c18a c230  1.xml.rels.....0
-00007cd0: 1445 f703 fe43 787b 93d6 850c 4353 3722  .E...Cx{....CS7"
-00007ce0: b855 e703 62fa da06 db97 90f7 14fd 7bb3  .U..b.........{.
-00007cf0: 1c65 c0e5 e570 cfe5 369b fb3c a91b 660e  .e...p..6..<..f.
-00007d00: 912c d4ba 0285 e463 1768 b0f0 7bda 2dbf  .,.....c.h..{.-.
-00007d10: 41b1 38ea dc14 092d 3c90 61d3 2ebe 9a03  A.8....-<.a.....
-00007d20: 4e4e 4a89 c790 5815 0bb1 8551 24fd 18c3  NNJ...X....Q$...
-00007d30: 7ec4 d9b1 8e09 a990 3ee6 d949 8979 30c9  ~.......>..I.y0.
-00007d40: f98b 1bd0 acaa 6a6d f25f 07b4 2f4e b5ef  ......jm._../N..
-00007d50: 2ce4 7d57 833a 3d52 59fe ec8e 7d1f 3c6e  ,.}W.:=RY...}.<n
-00007d60: a3bf ce48 f2cf 8449 3990 603e a248 39c8  ...H...I9.`>.H9.
-00007d70: 45ed f280 6241 eb77 f69e 6b7d 0e04 a66d  E...bA.w..k}...m
-00007d80: cccb f3f6 0900 00ff ff03 0050 4b03 0414  ...........PK...
-00007d90: 0006 0008 0000 0021 0013 c42c 13c2 0000  .......!...,....
-00007da0: 0042 0100 0023 0000 0078 6c2f 776f 726b  .B...#...xl/work
-00007db0: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
-00007dc0: 6574 322e 786d 6c2e 7265 6c73 848f c16a  et2.xml.rels...j
-00007dd0: c330 1044 ef85 fc83 d87b 243b 8750 8a25  .0.D.....{$;.P.%
-00007de0: 5f4a 21d7 26fd 0045 5edb a2f6 4a68 b725  _J!.&..E^...Jh.%
-00007df0: f9fb e8d8 8442 8ec3 63de 305d 7f59 17f5  .....B..c.0].Y..
-00007e00: 8b85 6322 0bad 6e40 2185 3444 9a2c 7c9d  ..c"..n@!.4D.,|.
-00007e10: 3eb6 afa0 583c 0d7e 4984 16ae c8d0 bbcd  >...X<.~I.......
-00007e20: 4bf7 898b 975a e239 6656 d542 6c61 16c9  K....Z.9fV.Bla..
-00007e30: 6fc6 7098 71f5 ac53 46aa 644c 65f5 5263  o.p.q..SF.dLe.Rc
-00007e40: 994c f6e1 db4f 6876 4db3 37e5 af03 dc9d  .L...OhvM.7.....
-00007e50: 531d 060b e530 b4a0 4ed7 5c97 9fbb d338  S....0..N.\....8
-00007e60: c680 ef29 fcac 48f2 cf84 c925 9260 39a2  ...)..H....%.`9.
-00007e70: 483d c855 edcb 8462 41eb 47f6 9877 fa1c  H=.U...bA.G..w..
-00007e80: 098c ebcc dd73 7703 0000 ffff 0300 504b  .....sw.......PK
-00007e90: 0304 1400 0600 0800 0000 2100 34a1 0992  ..........!.4...
-00007ea0: c200 0000 4201 0000 2300 0000 786c 2f77  ....B...#...xl/w
-00007eb0: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
-00007ec0: 7368 6565 7433 2e78 6d6c 2e72 656c 7384  sheet3.xml.rels.
-00007ed0: 8fc1 6ac3 3010 44ef 81fc 83d8 7b24 2785  ..j.0.D.....{$'.
-00007ee0: 5282 e55c 4220 d736 fd00 555e cb22 f64a  R..\B .6..U^.".J
-00007ef0: 68b7 a5f9 fbea 589b 428f c363 de30 ede9  h.....X.B..c.0..
-00007f00: 7b9e d417 168e 892c ec75 030a c9a7 3e52  {......,.u....>R
-00007f10: b0f0 7ebb ec5e 40b1 38ea dd94 082d 3c90  ..~..^@.8....-<.
-00007f20: e1d4 6d37 ed2b 4e4e 6a89 c798 5955 0bb1  ..m7.+NNj...YU..
-00007f30: 8551 241f 8d61 3fe2 ec58 a78c 54c9 90ca  .Q$..a?..X..T...
-00007f40: eca4 c612 4c76 feee 029a 43d3 3c9b f2db  ....Lv....C.<...
-00007f50: 01dd c2a9 aebd 8572 edf7 a06e 8f5c 97ff  .......r...n.\..
-00007f60: 77a7 6188 1ecf c97f ce48 f2c7 84c9 2592  w.a......H....%.
-00007f70: 6079 4391 7a90 abda 9580 6241 eb35 5be7  `yC.z.....bA.5[.
-00007f80: 27fd 1109 4cd7 9ac5 f3ee 0700 00ff ff03  '...L...........
-00007f90: 0050 4b03 0414 0006 0008 0000 0021 0043  .PK..........!.C
-00007fa0: 9611 a3c2 0000 0042 0100 0023 0000 0078  .......B...#...x
-00007fb0: 6c2f 776f 726b 7368 6565 7473 2f5f 7265  l/worksheets/_re
-00007fc0: 6c73 2f73 6865 6574 342e 786d 6c2e 7265  ls/sheet4.xml.re
-00007fd0: 6c73 848f c16a c330 1044 ef81 fc83 d87b  ls...j.0.D.....{
-00007fe0: 2427 9452 82e5 5c42 20d7 36fd 0055 5ecb  $'.R..\B .6..U^.
-00007ff0: 22f6 4a68 b7a5 f9fb ea58 9b42 8fc3 63de  ".Jh.....X.B..c.
-00008000: 30ed e97b 9ed4 1716 8e89 2cec 7503 0ac9  0..{......,.u...
-00008010: a73e 52b0 f07e bbec 5e40 b138 eadd 9408  .>R..~..^@.8....
-00008020: 2d3c 90e1 d46d 37ed 2b4e 4e6a 89c7 9859  -<...m7.+NNj...Y
-00008030: 550b b185 5124 1f8d 613f e2ec 58a7 8c54  U...Q$..a?..X..T
-00008040: c990 caec a4c6 124c 76fe ee02 9a43 d33c  .......Lv....C.<
-00008050: 9bf2 db01 ddc2 a9ae bd85 72ed f7a0 6e8f  ..........r...n.
-00008060: 5c97 ff77 a761 881e cfc9 7fce 48f2 c784  \..w.a......H...
-00008070: c925 9260 7943 917a 90ab da95 8062 41eb  .%.`yC.z.....bA.
-00008080: 355b e727 fd11 094c d79a c5f3 ee07 0000  5[.'...L........
-00008090: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-000080a0: 2100 64f3 3422 c200 0000 4201 0000 2300  !.d.4"....B...#.
-000080b0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000080c0: 5f72 656c 732f 7368 6565 7435 2e78 6d6c  _rels/sheet5.xml
-000080d0: 2e72 656c 7384 8fc1 6ac3 3010 44ef 81fc  .rels...j.0.D...
-000080e0: 83d8 7b24 27d0 5282 e55c 4220 d736 fd00  ..{$'.R..\B .6..
-000080f0: 555e cb22 f64a 68b7 a5f9 fbea 589b 428f  U^.".Jh.....X.B.
-00008100: c363 de30 ede9 7b9e d417 168e 892c ec75  .c.0..{......,.u
-00008110: 030a c9a7 3e52 b0f0 7ebb ec5e 40b1 38ea  ....>R..~..^@.8.
-00008120: dd94 082d 3c90 e1d4 6d37 ed2b 4e4e 6a89  ...-<...m7.+NNj.
-00008130: c798 5955 0bb1 8551 241f 8d61 3fe2 ec58  ..YU...Q$..a?..X
-00008140: a78c 54c9 90ca eca4 c612 4c76 feee 029a  ..T.......Lv....
-00008150: 43d3 3c9b f2db 01dd c2a9 aebd 8572 edf7  C.<..........r..
-00008160: a06e 8f5c 97ff 77a7 6188 1ecf c97f ce48  .n.\..w.a......H
-00008170: f2c7 84c9 2592 6079 4391 7a90 abda 9580  ....%.`yC.z.....
-00008180: 6241 eb35 5be7 27fd 1109 4cd7 9ac5 f3ee  bA.5[.'...L.....
-00008190: 0700 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000081a0: 0000 0021 00e8 f726 32a9 0100 0054 0f00  ...!...&2....T..
-000081b0: 0027 0000 0078 6c2f 7072 696e 7465 7253  .'...xl/printerS
-000081c0: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-000081d0: 6574 7469 6e67 7331 2e62 696e ec57 b94e  ettings1.bin.W.N
-000081e0: c340 107d bb36 71a2 8810 2828 517a 84c4  .@.}.6q...((Qz..
-000081f0: 1104 8826 1202 8906 1091 2042 2938 9282  ...&...... B)8..
-00008200: a340 1c22 e99c 8e96 36d4 fc03 1f42 49c1  .@."....6....BI.
-00008210: 6750 61de ac73 1870 0428 4713 bfd5 dad6  gPa..s.p.(G.....
-00008220: ceec 78fc 7676 c65b 4411 3728 e30c 33b8  ..x.vv.[D.7(..3.
-00008230: c335 6ed9 8b58 c70e f2d8 c616 32d8 c706  .5n..X......2...
-00008240: 656b 58c4 1256 b0cb 913c f5af 700a 81b2  ekX..V...<..p...
-00008250: a15f 5149 8d3d ba8e 4202 f564 365e 8282  ._QI.=..B..d6^..
-00008260: 8382 56bc 1734 758c 66ef 2f62 97e6 3bda  ..V..4u.f./b..;.
-00008270: afa4 2823 4429 e8c3 32e7 b8a3 c033 7b8e  ..(#D)..2....3{.
-00008280: cfef bcbb 01f7 c661 db7f 63a0 4cb6 c221  .......a..c.L..!
-00008290: 7e09 d2f4 a109 f141 c1e2 759a bc14 b463  ~......A..u....c
-000082a0: 0409 64e3 f5e4 14fc 26cf abd6 832d ba31  ..d.....&....-.1
-000082b0: 4c86 1817 cbb1 d6b8 794f e3fb 9aef 0cf7  L.......yO......
-000082c0: 281a 8d18 8818 1846 0624 e3d8 ec25 b660  (......F.$...%.`
-000082d0: ae49 04c8 f0bc 2033 fdca d851 fc0d 1f03  .I.... 3...Q....
-000082e0: 9ab1 d7ae 4c0a f36c 2f1f 83e3 41fe 427c  ....L..l/...A.B|
-000082f0: d8b2 09c2 9181 ebc4 6d6a 4aeb acd6 8dd7  ........mjJ.....
-00008300: 0d2f fca2 6f0c 69f2 126b 7193 4e79 849e  ./..o.i..kq.Ny..
-00008310: 1591 85b7 a898 47c9 a26b 0634 23a9 1d48  ......G..k.4#..H
-00008320: 1677 5e09 977d da7b 3f6b 86fc 786f febe  .w^..}.{?k..xo..
-00008330: f77a b6ce c7b8 c011 4e70 dec1 e21c bf7f  .z......Np......
-00008340: 01d9 81c6 5554 49ff 47f7 3dd1 ed02 1d54  ....UTI.G.=....T
-00008350: 750d eac9 e4fd c3b4 7fc6 6b9f 98be 5bff  u.........k...[.
-00008360: ba42 7b0d b10b 1e61 09bf 168c 98d3 5970  .B{....a......Yp
-00008370: a682 6726 d626 5af3 7322 97f3 e627 0000  ..g&.&Z.s"...'..
-00008380: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00008390: 0021 00e8 f726 32a9 0100 0054 0f00 0027  .!...&2....T...'
-000083a0: 0000 0078 6c2f 7072 696e 7465 7253 6574  ...xl/printerSet
-000083b0: 7469 6e67 732f 7072 696e 7465 7253 6574  tings/printerSet
-000083c0: 7469 6e67 7332 2e62 696e ec57 b94e c340  tings2.bin.W.N.@
-000083d0: 107d bb36 71a2 8810 2828 517a 84c4 1104  .}.6q...((Qz....
-000083e0: 8826 1202 8906 1091 2042 2938 9282 a340  .&...... B)8...@
-000083f0: 1c22 e99c 8e96 36d4 fc03 1f42 49c1 6750  ."....6....BI.gP
-00008400: 61de ac73 1870 0428 4713 bfd5 dad6 ceec  a..s.p.(G.......
-00008410: 78fc 7676 c65b 4411 3728 e30c 33b8 c335  x.vv.[D.7(..3..5
-00008420: 6ed9 8b58 c70e f2d8 c616 32d8 c706 656b  n..X......2...ek
-00008430: 58c4 1256 b0cb 913c f5af 700a 81b2 a15f  X..V...<..p...._
-00008440: 5149 8d3d ba8e 4202 f564 365e 8282 8382  QI.=..B..d6^....
-00008450: 56bc 1734 758c 66ef 2f62 97e6 3bda afa4  V..4u.f./b..;...
-00008460: 2823 4429 e8c3 32e7 b8a3 c033 7b8e cfef  (#D)..2....3{...
-00008470: bcbb 01f7 c661 db7f 63a0 4cb6 c221 7e09  .....a..c.L..!~.
-00008480: d2f4 a109 f141 c1e2 759a bc14 b463 0409  .....A..u....c..
-00008490: 64e3 f5e4 14fc 26cf abd6 832d ba31 4c86  d.....&....-.1L.
-000084a0: 1817 cbb1 d6b8 794f e3fb 9aef 0cf7 281a  ......yO......(.
-000084b0: 8d18 8818 1846 0624 e3d8 ec25 b660 ae49  .....F.$...%.`.I
-000084c0: 04c8 f0bc 2033 fdca d851 fc0d 1f03 9ab1  .... 3...Q......
-000084d0: d7ae 4c0a f36c 2f1f 83e3 41fe 427c d8b2  ..L..l/...A.B|..
-000084e0: 09c2 9181 ebc4 6d6a 4aeb acd6 8dd7 0d2f  ......mjJ....../
-000084f0: fca2 6f0c 69f2 126b 7193 4e79 849e 1591  ..o.i..kq.Ny....
-00008500: 85b7 a898 47c9 a26b 0634 23a9 1d48 1677  ....G..k.4#..H.w
-00008510: 5e09 977d da7b 3f6b 86fc 786f febe f77a  ^..}.{?k..xo...z
-00008520: b6ce c7b8 c011 4e70 dec1 e21c bf7f 01d9  ......Np........
-00008530: 81c6 5554 49ff 47f7 3dd1 ed02 1d54 750d  ..UTI.G.=....Tu.
-00008540: eac9 e4fd c3b4 7fc6 6b9f 98be 5bff ba42  ........k...[..B
-00008550: 7b0d b10b 1e61 09bf 168c 98d3 5970 a682  {....a......Yp..
-00008560: 6726 d626 5af3 7322 97f3 e627 0000 00ff  g&.&Z.s"...'....
-00008570: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00008580: 00e8 f726 32a9 0100 0054 0f00 0027 0000  ...&2....T...'..
-00008590: 0078 6c2f 7072 696e 7465 7253 6574 7469  .xl/printerSetti
-000085a0: 6e67 732f 7072 696e 7465 7253 6574 7469  ngs/printerSetti
-000085b0: 6e67 7333 2e62 696e ec57 b94e c340 107d  ngs3.bin.W.N.@.}
-000085c0: bb36 71a2 8810 2828 517a 84c4 1104 8826  .6q...((Qz.....&
-000085d0: 1202 8906 1091 2042 2938 9282 a340 1c22  ...... B)8...@."
-000085e0: e99c 8e96 36d4 fc03 1f42 49c1 6750 61de  ....6....BI.gPa.
-000085f0: ac73 1870 0428 4713 bfd5 dad6 ceec 78fc  .s.p.(G.......x.
-00008600: 7676 c65b 4411 3728 e30c 33b8 c335 6ed9  vv.[D.7(..3..5n.
-00008610: 8b58 c70e f2d8 c616 32d8 c706 656b 58c4  .X......2...ekX.
-00008620: 1256 b0cb 913c f5af 700a 81b2 a15f 5149  .V...<..p...._QI
-00008630: 8d3d ba8e 4202 f564 365e 8282 8382 56bc  .=..B..d6^....V.
-00008640: 1734 758c 66ef 2f62 97e6 3bda afa4 2823  .4u.f./b..;...(#
-00008650: 4429 e8c3 32e7 b8a3 c033 7b8e cfef bcbb  D)..2....3{.....
-00008660: 01f7 c661 db7f 63a0 4cb6 c221 7e09 d2f4  ...a..c.L..!~...
-00008670: a109 f141 c1e2 759a bc14 b463 0409 64e3  ...A..u....c..d.
-00008680: f5e4 14fc 26cf abd6 832d ba31 4c86 1817  ....&....-.1L...
-00008690: cbb1 d6b8 794f e3fb 9aef 0cf7 281a 8d18  ....yO......(...
-000086a0: 8818 1846 0624 e3d8 ec25 b660 ae49 04c8  ...F.$...%.`.I..
-000086b0: f0bc 2033 fdca d851 fc0d 1f03 9ab1 d7ae  .. 3...Q........
-000086c0: 4c0a f36c 2f1f 83e3 41fe 427c d8b2 09c2  L..l/...A.B|....
-000086d0: 9181 ebc4 6d6a 4aeb acd6 8dd7 0d2f fca2  ....mjJ....../..
-000086e0: 6f0c 69f2 126b 7193 4e79 849e 1591 85b7  o.i..kq.Ny......
-000086f0: a898 47c9 a26b 0634 23a9 1d48 1677 5e09  ..G..k.4#..H.w^.
-00008700: 977d da7b 3f6b 86fc 786f febe f77a b6ce  .}.{?k..xo...z..
-00008710: c7b8 c011 4e70 dec1 e21c bf7f 01d9 81c6  ....Np..........
-00008720: 5554 49ff 47f7 3dd1 ed02 1d54 750d eac9  UTI.G.=....Tu...
-00008730: e4fd c3b4 7fc6 6b9f 98be 5bff ba42 7b0d  ......k...[..B{.
-00008740: b10b 1e61 09bf 168c 98d3 5970 a682 6726  ...a......Yp..g&
-00008750: d626 5af3 7322 97f3 e627 0000 00ff ff03  .&Z.s"...'......
-00008760: 0050 4b03 0414 0006 0008 0000 0021 00e8  .PK..........!..
-00008770: f726 32a9 0100 0054 0f00 0027 0000 0078  .&2....T...'...x
-00008780: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
-00008790: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
-000087a0: 7334 2e62 696e ec57 b94e c340 107d bb36  s4.bin.W.N.@.}.6
-000087b0: 71a2 8810 2828 517a 84c4 1104 8826 1202  q...((Qz.....&..
-000087c0: 8906 1091 2042 2938 9282 a340 1c22 e99c  .... B)8...@."..
-000087d0: 8e96 36d4 fc03 1f42 49c1 6750 61de ac73  ..6....BI.gPa..s
-000087e0: 1870 0428 4713 bfd5 dad6 ceec 78fc 7676  .p.(G.......x.vv
-000087f0: c65b 4411 3728 e30c 33b8 c335 6ed9 8b58  .[D.7(..3..5n..X
-00008800: c70e f2d8 c616 32d8 c706 656b 58c4 1256  ......2...ekX..V
-00008810: b0cb 913c f5af 700a 81b2 a15f 5149 8d3d  ...<..p...._QI.=
-00008820: ba8e 4202 f564 365e 8282 8382 56bc 1734  ..B..d6^....V..4
-00008830: 758c 66ef 2f62 97e6 3bda afa4 2823 4429  u.f./b..;...(#D)
-00008840: e8c3 32e7 b8a3 c033 7b8e cfef bcbb 01f7  ..2....3{.......
-00008850: c661 db7f 63a0 4cb6 c221 7e09 d2f4 a109  .a..c.L..!~.....
-00008860: f141 c1e2 759a bc14 b463 0409 64e3 f5e4  .A..u....c..d...
-00008870: 14fc 26cf abd6 832d ba31 4c86 1817 cbb1  ..&....-.1L.....
-00008880: d6b8 794f e3fb 9aef 0cf7 281a 8d18 8818  ..yO......(.....
-00008890: 1846 0624 e3d8 ec25 b660 ae49 04c8 f0bc  .F.$...%.`.I....
-000088a0: 2033 fdca d851 fc0d 1f03 9ab1 d7ae 4c0a   3...Q........L.
-000088b0: f36c 2f1f 83e3 41fe 427c d8b2 09c2 9181  .l/...A.B|......
-000088c0: ebc4 6d6a 4aeb acd6 8dd7 0d2f fca2 6f0c  ..mjJ....../..o.
-000088d0: 69f2 126b 7193 4e79 849e 1591 85b7 a898  i..kq.Ny........
-000088e0: 47c9 a26b 0634 23a9 1d48 1677 5e09 977d  G..k.4#..H.w^..}
-000088f0: da7b 3f6b 86fc 786f febe f77a b6ce c7b8  .{?k..xo...z....
-00008900: c011 4e70 dec1 e21c bf7f 01d9 81c6 5554  ..Np..........UT
-00008910: 49ff 47f7 3dd1 ed02 1d54 750d eac9 e4fd  I.G.=....Tu.....
-00008920: c3b4 7fc6 6b9f 98be 5bff ba42 7b0d b10b  ....k...[..B{...
-00008930: 1e61 09bf 168c 98d3 5970 a682 6726 d626  .a......Yp..g&.&
-00008940: 5af3 7322 97f3 e627 0000 00ff ff03 0050  Z.s"...'.......P
-00008950: 4b03 0414 0006 0008 0000 0021 00e8 f726  K..........!...&
-00008960: 32a9 0100 0054 0f00 0027 0000 0078 6c2f  2....T...'...xl/
-00008970: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00008980: 7072 696e 7465 7253 6574 7469 6e67 7335  printerSettings5
-00008990: 2e62 696e ec57 b94e c340 107d bb36 71a2  .bin.W.N.@.}.6q.
-000089a0: 8810 2828 517a 84c4 1104 8826 1202 8906  ..((Qz.....&....
-000089b0: 1091 2042 2938 9282 a340 1c22 e99c 8e96  .. B)8...@."....
-000089c0: 36d4 fc03 1f42 49c1 6750 61de ac73 1870  6....BI.gPa..s.p
-000089d0: 0428 4713 bfd5 dad6 ceec 78fc 7676 c65b  .(G.......x.vv.[
-000089e0: 4411 3728 e30c 33b8 c335 6ed9 8b58 c70e  D.7(..3..5n..X..
-000089f0: f2d8 c616 32d8 c706 656b 58c4 1256 b0cb  ....2...ekX..V..
-00008a00: 913c f5af 700a 81b2 a15f 5149 8d3d ba8e  .<..p...._QI.=..
-00008a10: 4202 f564 365e 8282 8382 56bc 1734 758c  B..d6^....V..4u.
-00008a20: 66ef 2f62 97e6 3bda afa4 2823 4429 e8c3  f./b..;...(#D)..
-00008a30: 32e7 b8a3 c033 7b8e cfef bcbb 01f7 c661  2....3{........a
-00008a40: db7f 63a0 4cb6 c221 7e09 d2f4 a109 f141  ..c.L..!~......A
-00008a50: c1e2 759a bc14 b463 0409 64e3 f5e4 14fc  ..u....c..d.....
-00008a60: 26cf abd6 832d ba31 4c86 1817 cbb1 d6b8  &....-.1L.......
-00008a70: 794f e3fb 9aef 0cf7 281a 8d18 8818 1846  yO......(......F
-00008a80: 0624 e3d8 ec25 b660 ae49 04c8 f0bc 2033  .$...%.`.I.... 3
-00008a90: fdca d851 fc0d 1f03 9ab1 d7ae 4c0a f36c  ...Q........L..l
-00008aa0: 2f1f 83e3 41fe 427c d8b2 09c2 9181 ebc4  /...A.B|........
-00008ab0: 6d6a 4aeb acd6 8dd7 0d2f fca2 6f0c 69f2  mjJ....../..o.i.
-00008ac0: 126b 7193 4e79 849e 1591 85b7 a898 47c9  .kq.Ny........G.
-00008ad0: a26b 0634 23a9 1d48 1677 5e09 977d da7b  .k.4#..H.w^..}.{
-00008ae0: 3f6b 86fc 786f febe f77a b6ce c7b8 c011  ?k..xo...z......
-00008af0: 4e70 dec1 e21c bf7f 01d9 81c6 5554 49ff  Np..........UTI.
-00008b00: 47f7 3dd1 ed02 1d54 750d eac9 e4fd c3b4  G.=....Tu.......
-00008b10: 7fc6 6b9f 98be 5bff ba42 7b0d b10b 1e61  ..k...[..B{....a
-00008b20: 09bf 168c 98d3 5970 a682 6726 d626 5af3  ......Yp..g&.&Z.
-00008b30: 7322 97f3 e627 0000 00ff ff03 0050 4b03  s"...'.......PK.
-00008b40: 0414 0006 0008 0000 0021 00a9 9076 df52  .........!...v.R
-00008b50: 0100 0063 0200 0011 0008 0164 6f63 5072  ...c.......docPr
-00008b60: 6f70 732f 636f 7265 2e78 6d6c 20a2 0401  ops/core.xml ...
-00008b70: 28a0 0001 0000 0000 0000 0000 0000 0000  (...............
+00000c00: 0000 0000 0000 bc94 4d6a c330 1085 f785  ........Mj.0....
+00000c10: de41 685f cb76 1237 2d91 b309 856c 5bf7  .Ah_.v.7-....l[.
+00000c20: 00c2 1eff 105b 329a 495b dfbe c2a5 8d03  .....[2.I[......
+00000c30: 41dd 186f 0433 83de fb34 82b7 db7f 752d  A..o.3...4....u-
+00000c40: fb00 8b8d d192 4741 c819 e8dc 148d ae24  ......GA.......$
+00000c50: 7fcf 5e1e b69c 2129 5da8 d668 907c 00e4  ..^...!)]..h.|..
+00000c60: fbf4 fe6e f70a ad22 7709 eba6 47e6 5434  ...n..."w...G.T4
+00000c70: 4a5e 13f5 cf42 605e 43a7 3030 3d68 3729  J^...B`^C.00=h7)
+00000c80: 8ded 14b9 d256 a257 f949 5520 e230 4c84  .....V.W.IU .0L.
+00000c90: 9d6a f0f4 4a93 1d0b c9ed b170 fed9 d03b  .j..J......p...;
+00000ca0: e7ff b54d 5936 391c 4c7e ee40 d30d 0b81  ...MY69.L~.@....
+00000cb0: 34b4 ee01 2c53 b602 92fc a70e 1c23 17b7  4...,S.......#..
+00000cc0: ed57 73da 7f1a 7bc2 1a80 2e04 7f2d 14e3  .Ws...{......-..
+00000cd0: 64e5 8379 9c13 86dc 1fc1 0564 2cc5 7846  d..y.......d,.xF
+00000ce0: 3e86 78e1 85c4 3e98 6861 18ef 6692 8561  >.x...>.ha..f..a
+00000cf0: 12df 6636 0bc3 6c7c 30eb 8561 d63e 98a7  ..f6..l|0..a.>..
+00000d00: 5903 a556 168a 37b2 2e2f a7b9 326d ffc2  Y..V..7../..2m..
+00000d10: 88ab c84c bf01 0000 ffff 0300 504b 0304  ...L........PK..
+00000d20: 1400 0600 0800 0000 2100 3875 47bc f314  ........!.8uG...
+00000d30: 0000 65b8 0000 1800 0000 786c 2f77 6f72  ..e.......xl/wor
+00000d40: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
+00000d50: 6d6c 9c93 c96e db30 1086 ef05 fa0e 04ef  ml...n.0........
+00000d60: 1625 3976 13c1 72d0 d630 1aa0 87a2 5bce  .%9v..r..0....[.
+00000d70: 1435 b208 93a2 4ad2 1b8a be7b 8794 9700  .5....J....{....
+00000d80: 3ec4 8820 0dd7 f9fe 1972 347b dc6b 45b6  >.. .....r4{.kE.
+00000d90: 609d 345d 49b3 24a5 043a 616a d9ad 4afa  `.4]I.$..:aj..J.
+00000da0: ebe7 7274 4f89 f3bc abb9 321d 94f4 008e  ..rtO.....2.....
+00000db0: 3ece dfbf 9bed 8c5d bb16 c013 2474 aea4  >......]....$t..
+00000dc0: adf7 7dc1 9813 2d68 ee12 d343 872b 8db1  ..}...-h...C.+..
+00000dd0: 9a7b 1cda 1573 bd05 5e47 27ad 589e a653  .{...s..^G'.X..S
+00000de0: a6b9 ece8 4028 ec2d 0cd3 3452 c0c2 888d  ....@(.-..4R....
+00000df0: 86ce 0f10 0b8a 7b8c dfb5 b277 279a 16b7  ......{....w'...
+00000e00: e034 b7eb 4d3f 1246 f788 a8a4 92fe 10a1  .4..M?.F........
+00000e10: 9468 513c ad3a 6379 a530 ef7d 76c7 05d9  .hQ<.:cy.0.}v...
+00000e20: 5b7c 73fc c627 9938 7fa5 a4a5 b0c6 99c6  [|s..'.8........
+00000e30: 2748 6643 ccd7 e93f b007 c6c5 9974 9dff  'HfC...?.....t..
+00000e40: 4d98 ec8e 59d8 ca70 8117 54fe b690 b2c9  M...Y..p..T.....
+00000e50: 9995 5f60 e337 c2a6 6758 382e 5b6c 645d  .._`.7..gX8.[ld]
+00000e60: d2bf e9f1 1961 9b05 935e cc69 ed1f 9dcf  .....a...^.i....
+00000e70: 6a89 371c b222 169a 927e cc8a 4fe3 c93d  j.7.."...~..O..=
+00000e80: 65f3 59ac a0df 1276 ee45 9f78 5efd 0005  e.Y....v.E.x^...
+00000e90: c203 aa64 9478 d37f 85c6 7f06 a5d0 7b3c  ...d.x........{<
+00000ea0: c1a9 50b3 9531 ebe0 fb84 bb52 9471 d127  ..P..1.....R.q.'
+00000eb0: c870 e1e5 1686 fd8b 2045 dc9f 281d 07a8  .p...... E..(...
+00000ec0: cbce c22f fba7 2096 b1d2 bf59 5243 c337  .../.. ....YRC.7
+00000ed0: ca7f 37bb 2f20 57ad c768 a6c9 044f 2094  ..7./ W..h...O .
+00000ee0: 5051 1f16 e004 d62e ca27 f924 e423 8c42  PQ.......'.$.#.B
+00000ef0: 085a a265 f809 b1f6 f83e b63b 59fb b6a4  .Z.e.....>.;Y...
+00000f00: 7996 7c40 4005 ce2f 65e0 5122 36ce 1bfd  y.|@@../e.Q"6...
+00000f10: 3cac 6747 cae0 8f37 17fd b13d faa3 7e86  <.gG...7...=..~.
+00000f20: 52af 0058 8ce3 3f00 0000 ffff 0000 00ff  R..X..?.........
+00000f30: ff94 9d6d aedc c615 44b7 6268 01f1 ebee  ...m....D.bh....
+00000f40: f90c 6401 31bc 11c1 11e0 5f4e 6009 4eb2  ..d.1....._N`.N.
+00000f50: fbdc d763 486f 6e9d 1258 ff2c bfc2 dc3b  ...cHon..X.,...;
+00000f60: 4df2 4c93 ec43 beff fcdb a74f 5f7e f9f8  M.L..C.....O_~..
+00000f70: e5e3 87f7 7ffc eb3f 3ffc f1d3 bbf1 ee87  .......??.......
+00000f80: cfff fef8 fbe7 faaf bfcf 773f fc77 9c3e  ..........w?.w.>
+00000f90: fefa f77f feef 974f 9f7f fdf4 fb97 9fde  .......O........
+00000fa0: bdfc 6d9e df7d 78ff eb6b f61f 15ae fff5  ..m..}x..k......
+00000fb0: b9fe fde7 8771 bfbc fff1 cf0f ef7f fcf5  .....q..........
+00000fc0: afbf fefc fcd7 ebd7 bffe 58a5 bed6 ab1a  ..........X.....
+00000fd0: c7eb bd86 778b 5fab f69a 9a30 7557 52f7  ....w._....0uWR.
+00000fe0: 35fc 5cf7 d6be ab26 4cdd 5352 f735 fc5c  5.\....&L.SR.5.\
+00000ff0: f7de ea6a c2d4 3d27 755f c3cf 75c7 4b2b  ...j..='u_..u.K+
+00001000: ac11 53f8 9214 7e0d b7c2 a315 d688 297c  ..S...~.......)|
+00001010: 4d0a bf86 5be1 d90a 6bc4 14be 2585 5fc3  M...[...k...%._.
+00001020: adf0 6a85 3562 0adf 93c2 afe1 56f8 d40a  ..j.5b......V...
+00001030: 6bc4 141e 2f49 e59d 6ea5 cf9d 1daf 9ff8  k.../I..n.......
+00001040: 9c71 b533 62bd a65b 6de1 9666 5ced 885e  .q.3b..[m..f\..^
+00001050: 43e1 34be 7df0 26ea cf90 71b5 2382 0d05  C.4.}.&...q.#...
+00001060: d4e8 0c83 8cab 1d51 6c28 a446 e718 645c  .......Ql(.F..d\
+00001070: ed88 6443 3935 3bca 20e3 6a47 301b 8aaa  ..dC95;. .jG0...
+00001080: d969 0619 573b e2d9 505a cd0e 34c8 b8da  .i..W;..PZ..4...
+00001090: 11d2 8602 6b76 a641 c6d5 8ea8 3694 59b3  ....kv.A....6.Y.
+000010a0: 630d 32a6 f68c b8b6 d3cf 6c99 9d6b 9071  c.2.......l..k.q
+000010b0: b523 ae4d 65d6 94b9 d161 aecd 6c56 a65c  .#.Me....a..lV.\
+000010c0: 9b9d 6bfb 130f f17c 465c dbe9 36e6 9d6b  ..k....|F\..6..k
+000010d0: 9071 631e 716d 2ad7 66e7 1a64 5ced 886b  .qc.qm*.f..d\..k
+000010e0: 3509 efbf 63ab 730d 32ae 76c4 b5a9 5c5b  5...c.s.2.v...\[
+000010f0: 9d6b 9071 b523 ae4d e5da ea5c 838c ab1d  .k.q.#.M...\....
+00001100: 716d 2ad7 e410 d3c8 fa86 9fe7 139f 886b  qm*............k
+00001110: 53b9 26bb b946 5ced 1571 6da7 9f8f b1d5  S.&..F\..qm.....
+00001120: b946 19f3 c557 04b6 9d6e c5fb a853 c615  .F...W...n...S..
+00001130: 8fc8 b694 6cab 938d 32ae 7876 d2a9 53b6  ....l...2.xv..S.
+00001140: 25a7 9d90 71c5 23b6 2d65 dbea 6ca3 8c2b  %...q.#.-e..l..+
+00001150: 1ec1 6d29 dc4e 1d6e 90b1 7b7b 44b7 a574  ..m).N.n..{{D..t
+00001160: 3b75 ba41 c616 8ff0 b614 6fa7 8e37 c8d8  ;u.A......o..7..
+00001170: e211 df96 c2eb d4e7 6d90 b1c5 23c0 2da5  ........m...#.-.
+00001180: d7a9 4fdc 20e3 8a9f 22c2 edf4 3364 4e9d  ..O. ..."...3dN.
+00001190: 7090 b1c5 23c2 9d74 5a76 ea84 838c 2d1e  p...#..tZv....-.
+000011a0: 11ee a484 3b75 c241 c616 8f08 7752 7a9d  ....;u.A....wRz.
+000011b0: 3ae1 2063 8b67 d7d6 9470 27b9 ba06 1434  :. c.g...p'....4
+000011c0: 843b 4584 dbe9 e71d eedc 0907 19fb cd23  .;E............#
+000011d0: c29d 9470 e74e 38c8 d8e2 11e1 4e4a b873  ...p.N8.....NJ.s
+000011e0: 271c 646c f188 7027 25dc b913 0e32 b678  '.dl..p'%....2.x
+000011f0: 44b8 9312 eedc 0907 1957 fc1c 116e a7db  D........W...n..
+00001200: 0ed7 0907 195b 3c22 dc59 0977 ee84 838c  .....[<".Y.w....
+00001210: 2d1e 11ee ac84 3b77 c241 c616 8f08 77ae  -.....;w.A....w.
+00001220: f4d7 7b15 f74b e7cb eb9f dbd5 485b 3782  ..{..K......H[7.
+00001230: dbb9 d2df ea5e e5e2 fd71 ae9d b31b 0795  .....^...q......
+00001240: 7e53 b753 657f 589b cc1b 9e9e 23a4 edf4  ~S.Se.X.....#...
+00001250: f307 cb0e 06d4 fbf6 63f3 746a 768e 88b6  ........c.tjv...
+00001260: d3cf b5fb 8f18 44ce ae76 04b4 3300 4d76  ......D..v..3.Mv
+00001270: 32c8 b8e2 11d0 ce0a b48b ec69 003d 53fc  2..........i.=S.
+00001280: 1201 6da7 db16 975b 457a 13c1 0dfb 2502  ..m....[Ez....%.
+00001290: da4e b7e2 fd47 0c32 b678 04b4 0bdc 05ed  .N...G.2.x......
+000012a0: 3f62 90b1 c523 a05d 9458 97fe 2306 195b  ?b...#.].X..#..[
+000012b0: 3ca2 da45 b175 e93f 6290 b1c5 23b4 5df4  <..E.u.?b...#.].
+000012c0: a4f4 d219 0319 5b3c bb2f aaf0 baf4 1fb1  ......[<./......
+000012d0: cb71 c05d 22c0 ed74 dbdb 3be1 2063 bf79  .q.]"..t..;. c.y
+000012e0: 44b8 0b5c 74eb 8483 8c2d 1e11 ee02 7740  D..\t....-....w@
+000012f0: 3be1 20e3 8a5f 23c2 ed74 bb64 de09 0719  ;. .._#..t.d....
+00001300: 5b3c 22dc 15ee 15c8 0d71 98d6 19b6 5f23  [<"......q...._#
+00001310: c2ed 74fb e69d 7090 b1df 3c22 dc15 9672  ..t...p...<"...r
+00001320: 74c2 41c6 168f 0877 85f5 1c9d 7090 b1c5  t.A....w....p...
+00001330: 23c2 5d61 4d47 271c 646c f188 7057 58d7  #.]aMG'.dl..pWX.
+00001340: d109 0719 5b3c 5bfd 016b 3b3a e1ae 70e2  ....[<[..k;:..p.
+00001350: eaf6 f688 7057 58df d109 0719 fbcd 23c2  ....pWX.......#.
+00001360: 5de1 be42 271c 645c f15b 44b8 9d6e 33e7  ]..B'.d\.[D..n3.
+00001370: 4e38 c8d8 e211 e16e 4aaf 5b27 1c64 6cf1  N8.....nJ.['.dl.
+00001380: 8870 379d c3dd 64d9 0f9c b89a 1dee 1611  .p7...d.........
+00001390: 6ea7 dbb0 77c2 41c6 7ef3 8870 3725 dcad  n...w.A.~..p7%..
+000013a0: 130e 32b6 7844 b89b 12ee d609 0719 5b3c  ..2.xD........[<
+000013b0: 22dc 4d09 77eb 8483 8c2d 1e11 eea6 f4ba  ".M.w....-......
+000013c0: 75c2 41c6 168f 0877 53c2 dd3a e120 638b  u.A....wS..:. c.
+000013d0: 4784 bbc1 596a 5f60 a791 fb37 083e 5d1a  G...Yj_`...7.>].
+000013e0: b847 80db e9ef 5f1a 8088 ad1d f1ed ae7c  .G...._........|
+000013f0: 93bb b690 b1c5 23be dd95 5df7 4e76 cab8  ......#...].Nv..
+00001400: 518f f876 d719 dcbd 939d 32ae 78c4 b7bb  Q..v......2.x...
+00001410: f2ed dec9 4e19 573c e2db 5df9 7697 459d  ....N.W<..].v.E.
+00001420: 9071 c523 bedd 956f f74e 76ca b8e2 11df  .q.#...o.Nv.....
+00001430: eeca 3759 8f4e 1957 3ce2 db5d f976 ef64  ..7Y.N.W<..].v.d
+00001440: a78c 2b1e f1ed 0ef0 ea64 a78c 293e 5ec2  ..+......d..)>^.
+00001450: b5bc 7a8d ed2e 8b3b f767 3e73 d071 66bc  ..z....;.g>s.qf.
+00001460: 4494 7bc4 9f3f babe 82ac 2656 18fa 0622  D.{..?....&V..."
+00001470: d28d 1745 5d35 250d 0010 ed16 8868 375e  ...E]5%......h7^
+00001480: 1477 d594 3400 50b4 0d44 c41b 2f8a bc6a  .w..4.P..D../..j
+00001490: 4a1a 0030 da06 22ea 8d17 455a 3525 0d1c  J..0.."...EZ5%..
+000014a0: 07df 7889 c8f7 88f7 9d50 97b4 0320 ed08  ..x......P... ..
+000014b0: 44f4 1b2f 8abf 6a4a 4600 2069 1b88 0838  D../..jJF. i...8
+000014c0: 5e14 81d5 9434 00a0 b40d 4414 1c2f 8ac1  ^....4....D../..
+000014d0: 6a4a 1a38 3ed3 1ba1 d440 56c3 8b90 1052  jJ.8>....@V....R
+000014e0: 1644 2323 e18e b79d 50b4 9d01 29df 4046  .D##....P...).@F
+000014f0: 42f2 1b86 9010 52be 818c 8424 390c 2121  B.....R....$9.!!
+00001500: a47c 0319 09c9 7418 4242 48f9 0632 1282  .|....t.BBH..2..
+00001510: ca30 8690 1052 be81 8c84 e033 8c21 2484  .0...R.....3.!$.
+00001520: 946f 2023 2148 0d63 a8e1 1390 70ab 0ac7  .o #!H.c....p...
+00001530: 9548 301b 866a 3e90 f223 9091 10f4 86a1  .H0..j>..#......
+00001540: ae0f a46c 0399 0631 c071 182a fc40 ca37  ...l...1.q.*.@.7
+00001550: 9091 1064 886a aaff 1640 ca37 9091 106c  ...d.j...@.7...l
+00001560: 87a1 ea0f a47c 0319 0941 7918 eaff 40ca  .....|...Ay...@.
+00001570: 3790 9110 bc87 a112 10a4 7c03 1909 417e  7.........|...A~
+00001580: 186a 0241 ca37 9091 100c 8821 3ad0 8094  .j.A.7.....!:...
+00001590: 6f20 2321 6810 554e 8e82 8084 5b80 384e  o #!h.UN....[.8N
+000015a0: 42f0 2586 8841 0352 7e04 3212 8234 51e5  B.%..A.R~.2..4Q.
+000015b0: 6404 8239 6126 4e0c b022 8628 4294 b223  d..9a&N..".(B..#
+000015c0: 90c9 1303 cc88 2ad7 4700 52be 818c 8460  ......*.G.R....`
+000015d0: 4754 53d2 4070 76bc 3212 ee78 9b15 8b31  GTS.@pv.2..x...1
+000015e0: 3420 e547 2023 2158 1255 4e46 2038 3bde  4 .G #!X.UNF 8;.
+000015f0: eac3 f1c3 104c 89f1 6695 e15f de31 a4fc  .....L..f.._.1..
+00001600: 0864 2404 5b62 c8a5 e801 29df 4046 4230  .d$.[b....).@FB0
+00001610: 26aa 9c6c 8280 845b 8308 3601 9c1d 8b48  &..l...[..6....H
+00001620: 34c0 adf0 2390 9110 cc89 2a27 2310 9030  4...#.....*'#..0
+00001630: 132c 06d8 1343 8422 4ad9 11d8 4ac4 f14d  .,...C."J...J..M
+00001640: 0006 4595 eb23 0029 df40 4642 b028 8688  ..E..#.).@FB.(..
+00001650: 4503 52be 818c 8460 5254 3919 81e0 3ae1  E.R....`RT9...:.
+00001660: 2923 e18e 3714 8b60 3420 e547 209b 1382  )#..7..`4 .G ...
+00001670: 5151 e564 0482 eb84 5b93 0876 42bd 0238  QQ.d....[..vB..8
+00001680: 4434 1ae0 5ef8 11c8 4808 6645 9593 1108  D4..^...H.fE....
+00001690: 48b8 7589 6004 8084 221c 0d70 30fc 0864  H.u.`..."..p0..d
+000016a0: 2404 c3a2 cac9 0804 24cc 448c 0196 c510  $.......$.D.....
+000016b0: f188 5276 04b6 3a71 7c13 8069 217b 0064  ..Rv..:q|..i!{.d
+000016c0: aaa5 afa3 f474 4b7c 6c7b 22a8 0f6b 5ffa  .....tK|l{"..k_.
+000016d0: f883 90f1 9dfa 1907 49ba 902b 5410 fa4e  ........I..+T..N
+000016e0: 0319 075f e58c fe0c 1a11 b006 a6ec 26c8  ..._..........&.
+000016f0: 4008 1e46 6d45 d908 705b c5ef 04d9 9c10  @..FmE..p[......
+00001700: 848d 212a d6c0 941d 830c 85e0 64d4 98cb  ..!*........d...
+00001710: 18c0 8d15 3f06 d93d 1390 37c6 59f7 4420  ....?..=..7.Y.D 
+00001720: a6ef 2083 2118 1c35 e632 0670 6bc5 7690  .. .!..5.2.pk.v.
+00001730: 591c 0334 8e21 7a16 a7dc 7e90 a91c 033c  Y..4.!z...~....<
+00001740: 8df1 66e5 d15f a747 98b2 1d64 3343 9035  ..f.._.G...d3C.5
+00001750: c659 ee1c 61ca 7690 2111 8c8d 1af3 be1f  .Y..a.v.!.......
+00001760: 50ca ef07 1913 41db a82d 231d 1039 ed18  P.....A..-#..9..
+00001770: 644c 0477 635c 8489 94f2 6390 3111 048e  dL.wc\....c.1...
+00001780: 7191 2b05 94f2 1d64 4c04 8b63 88de 3328  q.+....dL..c..3(
+00001790: e53b c898 082a c710 c767 50ca 7790 3111  .;...*...gP.w.1.
+000017a0: 7c8e 21a2 cfa0 94ed 20f3 3e06 481d 35e6  |.!..... .>.H.5.
+000017b0: fd58 a094 ef20 bb81 02f6 478d b974 a08b  .X... ....G..t..
+000017c0: 6afc 1c29 3340 06e8 1d35 e6d2 01ac bdf1  j..)3@...5......
+000017d0: 6390 3111 1c8f da32 d201 2cbe f11d 644c  c.1....2..,...dL
+000017e0: 04d1 635c 8589 94f2 1d64 4c04 dba3 b68c  ..c\.....dL.....
+000017f0: 8c41 324f dc0e c7f1 9305 503e 647e 0299  .A2O......P>d~..
+00001800: 71fd c6cd e793 95ad 7104 f575 fea7 c701  q.......q..u....
+00001810: cc11 7dfd 8c87 247e e86d 2c48 7d67 0432  ..}...$~.m,H}g.2
+00001820: 1e92 fda1 b791 20e5 3bc8 2c91 010a 885e  ...... .;.,....^
+00001830: 3e86 d077 1ac8 7008 1ac8 b8ca a902 a6dc  >..w..p.........
+00001840: 6eb8 0590 e3bb 21f8 22e3 2aa7 0a98 b21d  n.....!.".*.....
+00001850: 6438 0421 645c e550 c494 ed20 c321 5821  d8.!d\.P... .!X!
+00001860: e32a 3f8b 98b2 1d64 3804 3564 5c05 0798  .*?....d8.5d\...
+00001870: b21d 6453 44f0 43c6 557e 1631 653b c8a6  ..dSD.C.U~.1e;..
+00001880: 8820 89d4 01da 7f12 2865 91b8 d58f e058  . ......(e.....X
+00001890: 8013 e29b fc2c 824f f21d 1e64 4804 a564  .....,.O...dH..d
+000018a0: 883b 3628 65c7 20f3 4a06 5823 4304 324c  .;6(e. .J.X#C.2L
+000018b0: f90e 3226 823a 326e c244 4af9 0eb2 d366  ..2&.:2n.DJ....f
+000018c0: f047 86a8 6483 52be 838c 8920 910c f1c9  .G..d.R.... ....
+000018d0: 06a5 7c07 1913 c124 1922 950d 4af9 0e32  ..|....$."..J..2
+000018e0: 2682 7232 c42c 1b94 f21d 644c 04a7 a48e  &.r2.,....dL....
+000018f0: bd4e 244a f90e 3226 8258 52c7 9e74 904c  .N$J..2&.XR..t.L
+00001900: 13b7 2e72 9c89 6097 4c5d 7408 a937 2b11  ...r..`.L]t..7+.
+00001910: 9ee7 c95b 1909 1ad0 6b84 5317 1d82 87e2  ...[....k.S.....
+00001920: 1a98 9987 f288 3fdf 5c9c b2e8 9052 be81  ......?.\....R..
+00001930: 0888 737b 2bad 0159 7448 29df 40c4 c309  ..s{+..YtH).@...
+00001940: 22ca 9445 8794 f20d 4438 9c20 a24c 5974  "..E....D8. .LYt
+00001950: 4829 df40 44c3 0922 ca94 4587 94f2 0d44  H).@D.."..E....D
+00001960: 309c 20a2 4c39 5ba3 946f 2062 e1dc de4a  0. .L9[..o b...J
+00001970: df09 f519 e47a 1bda 3710 a170 8288 32f5  .....z..7..p..2.
+00001980: 41e4 90f2 0d44 27cc 1344 94a9 4f23 8794  A....D'..D..O#..
+00001990: 6f20 9a1c 4e10 51a6 2c3a a494 6d20 1351  o ..N.Q.,:..m .Q
+000019a0: 2628 2653 9f4b 0e29 df40 4642 524c e407  &(&S.K.).@FBRL..
+000019b0: 7942 ca37 9091 1014 93a9 4f47 8794 6f20  yB.7......OG..o 
+000019c0: 2321 2826 531f 910e 29df 4046 4250 4ca6  #!(&S...).@FBPL.
+000019d0: 3e27 1d52 be81 8c84 f4de 8d37 9ffd b8ab  >'.R.......7....
+000019e0: 3621 e51b c848 482f df90 558f 1352 be81  6!...HH/..U..R..
+000019f0: 8c84 f406 0eb9 6c55 9334 7d02 a439 53af  ......lU.4}..9S.
+00001a00: f954 f296 9d47 bcfd 16c8 aa47 4af9 11c8  .T...G.....GJ...
+00001a10: 4848 efe2 9055 8f35 493b 3e02 e1fb 38e8  HH...U.5I;>...8.
+00001a20: 851c b2ea 7142 ca8e c076 460e cf8a 6bfa  ....qB...vF...k.
+00001a30: 25df 6dca aa47 4af9 0632 1282 6232 65d5  %.m..GJ..2..b2e.
+00001a40: 634d d282 4d90 9190 decf 21ab 1e6b 9216  cM..M.....!..k..
+00001a50: 3490 9190 5ed2 21ab 1e6b 9216 3490 9110  4...^.!..k..4...
+00001a60: 1493 29ab 1e27 bdcf c371 603b 23c1 4ea8  ..)..'...q`;#.N.
+00001a70: b3bd 29ab 1e6b 9216 8c40 4642 1051 a6ac  ..)..k...@FB.Q..
+00001a80: 7aac 495a d040 4642 504c a6ac 7aac 495a  z.IZ.@FBPL..z.IZ
+00001a90: d040 4642 1051 a6ac 7aac 49da f106 3211  .@FB.Q..z.I...2.
+00001aa0: a566 3f0a 2259 f548 290b a24c 44a9 d90f  .f?."Y.H)..LD...
+00001ab0: 3420 2fcb a117 79b8 a360 9b25 c78f 0210  4 /...y..`.%....
+00001ac0: 51a6 3c72 bde6 48c1 26c8 4808 8ac9 9455  Q.<r..H.&.H....U
+00001ad0: 7f13 527e 1364 2404 1165 caa2 bf49 2ff5  ..R~.d$..e...I/.
+00001ae0: b09b 2023 2128 2653 d6fc 4d7a b187 6d20  .. #!(&S..Mz..m 
+00001af0: 9b13 8262 3265 c9df a497 7bd8 0632 1282  ...b2e....{..2..
+00001b00: 8832 65c5 dfa4 177c d806 3212 8262 3265  .2e....|..2..b2e
+00001b10: c1df a497 7cd8 0632 1282 8832 65bd 5fcd  ....|..2...2e._.
+00001b20: 918e 1f86 9988 52b3 1f05 912c f7a3 943d  ......R....,...=
+00001b30: 0c33 1165 8262 3265 b51f a57c 03d9 9c10  .3.e.b2e...|....
+00001b40: 1493 298b fd26 bdf4 c3ed 03db 2c39 8e62  ..)..&......,9.b
+00001b50: 1051 a6ac f5ab 3952 b00f 6424 04c5 64ca  .Q....9R..d$..d.
+00001b60: 52bf 9a23 050d 6424 0411 65ca 4abf 9a23  R..#..d$..e.J..#
+00001b70: 050d 6424 04c5 64ca 42bf 9a23 050d 6424  ..d$..d.B..#..d$
+00001b80: 0411 65ca 3abf 9a23 050d 6424 04c5 64ca  ..e.:..#..d$..d.
+00001b90: 32bf 492f 03b1 4741 4642 1051 a6ac f29b  2.I/..GAFB.Q....
+00001ba0: f442 10d7 4026 a2d4 ec47 0657 1e94 4121  .B..@&...G.W..A!
+00001bb0: cba1 cc43 a9c9 8f92 5816 1952 ca37 9081  ...C....X..R.7..
+00001bc0: 1024 9329 6b0c 6b8a 747c 1fdc d6c8 7110  .$.)k.k.t|....q.
+00001bd0: 8264 3265 8961 4d91 8206 3210 8263 3265  .d2e.aM...2..c2e
+00001be0: 8561 4d91 8206 3210 8288 3265 8161 4d91  .aM...2...2e.aM.
+00001bf0: 8206 3210 8261 32df dc16 feeb 3a25 a4fc  ..2..a2.....:%..
+00001c00: 4e98 8110 3494 296b cb6a 8a14 8c40 0642  N...4.)k.j...@.B
+00001c10: b050 a62c 2d9b 90f2 2390 8110 2494 292b  .P.,-...#...$.)+
+00001c20: cb6a 8a74 7c04 3207 a526 3f0a 2259 5846  .j.t|.2..&?."YXF
+00001c30: 293b 0299 8252 931f 68a0 af2b a394 6f20  );...R..h..+..o 
+00001c40: 2321 b825 5396 95d5 1429 d804 d9c9 31a8  #!.%S....)....1.
+00001c50: 2553 5695 d514 2968 2023 21f8 2753 1695  %SV...)h #!.'S..
+00001c60: d514 2968 2023 2188 2553 d694 d514 2968  ..)h #!.%S....)h
+00001c70: 2023 2178 2553 9694 d514 2968 2023 2168   #!x%S....)h #!h
+00001c80: 2553 5694 d514 2968 2023 2159 257a 1406  %SV...)h #!Y%z..
+00001c90: 5709 b724 727c 3a40 4e89 5c22 8390 a540  W..$r|:@N.\"...@
+00001ca0: e69d d4d4 4331 d457 3151 c8d7 cfee 1b83  ....C1.W1Q......
+00001cb0: 75a2 eb57 20e4 eb67 1404 e744 578f 40c8  u..W ..g...DW.@.
+00001cc0: d7cf 2008 c6c9 9405 8d35 3b39 7e00 6c37  .. ......5;9~.l7
+00001cd0: e4f8 0e88 c249 5bc6 5693 93a0 7ec6 40d0  .....I[.V...~.@.
+00001ce0: 4da6 aca7 acc9 49d0 40c6 4030 49a6 2ca7  M.....I.@.@0I.,.
+00001cf0: acc9 49d0 40c6 4078 c9c8 94d5 9413 527e  ..I.@.@x......R~
+00001d00: 1fcc 1808 26c9 d4b5 1b90 f20d 64b3 4110  ....&.......d.A.
+00001d10: 49a6 aca5 acc9 c9f1 4d90 d926 35ed 500a  I.......M..&5.P.
+00001d20: cab3 eb29 6547 608b 21c7 8f42 f048 a63c  ...)eG`.!..B.H.<
+00001d30: bfbe 2627 c108 641c 048d 64ca 33ec 6b72  ..&'..d...d.3.kr
+00001d40: 1234 9081 102c 9229 cfb1 afc9 49d0 4036  .4...,.)....I.@6
+00001d50: 1b04 8964 cab3 ec6b 7212 3490 9110 1c92  ...d...kr.4.....
+00001d60: 29cf b3af 1f87 a081 8c84 a090 4c79 a67d  )...........Ly.}
+00001d70: c139 6820 2321 1824 f32e b331 48f9 c330  .9h #!.$...1H..0
+00001d80: 2321 0824 539e 6c5f 700e 4620 2321 f823  #!.$S.l_p.F #!.#
+00001d90: 4b9e 6c5f 703e de40 2699 1476 f5a3 e5c9  K.l_p>.@&..v....
+00001da0: f698 7257 28b7 0e72 9c84 f40a 1379 b2fd  ..rW(..r.....y..
+00001db0: a494 6d20 2321 c823 4b9e 6c5f 700e 3641  ..m #!.#K.l_p.6A
+00001dc0: 4642 7047 963c d9be e01c 3490 9110 d491  FBpG.<....4.....
+00001dd0: f522 0b8a 2965 3741 4642 3047 963c d9be  ."..)e7AFB0G.<..
+00001de0: e01c 8c40 4642 1047 963c d9be e01c 3490  ...@FB.G.<....4.
+00001df0: 9110 ec92 254f b62f 3807 0d64 2424 6d44  ....%O./8..d$$mD
+00001e00: 9e6c 5f70 0e1a c848 48da 883c d9be e07c  .l_p...HH..<...|
+00001e10: b881 e268 650f 83e8 117f 5e4a b9e4 c9f6  ...he.....^J....
+00001e20: 9832 47c1 cade 72f2 88f7 06ba 888f 29db  .2G...r.......).
+00001e30: 4044 c205 72c9 9227 db63 ca36 1091 b0b0  @D..r..'.c.6....
+00001e40: ab5b 579e 6c8f 29db 4044 c2c2 2e34 d049  .[W.l.).@D...4.I
+00001e50: 8829 db40 44c2 c22e 34d0 0d6c 4cd9 0622  .).@D...4..lL.."
+00001e60: 1216 76a1 812e 6063 ca36 1091 b0b0 0b0d  ..v...`c.6......
+00001e70: f439 21a6 6c03 1109 0bbb d040 bf44 8729  .9!.l......@.D.)
+00001e80: db40 44c2 0572 c912 c90c 53ae 814c 2e59  .@D..r....S..L.Y
+00001e90: a48d c845 3a4c d906 a28b 8485 5ddd 0422  ...E:L......].."
+00001ea0: 9961 ca36 9091 90b4 11b9 4cb8 02b9 a438  .a.6......L....8
+00001eb0: 1afd 1891 3622 92d9 e343 db2f 861d 818c  ....6"...C./....
+00001ec0: 84a4 8dc8 93ed 5720 97ac ed81 1cff 3926  ......W ......9&
+00001ed0: 6d44 24b3 c787 1e1d 818c 84a4 8d88 64b6  mD$...........d.
+00001ee0: 02b9 646d 0f24 1801 25a1 2c66 7d7c e6d1  ..dm.$..%.,f}|..
+00001ef0: 01c8 4008 af2f 5922 b92d 4ad9 7d30 0321  ..@../Y".-J.}0.!
+00001f00: 5923 22b9 adc0 2d29 8c46 4721 5a23 fd6e  Y#"...-).FG!Z#.n
+00001f10: c9e3 430f 6e82 cc2d 59e0 962c 71cc 38c5  ..C.n..-Y..,q.8.
+00001f20: cf71 5d5b 0339 be0f a25b d2ee 163c 3ef3  .q][.9...[...<>.
+00001f30: e800 641c 24b5 44e6 6381 59b2 b604 127c  ..d.$.D.c.Y....|
+00001f40: 7f9d 102a 8402 b164 6d07 24a8 aff3 4165  ...*...dm.$...Ae
+00001f50: 50e0 95ac cc2b 79c4 fba6 9573 92c0 2b59  P....+y....s..+Y
+00001f60: 5b01 0906 804e 79bf f1e5 b176 e7f1 a147  [....Ny....v...G
+00001f70: f7c0 8c82 e495 c874 34d0 4ad6 3640 8201  .......t4.J.6@..
+00001f80: d033 5e65 6060 95ac cc2a 79c4 dbd0 0a02  .3^e``...*y.....
+00001f90: 413d 7197 688b 5f11 8349 17e9 0f02 7a7c  A=q.h._..I....z|
+00001fa0: e6c1 ed9f 3925 8b6c 1139 0002 a564 65ef  ....9%.l.9...de.
+00001fb0: 3679 c4fb 57eb cfe0 e194 f909 d8f6 c7f1  6y..W...........
+00001fc0: 1d10 6511 6170 a094 acec dd26 8f78 1f01  ..e.ap.....&.x..
+00001fd0: 3927 0e94 92b5 ed8f 6004 e8ba 9f9c 1307  9'......`.......
+00001fe0: 4ac9 daf6 47d0 0041 5020 1428 252b 7bb7  J...G..AP .(%+{.
+00001ff0: c923 de37 819c 1307 4ac9 daf6 4730 0270  .#.7....J...G0.p
+00002000: dd4f 1cd7 c787 1ec4 40a6 942c 504a 9638  .O......@..,PJ.8
+00002010: ae98 7293 e14c 29a9 627a 4e2c 8e2b a66c  ..r..L).bzN,.+.l
+00002020: 03d9 3931 c922 e2b8 ae40 2959 9952 f288  ..91."...@)Y.R..
+00002030: b7ad 2b8e 2ba6 ec08 64e7 c424 8b88 e3ba  ..+.+...d..$....
+00002040: 02a5 646d fbe3 f851 40b2 8838 ae8f 0f3d  ..dm...Q@..8...=
+00002050: 7a14 64e7 c424 8b88 e3ba 02a5 646d fb23  z.d..$......dm.#
+00002060: 1801 20a1 38ae 8f0f 3d3a 02d9 7490 6411  .. .8...=:..t.d.
+00002070: 79b3 c70a 9492 b5ed 8f60 0480 847a 5920  y........`...zY 
+00002080: 504a 56a6 943c e26d 70c5 71c5 943b 0c33  PJV..<.mp.q..;.3
+00002090: a764 8153 b2c4 71c5 946d 2023 21d9 22e2  .d.S..q..m #!.".
+000020a0: b856 4bc7 6f55 654e c9c2 b79b c89c 3070  .VK.oUeN......0p
+000020b0: 4ad6 d63f 8eef 84af f12f 3fbd fbfc eec3  J..?...../?.....
+000020c0: fb3f 3f2c b15b 1f1f 77f0 00dc e247 50ba  .??,.[..w....GP.
+000020d0: ce88 df94 9679 60e0 91ac ad7c 04a5 0b96  .....y`....|....
+000020e0: 5f4b ebf5 e840 2059 dbf5 082a 17f6 de7c  _K...@ Y...*...|
+000020f0: 6999 7b06 eac8 da96 4750 baf8 f8a6 b4cc  i.{.....GP......
+00002100: 3a8f 4823 3f7e feed d3a7 2fbf 7cfc f2f1  :.H#?~..../.|...
+00002110: c3ff 0100 00ff ff00 0000 ffff 4451 db6a  ............DQ.j
+00002120: c330 0cfd 15a3 f7d5 4d4a e91a 9ac2 2e0c  .0......MJ......
+00002130: fa30 18f4 0bbc 44a9 cd12 cbc8 ead6 75ec  .0....D.......u.
+00002140: dfa7 f4b2 fa41 f6b1 d139 3ac7 2bb7 177a  .....A...9:.+..z
+00002150: 09bd 201b c6ae 8687 a27a 9ccd 1760 0e5c  .. ......z...`.\
+00002160: ed43 5bc3 cff4 b2ee 745f 8e65 7a2b d7b7  .C[.....t_.ez+..
+00002170: 5fb0 eb55 2696 ad38 c11b d3bd f20c 7dcc  _..U&..8......}.
+00002180: d5a1 e7b6 acc1 8ba4 cada dc78 1c5c 9e0c  ...........x.\..
+00002190: a161 cad4 c9a4 a1c1 52d7 8506 6d4e 8cae  .a......R...mN..
+000021a0: cd1e 5186 de96 d362 6139 34be 75e2 4a38  ..Q....ba94.u.J8
+000021b0: ab3c 516c 8304 8a17 a572 94b7 fffa eb55  .<Ql.....r.....U
+000021c0: f214 5142 f3c6 a6a3 281b f551 8091 ef84  ..QB....(..Q....
+000021d0: 3544 d2f6 4fe4 acfd 635f 723b 7c75 bc0b  5D..O...c_r;|u..
+000021e0: 319b 1e3b a961 3a51 ff1c 76fe 7a16 4aa7  1..;.a:Q..v.z.J.
+000021f0: db39 9877 12a1 e18a bc4e 8a3c a219 a812  .9.w.....N.<....
+00002200: 698c 6770 e1dd a2ec 9349 2e21 6fc3 51c5  i.gp.....I.!o.Q.
+00002210: 9760 8803 468d 49e5 6b48 9a19 bb20 60bc  .`..F.I.kH... `.
+00002220: de1f 7556 d73f a7a0 2460 7446 b570 c35c  ..uV.?..$`tF.p.\
+00002230: 8dff c19b b638 d9fd 22fe 38a5 b4fe 0300  .....8..".8.....
+00002240: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00002250: 0021 0038 a77c 8910 2500 0034 1801 0018  .!.8.|..%..4....
+00002260: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00002270: 2f73 6865 6574 322e 786d 6c9c 934b 8fdb  /sheet2.xml..K..
+00002280: 2010 c7ef 95fa 1d10 f718 db49 dcc6 8ab3   ..........I....
+00002290: 6a1b 455d a987 6ad5 c799 e071 8c02 c605  j.E]..j....q....
+000022a0: f252 d5ef de81 3c36 522e d65a 3603 86f9  .R....<6R..Z6...
+000022b0: fd67 6098 3f1d b522 7bb0 4e9a aea2 5992  .g`.?.."{.N...Y.
+000022c0: 5202 9d30 b5ec 3615 fdf9 6335 fa48 89f3  R..0..6...c5.H..
+000022d0: bcab b932 1d54 f404 8e3e 2dde bf9b 1f8c  ...2.T...>-.....
+000022e0: ddba 16c0 1324 74ae a2ad f77d c998 132d  .....$t....}...-
+000022f0: 68ee 12d3 4387 338d b19a 7b1c da0d 73bd  h...C.3...{...s.
+00002300: 055e 4727 ad58 9ea6 05d3 5c76 f44c 28ed  .^G'.X....\v.L(.
+00002310: 1086 691a 2960 69c4 4e43 e7cf 100b 8a7b  ..i.)`i.NC.....{
+00002320: 8cdf b5b2 7757 9a16 4370 9adb edae 1f09  ....wW..Cp......
+00002330: a37b 44ac a592 fe14 a194 6851 3e6f 3a63  .{D.......hQ>o:c
+00002340: f95a 61de c76c c205 395a 7c73 fcc6 5799  .Za..l..9Z|s..W.
+00002350: f8ff 4149 4b61 8d33 8d4f 90cc ce31 3fa6  ..AIKa.3.O...1?.
+00002360: 3f63 33c6 c58d f498 ff20 4c36 6116 f632  ?c3...... L6a..2
+00002370: 1ce0 2b2a 7f5b 48d9 f4c6 ca5f 61e3 37c2  ..+*.[H...._a.7.
+00002380: 8a1b 2c6c 972d 77b2 aee8 dff4 f28c d066  ..,l.-w........f
+00002390: a149 4769 169a bbe7 1f5d cc6b 8927 1cb2  .IGi.....].k.'..
+000023a0: 2216 9a8a 7eca cae5 b828 285b cc63 05fd  "...~....(([.c..
+000023b0: 9270 7077 7de2 4dff 0d1a ff05 94c2 d5e3  .ppw}.M.........
+000023c0: 7446 49a8 d1b5 31db b0f6 19b5 53c4 3a50  tFI...1.....S.:P
+000023d0: 2042 b510 8e66 0fe7 f59f c7f9 040b fd4f   B...f.........O
+000023e0: 948a 03d4 6137 a1fb fe55 7415 2bfb bb25  ....a7...Ut.+..%
+000023f0: 3534 7ca7 fc8b 397c 05b9 693d 5ea3 2299  54|...9|..i=^.".
+00002400: 62c6 a164 cafa b404 27b0 5651 3ec9 a721  b..d....'.VQ>..!
+00002410: 7e61 1442 b025 5a86 4b87 b5c6 8fd1 1e64  ~a.B.%Z.K......d
+00002420: ed5b ec65 c17f 0dce af64 c051 2276 ce1b  .[.e.....d.Q"v..
+00002430: fdfb 327d 819c ddf1 a0a2 3bda 8b7b 5e24  ..2}......;..{^$
+00002440: 192a 0d05 e0e1 4400 da0b a0c8 930f c3fd  .*....D.........
+00002450: 71e3 a23f da6b fc83 0260 711f fe03 0000  q..?.k...`q.....
+00002460: ffff 0000 00ff ff94 5ded aee5 3672 7c95  ........]...6r|.
+00002470: c53c 407c 49ea 835a d803 e448 2f62 3806  .<@|I..Z...H/b8.
+00002480: f6d7 26d8 319c e4ed d394 8339 ecaa eab9  ..&.1......9....
+00002490: ea7f f654 1dde 6e89 5491 54b3 f4f3 b77f  ...T..n.T.T.....
+000024a0: fcfe fb1f d7af 7ffc faf5 e77f fde7 7fff  ................
+000024b0: ed5f bf7c 295f fef6 edbf 7efd e737 fbaf  ._.|)_....~..7..
+000024c0: bf2f 5ffe f63f 65f9 f5b7 bfff c7ff 5ebf  ./_..?e.......^.
+000024d0: 7ffb edf7 7ffe f1cb 978f 7fab eb97 af3f  ...............?
+000024e0: ff36 b8ff 6e64 fba7 6ff6 ff7f 7e3d caf6  .6..nd..o...~=..
+000024f0: f34f 7f7e fdf9 a7df fe1f 7d79 74f7 e8e9  .O.~......}yt...
+00002500: d1ee d1cb a3c7 77f4 270b f37b ac35 13eb  ......w.'..{.5..
+00002510: 20df e97d 8f18 e365 465b df7f f9ce f8fc   ..}...eF[......
+00002520: b495 8b19 efcc 5df4 2d13 fd20 fbe8 e18a  ......].-.. ....
+00002530: bd98 d1b6 0fb8 e69f b672 3123 88de fac6  .........r1#....
+00002540: f37e 32c8 3e7a b8ae af4f 19e7 a78c 8b19  .~2.>z...O......
+00002550: 41ec 6b26 f641 f6b1 17b8 ac2f a674 1c0c  A.k&.A...../.t..
+00002560: e7e7 cd5c 4c09 e2df 32f1 0f32 c45f 60a0  ...\L...2..2._`.
+00002570: 32a5 171c ae9f 3773 3125 887f cfc4 3fc8  2.....7s1%....?.
+00002580: 107f 85f8 3fa7 9c9f 532e a604 e1f7 4cf8  ....?...S.....L.
+00002590: 830c e137 089f 29bd c0e8 3e3f 6fe6 624a  ...7..)...>?o.bJ
+000025a0: 10ff 9189 7f90 21fe 05e2 674a 2ff8 dcfc  ......!...gJ/...
+000025b0: bc99 8b29 41fc e523 93c0 cd86 0c56 54aa  ...)A..#.....VT.
+000025c0: d122 3c5e 2b3e 3c1f 3474 094e 9444 4e68  ."<^+><.4t.N.DNh
+000025d0: 071b 9220 b965 4edb 60a8 9f45 9160 3c5d  ... .eN.`..E.`<]
+000025e0: 8214 6591 92e0 c2da 88cf 9997 e0b4 0d46  ..e............F
+000025f0: cc29 49d0 2d2f 418a b248 4971 618d c4e1  .)I.-/A..HIqa...
+00002600: fa12 9cb6 41af 3b25 09ee ea25 4851 1629  ....A.;%...%HQ.)
+00002610: 492e ac96 3868 5f82 d336 9ac7 7143 6da3  I...8h_..6..qCm.
+00002620: e9dc 636d 2e29 71be d97e 5ce0 b87d 094e  ..cm.)q..~\..}.N
+00002630: dbf0 f9a4 483b 3c01 2e41 8aee 454a a20b  ....H;<..A..EJ..
+00002640: 2b67 458d 169c b6d3 e8e6 86da 4ea3 fbb1  +gE.........N...
+00002650: 4e97 9450 df6c b817 a8d4 82d3 761a ddac  N..P.l......v...
+00002660: c46d a7d1 fd58 ae4b 4aaf 6f36 6481 822d  .m...X.KJ.o6d..-
+00002670: 386d a7d1 cd7a dc76 1add 8f45 bba4 54fb  8m...z.v...E..T.
+00002680: 6643 1628 db82 d376 1add acca 6da7 d1fd  fC.(...v....m...
+00002690: 58ba 6b4a ba6f 3664 81d2 2d38 6da7 551b  X.kJ.o6d..-8m.U.
+000026a0: eb7b eb38 ba45 4bc1 e8ae 29ed bed9 9005  .{.8.EK...).....
+000026b0: 2d3d 852c 771c dda2 a1d6 7174 0b52 9445  -=.,w.....qt.R.E
+000026c0: 6ef9 ccda 5da1 b3bc aa58 4177 1cdd 9284  n...]....XAw....
+000026d0: a35b 90a2 2c52 da5d 59bb 2b2e a405 a775  .[..,R.]Y.+....u
+000026e0: 1cdd 9284 a35b 90a2 2c52 da5d 594d 2b2e  .....[..,R.]YM+.
+000026f0: a805 a775 1cdd 9284 a35b 90a2 2c52 da6d  ...u.....[..,R.m
+00002700: fb48 38a7 6db8 b256 9c4e a35b 3474 d0e8  .H8.m..V.N.[4t..
+00002710: 7ebc baae 29ed bed9 7e74 37d4 6ec5 3968  ~...)...~t7.n.9h
+00002720: 740b ed3e 6874 3fd6 ee9a d2ee 9b0d 59a0  t..>ht?.......Y.
+00002730: 762b ce41 a35b 68f7 41a3 fbb1 76d7 9476  v+.A.[h.A...v..v
+00002740: df6c 9f05 3d68 852a f326 1f93 6868 8b76  .l..=h.*.&..hh.v
+00002750: de69 fa5d ca94 7257 b19a 86d5 aaa0 f056  .i.]..rW.......V
+00002760: dfe7 ed5c aa9d 2087 96d2 ed9b 0dbd 0975  ...\.. ........u
+00002770: 5b71 0e7c ca0a d2b1 4297 bb54 4b51 1a29  [q.|....B..TKQ.)
+00002780: e16e 6aad 0cf7 4271 0ee8 2ca7 2075 9ce0  .nj...Bq..,. u..
+00002790: 5faa a528 8d94 7237 a1ca a8dc 8a73 a05a  _..(..r7.....s.Z
+000027a0: 0852 aff8 8452 2d45 69e4 76c0 c506 37ed  .R...R-Ei.v...7.
+000027b0: 810b ce81 5b69 4dec 8257 ea54 a2a5 288d  ....[iM..W.T..(.
+000027c0: 9476 37b1 5c46 ed96 1c54 3d41 ea15 9fb4  .v7.\F...T=A....
+000027d0: aaa5 288d 9478 3796 d305 c55b 72e8 9504  ..(..x7....[r...
+000027e0: 3774 6cd4 a984 c247 69a4 d4bb b19e 2ea8  7tl....Gi.......
+000027f0: de8a f381 ea2d 481d e701 9720 b528 8d94  .....-H.... .(..
+00002800: 7c37 16d4 05e5 5b71 3e80 740a 52af f054  |7....[q>.t.R..T
+00002810: be04 294c 23a5 df8d 4575 c1b5 b7e2 7ce0  ..)L#...Eu....|.
+00002820: 2c44 907a 4509 17a4 308d 9484 3796 f005  ,D.zE...0...7...
+00002830: 17df 8af3 01a4 5390 7aa3 b121 56e8 41a7  ......S.z..!V.A.
+00002840: 5a52 2a7e b3bd 8a2f a8e2 8af3 812a 2e48  ZR*~.../.....*.H
+00002850: bde1 0357 90a2 bbb1 a454 fc66 431a 382b  ...W.....T.fC.8+
+00002860: 549c 0f54 7141 ea53 88f7 fbe1 4b90 c234  T..TqA.S....K..4
+00002870: 522a beb0 8a2f a8e2 8af3 812a 2e48 1d57  R*.../.....*.H.W
+00002880: f297 2085 69a4 547c 615d 5d50 c515 e703  .. .i.T|a]]P....
+00002890: 555c 907a c327 9520 8569 e45e 68b3 8a2f  U\.z.'. .i.^h../
+000028a0: f44a 5b70 3e50 c517 2675 dc91 b804 294c  .J[p>P..&u....)L
+000028b0: 23a5 e20b ebea 8a2a 2e38 0bbe 013f 05a9  #......*.8...?..
+000028c0: 377c e00a 5298 464a c517 56f1 1555 5c70  7|..R.FJ..V..U\p
+000028d0: 9682 2a2e 48bd c100 ba04 294c 23a5 e20b  ..*.H.....)L#...
+000028e0: abf8 8a2a 2e38 4b41 1517 a4de 705b 4790  ...*.8KA....p[G.
+000028f0: c234 522a beb0 8ae3 9aed 2538 4b41 1517  .4R*......%8KA..
+00002900: a4de 6000 5d82 14a6 9152 f185 7575 4515  ..`.]....R..uuE.
+00002910: 179c a5a0 8a0b 52c7 edba 4b90 a234 d694  ......R...K..4..
+00002920: 8adf 6c2f 7f2b aab8 e02c 0555 5c90 3aee  ..l/.+...,.U\.:.
+00002930: d75d 8214 a691 52f1 95d7 e22b aab8 e02c  .]....R....+...,
+00002940: 5c87 c30d 755c b95c a2a5 308d 948a afac  \...u\.\..0.....
+00002950: e22b aab8 e02c 548e 2348 1d57 2e97 2085  .+...,T.#H.W.. .
+00002960: 69a4 547c 6515 a79b 2116 d0b4 d1f6 793b  i.T|e...!.....y;
+00002970: 97a0 acef 4799 db68 5b53 127e b3a1 e603  ....G..h[S.~....
+00002980: 3677 0485 37da 3e6f e712 9430 875c 6d9a  6w..7.>o...0.\m.
+00002990: d06f 9c86 ac62 a54e 8a21 4878 b32e c589  .o...b.N.!Hx....
+000029a0: ee44 4abe 5796 6fac 5c7c 09ce 4245 5282  .DJ.W.o.\|..BER.
+000029b0: 7460 39c0 2548 e1cd 48c9 f7ca f28d e537  t`9.%H..H......7
+000029c0: 2fc1 59a8 564a 900e da2e 14a4 308d 947c  /.Y.VJ......0..|
+000029d0: af62 f31b 6721 82b3 50bd 9420 1db4 5d28  .b..g!..P.. ..](
+000029e0: 4861 1a29 f95e 59be b18c e825 380b 5ee8  Ha.).^Y....%8.^.
+000029f0: 5390 0eda 2e14 a428 8d2d 25df 371b 5e69  S......(.-%.7.^i
+00002a00: e02c 4470 16bc d0a7 201d b45d 2848 611a  .,Dp.... ..](Ha.
+00002a10: 29f9 de58 75b1 1cea 2538 0b5e e853 900e  )..Xu...%8.^.S..
+00002a20: daa0 12a4 308d 947c 6fa2 fc1b 854f 7016  ....0..|o....Op.
+00002a30: bcd0 a720 1db4 4125 4861 1a29 f9de 847c  ... ..A%Ha.)...|
+00002a40: e32c 4470 16bc d0a7 201d b497 2048 611a  .,Dp.... ... Ha.
+00002a50: 2905 df78 ed8c 8567 2fc1 59f0 429f 8274  )..x...g/.Y.B..t
+00002a60: d022 5c90 c234 5222 beb1 4063 79da 4b70  ."\..4R"..@cy.Kp
+00002a70: 16bc d0a7 201d b4d0 10a4 308d 948a 6fe2  .... .....0...o.
+00002a80: d534 ee25 08ce 8217 fa14 a483 161a 8214  .4.%............
+00002a90: a691 52f1 4dbc 9ba6 7a79 b5dd 8e3b 3ba2  ..R.M...zy...;;.
+00002aa0: a183 de08 0852 9846 4ac5 3751 5886 2a2e  .....R.FJ.7QX.*.
+00002ab0: 380b 5ee8 5390 0eda 8316 a430 8d94 8a6f  8.^.S......0...o
+00002ac0: a2b2 0cdf 0808 ce82 17fa 14a4 83f6 a005  ................
+00002ad0: 294a 634f a9f8 cdf6 2a8e 058d 2fc1 59f0  )JcO....*.../.Y.
+00002ae0: 429f 8274 d01e b420 8569 a454 7c67 15c7  B..t... .i.T|g..
+00002af0: b2c7 97e0 2c78 a14f 413a 68f3 5690 c234  ....,x.OA:h.V..4
+00002b00: 522a be8b 235a a8e2 8253 3e48 c635 0b77  R*..#Z...S>H.5.w
+00002b10: a105 2b4c 24a5 e33b eb38 1670 be04 67c1  ..+L$..;.8.p..g.
+00002b20: 1e73 0ad2 41db b782 14a6 91d2 f15d 1487  .s..A........]..
+00002b30: e33b 01c1 59b0 c79c 8274 d0f6 ad20 8569  .;..Y....t... .i
+00002b40: a474 7c17 1566 b818 179c 052f f429 4807  .t|..f...../.)H.
+00002b50: 6ddf 0a52 9846 4ac7 77d6 712c 957d 098e  m..R.FJ.w.q,.}..
+00002b60: 8d0e 7c61 2658 07ed df0a 5298 474a c877  ..|a&X....R.GJ.w
+00002b70: 1669 aca8 7d09 8ee5 816f cc04 eba0 2d43  .i..}....o....-C
+00002b80: 410a f348 29f9 ce4a 8e45 bf2f c159 b0e3  A..H)..J.E./.Y..
+00002b90: 9f82 74d0 96a1 2085 69a4 947c 1775 6da8  ..t... .i..|.um.
+00002ba0: e482 b360 c73f 05e9 c062 874b 90a2 347a  ...`.?...b.K..4z
+00002bb0: 4ac9 6f36 ec1a e27a 5c70 16ec f7a7 201d  J.o6...z\p.... .
+00002bc0: 58ec 7009 5298 464a c9bb d805 c7b7 0282  X.p.R.FJ........
+00002bd0: c32f fe04 e9a0 9a74 410a d348 2979 6725  ./.....tA..H)yg%
+00002be0: efa8 e482 b3e0 e83d 05e9 c09a 8d4b 90c2  .......=.....K..
+00002bf0: 3452 3ade 4545 1aae c705 67c1 d17b 0ad2  4R:.EE....g..{..
+00002c00: 8135 1b97 2085 69a4 74bc 8b77 d9a8 e382  .5.. .i.t..w....
+00002c10: b3e0 e83d 05e9 58f0 6db2 2085 69a4 74bc  ...=..X.m. .i.t.
+00002c20: b38e 63c9 f94b 704c 38e8 d0ae a86d c3a2  ..c..KpL8....m..
+00002c30: 8d4b 3415 e691 12f2 2eb6 d5f1 e4b1 a839  .K4............9
+00002c40: a797 349f b773 09ca 5480 ef5e d2f4 9488  ..4..s..T..^....
+00002c50: dfec 1fbf a411 147e 49f3 793b 97a0 8439  .......~I.y;...9
+00002c60: a404 bcab 9273 bc11 8243 d5d0 a2a1 834e  .....s...C.....N
+00002c70: f729 d27b 1bc6 df8a 9480 7716 703c c3f0  .).{......w.p<..
+00002c80: 129c 0545 ed14 a44e 02ae fe5a 90c6 9112  ...E...N...Z....
+00002c90: f09b ed7b 149e b278 09ce 826a 700a 5227  ...{...x...jp.R'
+00002ca0: 0157 7f2d 4a23 25e0 070b 389e c578 09ce  .W.-J#%...8..x..
+00002cb0: 826a 70aa 86b0 22eb 52a4 288d 9480 1f2c  .jp...".R.(....,
+00002cc0: e078 5ae4 2538 0baa c129 489d 045c fdb5  .xZ.%8...)H..\..
+00002cd0: 288d 9480 1f2c e038 7a5f 82b3 a018 9c82  (....,.8z_......
+00002ce0: d449 c0d5 5f8b d248 09f8 c102 8e67 195e  .I.._..H.....g.^
+00002cf0: 82b3 607f 3955 4358 1f77 2952 9446 4ac0  ..`.9UCX.w)R.FJ.
+00002d00: 0f21 bb38 9d12 9c05 233c 05a9 d33c 44fd  .!.8....#<...<D.
+00002d10: b528 8d94 7e1f 2cce 7896 e125 380b 56f0  .(..~.,.x..%8.V.
+00002d20: 9d82 d469 1aa2 fe5a 9446 4ac2 0f5e 871f  ...i...Z.FJ..^..
+00002d30: b82d 2238 0b56 f09d 82d4 f949 25fe 5a94  .-"8.V.....I%.Z.
+00002d40: 464a c50f 56e8 f281 ef37 0469 c112 be53  FJ..V....7.i...S
+00002d50: 900e 3c03 7f29 5294 474a c60f 96f1 82a7  ..<..)R.GJ......
+00002d60: 195e 82b4 600d df29 489d 07b9 9835 0479  .^..`..)H....5.y
+00002d70: d8e5 ccf9 baf0 a16e 9b83 93b3 0bb3 16ac  .......n........
+00002d80: e33b fffa d330 cfc4 7164 e62e dc56 3445  .;...0..qd...V4E
+00002d90: b46b 9a4b 86f5 bce0 b186 d75f 8d62 493e  .k.K......._.bI>
+00002da0: 190f dc7f 1aa6 3822 1931 8308 ef4c 4ad4  ......8".1...LJ.
+00002db0: ed2e 08cf 2cdc 2551 ac05 6bfa ecce 8825  ....,.%Q..k....%
+00002dc0: 3e3e 1aec ce88 7944 984c 4ada ed2e 8864  >>....yD.LJ....d
+00002dd0: d840 48d4 b563 659f 2523 16fa f87c b064  .@H..ce.%#...|.d
+00002de0: c46c 224c 2625 f0e5 8315 bee0 4107 eb66  .l"L&%......A..f
+00002df0: a272 7d5a 93fe e584 a758 9d0e 672a 563c  .r}Z.....X..g*V<
+00002e00: 6652 325f 3e58 e70b 1e77 b064 44fd 1bad  fR2_>X...w.dD...
+00002e10: 7115 eb60 cf11 d156 9c4c 4aec ed2e 886e  q..`...V.LJ....n
+00002e20: 86bb 278a b590 cb9f 6275 7ce6 5937 13f3  ..'.....bu|.Y7..
+00002e30: 8bb0 9ba5 24df ee82 4806 455f b116 36ac  ....$...H.E_..6.
+00002e40: 126d 75ac 60b6 649e eb7e f948 09ff 5f74  .mu.`.d..~.H.._t
+00002e50: ff38 2d64 01a8 580b 9e63 b407 00cf 220e  .8-d..X..c....".
+00002e60: 7c85 6ac9 0856 7867 52ea 5f3e 84fc e331  |.j..VxgR._>...1
+00002e70: 081b 33cc 5ad8 844b b03a 3ec0 2d99 c40c  ..3.Z..K.:>.-...
+00002e80: 20e9 eca6 1cd9 b0b4 f565 f78a 3ae3 b261   ........e..:..a
+00002e90: 91be 6275 7c80 9b31 5a62 0670 bba8 3db7  ..bu|..1Zb.p..=.
+00002ea0: 5215 a66b 058f 4458 32ac da0b 1b8b 09d6  R..k..DX2.......
+00002eb0: c1de 438a 1575 b3db 4c2d 918c 9801 e0c1  ..C..u..L-......
+00002ec0: 084b 469c 69db f02d a262 7554 23bb 3389  .KF.i..-.buT#.3.
+00002ed0: 19c0 eda9 9648 46cc 00f0 7884 2523 6600  .....HF...x.%#f.
+00002ee0: 6c96 2658 9d2a ad55 5ba1 cedc 266d 8964  l.&X.*.U[...&m.d
+00002ef0: c40c 809d 7b85 f3db 82b5 75e6 2528 f60b  ....{.....u.%(..
+00002f00: 786e a658 6137 cbcd 0084 215b 6147 41c1  xn.Xa7....![aGA.
+00002f10: 5ad8 004e b03a 4aab 7533 b1b7 1026 939b  Z..N.:J.u3...&..
+00002f20: 0108 87b7 c2c6 8282 b5a0 519d dd19 f112  ..........Q.....
+00002f30: 1fa5 d592 49cc 0092 5e70 c2e8 adb0 bfa0  ....I...^p......
+00002f40: 602d 6c6a 2758 9d2c 02ec bed3 633e 1e33  `-lj'X.,....c>.3
+00002f50: b919 80f0 7b2b 6c33 2858 0b6e cfdb 9d51  ....{+l3(X.n...Q
+00002f60: 3300 3c62 2859 6137 cbcd 0084 ed5b 61b7  3.<b(Ya7.....[a.
+00002f70: 41c1 5ad8 a84f b03a ce13 ac9b 2566 0039  A.Z..O.:....%f.9
+00002f80: 8338 bb0b 3cd1 c4d2 77b3 1415 3300 9cdc  .8..<...w...3...
+00002f90: 9ba7 28b3 3ace 13cc 5434 3103 c8f9 c4d9  ..(.:...T41.....
+00002fa0: 5d10 c990 f7a0 602d 6c3e 2858 07fb f629  ].....`-l>(X...)
+00002fb0: 56d4 cd6e 4bb6 e73a 231c dc0a d6cf d99d  V..nK..:#.......
+00002fc0: 1133 009c a8d8 9d51 aff9 b1ca 4eb1 c207  .3.....Q....N...
+00002fd0: c0ed cc96 4846 cc00 b018 de92 1133 0036  ....HF.......3.6
+00002fe0: 5414 ac8e 931e eb66 893d 80db a02d 918c  T......f.=...-..
+00002ff0: 9801 60ed 9625 23f6 00b0 03d9 9d11 affc  ..`..%#.........
+00003000: 71d2 63c9 8879 42d8 cd72 3300 6110 57c8  q.c..yB..r3.a.W.
+00003010: 97b0 08d6 4226 918a 7520 cb92 49cc 0072  ....B&..u ..I..r
+00003020: 5672 45f8 c415 b227 54ac 052b f4ec cea8  VrE....'T..+....
+00003030: 1900 1977 0a56 3c66 727b 00c2 2eae 904b  ...w.V<fr{.....K
+00003040: a1dd 2b5e 9c91 f1a5 6275 9cc1 d99d 49cc  ..+^....bu....I.
+00003050: 0072 c672 7617 f8d1 4c66 858a b560 3194  .r.rv...Lf...`1.
+00003060: dd19 51d0 c756 c382 15df 99dc 0c40 f8be  ..Q..V.......@..
+00003070: 15f2 2cb4 7b25 ee0c 1b71 0b6d 2767 55d5  ..,.{%...q.m'gU.
+00003080: 5698 4cce 6aae 08f7 b782 65f3 66c7 2d66  V.L.j.....e.f.-f
+00003090: 009d f600 04ab e374 d40c b913 3380 dbd4  .......t....3...
+000030a0: edf9 a359 78c0 152c 9eb7 64c4 1e00 1994  ...Yx..,..d.....
+000030b0: 2a56 672f 68d1 567c 6772 6f01 8413 5cc1  *Vg/h.V|gro...\.
+000030c0: ca73 4b46 cc00 b086 cf9c d2c5 0c80 de99  .sKF............
+000030d0: 2956 9c4c ee2d 8030 8d2b 587f 6ec9 8819  )V.L.-.0.+X.n...
+000030e0: 0099 ae2a 56e7 bd66 d156 9c4c ee2d 8070  ...*V..f.V.L.-.p
+000030f0: 852b 5885 6ec9 8819 40c7 1237 c53a f001  .+X.n...@..7.:..
+00003100: 6e63 2631 03b8 6de3 1263 46bc 05c0 da67  nc&1..m..cF....g
+00003110: 4b46 bc05 2023 59c5 eabc 3d2b da8a ef4c  KF.. #Y...=+...L
+00003120: 6e0f 4038 c415 ac80 b664 58db 1734 bcb5  n.@8.....dX..4..
+00003130: 3123 6600 bc09 2858 7132 b919 80f0 892b  1#f...(Xq2.....+
+00003140: 5807 6dc9 8819 0099 e32a 56c7 b9b5 75b3  X.m......*V...u.
+00003150: c40c e0b6 7f4b 7433 3103 20c7 43bb 572c  .....Kt31. .C.W,
+00003160: 9a58 5e66 7746 cd00 686e 2658 f19d c9cd  .X^fwF..hn&X....
+00003170: 0084 b15c 21df 43bb 5722 199a 0128 933a  ...\!.C.W"...(.:
+00003180: 9e35 0b56 984c cea6 ae08 e7b8 42ee 878a  .5.V.L......B...
+00003190: b560 a9d9 a958 9da7 33e2 2fc6 c9e4 ea00  .`...X..3./.....
+000031a0: 847f 5c21 0f44 bb57 e2ce 501d 806a eb83  ..\!.D.W..P..j..
+000031b0: 0e04 abc6 e26c 7253 0061 2357 c80a d16e  .....lrS.a#W...n
+000031c0: 96c8 865e 0328 df3a 161a c18a 93c9 4d01  ...^.(.:......M.
+000031d0: 8499 5c21 4344 bb59 2219 3c51 a458 9d8e  ..\!CD.Y".<Q.X..
+000031e0: 4d28 569c 4c6e 0a20 2ce5 0a96 b6d9 f75f  M(V.Ln. ,......_
+000031f0: c414 80fc 7415 aba3 edff a558 7132 b94d  ....t......Xq2.M
+00003200: 0061 2c57 c81c d1ee 95b8 33f4 1d18 e564  .a,W......3....d
+00003210: 872b 054b 26b1 0970 fbc5 3d17 1a61 2f57  .+.K&..p..=..a/W
+00003220: c822 d1ee 1525 b362 399a 3dce c414 0057  ."...%.b9.=....W
+00003230: 0a96 4ce2 35c0 ed1a 9748 4614 0290 51a2  ..L.5....HF...Q.
+00003240: dd2b 910c 7ddb 46b9 dae1 4ac1 9249 4c01  .+..}.F...J..IL.
+00003250: 6eef b844 322c db78 d8c8 ee14 a5c2 1f91  n..D2,.x........
+00003260: 542c 3cde a238 65aa e272 95fc e5b6 8f4b  T,<..8e..r.....K
+00003270: 64c2 ca4e a526 ca91 8e4b 4d94 b91d 7eca  d..N.&...KM...~.
+00003280: 5370 e24c 72ee 76d6 8eb8 de58 03a8 4874  Sp.Lr.v....X..Ht
+00003290: ba42 35c5 c72b 14eb 07c9 e4c4 5fd8 ce15  .B5..+......_...
+000032a0: 32b2 b47f 11a3 052d 2015 8bda b20f 5a89  2......- .....Z.
+000032b0: 570e 6127 bbed e49e 7732 e13e 57c8 cfd2  W.a'....w2.>W...
+000032c0: fe45 6443 934c 6577 870b 6bcb 4654 1dc4  .EdC.Lew..k.FT..
+000032d0: d9e4 d45f f8d0 15b2 b5b4 7f11 d9d0 3e93  ..._..........>.
+000032e0: 6075 5c59 5b36 e2a5 439c 4d4e fe85 235d  `u\Y[6..C.MN..#]
+000032f0: 2177 4bfb 1791 0d4d 339f b465 d988 b70e  !wK....M3..e....
+00003300: 7136 39fd 17ce 7485 4c2e ed5f 4436 34cd  q69...t.L.._D64.
+00003310: 14ac 8e1b 0596 8dd8 7488 b3c9 ed01 0883  ........t.......
+00003320: ba42 5e97 f62f 221b 9a67 0a56 c79d 02cb  .B^../"..g.V....
+00003330: 46d4 1ec6 d9e4 3601 844f 5d21 cb4b fb17  F.....6..O]!.K..
+00003340: 910d ed35 0956 c7ad 02cb 46cc 39e2 6c72  ...5.V....F.9.lr
+00003350: 9500 c2ae ae60 2d92 7d70 9027 012b 393f  .....`-.}p.'.+9?
+00003360: 2b56 a70f fe28 d60f f426 b70d 205c eb0a  +V...(...&.. \..
+00003370: 1623 5936 3c59 58c9 005a b13a 9e48 b37b  .#Y6<YX..Z.:.H.{
+00003380: 23ca 0fc3 7b93 73ca 2bc2 bcce fe0d e702  #...{.s.+.......
+00003390: cae2 8e7c a055 5b9d 3e63 24ff 629c 4d6e  ...|.U[.>c$.b.Mn
+000033a0: 2e20 3cec 0ad9 49da bff0 b821 734f c5ea  . <...I....!sO..
+000033b0: 38ff b914 2bee 69b7 37dd f3b9 80b0 b22b  8...+.i.7......+
+000033c0: 58c2 f3b2 7f11 d9d0 5c40 b03a 1e53 b36c  X.......\@.:.S.l
+000033d0: 3273 81db a22e 918d 5066 3297 2cca f78e  2s......Pf2.,...
+000033e0: cca1 15ab e397 772c 9bcc 5ce0 76aa 4b64  ......w,..\.v.Kd
+000033f0: 2394 19eb 5eec de88 b900 7944 2b56 c70d  #...^.....yD+V..
+00003400: 03cb 2633 17b8 0deb 12d9 0865 26ab c9a2  ..&3.......e&...
+00003410: 5cf0 c82a 5ab1 3a9e 5db3 6c32 7381 dbb7  \..*Z.:.].l2s...
+00003420: 2e91 8d50 662c 16b1 7b23 e602 e418 ad58  ...Pf,..{#.....X
+00003430: 076e 1958 3699 b9c0 6d5f 97c8 4628 3356  .n.X6...m_..F(3V
+00003440: 8b58 3662 2e40 56bf 8a75 e039 36cb 2633  .X6b.@V..u.96.&3
+00003450: 17b8 5dec 12d9 8837 02e4 3f59 9435 1e39  ..]....7..?Y.5.9
+00003460: fe2a d681 67d9 2c1b f117 63bd c9cd 0584  .*..g.,...c.....
+00003470: f75d 211b 4afb 177e 42f3 87d2 95d9 1e1e  .]!.J..~B.......
+00003480: 66b3 6c32 7381 9cdf 5e11 1678 f66f 3817  f.l2s...^..x.o8.
+00003490: 5046 79e4 ffab da3a f053 3d97 fc8b e1bd  PFy....:.S=.....
+000034a0: b9ad ed9e f734 e184 57b0 2ee1 65ff 22ee  .....4..W...e.".
+000034b0: 0ded 0b28 eb3d fc62 8f65 93d9 17b8 fded  ...(.=.b.e......
+000034c0: 12d9 0865 c6c2 04cb 46cc 05c8 0d58 b10e  ...e....F....X..
+000034d0: 3ccf 66d9 64e6 02b7 cd5d 221b 5666 da14  <.f.d....]".Vf..
+000034e0: 14ce 7962 5350 b068 5350 70ca 5407 e137  ..ybSP.hSPp.T..7
+000034f0: 056f a7bb 4426 a296 8f46 0c73 d86c a508  .o..D&...F.s.l..
+00003500: 8b3d 7abb 2938 3fc8 24b7 1fa0 bcf1 b8f6  .=z.)8?.$.......
+00003510: 54b2 6877 4399 f1f1 b100 c1fa 4136 b9fd  T.hwC.......A6..
+00003520: 00e5 90c7 f59a 9245 fb01 ca92 8fcf 0528  .......E.......(
+00003530: 7bbf b897 e5f6 0384 4f1e d7d1 2812 6fd8  {.......O...(.o.
+00003540: 2a5f 3e3e 80aa 3cfe e264 72db 01c2 2dcf  *_>>..<..dr...-.
+00003550: 3a3f 0d1a b11d 405e 5145 d9f3 f1a1 4df9  :?....@^QE....M.
+00003560: 17df 4b24 7800 e4a6 00c2 34af 90bf 6b51  ..K$x.....4...kQ
+00003570: d67a f852 f954 ac83 4f6d cabf 1865 9333  .z.R.T..Om...e.3
+00003580: ea2b c23b af60 f9cb 4bb1 56f2 4056 ac83  .+.;.`..K.V.@V..
+00003590: 4f3a cabf 1866 93db 0e10 167a 85bc 5e8b  O:...f.....z..^.
+000035a0: 32da 232b 64c5 3af0 dcf4 a558 f123 edb6  2.#+d.:....X.#..
+000035b0: c67b 2e35 c249 cffa 3f8e 1be5 b747 8ec8  .{.5.I..?....G..
+000035c0: 4559 f7e1 d7e2 2c1b 35e9 08ef 4dee d580  EY....,.5...M...
+000035d0: 30d4 b3fe 4fd9 8857 0364 8c5c 9483 1f6e  0...O..W.d.\...n
+000035e0: 1d5a 3662 3b20 7ca6 dd46 7989 7b23 16e7  .Z6b; |..Fy.{#..
+000035f0: 6400 5b94 fb1e d90a 2bd6 815b 8796 8df8  d.[.....+..[....
+00003600: 8b71 36b9 a980 32ea 231b d8a2 3cf8 c85d  .q6...2.#...<..]
+00003610: 58b1 0edc 3ab4 6cc4 7640 9c4d 6e2a 207c  X...:.l.v@.Mn* |
+00003620: f6ac 6753 4f13 db01 6432 5c94 671f 1f78  ..gSO...d2\.g..x
+00003630: 567f 31ce 2637 1510 8e7b d6b3 291b b11d  V.1.&7...{..)...
+00003640: 40de b645 b9f7 f121 61f5 17e3 6c72 7301  @..E...!a...lrs.
+00003650: 61bc 673d 9bb2 1173 01b2 b82d cac4 0fb7  a.g=...s...-....
+00003660: 75ad a789 ed80 389b dc5c 40f8 ef59 cfa6  u.....8..\@..Y..
+00003670: 6cc4 7600 39dd 16e9 1c88 df7f 55ac 586f  l.v.9.......U.Xo
+00003680: 729e 7f45 d8f0 59ff c76c 046b 25a7 58d9  r..E..Y..l.k%.X.
+00003690: d607 7d9f 42d2 c29b 73fb eb3d 7f44 0b3b  ..}.B...s..=.D.;
+000036a0: 3e1b 0094 8ed8 0f20 c7d8 a2ac fd70 97fa  >...... .....p..
+000036b0: 52ac 1fdc 9c5c 91a0 70e5 b3ae 4dd9 88fd  R....\..p...M...
+000036c0: 0032 8e2d cae1 0f77 a92d 9bcc 64e0 76db  .2.-...w.-..d.v.
+000036d0: 4bdc 1b21 cd64 1f5b 8485 df4a 4699 8a75  K..!.d.[...JF..u
+000036e0: b059 8068 eb07 f726 5727 203c faac 67d3  .Y.h...&W' <..g.
+000036f0: bd11 ef06 c82f b3a8 b63e e88b 2892 160f  ...../...>..(...
+00003700: 9cdc 6c60 78f5 fdf1 cb97 6f5f befe fce7  ..l`x.....o_....
+00003710: d783 b737 01a7 574f 80c3 d3dd 3a16 6b7f  ...7..WO....:.k.
+00003720: f4c1 c572 1bee 25fa 9589 fa3b 74de cb1c  ...r..%....;t...
+00003730: cd4d a9d1 3e06 e0b4 b324 fcff e2d0 733a  .M..>....$....s:
+00003740: 3f8c fba6 d0f1 6b3a c5e3 ec99 0138 6d25  ?.....k:.....8m%
+00003750: 0963 c038 f49c a80f 1bbe efa1 57b6 9670  .c.8........W..p
+00003760: f84a e6aa c5e1 0717 c53a 7c5a 0df8 75fc  .J.......:|Z..u.
+00003770: edb4 97e8 2aa6 ca53 d0fc 289d f195 ac54  ....*..S..(....T
+00003780: cbf8 73ef fbc5 c5af 0e8f 82ae 3937 bf9b  ..s.........97..
+00003790: 3e05 8dcb 278f af64 9c8a 3876 128f c741  >...'..d..8v...A
+000037a0: a756 e575 38ed bd83 264b 088f afe4 2fea  .V.u8...&K..../.
+000037b0: f183 2a73 3d1e 079d d2db 3abc f2a6 a071  ..*s=.....:....q
+000037c0: 387a 7c25 3751 c4e1 f797 c7e3 a053 6bec  8z|%7Q.......Sk.
+000037d0: 3a3c f1a6 a071 cde3 f195 3c37 11c7 d9a7  :<...q....<7....
+000037e0: c7e3 a053 ea59 878f de14 342e 6d3c be92  ...S.Y....4.m<..
+000037f0: 2b25 e2e8 78e0 f138 e894 46d6 e171 3705  +%..x..8..F..q7.
+00003800: 8d2b 188f af64 d888 385a 9b78 3c0e 3ab5  .+...d..8Z.x<.:.
+00003810: 30ae c3cb 6e0a 1a17 2a1e 5fc9 cb10 71fc  0...n...*._...q.
+00003820: c8b8 c7e3 a053 ba58 8767 ddf4 9cc5 f508  .....S.X.g......
+00003830: e2b8 998f 383f f2e6 f6e3 a053 8a58 8737  ....8?.....S.X.7
+00003840: dd74 a539 e819 5fa9 60dc ff7e a577 0f1e  .t.9.._.`..~.w..
+00003850: 8f83 4ead 66eb f0a0 9b82 c6a5 92c7 57b2  ..N.f.........W.
+00003860: ed43 9c9f 1e73 fb61 d039 77bb 3ae8 53d0  .C...s.a.9w.:.S.
+00003870: 28e3 1e5f c9d1 0e71 7a7a b8f6 e3a0 738a  (.._...qzz....s.
+00003880: 383c e5a6 a049 c61d be92 d95b 059c 9e1e  8<...I.....[....
+00003890: 0e8f 83ce 29e2 f08e 9b06 2207 ed70 3a69  ....)....."..p:i
+000038a0: 5bfd efa9 22d5 e371 d039 451c 4e72 ef2b  [..."..q.9E.Nr.+
+000038b0: 4d66 14d5 e12b 99b7 214e 8f3c f7fb 38e8  Mf...+..!N.<..8.
+000038c0: 9c22 0e2f b829 689a 7b38 7c25 5fb3 0a38  ."./.)h.{8|%_..8
+000038d0: cd3d 1c1e 079d 53c4 e1f9 3605 4d73 0f87  .=....S...6.Ms..
+000038e0: af64 f955 01a7 a787 c3e3 a073 8a38 bcdd  .d.U.......s.8..
+000038f0: a6a0 69ee e1f0 95dc b02a e0fc f498 db8f  ..i......*......
+00003900: 83ce 29e2 f070 9b82 a6b9 87c3 5732 8ab2  ..)..p......W2..
+00003910: 05da f4fb 95ce 877b 3c0e 3aa7 88c3 d16d  .......{<.:....m
+00003920: 0a9a e61e 0e5f c943 a93a fca0 0a70 8fc7  ....._.C.:...p..
+00003930: 41e7 1471 78b2 4d41 938c 3b7c 25af a4ea  A..qx.MA..;|%...
+00003940: 713a 22ed f130 e89c db5b 1df4 2968 9271  q:"..0...[..)h.q
+00003950: 87af 6423 e47f bfd2 795b 8fc7 41e7 1471  ..d#....y[..A..q
+00003960: 78ac 4d41 938c 3b7c c52d 82b3 3afc a092  x.MA..;|.-..:...
+00003970: 7a8f c741 e714 7138 ae4d 4193 223a 7c25  z..A..q8.MA.":|%
+00003980: 279d eaf0 832a e73d 1e07 9d53 c4e1 99f6  '....*.=...S....
+00003990: 0e9a cc19 aac3 5772 cc41 1cb7 c83c 1e07  ......Wr.A...<..
+000039a0: 9d53 c4e1 8d36 054d 8ae8 f095 cc64 2ae0  .S...6.M.....d*.
+000039b0: b408 7078 1c74 4e11 8707 da14 3429 a2c3  ..px.tN.....4)..
+000039c0: 57f2 59a9 1ea7 0349 1e8f 83ce 29e2 f03a  W.Y....I....)..:
+000039d0: 9b82 2645 74f8 4a16 24d5 e107 9d9f f078  ..&Et.J.$......x
+000039e0: 1c74 4e11 87a7 d914 3429 a2c3 57b2 1aa9  .tN.....4)..W...
+000039f0: 0e3f e898 84c7 e3a0 738a 38bc cba6 a049  .?......s.8....I
+00003a00: 111d bee2 23cd 1e79 f3ef 0f3a 0de1 f138  ....#..y...:...8
+00003a10: e89c 220e bfb3 2968 5244 87af 641d 521d  .."...)hRD..d.R.
+00003a20: 7ed0 a107 8f87 41e7 dccf eaa0 4f41 9322  ~.....A.....OA."
+00003a30: 3a7c a512 3aff fb83 ce36 783c 0e3a a788  :|..:....6x<.:..
+00003a40: c373 6c0a 9a14 d1e1 2bf6 d9b3 024e 6b44  .sl.....+....NkD
+00003a50: 87c7 41e7 1471 3890 4d41 9322 3a7c 2593  ..A..q8.MA.":|%.
+00003a60: 8c0a 382d b71c 1e07 9d53 c4e1 21f6 0e1a  ..8-.....S..!...
+00003a70: b772 5fd5 e11b f947 204e cb2d f7fb 38e8  .r_....G N.-..8.
+00003a80: 9c22 0eaf b029 6852 4487 6f78 4ac2 bac7  ."...)hRD.oxJ...
+00003a90: fcfb 8dce 1d78 3c0e 3aa7 88c3 136c 0a9a  .....x<.:....l..
+00003aa0: 14d1 e11b 1e1f b0a0 e7df 6f54 90ef f138  ..........oT...8
+00003ab0: e89c 220e efaf 2968 5244 876f 5857 6f41  .."...)hRD.oXWoA
+00003ac0: cfbf b7af 23c1 8be1 cb13 e2a8 7392 384c  ....#.......s.8L
+00003ad0: bea6 a849 121d be61 61a3 453d ff7e a352  ...I...aa.E=.~.R
+00003ae0: 418f c741 e724 7198 794d 4193 243a 7ca3  A..A.$q.yMA.$:|.
+00003af0: c3c2 d5e3 5443 e7f1 38e8 9c24 0ed3 ae29  ....TC..8..$...)
+00003b00: 6892 4487 6f74 8ab6 3adc fa07 3f3f 1eed  h.D.ot..:...??..
+00003b10: 9be6 fcc0 eaa0 4f51 9326 3a7c a3d3 b2fe  ......OQ.&:|....
+00003b20: f71b 7e82 e3f2 7878 a96f f3ad c7ef 6ceb  ..~...xx.o....l.
+00003b30: a04f 4193 263a 7ca3 63a4 fef7 1b95 bc78  .OA.&:|.c......x
+00003b40: 3c0e 3aa7 89c3 6c6b 0a9a 34d1 e11b 9daf  <.:...lk..4.....
+00003b50: ac80 9390 3b3c 0e3a a789 c3a0 eb1d 341d  ....;<.:......4.
+00003b60: 10af 0edf e8e0 21e2 24e4 eef7 71d0 394d  ......!.$...q.9M
+00003b70: 1c46 5c53 d0a4 890e dfe8 445e 059c 06a2  .F\S......D^....
+00003b80: c3e3 a073 9a38 4cb2 a6a0 4913 1dbe a16d  ...s.8L...I....m
+00003b90: ff59 01a7 7d53 87c7 41e7 3471 9861 4d41  .Y..}S..A.4q.aMA
+00003ba0: 9326 3a7c c353 4516 f4fc fb0d 4de2 ede9  .&:|.SE.....M...
+00003bb0: f168 df34 67b3 5507 7d0a 9a24 d1e1 1b1e  .h.4g.U.}..$....
+00003bc0: 1eb2 a09d 24a2 7fba 05fd e84d 62ce 4eab  ....$......Mb.N.
+00003bd0: 0efa 1434 49a2 c337 3a30 e37f bf91 afa1  ...4I..7:0......
+00003be0: c7e3 ee91 93c4 e165 3505 4d92 e8f0 8d4e  .......e5.M....N
+00003bf0: 9254 c079 203e 52c4 9c49 561d f429 6852  .T.y >R..IV..)hR
+00003c00: 4487 6f74 c4c2 ff7e 9b2e e5fd 25c0 cbe3  D.ot...~....%...
+00003c10: e195 bebd a69e 2be2 a07f 0f9a be50 541d  ......+......PT.
+00003c20: dce8 b371 88c3 c3c7 629e 9b8f 63ce 09e2  ...q....b...c...
+00003c30: 30a0 9a2e 34a9 b8c3 373a 2f51 01a7 972e  0...4...7:/Q....
+00003c40: 0e8f 83ce 09e2 f099 9a82 2615 77f8 4607  ..........&.w.F.
+00003c50: 092a e0a4 e20e 8f83 ce09 e2b0 937a 074d  .*...........z.M
+00003c60: e590 d5e1 1b55 d823 4e2a ee7e 1f07 9d13  .....U.#N*.~....
+00003c70: c4e1 1a35 054d 2aee f08d 4acf 2be0 f4f0  ...5.M*...J.+...
+00003c80: 7078 1c74 4e10 8739 d414 34a9 b8c3 372a  px.tN..9..4...7*
+00003c90: c9ae 8093 8a3b 3c0e 3ab7 461c 1e50 53d0  .....;<.:.F..PS.
+00003ca0: a4e2 0edf a856 b902 ce03 f191 20de 3e50  .....V...... .>P
+00003cb0: 8927 de2c 88b6 5ce2 4b0d 04ac 4fae e30f  .'.,..\.K...O...
+00003cc0: be9f 991f e452 e009 f1c5 ce69 e230 759a  .....R.....i.0u.
+00003cd0: 2e36 cd3e 1cbe 51bd 6905 9c1f 208f 3431  .6.>..Q.i... .41
+00003ce0: e716 5507 7d0a 9a66 1f0e dfe8 0bf7 fef7  ..U.}..f........
+00003cf0: 1b7d f7da e3e1 95be fd9b 9ef7 9041 9f82  .}...........A..
+00003d00: a6d9 87c3 372e dd04 9c1e 200e 8f83 ce89  ....7..... .....
+00003d10: e270 629a 82a6 d987 c337 2edd 049c 1e20  .pb......7..... 
+00003d20: 0e8f 83ce 89e2 305c 9a47 12f7 0f20 a091  ......0\.G... ..
+00003d30: 60c5 16a8 5b3b 421c 774e 1787 b5d2 74b1  `...[;B.wN....t.
+00003d40: 6906 e2f0 8d4b 4e01 a707 9fc3 e3a0 73ba  i....KN.......s.
+00003d50: 381c 94a6 a069 06e2 f08d 4b4e 01e7 2b3d  8....i....KN..+=
+00003d60: b71f 079d d3c5 6194 34f7 10be d440 40ab  ......a.4....@@.
+00003d70: e90a 2df0 a69e 23c4 71e7 a471 5822 4d71  ..-...#.q..qX"Mq
+00003d80: d3c7 7f2b 12d0 4286 083c 221f a963 ce6e  ...+..B..<"..c.n
+00003d90: a90e fabb 93d0 8964 8f6f 5ce2 eb7e bfd1  .......d.o\..~..
+00003da0: 312a fffb f862 e7a4 7178 1c4d 41d3 8ccf  1*...b..qx.MA...
+00003db0: e11b 57cb 02ce 0fec 47d2 9833 4faa 833e  ..W.....G..3O..>
+00003dc0: f710 1274 24e0 6123 6a81 4a29 5c0b e1c5  ...t$.a#j.J)\...
+00003dd0: ced9 24d5 419f e326 a541 021a 8c52 0bb4  ..$.A..&.A...R..
+00003de0: 2c70 2dc4 71e7 0472 d813 4d9d 84a6 7d0e  ,p-.q..r..M...}.
+00003df0: dfb8 3a19 701a 8e0e 8f83 ce09 e470 229a  ..:.p........p".
+00003e00: 82a6 19b6 c337 ae4e 069c 84c6 e171 d039  .....7.N.....q.9
+00003e10: 751c a643 530f e103 3b48 8001 7756 24d0  u..CS...;H..wV$.
+00003e20: be82 23c4 71e7 0472 d80b 4d17 9b07 a47b  ..#.q..r..M....{
+00003e30: 7bc8 55d5 eef7 e503 7db4 aeea 0871 d439  {.U.....}....q.9
+00003e40: 851c 3642 efab 4dfa e8e0 461f 31af 80f3  ..6B..M...F.1...
+00003e50: 33e4 d14e ea6d fff3 7c86 3de8 ef98 6926  3..N.m..|.=...i&
+00003e60: e2e0 4647 152b e054 8de5 f1f7 a071 e7fd  ..FG.+.T.....q..
+00003e70: ea6d f293 88d9 2923 9ece bd5b fb9e 52a3  .m....)#...[..R.
+00003e80: 0f5f 034e 5f22 043c 8c39 278c c3f9 e7dd  ._.N_".<.9'.....
+00003e90: a349 171d dce8 93d0 1570 1e85 8f74 31e7  .I.......p...t1.
+00003ea0: 2854 07fd 1d33 3df1 1cdc e893 bcfe e78d  (T...3=.........
+00003eb0: bec4 0578 749d 6f8b 9fe7 7d63 d0a7 2707  ...xt.o...}c..'.
+00003ec0: 2d63 1cbe 7187 069c 3ab4 c3c3 0747 ce1e  -c..q...:....G..
+00003ed0: a80e fa7b 1092 8c3b b8a1 f1ee e97f dee8  ...{...;........
+00003ee0: 13ce 8087 173a a787 c392 67ba d0b4 3477  .....:....g...4w
+00003ef0: f8c6 a3d0 e33c 0a1d 1e5f e89c 1e0e e79d  .....<..._......
+00003f00: 2968 bed2 ae94 8687 a1fb fd46 5f97 ac0e  )h.........F_...
+00003f10: 8f83 ce89 e130 d899 8226 5d71 f846 1f2d  .....0...&]q.F.-
+00003f20: af80 e321 7e8f c741 e7b4 70f8 e84c 4193  ...!~..A..p..LA.
+00003f30: b038 7c13 0f0f f75a 513c 3c1e 89e1 ed7f  .8|....ZQ<<.....
+00003f40: 9378 78b8 5d54 f27d a8a3 b9ef 496d f4a9  .xx.]T.}....Im..
+00003f50: 6bc4 f9e1 f168 9d78 dbdc 2482 766a 8865  k....h.x..$.vj.e
+00003f60: bcaf 3a9a 9b82 a655 b9c7 f964 83c3 e3ee  ..:....U...d....
+00003f70: 9193 c361 91f3 ee1e 58c6 6b41 cff8 c627  ...a....X.kA...'
+00003f80: 1b00 273d 7478 1874 ce55 a70e fa14 3409  ..'=tx.t.U....4.
+00003f90: a2c3 373e d900 380d 4487 c741 e78a 4f87  ..7>..8.D..A..O.
+00003fa0: dfcd 1434 4da5 1dbe f121 01c0 6956 eaf0  ...4M....!..iV..
+00003fb0: 38e8 dc0a 7118 d64c 4193 8a3b 7ce3 4302  8...q..LA..;|.C.
+00003fc0: 80d3 4074 781c 744e 1187 2fcd 1434 29a2  ..@tx.tN../..4).
+00003fd0: c337 3e24 e071 3e24 e0f0 38e8 9c22 0e93  .7>$.q>$..8.."..
+00003fe0: 9a29 6852 4487 6f7c 4800 701a 880e 8f83  .)hRD.o|H.p.....
+00003ff0: ce29 a2b3 a5a9 587b fcaa 0edf b8de 1e70  .)....X{.......p
+00004000: 1e88 8ff6 4f73 8636 d519 d254 2c3d b7a0  ....Os.6...T,=..
+00004010: 9de2 71e9 3ae0 3c10 1f29 e2ed 1df3 5c5c  ..q.:.<..)....\\
+00004020: 9c15 4dc3 8257 0bda 2922 9e5c 3811 e781  ..M..W..)".\8...
+00004030: f848 1187 6bcc b744 d0b3 e235 acc2 b4a0  .H..k..D...5....
+00004040: 9d22 e29d b0a0 677c e72a df47 2636 7687  ."....g|.*.G&6v.
+00004050: 7341 bb15 1cbf 0b75 2634 3b26 6541 cfbf  sA.....u&4;&eA..
+00004060: dfc9 4bdf e3d1 40b4 3b9c 09fa a67f 7f7a  ..K...@.;......z
+00004070: 342c 3d7f 797c 47fc 441c 0722 b41f ac5c  4,=.y|G.D.."...\
+00004080: ec0e e782 7695 30f8 ced8 829e f11d 4bd3  ....v.0.......K.
+00004090: 2d68 8fe3 40f4 787c a553 8ad8 9c89 4dc3  -h..@.x|.S....M.
+000040a0: a02c e859 3177 2a02 471c 0722 b41f 5ee9  .,.Y1w*.G.."..^.
+000040b0: 9422 5a87 98c4 a561 3dbd 053d e33b 1581  ."Z....a=..=.;..
+000040c0: 034e ef8b a0fd 30e8 9422 3667 62d3 f04a  .N....0.."6gb..J
+000040d0: 5ad0 b362 ee54 048e 382a 22b4 1f06 9d52  Z..b.T..8*"....R
+000040e0: 44eb 10ee 4ae3 1ad1 e33b d678 5b9f 9e7f  D...J....;.x[...
+000040f0: bf93 1f22 b41f 069d 5a23 5a87 7041 e31a  ..."....Z#Z.pA..
+00004100: d1e3 3b7d 7c07 711e 884f 14d1 ee70 eee9  ..;}|.q..O...p..
+00004110: e114 0bfb a475 8f19 dfe9 ab34 88f3 407c  .....u.....4..@|
+00004120: a288 6db8 d23c 57c4 9bfe 7e4e d32b 508f  ..m..<W...~N.+P.
+00004130: eff4 b916 c0f1 35c2 05ed 87dd 23a5 88cd  ......5.....#...
+00004140: 99d8 343c b760 57da 291e 7dc7 0471 1e88  ..4<.`W.).}..q..
+00004150: 4ff6 4c5b cec4 e6a6 4f57 1ad7 881e dfe9  O.L[....OW......
+00004160: 031f 8893 223e 32b1 69c3 3526 d13d bcc9  ....">2.i.5&.=..
+00004170: 0c8e fed7 dddc f7a4 76ac f13e 11a7 81f8  ........v..>....
+00004180: c8c4 c6ee 702e e859 f11a 3e1d 2c68 a788  ....p..Y..>.,h..
+00004190: 58e3 6d41 7b9c 06a2 c343 191f ae31 992b  X.mA{....C...1.+
+000041a0: ed14 91aa 7c9b 33a1 d9e9 3303 8093 0baf  ....|.3...3.....
+000041b0: c7e3 a073 8ae8 4d66 c814 b239 7c27 ff7d  ...s..Mf...9|'.}
+000041c0: c469 203e 32b1 b13b 9cbb d24e 11f1 588b  .i >2..;...N..X.
+000041d0: 750f a778 d3a5 ba6b bcad 7b78 9c07 e293  u..x...k..{x....
+000041e0: 3562 1bae 3299 eee1 140b 9fc3 16f4 8cef  5b..2...........
+000041f0: e4d8 8e38 0fc4 478a 385c 6532 413b c5a2  ...8..G.8\e2A;..
+00004200: 77cc cd99 d4ec 6465 8e38 0fc4 478a 385c  w.....de.8..G.8\
+00004210: 6532 41bb 3522 8a87 5d69 b706 248f 6fc0  e2A.5"..]i..$.o.
+00004220: b174 f9f2 783c 1073 8ae8 4c68 1a1e 20b2  .t..x<.s..Lh.. .
+00004230: a09d 2292 f735 e23c 101f 2962 cec4 a639  .."..5.<..)b...9
+00004240: 939a 868a f7f2 f84e a6d0 88d3 40f4 ed47  .......N....@..G
+00004250: 738f e12a 93e8 1ece 84a6 d1b7 949a c377  s..*...........w
+00004260: f2c1 459c 06a2 6f3f 0c3a a788 ce84 a6a1  ..E...o?.:......
+00004270: 4cdb 9576 8a47 96b2 88d3 40f4 ed87 41e7  L..v.G....@...A.
+00004280: 14d1 99d4 34fa ce93 7598 6991 b093 a52c  ....4...u.i....,
+00004290: e058 027c 793c 1c88 c335 26d3 3de6 3560  .X.|y<...5&.=.5`
+000042a0: c3b9 855d 69b7 46c4 4fda 9f88 d340 7c64  ...]i.F.O....@|d
+000042b0: 6263 7738 17f4 ac58 e48d 70b7 f69e e4e1  bcw8...X..p.....
+000042c0: 77a5 2c66 2788 f4a5 268f c717 3a27 88ce  w.,f'...&...:'..
+000042d0: 83a6 e199 38bb d04e 10f1 834b 16b4 c779  ....8..N...K...y
+000042e0: 1c3e 12c4 612a 93e9 1d5e 1069 5deb 3c6a  .>..a*...^.i].<j
+000042f0: 76fc 0689 05ed 9690 f455 0f8f c757 3a27  v........U...W:'
+00004300: 88ce 83a6 91bd a25d fb79 1c62 39a9 05ed  .......].y.b9...
+00004310: 70fa 629c c7e3 a073 82e8 3c68 1ace 3cad  p.b....s..<h..<.
+00004320: 7b38 41a4 4373 88f3 387c 2488 390f 1bbb  {8A.Cs..8|$.9...
+00004330: b6f3 2b17 7c21 e7e1 462f 9911 a7a7 b46b  ..+.|!..F/.....k
+00004340: 3ebc d0c3 3326 d1a5 bd85 0dbe 8fb3 2b3f  >...3&........+?
+00004350: efe4 907b 1ee0 f48e 19f0 4859 8665 4c26  ...{......HY.eL&
+00004360: 66f7 1211 5fc7 356f 4043 af98 11a7 bef1  f..._.5o@C......
+00004370: c8c0 a60d c798 4ccc ee1d 22be 8dbb 5b7b  ......L..."...[{
+00004380: ef2e d01b 66c4 69ae f4c8 bfa6 0d43 994c  ....f.i......C.L
+00004390: cc4e 0cf1 34ed eb6e ee2d 2c54 be84 3807  .N..4..n.-,T..8.
+000043a0: eddb fffe 310e 5743 d886 a14c 2668 bf7c  ....1.WC...L&h.|
+000043b0: a37d 1ae7 4fb3 53b1 e6fd e7a6 a448 58dc  .}..O.S......HX.
+000043c0: efe3 5198 5343 ef5f 439b bc0e 6ef4 2abf  ..Q.SC._C...n.*.
+000043d0: 01ce 313f 12c3 6127 93b9 d0be a606 3ea5  ..1?..a'......>.
+000043e0: d29c 394d a337 f988 f3d3 eed1 e270 b8c9  ..9M.7.......p..
+000043f0: 6462 f62f 1029 6607 d38b fce6 bc6b 1abd  db./.)f......k..
+00004400: c807 3c7c dae5 a4d0 79cf b012 7a98 dee3  ..<|....y...z...
+00004410: 37c0 f969 f748 0973 ce35 cd39 d3f0 83c3  7..i.H.s.5.9....
+00004420: c3f4 1a1f 7e4e a69b 8047 d739 675c d39c  ....~N...G.9g\..
+00004430: 318d 3dbb b073 387c a702 53ff fb1d 6daa  1.=..s8|..S...m.
+00004440: 2f6c 3f78 da0d a798 4487 0663 19d2 6f87  /l?x....D..c..o.
+00004450: ef54 acd9 3c4e c59a 1e0f 9f76 c329 2613  .T..<N.....v.)&.
+00004460: b4db 2bc5 73f8 afe6 8c67 762a d644 9cba  ..+.s....gv*.D..
+00004470: f423 e39a 369c 6232 417b b122 0577 c633  .#..6.b2A{.".w.3
+00004480: 3b15 6bde 7fee ad2b 6853 6ddd e391 180e  ;.k....+hSm.....
+00004490: a798 4cd0 5e0c 4958 9cf1 cc4e c59a 0d70  ..L.^.IX...N...p
+000044a0: 1296 47c6 356d 38c5 6482 f66a 45ab 2c67  ..G.5m8.d..jE.,g
+000044b0: 3cb3 f33c 1a70 5296 47c6 352d 675c 73d3  <..<.pR.G.5-g\s.
+000044c0: df13 38b2 ecf5 f8ce 1369 674c b3f3 44fa  ..8......igL..D.
+000044d0: 9171 4dcb 19d7 dcf4 2968 3cbc e0f1 9d67  .qM.....)h<....g
+000044e0: d2ce d866 271b 6a68 3f7c 4ee7 f4d0 19cf  ...f'.jh?|N.....
+000044f0: d803 8a9e d36e 69c8 5369 f7fb 9d3e 0ad5  .....ni.Si...>..
+00004500: 7cfb 51d0 39e3 9ae6 8c69 ec01 8641 3b7c  |.Q.9....i...A;|
+00004510: e719 9ec3 0f3c 5a7e 41fb 61d0 b9b5 a177  .....<Z~A.a....w
+00004520: 9641 6f89 5773 f88e 9fa1 3c11 c7d3 cc1e  .Ao.Ws....<.....
+00004530: 0fc5 6558 c524 9e1e de59 0637 702d 68b7  ..eX.$...Y.7p-h.
+00004540: 578a 9f67 b4a0 3d8e 0727 3d1e 079d 5344  W..g..=..'=...SD
+00004550: ef2c 83c6 1216 b4db 2ba5 ef76 208e a76b  .,......+..v ..k
+00004560: 3d1e 079d 5344 ef2c 83bb ce16 b4db 2b25  =...SD.,......+%
+00004570: 4767 c461 4c58 9f7e a488 c32a 26d3 3d9c  Gg.aLX.~...*&.=.
+00004580: 22a2 1b86 05ed 3643 c91c 1971 3ced e9f1  ".....6C...q<...
+00004590: f84a e714 d13b cbe0 56b9 05ed 3643 c967  .J...;..V...6C.g
+000045a0: 1871 1e88 8fd6 87c3 4a26 73a5 dd02 8eb7  .q......J&s.....
+000045b0: a59d 33cd 4e3e c30d 701e 888f 1688 39e7  ..3.N>..p.....9.
+000045c0: 9ae6 7c67 ec01 45cf e979 85d8 c967 d8ff  ..|g..E..y...g..
+000045d0: be93 4f28 b41f 3ea7 738a e86c 67ec 0145  ..O(..>.s..lg..E
+000045e0: 41cf 8ad8 c967 b8b9 df77 f219 f678 d8a7  A....g...w...x..
+000045f0: 73b6 35cd d9d2 d803 0a83 7678 279f 61ff  s.5.......vx'.a.
+00004600: fb4e 3ec3 d07e 74a5 73b6 35e6 ce36 6f87  .N>..~t.s.5..6o.
+00004610: e2ab 9297 c73b f90c 234e 03f1 916d 4d1b  .....;..#N...mM.
+00004620: 3e31 8981 e86d 65f0 558a 053d 2b5e 471b  >1...me.U..=+^G.
+00004630: e113 711a 888f 6c6b ec74 632e 68b7 4644  ..q...lk.tc.h.FD
+00004640: a714 0b7a c63b 56eb 59d0 1e27 457c e459  ...z.;V.Y..'E|.Y
+00004650: 6347 2e73 41cf 8ac5 6ff1 bde5 0c2f 1101  cG.sA...o..../..
+00004660: a7fd d247 9635 76fe 3c17 b313 447c 6765  ...G.5v.<...D|ge
+00004670: 177a c63b 990c 234e 2aee 7e1f 3f3c 7282  .z.;..#N*.~.?<r.
+00004680: e8fd 64f0 459a 053d 0b5a 2793 61c4 49c5  ..d.E..=.Z'.a.I.
+00004690: 7fec 57f3 d3b7 7ffc fefb 1fd7 af7f fcfa  ..W.............
+000046a0: f5ff 0000 00ff ff00 0000 ffff 4c90 6f4b  ............L.oK
+000046b0: 0331 0cc6 bf4a c8fb b92b c389 c73a 1087  .1...J...+...:..
+000046c0: b017 82b0 4f50 bddc b578 3625 97f3 cfc4  ....OP...x6%....
+000046d0: ef6e 3a1d 9a17 699f d0e6 f925 9b30 2bdf  .n:...i....%.0+.
+000046e0: a551 4940 a8f7 78e3 dadd 6abd 4678 9776  .QI@..x...j.Fx.v
+000046f0: 4e9d c7cf e637 1676 ba9a 9a45 e36a fa17  N....7.v...E.j..
+00004700: 5fb8 dc6e 4ae4 4c9a 9e1e 047a ceba b7cf  _..nJ.L....z....
+00004710: 0e41 3f0a 79cc 7ccb f995 644a 9c4f 6fc3  .A?.y.|...dJ.Oo.
+00004720: 40f7 4186 9427 18a9 578f cdc5 1582 a421  @.A..'..W......!
+00004730: 9eef cae5 54bd 4478 6455 7e39 ab48 a123  ....T.DxdU~9.H.#
+00004740: a96a 85e6 c4c6 fe23 2a83 f53d 90ce 054a  .j.....#*..=...J
+00004750: 2824 8774 34f3 6b04 9644 5983 9abd c7c2  ($.t4.k..DY.....
+00004760: a212 9222 44ab 1f8d 358c bb92 ac09 8231  ..."D...5......1
+00004770: da08 7f5a daba 04d9 77ae 622f df58 9ea7  ...Z....w.b/.X..
+00004780: 48a4 db6f 0000 00ff ff03 0050 4b03 0414  H..o.......PK...
+00004790: 0006 0008 0000 0021 0011 d781 143c 0300  .......!.....<..
+000047a0: 0029 0800 0018 0000 0078 6c2f 776f 726b  .).......xl/work
+000047b0: 7368 6565 7473 2f73 6865 6574 332e 786d  sheets/sheet3.xm
+000047c0: 6c9c 934b 6fa3 3010 c7ef 95f6 3b58 be07  l..Ko.0.....;X..
+000047d0: 0369 a216 8554 dd56 d1f6 b65a f571 76cc  .i...T.V...Z.qv.
+000047e0: 10ac f841 6d93 8756 fbdd 77ec 3469 a55c  ...Am..V..w.4i.\
+000047f0: a222 f00c 8cfd 9b19 fcf7 ec6e a715 d980  .".........n....
+00004800: f3d2 9a9a 1659 4e09 1861 1b69 5635 7d79  .....YN..a.iV5}y
+00004810: 5e8c 6e28 f181 9b86 2b6b a0a6 7bf0 f46e  ^.n(....+k..{..n
+00004820: fee3 6ab6 b56e ed3b 8040 9060 7c4d bb10  ..j..n.;.@.`|M..
+00004830: fa8a 312f 3ad0 dc67 b607 8391 d63a cd03  ..1/:..g.....:..
+00004840: beba 15f3 bd03 dea4 455a b132 cfa7 4c73  ........EZ.2..Ls
+00004850: 69e8 8150 b94b 18b6 6da5 8047 2b06 0d26  i..P.K..m..G+..&
+00004860: 1c20 0e14 0f58 bfef 64ef 8f34 2d2e c169  . ...X..d..4-..i
+00004870: eed6 433f 1256 f788 584a 25c3 3e41 29d1  ..C?.V..XJ%.>A).
+00004880: a27a 5a19 ebf8 5261 dfbb e29a 0bb2 7378  .zZ...Ra......sx
+00004890: 97f8 8c8f 69d2 f7b3 4c5a 0a67 bd6d 4386  ....i...LZ.g.mC.
+000048a0: 6476 a8f9 bcfd 5b76 cbb8 3891 cefb bf08  dv....[v..8.....
+000048b0: 535c 3307 1b19 37f0 1355 7eaf a462 7262  S\3...7..U~..brb
+000048c0: 959f b0f1 3761 d313 2cfe 2e57 0db2 a9e9  ....7a..,..W....
+000048d0: dffc e31a a12d e290 8f72 d442 f28e b17f  .....-...r.B....
+000048e0: 743e 6b24 ee70 ec8a 3868 6b7a 5f54 3f6f  t>k$.p..8hkz_T?o
+000048f0: 289b cf92 7e5e 256c fd17 9f44 392e ad5d  (...~^%l...D9..]
+00004900: c7c0 13a6 c991 e041 8188 c220 1ccd 061e  .......A... ....
+00004910: 4029 0461 31fe fdc0 1c47 203b 11bf fa47  @).a1....G ;...G
+00004920: fa22 09f8 b723 0db4 7c50 e18f ddfe 02b9  ."...#..|P......
+00004930: ea02 9e96 6936 c1c6 a232 aa66 ff08 5ea0  ....i6...2.f..^.
+00004940: 2431 7556 4e22 5758 8510 1c89 96f1 6ca1  $1uVN"WX......l.
+00004950: a4f8 2ed9 ad6c 4297 d617 3895 2cc1 8785  .....lB...8.,...
+00004960: 8c40 4ac4 e083 d56f 1f13 5279 89f3 1f00  .@J....o..Ry....
+00004970: 00ff ff00 0000 ffff 94d3 d10e 8220 1406  ............. ..
+00004980: e057 713c 4078 5054 1ab2 e57c 1146 6e5d  .Wq<@xPT...|.Fn]
+00004990: 5913 67f5 f69d 5a03 24dd e24e fdff f979  Y.g...Z.$..N...y
+000049a0: 7650 dacb 30cc bd9e b592 d3f5 9e4d 2d01  vP..0........M-.
+000049b0: 92d9 9b1e 2d5e 1d19 c91e 506a 733c 3ffb  ....-^....Pjs<?.
+000049c0: c19a 619c 5b92 1f18 274a 9a77 f784 657c  ..a.[...'J.w..e|
+000049d0: 64f1 7e51 201a 4917 25a9 f9a6 5d98 b2bc  d.~Q .I.%...]...
+000049e0: 7629 45ca 7968 fcef 61d9 79fe 7d9f 6fe9  v)E.yh..a.y.}.o.
+000049f0: c20c 04db d68a 140d cb4e 2b8a 68b8 3064  .........N+.h.0d
+00004a00: 506d 7365 0a87 65cf 9511 1786 2060 9be3  Pmse..e..... `..
+00004a10: 291c 961d c7e3 d585 2108 3ffb 6a75 550a  ).......!.?.juU.
+00004a20: 8765 c789 3c9a 2e0c 77a7 ab53 382c fb93  .e..<...w..S8,..
+00004a30: c963 6f95 ee8d d7a4 7858 f65e 1d1f 9655  .co.....xX.^...U
+00004a40: fab3 3dea ffc2 1700 0000 ffff 0000 00ff  ..=.............
+00004a50: ff44 8fcd 0e01 510c 855f a5e9 03f8 8988  .D....Q.._......
+00004a60: 1063 c366 1612 8927 b84c cd6d 70db 748a  .c.f...'.L.mp.t.
+00004a70: f0f4 4a4c ecce 7716 e767 a959 0a39 1f77  ..JL..w..g.Y.9.w
+00004a80: 0627 295e 3715 8e11 fca9 5461 91b5 943b  .')^7.....Ta...;
+00004a90: 59c7 5270 b85a 6a6a 699b ace5 d2c1 854e  Y.Rp.Zjji......N
+00004aa0: 5ee1 6830 4330 6e73 af5d f4eb 4e11 0ee2  ^.h0C0ns.]..N...
+00004ab0: 2ed7 9e32 a586 ec43 138c 26f1 1e7e b97b  ...2...C..&..~.{
+00004ac0: f29b 8226 25db f32b cae7 0862 4cc5 9347  ...&%..+...bL..G
+00004ad0: 7d85 2ae6 96d8 1172 f8af d89a 2e1b e548  }.*....r.......H
+00004ae0: 4488 8d71 e1cf b6e0 f861 7533 fecc 1e3e  D..q.....au3...>
+00004af0: c4ce 5d26 f2d5 1b00 00ff ff03 0050 4b03  ..]&.........PK.
+00004b00: 0414 0006 0008 0000 0021 0051 0823 677f  .........!.Q.#g.
+00004b10: 0300 0099 0900 0018 0000 0078 6c2f 776f  ...........xl/wo
+00004b20: 726b 7368 6565 7473 2f73 6865 6574 342e  rksheets/sheet4.
+00004b30: 786d 6c9c 934b 8fdb 2010 c7ef 95fa 1d10  xml..K.. .......
+00004b40: f718 dbd9 a41b 2bce aadd 55d4 bd55 d5b6  ......+...U..U..
+00004b50: 3d13 3c8e 5178 b840 5eaa fadd 3b90 a794  =.<.Qx.@^...;...
+00004b60: 43a3 4536 830d f39b f9c3 307d da69 4536  C.E6......0}.iE6
+00004b70: e0bc b4a6 a645 9653 0246 d846 9a65 4d7f  .....E.S.F.F.eM.
+00004b80: bccd 078f 94f8 c04d c395 3550 d33d 78fa  .......M..5P.=x.
+00004b90: 34fb f861 bab5 6ee5 3b80 4090 607c 4dbb  4..a..n.;.@.`|M.
+00004ba0: 10fa 8a31 2f3a d0dc 67b6 0783 33ad 759a  ...1/:..g...3.u.
+00004bb0: 07fc 744b e67b 07bc 494e 5ab1 32cf c74c  ..tK.{..INZ.2..L
+00004bc0: 7369 e881 50b9 7b18 b66d a580 172b d61a  si..P.{..m...+..
+00004bd0: 4c38 401c 281e 307f dfc9 de9f 685a dc83  L8@.(.0.....hZ..
+00004be0: d3dc add6 fd40 58dd 2362 2195 0cfb 04a5  .....@X.#b!.....
+00004bf0: 448b ea75 69ac e30b 85ba 77c5 0317 64e7  D..ui.....w...d.
+00004c00: f029 f11d 9ec2 a4ff 3791 b414 ce7a db86  .)......7....z..
+00004c10: 0cc9 ec90 f3ad fc09 9b30 2ece a45b fd77  .........0...[.w
+00004c20: 618a 07e6 6023 e301 5e50 e5fb 522a 4667  a...`#..^P..R*Fg
+00004c30: 5679 810d df09 1b9f 6171 bb5c b596 4d4d  Vy......aq.\..MM
+00004c40: ffe4 c736 405b c42e 1fe4 c3d8 5db5 bf74  ...6@[......]..t
+00004c50: 366d 249e 7054 451c b435 fd5c 54cf 8f94  6m$.pTE..5.\T...
+00004c60: cda6 a97e 7e4a d8fa ab31 89e5 b8b0 7615  ...~~J...1....v.
+00004c70: 275e 314c 8e04 0f0a 442c 0cc2 d16c e019  '^1L....D,...l..
+00004c80: 94aa e917 4cc6 ff4e 4c1c 2290 9d89 d7e3  ....L..NL.".....
+00004c90: 137d 9e0a f89b 230d b47c adc2 77bb fd0a  .}....#..|..w...
+00004ca0: 72d9 05bc 2de3 6c84 c262 6554 cdfe 05bc  r...-.l..beT....
+00004cb0: c092 c4d0 5939 8a5c 6115 42b0 275a c6bb  ....Y9.\a.B.'Z..
+00004cc0: 8525 c577 c96e 6513 bae4 5fe0 52b2 001f  .%.w.ne..._.R...
+00004cd0: e632 0229 116b 1fac fe75 5c70 c41c 0078  .2.).k...u\p...x
+00004ce0: 2209 80f6 0498 c450 f7fa a3ee e48f f692  "......P........
+00004cf0: c0a7 fffa b3a4 e31f 0000 00ff ff00 0000  ................
+00004d00: ffff 94d4 516e c230 0cc6 f1ab 5439 c06a  ....Qn.0....T9.j
+00004d10: bb0d a528 541a e522 5557 694f 6c22 5581  ...(T.."UWiOl"U.
+00004d20: dbe3 0914 c77e 5ade 80ff 87f4 531a 08f1  .....~Z.....S...
+00004d30: 7b59 d6f3 b44e 43b8 fedc aaeb d1a1 abe2  {Y...NC.........
+00004d40: ef74 89fc ead0 b8ea 8eed 341f be1e e725  .t........4....%
+00004d50: cecb 653d 3af8 20ef 8630 ff6d 3f79 cc1f  ..e=:. ..0.m?y..
+00004d60: 457e bf0d d8ef 43bd 0da1 9edf f5a4 6baf  E~....C.......k.
+00004d70: eb98 5702 f96e cd90 a4a1 120d 8f93 a633  ..W..n.........3
+00004d80: 96bc 1180 b1e8 2a52 65e1 d3f8 ffc9 f038  ......*Re......8
+00004d90: 599a c660 f248 8006 a32a 0a55 61da 120c  Y..`.H...*.Ua...
+00004da0: 8f05 d31a 4c1e 09c8 6054 45a1 2a8c 2fc1  ....L...`TE.*./.
+00004db0: f038 61bc bd32 7924 30e7 36aa 8a42 5598  .8a..2y$0.6..BU.
+00004dc0: 5d09 86c7 09d3 9b5b 71ca 2381 39b7 5155  ]......[q.#.9.QU
+00004dd0: 14aa c274 2518 1ecb afc9 5b4d 5e09 bc79  ...t%.....[M^..y
+00004de0: 4eaa a258 9566 5fa2 e1b1 683a 7b85 f34a  N..X.f_...h:{..J
+00004df0: b033 1a55 51ac 2f4d 2dff 3a4f 0000 00ff  .3.UQ./M-.:O....
+00004e00: ff00 0000 ffff 448f cd0e 0151 0c85 5fa5  ......D....Q.._.
+00004e10: e903 f889 8810 63c3 6616 1289 27b8 4ccd  ......c.f...'.L.
+00004e20: 6d70 db74 8af0 f44a 4cec ce77 16e7 67a9  mp.t...JL..w..g.
+00004e30: 590a 391f 7706 2729 5e37 158e 11fc a954  Y.9.w.')^7.....T
+00004e40: 6191 b594 3b59 c752 70b8 5a6a 6a69 9bac  a...;Y.Rp.Zjji..
+00004e50: e5d2 c185 4e5e e168 3043 306e 73af 5df4  ....N^.h0C0ns.].
+00004e60: eb4e 110e e22e d79e 32a5 86ec 4313 8c26  .N......2...C..&
+00004e70: f11e 7eb9 7bf2 9b82 2625 dbf3 2bca e708  ..~.{...&%..+...
+00004e80: 624c c593 477d 852a e696 d811 72f8 afd8  bL..G}.*....r...
+00004e90: 9a2e 1be5 4844 888d 71e1 cfb6 e0f8 6175  ....HD..q.....au
+00004ea0: 33fe cc1e 3ec4 ce5d 26f2 d51b 0000 ffff  3...>..]&.......
+00004eb0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00004ec0: 474b 9f37 4203 0000 3208 0000 1800 0000  GK.7B...2.......
+00004ed0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00004ee0: 6565 7435 2e78 6d6c 9c93 4b8f 9b30 10c7  eet5.xml..K..0..
+00004ef0: ef95 fa1d 2cdf 8381 9074 8342 566d 5751  ....,....t.BVmWQ
+00004f00: b7a7 6ad5 c7d9 3143 b0e2 07b5 4d1e aafa  ..j...1C....M...
+00004f10: dd3b 268f 8d94 43a3 b5c0 3360 fc9b 19e6  .;&...C...3`....
+00004f20: eff9 e35e 2bb2 05e7 a535 15cd 9294 1230  ...^+....5.....0
+00004f30: c2d6 d2ac 2bfa e3fb 72f4 4089 0fdc d45c  ....+...r.@....\
+00004f40: 5903 153d 80a7 8f8b f7ef e63b eb36 be05  Y..=.......;.6..
+00004f50: 0804 09c6 57b4 0da1 2b19 f3a2 05cd 7d62  ....W...+.....}b
+00004f60: 3b30 b8d2 58a7 79c0 47b7 66be 73c0 eb61  ;0..X.y.G.f.s..a
+00004f70: 9356 2c4f d329 d35c 1a7a 2494 ee1e 866d  .V,O.).\.z$....m
+00004f80: 1a29 e0c9 8a5e 8309 4788 03c5 03e6 ef5b  .)...^..G......[
+00004f90: d9f9 334d 8b7b 709a bb4d df8d 84d5 1d22  ..3M.{p..M....."
+00004fa0: 5652 c970 18a0 9468 513e af8d 757c a5b0  VR.p...hQ>..u|..
+00004fb0: ee7d 5670 41f6 0eaf 1cef f139 ccf0 fe26  .}VpA......9...&
+00004fc0: 9296 c259 6f9b 9020 991d 73be 2d7f c666  ...Yo.. ..s.-..f
+00004fd0: 8c8b 0be9 b6fe bb30 59c1 1c6c 656c e02b  .......0Y..lel.+
+00004fe0: 2a7f 5b4a d9e4 c2ca 5f61 e337 c2a6 1758  *.[J...._a.7...X
+00004ff0: fc5d aeec 655d d13f e969 8cd0 6671 4a47  .]..e].?.i..fqJG
+00005000: 6911 a7ab f197 2ee6 b5c4 0ec7 aa88 83a6  i...............
+00005010: a21f b3f2 d303 658b f9a0 9f9f 1276 feca  ......e......v..
+00005020: 2751 8e2b 6b37 71e1 19c3 a448 f0a0 4044  'Q.+k7q....H..@D
+00005030: 6110 8e66 0b9f 41a9 8a7e cd66 28e9 df03  a..f..A..~.f(...
+00005040: 34fa 8864 17e6 b57f e62f 0709 7f73 a486  4..d...../...s..
+00005050: 86f7 2abc d8dd 1790 eb36 e079 9926 132c  ..*......6.y.&.,
+00005060: 2d6a a3ac 0f4f e005 8a12 8327 f924 7285  -j...O.....'.$r.
+00005070: 5508 c199 6819 4f17 8a8a ef07 bb93 7568  U...h.O.......uh
+00005080: d12b 92f1 0724 acc0 87a5 8c40 4a44 ef83  .+...$.....@JD..
+00005090: d5bf 4e1f 9c30 4700 f664 00a0 3d01 8a18  ..N..0G..d..=...
+000050a0: e93f dbd9 90c6 3f00 0000 ffff 0000 00ff  .?....?.........
+000050b0: ff94 d3ed 0a82 3014 06e0 5b91 5d40 d37d  ......0...[.]@.}
+000050c0: 388d 3928 bc91 b106 fdb2 7062 75f7 1d2b  8.9(......pbu..+
+000050d0: 363a 98b4 7fea 79e1 f13d 4e1d cede 4fbd  6:....y..=N...O.
+000050e0: 9dac d1e3 e556 8c1d a948 11ae 7608 70b5  .....V...H..v.p.
+000050f0: 67a4 b857 c2ba fde9 d1fb e0fc 3075 a4dc  g..W........0u..
+00005100: 3149 8c76 4bf6 0061 7814 e07e 3655 2b34  1I.vK..ax..~6U+4
+00005110: 9d8d a6ee 333d 7e4f 659c 52a0 a207 c6ff  ....3=~Oe.R.....
+00005120: 1e84 a3a7 90c6 5e6f c1d6 159e a340 382a  ......^o.....@8*
+00005130: 9c23 866f 3122 8781 7062 f0ee c47b a7eb  .#.o1"..pb...{..
+00005140: 6d64 0e03 e1c8 c806 b559 3ee5 6c7e 2cad  md.......Y>.l~,.
+00005150: ce61 201c 99b6 444c bdd5 46e5 3010 4e27  .a ...DL..F.0.N'
+00005160: 4e62 476d d569 721c 0827 47e1 43d0 acf6  NbGm.ir..'G.C...
+00005170: a1e9 6f7a 0200 00ff ff00 0000 ffff 448f  ..oz..........D.
+00005180: cd0e 0151 0c85 5fa5 e903 f889 8810 63c3  ...Q.._.......c.
+00005190: 6616 1289 27b8 4ccd 6d70 db74 8af0 f44a  f...'.L.mp.t...J
+000051a0: 4cec ce77 16e7 67a9 590a 391f 7706 2729  L..w..g.Y.9.w.')
+000051b0: 5e37 158e 11fc a954 6191 b594 3b59 c752  ^7.....Ta...;Y.R
+000051c0: 70b8 5a6a 6a69 9bac e5d2 c185 4e5e e168  p.Zjji......N^.h
+000051d0: 3043 306e 73af 5df4 eb4e 110e e22e d79e  0C0ns.]..N......
+000051e0: 32a5 86ec 4313 8c26 f11e 7eb9 7bf2 9b82  2...C..&..~.{...
+000051f0: 2625 dbf3 2bca e708 624c c593 477d 852a  &%..+...bL..G}.*
+00005200: e696 d811 72f8 afd8 9a2e 1be5 4844 888d  ....r.......HD..
+00005210: 71e1 cfb6 e0f8 6175 33fe cc1e 3ec4 ce5d  q.....au3...>..]
+00005220: 26f2 d51b 0000 ffff 0300 504b 0304 1400  &.........PK....
+00005230: 0600 0800 0000 2100 396a 59f5 ae02 0000  ......!.9jY.....
+00005240: 0806 0000 1800 0000 786c 2f77 6f72 6b73  ........xl/works
+00005250: 6865 6574 732f 7368 6565 7436 2e78 6d6c  heets/sheet6.xml
+00005260: 9c93 c94e c330 1086 ef48 bc83 e57b e324  ...N.0...H...{.$
+00005270: 5d44 a3a6 158b 10dc 1002 eeae 3369 ac7a  ]D..........3i.z
+00005280: 09b6 bb09 f1ee 8c53 5a2a f552 6139 f6c4  .......SZ*.Ra9..
+00005290: 56be 99df fe33 996d b522 6b70 5e5a 53d2  V....3.m."kp^ZS.
+000052a0: 2c49 2901 236c 25cd a2a4 ef6f 8fbd 1b4a  ,I).#l%....o...J
+000052b0: 7ce0 a6e2 ca1a 28e9 0e3c 9d4d afaf 261b  |.....(..<.M..&.
+000052c0: eb96 be01 0804 09c6 97b4 09a1 2d18 f3a2  ............-...
+000052d0: 01cd 7d62 5b30 b853 5ba7 79c0 57b7 60be  ..}b[0.S[.y.W.`.
+000052e0: 75c0 abee 23ad 589e a623 a6b9 3474 4f28  u...#.X..#..4tO(
+000052f0: dc25 0c5b d752 c083 152b 0d26 ec21 0e14  .%.[.R...+.&.!..
+00005300: 0f58 bf6f 64eb 0f34 2d2e c169 ee96 abb6  .X.od..4-..i....
+00005310: 27ac 6e11 3197 4a86 5d07 a544 8be2 7961  '.n.1.J.]..D..ya
+00005320: ace3 7385 bab7 d980 0bb2 75d8 737c fa87  ..s.......u.s|..
+00005330: 34dd fa59 262d 85b3 ded6 2141 32db d77c  4..Y&-....!A2..|
+00005340: 2e7f ccc6 8c8b 23e9 5cff 4598 6cc0 1cac  ......#.\.E.l...
+00005350: 65bc c03f 54fe bf92 b2e1 9195 ffc1 faff  e..?T...........
+00005360: 848d 8eb0 785c ae58 c9aa a45f e96f ebe1  ....x\.X..._.o..
+00005370: 9cc5 21ed a5c3 389c b46f 3a9d 5412 6f38  ..!...8..o:.T.o8
+00005380: aa22 0eea 92de 66c5 dd90 b2e9 a4f3 cf87  ."....f.........
+00005390: 848d 3f89 49b4 e3dc da65 dc78 c634 2912  ..?.I....e.x.4).
+000053a0: 3c28 10d1 1884 e3b4 867b 50aa a44f 7d94  <(.......{P..O}.
+000053b0: e63f 3b68 8c11 c98e ccd3 f8c0 7fec 2cfc  .?;h..........,.
+000053c0: e248 0535 5fa9 f06a 374f 2017 4dc0 ff65  .H.5_..j7O .M..e
+000053d0: 940c 515a f446 51ed 1ec0 0b34 2526 4ff2  ..QZ.FQ....4%&O.
+000053e0: 58ea 0f00 0000 ffff 0000 00ff ff94 d24b  X..............K
+000053f0: 0ac3 2010 06e0 ab88 07a8 f1b5 0946 68c8  .. ..........Fh.
+00005400: 45c4 0a5d a525 8a6d 6fdf 892d 6309 2eea  E..].%.mo..-c...
+00005410: 4e9d e1ff 46d4 c46b 0869 71c9 59b3 dd1e  N...F..k.iq.Y...
+00005420: 649b 28a7 24de dd1a 6135 0a4a 9e5c 393f  d.(.$...a5.J.\9?
+00005430: 5e5e 4b88 3eac 69a2 c349 686a 8ddf 7bcf  ^^K.>.i..Ihj..{.
+00005440: d00c 4711 f6d9 0e86 656b 98ff d6e6 df1a  ..G.....ek......
+00005450: c71a 0306 2dc8 ffdf 1245 a949 6582 1922  ....-....E.Ie.."
+00005460: 7002 d156 648f 229b 0a44 a022 db8a ea51  p..Vd."..D."...Q
+00005470: 5451 eabc 9fbb 4004 2aaa ade8 1e65 7fa7  TQ....@.*....e..
+00005480: 6c8f 0a44 a0a2 0f0a abff e10d 0000 ffff  l..D............
+00005490: 0000 00ff ff34 cdc1 0ac2 3010 04d0 5f09  .....4....0..._.
+000054a0: fb01 5611 e9a5 e9c5 9307 a1bf 10db 6d12  ..V...........m.
+000054b0: d49d b059 14ff de2a e436 6f0e 3343 4910  ...Y...*.6o.3CI.
+000054c0: b63c 4fea 5688 5d16 4f07 72f6 29ec 4970  .<O.V.].O.r.).Ip
+000054d0: 86bc 586b 8650 370e 2544 be06 8d59 aa7b  ..Xk.P7.%D...Y.{
+000054e0: f06a 9ef6 bb9e 9ce6 985a 3694 7f7b 2277  .j.......Z6..{"w
+000054f0: 8319 9e4d 89c3 c2fa d391 b627 58c3 b6db  ...M.......'X...
+00005500: bda1 f79a 986d fc02 0000 ffff 0300 504b  .....m........PK
+00005510: 0304 1400 0600 0800 0000 2100 a22d f25a  ..........!..-.Z
+00005520: a606 0000 951a 0000 1300 0000 786c 2f74  ............xl/t
+00005530: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
+00005540: 595b 8b1b 3714 7e2f f43f 0cf3 eef8 36e3  Y[..7.~/.?....6.
+00005550: cb12 6fb0 c776 d266 3709 5927 258f 5a5b  ..o..v.f7.Y'%.Z[
+00005560: f628 ab19 9991 bc1b 1302 2579 29b4 144a  .(........%y)..J
+00005570: d3d2 3e14 daa7 3e94 3681 045a 68f2 6b36  ..>...>.6..Zh.k6
+00005580: 4d49 5bc8 5fe8 9166 ec91 d672 3749 3790  MI[._..f...r7I7.
+00005590: 96ac 6199 d17c 3afa 74ce d1a7 dbe9 3337  ..a..|:.t.....37
+000055a0: 22ea ece3 8413 16b7 dcf2 a992 ebe0 78c8  ".............x.
+000055b0: 4624 9eb4 dc2b 837e a1e1 3a5c a078 8428  F$...+.~..:\.x.(
+000055c0: 8b71 cb9d 63ee 9ed9 7cf7 9dd3 6843 8438  .q..c...|...hC.8
+000055d0: c20e d48f f906 6ab9 a110 d38d 6291 0fa1  ......j.....b...
+000055e0: 18f1 536c 8a63 f836 6649 8404 bc26 93e2  ..Sl.c.6fI...&..
+000055f0: 2841 0760 37a2 c54a a954 2b46 88c4 ae13  (A.`7..J.T+F....
+00005600: a308 cc5e 1c8f c910 3b4f 1e7f f4f4 eb7b  ...^....;O.....{
+00005610: 4f7e f9f5 d977 9fb8 9b8b 367a 141a 8a05  O~...w....6z....
+00005620: 9705 439a ecc8 16b0 5151 6147 7b65 89e0  ..C.....QQaG{e..
+00005630: 731e d0c4 d947 b4e5 4273 2376 30c0 3784  s....G..Bs#v0.7.
+00005640: eb50 c405 7c68 b925 f5e7 1637 4f17 d146  .P..|h.%...7O..F
+00005650: 5689 8a35 75b5 7a7d f597 d5cb 2a8c f62a  V..5u.z}....*..*
+00005660: aacd 64b2 bb6c d4f3 7caf d65e da57 002a  ..d..l..|..^.W.*
+00005670: 5671 bd7a afd6 ab2d ed29 001a 0ea1 a729  Vq.z...-.).....)
+00005680: 17dd a6df 6976 ba7e 86d5 40e9 a3c5 76b7  ....iv.~..@...v.
+00005690: dead 960d bc66 bfba c2b9 edcb 9f81 57a0  .....f........W.
+000056a0: d4be b782 eff7 03f0 a281 57a0 14ef 5b7c  ..........W...[|
+000056b0: 52af 049e 8157 a014 5f5b c1d7 4bed ae57  R....W.._[..K..W
+000056c0: 37f0 0a14 5212 efad a04b 7ead 1a2c 7abb  7...R....K~..,z.
+000056d0: 848c 193d 6785 377d af5f af64 c673 1464  ...=g.7}._.d.s.d
+000056e0: c332 bb64 1363 168b 75b9 16a1 eb2c e903  .2.d.c..u....,..
+000056f0: 4002 2912 2476 c47c 8ac7 6808 c91c 204a  @.).$v.|..h... J
+00005700: 7613 e26c 9149 0889 3745 31e3 505c aa94  v..l.I..7E1.P\..
+00005710: faa5 2afc 973f 4f3d 298f a00d 8cb4 da92  ..*..?O=).......
+00005720: 1730 e12b 4592 8fc3 8709 998a 96fb 3e58  .0.+E.........>X
+00005730: 7535 c8f3 473f 3e7f f4c0 79fe e8fe e1ed  u5..G?>...y.....
+00005740: 8787 b77f 3ebc 73e7 f0f6 bdd4 9651 f11c  ....>.s......Q..
+00005750: 8a27 7ac5 3fbf ffec af6f 3e74 fe78 f0ed  .'z.?....o>t.x..
+00005760: 9f77 bfb0 e3b9 8eff eda7 8f9f 3cfe dc0e  .w..........<...
+00005770: 84ce e65e 78fa e5fd df1f de7f fad5 a7cf  ...^x...........
+00005780: 7eb8 6b81 b713 b4ab c307 24c2 dcb9 800f  ~.k.......$.....
+00005790: 9ccb 2c82 be29 2f98 ccf1 6ef2 7235 0621  ..,..)/...n.r5.!
+000057a0: 2246 0d14 826d 8be9 9e08 0de0 8539 a236  "F...m.......9.6
+000057b0: 5c07 9bce bb9a 80c0 d880 6767 d70d ae3b  \.........gg...;
+000057c0: 6132 13c4 d2f2 f930 3280 db8c d10e 4bac  a2.....02.....K.
+000057d0: 0e38 2fdb d23c 3c98 c513 7be3 c94c c75d  .8/..<<...{..L.]
+000057e0: 4668 dfd6 7680 6223 b4bd d914 9495 d84c  Fh..v.b#.......L
+000057f0: 0621 3668 5ea2 2816 6882 632c 1cf9 8ded  .!6h^.(.h.c,....
+00005800: 616c e9dd 3542 0cbf 6e93 61c2 381b 0be7  al..5B..n.a.8...
+00005810: 1a71 3a88 585d 3220 bb46 22e5 95ce 9108  .q:.X]2 .F".....
+00005820: e232 b711 8450 1bbe d9be ea74 18b5 f5ba  .2...P.....t....
+00005830: 8bf7 4d24 0c08 442d e407 981a 6e3c 8b66  ..M$..D-....n<.f
+00005840: 0245 3693 0314 51dd e15b 4884 3692 3bf3  .E6...Q..[H.6.;.
+00005850: 64a8 e37a 5c40 a427 9832 a737 c29c dbea  d..z\@.'.2.7....
+00005860: 5c4c a0bf 5ad0 cf83 b8d8 c3be 4de7 9189  \L..Z.......M...
+00005870: 4c04 d9b3 d9dc 428c e9c8 2edb 0b42 144d  L.....B......B.M
+00005880: ad9c 491c ead8 f7f8 1ea4 2872 2e31 6183  ..I.......(r.1a.
+00005890: 6f33 7384 c877 8803 8ad7 86fb 2ac1 46b8  o3s..w......*.F.
+000058a0: 8f17 822b a0ab 3aa5 3c41 e497 5962 89e5  ...+..:.<A..Yb..
+000058b0: 59cc ccf1 38a7 6384 95ca 80ec 1b6a 1e91  Y...8.c......j..
+000058c0: f858 693f 22ea fe5b 514f 67a5 a3a2 de4e  .Xi?"..[QOg....N
+000058d0: 8875 689d 3b22 e5eb 70ff 4101 efa2 597c  .uh.;"..p.A...Y|
+000058e0: 09c3 9859 9dc0 deea f75b fd76 fff7 fabd  ...Y.....[.v....
+000058f0: 6e2c 9fbc 6ae7 420d 1a9e afd6 d5da 3d5a  n,..j.B.......=Z
+00005900: bb74 1f13 4a77 c49c e22d ae56 ef1c a6a7  .t..Jw...-.V....
+00005910: 511f 0ad5 b642 ed2d 975b b969 088f d946  Q....B.-.[.i...F
+00005920: c1c0 4d12 a4ea 3809 131f 1011 ee84 680a  ..M...8.......h.
+00005930: 4bfc b2da 884e 7866 7ac2 9d29 e3b0 f257  K....Nxfz..)...W
+00005940: c56a 678c 8fd8 56fb 8759 b4cd 46e9 8eb5  .jg...V..Y..F...
+00005950: 5c96 bbd3 543c 3812 7979 c95f 96c3 6e43  \...T<8.yy._..nC
+00005960: a4e8 5a3d df85 2dcd ab7d ed44 ed96 1704  ..Z=..-..}.D....
+00005970: 64dd 9721 a135 6692 a85a 48d4 1785 1085  d..!.5f..ZH.....
+00005980: 7f22 a17a 7622 2c9a 1616 0d69 7e11 aa45  .".zv",....i~..E
+00005990: 1497 ae00 6acb a8c0 fac9 8155 57cb f5bd  ....j......UW...
+000059a0: f424 0036 5588 e291 8c53 7a28 b088 ae0c  .$.6U....Sz(....
+000059b0: ce89 467a 9d33 a99e 01b0 9858 6440 1ee9  ..Fz.3.....Xd@..
+000059c0: a6e4 bab6 7bb2 7769 aabd 40a4 0d12 5aba  ....{.wi..@...Z.
+000059d0: 9924 b434 0cd1 0867 d9a9 1f9d 9c64 ac9b  .$.4...g.....d..
+000059e0: 7948 0d7a d215 8bd1 90d3 a837 5e47 aca5  yH.z.......7^G..
+000059f0: 881c d106 1aeb 4a41 63e7 a0e5 d6aa 3e1c  ......JAc.....>.
+00005a00: 920d d1b4 e58e 61e7 0f8f d114 7287 cb75  ......a.....r..u
+00005a10: 2fa2 1338 451b 8a24 1df0 afa2 2cd3 848b  /..8E..$....,...
+00005a20: 2ee2 61ea 7025 3aa9 1a44 44e0 c4a1 246a  ..a.p%:..DD...$j
+00005a30: b9b2 fbcb 6ca0 b1d2 10c5 ad5c 0141 7863  ....l......\.Axc
+00005a40: c935 4156 de34 7210 7433 c878 3cc6 43a1  .5AV.4r.t3.x<.C.
+00005a50: 875d 2b91 9e4e 5f41 e153 adb0 7e55 d55f  .]+..N_A.S..~U._
+00005a60: 1d2c 6bb2 1984 7b27 1c1d 38bb 7496 5c46  .,k...{'..8.t.\F
+00005a70: 9062 7ebd 2c1d 3822 1c0e 80ca a937 4704  .b~.,.8".....7G.
+00005a80: 4e34 9742 96e7 df91 8929 935d fd48 51e5  N4.B.....).].HQ.
+00005a90: 505a 8ee8 3444 d98c a28b 790a 5722 baa4  PZ..4D....y.W"..
+00005aa0: a3de 963e d0de b23e 8343 575d b83b 9113  ...>...>.CW].;..
+00005ab0: ecbf 9e75 8f9f aaa5 e734 d1cc e74c 4355  ...u.....4...LCU
+00005ac0: e4ac 6917 d3d7 37c9 6bac f249 d460 954a  ..i...7.k..I.`.J
+00005ad0: b7da 36f0 5ceb 9a0b ad83 44b5 ce12 c7cc  ..6.\.....D.....
+00005ae0: ba2f 3021 68d4 f2c6 0c6a 92f1 aa0c 4bcd  ./0!h....j....K.
+00005af0: ce4a 4d6a 27b8 20d0 3c51 5be3 b7e5 1c61  .JMj'. .<Q[....a
+00005b00: f5c4 abce fc50 ef68 d6ca 0962 b1ae 5489  .....P.h...b..T.
+00005b10: af6e 40f4 db09 b67b 1dc4 a30b e7c0 332a  .n@....{......3*
+00005b20: b80a 25dc 3d24 0816 7de9 4972 2a1b 3044  ..%.=$..}.Ir*.0D
+00005b30: 6e88 6c8d 084f ce2c 212d f766 c96f 7b41  n.l..O.,!-.f.o{A
+00005b40: c50f 0aa5 86df 2b78 55af 5468 f8ed 6aa1  ......+xU.Th..j.
+00005b50: edfb d572 cf2f 97ba 9dca 2d98 5844 1895  ...r./....-.XD..
+00005b60: fdf4 f6a5 0fe7 5174 9edd c1a8 f295 7b98  ......Qt......{.
+00005b70: 6871 e476 6ac8 a222 53f7 2c45 455c ddc3  hq.vj.."S.,EE\..
+00005b80: 942b b67b 9881 bc61 711d 02a2 73b3 56e9  .+.{...aq...s.V.
+00005b90: 37ab cd4e add0 acb6 fb05 afdb 6914 9a41  7..N........i..A
+00005ba0: ad53 e8d6 827a b7df 0dfc 46b3 7fcb 75f6  .S...z....F...u.
+00005bb0: 15d8 6b57 03af d66b 146a e520 2878 b592  ..kW...k.j. (x..
+00005bc0: a4df 6816 ea5e a5d2 f6ea ed46 cf6b dfca  ..h..^.....F.k..
+00005bd0: 9631 d0f3 543e 325f 807b 15af cdbf 0100  .1..T>2_.{......
+00005be0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00005bf0: 0021 0020 4456 f605 0300 006e 0700 000d  .!. DV.....n....
+00005c00: 0000 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
+00005c10: b455 cd6e d340 10be 23f1 0eab bdbb fe49  .U.n.@..#......I
+00005c20: 1c92 c876 d534 b554 a948 482d 12d7 8dbd  ...v.4.T.HH-....
+00005c30: 4e56 dd1f 6bbd 290e 0889 2327 4e08 f10e  NV..k.)...#'N...
+00005c40: 70e8 8103 0f84 0abc 05b3 b6d3 b8aa 04b4  p...............
+00005c50: 1597 7877 76f7 9b6f e69b 9944 fbb5 e0e8  ..xwv..o...D....
+00005c60: 82ea 8a29 1963 7fcf c388 ca4c e54c 2e63  ...).c.....L.L.c
+00005c70: fcfc 2c75 c618 5586 c89c 7025 698c 37b4  ..,u..U...p%i.7.
+00005c80: c2fb c9e3 4751 6536 9c9e ae28 3508 2064  ....GQe6...(5. d
+00005c90: 15e3 9531 e5d4 75ab 6c45 05a9 f654 4925  ...1..u.lE...TI%
+00005ca0: 9c14 4a0b 6260 ab97 6e55 6a4a f2ca 3e12  ..J.b`..nUjJ..>.
+00005cb0: dc0d 3c6f e40a c224 6e11 a622 fb17 1041  ..<o...$n.."...A
+00005cc0: f4f9 ba74 3225 4a62 d882 7166 360d 1646  ...t2%Jb..qf6..F
+00005cd0: 229b 1e2f a5d2 64c1 816a ed0f 4986 6a7f  "../..d..j..I.j.
+00005ce0: a403 54eb ad93 c67a cb8f 6099 5695 2acc  ..T....z..`.V.*.
+00005cf0: 1ee0 baaa 2858 466f d39d b813 9764 3b24  ....(XFo.....d;$
+00005d00: 40be 1f92 1fba 5e70 23f6 5adf 1369 e86a  @.....^p#.Z..i.j
+00005d10: 7ac1 ac7c 3889 0a25 4d85 32b5 9626 c601  z..|8..%M.2..&..
+00005d20: 10b5 2998 9e4b f552 a6f6 0814 ee6e 2551  ..)..K.R.....n%Q
+00005d30: f50a 5d10 0e96 00bb 4994 29ae 3432 201d  ..].....I.).42 .
+00005d40: 64ce b716 4904 6d6f 5c7d bcfc f1f5 f2ea  d...I.mo\}......
+00005d50: d3fb 5f9f 3fd8 9382 08c6 37ed 59fb 7845  .._.?.....7.Y.xE
+00005d60: 7405 85d0 e20d 46f6 5253 061d 8060 208a  t.....F.RS...` .
+00005d70: 35ba 9660 4b73 4760 f29f bd35 4e2b f0ca  5..`KsG`...5N+..
+00005d80: 38ef 25a7 3524 1154 91a1 5aa6 708a baf5  8.%.5$.T..Z.p...
+00005d90: d9a6 842c 4828 f896 341c fdf5 f652 938d  ...,H(..4....R..
+00005da0: 1f84 bd07 6ee3 3089 164a e7d0 605b 59ac  ....n.0..J..`[Y.
+00005db0: 02ad 2989 382d 0ca4 45b3 e5ca 7e8d 2ae1  ..).8-..E...~.*.
+00005dc0: 77a1 8c81 224c a29c 91a5 9284 dbc4 6d5f  w..."L........m_
+00005dd0: 740b 0827 a39c 9fda 267c 51dc c0ae 0b24  t..'....&|Q....$
+00005de0: d722 15e6 388f 31b4 b34d f976 0981 74cb  ."..8.1..M.v..t.
+00005df0: 16af dd24 11e1 6c29 0595 2021 d586 65b6  ...$..l).. !..e.
+00005e00: 2e32 d8d2 56b5 ba00 067d 7fad f79e e300  .2..V....}......
+00005e10: 82ba bb63 5417 7760 f000 7c44 ca92 6f0e  ...cT.w`..|D..o.
+00005e20: b651 7615 de84 0441 f472 7923 93d7 1123  .Qv....A.ry#...#
+00005e30: db0b 31fe feed edcf 775f a0ab 3ad6 68b1  ..1.....w_..:.h.
+00005e40: 66dc 30d9 c660 55ba 7e01 9879 bdd3 c5b3  f.0..`U.~..y....
+00005e50: 6561 ec58 6a14 bbf6 02f2 e4b4 206b 6ece  ea.Xj....... kn.
+00005e60: ae0f 63bc 5b3f a539 5b0b 68e4 eed6 3376  ..c.[?.9[.h...3v
+00005e70: a14c 0311 e3dd fac4 968f df74 1dad cd49  .L.........t...I
+00005e80: 051d 065f b4d6 2cc6 af8f 664f 26f3 a334  ..._..,...fO&..4
+00005e90: 70c6 de6c ec0c 0734 7426 e16c ee84 c3c3  p..l...4t&.l....
+00005ea0: d97c 9e4e bcc0 3b7c d31b 8e0f 188d cd2c  .|.N..;|.......,
+00005eb0: 873a f087 d38a c300 d55d b01d f9d3 9d2d  .:.......].....-
+00005ec0: c6bd 4d4b bf69 1ca0 dde7 3e09 46de 41e8  ..MK.i....>.F.A.
+00005ed0: 7b4e 3af0 7c67 3822 6367 3c1a 844e 1afa  {N:.|g8"cg<..N..
+00005ee0: c17c 349c 1d85 69d8 e31e de73 847a aeef  .|4...i....s.z..
+00005ef0: b7c3 d892 0fa7 8609 ca99 dc6a b555 a86f  ...........j.U.o
+00005f00: 0591 60fb 8720 dcad 12ee ee8f 32f9 0d00  ..`.. ......2...
+00005f10: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00005f20: 0021 0016 1bf7 990e 1d00 009d 8600 0014  .!..............
+00005f30: 0000 0078 6c2f 7368 6172 6564 5374 7269  ...xl/sharedStri
+00005f40: 6e67 732e 786d 6cc4 5d59 731b 4792 7edf  ngs.xml.]Ys.G.~.
+00005f50: 88fd 0f0a 466c c4ec 8347 bcc7 de90 3541  ....Fl...G....5A
+00005f60: 5294 c519 5e16 693b fcd4 d168 34c8 1e01  R...^.i;...h4...
+00005f70: 680c ba41 89fb a4c3 3429 8ab2 e41d 9196  h..A....4)......
+00005f80: 2cea b2a4 19da 1645 8bb2 25ea fe33 6c1c  ,......E..%..3l.
+00005f90: 4ffb 17f6 abaa 06d0 eccc 6a80 a223 f60d  O.........j..#..
+00005fa0: a8ca caca cacc caca caca aa3e f2e7 33b9  ...........>..3.
+00005fb0: eca1 39bb e839 6efe e38e ae3f 7676 1cb2  ..9..9n....?vv..
+00005fc0: f396 9b76 f233 1f77 7c36 7dfc 830f 3b0e  ...v.3.w|6}...;.
+00005fd0: 79be 994f 9b59 376f 7fdc 316f 7b1d 7f3e  y..O.Y7o..1o{..>
+00005fe0: faef ff76 c4f3 fc43 689b f73e ee98 f5fd  ...v...Ch..>....
+00005ff0: c27f 1d3e ec59 b376 cef4 fee8 16ec 3c6a  ...>.Y.v......<j
+00006000: 326e 3167 faf8 5b9c 39ec 158a b699 f666  2n1g..[.9......f
+00006010: 6ddb cf65 0f77 7776 f61f ce99 4ebe e390  m..e.wwv....N...
+00006020: e596 f2fe c71d dddd 3d7d 1d87 4a79 e7ef  ........=}..Jy..
+00006030: 257b 4815 7575 f674 771c 3de2 3947 8ff8  %{H.uu.tw.=.9G..
+00006040: 4727 8e1d 39ec 1f3d 5298 050d be63 4d16  G'..9..=R....cM.
+00006050: 0f65 dcbc 3f92 06c5 1d87 fcf9 0208 cbbb  .e..?...........
+00006060: 436e 3e1c 48c7 e1a3 470e 8b96 aaf5 5f87  Cn>.H...G....._.
+00006070: bf9c 3a48 7bcb 75d2 0769 9f4b 9bbe fdff  ..:H{.u..i.K....
+00006080: 4980 99cd 1a82 06ef 7721 22c2 d98c 9337  I.......w!"....7
+00006090: 3c3b 9b31 4ccb 92b8 2375 cd51 470a 4fd9  <;.1L...#u.QG.O.
+000060a0: f33d 71c0 bc1b 2ff1 ec5c bc48 f424 041d  .=q.../..\.H.$..
+000060b0: 2fb7 4ac5 62bc cccc e795 bc62 943a b4d8  /.J.b......b.:..
+000060c0: 2974 75c7 9bcf 90ce 1dcf 75e2 508e e7a4  )tu.......u.P...
+000060d0: 7c5a 9867 00f3 4e21 0e58 ece9 ec8f 97d9  |Z.g..N!.X......
+000060e0: 0525 9f08 d5c5 aece 3ed2 b48b 3605 dc9f  .%......>...6...
+000060f0: 18b8 0f49 596f 6717 5346 5850 eced 2462  ...IYog.SFXP..$b
+00006100: 4259 2fd3 96d0 2724 6596 d28e ef12 c178  BY/...'$e......x
+00006110: fe29 a350 742c 22c5 dc29 c24a 6145 0c22  .).Pt,"..).JaE."
+00006120: c659 6766 9696 66dd d3b4 d0ca ba9e 4d8b  .Ygf..f.......M.
+00006130: cdf4 df32 2651 d639 374b b428 4768 f28b  ...2&Q.97K.(Gh..
+00006140: f938 542a 340d 11a1 b999 8c4d 7572 6ea6  .8T*4......Murn.
+00006150: 5024 dd16 a95e cde6 b205 8bf6 5c2a e65d  P$...^......\*.]
+00006160: 5837 3253 66cd 6238 ada3 53ef 946f 9944  X72Sf.b8..S..o.D
+00006170: e7c0 6494 1a0c 7633 e773 c505 da5f 2145  ..d...v3.s..._!E
+00006180: 4848 3b73 c63c e582 a529 cfc1 70cf 1a9e  HH;s.<...)..p...
+00006190: 99a5 648b 796b 9039 90ee eca4 4a2b 0a89  ..d.yk.9....J+..
+000061a0: d68a 42a2 b6a2 90e8 ad28 248a 2b0a c9a4  ..B......($.+...
+000061b0: 1485 646a 99bd 39f3 cc2c 5118 514a 3456  ..dj..9..,Q.QJ4V
+000061c0: c2b2 4cef cd39 790e 0963 a680 04b3 8a93  ..L..9y..c......
+000061d0: 5cef 6c66 8612 32cf 15e6 68a1 9735 a43c  \.lf..2...h..5.<
+000061e0: e218 fc0f 1983 82c2 2e6a 3dba 8891 015c  .........j=....\
+000061f0: 0f11 8328 a4e6 a39b 5ab7 6e22 8262 77bf  ...(....Z.n".bw.
+00006200: 1927 1062 a16d 4521 27c0 6ec6 367e 444c  .'.b.mE!'.n.6~DL
+00006210: 1985 4a99 c519 7829 3386 35eb 50db fcf7  ..J...x)3.5.P...
+00006220: 8ce3 18a9 d27c 1c91 2cc7 a248 0c8a acb0  .....|..,..H....
+00006230: cfb0 f029 4c41 1e91 aec2 3ea3 ab61 d424  ...)LA....>..a.$
+00006240: 53c2 cc62 6895 e51c adb2 82d2 aaf0 301d  S..bh.........0.
+00006250: 2b44 ba0a 96d6 4c9a 53e8 74b6 58e0 2895  +D....L.S.t.X.(.
+00006260: e51c a5b2 8252 aaf0 3004 2944 ba0a 9652  .....R..0.)D...R
+00006270: 3499 d5d0 044b c648 5a36 6069 021e be6b  4....K.HZ6`i...k
+00006280: 6112 a90a 8488 f81a 8e7d beeb 7394 8a62  a........}..s..b
+00006290: 8e50 514e e994 4898 3e25 164d 39cb 3868  .PQN..H.>%.M9.8h
+000062a0: 9c41 a681 a083 9662 7731 6390 29a0 4ac9  .A.....bw1c.).J.
+000062b0: ecb7 4c6f 9641 e1e4 1c9f 160b 22c8 a222  ..Lo.A......".."
+000062c0: 89a0 a5b3 6ed1 a754 78aa 9890 5130 19cc  ....n..Tx...Q0..
+000062d0: 5949 0545 6d64 3979 c157 f06c df20 8b6a  YI.Emd9y.W.l. .j
+000062e0: 584e ba14 eba6 9122 5638 2c26 e045 db87  XN....."V8,&.E..
+000062f0: e340 8849 b9c5 a2e1 132c 6131 c1a2 8644  .@.I.....,a1...D
+00006300: 7bcd e6a8 3f42 8b7c 5a04 6fcb 4813 61ab  {...?B.|Z.o.H.a.
+00006310: 52e2 b678 c2c5 31d2 8ee7 179d 54c9 c73e  R..x..1.....T..>
+00006320: 356e 286d b1b7 21a3 c958 54ec 85ac 9d9e  5n(m..!..XT.....
+00006330: a1c5 1201 7127 bcd9 62ce 28f5 7676 52a7  ....q'..b.(.vvR.
+00006340: abe8 e92a 0aba 8a9c e1ea 5069 2a0a ba16  ...*......Pi*...
+00006350: 39a3 d720 eb1c a8f5 34e5 054d 79ce e837  9.. ....4..My..7
+00006360: c8ea 2df1 f0e5 050d 7cce f8d0 e8e2 b9a4  ..-.....|.......
+00006370: a928 e85a 804b 5df0 b858 8eeb 6ac0 27b6  .(.Z.K]..X..j.'.
+00006380: 0d36 1ba6 ef13 1585 1b6c a488 9b06 a7ab  .6.......l......
+00006390: 040d 9b37 888f dea8 21bb 1660 c71e 857a  ...7....!..`...z
+000063a0: 55d0 d502 539c b366 b1fb 213d 7b25 163a  U...S..f..!={%.:
+000063b0: 5382 99a4 b8d5 5c64 cb5d 06dc 4b99 699f  S.....\d.]..K.i.
+000063c0: 2977 d267 0cff 74be 8f70 5a54 e43c 8bee  )w.g..t..pZT.<..
+000063d0: 6251 eefa 16df 0015 88e9 c485 2650 cd62  bQ..........&P.b
+000063e0: 17c0 95e7 98fd c940 c3d1 7fcf 388f 40a0  .......@....8.@.
+000063f0: 66f1 0110 28cf f53d 114c 0f0c 8e0e 1be3  f...(..=.L......
+00006400: 0363 c353 72d4 ef89 e660 e1ae a189 d1cf  .c.Sr....`......
+00006410: c6c6 0f44 c0ef 348e df09 cdc0 e488 2151  ...D..4.......!Q
+00006420: 1d84 a7d3 5f8c 1f1e 383e 3c35 3d46 560a  ...._...8><5=FV.
+00006430: 5935 32fe f9f1 91f1 4fe3 ca2a eb26 4726  Y52.....O..*.&G&
+00006440: 4f0e 1d3b 70ef 9323 5303 a3c3 9a1e a64e  O..;p..#S......N
+00006450: 9c1c 189a 4eac fc42 573b fdd7 81e9 e993  ....N..BW;......
+00006460: f15a c1b6 a189 63aa c3f7 d4c4 a113 e307  .Z....c.........
+00006470: 57e7 eaf6 bde0 d28d 0faa 8b3f 557e bb5a  W..........?U~.Z
+00006480: 5edd 3908 23eb b8b6 ef55 7e79 7320 44e7  ^.9.#....U~ys D.
+00006490: ef55 1e6e 94bf 7b58 7dba 585e bb51 bdb7  .U.n..{X}.X^.Q..
+000064a0: 7110 6ce5 f5a5 cae2 9df2 b567 0741 5279  q.l........g.ARy
+000064b0: b252 f9e1 b5a2 e720 786a 37bf de7d 77eb  .R..... xj7..}w.
+000064c0: e078 aa92 45c1 9347 e5b3 ff3a 3836 619d  .x..E..G...:86a.
+000064d0: 5504 e03d 7531 55a0 e107 9411 bf2d 55e8  U..=u1U......-U.
+000064e0: a6ae 6da1 9b81 eb61 e07a 99b2 3eae 8cc1  ..m....a.z..>...
+000064f0: d747 c21e a942 3fd3 b69f 69db cfb5 2511  .G...B?...i...%.
+00006500: 9354 e14f 0cbe 3f31 f83e 221e 62aa f011  .T.O..?1.>".b...
+00006510: 0984 a08c 7880 2823 d191 d41c c3fb 3986  ....x.(#......9.
+00006520: f773 5d74 1c73 5d74 1c73 8c8c e618 79cc  .s]t.s]t.s....y.
+00006530: 31f2 98eb a5e3 cd30 f465 18fa 324c bf19  1......0.e..2L..
+00006540: 4637 320c 2d19 8696 0c47 4b2f e541 a697  F72.-....GK/.A..
+00006550: f220 d34b c25f a90c c37b cf22 5bb2 9497  . .K._...{."[...
+00006560: e70a 7d06 d022 3b70 d198 29f4 9932 8f38  ..}..";p..)..2.8
+00006570: bd29 2f4b 0bd3 363d 0bf9 7bc9 b14e c5d7  .)/K..6=..{..N..
+00006580: a402 3dc1 3189 878e 4319 a2e4 0e33 a951  ..=.1...C....3.Q
+00006590: 4614 c129 50c1 3905 2a38 9431 6da9 e000  F..)P.9.*8.1m...
+000065a0: 4784 e414 a841 7098 4983 3232 b91c 6622  G....Ap.I.22..f"
+000065b0: 39cc 6440 1951 1887 9920 0e33 411c 6632  9.d@.Q... .3A.f2
+000065c0: 388c 4263 9be2 91ed 885b 20be 7fbe 488a  8.Bc.....[ ...H.
+000065d0: 6849 9e69 68a7 1cb2 cbb7 1801 a18c 08c3  hI.ih...........
+000065e0: 723c 7a96 6671 6a20 0a99 e65c 3f9c 26a0  r<z.fqj ...\?.&.
+000065f0: 3955 058b 5b44 5048 950b 8554 bb50 48ed  9U..[DPH...T.PH.
+00006600: be28 a474 a290 580b 0149 a46f 315a 6731  .(.t..X..I.o1Zg1
+00006610: da84 32da 0ba3 61d6 1cc3 3546 c3ac 3946  ..2...a...5F..9F
+00006620: 388c d659 8cd6 a18c d2c2 9860 8bd1 4e8b  8..Y.......`..N.
+00006630: 31b7 964f 2d83 e553 936e 2117 811c 8b58  1..O-..S.n!....X
+00006640: 5eca 22e7 2d80 cc90 f367 5148 545e 1466  ^.".-....gQHT^.f
+00006650: e2f6 ccf2 6c8a 13e7 661e 8d52 9d36 e708  ....l...f..R.6..
+00006660: 49be 79a6 58cf 0dd8 7bec 4bcf 4aba ba98  I.y.X...{.K.J...
+00006670: c312 e638 b78b b21c 47b7 dc51 303d 03e9  ...8....G..Q0=..
+00006680: a561 9c62 1f3d 6843 1931 d0c5 6ee6 a8ba  .a.b.=hC.1..n...
+00006690: 8f2b eba2 c731 7d0c cd7d 9d94 be7e 661c  .+...1}..}...~f.
+000066a0: fd5d f4c4 a89f 1947 3f73 44de 4fbd 9562  .].....G?sD.O..b
+000066b0: 3f43 4b3f 470b f56a d096 f2a5 9f91 5b0f  ?CK?G..j......[.
+000066c0: 434b 0f73 bcde c3f0 af87 19ef 87f4 6c4d  CK.s..........lM
+000066d0: 39ef bbaf ee63 4b11 d75a ec7a caeb 77e2  9....cK..Z.z..w.
+000066e0: a562 03f3 70b3 b2f3 06db 9860 e121 d96c  .b..p......`.!.l
+000066f0: babe 9935 26a0 dca6 2f0e c546 9026 9423  ...5&.../..F.&.#
+00006700: ee41 79eb 66b0 f463 bced 2745 d7f3 8cc9  .Ay.f..c..'E....
+00006710: a29b 4184 7e54 fcce 14dd 5c1d 994b 23d4  ..A.~T....\..K#.
+00006720: 8a16 602a bf79 1047 d624 4121 8cd7 ab56  ..`*.y.G.$A!...V
+00006730: 1847 edde e578 5d48 c2a0 8dec 24db 9836  .G...x]H....$..6
+00006740: c969 5cf9 f906 dfeb 38c2 f46a c872 0084  .i\.....8..j.r..
+00006750: a55b 9783 8547 c195 1d85 205e 1d69 3d80  .[...G.... ^.i=.
+00006760: 98a4 0864 9b29 84f2 7dd7 9844 783b 4f96  ...d.)..}..Dx;O.
+00006770: c9f2 d615 21c1 8d85 e0e2 65a0 acdc 5ca6  ....!.....e...\.
+00006780: 4391 03a8 1335 6917 8d29 112a d753 a650  C....5i..).*.S.P
+00006790: de5c aa3d b81e 071a 343d c732 86cd 621e  .\.=....4=.2..b.
+000067a0: a285 a474 c894 5c94 902b df2c f272 1ec3  ...t..\..+.,.r..
+000067b0: b929 8eab 4fc2 b219 5017 8b19 5e43 be18  .)..O...P...^C..
+000067c0: 1883 27ae 65c9 b8ea 4c82 e018 5c93 4ad0  ..'.e...L...\.J.
+000067d0: 753e 2552 054c 6f57 9404 194c 1121 b61a  u>%R.LoW...L.!..
+000067e0: dbb5 67e5 a5ab b5d5 e70c 9629 91fa 6060  ..g........)..``
+000067f0: 469c 461e 84c0 c3cf 43c5 632d 1635 a342  F.F.....C.c-.5.B
+00006800: 4eb7 4426 3873 7359 8b8c b03b 0961 84db  N.D&8ssY...;.a..
+00006810: 5a84 319e b740 5767 b916 5d84 f109 a882  Z.1..@Wg..].....
+00006820: 9df3 c1dd 5f83 2562 b96a 6b97 2a37 1f04  ...._.%b.jk.*7..
+00006830: 175e 90a9 b17e b6f6 f375 be62 f7cd 375c  .^...~...u.b..7\
+00006840: c5b5 673c aaea 4fef caab bfee be3b 5f8f  ..g<..O......;_.
+00006850: 6f45 9673 8c6b f7e5 83da e215 23b8 7c01  oE.s.k......#.|.
+00006860: b39a 9011 d67f 0b83 6504 0b17 f8fa cae6  ........e.......
+00006870: d71c eef5 b342 65af 6c56 1ebc ac6e 3fe7  .....Be.lV...n?.
+00006880: c7d2 8478 7a9f 81a8 ac3e c38a 10dc 5a64  ...xz....>....Zd
+00006890: ea82 bb4f 6a0b 8f18 3506 e314 8b82 e78f  ...Oj...5.......
+000068a0: 8905 fe76 a3fa e622 d3a8 fcdb b9da d9ef  ...v..."........
+000068b0: 83f5 8de0 c11a 1881 f168 5812 9cbd 847a  .........hX....z
+000068c0: 21d1 b3af 3996 a89a f2d6 b5da 22b1 f175  !...9......."..u
+000068d0: 760b 766a 20d6 1f89 e9b0 752d 4eb8 e8f3  v.vj .....u-N...
+000068e0: c20b 6100 cebe d654 6349 7abc c65b 9aca  ..a....TcIz..[..
+000068f0: 95b7 b5c5 6f05 0ed6 1005 6b8f 1b61 4231  ....o.....k..aB1
+00006900: 6c46 d2c1 37af 8217 bfb6 0318 c1d5 9836  lF..7..........6
+00006910: fffb 7a81 4822 0257 5d5a dcdd 5906 0918  ..z.H".W]Z..Y...
+00006920: 1903 5af9 75ab ba11 4631 13c9 6b03 300a  ..Z.u...F1..k.0.
+00006930: 9244 5e79 f379 7065 bbac a661 6bf6 e8c1  .D^y.ype...ak...
+00006940: 5ffc 8a71 1169 2e2d ea5a 8005 ff41 a659  _..q.i.-.Z...A.Y
+00006950: 9d18 a1d7 fb20 8680 b724 26d6 8223 26b8  ..... ...$&..#&.
+00006960: f85b 79ed 174c b2c3 0026 528d 561a d577  .[y..L...&R.V..w
+00006970: dfee ee9c 85de 2483 0557 5794 ecab af89  ......$..WW.....
+00006980: 8501 8aae 6ea1 9ced eac0 3e1a 70a0 493a  ....n.....>.p.I:
+00006990: 01f8 9e18 29fb 046f a1e8 4c07 d5c7 cbc1  ....)..o..L.....
+000069a0: a555 182c ed14 0afd 3119 e3e7 0c92 e25c  .U.,....1......\
+000069b0: 2ba8 3a2f 5ac1 09f3 f874 11f6 bc76 763b  +.:/Z....t...vv;
+000069c0: 78fd 1b63 f743 08d8 f3c5 9789 10db cfab  x..c.C..........
+000069d0: 4fef 579f 2db4 0042 47b0 5d9a 0528 da59  O.W.-..BG.]..(.Y
+000069e0: 4ba8 7a87 ad00 cb2b e784 874b 9dc8 f2f2  K.z....+...K....
+000069f0: eaee bb7b 4983 0f21 1206 dfc0 9134 f868  ...{I..!.....4.h
+00006a00: 477a 6aa3 9db5 846a 3d78 854e 3b78 7148  Gzj....j=x.N;xqH
+00006a10: b678 2758 fd3a 3a7e 03a5 d57b 2bc4 be35  .x'X.::~...{+..5
+00006a20: 6023 9c48 8405 d228 435a e295 0a18 0eba  `#.H...(CZ......
+00006a30: 2d1a da80 6dd0 d026 dec8 2430 6ae7 ded5  -...m..&..$0j...
+00006a40: beff a93d 3e24 c1c6 f9d0 0a6f 940f 6dd1  ...=>$.....o..m.
+00006a50: 108e ad2d 1ada 8085 3e68 3526 b8ba 8475  ...-....>h5&...u
+00006a60: 3bd1 5628 8824 5b51 c791 682b 221d 254c  ;.V(.$[Q..h+".%L
+00006a70: ee48 672d a15a 4f97 eaed cb0d 4b48 e4ae  .Hg-.ZO.....KH..
+00006a80: eae4 b8f8 3aec 7499 2080 c2a9 ea58 5b2e  ....:.t. ....X[.
+00006a90: fdb8 e0ab 3bb5 f35f 69f0 deb8 cae3 0d96  ....;.._i.......
+00006aa0: 7694 2498 76a2 4e47 2bea b4b4 36ea 34b4  v.$.v.NG+...6.4.
+00006ab0: a25e 4bab 68cb d3fa 7411 759c 8f2b 2b76  .^K.h...t.u..++v
+00006ac0: 5ffe 4f79 f937 3288 481d eb95 9fbd a31d  _.Oy.72.H.......
+00006ad0: 6410 a963 0722 3721 e038 3010 4746 b6e5  d..c."7!.80.GF..
+00006ae0: 19a4 f0ea 85a9 ea83 2b5b bb6f de55 ae6d  ........+[.o.U.m
+00006af0: 406c c1cb 7ff2 52ad 3cdb c42c 6356 2428  @l....R.<..,cV$(
+00006b00: 0ca8 d256 63e3 575e 7aa6 ad16 dbab ed35  ...Vc.W^z......5
+00006b10: b52b 49dc f428 4065 9b82 cb77 19e1 a893  .+I..(@e...w....
+00006b20: fdca 8dd7 c1ce 056c d9e2 c350 d5c1 cb9f  .......l...P....
+00006b30: 83cd eb89 3d55 3736 ab4f 7f4a de81 219a  ....=U76.O.J..!.
+00006b40: f5ed 323a f943 984e 80ed daa3 e5ff 244e  ..2:.C.N......$N
+00006b50: f3fa 4fe5 57ef 90d9 08ff 4201 eebe 7cc9  ..O.W.....B...|.
+00006b60: ee53 e370 bc43 5226 f878 4ec0 a3a9 9dfb  .S.p.CR&.xN.....
+00006b70: a675 bf14 8eef 9781 6325 801e 3fe8 6f39  .u......c%..?.o9
+00006b80: da38 14df 2781 627b 446f 1f7c d8b2 c738  .8..'.b{Do.|...8
+00006b90: 14df 2381 627b 446f 1f88 8cca 1622 2560  ..#.b{Do....."%`
+00006ba0: 7c9f 148c ed54 09a0 8d6e 19c0 2491 eec1  |....T...n..$...
+00006bb0: c8eb 12ae a5f9 059a f859 ddbc 2866 fdc6  .........Y..(f..
+00006bc0: e3da bddb 7fd8 ddd9 24ba afda 91f8 dd9e  ........$.......
+00006bd0: 76d5 4b4f e89c b9f5 2eb8 b7cc 04aa 2ad7  v.KO..........*.
+00006be0: 7e40 041e 1506 ba2b af91 f06a b31e 6899  ~@.....+...j..h.
+00006bf0: faf2 f5ad e0ea 3f2b e75f 969f 6e94 bf92  ......?+._..n...
+00006c00: 01e4 872a ad29 1a8d aa03 556f ac56 de3c  ...*.)....Uo.V.<
+00006c10: 56e7 04c4 e22e 7d8d 3857 6ded 1fb5 efaf  V.....}.8Wm.....
+00006c20: 956f 9cc7 0f32 f125 9af2 f73f 07e7 d611  .o...2.%...?....
+00006c30: dd2a 5fd7 4004 0bc2 e602 22b8 b84d 70bc  .*_.@....."..Mp.
+00006c40: deae 3e5f 0182 eac6 abea 0609 4aab e184  ..>_........J...
+00006c50: d1bb cb4f cb75 6882 4612 a1ac 67b0 b024  ...O.uh.F...g..$
+00006c60: 16d9 b72b c28c 2660 0593 aa8b 2f2b e7ee  ...+..&`..../+..
+00006c70: f775 c232 074b 5f73 71b9 3aa7 c6a6 8646  .u.2.K_sq.:....F
+00006c80: 5a43 055b 2be5 9f2f b483 4f41 2265 b635  ZC.[+../..OA"e.5
+00006c90: 5244 0084 993e b755 5e59 8459 550d 7859  RD...>.U^Y.YU.xY
+00006ca0: 6048 509b e0f6 25a8 bc16 b18a 5105 5796  `HP...%.....Q.W.
+00006cb0: 2bbf 7e05 8ea9 bf44 fa9b d7cb d7de 8a80  +.~....D........
+00006cc0: c1c3 4dd2 d7e2 4571 3eb4 f3b4 fce8 6dbc  ..M...Eq>.....m.
+00006cd0: 6ec0 92f7 b93d e3a4 6dd9 ce9c 38e1 204b  n....=..m...8. K
+00006ce0: d4ea 731c 3d95 2512 0683 58b8 b689 ca8e  ..s.=.%...X.....
+00006cf0: e062 771e f749 1d7a 6710 9876 5f5d 6f41  .bw..I.zg..v_]oA
+00006d00: cea4 39cf d112 dc7c 193c fe1e ee25 e655  ..9....|.<...%.U
+00006d10: 9cce e3ce 193b 6d0c 78b8 9d41 ae4f 54ae  .....;m.x..A.OT.
+00006d20: dda9 5cfc 916f 37ea cc89 c331 4dc3 afee  ..\..o7....1M...
+00006d30: 056f 7ee0 1b8e e471 cb7e c611 8742 7ce3  .o~....q.~...B|.
+00006d40: dadd ab18 29c3 3304 db71 1325 070e 114a  ....).3..q.%...J
+00006d50: 8385 67bb afd6 b4dc 9ef0 6771 d0d3 1416  ..g.......gq....
+00006d60: 698f 3e21 6cf4 6920 728b 0809 1178 7ace  i.>!l.i r....xz.
+00006d70: cc5b 38ce 9038 0abe 670c e13e 3673 ded3  .[8..8..g..>6s..
+00006d80: 2084 1f82 22a4 a13e 3a79 bd5d 10d1 8e6b   ..."..>:y.]...k
+00006d90: 8f6b b76e 2b7a 7856 8ebb 7943 dc0b 071d  .k.n+zxV..yC....
+00006da0: 212f 8da1 ace9 794e c681 4c4d cf38 6167  !/....yN..LM.8ag
+00006db0: d306 4e00 0d71 1643 94bf de8b 425e b9b9  ..N..q.C....B^..
+00006dc0: 53fb 6ebd ba7d 3738 4ffc e151 c74c 3959  S.n..}78O..Q.L9Y
+00006dd0: c787 5e8a e3a5 6c29 0dfc 38f9 3a86 cc1a  ..^...l)..8.:...
+00006de0: 1777 72c4 294f a900 a6ec a377 2931 8400  .wr.)O.....w)1..
+00006df0: 6ae7 2e25 8d51 712c e4b6 4663 14d3 15ae  j..%.Qq,..Fc....
+00006e00: 162c 53e8 28e3 0873 2879 2c67 f692 17e1  .,S.(..s(y,g....
+00006e10: 5312 c226 8d2c 4e11 5b97 3b3e b10c b2ea  S..&.,N.[.;>....
+00006e20: 3889 eb5b 1937 ebb8 869b 6948 9e57 c810  8..[.7....iH.W..
+00006e30: 99ec a80d 6451 496b 543c 4a5e 6324 c4fc  ....dQIkT<J^c$..
+00006e40: a931 c86e b540 95cd b5ca ea43 24dd 2256  .1.n.@.....C$."V
+00006e50: 0425 8ce3 1846 669d 3f6f 8cd9 feac 9b86  .%...Ff.?o......
+00006e60: decd d99e 2f66 3fb1 d4b2 35d0 ecee 5c16  ..../f?...5...\.
+00006e70: d14d 6ae4 701a 8ef3 59e0 6a22 2126 0004  .Mj.p...Y.j"!&..
+00006e80: 8891 6def 20aa aab1 02c7 9d3c ac80 3a38  ..m. ......<..:8
+00006e90: 2eba 738e 9805 1a26 edc1 d682 4bd8 b9e9  ..s....&....K...
+00006ea0: 2d8f e276 08a2 4774 ebf6 1e40 5ed2 68de  -..v..Gt...@^.h.
+00006eb0: 1eba f2d2 5a79 fd22 6f0b f0fa 8848 8b10  ....Zy."o....H..
+00006ec0: 3627 41dd cb37 1ee3 000c 2bba 58d4 d71f  6'A..7....+.X...
+00006ed0: c545 36e4 e670 1fdb 98f2 5deb 1427 0934  .E6..p....]..'.4
+00006ee0: 4196 41e5 4772 e635 6416 1c91 9e71 d2f6  A.A.Gr.5d....q..
+00006ef0: ec22 1422 8e18 f9e0 95d5 1b15 f6ec 7f5a  ."."...........Z
+00006f00: 2676 9cb4 7ddc 7586 e4ea 4900 7114 958b  &v..}.u...I.q...
+00006f10: 2fe0 996a 49c7 2a84 670f 8a40 c053 2f64  /..jI.*.g..@.S/d
+00006f20: f4cd bf82 25ac 26cb 4c36 43b8 40b0 758a  ....%.&.L6C.@.u.
+00006f30: 4065 5242 e5c7 6a69 e3e1 03aa f3d2 2e28  @eRB..ji.......(
+00006f40: cbad 0263 f161 2864 c986 3366 2c79 44e1  ...c.a(d..3f,yD.
+00006f50: f2b0 f306 d137 be13 7e1d 0fad ba34 01ed  .....7..~....4..
+00006f60: 9098 a04d 3183 9984 2d6a da13 302a dde6  ...M1...-j..0*..
+00006f70: 7367 14e7 921a 43a7 6f3d 51f2 050a 2d5f  sg....C.o=Q...-_
+00006f80: 940c e33c 535d c333 1553 a31d 3451 9b8c  ...<S].3.S..4Q..
+00006f90: 078a 0c1e ad48 c2b8 b309 9f53 d98a 78af  .....H.....S..x.
+00006fa0: 83b8 0aeb 9e16 b68b 986a 049d 2e09 fbcb  .........j......
+00006fb0: 18ce 4f45 6eb3 de3b c425 1544 5882 f337  ..OEn..;.%.DX..7
+00006fc0: 78bd 48f2 2d1b e42a a7ad 6d3f bb6e 700d  x.H.-..*..m?.np.
+00006fd0: c109 216c 8d01 0e13 78d8 0caf 56b9 5d61  ..!l....x...V.]a
+00006fe0: dba5 ab8c e56a b61d 72e9 b46c a696 b18d  .....j..r..l....
+00006ff0: c309 de48 2dd3 a3a8 6ebf 4210 8f67 6b93  ...H-...n.B..gk.
+00007000: 84e1 3378 3cc6 a356 103b 5eb1 d393 222d  ..3x<..V.;^..."-
+00007010: 5fbd cc98 a14f 6003 0d38 86cd 1cb5 862f  _....O`..8...../
+00007020: d770 2988 0b13 d946 9477 6e02 711c 6224  .p)....F.wn.q.b$
+00007030: 5730 9da2 58a3 15e2 93b6 78a8 0ae6 1a72  W0..X.....x....r
+00007040: 6aac c193 5913 f575 452e 702b 7a74 e3b1  j...Y..uE.p+zt..
+00007050: ff9e 061d 37eb ce38 16fa 6dbd 3d69 0f3d  ....7..8..m.=i.=
+00007060: e86f b96f 295f 4486 ca77 c864 235c 9109  .o.o)_D..w.d#\..
+00007070: 8422 09cf 0805 4638 1bf5 3659 79a9 4521  ."....F8..6Yy.E!
+00007080: 2a35 1e87 4acf a9dd 2544 843b 8ff4 df70  *5..J...%D.;...p
+00007090: fb57 0a68 c4b7 7374 1fb5 b215 2cac b4ab  .W.h..st....,...
+000070a0: 32c3 67ac 59ec e568 60e8 c755 915d d25a  2.g.Y..h`..U.].Z
+000070b0: f1c0 d6cf cd6c 0979 96f8 a5d7 3bb5 b953  .....l.y....;..S
+000070c0: 5e5e 5b48 5db9 df4b 70f6 42cf 53a1 946b  ^^[H]..Kp.B.S..k
+000070d0: 71f9 e92a 4f70 138b a1d8 9f51 babd c73b  q..*Op.....Q...;
+000070e0: 25c2 40f6 0c42 1909 f9a5 f585 5d93 5e2a  %.@..B......].^*
+000070f0: 7233 0582 2d6c 04a9 3e29 9f40 a74d 310f  r3..-l..>).@.M1.
+00007100: 841f d61e 2fe7 dc56 bc8f 9897 839d 9e70  ..../..V.......p
+00007110: 77f3 691a 2390 c9b4 2aef 2e8e 44a4 b391  w.i.#...*...D...
+00007120: 943b 6171 c812 74eb 76b0 b353 79b9 0227  .;aq..t.v..Sy..'
+00007130: 5e83 0a0a 82bd 37f6 3822 ead0 cc93 238c  ^.....7.8"....#.
+00007140: 4f46 d30e 0ab0 2f9a b549 0605 4a5a 2e20  OF..../..I..JZ. 
+00007150: 2a77 f0dc 964a 6a65 1285 1b19 a861 866e  *w...Jje.....a.n
+00007160: 431d 845d 64d2 7595 4587 5dd4 2eb9 b0af  C..]d.u.E.].....
+00007170: 966d a7c3 8ce3 a835 57cb b040 dcd2 8655  .m.....5W..@...U
+00007180: 9fbe 463c 31b1 9b52 1193 1e0f 8e61 baee  ..F<1..R.....a..
+00007190: 0371 23dd d818 3ace a949 24e3 9881 285f  .q#...:..I$...(_
+000071a0: 41e4 f2bb e0db afe1 26c4 5b37 d718 6c85  A.......&.[7..l.
+000071b0: b378 214d 046a 64d0 e398 5b4a f978 5ec0  .x!M.jd...[J.x^.
+000071c0: 3886 5b5b d4d4 c908 9c08 cb5e 7801 cce5  8.[[.......^x...
+000071d0: 575b 9828 c183 27ed e1af 47ea e68d 8994  W[.(..'...G.....
+000071e0: e722 d115 c9bf f4b9 b7f2 f2f5 ead2 325c  ."............2\
+000071f0: bdf2 b507 1843 1cf5 311b cf45 5a8e 327f  .....C..1..EZ.2.
+00007200: 423e 0339 6cec 1d4f 16c4 81a9 06a8 89cd  B>.9l..O........
+00007210: b0ab 9dc5 9d69 1615 7be8 3bc8 559e 017d  .....i..{.;.U..}
+00007220: df85 9e93 6d24 ce1a fc70 1beb 3165 9385  ....m$...p..1e..
+00007230: 5735 a172 5012 f503 be8b 8aa1 e129 107d  W5.rP........).}
+00007240: 0856 c558 f781 b3cd f02b 8fb1 41dc 313b  .V.X.....+..A.1;
+00007250: 4e25 c285 9a48 5f23 d6b9 0f2a db0f 83ee  N%...H_#...*....
+00007260: 0369 fb11 d2fd 8c3e 1e35 e57d 1615 da46  .i.....>.5.}...F
+00007270: 0864 1fa8 db0c a446 fc2a fe04 80b8 45d1  .d.....F.*....E.
+00007280: fb1a 22be 6df9 58f9 44e0 334e 3bd6 6611  ..".m.X.D.3N;.f.
+00007290: e395 2e04 8f7b 48bc de04 c14b 770b e632  .....{H....Kw..2
+000072a0: 2182 0547 e1e6 ed24 5c7a eb9e 8075 ed17  !..G...$\z...u..
+000072b0: 70b4 4590 4d12 795c 3c2c 2947 3e60 21e8  p.E.M.y\<,)G>`!.
+000072c0: e661 c0ca 216b 3704 171a a7e4 785e 744d  .a..!k7.....x^tM
+000072d0: 6a1b 7124 2aa7 b82c c20a f4d2 8e1c c648  j.q$*..,.......H
+000072e0: 3ed3 1808 13ab 2316 95c5 4dfd 2d89 7ba2  >.....#...M.-.{.
+000072f0: e4ef 0b79 18e7 4950 0f5e f522 eea6 5ef7  ...y..IP.^."..^.
+00007300: d416 3f89 1f51 5329 963f e271 9dff 0a13  ..?..QS).?.q....
+00007310: ae89 818e 5ab4 8271 4ddb 76ce 2697 67b1  ....Z..qM.v.&.g.
+00007320: bbac 2d5c 5619 e022 5828 e782 f259 b5de  ..-\V.."X(...Y..
+00007330: eaa4 491f cf0c 6328 320f 8917 ec5e c5af  ..I...c(2....^..
+00007340: 87ff 88b1 e52d 4b18 4697 e8e3 103c fb1b  .....-K.F....<..
+00007350: 6a93 30f3 8395 2de4 ce04 6f9e d4ee e02e  j.0...-...o.....
+00007360: 0449 e219 c6b3 a896 2ffc a3fa fe48 ddea  .I....../....H..
+00007370: 1992 7b25 4fec 85a5 4689 055f fe10 7361  ..{%O...F.._..sa
+00007380: 0e07 34da 732d 6d57 e1e9 83b0 3311 24cd  ..4.s-mW....3.$.
+00007390: 75b2 be14 c5c7 1eca 1de9 ff3f dc0e 96ef  u..........?....
+000073a0: 3229 5eec 6ad6 36d9 220a b574 ab79 048b  2)^.j.6."..t.y..
+000073b0: 0483 0b2f 7094 082f 90e9 4b8b d618 b471  .../p../..K....q
+000073c0: bf4a dcd4 2203 90e7 4608 5889 4841 5d7b  .J.."...F.X.HA]{
+000073d0: 70f1 240e 17b3 6e4d bf3d c1ae ab29 bb5f  p.$...nM.=...)._
+000073e0: d46a deca 2351 ed92 d138 d5d9 1fd5 ede8  .j..#Q...8......
+000073f0: a438 6b5e fff9 e01c 1fce 8b17 d1c9 6cfa  .8k^..........l.
+00007400: c7bd e0f9 433e e169 bc94 4be1 7055 a87b  ....C>.i..K.pU.{
+00007410: ae90 75e7 6d66 a994 c4a9 2c2c 22a1 c849  ..u.mf....,,"..I
+00007420: 80ba d787 2346 cf2b 21be 3e3d eb96 3c31  ....#F.+!.>=..<1
+00007430: 4be4 753f eac0 2fdf 85f9 085e 3cc5 851e  K.u?../....^<...
+00007440: 1ef7 1736 5e51 f6c5 f136 c250 e68c 6dc0  ...6^Q...6.P..m.
+00007450: 88cb 37de 8598 14d2 4627 44c3 3616 9804  ..7.....F'D.6...
+00007460: 39ec ccb8 7bcc 6af3 7a72 6238 8e05 870d  9...{.j.zrb8....
+00007470: 7897 50cd 7fcc fb70 d51b d0dd 16ac e319  x.P....p........
+00007480: d0e0 010a 1542 5471 2d43 8b48 6d60 5510  .....BTq-C.Hm`U.
+00007490: 31f1 da61 3d82 2848 74c8 fd70 91a4 f300  1..a=.(Ht..p....
+000074a0: d6fd 190c bce6 9ea0 08c1 8ac3 b5e8 5d59  ..............]Y
+000074b0: 1e59 b8a5 d05d 17dc 33b0 84db 6fe1 a5a5  .Y...]..3...o...
+000074c0: 6434 21a3 932e d145 8399 3a64 f50d 9a48  d4!....E..:d...H
+000074d0: 5688 06b3 936e 35d6 6438 1d39 8d0c c306  V....n5.d8.9....
+000074e0: 2c07 6aad 3dce e11b d58f 7058 0945 8d9f  ,.j.=.....pX.E..
+000074f0: a6b9 581d 9a0e 5ed3 04b2 f8d4 e104 8f29  ..X...^........)
+00007500: 7a0e c136 8e06 ad98 d137 621c a1d2 255e  z..6.....7b...%^
+00007510: 7655 b870 9c57 fb7e 3d38 7b99 5967 a79d  vU.p.W.~=8{.Yg..
+00007520: 9c4c 47a8 07c3 70a7 9771 54e4 d9ea eedb  .LG...p..qT.....
+00007530: 5bd8 0c32 f9b0 d1c3 87da d927 fc65 3e26  [..2.......'.e>&
+00007540: dbc7 98d6 bc53 1e4d d369 8d30 dc15 6ab1  .....S.M.i.0..j.
+00007550: a91d ac16 4f33 08a1 2347 9c4e c953 002d  ....O3..#G.N.S.-
+00007560: 8e3d d34e 3b2a 7951 508b 239c 6dba d6d1  .=.N;*yQP.#.m...
+00007570: f423 2d8e c8f4 d233 57ae 232a 2b2b 78f0  .#-....3W.#*++x.
+00007580: 23a3 13c7 ccf9 6844 c08b 5a7c b281 93d8  #.....hD..Z|....
+00007590: 5452 5502 b650 466d a042 c20e 72ba 1250  TRU..PFm.B..r..P
+000075a0: 4582 46cd 8588 9085 4bf0 32a6 0a56 318f  E.F.....K.2..V1.
+000075b0: 17ec 8da9 0ecd 5b34 b147 5dba 5276 328e  ......[4.G].Rv2.
+000075c0: 7dd0 754f c998 bbdd bcfb 6e90 e5a6 796d  }.uO......n...ym
+000075d0: ebe1 261f c456 97bb 13ee e2cb a4cc 84d8  ..&..V..........
+000075e0: 3089 0bb7 c215 b9b2 1e1f 54e4 da74 1216  0.........T..t..
+000075f0: f82f 91b7 eb22 99a2 cdc1 d45d 18e2 0d5c  ./...".....]...\
+00007600: 5c62 ce02 83cd fb8c 4d09 5edc e752 5e75  \b......M.^..R^u
+00007610: b9ec 8d5c 57b2 41c1 d95e bcec 041c 9a78  ...\W.A..^.....x
+00007620: d9a8 7b9a 3855 e293 10f1 4271 d262 1bc7  ..{.8U....Bq.b..
+00007630: dc6c d62c 1267 6aba 68e6 3d13 9e2b 7dcf  .l.,.gj.h.=..+}.
+00007640: e5e4 c448 1c95 6ea6 4f0e 9f34 a6bf 9822  ...H..n.O..4..."
+00007650: 6ed0 e420 5ffe b99b 2de5 6cbc a9db d9a9  n.. _...-.l.....
+00007660: 71f2 464d cf37 06e9 c651 964f 701f a0a8  q.FM.7...Q.Op...
+00007670: fb7a 1851 1a4a ce7d 8543 7011 8738 a771  .z.Q.J.}.Cp..8.q
+00007680: aa41 5fba 91ce 67dd 3b4c a00c 4f12 9cc2  .A_...g.;L..O...
+00007690: f906 76a4 3a9e 4620 a096 e275 08f8 a084  ..v.:.F ...u....
+000076a0: 9592 4c25 1b3d 54fd f8c5 f8d2 1129 7d1c  ..L%.=T......)}.
+000076b0: 8fe5 5627 0e37 fc97 787f 9f8a d7fc 07f1  ..V'.7..x.......
+000076c0: 5438 78cf d64d 8967 cb75 95a2 e100 7dbe  T8x..M.g.u....}.
+000076d0: 5d22 950d b595 22d3 c738 e166 c5f6 c298  ]"...."..8.f....
+000076e0: a41f fe38 2e5e eed7 d025 eb74 7435 1a32  ...8.^...%.tt5.2
+000076f0: 5d37 1b6a 2b5b d175 ccc6 cebc 284f af91  ]7.j+[.u....(O..
+00007700: 96eb 9b78 3959 4325 03a9 a359 8394 2152  ...x9YC%...Y..!R
+00007710: 8754 0f7a 022f 7fdb 2d68 5430 2da8 6b22  .T.z./..-hT0-.k"
+00007720: 6ad5 994e f221 f132 4f2a 49f6 ca07 d1b0  j..N.!.2O*I.....
+00007730: 5555 ea68 6d36 6588 8c34 656a c337 4526  UU.hm6e..4ej.7E&
+00007740: c303 adf8 6408 abb9 ccd9 b06a d044 2603  ....d......j.D&.
+00007750: ce9a 98c9 2227 a308 9ee5 0a9c 490d 117c  ...."'......I..|
+00007760: 5a42 469a ae5f f916 ff90 f816 8e48 b74b  ZBF.._.......H.K
+00007770: 844a 20a4 3e0a 89ad 0ea7 6786 1295 243c  .J .>.....g...$<
+00007780: 81ee 2989 2d89 7af8 6186 30c0 62b2 33ec  ..).-.z.a.0.b.3.
+00007790: 09a9 8a42 3134 4d0d 8ec2 0e8b 2f15 a805  ...B14M...../...
+000077a0: 9a41 1407 49c4 a236 e31e 4750 134f 022f  .A..I..6..GP.O./
+000077b0: 9b40 4943 1f43 660d 9e4b 979a c1ee 92f6  .@IC.Cf..K......
+000077c0: 88a4 2574 b8f9 305a 02c6 58de 625d 8d42  ..%t..0Z..X.b].B
+000077d0: 33d6 b89e 3ce8 f9f8 429e 4875 949f 5f52  3...<...B.Hu.._R
+000077e0: 0bf5 a84b 0f53 27c5 f706 ea29 912d a187  ...K.S'....).-..
+000077f0: 9083 a2f0 7e96 4fc3 b8e2 7e18 9663 9c92  ....~.O...~..c..
+00007800: a96e c52a 81b4 21e2 d424 b7e2 c8d2 76c4  .n.*..!..$....v.
+00007810: 0cb9 093b 8a67 9d40 d534 e2b5 fb26 2da1  ...;.g.@.4...&-.
+00007820: 6d32 816c c364 3205 c706 6dff b48d c7f9  m2.l.d2...m.....
+00007830: 050b 71e9 ad5d 0e4a 6ef3 6d5b 90c9 75da  ..q..].Jn.m[..u.
+00007840: 3e99 8244 dc93 7b2f 32f7 b6dd 0799 f586  >..D..{/2.......
+00007850: ed93 2948 94ae 5f9b 0ab9 879d b1c6 fb20  ..)H.._........ 
+00007860: b4d1 3291 d24f 7006 8e98 87d2 4f49 e57e  ..2..Op.....OI.~
+00007870: e64e 62eb 645a 354d 1962 f1f4 1bbc 5d71  .Nb.dZ5M.b....]q
+00007880: 86a8 1694 e364 fd52 6781 ea9c 5107 3366  .....d.Rg...Q.3f
+00007890: faf8 2095 7017 eda2 e392 33a8 297c 4f02  .. .p.....3.)|O.
+000078a0: 1949 2250 1cae 343a 44c7 c527 268e d959  .I"P..4:D..'&..Y
+000078b0: 078b e9bc 9624 854f 7c1f 5404 b3a5 a79b  .....$.O|.T.....
+000078c0: 117c 8e9a 4a3a 1064 b217 f0b1 4e64 34aa  .|..J:.d....Nd4.
+000078d0: ded1 144f e9f7 751a ed81 4e0e 9fd9 0f2c  ...O..u...N....,
+000078e0: aed2 7188 0ffe 2104 f1fe bdfa 9ec2 c19f  ..q...!.........
+000078f0: c11f 1eff e477 c3f5 3b7d 5941 3910 63e2  .....w..;}YA9.c.
+00007900: 937c 59f2 21b3 3d95 86d8 597e 69d3 c79a  .|Y.!.=...Y~i...
+00007910: bf74 bf34 4204 ca1f 212e 993b 960c a0fa  .t.4B...!..;....
+00007920: c182 5eca 95b2 98c2 54a3 e58b 7902 2091  ..^.....T...y. .
+00007930: 0a09 2091 71e1 0144 9793 c910 bb5f 0264  .. .q..D....._.d
+00007940: 7c39 46c7 233e 60a8 8816 5a8e 2717 31d5  |9F.#>`...Z.'.1.
+00007950: 5c43 ee9e 2527 c2ca 3197 b4c5 e6ba 251d  \C..%'..1.....%.
+00007960: 1ccc 3ec8 8836 d713 521f ec84 4875 9634  ..>..6..R...Hu.4
+00007970: 2147 cc10 a163 1def 9a90 2379 a3ab 9b0c  !G...c....#y....
+00007980: 8d62 9c32 11c3 900c 89e3 6c4a 9cc3 b4b7  .b.2......lJ....
+00007990: 568a dcd0 699e 90b9 8267 488a 20ea 21f4  V...i....gH. .!.
+000079a0: eea9 6c53 af0c 8a06 4216 3957 a590 d514  ..lS....B.9W....
+000079b0: e053 f7d3 6480 58c8 d098 8269 c7b9 4a02  .S..d.X....i..J.
+000079c0: e31a c13c 8998 67ee 5e18 3d9b 6370 0cfd  ...<..g.^.=.cp..
+000079d0: 2230 2202 42da e087 acd4 0512 7495 e11e  "0".B.......t...
+000079e0: 586d a6f5 40c8 b508 a3e8 ba3d 0382 4dcc  Xm..@......=..M.
+000079f0: 2650 84a0 065d 937e 6d69 24fc ce53 bc4d  &P...].~mi$..S.M
+00007a00: bddc 18a6 9bca 51f9 49b7 cff0 9d29 ac7a  ......Q.I....).z
+00007a10: ee69 127d 8cd7 8b2b a088 e38a 03fa f696  .i.}...+........
+00007a20: 3b69 3a1a 312a ba42 4e89 0c5f 71e7 6f1a  ;i:.1*.BN.._q.o.
+00007a30: 5f40 3686 b0f8 e39a 1791 fb1e 200c 23eb  _@6......... .#.
+00007a40: 7824 283a 2013 dd8d e308 69d2 cff3 2294  x$(: .....i...".
+00007a50: ab9e 4534 a669 804c c630 6971 ecc5 44b6  ..E4.i.L.0iq..D.
+00007a60: a588 72ea 5aaa c833 0ed6 d896 536c 4b1c  ..r.Z..3....SlK.
+00007a70: ab1a befd b738 03f0 6d5a b6d8 638b 5514  .....8..mZ..c.U.
+00007a80: 52e2 78cf ef91 c828 9a6e 6630 01aa fd82  R.x....(.nf0....
+00007a90: b60a 2fe9 f029 e7bc 8d5a 7dbc a38d 8848  ../..)...Z}....H
+00007aa0: 3300 a189 c1d4 71b0 1397 c938 4888 29eb  3.....q....8H.).
+00007ab0: 3261 e23d e35c da45 929e c8e7 b68b 2933  2a.=.\.E......)3
+00007ac0: 7fca 1032 223b e651 f1ad c969 1b5f f76b  ...2";.Q...i._.k
+00007ad0: e3c1 8254 a18f bcc5 5ede 7e51 fee5 3e7f  ...T....^.~Q..>.
+00007ae0: 356c c2c9 ca4b 3c9f e09e 397f cd06 8ffb  5l...K<...9.....
+00007af0: f7c5 296f 5eb4 d7de 651d 2077 ed13 ae79  ..)o^...e. w...y
+00007b00: 35ef 73d7 8fc9 13ee ed71 d7a6 1370 ef01  5.s......q...p..
+00007b10: 8f1e 7e27 b4e1 ae08 2780 abf0 9614 51f3  ..~'....'.....Q.
+00007b20: 821e 520d e43d 63dc 5f1a c97b bee3 cb8f  ..R..=c._..{....
+00007b30: 4126 4877 df4d f96e 059d 07e8 bafd e692  A&Hw.M.n........
+00007b40: 21f0 c58b 388b 126b 87ee 92ab 9ae0 11f6  !...8..k........
+00007b50: 6914 0d1f b648 54dd fd5f 216b addc f8e6  i....HT.._!k....
+00007b60: 0979 de1f f752 77df e039 d317 ea47 e3f2  .y...Rw..9...G..
+00007b70: 07f3 b6bb 4cd1 6f5e be9b 2aa5 3c27 ed88  ....L.o^..*.<'..
+00007b80: d385 f0e5 f694 7ab9 1db7 ad71 bdc0 111f  ......z....q....
+00007b90: fe24 db05 7c3a 857c 7402 ef7c 887b 43fb  .$..|:.|t..|.{C.
+00007ba0: b82b a50e de23 d791 ead7 ec89 c2a1 bf9e  .+...#..........
+00007bb0: f87c 1679 678f 96db bd30 76bc 8474 2824  .|.yg....0v..t($
+00007bc0: 6d88 a4ae 0919 1967 3aa1 5fe1 88de d652  m......g:._....R
+00007bd0: 99c6 eddd 2d6b 27e1 9823 808c 720f 01ef  ....-k'..#..r...
+00007be0: 7bb9 4d97 f24c 2960 3e1c 021b 2cee c4af  {.M..L)`>...,...
+00007bf0: 8817 99b5 17c3 c2ec 58e7 bfb1 51d3 cda9  ........X...Q...
+00007c00: 8407 fadb 9d96 78b2 775c bcb0 ab7d b6f7  ......x.w\...}..
+00007c10: 0496 a671 fbb4 da29 aafd 14e8 31c6 95af  ...q...)....1...
+00007c20: 4fc6 cbbc 539b f82e 73fb f021 64ab 5768  O...S...s..!d.Wh
+00007c30: 69f4 9ff1 1898 408f 782e 09d1 9ef6 7cdf  i.....@.x.....|.
+00007c40: 3127 0df9 60f1 df03 7ed8 f3fc a3ff 0700  1'..`...~.......
+00007c50: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00007c60: 0021 003b 6d32 4bc1 0000 0042 0100 0023  .!.;m2K....B...#
+00007c70: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00007c80: 2f5f 7265 6c73 2f73 6865 6574 312e 786d  /_rels/sheet1.xm
+00007c90: 6c2e 7265 6c73 848f c18a c230 1445 f703  l.rels.....0.E..
+00007ca0: fe43 787b 93d6 850c 4353 3722 b855 e703  .Cx{....CS7".U..
+00007cb0: 62fa da06 db97 90f7 14fd 7bb3 1c65 c0e5  b.........{..e..
+00007cc0: e570 cfe5 369b fb3c a91b 660e 912c d4ba  .p..6..<..f..,..
+00007cd0: 0285 e463 1768 b0f0 7bda 2dbf 41b1 38ea  ...c.h..{.-.A.8.
+00007ce0: dc14 092d 3c90 61d3 2ebe 9a03 4e4e 4a89  ...-<.a.....NNJ.
+00007cf0: c790 5815 0bb1 8551 24fd 18c3 7ec4 d9b1  ..X....Q$...~...
+00007d00: 8e09 a990 3ee6 d949 8979 30c9 f98b 1bd0  ....>..I.y0.....
+00007d10: acaa 6a6d f25f 07b4 2f4e b5ef 2ce4 7d57  ..jm._../N..,.}W
+00007d20: 833a 3d52 59fe ec8e 7d1f 3c6e a3bf ce48  .:=RY...}.<n...H
+00007d30: f2cf 8449 3990 603e a248 39c8 45ed f280  ...I9.`>.H9.E...
+00007d40: 6241 eb77 f69e 6b7d 0e04 a66d cccb f3f6  bA.w..k}...m....
+00007d50: 0900 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00007d60: 0000 0021 0013 c42c 13c2 0000 0042 0100  ...!...,.....B..
+00007d70: 0023 0000 0078 6c2f 776f 726b 7368 6565  .#...xl/workshee
+00007d80: 7473 2f5f 7265 6c73 2f73 6865 6574 322e  ts/_rels/sheet2.
+00007d90: 786d 6c2e 7265 6c73 848f c16a c330 1044  xml.rels...j.0.D
+00007da0: ef85 fc83 d87b 243b 8750 8a25 5f4a 21d7  .....{$;.P.%_J!.
+00007db0: 26fd 0045 5edb a2f6 4a68 b725 f9fb e8d8  &..E^...Jh.%....
+00007dc0: 8442 8ec3 63de 305d 7f59 17f5 8b85 6322  .B..c.0].Y....c"
+00007dd0: 0bad 6e40 2185 3444 9a2c 7c9d 3eb6 afa0  ..n@!.4D.,|.>...
+00007de0: 583c 0d7e 4984 16ae c8d0 bbcd 4bf7 898b  X<.~I.......K...
+00007df0: 975a e239 6656 d542 6c61 16c9 6fc6 7098  .Z.9fV.Bla..o.p.
+00007e00: 71f5 ac53 46aa 644c 65f5 5263 994c f6e1  q..SF.dLe.Rc.L..
+00007e10: db4f 6876 4db3 37e5 af03 dc9d 531d 060b  .OhvM.7.....S...
+00007e20: e530 b4a0 4ed7 5c97 9fbb d338 c680 ef29  .0..N.\....8...)
+00007e30: fcac 48f2 cf84 c925 9260 39a2 483d c855  ..H....%.`9.H=.U
+00007e40: edcb 8462 41eb 47f6 9877 fa1c 098c ebcc  ...bA.G..w......
+00007e50: dd73 7703 0000 ffff 0300 504b 0304 1400  .sw.......PK....
+00007e60: 0600 0800 0000 2100 34a1 0992 c200 0000  ......!.4.......
+00007e70: 4201 0000 2300 0000 786c 2f77 6f72 6b73  B...#...xl/works
+00007e80: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
+00007e90: 7433 2e78 6d6c 2e72 656c 7384 8fc1 6ac3  t3.xml.rels...j.
+00007ea0: 3010 44ef 81fc 83d8 7b24 2785 5282 e55c  0.D.....{$'.R..\
+00007eb0: 4220 d736 fd00 555e cb22 f64a 68b7 a5f9  B .6..U^.".Jh...
+00007ec0: fbea 589b 428f c363 de30 ede9 7b9e d417  ..X.B..c.0..{...
+00007ed0: 168e 892c ec75 030a c9a7 3e52 b0f0 7ebb  ...,.u....>R..~.
+00007ee0: ec5e 40b1 38ea dd94 082d 3c90 e1d4 6d37  .^@.8....-<...m7
+00007ef0: ed2b 4e4e 6a89 c798 5955 0bb1 8551 241f  .+NNj...YU...Q$.
+00007f00: 8d61 3fe2 ec58 a78c 54c9 90ca eca4 c612  .a?..X..T.......
+00007f10: 4c76 feee 029a 43d3 3c9b f2db 01dd c2a9  Lv....C.<.......
+00007f20: aebd 8572 edf7 a06e 8f5c 97ff 77a7 6188  ...r...n.\..w.a.
+00007f30: 1ecf c97f ce48 f2c7 84c9 2592 6079 4391  .....H....%.`yC.
+00007f40: 7a90 abda 9580 6241 eb35 5be7 27fd 1109  z.....bA.5[.'...
+00007f50: 4cd7 9ac5 f3ee 0700 00ff ff03 0050 4b03  L............PK.
+00007f60: 0414 0006 0008 0000 0021 0043 9611 a3c2  .........!.C....
+00007f70: 0000 0042 0100 0023 0000 0078 6c2f 776f  ...B...#...xl/wo
+00007f80: 726b 7368 6565 7473 2f5f 7265 6c73 2f73  rksheets/_rels/s
+00007f90: 6865 6574 342e 786d 6c2e 7265 6c73 848f  heet4.xml.rels..
+00007fa0: c16a c330 1044 ef81 fc83 d87b 2427 9452  .j.0.D.....{$'.R
+00007fb0: 82e5 5c42 20d7 36fd 0055 5ecb 22f6 4a68  ..\B .6..U^.".Jh
+00007fc0: b7a5 f9fb ea58 9b42 8fc3 63de 30ed e97b  .....X.B..c.0..{
+00007fd0: 9ed4 1716 8e89 2cec 7503 0ac9 a73e 52b0  ......,.u....>R.
+00007fe0: f07e bbec 5e40 b138 eadd 9408 2d3c 90e1  .~..^@.8....-<..
+00007ff0: d46d 37ed 2b4e 4e6a 89c7 9859 550b b185  .m7.+NNj...YU...
+00008000: 5124 1f8d 613f e2ec 58a7 8c54 c990 caec  Q$..a?..X..T....
+00008010: a4c6 124c 76fe ee02 9a43 d33c 9bf2 db01  ...Lv....C.<....
+00008020: ddc2 a9ae bd85 72ed f7a0 6e8f 5c97 ff77  ......r...n.\..w
+00008030: a761 881e cfc9 7fce 48f2 c784 c925 9260  .a......H....%.`
+00008040: 7943 917a 90ab da95 8062 41eb 355b e727  yC.z.....bA.5[.'
+00008050: fd11 094c d79a c5f3 ee07 0000 ffff 0300  ...L............
+00008060: 504b 0304 1400 0600 0800 0000 2100 64f3  PK..........!.d.
+00008070: 3422 c200 0000 4201 0000 2300 0000 786c  4"....B...#...xl
+00008080: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
+00008090: 732f 7368 6565 7435 2e78 6d6c 2e72 656c  s/sheet5.xml.rel
+000080a0: 7384 8fc1 6ac3 3010 44ef 81fc 83d8 7b24  s...j.0.D.....{$
+000080b0: 27d0 5282 e55c 4220 d736 fd00 555e cb22  '.R..\B .6..U^."
+000080c0: f64a 68b7 a5f9 fbea 589b 428f c363 de30  .Jh.....X.B..c.0
+000080d0: ede9 7b9e d417 168e 892c ec75 030a c9a7  ..{......,.u....
+000080e0: 3e52 b0f0 7ebb ec5e 40b1 38ea dd94 082d  >R..~..^@.8....-
+000080f0: 3c90 e1d4 6d37 ed2b 4e4e 6a89 c798 5955  <...m7.+NNj...YU
+00008100: 0bb1 8551 241f 8d61 3fe2 ec58 a78c 54c9  ...Q$..a?..X..T.
+00008110: 90ca eca4 c612 4c76 feee 029a 43d3 3c9b  ......Lv....C.<.
+00008120: f2db 01dd c2a9 aebd 8572 edf7 a06e 8f5c  .........r...n.\
+00008130: 97ff 77a7 6188 1ecf c97f ce48 f2c7 84c9  ..w.a......H....
+00008140: 2592 6079 4391 7a90 abda 9580 6241 eb35  %.`yC.z.....bA.5
+00008150: 5be7 27fd 1109 4cd7 9ac5 f3ee 0700 00ff  [.'...L.........
+00008160: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00008170: 00e8 f726 32a9 0100 0054 0f00 0027 0000  ...&2....T...'..
+00008180: 0078 6c2f 7072 696e 7465 7253 6574 7469  .xl/printerSetti
+00008190: 6e67 732f 7072 696e 7465 7253 6574 7469  ngs/printerSetti
+000081a0: 6e67 7331 2e62 696e ec57 b94e c340 107d  ngs1.bin.W.N.@.}
+000081b0: bb36 71a2 8810 2828 517a 84c4 1104 8826  .6q...((Qz.....&
+000081c0: 1202 8906 1091 2042 2938 9282 a340 1c22  ...... B)8...@."
+000081d0: e99c 8e96 36d4 fc03 1f42 49c1 6750 61de  ....6....BI.gPa.
+000081e0: ac73 1870 0428 4713 bfd5 dad6 ceec 78fc  .s.p.(G.......x.
+000081f0: 7676 c65b 4411 3728 e30c 33b8 c335 6ed9  vv.[D.7(..3..5n.
+00008200: 8b58 c70e f2d8 c616 32d8 c706 656b 58c4  .X......2...ekX.
+00008210: 1256 b0cb 913c f5af 700a 81b2 a15f 5149  .V...<..p...._QI
+00008220: 8d3d ba8e 4202 f564 365e 8282 8382 56bc  .=..B..d6^....V.
+00008230: 1734 758c 66ef 2f62 97e6 3bda afa4 2823  .4u.f./b..;...(#
+00008240: 4429 e8c3 32e7 b8a3 c033 7b8e cfef bcbb  D)..2....3{.....
+00008250: 01f7 c661 db7f 63a0 4cb6 c221 7e09 d2f4  ...a..c.L..!~...
+00008260: a109 f141 c1e2 759a bc14 b463 0409 64e3  ...A..u....c..d.
+00008270: f5e4 14fc 26cf abd6 832d ba31 4c86 1817  ....&....-.1L...
+00008280: cbb1 d6b8 794f e3fb 9aef 0cf7 281a 8d18  ....yO......(...
+00008290: 8818 1846 0624 e3d8 ec25 b660 ae49 04c8  ...F.$...%.`.I..
+000082a0: f0bc 2033 fdca d851 fc0d 1f03 9ab1 d7ae  .. 3...Q........
+000082b0: 4c0a f36c 2f1f 83e3 41fe 427c d8b2 09c2  L..l/...A.B|....
+000082c0: 9181 ebc4 6d6a 4aeb acd6 8dd7 0d2f fca2  ....mjJ....../..
+000082d0: 6f0c 69f2 126b 7193 4e79 849e 1591 85b7  o.i..kq.Ny......
+000082e0: a898 47c9 a26b 0634 23a9 1d48 1677 5e09  ..G..k.4#..H.w^.
+000082f0: 977d da7b 3f6b 86fc 786f febe f77a b6ce  .}.{?k..xo...z..
+00008300: c7b8 c011 4e70 dec1 e21c bf7f 01d9 81c6  ....Np..........
+00008310: 5554 49ff 47f7 3dd1 ed02 1d54 750d eac9  UTI.G.=....Tu...
+00008320: e4fd c3b4 7fc6 6b9f 98be 5bff ba42 7b0d  ......k...[..B{.
+00008330: b10b 1e61 09bf 168c 98d3 5970 a682 6726  ...a......Yp..g&
+00008340: d626 5af3 7322 97f3 e627 0000 00ff ff03  .&Z.s"...'......
+00008350: 0050 4b03 0414 0006 0008 0000 0021 00e8  .PK..........!..
+00008360: f726 32a9 0100 0054 0f00 0027 0000 0078  .&2....T...'...x
+00008370: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00008380: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00008390: 7332 2e62 696e ec57 b94e c340 107d bb36  s2.bin.W.N.@.}.6
+000083a0: 71a2 8810 2828 517a 84c4 1104 8826 1202  q...((Qz.....&..
+000083b0: 8906 1091 2042 2938 9282 a340 1c22 e99c  .... B)8...@."..
+000083c0: 8e96 36d4 fc03 1f42 49c1 6750 61de ac73  ..6....BI.gPa..s
+000083d0: 1870 0428 4713 bfd5 dad6 ceec 78fc 7676  .p.(G.......x.vv
+000083e0: c65b 4411 3728 e30c 33b8 c335 6ed9 8b58  .[D.7(..3..5n..X
+000083f0: c70e f2d8 c616 32d8 c706 656b 58c4 1256  ......2...ekX..V
+00008400: b0cb 913c f5af 700a 81b2 a15f 5149 8d3d  ...<..p...._QI.=
+00008410: ba8e 4202 f564 365e 8282 8382 56bc 1734  ..B..d6^....V..4
+00008420: 758c 66ef 2f62 97e6 3bda afa4 2823 4429  u.f./b..;...(#D)
+00008430: e8c3 32e7 b8a3 c033 7b8e cfef bcbb 01f7  ..2....3{.......
+00008440: c661 db7f 63a0 4cb6 c221 7e09 d2f4 a109  .a..c.L..!~.....
+00008450: f141 c1e2 759a bc14 b463 0409 64e3 f5e4  .A..u....c..d...
+00008460: 14fc 26cf abd6 832d ba31 4c86 1817 cbb1  ..&....-.1L.....
+00008470: d6b8 794f e3fb 9aef 0cf7 281a 8d18 8818  ..yO......(.....
+00008480: 1846 0624 e3d8 ec25 b660 ae49 04c8 f0bc  .F.$...%.`.I....
+00008490: 2033 fdca d851 fc0d 1f03 9ab1 d7ae 4c0a   3...Q........L.
+000084a0: f36c 2f1f 83e3 41fe 427c d8b2 09c2 9181  .l/...A.B|......
+000084b0: ebc4 6d6a 4aeb acd6 8dd7 0d2f fca2 6f0c  ..mjJ....../..o.
+000084c0: 69f2 126b 7193 4e79 849e 1591 85b7 a898  i..kq.Ny........
+000084d0: 47c9 a26b 0634 23a9 1d48 1677 5e09 977d  G..k.4#..H.w^..}
+000084e0: da7b 3f6b 86fc 786f febe f77a b6ce c7b8  .{?k..xo...z....
+000084f0: c011 4e70 dec1 e21c bf7f 01d9 81c6 5554  ..Np..........UT
+00008500: 49ff 47f7 3dd1 ed02 1d54 750d eac9 e4fd  I.G.=....Tu.....
+00008510: c3b4 7fc6 6b9f 98be 5bff ba42 7b0d b10b  ....k...[..B{...
+00008520: 1e61 09bf 168c 98d3 5970 a682 6726 d626  .a......Yp..g&.&
+00008530: 5af3 7322 97f3 e627 0000 00ff ff03 0050  Z.s"...'.......P
+00008540: 4b03 0414 0006 0008 0000 0021 00e8 f726  K..........!...&
+00008550: 32a9 0100 0054 0f00 0027 0000 0078 6c2f  2....T...'...xl/
+00008560: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
+00008570: 7072 696e 7465 7253 6574 7469 6e67 7333  printerSettings3
+00008580: 2e62 696e ec57 b94e c340 107d bb36 71a2  .bin.W.N.@.}.6q.
+00008590: 8810 2828 517a 84c4 1104 8826 1202 8906  ..((Qz.....&....
+000085a0: 1091 2042 2938 9282 a340 1c22 e99c 8e96  .. B)8...@."....
+000085b0: 36d4 fc03 1f42 49c1 6750 61de ac73 1870  6....BI.gPa..s.p
+000085c0: 0428 4713 bfd5 dad6 ceec 78fc 7676 c65b  .(G.......x.vv.[
+000085d0: 4411 3728 e30c 33b8 c335 6ed9 8b58 c70e  D.7(..3..5n..X..
+000085e0: f2d8 c616 32d8 c706 656b 58c4 1256 b0cb  ....2...ekX..V..
+000085f0: 913c f5af 700a 81b2 a15f 5149 8d3d ba8e  .<..p...._QI.=..
+00008600: 4202 f564 365e 8282 8382 56bc 1734 758c  B..d6^....V..4u.
+00008610: 66ef 2f62 97e6 3bda afa4 2823 4429 e8c3  f./b..;...(#D)..
+00008620: 32e7 b8a3 c033 7b8e cfef bcbb 01f7 c661  2....3{........a
+00008630: db7f 63a0 4cb6 c221 7e09 d2f4 a109 f141  ..c.L..!~......A
+00008640: c1e2 759a bc14 b463 0409 64e3 f5e4 14fc  ..u....c..d.....
+00008650: 26cf abd6 832d ba31 4c86 1817 cbb1 d6b8  &....-.1L.......
+00008660: 794f e3fb 9aef 0cf7 281a 8d18 8818 1846  yO......(......F
+00008670: 0624 e3d8 ec25 b660 ae49 04c8 f0bc 2033  .$...%.`.I.... 3
+00008680: fdca d851 fc0d 1f03 9ab1 d7ae 4c0a f36c  ...Q........L..l
+00008690: 2f1f 83e3 41fe 427c d8b2 09c2 9181 ebc4  /...A.B|........
+000086a0: 6d6a 4aeb acd6 8dd7 0d2f fca2 6f0c 69f2  mjJ....../..o.i.
+000086b0: 126b 7193 4e79 849e 1591 85b7 a898 47c9  .kq.Ny........G.
+000086c0: a26b 0634 23a9 1d48 1677 5e09 977d da7b  .k.4#..H.w^..}.{
+000086d0: 3f6b 86fc 786f febe f77a b6ce c7b8 c011  ?k..xo...z......
+000086e0: 4e70 dec1 e21c bf7f 01d9 81c6 5554 49ff  Np..........UTI.
+000086f0: 47f7 3dd1 ed02 1d54 750d eac9 e4fd c3b4  G.=....Tu.......
+00008700: 7fc6 6b9f 98be 5bff ba42 7b0d b10b 1e61  ..k...[..B{....a
+00008710: 09bf 168c 98d3 5970 a682 6726 d626 5af3  ......Yp..g&.&Z.
+00008720: 7322 97f3 e627 0000 00ff ff03 0050 4b03  s"...'.......PK.
+00008730: 0414 0006 0008 0000 0021 00e8 f726 32a9  .........!...&2.
+00008740: 0100 0054 0f00 0027 0000 0078 6c2f 7072  ...T...'...xl/pr
+00008750: 696e 7465 7253 6574 7469 6e67 732f 7072  interSettings/pr
+00008760: 696e 7465 7253 6574 7469 6e67 7334 2e62  interSettings4.b
+00008770: 696e ec57 b94e c340 107d bb36 71a2 8810  in.W.N.@.}.6q...
+00008780: 2828 517a 84c4 1104 8826 1202 8906 1091  ((Qz.....&......
+00008790: 2042 2938 9282 a340 1c22 e99c 8e96 36d4   B)8...@."....6.
+000087a0: fc03 1f42 49c1 6750 61de ac73 1870 0428  ...BI.gPa..s.p.(
+000087b0: 4713 bfd5 dad6 ceec 78fc 7676 c65b 4411  G.......x.vv.[D.
+000087c0: 3728 e30c 33b8 c335 6ed9 8b58 c70e f2d8  7(..3..5n..X....
+000087d0: c616 32d8 c706 656b 58c4 1256 b0cb 913c  ..2...ekX..V...<
+000087e0: f5af 700a 81b2 a15f 5149 8d3d ba8e 4202  ..p...._QI.=..B.
+000087f0: f564 365e 8282 8382 56bc 1734 758c 66ef  .d6^....V..4u.f.
+00008800: 2f62 97e6 3bda afa4 2823 4429 e8c3 32e7  /b..;...(#D)..2.
+00008810: b8a3 c033 7b8e cfef bcbb 01f7 c661 db7f  ...3{........a..
+00008820: 63a0 4cb6 c221 7e09 d2f4 a109 f141 c1e2  c.L..!~......A..
+00008830: 759a bc14 b463 0409 64e3 f5e4 14fc 26cf  u....c..d.....&.
+00008840: abd6 832d ba31 4c86 1817 cbb1 d6b8 794f  ...-.1L.......yO
+00008850: e3fb 9aef 0cf7 281a 8d18 8818 1846 0624  ......(......F.$
+00008860: e3d8 ec25 b660 ae49 04c8 f0bc 2033 fdca  ...%.`.I.... 3..
+00008870: d851 fc0d 1f03 9ab1 d7ae 4c0a f36c 2f1f  .Q........L..l/.
+00008880: 83e3 41fe 427c d8b2 09c2 9181 ebc4 6d6a  ..A.B|........mj
+00008890: 4aeb acd6 8dd7 0d2f fca2 6f0c 69f2 126b  J....../..o.i..k
+000088a0: 7193 4e79 849e 1591 85b7 a898 47c9 a26b  q.Ny........G..k
+000088b0: 0634 23a9 1d48 1677 5e09 977d da7b 3f6b  .4#..H.w^..}.{?k
+000088c0: 86fc 786f febe f77a b6ce c7b8 c011 4e70  ..xo...z......Np
+000088d0: dec1 e21c bf7f 01d9 81c6 5554 49ff 47f7  ..........UTI.G.
+000088e0: 3dd1 ed02 1d54 750d eac9 e4fd c3b4 7fc6  =....Tu.........
+000088f0: 6b9f 98be 5bff ba42 7b0d b10b 1e61 09bf  k...[..B{....a..
+00008900: 168c 98d3 5970 a682 6726 d626 5af3 7322  ....Yp..g&.&Z.s"
+00008910: 97f3 e627 0000 00ff ff03 0050 4b03 0414  ...'.......PK...
+00008920: 0006 0008 0000 0021 00e8 f726 32a9 0100  .......!...&2...
+00008930: 0054 0f00 0027 0000 0078 6c2f 7072 696e  .T...'...xl/prin
+00008940: 7465 7253 6574 7469 6e67 732f 7072 696e  terSettings/prin
+00008950: 7465 7253 6574 7469 6e67 7335 2e62 696e  terSettings5.bin
+00008960: ec57 b94e c340 107d bb36 71a2 8810 2828  .W.N.@.}.6q...((
+00008970: 517a 84c4 1104 8826 1202 8906 1091 2042  Qz.....&...... B
+00008980: 2938 9282 a340 1c22 e99c 8e96 36d4 fc03  )8...@."....6...
+00008990: 1f42 49c1 6750 61de ac73 1870 0428 4713  .BI.gPa..s.p.(G.
+000089a0: bfd5 dad6 ceec 78fc 7676 c65b 4411 3728  ......x.vv.[D.7(
+000089b0: e30c 33b8 c335 6ed9 8b58 c70e f2d8 c616  ..3..5n..X......
+000089c0: 32d8 c706 656b 58c4 1256 b0cb 913c f5af  2...ekX..V...<..
+000089d0: 700a 81b2 a15f 5149 8d3d ba8e 4202 f564  p...._QI.=..B..d
+000089e0: 365e 8282 8382 56bc 1734 758c 66ef 2f62  6^....V..4u.f./b
+000089f0: 97e6 3bda afa4 2823 4429 e8c3 32e7 b8a3  ..;...(#D)..2...
+00008a00: c033 7b8e cfef bcbb 01f7 c661 db7f 63a0  .3{........a..c.
+00008a10: 4cb6 c221 7e09 d2f4 a109 f141 c1e2 759a  L..!~......A..u.
+00008a20: bc14 b463 0409 64e3 f5e4 14fc 26cf abd6  ...c..d.....&...
+00008a30: 832d ba31 4c86 1817 cbb1 d6b8 794f e3fb  .-.1L.......yO..
+00008a40: 9aef 0cf7 281a 8d18 8818 1846 0624 e3d8  ....(......F.$..
+00008a50: ec25 b660 ae49 04c8 f0bc 2033 fdca d851  .%.`.I.... 3...Q
+00008a60: fc0d 1f03 9ab1 d7ae 4c0a f36c 2f1f 83e3  ........L..l/...
+00008a70: 41fe 427c d8b2 09c2 9181 ebc4 6d6a 4aeb  A.B|........mjJ.
+00008a80: acd6 8dd7 0d2f fca2 6f0c 69f2 126b 7193  ...../..o.i..kq.
+00008a90: 4e79 849e 1591 85b7 a898 47c9 a26b 0634  Ny........G..k.4
+00008aa0: 23a9 1d48 1677 5e09 977d da7b 3f6b 86fc  #..H.w^..}.{?k..
+00008ab0: 786f febe f77a b6ce c7b8 c011 4e70 dec1  xo...z......Np..
+00008ac0: e21c bf7f 01d9 81c6 5554 49ff 47f7 3dd1  ........UTI.G.=.
+00008ad0: ed02 1d54 750d eac9 e4fd c3b4 7fc6 6b9f  ...Tu.........k.
+00008ae0: 98be 5bff ba42 7b0d b10b 1e61 09bf 168c  ..[..B{....a....
+00008af0: 98d3 5970 a682 6726 d626 5af3 7322 97f3  ..Yp..g&.&Z.s"..
+00008b00: e627 0000 00ff ff03 0050 4b03 0414 0006  .'.......PK.....
+00008b10: 0008 0000 0021 005b 10e8 d453 0100 0063  .....!.[...S...c
+00008b20: 0200 0011 0008 0164 6f63 5072 6f70 732f  .......docProps/
+00008b30: 636f 7265 2e78 6d6c 20a2 0401 28a0 0001  core.xml ...(...
+00008b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008c70: 0000 0000 8492 d14a c330 1885 ef05 dfa1  .......J.0......
-00008c80: e4be 4dda e1d4 d076 a0b2 2b07 8213 c5bb  ..M....v..+.....
-00008c90: 90fc db8a 4d1a 9268 b74b f175 041f c0d7  ....M..h.K.u....
-00008ca0: d10b dfc2 b4dd 6a65 8297 f9cf c997 737e  ......je......s~
-00008cb0: 924e d6b2 0c9e c0d8 a252 198a 2382 0250  .N.......R..#..P
-00008cc0: bc12 855a 66e8 663e 0d4f 5060 1d53 8295  ...Zf.f>.OP`.S..
-00008cd0: 9582 0c6d c0a2 497e 7890 724d 7965 e0ca  ...m..I~x.rMye..
-00008ce0: 541a 8c2b c006 9ea4 2ce5 3a43 2be7 34c5  T..+....,.:C+.4.
-00008cf0: d8f2 1548 6623 ef50 5e5c 5446 32e7 8f66  ...Hf#.P^\TF2..f
-00008d00: 8935 e30f 6c09 3821 648c 2538 2698 63b8  .5..l.8!d.%8&.c.
-00008d10: 0186 ba27 a22d 52f0 1ea9 1f4d d902 04c7  ...'.-R....M....
-00008d20: 5082 04e5 2c8e a318 ff78 1d18 69ff bcd0  P...,....x..i...
-00008d30: 2a03 a72c dc46 fb4e dbb8 43b6 e09d d8bb  *..,.F.N..C.....
-00008d40: d7b6 e88d 755d 47f5 a88d e1f3 c7f8 6e76  ....u]G.......nv
-00008d50: 79dd 560d 0bd5 ec8a 03ca 53c1 2937 c05c  y.V.......S.)7.\
-00008d60: 65f2 aff7 978f f7e7 cfb7 d714 0fa6 cd06  e...............
-00008d70: 4b66 ddcc 2f7b 5180 38db 0c8d fba2 27b6  Kf../{Q.8.....'.
-00008d80: 053a 2c88 c047 a25d 819d 723b 3abf 984f  .:,..G.]..r;:..O
-00008d90: 519e 9064 1492 2424 c773 32a6 7142 c9e9  Q..d..$$.s2.qB..
-00008da0: 7df3 f6af fb4d c46e 20b7 09fe 258e 4372  }....M.n ...%.Cr
-00008db0: d410 4942 6332 20ee 0079 8af7 be45 fe0d  ..IBc2 ..y...E..
-00008dc0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00008dd0: 0000 2100 668a 974a d101 0000 b703 0000  ..!.f..J........
-00008de0: 1000 0801 646f 6350 726f 7073 2f61 7070  ....docProps/app
-00008df0: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
+00008c40: 8492 d14a c330 1885 ef05 dfa1 e4be 4dda  ...J.0........M.
+00008c50: caa6 a1ed 4065 570e 0427 8a77 21f9 b715  ....@eW..'.w!...
+00008c60: db34 24d1 6e97 e2eb 083e c05e 472f 7c0b  .4$.n....>.^G/|.
+00008c70: d376 ab95 095e e63f 275f cef9 4932 5997  .v...^.?'_..I2Y.
+00008c80: 85f7 0cda e495 4c51 1810 e481 e495 c8e5  ......LQ........
+00008c90: 3245 b7f3 a97f 8a3c 6399 14ac a824 a468  2E.....<c....$.h
+00008ca0: 0306 4db2 e3a3 842b ca2b 0dd7 ba52 a06d  ..M....+.+...R.m
+00008cb0: 0ec6 7324 6928 5729 5a59 ab28 c686 afa0  ..s$i(W)ZY.(....
+00008cc0: 6426 700e e9c4 45a5 4b66 dd51 2fb1 62fc  d&p...E.Kf.Q/.b.
+00008cd0: 912d 0147 848c 7009 9609 6619 6e80 beea  .-.G..p...f.n...
+00008ce0: 8968 8714 bc47 aa27 5db4 00c1 3114 5082  .h...G.']...1.P.
+00008cf0: b406 8741 887f bc16 7469 febc d02a 0367  ...A....ti...*.g
+00008d00: 99db 8d72 9d76 7187 6cc1 3bb1 77af 4dde  ...r.vq.l.;.w.M.
+00008d10: 1beb ba0e eab8 8de1 f287 f87e 7675 d356  ...........~vu.V
+00008d20: f573 d9ec 8a03 ca12 c129 d7c0 6ca5 b3af  .s.......)..l...
+00008d30: edeb c7f6 e5f3 fd2d c183 69b3 c182 193b  .......-..i....;
+00008d40: 73cb 5ee4 20ce 3743 e3a1 e888 6d81 0e0b  s.^. .7C....m...
+00008d50: c273 9168 5760 afdc c517 97f3 29ca 2212  .s.hW`......).".
+00008d60: c53e 897c 329e 9311 0d23 4ace 1e9a b77f  .>.|2....#J.....
+00008d70: dd6f 2276 8372 97e0 5fe2 b825 8e69 7c4a  .o"v.r.._..%.i|J
+00008d80: a393 0171 0fc8 127c f02d b26f 0000 00ff  ...q...|.-.o....
+00008d90: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00008da0: 0066 8a97 4ad1 0100 00b7 0300 0010 0008  .f..J...........
+00008db0: 0164 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+00008dc0: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
+00008dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008ef0: 0000 0000 0000 0000 0000 0000 9c93 c16e  ...............n
-00008f00: d430 1086 ef48 bc43 e47b 3769 412b b472  .0...H.C.{7iA+.r
-00008f10: 5c55 5b50 9140 acb4 db5e a3a9 33c9 5a75  \U[P.@...^..3.Zu
-00008f20: ecc8 9e8d 7679 162e 1c90 7803 4ebc 0d48  ....vy....x.N..H
-00008f30: 3c06 4ea2 6613 babd 701b cf8c 7f7f fe3d  <.N.f...p......=
-00008f40: e697 fb4a 470d 3aaf ac49 d9f9 2c61 111a  ...JG.:..I..,a..
-00008f50: 6973 65ca 94dd 6ede 9dbd 6191 2730 3968  ise...n...a.'09h
-00008f60: 6b30 6507 f4ec 52bc 7cc1 57ce d6e8 48a1  k0e...R.|.W...H.
-00008f70: 8f82 84f1 29db 12d5 8b38 f672 8b15 f859  ....)....8.r...Y
-00008f80: 289b 5029 acab 80c2 d295 b12d 0a25 f1da  (.P).......-.%..
-00008f90: ca5d 8586 e28b 2499 c7b8 2734 39e6 67f5  .]....$...'49.g.
-00008fa0: 20c8 7ac5 4543 ff2b 9a5b d9f2 f9bb cda1   .z.EC.+.[......
-00008fb0: 0ec0 825f d5b5 5612 28dc 527c 54d2 596f  ..._..V.(.R|T.Yo
-00008fc0: 0b8a deee 256a 1e8f 8b3c d0ad 51ee 9ca2  ....%j...<..Q...
-00008fd0: 8348 783c 5ef2 b504 8dcb 202c 0ad0 1e79  .Hx<^..... ,...y
-00008fe0: 7c4c f01b 84d6 b415 28e7 056f 68d1 a024  |L......(..oh..$
-00008ff0: eb22 af3e 07db 2e58 740f 1e5b 9c94 35e0  .".>...Xt..[..5.
-00009000: 1418 0a58 6d5b bfe8 625d 7b72 e2f7 8f6f  ...Xm[..b]{r...o
-00009010: bf7e 7ef9 f3f5 3b8f 43bd cf75 e1b8 751c  .~~...;.C..u..u.
-00009020: abd7 62de 3584 60da d80a f41c a130 25dc  ..b.5.`......0%.
-00009030: 28d2 e83f 152b 7074 0278 3e06 ee18 7adc  (..?.+pt.x>...z.
-00009040: 1e87 e05e 6326 adde 55c6 8f31 0760 7260  ...^c&..U..1.`r`
-00009050: 7c81 2ed3 60ca 1d94 c1ac e365 86e8 6af5  |...`......e..j.
-00009060: fe64 be50 2653 a641 4f59 77d4 3367 7414  .d.P&S.AOYw.3gt.
-00009070: 363f 2951 a12b 317b c0c3 64ef c490 7f2c  6?)Q.+1{..d....,
-00009080: 58da aa06 7308 4e0d d107 651e fc6d bdb1  X...s.N...e..m..
-00009090: d740 f8f8 e8d3 245f 6fc1 611e e664 188a  .@....$_o.a..d..
-000090a0: 21c1 6fc2 7b3b dd8a 2cb7 c107 cc1f 7b9e  !.o.{;..,.....{.
-000090b0: 16da 11bd ebff a138 9fcf 9257 4998 be51  .......8...WI..Q
-000090c0: 8ec7 c71f 27fe 0200 00ff ff03 0050 4b01  ....'........PK.
-000090d0: 022d 0014 0006 0008 0000 0021 00a6 7404  .-.........!..t.
-000090e0: 5285 0100 00ac 0700 0013 0000 0000 0000  R...............
-000090f0: 0000 0000 0000 0000 0000 005b 436f 6e74  ...........[Cont
-00009100: 656e 745f 5479 7065 735d 2e78 6d6c 504b  ent_Types].xmlPK
-00009110: 0102 2d00 1400 0600 0800 0000 2100 b555  ..-.........!..U
-00009120: 3023 f400 0000 4c02 0000 0b00 0000 0000  0#....L.........
-00009130: 0000 0000 0000 0000 be03 0000 5f72 656c  ............_rel
-00009140: 732f 2e72 656c 7350 4b01 022d 0014 0006  s/.relsPK..-....
-00009150: 0008 0000 0021 0088 e8eb 39b1 0300 00f5  .....!....9.....
-00009160: 0800 000f 0000 0000 0000 0000 0000 0000  ................
-00009170: 00e3 0600 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
-00009180: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00009190: 0000 2100 0e15 64c9 1601 0000 7b05 0000  ..!...d.....{...
-000091a0: 1a00 0000 0000 0000 0000 0000 0000 c10a  ................
-000091b0: 0000 786c 2f5f 7265 6c73 2f77 6f72 6b62  ..xl/_rels/workb
-000091c0: 6f6f 6b2e 786d 6c2e 7265 6c73 504b 0102  ook.xml.relsPK..
-000091d0: 2d00 1400 0600 0800 0000 2100 cfec 59b8  -.........!...Y.
-000091e0: 3915 0000 57bc 0000 1800 0000 0000 0000  9...W...........
-000091f0: 0000 0000 0000 170d 0000 786c 2f77 6f72  ..........xl/wor
-00009200: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-00009210: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00009220: 2100 1162 deb5 f824 0000 3618 0100 1800  !..b...$..6.....
-00009230: 0000 0000 0000 0000 0000 0000 8622 0000  ............."..
-00009240: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00009250: 6565 7432 2e78 6d6c 504b 0102 2d00 1400  eet2.xmlPK..-...
-00009260: 0600 0800 0000 2100 0161 920c 3f03 0000  ......!..a..?...
-00009270: 2b08 0000 1800 0000 0000 0000 0000 0000  +...............
-00009280: 0000 b447 0000 786c 2f77 6f72 6b73 6865  ...G..xl/workshe
-00009290: 6574 732f 7368 6565 7433 2e78 6d6c 504b  ets/sheet3.xmlPK
-000092a0: 0102 2d00 1400 0600 0800 0000 2100 be1d  ..-.........!...
-000092b0: 901e 7e03 0000 9b09 0000 1800 0000 0000  ..~.............
-000092c0: 0000 0000 0000 0000 294b 0000 786c 2f77  ........)K..xl/w
-000092d0: 6f72 6b73 6865 6574 732f 7368 6565 7434  orksheets/sheet4
-000092e0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-000092f0: 0000 2100 474b 9f37 4203 0000 3208 0000  ..!.GK.7B...2...
-00009300: 1800 0000 0000 0000 0000 0000 0000 dd4e  ...............N
-00009310: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00009320: 7368 6565 7435 2e78 6d6c 504b 0102 2d00  sheet5.xmlPK..-.
-00009330: 1400 0600 0800 0000 2100 396a 59f5 ae02  ........!.9jY...
-00009340: 0000 0806 0000 1800 0000 0000 0000 0000  ................
-00009350: 0000 0000 5552 0000 786c 2f77 6f72 6b73  ....UR..xl/works
-00009360: 6865 6574 732f 7368 6565 7436 2e78 6d6c  heets/sheet6.xml
-00009370: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00009380: a22d f25a a606 0000 951a 0000 1300 0000  .-.Z............
-00009390: 0000 0000 0000 0000 0000 3955 0000 786c  ..........9U..xl
-000093a0: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
-000093b0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000093c0: 0020 4456 f605 0300 006e 0700 000d 0000  . DV.....n......
-000093d0: 0000 0000 0000 0000 0000 0010 5c00 0078  ............\..x
-000093e0: 6c2f 7374 796c 6573 2e78 6d6c 504b 0102  l/styles.xmlPK..
-000093f0: 2d00 1400 0600 0800 0000 2100 3968 e2c5  -.........!.9h..
-00009400: 171d 0000 a886 0000 1400 0000 0000 0000  ................
-00009410: 0000 0000 0000 405f 0000 786c 2f73 6861  ......@_..xl/sha
-00009420: 7265 6453 7472 696e 6773 2e78 6d6c 504b  redStrings.xmlPK
-00009430: 0102 2d00 1400 0600 0800 0000 2100 3b6d  ..-.........!.;m
-00009440: 324b c100 0000 4201 0000 2300 0000 0000  2K....B...#.....
-00009450: 0000 0000 0000 0000 897c 0000 786c 2f77  .........|..xl/w
-00009460: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
-00009470: 7368 6565 7431 2e78 6d6c 2e72 656c 7350  sheet1.xml.relsP
-00009480: 4b01 022d 0014 0006 0008 0000 0021 0013  K..-.........!..
-00009490: c42c 13c2 0000 0042 0100 0023 0000 0000  .,.....B...#....
-000094a0: 0000 0000 0000 0000 008b 7d00 0078 6c2f  ..........}..xl/
-000094b0: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
-000094c0: 2f73 6865 6574 322e 786d 6c2e 7265 6c73  /sheet2.xml.rels
-000094d0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000094e0: 34a1 0992 c200 0000 4201 0000 2300 0000  4.......B...#...
-000094f0: 0000 0000 0000 0000 0000 8e7e 0000 786c  ...........~..xl
-00009500: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
-00009510: 732f 7368 6565 7433 2e78 6d6c 2e72 656c  s/sheet3.xml.rel
-00009520: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-00009530: 0043 9611 a3c2 0000 0042 0100 0023 0000  .C.......B...#..
-00009540: 0000 0000 0000 0000 0000 0091 7f00 0078  ...............x
-00009550: 6c2f 776f 726b 7368 6565 7473 2f5f 7265  l/worksheets/_re
-00009560: 6c73 2f73 6865 6574 342e 786d 6c2e 7265  ls/sheet4.xml.re
-00009570: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-00009580: 2100 64f3 3422 c200 0000 4201 0000 2300  !.d.4"....B...#.
-00009590: 0000 0000 0000 0000 0000 0000 9480 0000  ................
-000095a0: 786c 2f77 6f72 6b73 6865 6574 732f 5f72  xl/worksheets/_r
-000095b0: 656c 732f 7368 6565 7435 2e78 6d6c 2e72  els/sheet5.xml.r
-000095c0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-000095d0: 0021 00e8 f726 32a9 0100 0054 0f00 0027  .!...&2....T...'
-000095e0: 0000 0000 0000 0000 0000 0000 0097 8100  ................
-000095f0: 0078 6c2f 7072 696e 7465 7253 6574 7469  .xl/printerSetti
-00009600: 6e67 732f 7072 696e 7465 7253 6574 7469  ngs/printerSetti
-00009610: 6e67 7331 2e62 696e 504b 0102 2d00 1400  ngs1.binPK..-...
-00009620: 0600 0800 0000 2100 e8f7 2632 a901 0000  ......!...&2....
-00009630: 540f 0000 2700 0000 0000 0000 0000 0000  T...'...........
-00009640: 0000 8583 0000 786c 2f70 7269 6e74 6572  ......xl/printer
-00009650: 5365 7474 696e 6773 2f70 7269 6e74 6572  Settings/printer
-00009660: 5365 7474 696e 6773 322e 6269 6e50 4b01  Settings2.binPK.
-00009670: 022d 0014 0006 0008 0000 0021 00e8 f726  .-.........!...&
-00009680: 32a9 0100 0054 0f00 0027 0000 0000 0000  2....T...'......
-00009690: 0000 0000 0000 0073 8500 0078 6c2f 7072  .......s...xl/pr
-000096a0: 696e 7465 7253 6574 7469 6e67 732f 7072  interSettings/pr
-000096b0: 696e 7465 7253 6574 7469 6e67 7333 2e62  interSettings3.b
-000096c0: 696e 504b 0102 2d00 1400 0600 0800 0000  inPK..-.........
-000096d0: 2100 e8f7 2632 a901 0000 540f 0000 2700  !...&2....T...'.
-000096e0: 0000 0000 0000 0000 0000 0000 6187 0000  ............a...
-000096f0: 786c 2f70 7269 6e74 6572 5365 7474 696e  xl/printerSettin
-00009700: 6773 2f70 7269 6e74 6572 5365 7474 696e  gs/printerSettin
-00009710: 6773 342e 6269 6e50 4b01 022d 0014 0006  gs4.binPK..-....
-00009720: 0008 0000 0021 00e8 f726 32a9 0100 0054  .....!...&2....T
-00009730: 0f00 0027 0000 0000 0000 0000 0000 0000  ...'............
-00009740: 004f 8900 0078 6c2f 7072 696e 7465 7253  .O...xl/printerS
-00009750: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-00009760: 6574 7469 6e67 7335 2e62 696e 504b 0102  ettings5.binPK..
-00009770: 2d00 1400 0600 0800 0000 2100 a990 76df  -.........!...v.
-00009780: 5201 0000 6302 0000 1100 0000 0000 0000  R...c...........
-00009790: 0000 0000 0000 3d8b 0000 646f 6350 726f  ......=...docPro
-000097a0: 7073 2f63 6f72 652e 786d 6c50 4b01 022d  ps/core.xmlPK..-
-000097b0: 0014 0006 0008 0000 0021 0066 8a97 4ad1  .........!.f..J.
-000097c0: 0100 00b7 0300 0010 0000 0000 0000 0000  ................
-000097d0: 0000 0000 00c6 8d00 0064 6f63 5072 6f70  .........docProp
-000097e0: 732f 6170 702e 786d 6c50 4b05 0600 0000  s/app.xmlPK.....
-000097f0: 0019 0019 001c 0700 00cd 9000 0000 00    ...............
+00008ec0: 0000 0000 0000 0000 009c 93c1 6ed4 3010  ............n.0.
+00008ed0: 86ef 48bc 43e4 7b37 6941 2bb4 725c 555b  ..H.C.{7iA+.r\U[
+00008ee0: 5091 40ac b4db 5ea3 a933 c95a 75ec c89e  P.@...^..3.Zu...
+00008ef0: 8d76 7916 2e1c 9078 034e bc0d 483c 064e  .vy....x.N..H<.N
+00008f00: a266 13ba bd70 1bcf 8c7f 7ffe 3de6 97fb  .f...p......=...
+00008f10: 4a47 0d3a afac 49d9 f92c 6111 1a69 7365  JG.:..I..,a..ise
+00008f20: ca94 dd6e de9d bd61 9127 3039 686b 3065  ...n...a.'09hk0e
+00008f30: 07f4 ec52 bc7c c157 ced6 e848 a18f 8284  ...R.|.W...H....
+00008f40: f129 db12 d58b 38f6 728b 15f8 5928 9b50  .)....8.r...Y(.P
+00008f50: 29ac ab80 c2d2 95b1 2d0a 25f1 daca 5d85  ).......-.%...].
+00008f60: 86e2 8b24 99c7 b827 3439 e667 f520 c87a  ...$...'49.g. .z
+00008f70: c545 43ff 2b9a 5bd9 f2f9 bbcd a10e c082  .EC.+.[.........
+00008f80: 5fd5 b556 1228 dc52 7c54 d259 6f0b 8ade  _..V.(.R|T.Yo...
+00008f90: ee25 6a1e 8f8b 3cd0 ad51 ee9c a283 4878  .%j...<..Q....Hx
+00008fa0: 3c5e f2b5 048d cb20 2c0a d01e 797c 4cf0  <^..... ,...y|L.
+00008fb0: 1b84 d6b4 1528 e705 6f68 d1a0 24eb 22af  .....(..oh..$.".
+00008fc0: 3e07 db2e 5874 0f1e 5b9c 9435 e014 180a  >...Xt..[..5....
+00008fd0: 586d 5bbf e862 5d7b 72e2 f78f 6fbf 7e7e  Xm[..b]{r...o.~~
+00008fe0: f9f3 f53b 8f43 bdcf 75e1 b875 1cab d762  ...;.C..u..u...b
+00008ff0: de35 8460 dad8 0af4 1ca1 3025 dc28 d2e8  .5.`......0%.(..
+00009000: 3f15 2b70 7402 783e 06ee 187a dc1e 87e0  ?.+pt.x>...z....
+00009010: 5e63 26ad de55 c68f 3107 6072 607c 812e  ^c&..U..1.`r`|..
+00009020: d360 ca1d 94c1 ace3 6586 e86a f5fe 64be  .`......e..j..d.
+00009030: 5026 53a6 414f 5977 d433 6774 1436 3f29  P&S.AOYw.3gt.6?)
+00009040: 51a1 2b31 7bc0 c364 efc4 907f 2c58 daaa  Q.+1{..d....,X..
+00009050: 0673 084e 0dd1 0765 1efc 6dbd b1d7 40f8  .s.N...e..m...@.
+00009060: f8e8 d324 5f6f c161 1ee6 6418 8a21 c16f  ...$_o.a..d..!.o
+00009070: c27b 3bdd 8a2c b7c1 07cc 1f7b 9e16 da11  .{;..,.....{....
+00009080: bdeb ffa1 389f cf92 5749 98be 518e c7c7  ....8...WI..Q...
+00009090: 1f27 fe02 0000 ffff 0300 504b 0102 2d00  .'........PK..-.
+000090a0: 1400 0600 0800 0000 2100 a674 0452 8501  ........!..t.R..
+000090b0: 0000 ac07 0000 1300 0000 0000 0000 0000  ................
+000090c0: 0000 0000 0000 0000 5b43 6f6e 7465 6e74  ........[Content
+000090d0: 5f54 7970 6573 5d2e 786d 6c50 4b01 022d  _Types].xmlPK..-
+000090e0: 0014 0006 0008 0000 0021 00b5 5530 23f4  .........!..U0#.
+000090f0: 0000 004c 0200 000b 0000 0000 0000 0000  ...L............
+00009100: 0000 0000 00be 0300 005f 7265 6c73 2f2e  ........._rels/.
+00009110: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
+00009120: 0000 2100 54bb c217 b603 0000 f108 0000  ..!.T...........
+00009130: 0f00 0000 0000 0000 0000 0000 0000 e306  ................
+00009140: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
+00009150: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00009160: 000e 1564 c916 0100 007b 0500 001a 0000  ...d.....{......
+00009170: 0000 0000 0000 0000 0000 00c6 0a00 0078  ...............x
+00009180: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00009190: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
+000091a0: 0006 0008 0000 0021 0038 7547 bcf3 1400  .......!.8uG....
+000091b0: 0065 b800 0018 0000 0000 0000 0000 0000  .e..............
+000091c0: 0000 001c 0d00 0078 6c2f 776f 726b 7368  .......xl/worksh
+000091d0: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
+000091e0: 4b01 022d 0014 0006 0008 0000 0021 0038  K..-.........!.8
+000091f0: a77c 8910 2500 0034 1801 0018 0000 0000  .|..%..4........
+00009200: 0000 0000 0000 0000 0045 2200 0078 6c2f  .........E"..xl/
+00009210: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00009220: 322e 786d 6c50 4b01 022d 0014 0006 0008  2.xmlPK..-......
+00009230: 0000 0021 0011 d781 143c 0300 0029 0800  ...!.....<...)..
+00009240: 0018 0000 0000 0000 0000 0000 0000 008b  ................
+00009250: 4700 0078 6c2f 776f 726b 7368 6565 7473  G..xl/worksheets
+00009260: 2f73 6865 6574 332e 786d 6c50 4b01 022d  /sheet3.xmlPK..-
+00009270: 0014 0006 0008 0000 0021 0051 0823 677f  .........!.Q.#g.
+00009280: 0300 0099 0900 0018 0000 0000 0000 0000  ................
+00009290: 0000 0000 00fd 4a00 0078 6c2f 776f 726b  ......J..xl/work
+000092a0: 7368 6565 7473 2f73 6865 6574 342e 786d  sheets/sheet4.xm
+000092b0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+000092c0: 0047 4b9f 3742 0300 0032 0800 0018 0000  .GK.7B...2......
+000092d0: 0000 0000 0000 0000 0000 00b2 4e00 0078  ............N..x
+000092e0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+000092f0: 6574 352e 786d 6c50 4b01 022d 0014 0006  et5.xmlPK..-....
+00009300: 0008 0000 0021 0039 6a59 f5ae 0200 0008  .....!.9jY......
+00009310: 0600 0018 0000 0000 0000 0000 0000 0000  ................
+00009320: 002a 5200 0078 6c2f 776f 726b 7368 6565  .*R..xl/workshee
+00009330: 7473 2f73 6865 6574 362e 786d 6c50 4b01  ts/sheet6.xmlPK.
+00009340: 022d 0014 0006 0008 0000 0021 00a2 2df2  .-.........!..-.
+00009350: 5aa6 0600 0095 1a00 0013 0000 0000 0000  Z...............
+00009360: 0000 0000 0000 000e 5500 0078 6c2f 7468  ........U..xl/th
+00009370: 656d 652f 7468 656d 6531 2e78 6d6c 504b  eme/theme1.xmlPK
+00009380: 0102 2d00 1400 0600 0800 0000 2100 2044  ..-.........!. D
+00009390: 56f6 0503 0000 6e07 0000 0d00 0000 0000  V.....n.........
+000093a0: 0000 0000 0000 0000 e55b 0000 786c 2f73  .........[..xl/s
+000093b0: 7479 6c65 732e 786d 6c50 4b01 022d 0014  tyles.xmlPK..-..
+000093c0: 0006 0008 0000 0021 0016 1bf7 990e 1d00  .......!........
+000093d0: 009d 8600 0014 0000 0000 0000 0000 0000  ................
+000093e0: 0000 0015 5f00 0078 6c2f 7368 6172 6564  ...._..xl/shared
+000093f0: 5374 7269 6e67 732e 786d 6c50 4b01 022d  Strings.xmlPK..-
+00009400: 0014 0006 0008 0000 0021 003b 6d32 4bc1  .........!.;m2K.
+00009410: 0000 0042 0100 0023 0000 0000 0000 0000  ...B...#........
+00009420: 0000 0000 0055 7c00 0078 6c2f 776f 726b  .....U|..xl/work
+00009430: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
+00009440: 6574 312e 786d 6c2e 7265 6c73 504b 0102  et1.xml.relsPK..
+00009450: 2d00 1400 0600 0800 0000 2100 13c4 2c13  -.........!...,.
+00009460: c200 0000 4201 0000 2300 0000 0000 0000  ....B...#.......
+00009470: 0000 0000 0000 577d 0000 786c 2f77 6f72  ......W}..xl/wor
+00009480: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
+00009490: 6565 7432 2e78 6d6c 2e72 656c 7350 4b01  eet2.xml.relsPK.
+000094a0: 022d 0014 0006 0008 0000 0021 0034 a109  .-.........!.4..
+000094b0: 92c2 0000 0042 0100 0023 0000 0000 0000  .....B...#......
+000094c0: 0000 0000 0000 005a 7e00 0078 6c2f 776f  .......Z~..xl/wo
+000094d0: 726b 7368 6565 7473 2f5f 7265 6c73 2f73  rksheets/_rels/s
+000094e0: 6865 6574 332e 786d 6c2e 7265 6c73 504b  heet3.xml.relsPK
+000094f0: 0102 2d00 1400 0600 0800 0000 2100 4396  ..-.........!.C.
+00009500: 11a3 c200 0000 4201 0000 2300 0000 0000  ......B...#.....
+00009510: 0000 0000 0000 0000 5d7f 0000 786c 2f77  ........]...xl/w
+00009520: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
+00009530: 7368 6565 7434 2e78 6d6c 2e72 656c 7350  sheet4.xml.relsP
+00009540: 4b01 022d 0014 0006 0008 0000 0021 0064  K..-.........!.d
+00009550: f334 22c2 0000 0042 0100 0023 0000 0000  .4"....B...#....
+00009560: 0000 0000 0000 0000 0060 8000 0078 6c2f  .........`...xl/
+00009570: 776f 726b 7368 6565 7473 2f5f 7265 6c73  worksheets/_rels
+00009580: 2f73 6865 6574 352e 786d 6c2e 7265 6c73  /sheet5.xml.rels
+00009590: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+000095a0: e8f7 2632 a901 0000 540f 0000 2700 0000  ..&2....T...'...
+000095b0: 0000 0000 0000 0000 0000 6381 0000 786c  ..........c...xl
+000095c0: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
+000095d0: 2f70 7269 6e74 6572 5365 7474 696e 6773  /printerSettings
+000095e0: 312e 6269 6e50 4b01 022d 0014 0006 0008  1.binPK..-......
+000095f0: 0000 0021 00e8 f726 32a9 0100 0054 0f00  ...!...&2....T..
+00009600: 0027 0000 0000 0000 0000 0000 0000 0051  .'.............Q
+00009610: 8300 0078 6c2f 7072 696e 7465 7253 6574  ...xl/printerSet
+00009620: 7469 6e67 732f 7072 696e 7465 7253 6574  tings/printerSet
+00009630: 7469 6e67 7332 2e62 696e 504b 0102 2d00  tings2.binPK..-.
+00009640: 1400 0600 0800 0000 2100 e8f7 2632 a901  ........!...&2..
+00009650: 0000 540f 0000 2700 0000 0000 0000 0000  ..T...'.........
+00009660: 0000 0000 3f85 0000 786c 2f70 7269 6e74  ....?...xl/print
+00009670: 6572 5365 7474 696e 6773 2f70 7269 6e74  erSettings/print
+00009680: 6572 5365 7474 696e 6773 332e 6269 6e50  erSettings3.binP
+00009690: 4b01 022d 0014 0006 0008 0000 0021 00e8  K..-.........!..
+000096a0: f726 32a9 0100 0054 0f00 0027 0000 0000  .&2....T...'....
+000096b0: 0000 0000 0000 0000 002d 8700 0078 6c2f  .........-...xl/
+000096c0: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
+000096d0: 7072 696e 7465 7253 6574 7469 6e67 7334  printerSettings4
+000096e0: 2e62 696e 504b 0102 2d00 1400 0600 0800  .binPK..-.......
+000096f0: 0000 2100 e8f7 2632 a901 0000 540f 0000  ..!...&2....T...
+00009700: 2700 0000 0000 0000 0000 0000 0000 1b89  '...............
+00009710: 0000 786c 2f70 7269 6e74 6572 5365 7474  ..xl/printerSett
+00009720: 696e 6773 2f70 7269 6e74 6572 5365 7474  ings/printerSett
+00009730: 696e 6773 352e 6269 6e50 4b01 022d 0014  ings5.binPK..-..
+00009740: 0006 0008 0000 0021 005b 10e8 d453 0100  .......!.[...S..
+00009750: 0063 0200 0011 0000 0000 0000 0000 0000  .c..............
+00009760: 0000 0009 8b00 0064 6f63 5072 6f70 732f  .......docProps/
+00009770: 636f 7265 2e78 6d6c 504b 0102 2d00 1400  core.xmlPK..-...
+00009780: 0600 0800 0000 2100 668a 974a d101 0000  ......!.f..J....
+00009790: b703 0000 1000 0000 0000 0000 0000 0000  ................
+000097a0: 0000 938d 0000 646f 6350 726f 7073 2f61  ......docProps/a
+000097b0: 7070 2e78 6d6c 504b 0506 0000 0000 1900  pp.xmlPK........
+000097c0: 1900 1c07 0000 9a90 0000 0000            ............
```

### Comparing `tej-tool-api-1.0.1/TejTOolAPI/tables/mktboard.csv` & `tej-tool-api-1.0.2/TejTOolAPI/tables/mktboard.csv`

 * *Files identical despite different names*

### Comparing `tej-tool-api-1.0.1/setup.py` & `tej-tool-api-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 long_description = (this_directionary/"README.md").read_text(encoding='utf-8')
 setup(
     name='tej-tool-api',
     description='Package to fetch a large quantity of data from tejapi.',
     keywords=['tej', 'big data', 'data', 'financial', 'economic','stock','TEJ',],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.1',
+    version='1.0.2',
     author='tej',
     author_email='tej@tej.com.tw',
     maintainer='tej api Development Team',
     maintainer_email='tej@tej.com',
     url='https://api.tej.com.tw',
     license='MIT',
     install_requires=install_requires,
```

### Comparing `tej-tool-api-1.0.1/tej_tool_api.egg-info/PKG-INFO` & `tej-tool-api-1.0.2/tej_tool_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to fetch a large quantity of data from tejapi.
 Home-page: https://api.tej.com.tw
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com
 License: MIT
```

