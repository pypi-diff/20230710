# Comparing `tmp/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2.tar.gz` & `tmp/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2.tar", last modified: Mon Jul 10 03:58:45 2023, max compression
+gzip compressed data, was "dist/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3.tar", last modified: Mon Jul 10 06:39:39 2023, max compression
```

## Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2.tar` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21670 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py
--rw-r--r--   0 root         (0) root         (0)    29994 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21670 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py
+-rw-r--r--   0 root         (0) root         (0)    29927 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/setup.py
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/LICENSE` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/PKG-INFO` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_8146025f0aa2474a88d81f508253e029
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README-CN.md` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README.md` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-8146025f0aa2474a88d81f508253e029
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_8146025f0aa2474a88d81f508253e029',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_8146025f0aa2474a88d81f508253e029',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,79 +732,72 @@
 
 class SubmitHksecuritytechGatewayDeviceriskReportRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         request_data: str = None,
-        result: DeviceRiskReportResult = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # request_data
         self.request_data = request_data
-        # result
-        self.result = result
 
     def validate(self):
         self.validate_required(self.request_data, 'request_data')
-        self.validate_required(self.result, 'result')
-        if self.result:
-            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.request_data is not None:
             result['request_data'] = self.request_data
-        if self.result is not None:
-            result['result'] = self.result.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('request_data') is not None:
             self.request_data = m.get('request_data')
-        if m.get('result') is not None:
-            temp_model = DeviceRiskReportResult()
-            self.result = temp_model.from_map(m['result'])
         return self
 
 
 class SubmitHksecuritytechGatewayDeviceriskReportResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         result_status: int = None,
+        result: DeviceRiskReportResult = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 1000
         self.result_status = result_status
+        # result
+        self.result = result
 
     def validate(self):
-        pass
+        if self.result:
+            self.result.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -812,22 +805,27 @@
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.result_status is not None:
             result['result_status'] = self.result_status
+        if self.result is not None:
+            result['result'] = self.result.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('result_status') is not None:
             self.result_status = m.get('result_status')
+        if m.get('result') is not None:
+            temp_model = DeviceRiskReportResult()
+            self.result = temp_model.from_map(m['result'])
         return self
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/setup.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/setup.py`

 * *Files identical despite different names*

