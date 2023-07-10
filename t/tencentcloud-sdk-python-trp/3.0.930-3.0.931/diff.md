# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.930.tar", last modified: Fri Jul  7 00:35:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.931.tar", last modified: Mon Jul 10 00:55:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.930.tar` & `tencentcloud-sdk-python-trp-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud_sdk_python_trp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)      992 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   244279 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45620 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:35:26.000000 tencentcloud-sdk-python-trp-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   244909 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45620 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:55:31.000000 tencentcloud-sdk-python-trp-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-trp-3.0.930/setup.py` & `tencentcloud-sdk-python-trp-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.931/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.930/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.931/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.930/README.rst` & `tencentcloud-sdk-python-trp-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4819,26 +4819,32 @@
     """
 
     def __init__(self):
         r"""
         :param _CorpId: 企业ID, 默认为当前企业
 如果有渠道权限，可以传 0 会查渠道下所有的企业
         :type CorpId: int
-        :param _PageSize: 分页数量，默认为 100，最大为 1000
+        :param _PageSize: 分页数量，默认为 20，最大为 1000
         :type PageSize: int
         :param _PageNumber: 当前分页，默认为 1
         :type PageNumber: int
         :param _AfterLogId: 从哪个日志后查询
 即: LogId > $AfterLogId
         :type AfterLogId: int
+        :param _StartTime: 开始时间 >= StartTime
+        :type StartTime: str
+        :param _EndTime: 结束时间 < EndTime
+        :type EndTime: str
         """
         self._CorpId = None
         self._PageSize = None
         self._PageNumber = None
         self._AfterLogId = None
+        self._StartTime = None
+        self._EndTime = None
 
     @property
     def CorpId(self):
         return self._CorpId
 
     @CorpId.setter
     def CorpId(self, CorpId):
@@ -4864,20 +4870,38 @@
     def AfterLogId(self):
         return self._AfterLogId
 
     @AfterLogId.setter
     def AfterLogId(self, AfterLogId):
         self._AfterLogId = AfterLogId
 
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
 
     def _deserialize(self, params):
         self._CorpId = params.get("CorpId")
         self._PageSize = params.get("PageSize")
         self._PageNumber = params.get("PageNumber")
         self._AfterLogId = params.get("AfterLogId")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-trp-3.0.930/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.931/tencentcloud/trp/v20210515/trp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.931/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.930'
+__version__ = '3.0.931'
```

