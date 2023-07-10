# Comparing `tmp/vcsc_data_common-0.2.1.tar.gz` & `tmp/vcsc_data_common-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.2.1.tar", last modified: Tue Jun 13 08:26:36 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.2.2.tar", last modified: Mon Jul 10 09:41:07 2023, max compression
```

## Comparing `vcsc_data_common-0.2.1.tar` & `vcsc_data_common-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.556051 vcsc_data_common-0.2.1/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-06-13 08:26:36.556152 vcsc_data_common-0.2.1/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.1/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.1/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-06-13 08:26:36.556492 vcsc_data_common-0.2.1/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.552465 vcsc_data_common-0.2.1/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.1/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.553740 vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554047 vcsc_data_common-0.2.1/vcsc_data_common/backtest/
--rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.1/vcsc_data_common/backtest/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554340 vcsc_data_common-0.2.1/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.2.1/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554685 vcsc_data_common-0.2.1/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.2.1/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.554979 vcsc_data_common-0.2.1/vcsc_data_common/oneday_portfolio/
--rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.1/vcsc_data_common/oneday_portfolio/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.555261 vcsc_data_common-0.2.1/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.1/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.555542 vcsc_data_common-0.2.1/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3868 2023-06-13 08:25:14.000000 vcsc_data_common-0.2.1/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.555812 vcsc_data_common-0.2.1/vcsc_data_common/signals/
--rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.1/vcsc_data_common/signals/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-13 08:26:36.553348 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      648 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-06-13 08:26:36.000000 vcsc_data_common-0.2.1/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.857734 vcsc_data_common-0.2.2/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-10 09:41:07.857818 vcsc_data_common-0.2.2/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.2/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.2/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-07-10 09:41:07.858140 vcsc_data_common-0.2.2/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.853096 vcsc_data_common-0.2.2/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.2/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.854748 vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.855240 vcsc_data_common-0.2.2/vcsc_data_common/backtest/
+-rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.2/vcsc_data_common/backtest/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.855552 vcsc_data_common-0.2.2/vcsc_data_common/fiin_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2225 2023-07-05 03:00:30.000000 vcsc_data_common-0.2.2/vcsc_data_common/fiin_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.855866 vcsc_data_common-0.2.2/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.2.2/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856152 vcsc_data_common-0.2.2/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.2.2/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856438 vcsc_data_common-0.2.2/vcsc_data_common/oneday_portfolio/
+-rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.2/vcsc_data_common/oneday_portfolio/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856709 vcsc_data_common-0.2.2/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.2/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.856984 vcsc_data_common-0.2.2/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3868 2023-06-13 08:25:14.000000 vcsc_data_common-0.2.2/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.857258 vcsc_data_common-0.2.2/vcsc_data_common/proprietary_trading/
+-rw-r--r--   0 pd         (501) staff       (20)      740 2023-07-10 09:38:54.000000 vcsc_data_common-0.2.2/vcsc_data_common/proprietary_trading/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.857511 vcsc_data_common-0.2.2/vcsc_data_common/signals/
+-rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.2/vcsc_data_common/signals/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-10 09:41:07.853969 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      736 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-07-10 09:41:07.000000 vcsc_data_common-0.2.2/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.2.1/pyproject.toml` & `vcsc_data_common-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.2.2/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/backtest/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/oneday_portfolio/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/oneday_portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/portfolio_info/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common/signals/__init__.py` & `vcsc_data_common-0.2.2/vcsc_data_common/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.1/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.2.2/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,13 +6,15 @@
 vcsc_data_common.egg-info/SOURCES.txt
 vcsc_data_common.egg-info/dependency_links.txt
 vcsc_data_common.egg-info/requires.txt
 vcsc_data_common.egg-info/top_level.txt
 vcsc_data_common/ai_framework/__init__.py
 vcsc_data_common/ai_framework/interval_fetching.py
 vcsc_data_common/backtest/__init__.py
+vcsc_data_common/fiin_data/__init__.py
 vcsc_data_common/live_price_data/__init__.py
 vcsc_data_common/offline_price_data/__init__.py
 vcsc_data_common/oneday_portfolio/__init__.py
 vcsc_data_common/order/__init__.py
 vcsc_data_common/portfolio_info/__init__.py
+vcsc_data_common/proprietary_trading/__init__.py
 vcsc_data_common/signals/__init__.py
```

