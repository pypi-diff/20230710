# Comparing `tmp/canarytools-1.1.0.tar.gz` & `tmp/canarytools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/canarytools-1.1.0.tar", last modified: Thu Sep 22 10:26:38 2022, max compression
+gzip compressed data, was "dist/canarytools-1.1.1.tar", last modified: Mon Jul 10 16:13:08 2023, max compression
```

## Comparing `canarytools-1.1.0.tar` & `canarytools-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 leighton   (501) staff       (20)        0 2022-09-22 10:26:38.000000 canarytools-1.1.0/
--rw-r--r--   0 leighton   (501) staff       (20)     5064 2022-09-22 10:26:38.000000 canarytools-1.1.0/PKG-INFO
-drwxr-xr-x   0 leighton   (501) staff       (20)        0 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools.egg-info/
--rw-r--r--   0 leighton   (501) staff       (20)     5064 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools.egg-info/PKG-INFO
--rw-r--r--   0 leighton   (501) staff       (20)      607 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools.egg-info/SOURCES.txt
--rw-r--r--   0 leighton   (501) staff       (20)       50 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools.egg-info/requires.txt
--rw-r--r--   0 leighton   (501) staff       (20)       12 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools.egg-info/top_level.txt
--rw-r--r--   0 leighton   (501) staff       (20)        1 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools.egg-info/dependency_links.txt
--rw-r--r--   0 leighton   (501) staff       (20)       19 2022-09-20 09:12:54.000000 canarytools-1.1.0/MANIFEST.in
--rw-r--r--   0 leighton   (501) staff       (20)     1432 2022-09-22 10:24:48.000000 canarytools-1.1.0/setup.py
--rw-r--r--   0 leighton   (501) staff       (20)       67 2022-09-22 10:26:38.000000 canarytools-1.1.0/setup.cfg
-drwxr-xr-x   0 leighton   (501) staff       (20)        0 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools/
--rw-r--r--   0 leighton   (501) staff       (20)    12089 2022-09-22 10:13:00.000000 canarytools-1.1.0/canarytools/console.py
--rw-r--r--   0 leighton   (501) staff       (20)     1301 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/__init__.py
-drwxr-xr-x   0 leighton   (501) staff       (20)        0 2022-09-22 10:26:38.000000 canarytools-1.1.0/canarytools/models/
--rw-r--r--   0 leighton   (501) staff       (20)     2823 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/update.py
--rw-r--r--   0 leighton   (501) staff       (20)     3984 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/flocks.py
--rw-r--r--   0 leighton   (501) staff       (20)     2044 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/databundles.py
--rw-r--r--   0 leighton   (501) staff       (20)     9734 2022-09-22 10:13:00.000000 canarytools-1.1.0/canarytools/models/canarytokens.py
--rw-r--r--   0 leighton   (501) staff       (20)        0 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/__init__.py
--rw-r--r--   0 leighton   (501) staff       (20)      837 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/result.py
--rw-r--r--   0 leighton   (501) staff       (20)     1341 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/settings.py
--rw-r--r--   0 leighton   (501) staff       (20)    22100 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/incidents.py
--rw-r--r--   0 leighton   (501) staff       (20)     9456 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/devices.py
--rw-r--r--   0 leighton   (501) staff       (20)      913 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/models/base.py
--rw-r--r--   0 leighton   (501) staff       (20)     1589 2022-09-20 09:12:54.000000 canarytools-1.1.0/canarytools/exceptions.py
--rw-r--r--   0 leighton   (501) staff       (20)     3336 2022-09-20 09:12:54.000000 canarytools-1.1.0/README.rst
--rw-r--r--   0 leighton   (501) staff       (20)     1494 2022-09-20 09:12:54.000000 canarytools-1.1.0/LICENSE.txt
+drwxr-xr-x   0 azhar      (501) staff       (20)        0 2023-07-10 16:13:08.000000 canarytools-1.1.1/
+-rw-r--r--   0 azhar      (501) staff       (20)     5064 2023-07-10 16:13:08.000000 canarytools-1.1.1/PKG-INFO
+drwxr-xr-x   0 azhar      (501) staff       (20)        0 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools.egg-info/
+-rw-r--r--   0 azhar      (501) staff       (20)     5064 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools.egg-info/PKG-INFO
+-rw-r--r--   0 azhar      (501) staff       (20)      607 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools.egg-info/SOURCES.txt
+-rw-r--r--   0 azhar      (501) staff       (20)       50 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools.egg-info/requires.txt
+-rw-r--r--   0 azhar      (501) staff       (20)       12 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools.egg-info/top_level.txt
+-rw-r--r--   0 azhar      (501) staff       (20)        1 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools.egg-info/dependency_links.txt
+-rw-r--r--   0 azhar      (501) staff       (20)       19 2017-06-02 10:57:03.000000 canarytools-1.1.1/MANIFEST.in
+-rw-r--r--   0 azhar      (501) staff       (20)     1432 2023-07-10 16:08:55.000000 canarytools-1.1.1/setup.py
+-rw-r--r--   0 azhar      (501) staff       (20)       67 2023-07-10 16:13:08.000000 canarytools-1.1.1/setup.cfg
+drwxr-xr-x   0 azhar      (501) staff       (20)        0 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools/
+-rw-r--r--   0 azhar      (501) staff       (20)    12089 2023-01-04 15:49:28.000000 canarytools-1.1.1/canarytools/console.py
+-rw-r--r--   0 azhar      (501) staff       (20)     1301 2023-01-04 15:49:28.000000 canarytools-1.1.1/canarytools/__init__.py
+drwxr-xr-x   0 azhar      (501) staff       (20)        0 2023-07-10 16:13:08.000000 canarytools-1.1.1/canarytools/models/
+-rw-r--r--   0 azhar      (501) staff       (20)     2823 2017-06-02 10:57:03.000000 canarytools-1.1.1/canarytools/models/update.py
+-rw-r--r--   0 azhar      (501) staff       (20)     3984 2023-01-04 15:49:28.000000 canarytools-1.1.1/canarytools/models/flocks.py
+-rw-r--r--   0 azhar      (501) staff       (20)     2044 2017-06-02 10:57:03.000000 canarytools-1.1.1/canarytools/models/databundles.py
+-rw-r--r--   0 azhar      (501) staff       (20)     9909 2023-07-10 15:43:27.000000 canarytools-1.1.1/canarytools/models/canarytokens.py
+-rw-r--r--   0 azhar      (501) staff       (20)        0 2017-06-02 10:57:03.000000 canarytools-1.1.1/canarytools/models/__init__.py
+-rw-r--r--   0 azhar      (501) staff       (20)      837 2017-06-02 10:57:03.000000 canarytools-1.1.1/canarytools/models/result.py
+-rw-r--r--   0 azhar      (501) staff       (20)     1341 2017-06-02 10:57:03.000000 canarytools-1.1.1/canarytools/models/settings.py
+-rw-r--r--   0 azhar      (501) staff       (20)    22146 2023-07-10 15:48:19.000000 canarytools-1.1.1/canarytools/models/incidents.py
+-rw-r--r--   0 azhar      (501) staff       (20)     9456 2017-06-02 10:57:03.000000 canarytools-1.1.1/canarytools/models/devices.py
+-rw-r--r--   0 azhar      (501) staff       (20)      913 2020-10-19 10:44:42.000000 canarytools-1.1.1/canarytools/models/base.py
+-rw-r--r--   0 azhar      (501) staff       (20)     1589 2023-01-04 15:49:28.000000 canarytools-1.1.1/canarytools/exceptions.py
+-rw-r--r--   0 azhar      (501) staff       (20)     3336 2019-08-15 08:33:20.000000 canarytools-1.1.1/README.rst
+-rw-r--r--   0 azhar      (501) staff       (20)     1494 2017-06-02 10:57:03.000000 canarytools-1.1.1/LICENSE.txt
```

### Comparing `canarytools-1.1.0/PKG-INFO` & `canarytools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: canarytools
-Version: 1.1.0
+Version: 1.1.1
 Summary: An API for the Thinkst Canary Console
 Home-page: https://canary.tools/
 Author: Thinkst Applied Research
 Author-email: canary@thinkst.com
 License: Revised BSD License
 Description: Python Canary API Wrapper
         ===================================
