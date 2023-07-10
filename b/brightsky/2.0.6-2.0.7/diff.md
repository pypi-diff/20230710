# Comparing `tmp/brightsky-2.0.6.tar.gz` & `tmp/brightsky-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.6.tar", last modified: Fri Jun 23 12:40:59 2023, max compression
+gzip compressed data, was "brightsky-2.0.7.tar", last modified: Mon Jul 10 14:09:30 2023, max compression
```

## Comparing `brightsky-2.0.6.tar` & `brightsky-2.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.265739 brightsky-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 12:40:53.000000 brightsky-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-23 12:40:59.265739 brightsky-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-23 12:40:53.000000 brightsky-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.261739 brightsky-2.0.6/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.261739 brightsky-2.0.6/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-23 12:40:53.000000 brightsky-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:40:59.265739 brightsky-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-23 12:40:53.000000 brightsky-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.265739 brightsky-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.263547 brightsky-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 14:09:21.000000 brightsky-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-10 14:09:30.263547 brightsky-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-10 14:09:21.000000 brightsky-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.259547 brightsky-2.0.7/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-10 14:09:21.000000 brightsky-2.0.7/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.259547 brightsky-2.0.7/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 14:09:30.000000 brightsky-2.0.7/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 14:09:21.000000 brightsky-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:09:30.263547 brightsky-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 14:09:21.000000 brightsky-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:09:30.263547 brightsky-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-07-10 14:09:21.000000 brightsky-2.0.7/tests/test_web.py
```

### Comparing `brightsky-2.0.6/LICENSE` & `brightsky-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/PKG-INFO` & `brightsky-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.6
+Version: 2.0.7
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.6/README.md` & `brightsky-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/__main__.py` & `brightsky-2.0.7/brightsky/__main__.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/cli.py` & `brightsky-2.0.7/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/db.py` & `brightsky-2.0.7/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/export.py` & `brightsky-2.0.7/brightsky/export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/parsers.py` & `brightsky-2.0.7/brightsky/parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/polling.py` & `brightsky-2.0.7/brightsky/polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/query.py` & `brightsky-2.0.7/brightsky/query.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/settings.py` & `brightsky-2.0.7/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/tasks.py` & `brightsky-2.0.7/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky/utils.py` & `brightsky-2.0.7/brightsky/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,7 +68,17 @@
             return parse_date(date_str.replace(' ', '+'))
         raise e from None
 
 
 @lru_cache
 def sunrise_sunset(lat, lon, date):
     return daylight(Observer(lat, lon), date)
+
+
+def daytime(lat, lon, timestamp):
+    try:
+        sunrise, sunset = sunrise_sunset(lat, lon, timestamp.date())
+    except ValueError as e:
+        return 'day' if 'above' in e.args[0] else 'night'
+    if sunset < sunrise:
+        return 'night' if sunset <= timestamp <= sunrise else 'day'
+    return 'day' if sunrise <= timestamp <= sunset else 'night'
```

### Comparing `brightsky-2.0.6/brightsky/web.py` & `brightsky-2.0.7/brightsky/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from gunicorn.app.base import BaseApplication
 from gunicorn.util import import_app
 
 import brightsky
 from brightsky import query
 from brightsky.db import fetch
 from brightsky.settings import settings
-from brightsky.utils import parse_date, sunrise_sunset
+from brightsky.utils import daytime, parse_date
 
 
 @contextmanager
 def convert_exceptions():
     try:
         yield
     except ValueError as e:
@@ -166,25 +166,18 @@
         if is_rainy:
             return 'rain'
         elif (wind_speed or 0) > settings.ICON_WIND_THRESHOLD:
             return 'wind'
         elif (row['cloud_cover'] or 0) >= settings.ICON_CLOUDY_THRESHOLD:
             return 'cloudy'
         source = source_map[row['source_id']]
-        try:
-            sunrise, sunset = sunrise_sunset(
-                source['lat'], source['lon'], row['timestamp'].date())
-        except ValueError as e:
-            daytime = 'day' if 'above' in e.args[0] else 'night'
-        else:
-            daytime = (
-                'day' if sunrise <= row['timestamp'] <= sunset else 'night')
+        daytime_str = daytime(source['lat'], source['lon'], row['timestamp'])
         if (row['cloud_cover'] or 0) >= settings.ICON_PARTLY_CLOUDY_THRESHOLD:
-            return f'partly-cloudy-{daytime}'
-        return f'clear-{daytime}'
+            return f'partly-cloudy-{daytime_str}'
+        return f'clear-{daytime_str}'
 
 
 class CurrentWeatherResource(WeatherResource):
 
     PRECIPITATION_FIELD = 'precipitation_10'
     WIND_SPEED_FIELD = 'wind_speed_10'
```

### Comparing `brightsky-2.0.6/brightsky/worker.py` & `brightsky-2.0.7/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.7/brightsky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.6
+Version: 2.0.7
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.6/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.7/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/setup.py` & `brightsky-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/tests/test_export.py` & `brightsky-2.0.7/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/tests/test_parsers.py` & `brightsky-2.0.7/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/tests/test_polling.py` & `brightsky-2.0.7/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/tests/test_settings.py` & `brightsky-2.0.7/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/tests/test_tasks.py` & `brightsky-2.0.7/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.6/tests/test_utils.py` & `brightsky-2.0.7/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
-from dateutil.tz import tzoffset
+from dateutil.tz import tzoffset, tzutc
 
-from brightsky.utils import parse_date, sunrise_sunset
+from brightsky.utils import daytime, parse_date, sunrise_sunset
 
 
 def test_parse_date():
     assert parse_date('2020-08-18') == datetime.datetime(2020, 8, 18, 0, 0)
     assert parse_date('2020-08-18 12:34') == datetime.datetime(
         2020, 8, 18, 12, 34)
     assert parse_date('2020-08-18T12:34:56+02:00') == datetime.datetime(
@@ -15,7 +15,20 @@
 
 
 def test_sunrise_sunset():
     sunrise, sunset = sunrise_sunset(52, 7.6, datetime.date(2020, 8, 18))
     assert sunrise < sunset
     assert sunrise.utcoffset().total_seconds() == 0
     assert sunset.utcoffset().total_seconds() == 0
+
+
+def test_daytime():
+    midnight_0 = datetime.datetime(2023, 7, 10, 0, 0, tzinfo=tzutc())
+    noon_0 = datetime.datetime(2023, 7, 10, 12, 0, tzinfo=tzutc())
+    midnight_10 = datetime.datetime(2023, 7, 9, 14, 0, tzinfo=tzutc())
+    noon_10 = datetime.datetime(2023, 7, 10, 2, 0, tzinfo=tzutc())
+    # Muenster
+    assert daytime(52, 7.6, midnight_0) == 'night'
+    assert daytime(52, 7.6, noon_0) == 'day'
+    # Sydney
+    assert daytime(-33.8, 151, midnight_10) == 'night'
+    assert daytime(-33.8, 151, noon_10) == 'day'
```

### Comparing `brightsky-2.0.6/tests/test_web.py` & `brightsky-2.0.7/tests/test_web.py`

 * *Files identical despite different names*

