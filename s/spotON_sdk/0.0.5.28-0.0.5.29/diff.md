# Comparing `tmp/spotON_sdk-0.0.5.28.tar.gz` & `tmp/spotON_sdk-0.0.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.5.28.tar", last modified: Thu Jun 29 21:44:20 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.29.tar", last modified: Mon Jul 10 14:30:13 2023, max compression
```

## Comparing `spotON_sdk-0.0.5.28.tar` & `spotON_sdk-0.0.5.29.tar`

### file list

```diff
@@ -1,31 +1,39 @@
--rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.28/.gitignore
--rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.28/.gitmodules
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.28/LICENSE
--rw-r--r--   0        0        0      380 2023-06-06 23:00:41.979147 spotON_sdk-0.0.5.28/pyproject.toml
--rw-r--r--   0        0        0     1225 2023-06-02 16:15:25.317306 spotON_sdk-0.0.5.28/spotON_sdk/API/API_Call.py
--rw-r--r--   0        0        0     1433 2023-06-11 16:51:01.099711 spotON_sdk-0.0.5.28/spotON_sdk/API/HASS/auth.py
--rw-r--r--   0        0        0      789 2023-06-11 16:51:02.270454 spotON_sdk-0.0.5.28/spotON_sdk/API/HASS/hub.py
--rw-r--r--   0        0        0     1166 2023-06-11 16:51:08.318240 spotON_sdk-0.0.5.28/spotON_sdk/API/HASS/light.py
--rw-r--r--   0        0        0      101 2023-06-01 17:06:55.423781 spotON_sdk-0.0.5.28/spotON_sdk/API/__init__.py
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     2294 2023-06-29 09:35:25.034081 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      239 2023-06-01 17:02:39.339895 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/customBaseModel.py
--rw-r--r--   0        0        0     3012 2023-06-01 08:37:08.552222 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0    10473 2023-06-29 21:09:27.918036 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-06-01 17:04:16.714855 spotON_sdk-0.0.5.28/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      478 2023-06-29 21:44:16.004654 spotON_sdk-0.0.5.28/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      163 2023-06-06 23:18:18.249108 spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1858 2023-06-29 21:43:42.794981 spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     1853 2023-06-06 23:14:11.446293 spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/time_helper.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.28/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.28/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.29/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.29/.gitmodules
+-rw-r--r--   0        0        0      152 2023-07-09 08:46:51.283580 spotON_sdk-0.0.5.29/.vscode/settings.json
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.29/LICENSE
+-rw-r--r--   0        0        0      380 2023-06-06 23:00:41.979147 spotON_sdk-0.0.5.29/pyproject.toml
+-rw-r--r--   0        0        0     1225 2023-06-02 16:15:25.317306 spotON_sdk-0.0.5.29/spotON_sdk/API/API_Call.py
+-rw-r--r--   0        0        0     1433 2023-06-11 16:51:01.099711 spotON_sdk-0.0.5.29/spotON_sdk/API/HASS/auth.py
+-rw-r--r--   0        0        0      789 2023-06-11 16:51:02.270454 spotON_sdk-0.0.5.29/spotON_sdk/API/HASS/hub.py
+-rw-r--r--   0        0        0     1166 2023-06-11 16:51:08.318240 spotON_sdk-0.0.5.29/spotON_sdk/API/HASS/light.py
+-rw-r--r--   0        0        0      101 2023-06-01 17:06:55.423781 spotON_sdk-0.0.5.29/spotON_sdk/API/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     2294 2023-06-29 09:35:25.034081 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      239 2023-06-01 17:02:39.339895 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4830 2023-07-10 10:17:09.516353 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     3334 2023-07-10 14:28:57.905781 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0    10473 2023-06-29 21:09:27.918036 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-06-01 17:04:16.714855 spotON_sdk-0.0.5.29/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-10 14:29:23.688788 spotON_sdk-0.0.5.29/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      163 2023-06-06 23:18:18.249108 spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1860 2023-07-06 11:32:44.174210 spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0     1853 2023-06-06 23:14:11.446293 spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/time_helper.py
+-rw-r--r--   0        0        0     1753 2023-05-23 14:27:13.601664 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/Sensor_Device_function.py
+-rw-r--r--   0        0        0      764 2023-06-02 16:17:03.434973 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/api_call.py
+-rw-r--r--   0        0        0     7199 2023-06-29 21:10:17.505970 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/create_spotON_Areas.py
+-rw-r--r--   0        0        0     2055 2023-06-06 15:48:20.421855 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/create_token.py
+-rw-r--r--   0        0        0     1964 2023-05-28 14:25:22.033622 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/make_json.py
+-rw-r--r--   0        0        0     1527 2023-07-09 08:54:40.727681 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/pricelogic_functions.py
+-rw-r--r--   0        0        0     2930 2023-07-10 09:47:53.269320 spotON_sdk-0.0.5.29/spotON_sdk/private_functions/userstate_function.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.29/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.29/PKG-INFO
```

### Comparing `spotON_sdk-0.0.5.28/.gitignore` & `spotON_sdk-0.0.5.29/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/LICENSE` & `spotON_sdk-0.0.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/API/API_Call.py` & `spotON_sdk-0.0.5.29/spotON_sdk/API/API_Call.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/API/HASS/auth.py` & `spotON_sdk-0.0.5.29/spotON_sdk/API/HASS/auth.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/API/HASS/hub.py` & `spotON_sdk-0.0.5.29/spotON_sdk/API/HASS/hub.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/API/HASS/light.py` & `spotON_sdk-0.0.5.29/spotON_sdk/API/HASS/light.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/markets.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,34 @@
 from pydantic import Field, root_validator,validate_model
 
 class Market(CustomBaseModel):
     area: Area_details
     country: Country
     alias: Optional[str] = None
     cities: str = Field(default="")
-    name: str = Field(default="")
+    name: str = Field(default= "",init = False)
+
     @root_validator(pre=True)
     def set_codes(cls, values):
         country = values.get('country')
         if country and 'country_name' in country:
             values["name"] = country['country_name']
         return values
+    
+    @root_validator(pre=True)
+    def set_name(cls, values):
+        country :Country= values.get('country')
+        area = values.get('area')
+        if country and area:
+            values["name"] = f"{country.emoji} {country.country_name} {area.name}"
+        return values
+    
+
+     
+    
 
     '''@root_validator(pre=True)
     def set_codes(cls, values):
         area = values.get('area')
         print(type(area))
         area_code = area.name
         print(type(area_code))
@@ -83,15 +96,15 @@
 
         return None
 
     @staticmethod
     def get_market_by_code(area_code: str) -> Optional[Market]:
         for market in Markets.markets_List:
             #print (f"Try to find {area_code =} in {market}")
-            if market.country_code == area_code or market.alias == area_code:
+            if market.country.country_code == area_code or market.alias == area_code:
                 return market
 
         return None
```

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.29/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,9 @@
     df["Week"] = df["Week"].astype("int8")
     df["Day"] = df["Day"].astype("int8")
     df["Hour"] = df["Hour"].astype("int8")
     df["Price_daily_AVG"] = df["Price_daily_AVG"].astype('float16')
     df["savings"] = df["savings"].astype('float16')
     for timeslot_length in range(1,24):
         df[f"timeslot_{timeslot_length}H"] = df[f"timeslot_{timeslot_length}H"].astype('float16')
-    return df
+    return df
+
```

### Comparing `spotON_sdk-0.0.5.28/spotON_sdk/data_helpers/time_helper.py` & `spotON_sdk-0.0.5.29/spotON_sdk/data_helpers/time_helper.py`

 * *Files identical despite different names*

