# Comparing `tmp/pyezviz-0.2.2.1.tar.gz` & `tmp/pyezviz-0.2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.2.1.tar", last modified: Sat Jul  8 19:55:13 2023, max compression
+gzip compressed data, was "pyezviz-0.2.2.2.tar", last modified: Mon Jul 10 05:56:27 2023, max compression
```

## Comparing `pyezviz-0.2.2.1.tar` & `pyezviz-0.2.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    62740 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 19:55:13.000000 pyezviz-0.2.2.1/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 19:55:13.469589 pyezviz-0.2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-08 19:55:05.000000 pyezviz-0.2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:27.947186 pyezviz-0.2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 05:56:27.947186 pyezviz-0.2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:27.947186 pyezviz-0.2.2.2/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63562 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:27.947186 pyezviz-0.2.2.2/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 05:56:27.000000 pyezviz-0.2.2.2/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 05:56:27.000000 pyezviz-0.2.2.2/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:56:27.000000 pyezviz-0.2.2.2/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 05:56:27.000000 pyezviz-0.2.2.2/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 05:56:27.000000 pyezviz-0.2.2.2/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 05:56:27.000000 pyezviz-0.2.2.2/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 05:56:27.947186 pyezviz-0.2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-10 05:56:18.000000 pyezviz-0.2.2.2/setup.py
```

### Comparing `pyezviz-0.2.2.1/LICENSE.md` & `pyezviz-0.2.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/README.md` & `pyezviz-0.2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/__init__.py` & `pyezviz-0.2.2.2/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/__main__.py` & `pyezviz-0.2.2.2/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/api_endpoints.py` & `pyezviz-0.2.2.2/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/camera.py` & `pyezviz-0.2.2.2/pyezviz/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,17 +127,15 @@
             if self.fetch_key(["CONNECTION", "localRtspPort"], "554") != 0
             else "554",
             "supported_channels": self.fetch_key(["deviceInfos", "channelNumber"]),
             "battery_level": self.fetch_key(["STATUS", "optionals", "powerRemaining"]),
             "PIR_Status": self.fetch_key(["STATUS", "pirStatus"]),
             "Motion_Trigger": self._alarmmotiontrigger["alarm_trigger_active"],
             "Seconds_Last_Trigger": self._alarmmotiontrigger["timepassed"],
-            "last_alarm_time": self._last_alarm.get(
-                "alarmStartTimeStr", "2000-01-01 00:00:00"
-            ),
+            "last_alarm_time": self._last_alarm.get("alarmStartTimeStr"),
             "last_alarm_pic": self._last_alarm.get(
                 "picUrl",
                 "https://eustatics.ezvizlife.com/ovs_mall/web/img/index/EZVIZ_logo.png?ver=3007907502",
             ),
             "last_alarm_type_code": self._last_alarm.get("alarmType", "0000"),
             "last_alarm_type_name": self._last_alarm.get("sampleName", "NoAlarm"),
             "cam_timezone": self.fetch_key(["STATUS", "optionals", "timeZone"]),
```

### Comparing `pyezviz-0.2.2.1/pyezviz/cas.py` & `pyezviz-0.2.2.2/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/client.py` & `pyezviz-0.2.2.2/pyezviz/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,15 +563,26 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
-            raise PyEzvizError(f"Could not arm or disarm Camera: Got {json_output})")
+            if json_output["meta"]["code"] == 504:
+                _LOGGER.warning(
+                    "Arm or disarm for camera %s timed out. Retrying %s of %s",
+                    serial,
+                    max_retries,
+                    MAX_RETRIES,
+                )
+                return self.set_camera_defence(serial, enable, max_retries + 1)
+
+            raise PyEzvizError(
+                f"Could not arm or disarm Camera {serial}: Got {json_output})"
+            )
 
         return True
 
     def set_battery_camera_work_mode(self, serial: str, value: int) -> bool:
         """Set battery camera work mode."""
         return self.set_device_config_by_key(serial, value, key="batteryCameraWorkMode")
 
