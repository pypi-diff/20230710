# Comparing `tmp/tencentcloud-sdk-python-gse-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-gse-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gse-3.0.930.tar", last modified: Fri Jul  7 00:24:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gse-3.0.931.tar", last modified: Mon Jul 10 00:41:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gse-3.0.930.tar` & `tencentcloud-sdk-python-gse-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud_sdk_python_gse.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud_sdk_python_gse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud_sdk_python_gse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud_sdk_python_gse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud_sdk_python_gse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/
--rw-r--r--   0 root         (0) root         (0)     2578 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89075 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/gse_client.py
--rw-r--r--   0 root         (0) root         (0)   387109 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:24:56.000000 tencentcloud-sdk-python-gse-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud_sdk_python_gse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud_sdk_python_gse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud_sdk_python_gse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud_sdk_python_gse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud_sdk_python_gse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89075 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/gse_client.py
+-rw-r--r--   0 root         (0) root         (0)   387109 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:41:31.000000 tencentcloud-sdk-python-gse-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-gse-3.0.930/setup.py` & `tencentcloud-sdk-python-gse-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-gse-3.0.931/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gse
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Gse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gse-3.0.930/tencentcloud_sdk_python_gse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gse-3.0.931/tencentcloud_sdk_python_gse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gse
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Gse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gse-3.0.930/README.rst` & `tencentcloud-sdk-python-gse-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/errorcodes.py` & `tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/gse_client.py` & `tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/gse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.930/tencentcloud/gse/v20191112/models.py` & `tencentcloud-sdk-python-gse-3.0.931/tencentcloud/gse/v20191112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gse-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gse-3.0.931/tencentcloud/__init__.py`

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

