# Comparing `tmp/antchain_hk_securitytech-1.3.2.tar.gz` & `tmp/antchain_hk_securitytech-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_hk_securitytech-1.3.2.tar", last modified: Mon Jul  3 09:22:54 2023, max compression
+gzip compressed data, was "dist/antchain_hk_securitytech-1.3.5.tar", last modified: Mon Jul 10 08:18:52 2023, max compression
```

## Comparing `antchain_hk_securitytech-1.3.2.tar` & `antchain_hk_securitytech-1.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2234 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      840 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2234 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26858 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/client.py
--rw-r--r--   0 root         (0) root         (0)    42759 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 09:22:54.000000 antchain_hk_securitytech-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2550 2023-07-03 09:22:53.000000 antchain_hk_securitytech-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29160 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/client.py
+-rw-r--r--   0 root         (0) root         (0)    56622 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/setup.py
```

### Comparing `antchain_hk_securitytech-1.3.2/LICENSE` & `antchain_hk_securitytech-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.3.2/PKG-INFO` & `antchain_hk_securitytech-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_hk_securitytech
-Version: 1.3.2
+Version: 1.3.5
 Summary: Ant Chain HK_SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_hk_securitytech-1.3.2/README-CN.md` & `antchain_hk_securitytech-1.3.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.3.2/README.md` & `antchain_hk_securitytech-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.3.2/antchain_hk_securitytech.egg-info/PKG-INFO` & `antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-hk-securitytech
-Version: 1.3.2
+Version: 1.3.5
 Summary: Ant Chain HK_SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/client.py` & `antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 人脸盾结果
-            # 
+            # result.resultData
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -132,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.2',
+                    'sdk_version': '1.3.5',
                     '_prod_code': 'HK_SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -211,16 +210,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 人脸盾结果