@@ -731,17 +742,18 @@
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Can't get storage status from device %s, retrying %s",
+                    "Can't get storage status from device %s, retrying %s of %s",
                     serial,
                     max_retries,
+                    MAX_RETRIES,
                 )
                 return self.get_storage_status(serial, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get device storage status: Got {json_output})"
             )
 
         return json_output["storageStatus"]
@@ -950,17 +962,18 @@
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Unable to reboot camera, camera %s is unreachable, retrying %s",
+                    "Unable to reboot camera, camera %s is unreachable, retrying %s of %s",
                     serial,
                     max_retries,
+                    MAX_RETRIES,
                 )
                 return self.reboot_camera(serial, delay, operation, max_retries + 1)
             raise PyEzvizError(f"Could not reboot device {json_output})")
 
         return True
 
     def get_group_defence_mode(self, max_retries: int = 0) -> Any:
@@ -1221,17 +1234,18 @@
 
         if json_output["resultCode"] == "20002":
             raise EzvizAuthVerificationCode(f"MFA code required: Got {json_output})")
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Camera %s encryption key not found, retrying %s",
+                    "Camera %s encryption key not found, retrying %s of %s",
                     serial,
                     max_retries,
+                    MAX_RETRIES,
                 )
                 return self.get_cam_key(serial, smscode, max_retries + 1)
             raise PyEzvizError(
                 f"Could not get camera encryption key: Got {json_output})"
             )
 
         return json_output["encryptkey"]
@@ -1317,15 +1331,18 @@
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Camera %s busy or unreachable, retrying %s", serial, max_retries
+                    "Camera %s busy or unreachable, retrying %s of %s",
+                    serial,
+                    max_retries,
+                    MAX_RETRIES,
                 )
                 return self.return_panoramic(serial, max_retries + 1)
             raise PyEzvizError(f"Could retrieve panoramic photo: Got {json_output})")
 
         return json_output
 
     def ptz_control_coordinates(
@@ -1524,15 +1541,18 @@
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["resultCode"] != "0":
             if json_output["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Camara %s offline or unreachable, retrying %s", serial, max_retries
+                    "Camara %s offline or unreachable, retrying %s of %s",
+                    serial,
+                    max_retries,
+                    MAX_RETRIES,
                 )
                 return self.api_set_defence_schedule(
                     serial, schedule, enable, max_retries + 1
                 )
             raise PyEzvizError(f"Could not set the schedule: Got {json_output})")
 
         return True
@@ -1723,17 +1743,18 @@
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
             if response_json["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Camera %s is offline, can't set sensitivity, retrying %s",
+                    "Camera %s is offline or unreachable, can't set sensitivity, retrying %s of %s",
                     serial,
                     max_retries,
+                    MAX_RETRIES,
                 )
                 return self.detection_sensibility(
                     serial, sensibility, type_value, max_retries + 1
                 )
             raise PyEzvizError(
                 f"Unable to set detection sensibility. Got: {response_json}"
             )
@@ -1775,15 +1796,18 @@
 
         except ValueError as err:
             raise PyEzvizError("Could not decode response:" + str(err)) from err
 
         if response_json["resultCode"] != "0":
             if response_json["resultCode"] == "-1":
                 _LOGGER.warning(
-                    "Camera %s is offline, retrying %s", serial, max_retries
+                    "Camera %s is offline or unreachable, retrying %s of %s",
+                    serial,
+                    max_retries,
+                    MAX_RETRIES,
                 )
                 return self.get_detection_sensibility(
                     serial, type_value, max_retries + 1
                 )
             raise PyEzvizError(
                 f"Unable to get detection sensibility. Got: {response_json}"
             )
```

### Comparing `pyezviz-0.2.2.1/pyezviz/constants.py` & `pyezviz-0.2.2.2/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/exceptions.py` & `pyezviz-0.2.2.2/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/mqtt.py` & `pyezviz-0.2.2.2/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.2.2/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/pyezviz/utils.py` & `pyezviz-0.2.2.2/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.2.1/setup.py` & `pyezviz-0.2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.2.1",
+    version="0.2.2.2",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