```

### Comparing `canarytools-1.1.0/canarytools.egg-info/PKG-INFO` & `canarytools-1.1.1/canarytools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: canarytools
-Version: 1.1.0
+Version: 1.1.1
 Summary: An API for the Thinkst Canary Console
 Home-page: https://canary.tools/
 Author: Thinkst Applied Research
 Author-email: canary@thinkst.com
 License: Revised BSD License
 Description: Python Canary API Wrapper
         ===================================
```

### Comparing `canarytools-1.1.0/canarytools.egg-info/SOURCES.txt` & `canarytools-1.1.1/canarytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/setup.py` & `canarytools-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='canarytools',
 
-    version='1.1.0',
+    version='1.1.1',
 
     description='An API for the Thinkst Canary Console',
     long_description=long_description,
 
     url='https://canary.tools/',
 
     author='Thinkst Applied Research',
```

### Comparing `canarytools-1.1.0/canarytools/console.py` & `canarytools-1.1.1/canarytools/console.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/__init__.py` & `canarytools-1.1.1/canarytools/__init__.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/update.py` & `canarytools-1.1.1/canarytools/models/update.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/flocks.py` & `canarytools-1.1.1/canarytools/models/flocks.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/databundles.py` & `canarytools-1.1.1/canarytools/models/databundles.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/canarytokens.py` & `canarytools-1.1.1/canarytools/models/canarytokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,27 @@
         """
         self.console = console
 
     def create(
         self, 
         memo, 
         kind, 
+        flock_id=None,
         web_image=None, 
         mimetype=None, 
         cloned_web=None, 
         browser_redirect_url=None,
         s3_source_bucket=None,
         s3_log_bucket=None,
         process_name=None,
         ):
         """Create a new Canarytoken
 
         :param memo: Use this to remind yourself where you placed the Canarytoken