-            # 
+            # result.resultData
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -237,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.2',
+                    'sdk_version': '1.3.5',
                     '_prod_code': 'HK_SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -608,7 +606,63 @@
         Summary: 人脸盾Web查询
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             hk__securitytech_models.QueryFaceshieldWebResponse(),
             await self.do_request_async('1.0', 'hksecuritytech.gateway.faceshield.web.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def submit_devicerisk_report(
+        self,
+        request: hk__securitytech_models.SubmitDeviceriskReportRequest,
+    ) -> hk__securitytech_models.SubmitDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_devicerisk_report_ex(request, headers, runtime)
+
+    async def submit_devicerisk_report_async(
+        self,
+        request: hk__securitytech_models.SubmitDeviceriskReportRequest,
+    ) -> hk__securitytech_models.SubmitDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_devicerisk_report_ex_async(request, headers, runtime)
+
+    def submit_devicerisk_report_ex(
+        self,
+        request: hk__securitytech_models.SubmitDeviceriskReportRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> hk__securitytech_models.SubmitDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            hk__securitytech_models.SubmitDeviceriskReportResponse(),
+            self.do_request('1.0', 'hksecuritytech.gateway.devicerisk.report.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_devicerisk_report_ex_async(
+        self,
+        request: hk__securitytech_models.SubmitDeviceriskReportRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> hk__securitytech_models.SubmitDeviceriskReportResponse:
+        """
+        Description: 终端安全 设备信息上报
+        Summary: 设备信息上报
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            hk__securitytech_models.SubmitDeviceriskReportResponse(),
+            await self.do_request_async('1.0', 'hksecuritytech.gateway.devicerisk.report.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_hk_securitytech-1.3.2/antchain_sdk_hk_securitytech/models.py` & `antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -150,14 +150,114 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
+class DeviceRiskReportResultData(TeaModel):
+    def __init__(
+        self,
+        webrtc_url: str = None,
+        a_dynamic_swi: str = None,
+        dynamic_interval: str = None,
+        color: str = None,
+        os: str = None,
+        dynamic_cmd: str = None,
+        time_interval: str = None,
+        dynamic_trace: str = None,
+        dynamic_num: str = None,
+        result_type: str = None,
+    ):
+        # webrtc_url
+        self.webrtc_url = webrtc_url
+        # a_dynamic_swi
+        self.a_dynamic_swi = a_dynamic_swi
+        # dynamic_interval
+        self.dynamic_interval = dynamic_interval
+        # color
+        self.color = color
+        # os
+        self.os = os
+        # dynamic_cmd
+        self.dynamic_cmd = dynamic_cmd
+        # time_interval
+        self.time_interval = time_interval
+        # dynamic_trace
+        self.dynamic_trace = dynamic_trace
+        # dynamic_num
+        self.dynamic_num = dynamic_num
+        # result_type
+        self.result_type = result_type
+
+    def validate(self):
+        self.validate_required(self.webrtc_url, 'webrtc_url')
+        self.validate_required(self.a_dynamic_swi, 'a_dynamic_swi')
+        self.validate_required(self.dynamic_interval, 'dynamic_interval')
+        self.validate_required(self.color, 'color')
+        self.validate_required(self.os, 'os')
+        self.validate_required(self.dynamic_cmd, 'dynamic_cmd')
+        self.validate_required(self.time_interval, 'time_interval')
+        self.validate_required(self.dynamic_trace, 'dynamic_trace')
+        self.validate_required(self.dynamic_num, 'dynamic_num')
+        self.validate_required(self.result_type, 'result_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.webrtc_url is not None:
+            result['webrtc_url'] = self.webrtc_url
+        if self.a_dynamic_swi is not None:
+            result['a_dynamic_swi'] = self.a_dynamic_swi
+        if self.dynamic_interval is not None:
+            result['dynamic_interval'] = self.dynamic_interval
+        if self.color is not None:
+            result['color'] = self.color
+        if self.os is not None:
+            result['os'] = self.os
+        if self.dynamic_cmd is not None:
+            result['dynamic_cmd'] = self.dynamic_cmd
+        if self.time_interval is not None:
+            result['time_interval'] = self.time_interval
+        if self.dynamic_trace is not None:
+            result['dynamic_trace'] = self.dynamic_trace
+        if self.dynamic_num is not None:
+            result['dynamic_num'] = self.dynamic_num
+        if self.result_type is not None:
+            result['result_type'] = self.result_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('webrtc_url') is not None:
+            self.webrtc_url = m.get('webrtc_url')
+        if m.get('a_dynamic_swi') is not None:
+            self.a_dynamic_swi = m.get('a_dynamic_swi')
+        if m.get('dynamic_interval') is not None:
+            self.dynamic_interval = m.get('dynamic_interval')
+        if m.get('color') is not None:
+            self.color = m.get('color')
+        if m.get('os') is not None:
+            self.os = m.get('os')
+        if m.get('dynamic_cmd') is not None:
+            self.dynamic_cmd = m.get('dynamic_cmd')
+        if m.get('time_interval') is not None:
+            self.time_interval = m.get('time_interval')
+        if m.get('dynamic_trace') is not None:
+            self.dynamic_trace = m.get('dynamic_trace')
+        if m.get('dynamic_num') is not None:
+            self.dynamic_num = m.get('dynamic_num')
+        if m.get('result_type') is not None:
+            self.result_type = m.get('result_type')
+        return self
+
+
 class FaceShieldResult(TeaModel):
     def __init__(
         self,
         apdid_token: str = None,
         risk_level: int = None,
         risk_desc: str = None,
         sug_action: str = None,
@@ -205,14 +305,133 @@
         if m.get('risk_desc') is not None:
             self.risk_desc = m.get('risk_desc')
         if m.get('sug_action') is not None:
             self.sug_action = m.get('sug_action')
         return self
 
 
+class DeviceRiskReportResult(TeaModel):
+    def __init__(
+        self,
+        success: bool = None,
+        result_code: str = None,
+        result_status: str = None,
+        apdid: str = None,
+        token: str = None,
+        current_time: str = None,
+        version: str = None,
+        vkey_switch: str = None,
+        bug_track_switch: str = None,
+        app_list_ver: str = None,
+        dynamic_key: str = None,
+        result_data: DeviceRiskReportResultData = None,
+    ):
+        # success
+        self.success = success
+        # result_code
+        self.result_code = result_code
+        # result_status
+        self.result_status = result_status
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
+
+    def validate(self):
+        self.validate_required(self.success, 'success')
+        self.validate_required(self.result_code, 'result_code')
+        self.validate_required(self.result_status, 'result_status')
+        self.validate_required(self.apdid, 'apdid')
+        self.validate_required(self.token, 'token')
+        self.validate_required(self.current_time, 'current_time')
+        self.validate_required(self.version, 'version')
+        self.validate_required(self.vkey_switch, 'vkey_switch')
+        self.validate_required(self.bug_track_switch, 'bug_track_switch')
+        self.validate_required(self.app_list_ver, 'app_list_ver')
+        self.validate_required(self.dynamic_key, 'dynamic_key')
+        self.validate_required(self.result_data, 'result_data')
+        if self.result_data:
+            self.result_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.success is not None:
+            result['success'] = self.success
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_status is not None:
+            result['result_status'] = self.result_status
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
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_status') is not None:
+            self.result_status = m.get('result_status')
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
+        return self
+
+
 class ClassMethodConfig(TeaModel):
     def __init__(
         self,
         class_name: str = None,
         methods: str = None,
     ):
         # 加固类名
@@ -1227,7 +1446,162 @@
             self.request_id = m.get('request_id')
         if m.get('data') is not None:
             temp_model = FaceShieldResult()
             self.data = temp_model.from_map(m['data'])
         return self
 
 
+class SubmitDeviceriskReportRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        request_data: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # request_data
+        self.request_data = request_data
+
+    def validate(self):
+        self.validate_required(self.request_data, 'request_data')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.request_data is not None:
+            result['request_data'] = self.request_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('request_data') is not None:
+            self.request_data = m.get('request_data')
+        return self
+
+
+class SubmitDeviceriskReportResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
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
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+
+    def validate(self):
+        if self.result_data:
+            self.result_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
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
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
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
+        return self
+
+
```

### Comparing `antchain_hk_securitytech-1.3.2/setup.py` & `antchain_hk_securitytech-1.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_hk_securitytech.
 
-Created on 03/07/2023
+Created on 10/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_hk_securitytech"
 NAME = "antchain_hk_securitytech" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain HK_SECURITYTECH SDK Library for Python"
```

