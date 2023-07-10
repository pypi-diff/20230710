# Comparing `tmp/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1.tar.gz` & `tmp/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1.tar", last modified: Thu Jun 29 02:29:38 2023, max compression
+gzip compressed data, was "dist/antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2.tar", last modified: Mon Jul 10 03:58:45 2023, max compression
```

## Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1.tar` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18744 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py
--rw-r--r--   0 root         (0) root         (0)    18230 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-29 02:29:38.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-06-29 02:29:37.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21670 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py
+-rw-r--r--   0 root         (0) root         (0)    29994 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 03:58:45.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-07-10 03:58:44.000000 antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/setup.py
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/LICENSE` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/PKG-INFO` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_8146025f0aa2474a88d81f508253e029
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/README-CN.md` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/README.md` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-8146025f0aa2474a88d81f508253e029
-Version: 1.0.1
+Version: 1.0.2
 Summary: Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_ak_8146025f0aa2474a88d81f508253e029.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/antchain_sdk_ak_8146025f0aa2474a88d81f508253e029/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 设备风险查询data
+            # result.resultData
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.1',
+                    'sdk_version': '1.0.2',
                     '_prod_code': 'ak_8146025f0aa2474a88d81f508253e029',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -210,15 +210,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 设备风险查询data
+            # result.resultData
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.1',
+                    'sdk_version': '1.0.2',
                     '_prod_code': 'ak_8146025f0aa2474a88d81f508253e029',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -382,7 +382,63 @@
         Summary: 设备风险查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.QueryHksecuritytechGatewayDeviceriskDeviceriskResponse(),
             await self.do_request_async('1.0', 'hksecuritytech.gateway.devicerisk.devicerisk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def submit_hksecuritytech_gateway_devicerisk_report(
+        self,
+        request: ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportRequest,
+    ) -> ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_hksecuritytech_gateway_devicerisk_report_ex(request, headers, runtime)
+
+    async def submit_hksecuritytech_gateway_devicerisk_report_async(
+        self,
+        request: ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportRequest,
+    ) -> ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_hksecuritytech_gateway_devicerisk_report_ex_async(request, headers, runtime)
+
+    def submit_hksecuritytech_gateway_devicerisk_report_ex(
+        self,
+        request: ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportResponse(),
+            self.do_request('1.0', 'hksecuritytech.gateway.devicerisk.report.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_hksecuritytech_gateway_devicerisk_report_ex_async(
+        self,
+        request: ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__8146025f_0aa_2474a_88d_81f_508253e_029_models.SubmitHksecuritytechGatewayDeviceriskReportResponse(),
+            await self.do_request_async('1.0', 'hksecuritytech.gateway.devicerisk.report.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.1/setup.py` & `antchain_ak_8146025f0aa2474a88d81f508253e029-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_8146025f0aa2474a88d81f508253e029.
 
-Created on 29/06/2023
+Created on 10/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_8146025f0aa2474a88d81f508253e029"
 NAME = "antchain_ak_8146025f0aa2474a88d81f508253e029" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_8146025f0aa2474a88d81f508253e029 SDK Library for Python"
```

