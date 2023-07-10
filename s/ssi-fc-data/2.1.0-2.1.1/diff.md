# Comparing `tmp/ssi_fc_data-2.1.0.tar.gz` & `tmp/ssi_fc_data-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssi_fc_data-2.1.0.tar", last modified: Mon Jun 19 09:07:12 2023, max compression
+gzip compressed data, was "ssi_fc_data-2.1.1.tar", last modified: Mon Jul 10 08:46:44 2023, max compression
```

## Comparing `ssi_fc_data-2.1.0.tar` & `ssi_fc_data-2.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.030663 ssi_fc_data-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     2836 2023-06-19 09:07:12.030663 ssi_fc_data-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2365 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)      316 2023-06-19 09:07:12.030663 ssi_fc_data-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1067 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.022663 ssi_fc_data-2.1.0/ssi_fc_data/
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-19 09:07:10.000000 ssi_fc_data-2.1.0/ssi_fc_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/fc_md_client.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/fc_md_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.026663 ssi_fc_data-2.1.0/ssi_fc_data/model/
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/model/access_token.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/model/api.py
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/model/constants.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/model/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.026663 ssi_fc_data-2.1.0/ssi_fc_data/signalr/
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2155 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/_connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.026663 ssi_fc_data-2.1.0/ssi_fc_data/signalr/events/
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/events/_events.py
--rw-r--r--   0 root         (0) root         (0)     2756 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.026663 ssi_fc_data-2.1.0/ssi_fc_data/signalr/hubs/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/hubs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/hubs/_hub.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/hubs/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.030663 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/__init__.py
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/_parameters.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/_queue_events.py
--rw-r--r--   0 root         (0) root         (0)     8034 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/_transport.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/base_transport.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/connection.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-06-19 09:07:09.000000 ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/reconnection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:07:12.026663 ssi_fc_data-2.1.0/ssi_fc_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2836 2023-06-19 09:07:12.000000 ssi_fc_data-2.1.0/ssi_fc_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-19 09:07:12.000000 ssi_fc_data-2.1.0/ssi_fc_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:07:12.000000 ssi_fc_data-2.1.0/ssi_fc_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-19 09:07:12.000000 ssi_fc_data-2.1.0/ssi_fc_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-19 09:07:12.000000 ssi_fc_data-2.1.0/ssi_fc_data.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/fc_md_client.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/fc_md_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data/model/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/model/access_token.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/model/api.py
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/model/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/model/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data/signalr/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/_connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data/signalr/events/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/events/_events.py
+-rw-r--r--   0 root         (0) root         (0)     2756 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data/signalr/hubs/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/hubs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/hubs/_hub.py
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/hubs/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/_queue_events.py
+-rw-r--r--   0 root         (0) root         (0)     8034 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/_transport.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/base_transport.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/connection.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-07-10 08:46:41.000000 ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/reconnection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:46:44.097238 ssi_fc_data-2.1.1/ssi_fc_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-10 08:46:44.000000 ssi_fc_data-2.1.1/ssi_fc_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-10 08:46:44.000000 ssi_fc_data-2.1.1/ssi_fc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 08:46:44.000000 ssi_fc_data-2.1.1/ssi_fc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-10 08:46:44.000000 ssi_fc_data-2.1.1/ssi_fc_data.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-10 08:46:44.000000 ssi_fc_data-2.1.1/ssi_fc_data.egg-info/top_level.txt
```

### Comparing `ssi_fc_data-2.1.0/PKG-INFO` & `ssi_fc_data-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi_fc_data
-Version: 2.1.0
+Version: 2.1.1
 Summary: FastConnect Data client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fcdata
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi_fc_data-2.1.0/README.md` & `ssi_fc_data-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/setup.py` & `ssi_fc_data-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/fc_md_client.py` & `ssi_fc_data-2.1.1/ssi_fc_data/fc_md_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 				self._access_token = AccessTokenModel(ac)
 				return self._access_token.get_access_token()
 			else:
 				raise NameError(res_obj.message)
 		return self._access_token.get_access_token()
      
 	def access_token(self, _input_data: model.accessToken):
-		return self._make_post_request(api.MD_ACCESS_TOKEN, _req_body = _input_data)
+		return self._make_post_request(api.MD_ACCESS_TOKEN, data = _input_data)
 
 
 	def securities(self, _input_data, _object: model.securities):
 		return self._make_get_request(api.MD_SECURITIES, _object)
 
 	def securities_details(self, _input_data,_object: model.securities_details):
 		return self._make_get_request(api.MD_SECURITIES_DETAILS, _object)
```

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/fc_md_stream.py` & `ssi_fc_data-2.1.1/ssi_fc_data/fc_md_stream.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/model/access_token.py` & `ssi_fc_data-2.1.1/ssi_fc_data/model/access_token.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/model/api.py` & `ssi_fc_data-2.1.1/ssi_fc_data/model/api.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/model/model.py` & `ssi_fc_data-2.1.1/ssi_fc_data/model/model.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/_connection.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/_connection.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/events/_events.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/events/_events.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/helpers.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/helpers.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/hubs/_hub.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/_parameters.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/_transport.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/base_transport.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/base_transport.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data/signalr/transports/reconnection.py` & `ssi_fc_data-2.1.1/ssi_fc_data/signalr/transports/reconnection.py`

 * *Files identical despite different names*

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data.egg-info/PKG-INFO` & `ssi_fc_data-2.1.1/ssi_fc_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssi-fc-data
-Version: 2.1.0
+Version: 2.1.1
 Summary: FastConnect Data client by Python
 Home-page: https://github.com/SSI-Securities-Corporation/python-fcdata
 Author: ducdv
 Author-email: ducdv@ssi.com.vn
 License: MIT
 Platform: POSIX
 Platform: Windows
```

### Comparing `ssi_fc_data-2.1.0/ssi_fc_data.egg-info/SOURCES.txt` & `ssi_fc_data-2.1.1/ssi_fc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

