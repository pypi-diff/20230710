# Comparing `tmp/pylovens-0.2.1.tar.gz` & `tmp/pylovens-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylovens-0.2.1.tar", last modified: Fri Jun 23 06:36:26 2023, max compression
+gzip compressed data, was "pylovens-0.3.0.tar", last modified: Mon Jul 10 18:18:07 2023, max compression
```

## Comparing `pylovens-0.2.1.tar` & `pylovens-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-23 06:36:17.000000 pylovens-0.2.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 06:36:17.000000 pylovens-0.2.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-23 06:36:17.000000 pylovens-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-23 06:36:17.000000 pylovens-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-23 06:36:26.907061 pylovens-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-23 06:36:17.000000 pylovens-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-23 06:36:17.000000 pylovens-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:36:26.907061 pylovens-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/src/pylovens/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 06:36:17.000000 pylovens-0.2.1/src/pylovens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27756 2023-06-23 06:36:17.000000 pylovens-0.2.1/src/pylovens/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/src/pylovens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 06:36:17.000000 pylovens-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-06-23 06:36:17.000000 pylovens-0.2.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.442277 pylovens-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.438276 pylovens-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.438276 pylovens-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-10 18:17:56.000000 pylovens-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-10 18:17:56.000000 pylovens-0.3.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-10 18:17:56.000000 pylovens-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-10 18:17:56.000000 pylovens-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-07-10 18:18:07.442277 pylovens-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-07-10 18:17:56.000000 pylovens-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-10 18:17:56.000000 pylovens-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:18:07.442277 pylovens-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.438276 pylovens-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.438276 pylovens-0.3.0/src/pylovens/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-10 18:17:56.000000 pylovens-0.3.0/src/pylovens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 18:18:07.000000 pylovens-0.3.0/src/pylovens/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28405 2023-07-10 18:17:56.000000 pylovens-0.3.0/src/pylovens/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 18:17:56.000000 pylovens-0.3.0/src/pylovens/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.442277 pylovens-0.3.0/src/pylovens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-07-10 18:18:07.000000 pylovens-0.3.0/src/pylovens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 18:18:07.000000 pylovens-0.3.0/src/pylovens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:18:07.000000 pylovens-0.3.0/src/pylovens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 18:18:07.000000 pylovens-0.3.0/src/pylovens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 18:18:07.000000 pylovens-0.3.0/src/pylovens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:18:07.442277 pylovens-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-10 18:17:56.000000 pylovens-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-10 18:17:56.000000 pylovens-0.3.0/tests/test_client.py
```

### Comparing `pylovens-0.2.1/.github/workflows/publish.yaml` & `pylovens-0.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.1/.gitignore` & `pylovens-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.1/LICENSE` & `pylovens-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.1/PKG-INFO` & `pylovens-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pylovens
-Version: 0.2.1
-Summary: Python client for the Lovens API.
-Author-email: Rogier van der Geer <rogier@vander-geer.nl>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # pylovens
 
 Python client for the Lovens API.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rogiervandergeer/pylovens/test.yaml) 
 ![PyPI](https://img.shields.io/pypi/v/pylovens)
 ![PyPI - License](https://img.shields.io/pypi/l/pylovens)
@@ -23,61 +11,49 @@
 
 ## Usage
 
 Using the client is as simple as:
 ```python
 from pylovens import LovensClient
 
-client = LovensClient()
-client.login("your_username", "your_secret_password")
+client = LovensClient("your_username", "your_secret_password")
 
 bikes = client.get_bikes()
 ```
 
 _Note:_ only authentication with email/password is supported. 
 
 
 ## Methods
 
 The `LovensClient` exposes the following methods:
 
- - [Login & User](#login--user)
-   - [`login`](#login---log-in-using-your-username-e-mail-address-and-password)
-   - [`get_user`](#getuser---get-information-on-the-user)
+ - [User](#user)
+   - [`get_user`](#get_user---get-information-on-the-user)
  - [Bikes](#bikes)
-   - [`get_bikes`](#getbikes---fetch-all-bikes-accessible-to-your-user)
-   - [`get_bike`](#getbike---fetch-a-bike-by-its-id)
-   - [`get_state`](#getstate---get-the-state-of-a-bike)
-   - [`get_health`](#gethealth---get-bike-health-status)
+   - [`get_bikes`](#get_bikes---fetch-all-bikes-accessible-to-your-user)
+   - [`get_bike`](#get_bike---fetch-a-bike-by-its-id)
+   - [`get_state`](#get_state---get-the-state-of-a-bike)
+   - [`get_health`](#get_health---get-bike-health-status)
  - [Rides](#rides)
-   - [`iterate_rides`](#iteraterides---iterate-through-the-rides-of-a-bike)
-   - [`get_rides`](#getrides---fetch-a-list-of-rides-of-a-bike)
-   - [`get_ride`](#getride---fetch-a-ride-by-its-id)
-   - [`get_location`](#getlocation---get-location-history-in-a-time-range)
+   - [`iterate_rides`](#iterate_rides---iterate-through-the-rides-of-a-bike)
+   - [`get_rides`](#get_rides---fetch-a-list-of-rides-of-a-bike)
+   - [`get_ride`](#get_ride---fetch-a-ride-by-its-id)
+   - [`get_location`](#get_location---get-location-history-in-a-time-range)
  - [Battery](#battery)
-   - [`get_battery_state`](#getbatterystate---get-the-state-of-the-battery-of-a-bike)
-   - [`get_battery_statistics`](#getbatterystatistics---get-historical-state-of-the-battery-of-a-bike)
+   - [`get_battery_state`](#get_battery_state---get-the-state-of-the-battery-of-a-bike)
+   - [`get_battery_statistics`](#get_battery_statistics---get-historical-state-of-the-battery-of-a-bike)
  - [Statistics](#statistics)
-   - [`get_statistics`](#getstatistics---get-ride-statistics-for-a-bike)
+   - [`get_statistics`](#get_statistics---get-ride-statistics-for-a-bike)
  - [Geofences](#geofences)
-   - [`get_geofences`](#getgeofences---fetch-all-geofences-associated-to-a-bike)
-   - [`get_geofence`](#getgeofence---get-a-single-geofence-by-its-id)
-   - [`get_geofence_stats`](#getgeofencestats---get-statistics-of-a-geofence)
-
-### Login & User
-
-#### `login` - Log in using your username (e-mail address) and password.
-```python
-def login(self, username: str, password: str) -> None
-```
-
-##### Arguments
-- `username`: Your e-mail address.
-- `password`: The corresponding password.
+   - [`get_geofences`](#get_geofences---fetch-all-geofences-associated-to-a-bike)
+   - [`get_geofence`](#get_geofence---get-a-single-geofence-by-its-id)
+   - [`get_geofence_stats`](#get_geofence_stats---get-statistics-of-a-geofence)
 
+### User
 
 #### `get_user` - Get information on the user.
 ```python
 def get_user(self) -> dict
 ```
 
 ##### Returns
```

### Comparing `pylovens-0.2.1/README.md` & `pylovens-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pylovens
+Version: 0.3.0
+Summary: Python client for the Lovens API.
+Author-email: Rogier van der Geer <rogier@vander-geer.nl>
+License: MIT
+Project-URL: Repository, https://github.com/rogiervandergeer/pylovens
+Keywords: api,cargo bike,ebike,gps,lovens
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # pylovens
 
 Python client for the Lovens API.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rogiervandergeer/pylovens/test.yaml) 
 ![PyPI](https://img.shields.io/pypi/v/pylovens)
 ![PyPI - License](https://img.shields.io/pypi/l/pylovens)
@@ -11,61 +29,49 @@
 
 ## Usage
 
 Using the client is as simple as:
 ```python
 from pylovens import LovensClient
 
-client = LovensClient()
-client.login("your_username", "your_secret_password")
+client = LovensClient("your_username", "your_secret_password")
 
 bikes = client.get_bikes()
 ```
 
 _Note:_ only authentication with email/password is supported. 
 
 
 ## Methods
 
 The `LovensClient` exposes the following methods:
 
- - [Login & User](#login--user)
-   - [`login`](#login---log-in-using-your-username-e-mail-address-and-password)
-   - [`get_user`](#getuser---get-information-on-the-user)
+ - [User](#user)
+   - [`get_user`](#get_user---get-information-on-the-user)
  - [Bikes](#bikes)
-   - [`get_bikes`](#getbikes---fetch-all-bikes-accessible-to-your-user)
-   - [`get_bike`](#getbike---fetch-a-bike-by-its-id)
-   - [`get_state`](#getstate---get-the-state-of-a-bike)
-   - [`get_health`](#gethealth---get-bike-health-status)
+   - [`get_bikes`](#get_bikes---fetch-all-bikes-accessible-to-your-user)
+   - [`get_bike`](#get_bike---fetch-a-bike-by-its-id)
+   - [`get_state`](#get_state---get-the-state-of-a-bike)
+   - [`get_health`](#get_health---get-bike-health-status)
  - [Rides](#rides)
-   - [`iterate_rides`](#iteraterides---iterate-through-the-rides-of-a-bike)
-   - [`get_rides`](#getrides---fetch-a-list-of-rides-of-a-bike)
-   - [`get_ride`](#getride---fetch-a-ride-by-its-id)
-   - [`get_location`](#getlocation---get-location-history-in-a-time-range)
+   - [`iterate_rides`](#iterate_rides---iterate-through-the-rides-of-a-bike)
+   - [`get_rides`](#get_rides---fetch-a-list-of-rides-of-a-bike)
+   - [`get_ride`](#get_ride---fetch-a-ride-by-its-id)
+   - [`get_location`](#get_location---get-location-history-in-a-time-range)
  - [Battery](#battery)
-   - [`get_battery_state`](#getbatterystate---get-the-state-of-the-battery-of-a-bike)
-   - [`get_battery_statistics`](#getbatterystatistics---get-historical-state-of-the-battery-of-a-bike)
+   - [`get_battery_state`](#get_battery_state---get-the-state-of-the-battery-of-a-bike)
+   - [`get_battery_statistics`](#get_battery_statistics---get-historical-state-of-the-battery-of-a-bike)
  - [Statistics](#statistics)
-   - [`get_statistics`](#getstatistics---get-ride-statistics-for-a-bike)
+   - [`get_statistics`](#get_statistics---get-ride-statistics-for-a-bike)
  - [Geofences](#geofences)
-   - [`get_geofences`](#getgeofences---fetch-all-geofences-associated-to-a-bike)
-   - [`get_geofence`](#getgeofence---get-a-single-geofence-by-its-id)
-   - [`get_geofence_stats`](#getgeofencestats---get-statistics-of-a-geofence)
-
-### Login & User
-
-#### `login` - Log in using your username (e-mail address) and password.
-```python
-def login(self, username: str, password: str) -> None
-```
-
-##### Arguments
-- `username`: Your e-mail address.
-- `password`: The corresponding password.
+   - [`get_geofences`](#get_geofences---fetch-all-geofences-associated-to-a-bike)
+   - [`get_geofence`](#get_geofence---get-a-single-geofence-by-its-id)
+   - [`get_geofence_stats`](#get_geofence_stats---get-statistics-of-a-geofence)
 
+### User
 
 #### `get_user` - Get information on the user.
 ```python
 def get_user(self) -> dict
 ```
 
 ##### Returns
```

### Comparing `pylovens-0.2.1/src/pylovens/client.py` & `pylovens-0.3.0/src/pylovens/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from base64 import b64encode, urlsafe_b64encode
-from datetime import datetime, date, time
+from datetime import datetime, date, time, timezone
 from functools import partial
 from hashlib import sha256
 from itertools import islice
 from json import dumps
 from os import urandom
 from re import sub
 from typing import Iterable
 from urllib.parse import quote
 from zoneinfo import ZoneInfo
 
-from requests import get, post
+from requests import Response, get, post
 
 from pylovens._version import __version__
+from pylovens.exceptions import AuthenticationError, InvalidTokenError
 
 
 class LovensClient:
     client_id: str = "7d5d1a2a-3f6e-45c6-9e9e-b0b5f224f8a5"
     client_secret: str = ""
 
-    def __init__(self):
-        self.access_token: str | None = None
+    def __init__(self, username: str, password: str):
+        self.credentials: tuple[str, str] = (username, password)
+        self._access_token: tuple[str, datetime] | None = None
         self._login_settings_: dict | None = None
         self._timezone: str | None = None
 
     def get_battery_state(self, bike_id: int) -> dict[str]:
         """
         Get the state of the battery of a bike.
 
@@ -41,15 +43,15 @@
                 'charging': False,
                 'range': 30
               }
         """
         response = get(
             f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/battery/current-state", headers=self._headers_with_auth
         )
-        response.raise_for_status()
+        self._handle_errors(response)
         return self._parse_dates(response.json(), keys={"last_battery_update", "last_full_charge"})
 
     def get_battery_statistics(
         self,
         bike_id: int,
         start_date: date | datetime | None = None,
         end_date: date | datetime | None = None,
@@ -96,15 +98,15 @@
             url += f"from={quote(start_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}"
             if end_date is not None:
                 url += "&"
         if end_date is not None:
             url += f"till={quote(end_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}"
 
         response = get(url, headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return list(map(self._parse_dates, response.json()))
 
     def get_bike(self, bike_id: int) -> dict:
         """
         Fetch a bike by its ID.
 
         Args:
@@ -122,15 +124,15 @@
                 'battery_percentage': 50,
                 'owning_user': { <result of get_user method> },
                 'geofences': [ <result of get_geofences method> ],
                 ...
               }
         """
         response = get(f"https://lovens.api.bike.conneq.tech/bike/{bike_id}", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return self._parse_dates(response.json())
 
     def get_bikes(self) -> list[dict]:
         """
         Fetch all bikes accessible to your user.
 
         Returns:
@@ -145,15 +147,15 @@
                 'battery_percentage': 50,
                 'owning_user': { <result of get_user method> },
                 'geofences': [ <result of get_geofences method> ],
                 ...
               }
         """
         response = get("https://lovens.api.bike.conneq.tech/bike", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return list(map(self._parse_dates, response.json()))
 
     def get_geofences(self, bike_id: int) -> list[dict[str, datetime | dict[str, float] | int | str]]:
         """
         Fetch all geofences associated to a bike.
 
         Args:
@@ -169,15 +171,15 @@
                 'center': {'lat': 52.379189, 'lon': 4.899431},
                 'radius': 200,
                 'active_state': 0,
                 'creation_date': datetime(2023, 4, 1, 17, 10, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam'))
               }
         """
         response = get(f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/geofence", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return [self._parse_dates(geofence) for geofence in response.json()]
 
     def get_geofence(self, geofence_id: int) -> dict[str, datetime | dict[str, float] | int | str]:
         """
         Get a single geofence by its ID.
 
         Args:
@@ -195,15 +197,15 @@
                 'active_state': 0,
                 'creation_date': datetime(2023, 4, 1, 17, 10, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam'))
               }
         """
         response = get(
             f"https://lovens.api.bike.conneq.tech/bike/geofence/{geofence_id}", headers=self._headers_with_auth
         )
-        response.raise_for_status()
+        self._handle_errors(response)
         return self._parse_dates(response.json())
 
     def get_geofence_stats(
         self,
         geofence_id: int,
         start_date: datetime | date | None = None,
         end_date: datetime | date | None = None,
@@ -231,15 +233,15 @@
         if start_date is not None:
             url += (
                 f"?from={quote(start_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}&"
                 f"till={quote(end_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}"
             )
 
         response = get(url, headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return response.json()
 
     def get_health(self, bike_id: int) -> list[dict]:
         """
         Get bike health status.
 
         Args:
@@ -271,15 +273,15 @@
                 'status': True,
                 'value': 'true',
                 'value_type': 'bool'
               }
             ]
         """
         response = get(f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/health", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return [self._parse_dates(d, keys={"value"}) if d["value_type"] == "datetime" else d for d in response.json()]
 
     def get_location(
         self, bike_id: int, start_date: datetime | date, end_date: datetime | date
     ) -> list[dict, bool, datetime | int | float]:
         """
         Get location history in a time range.
@@ -309,15 +311,15 @@
 
         response = get(
             f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/location?"
             f"from={quote(start_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}&"
             f"till={quote(end_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}",
             headers=self._headers_with_auth,
         )
-        response.raise_for_status()
+        self._handle_errors(response)
         return list(sorted(map(self._parse_dates, response.json()), key=lambda d: d["date"]))
 
     def get_ride(self, ride_id: int) -> dict:
         """
         Fetch a ride by its ID.
 
         Args:
@@ -339,15 +341,15 @@
                 "creation_date": datetime(2023, 4, 1, 17, 10, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
                 "active_time": 330,
                 "timezone": "Europe/Amsterdam",
                 ...
             }
         """
         response = get(f"https://lovens.api.bike.conneq.tech/v2/bike/ride/{ride_id}", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return self._parse_dates(response.json())
 
     def get_rides(self, bike_id: int, newest_first: bool = True, n: int = 50) -> list[dict]:
         """
         Fetch a list of rides of a bike.
 
         If you are interested in fetching all rides of a bike, or are not sure how many you need,
@@ -413,15 +415,15 @@
         response = get(
             f"https://lovens.api.bike.conneq.tech/v2/bike/{bike_id}/ride?"
             f"limit={batch_size}&"
             f"offset={_offset}&"
             f"order%5B%5D=start_date%3B{'desc' if newest_first else 'asc'}",
             headers=self._headers_with_auth,
         )
-        response.raise_for_status()
+        self._handle_errors(response)
         data = response.json()
         yield from map(self._parse_dates, data["data"])
         if data["meta"]["total_records"] > data["meta"]["offset"] + data["meta"]["limit"]:
             yield from self.iterate_rides(bike_id=bike_id, batch_size=batch_size, _offset=_offset + batch_size)
 
     def get_state(self, bike_id: int) -> dict[str]:
         """
@@ -440,15 +442,15 @@
                 'charging': False,
                 'last_full_charge': datetime(2023, 4, 1, 17, 10, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
                 'odometer': 300,
                 'range': 30
               }
         """
         response = get(f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/state", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         return self._parse_dates(response.json()[0], keys={"last_full_charge"})
 
     def get_statistics(
         self,
         bike_id: int,
         start_date: date | datetime,
         end_date: date | datetime,
@@ -492,15 +494,15 @@
         response = get(
             f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/stats?"
             f"from={quote(start_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}&"
             f"till={quote(end_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}&"
             f"type={type}&tz={self.timezone.key}",
             headers=self._headers_with_auth,
         )
-        response.raise_for_status()
+        self._handle_errors(response)
         return list(map(partial(self._parse_dates, keys={"from", "till"}), response.json()))
 
     def get_user(self) -> dict:
         """
         Get information on the user.
 
         Returns:
@@ -511,32 +513,19 @@
                 "creation_date": datetime(2023, 4, 30, 23, 59, 59, tzinfo=ZoneInfo(key='Europe/Amsterdam'),
                 "email": "your@mail.address",
                 "timezone": "Europe/Amsterdam",
                 ...
             }
         """
         response = get(f"https://lovens.api.bike.conneq.tech/user/me", headers=self._headers_with_auth)
-        response.raise_for_status()
+        self._handle_errors(response)
         data = response.json()
         self._timezone = data["timezone"]
         return self._parse_dates(data)
 
-    def login(self, username: str, password: str) -> None:
-        """
-        Log in using your username (e-mail address) and password.
-
-        Args:
-            username: Your e-mail address.
-            password: The corresponding password.
-        """
-        token = self._get_aws_cognito_token(username, password)
-        challenge, verifier = self._create_code_challenge()
-        challenge_result = self._send_code_challenge(challenge, token)
-        self.access_token = self._get_access_token(code=challenge_result, verifier=verifier)
-
     @property
     def timezone(self) -> ZoneInfo:
         """The timezone of your user."""
         if self._timezone is None:
             self.get_user()
         return ZoneInfo(self._timezone)
 
@@ -545,32 +534,39 @@
         code_verifier = urlsafe_b64encode(urandom(40)).decode("utf-8")
         code_verifier = sub("[^a-zA-Z0-9]+", "", code_verifier)
         code_challenge = sha256(code_verifier.encode("utf-8")).digest()
         code_challenge = urlsafe_b64encode(code_challenge).decode("utf-8")
         code_challenge = code_challenge.replace("=", "")
         return code_challenge, code_verifier
 
+    def _login(self) -> tuple[str, datetime]:
+        """Log in using username (e-mail address) and password."""
+        token = self._get_aws_cognito_token(*self.credentials)
+        challenge, verifier = self._create_code_challenge()
+        challenge_result = self._send_code_challenge(challenge, token)
+        return self._get_access_token(code=challenge_result, verifier=verifier)
+
     @property
     def _login_settings(self) -> dict:
         """Return the login settings corresponding to our client ID."""
         if self._login_settings_ is None:
             response = get(
                 f"https://api.ids.conneq.tech/client/{self.client_id}/setting/loginpage", headers=self._headers
             )
-            response.raise_for_status()
+            self._handle_errors(response)
             self._login_settings_ = response.json()
         return self._login_settings_
 
     def _get_aws_cognito_client_id(self) -> str:
         """Obtain the AWS Cognito client_id."""
         response = get(
             f"https://api.ids.conneq.tech/client/{self._login_settings['idp_client_id']}/setting/signinpage",
             headers=self._headers,
         )
-        response.raise_for_status()
+        self._handle_errors(response)
         return response.json()["cognito_config"]["aws_user_pools_web_client_id"]
 
     def _get_aws_cognito_token(self, username: str, password: str) -> str:
         """Authenticate with AWS Cognito and obtain an AccessToken"""
         response = post(
             self._login_settings["idp_issuer_id"],
             data=dumps(
@@ -585,32 +581,35 @@
                 "Content-Type": "application/x-amz-json-1.1",
                 "Referer": "https://login.conneq.tech/",
                 "Origin": "https://login.conneq.tech",
                 "X-Amz-Target": "AWSCognitoIdentityProviderService.InitiateAuth",
                 **self._headers,
             },
         )
-        response.raise_for_status()
+        if response.status_code == 400:
+            raise AuthenticationError()
+        self._handle_errors(response)
         return response.json()["AuthenticationResult"]["AccessToken"]
 
-    def _get_access_token(self, code: str, verifier: str) -> str:
+    def _get_access_token(self, code: str, verifier: str) -> tuple[str, datetime]:
         """Sign in with Lovens using the previously obtained code and obtain the bearer token."""
         redirect_uri = self._login_settings["login_page_allowed_redirect_uris"][0]
         content = f"""code={code}&code_verifier={verifier}&redirect_uri={redirect_uri}&grant_type=authorization_code"""
         response = post(
             "https://api.ids.conneq.tech/oauth",
             data=content,
             headers={
                 "Authorization": b"Basic " + b64encode(f"{self.client_id}:{self.client_secret}".encode("utf-8")),
                 "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
                 **self._headers,
             },
         )
         response.raise_for_status()
-        return response.json()["access_token"]
+        data = response.json()
+        return data["access_token"], datetime.strptime(data["expires_at"][:-4] + "Z", "%Y-%m-%dT%H:%M:%S.%f%z")
 
     def _send_code_challenge(self, code_challenge: str, cognito_token: str) -> str:
         """Send a code challenge and the AWS Cognito token."""
         return post(
             "https://api.ids.conneq.tech/oauth",
             data=dumps(
                 {
@@ -636,27 +635,34 @@
     def _headers(self) -> dict[str, str]:
         """Get the HTTP headers to be sent with every request."""
         return {"User-Agent": f"pylovens {__version__.split('+')[0]}"}
 
     @property
     def _headers_with_auth(self) -> dict[str, str]:
         """The headers including authorization. Only possible when authenticated."""
-        if self.access_token is None:
-            raise ValueError("Not authenticated.")
-        return {"Authorization": f"Bearer {self.access_token}", **self._headers}
+        if self._access_token is None or self._access_token[1] < datetime.now(tz=timezone.utc):
+            self._access_token = self._login()
+        return {"Authorization": f"Bearer {self._access_token[0]}", **self._headers}
 
     def _parse_dates(self, data: dict[str], keys: set[str] | None = None) -> dict[str]:
         """Parse datetimes in a dictionary."""
         return {
             key: datetime.strptime(value, "%Y-%m-%dT%H:%M:%S%z").astimezone(self.timezone)
             if (keys is not None and key in keys) or (keys is None and (key.endswith("_date") or key == "date"))
             else value
             for key, value in data.items()
         }
 
+    def _handle_errors(self, response: Response) -> None:
+        """Check for error codes."""
+        if response.status_code in (401, 403):  # 401 is returned for invalid tokens, 403 for malformed tokens
+            self.access_token = None
+            raise InvalidTokenError()
+        response.raise_for_status()
+
     def _normalise_dates(
         self, start_date: datetime | date | None, end_date: datetime | date | None
     ) -> tuple[datetime | None, datetime | None]:
         """
         Normalise a date range input.
 
         If start_date and/or end_date is a date object, they are interpreted as the start and end of the day
```

### Comparing `pylovens-0.2.1/src/pylovens.egg-info/PKG-INFO` & `pylovens-0.3.0/src/pylovens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: pylovens
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python client for the Lovens API.
 Author-email: Rogier van der Geer <rogier@vander-geer.nl>
 License: MIT
+Project-URL: Repository, https://github.com/rogiervandergeer/pylovens
+Keywords: api,cargo bike,ebike,gps,lovens
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pylovens
 
@@ -23,61 +29,49 @@
 
 ## Usage
 
 Using the client is as simple as:
 ```python
 from pylovens import LovensClient
 
-client = LovensClient()
-client.login("your_username", "your_secret_password")
+client = LovensClient("your_username", "your_secret_password")
 
 bikes = client.get_bikes()
 ```
 
 _Note:_ only authentication with email/password is supported. 
 
 
 ## Methods
 
 The `LovensClient` exposes the following methods:
 
- - [Login & User](#login--user)
-   - [`login`](#login---log-in-using-your-username-e-mail-address-and-password)
-   - [`get_user`](#getuser---get-information-on-the-user)
+ - [User](#user)
+   - [`get_user`](#get_user---get-information-on-the-user)
  - [Bikes](#bikes)
-   - [`get_bikes`](#getbikes---fetch-all-bikes-accessible-to-your-user)
-   - [`get_bike`](#getbike---fetch-a-bike-by-its-id)
-   - [`get_state`](#getstate---get-the-state-of-a-bike)
-   - [`get_health`](#gethealth---get-bike-health-status)
+   - [`get_bikes`](#get_bikes---fetch-all-bikes-accessible-to-your-user)
+   - [`get_bike`](#get_bike---fetch-a-bike-by-its-id)
+   - [`get_state`](#get_state---get-the-state-of-a-bike)
+   - [`get_health`](#get_health---get-bike-health-status)
  - [Rides](#rides)
-   - [`iterate_rides`](#iteraterides---iterate-through-the-rides-of-a-bike)
-   - [`get_rides`](#getrides---fetch-a-list-of-rides-of-a-bike)
-   - [`get_ride`](#getride---fetch-a-ride-by-its-id)
-   - [`get_location`](#getlocation---get-location-history-in-a-time-range)
+   - [`iterate_rides`](#iterate_rides---iterate-through-the-rides-of-a-bike)
+   - [`get_rides`](#get_rides---fetch-a-list-of-rides-of-a-bike)
+   - [`get_ride`](#get_ride---fetch-a-ride-by-its-id)
+   - [`get_location`](#get_location---get-location-history-in-a-time-range)
  - [Battery](#battery)
-   - [`get_battery_state`](#getbatterystate---get-the-state-of-the-battery-of-a-bike)
-   - [`get_battery_statistics`](#getbatterystatistics---get-historical-state-of-the-battery-of-a-bike)
+   - [`get_battery_state`](#get_battery_state---get-the-state-of-the-battery-of-a-bike)
+   - [`get_battery_statistics`](#get_battery_statistics---get-historical-state-of-the-battery-of-a-bike)
  - [Statistics](#statistics)
-   - [`get_statistics`](#getstatistics---get-ride-statistics-for-a-bike)
+   - [`get_statistics`](#get_statistics---get-ride-statistics-for-a-bike)
  - [Geofences](#geofences)
-   - [`get_geofences`](#getgeofences---fetch-all-geofences-associated-to-a-bike)
-   - [`get_geofence`](#getgeofence---get-a-single-geofence-by-its-id)
-   - [`get_geofence_stats`](#getgeofencestats---get-statistics-of-a-geofence)
-
-### Login & User
-
-#### `login` - Log in using your username (e-mail address) and password.
-```python
-def login(self, username: str, password: str) -> None
-```
-
-##### Arguments
-- `username`: Your e-mail address.
-- `password`: The corresponding password.
+   - [`get_geofences`](#get_geofences---fetch-all-geofences-associated-to-a-bike)
+   - [`get_geofence`](#get_geofence---get-a-single-geofence-by-its-id)
+   - [`get_geofence_stats`](#get_geofence_stats---get-statistics-of-a-geofence)
 
+### User
 
 #### `get_user` - Get information on the user.
 ```python
 def get_user(self) -> dict
 ```
 
 ##### Returns
```

### Comparing `pylovens-0.2.1/tests/conftest.py` & `pylovens-0.3.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from datetime import datetime
 from os import environ
 
-from pytest import fixture, mark
+from pytest import fixture, skip
 
 from pylovens import LovensClient
 
 
 @fixture(scope="function")
 def client() -> LovensClient:
-    return LovensClient()
+    return LovensClient("username", "password")
 
 
 @fixture(scope="session")
 def authenticated_client() -> LovensClient:
-    client = LovensClient()
-    client.login(environ["LOVENS_USERNAME"], environ["LOVENS_PASSWORD"])
-    return client
+    try:
+        return LovensClient(environ["LOVENS_USERNAME"], environ["LOVENS_PASSWORD"])
+    except KeyError:
+        skip("Requires authentication.")
 
 
 @fixture(scope="session")
 def bike_id(authenticated_client: LovensClient) -> int:
     bikes = authenticated_client.get_bikes()
+    if len(bikes) == 0:
+        skip("No bikes found.")
     return bikes[0]["id"]
 
 
 @fixture(scope="session")
 def ride(authenticated_client: LovensClient, bike_id: int) -> dict:
     for ride in authenticated_client.iterate_rides(bike_id):
         return ride
+    skip("No rides found.")
```

### Comparing `pylovens-0.2.1/tests/test_client.py` & `pylovens-0.3.0/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,81 @@
-from datetime import date, datetime, timedelta
+from datetime import date, datetime, timedelta, timezone
 from itertools import islice
 from os import environ
 from zoneinfo import ZoneInfo
 
 from pytest import fixture, mark, raises, skip
 from requests import HTTPError
 
 from pylovens import LovensClient
-
-
-if_authenticated = mark.skipif(
-    "LOVENS_USERNAME" not in environ or "LOVENS_PASSWORD" not in environ, reason="Requires authentication."
-)
+from pylovens.exceptions import AuthenticationError, InvalidTokenError
 
 
 class TestHeaders:
     def test_user_agent(self, client: LovensClient):
         headers = client._headers
         assert headers["User-Agent"].startswith("pylovens ")
         assert len(headers["User-Agent"].split(".")) in (3, 4)  # Either pylovens x.y.z or pylovens x.y.z.dev0
         assert "+" not in headers["User-Agent"]
 
-    def test_headers_with_auth_without_token(self, client: LovensClient):
-        with raises(ValueError):
-            _ = client._headers_with_auth
+    def test_headers_with_auth_without_token(self, client: LovensClient, mocker):
+        mock = mocker.patch("pylovens.client.LovensClient._login")
+        mock.return_value = ("token", datetime.now(tz=timezone.utc))
+        client._access_token = None
+        _ = client._headers_with_auth
+        mock.assert_called_once()
 
     def test_headers_with_auth(self, client: LovensClient):
-        client.access_token = "token"
+        client._access_token = ("token", datetime.now(tz=timezone.utc) + timedelta(hours=1))
         headers = client._headers_with_auth
         assert headers["Authorization"] == "Bearer token"
 
+    def test_token_expired(self, client: LovensClient, mocker):
+        mock = mocker.patch("pylovens.client.LovensClient._login")
+        client._access_token = ("token", datetime.now(tz=timezone.utc) - timedelta(hours=1))
+        _ = client._headers_with_auth
+        mock.assert_called_once()
+
 
 class TestLogin:
     def test_login_settings(self, client: LovensClient):
         assert client._login_settings_ is None
         settings = client._login_settings
         for key in ("idp_client_id", "idp_issuer_id", "login_page_allowed_redirect_uris", "idp_redirect_uri"):
             assert key in settings
         assert client._login_settings_ is not None
 
     def test_aws_cognito_client_id(self, client: LovensClient):
         client_id = client._get_aws_cognito_client_id()
         assert len(client_id) > 0
 
-    @if_authenticated
     def test_get_aws_cognito_token(self, client: LovensClient):
-        token = client._get_aws_cognito_token(username=environ["LOVENS_USERNAME"], password=environ["LOVENS_PASSWORD"])
-        assert len(token) > 0
+        try:
+            token = client._get_aws_cognito_token(
+                username=environ["LOVENS_USERNAME"], password=environ["LOVENS_PASSWORD"]
+            )
+            assert len(token) > 0
+        except KeyError:
+            skip("Requires authentication.")
+
+    def test_invalid_credentials(self, client: LovensClient):
+        with raises(AuthenticationError):
+            client._get_aws_cognito_token(username="test", password="user")
+
+    @mark.parametrize("token", ["invalid_token", "at_i1yelzysa43u749it8nv9p7ceub73"])
+    def test_invalid_token(self, client: LovensClient, token: str):
+        client._access_token = (token, datetime.now(tz=timezone.utc) + timedelta(hours=1))
+        with raises(InvalidTokenError):
+            client.get_bikes()
+        assert client.access_token is None
 
 
 class TestNormalizeDates:
     @fixture(scope="function")
-    def client_with_timezone(self) -> LovensClient:
-        client = LovensClient()
+    def client_with_timezone(self, client: LovensClient) -> LovensClient:
         client._timezone = "Europe/Amsterdam"
         return client
 
     @mark.parametrize(
         "start_date,end_date",
         [
             (None, None),
@@ -82,15 +101,14 @@
         x, y = client_with_timezone._normalise_dates(
             datetime(2023, 1, 15), datetime(2023, 1, 30, tzinfo=ZoneInfo("Asia/Singapore"))
         )
         assert x == datetime(2023, 1, 15, tzinfo=ZoneInfo("Europe/Amsterdam"))
         assert y == datetime(2023, 1, 30, tzinfo=ZoneInfo("Asia/Singapore"))
 
 
-@if_authenticated
 class TestBattery:
     def test_get_battery_state(self, authenticated_client: LovensClient, bike_id: int):
         state = authenticated_client.get_battery_state(bike_id)
         assert "battery_percentage" in state
 
     def test_get_battery_statistics(self, authenticated_client: LovensClient, bike_id: int):
         stats = authenticated_client.get_battery_statistics(bike_id)
@@ -104,15 +122,14 @@
     def test_statistics_start_date_after_end_date(self, authenticated_client: LovensClient, bike_id: int):
         with raises(HTTPError):
             authenticated_client.get_battery_statistics(
                 bike_id, start_date=datetime.now() - timedelta(hours=3), end_date=datetime.now() - timedelta(hours=5)
             )
 
 
-@if_authenticated
 class TestRides:
     def test_iterate_rides(self, authenticated_client: LovensClient, bike_id: int):
         rides = authenticated_client.iterate_rides(bike_id)
         for ride in rides:
             assert isinstance(ride, dict)
             assert isinstance(ride["creation_date"], datetime)
             break
@@ -135,15 +152,14 @@
             assert location["date"] >= locations[0]["date"]
 
     def test_get_ride(self, authenticated_client: LovensClient, ride: dict):
         ride_ = authenticated_client.get_ride(ride["id"])
         assert ride_ == ride
 
 
-@if_authenticated
 class TestMisc:
     def test_user(self, authenticated_client: LovensClient):
         user = authenticated_client.get_user()
         assert "timezone" in user
         assert "username" in user
 
     def test_timezone(self, authenticated_client: LovensClient):
@@ -164,15 +180,14 @@
         health = authenticated_client.get_health(bike_id)
         assert isinstance(health[0]["value"], datetime)
         assert isinstance(health[1]["value"], datetime)
         assert isinstance(health[2]["value"], str)
         assert isinstance(health[3]["value"], str)
 
 
-@if_authenticated
 class TestGeofences:
     @fixture(scope="class")
     def geofence(self, authenticated_client: LovensClient, bike_id: int) -> dict:
         geofence_data = authenticated_client.get_geofences(bike_id)
         if len(geofence_data) == 0:
             skip("No geofences defined.")
         return geofence_data[0]
@@ -192,15 +207,14 @@
     def test_get_geofence_stats(self, authenticated_client: LovensClient, geofence: dict):
         geofence_stats = authenticated_client.get_geofence_stats(
             geofence["id"], geofence["creation_date"], geofence["creation_date"] + timedelta(days=7)
         )
         assert geofence_stats.keys() == {"entries_all_time", "entries_in_timespan"}
 
 
-@if_authenticated
 class TestStatistics:
     def test_get_daily_statistics(self, authenticated_client: LovensClient, bike_id: int):
         stats = authenticated_client.get_statistics(bike_id, start_date=date(2023, 4, 1), end_date=date(2023, 4, 5))
         assert len(stats) == 5  # There are 5 days in the range.
         assert stats[0]["from"] == datetime(2023, 4, 1, 0, 0, tzinfo=ZoneInfo("Europe/Amsterdam"))
         assert stats[-1]["till"] == datetime(2023, 4, 5, 23, 59, 59, tzinfo=ZoneInfo("Europe/Amsterdam"))
```