+        :param flock_id: Create token in different flock. Defaults to: 'flock:default'
         :param kind: The type of Canarytoken. Supported classes currently are: 
             aws-id, cloned-web, dns, doc-msword, http, 
             doc-msexcel, msexcel-macro, doc-msword, msword-macro, 
             pdf-acrobat-reader, qr-code, sensitive-cmd, signed-exe, 
             slack-api, web-image, windows-dir, wireguard
         :param web_image: The path to an image file for use with web-image tokens.
         :param mimetype: The type of image specified in web_image. e.g. 'image/png'
@@ -47,14 +49,17 @@
 
         Usage::
 
             >>> import canarytools
             >>> result = console.tokens.create(memo='Desktop Token', kind=canarytools.CanaryTokenKinds.DOC_MSWORD)
         """
         params = {'memo': memo, 'kind': kind}
+        if flock_id:
+            params['flock_id'] = flock_id
+
         if cloned_web:
             params['cloned_web'] = cloned_web
 
         if browser_redirect_url:
             params['browser_redirect_url'] = browser_redirect_url
 
         if s3_source_bucket:
@@ -266,8 +271,8 @@
     PDF = 'pdf-acrobat-reader'
     QRCODE = 'qr-code'
     SIGNEDEXE = 'signed-exe'
     SLACK = 'slack-api'
     SLOWREDIRECT = 'slow-redirect'
     WEB_IMAGE = 'web-image'
     WINDOWS_DIR = 'windows-dir'
-    WIREGUARD = 'wireguard'
+    WIREGUARD = 'wireguard'
```

### Comparing `canarytools-1.1.0/canarytools/models/result.py` & `canarytools-1.1.1/canarytools/models/result.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/settings.py` & `canarytools-1.1.1/canarytools/models/settings.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/incidents.py` & `canarytools-1.1.1/canarytools/models/incidents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 import datetime
 from dateutil.parser import parse
 
 from .base import CanaryToolsBase
 from ..exceptions import IncidentError
 
 
@@ -339,15 +340,15 @@
 
     def to_dict(self):
         """Convert incident to a dictionary format
 
         :return: Dictionary value of incident
         :rtype:  <type 'dict'>
         """
-        incident_dict = self.__dict__
+        incident_dict = deepcopy(self.__dict__)
         if 'console' in incident_dict.keys():
             incident_dict.pop('console')
 
         events_list = []
         for event in incident_dict['events']:
             if type(event) != dict:
                 event_dict = event.to_dict()
@@ -435,15 +436,15 @@
 
     def to_dict(self):
         """Convert event to a dictionary format
 
         :return: Dictionary value of event
         :rtype:  <type 'dict'>
         """
-        event_dict = self.__dict__
+        event_dict = deepcopy(self.__dict__)
         event_dict.pop('console')
 
         # It's likely by mistake that we expliclitly include and reformat timestamp field here. This method otherwise
         # transparently passes on the Event dict. This breaks on the ConsolidatedNetworkPortscan event, whose details
         # are formatted differently and don't include a timestamp. Instead of removing this, we preserve the behaviour
         # for customer code that relies on this by reformatting only if it exists.
         if 'timestamp' in event_dict:
```

### Comparing `canarytools-1.1.0/canarytools/models/devices.py` & `canarytools-1.1.1/canarytools/models/devices.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/models/base.py` & `canarytools-1.1.1/canarytools/models/base.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/canarytools/exceptions.py` & `canarytools-1.1.1/canarytools/exceptions.py`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/README.rst` & `canarytools-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `canarytools-1.1.0/LICENSE.txt` & `canarytools-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

