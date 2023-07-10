# Comparing `tmp/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3.tar.gz` & `tmp/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3.tar", last modified: Mon Jul 10 06:39:39 2023, max compression
+gzip compressed data, was "dist/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4.tar", last modified: Mon Jul 10 07:46:24 2023, max compression
```

## Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3.tar` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21670 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py
--rw-r--r--   0 root         (0) root         (0)    29927 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 06:39:39.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:46:24.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 07:46:24.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:46:24.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:46:24.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21670 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py
+-rw-r--r--   0 root         (0) root         (0)    27560 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 07:46:24.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 07:46:23.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/setup.py
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/LICENSE` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/PKG-INFO` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_8146025f0aa2474a88d81f508253e029
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README-CN.md` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/README.md` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-8146025f0aa2474a88d81f508253e029
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.3',
+                    'sdk_version': '1.0.4',
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
-                    'sdk_version': '1.0.3',
+                    'sdk_version': '1.0.4',
                     '_prod_code': 'ak_8146025f0aa2474a88d81f508253e029',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,133 +250,14 @@
         if m.get('dynamic_num') is not None:
             self.dynamic_num = m.get('dynamic_num')
         if m.get('result_type') is not None:
             self.result_type = m.get('result_type')
         return self
 
 
-class DeviceRiskReportResult(TeaModel):
-    def __init__(
-        self,
-        success: bool = None,
-        result_code: str = None,
-        result_status: str = None,
-        apdid: str = None,
-        token: str = None,
-        current_time: str = None,
-        version: str = None,
-        vkey_switch: str = None,
-        bug_track_switch: str = None,
-        app_list_ver: str = None,
-        dynamic_key: str = None,
-        result_data: DeviceRiskReportResultData = None,
-    ):
-        # success
-        self.success = success
-        # result_code
-        self.result_code = result_code
-        # result_status
-        self.result_status = result_status
-        # apdid
-        self.apdid = apdid
-        # token
-        self.token = token
-        # current_time
-        self.current_time = current_time
-        # version
-        self.version = version
-        # vkey_switch
-        self.vkey_switch = vkey_switch
-        # bug_track_switch
-        self.bug_track_switch = bug_track_switch
-        # app_list_ver
-        self.app_list_ver = app_list_ver
-        # dynamic_key
-        self.dynamic_key = dynamic_key
-        # result_data
-        self.result_data = result_data
-
-    def validate(self):
-        self.validate_required(self.success, 'success')
-        self.validate_required(self.result_code, 'result_code')
-        self.validate_required(self.result_status, 'result_status')
-        self.validate_required(self.apdid, 'apdid')
-        self.validate_required(self.token, 'token')
-        self.validate_required(self.current_time, 'current_time')
-        self.validate_required(self.version, 'version')
-        self.validate_required(self.vkey_switch, 'vkey_switch')
-        self.validate_required(self.bug_track_switch, 'bug_track_switch')
-        self.validate_required(self.app_list_ver, 'app_list_ver')
-        self.validate_required(self.dynamic_key, 'dynamic_key')
-        self.validate_required(self.result_data, 'result_data')
-        if self.result_data:
-            self.result_data.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.success is not None:
-            result['success'] = self.success
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_status is not None:
-            result['result_status'] = self.result_status
-        if self.apdid is not None:
-            result['apdid'] = self.apdid
-        if self.token is not None:
-            result['token'] = self.token
-        if self.current_time is not None:
-            result['current_time'] = self.current_time
-        if self.version is not None:
-            result['version'] = self.version
-        if self.vkey_switch is not None:
-            result['vkey_switch'] = self.vkey_switch
-        if self.bug_track_switch is not None:
-            result['bug_track_switch'] = self.bug_track_switch
-        if self.app_list_ver is not None:
-            result['app_list_ver'] = self.app_list_ver
-        if self.dynamic_key is not None:
-            result['dynamic_key'] = self.dynamic_key
-        if self.result_data is not None:
-            result['result_data'] = self.result_data.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_status') is not None:
-            self.result_status = m.get('result_status')
-        if m.get('apdid') is not None:
-            self.apdid = m.get('apdid')
-        if m.get('token') is not None:
-            self.token = m.get('token')
-        if m.get('current_time') is not None:
-            self.current_time = m.get('current_time')
-        if m.get('version') is not None:
-            self.version = m.get('version')
-        if m.get('vkey_switch') is not None:
-            self.vkey_switch = m.get('vkey_switch')
-        if m.get('bug_track_switch') is not None:
-            self.bug_track_switch = m.get('bug_track_switch')
-        if m.get('app_list_ver') is not None:
-            self.app_list_ver = m.get('app_list_ver')
-        if m.get('dynamic_key') is not None:
-            self.dynamic_key = m.get('dynamic_key')
-        if m.get('result_data') is not None:
-            temp_model = DeviceRiskReportResultData()
-            self.result_data = temp_model.from_map(m['result_data'])
-        return self
-
-
 class DeviceRiskResp(TeaModel):
     def __init__(
         self,
         apdid: str = None,
         apdid_token: str = None,
         risk_level: int = None,
         risk_desc: str = None,
@@ -773,59 +654,115 @@
 
 class SubmitHksecuritytechGatewayDeviceriskReportResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        result_status: int = None,
-        result: DeviceRiskReportResult = None,
+        success: bool = None,
+        apdid: str = None,
+        token: str = None,
+        current_time: str = None,
+        version: str = None,
+        vkey_switch: str = None,
+        bug_track_switch: str = None,
+        app_list_ver: str = None,
+        dynamic_key: str = None,
+        result_data: DeviceRiskReportResultData = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 1000
-        self.result_status = result_status
-        # result
-        self.result = result
+        # success
+        self.success = success
+        # apdid
+        self.apdid = apdid
+        # token
+        self.token = token
+        # current_time
+        self.current_time = current_time
+        # version
+        self.version = version
+        # vkey_switch
+        self.vkey_switch = vkey_switch
+        # bug_track_switch
+        self.bug_track_switch = bug_track_switch
+        # app_list_ver
+        self.app_list_ver = app_list_ver
+        # dynamic_key
+        self.dynamic_key = dynamic_key
+        # result_data
+        self.result_data = result_data
 
     def validate(self):
-        if self.result:
-            self.result.validate()
+        if self.result_data:
+            self.result_data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.result_status is not None:
-            result['result_status'] = self.result_status
-        if self.result is not None:
-            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        if self.apdid is not None:
+            result['apdid'] = self.apdid
+        if self.token is not None:
+            result['token'] = self.token
+        if self.current_time is not None:
+            result['current_time'] = self.current_time
+        if self.version is not None:
+            result['version'] = self.version
+        if self.vkey_switch is not None:
+            result['vkey_switch'] = self.vkey_switch
+        if self.bug_track_switch is not None:
+            result['bug_track_switch'] = self.bug_track_switch
+        if self.app_list_ver is not None:
+            result['app_list_ver'] = self.app_list_ver
+        if self.dynamic_key is not None:
+            result['dynamic_key'] = self.dynamic_key
+        if self.result_data is not None:
+            result['result_data'] = self.result_data.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('result_status') is not None:
-            self.result_status = m.get('result_status')
-        if m.get('result') is not None:
-            temp_model = DeviceRiskReportResult()
-            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('apdid') is not None:
+            self.apdid = m.get('apdid')
+        if m.get('token') is not None:
+            self.token = m.get('token')
+        if m.get('current_time') is not None:
+            self.current_time = m.get('current_time')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('vkey_switch') is not None:
+            self.vkey_switch = m.get('vkey_switch')
+        if m.get('bug_track_switch') is not None:
+            self.bug_track_switch = m.get('bug_track_switch')
+        if m.get('app_list_ver') is not None:
+            self.app_list_ver = m.get('app_list_ver')
+        if m.get('dynamic_key') is not None:
+            self.dynamic_key = m.get('dynamic_key')
+        if m.get('result_data') is not None:
+            temp_model = DeviceRiskReportResultData()
+            self.result_data = temp_model.from_map(m['result_data'])
         return self
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.3/setup.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.4/setup.py`

 * *Files identical despite different names*

