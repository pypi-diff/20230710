# Comparing `tmp/tencentcloud-sdk-python-dbdc-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-dbdc-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbdc-3.0.930.tar", last modified: Fri Jul  7 00:22:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbdc-3.0.931.tar", last modified: Mon Jul 10 00:38:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbdc-3.0.930.tar` & `tencentcloud-sdk-python-dbdc-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud_sdk_python_dbdc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud_sdk_python_dbdc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud_sdk_python_dbdc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud_sdk_python_dbdc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/
--rw-r--r--   0 root         (0) root         (0)     2111 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    72272 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/dbdc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:22:13.000000 tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud_sdk_python_dbdc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud_sdk_python_dbdc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud_sdk_python_dbdc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud_sdk_python_dbdc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    72272 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/dbdc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:38:49.000000 tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud_sdk_python_dbdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbdc
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Dbdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/setup.py` & `tencentcloud-sdk-python-dbdc-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-dbdc-3.0.931/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbdc
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Dbdc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/README.rst` & `tencentcloud-sdk-python-dbdc-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/errorcodes.py` & `tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/models.py` & `tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/dbdc/v20201029/dbdc_client.py` & `tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/dbdc/v20201029/dbdc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbdc-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbdc-3.0.931/tencentcloud/__init__.py`

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

