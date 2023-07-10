# Comparing `tmp/reolink_aio-0.7.2.tar.gz` & `tmp/reolink_aio-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.7.2.tar", last modified: Thu Jun 29 08:55:01 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.3.tar", last modified: Mon Jul 10 20:15:42 2023, max compression
```

## Comparing `reolink_aio-0.7.2.tar` & `reolink_aio-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   192290 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   192713 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-10 20:15:42.000000 reolink_aio-0.7.3/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:15:42.851384 reolink_aio-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-10 20:15:26.000000 reolink_aio-0.7.3/tests/test.py
```

### Comparing `reolink_aio-0.7.2/LICENSE` & `reolink_aio-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/PKG-INFO` & `reolink_aio-0.7.3/reolink_aio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reolink_aio
-Version: 0.7.2
+Name: reolink-aio
+Version: 0.7.3
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.2 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.3 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.2/README.md` & `reolink_aio-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/reolink_aio/api.py` & `reolink_aio-0.7.3/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,14 +612,20 @@
 
     def whiteled_mode(self, channel: int) -> Optional[int]:
         if channel not in self._whiteled_settings:
             return None
 
         return self._whiteled_settings[channel]["WhiteLed"].get("mode")
 
+    def whiteled_mode_list(self, channel: int) -> list[str]:
+        mode_values = [SpotlightModeEnum.off, SpotlightModeEnum.auto, SpotlightModeEnum.schedule]
+        if self.api_version("supportLightAutoBrightness", channel) > 0:
+            mode_values.extend([SpotlightModeEnum.adaptive, SpotlightModeEnum.autoadaptive])
+        return [val.name for val in mode_values]
+
     def whiteled_brightness(self, channel: int) -> Optional[int]:
         if channel not in self._whiteled_settings:
             return None
 
         return self._whiteled_settings[channel]["WhiteLed"].get("bright")
 
     def whiteled_schedule(self, channel: int) -> Optional[dict]:
@@ -1025,15 +1031,15 @@
             if self.api_version("ispSharpen", channel) > 0:
                 self._capabilities[channel].append("isp_sharpen")
             if self.api_version("ispContrast", channel) > 0:
                 self._capabilities[channel].append("isp_contrast")
             if self.api_version("ispBright", channel) > 0:
                 self._capabilities[channel].append("isp_bright")
 
-            if self.daynight_state(channel) is not None:
+            if self.api_version("ispDayNight", channel) > 0 and self.daynight_state(channel) is not None:
                 self._capabilities[channel].append("dayNight")
 
             if self.backlight_state(channel) is not None:
                 self._capabilities[channel].append("backLight")
 
     def supported(self, channel: int | None, capability: str) -> bool:
         """Return if a capability is supported by a camera channel."""
@@ -3002,15 +3008,15 @@
         body = [
             {
                 "cmd": "SetWhiteLed",
                 "param": {"WhiteLed": settings},
             }
         ]
 
-        await self.send_setting(body, wait_before_get=2)
+        await self.send_setting(body, wait_before_get=3)
 
     async def set_spotlight_lighting_schedule(self, channel: int, endhour=6, endmin=0, starthour=18, startmin=0) -> None:
         """Stub to handle setting the time period where spotlight (WhiteLed) will be on when NightMode set and AUTO is off.
         Time in 24-hours format"""
         if channel not in self._channels:
             raise InvalidParameterError(f"set_spotlight_lighting_schedule: no camera connected to channel '{channel}'")
         if channel not in self._whiteled_settings or not self._whiteled_settings[channel]:
```

### Comparing `reolink_aio-0.7.2/reolink_aio/enums.py` & `reolink_aio-0.7.3/reolink_aio/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 class SpotlightModeEnum(Enum):
     """Options for the spotlight mode"""
 
     off = 0
     auto = 1
     schedule = 3
+    adaptive = 5
+    autoadaptive = 4
 
 
 class StatusLedEnum(Enum):
     """Options for the status led mode"""
 
     stayoff = "KeepOff"
     auto = "Off"
```

### Comparing `reolink_aio-0.7.2/reolink_aio/exceptions.py` & `reolink_aio-0.7.3/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/reolink_aio/software_version.py` & `reolink_aio-0.7.3/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/reolink_aio/templates.py` & `reolink_aio-0.7.3/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/reolink_aio/typings.py` & `reolink_aio-0.7.3/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/reolink_aio/utils.py` & `reolink_aio-0.7.3/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.2/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: reolink-aio
-Version: 0.7.2
+Name: reolink_aio
+Version: 0.7.3
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.2 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.3 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.2/setup.py` & `reolink_aio-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.7.2',
+      version='0.7.3',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.7.2/tests/test.py` & `reolink_aio-0.7.3/tests/test.py`

 * *Files identical despite different names*

