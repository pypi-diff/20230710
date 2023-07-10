# Comparing `tmp/tencentcloud-sdk-python-lighthouse-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-lighthouse-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.930.tar", last modified: Fri Jul  7 00:26:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lighthouse-3.0.931.tar", last modified: Mon Jul 10 00:43:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lighthouse-3.0.930.tar` & `tencentcloud-sdk-python-lighthouse-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)    26127 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   360051 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)    92544 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/lighthouse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:58.000000 tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)    26127 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   360397 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)    92544 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:43:28.000000 tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/__init__.py
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/setup.py` & `tencentcloud-sdk-python-lighthouse-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.931/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud_sdk_python_lighthouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lighthouse
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Lighthouse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/README.rst` & `tencentcloud-sdk-python-lighthouse-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9192,19 +9192,16 @@
 
     def __init__(self):
         r"""
         :param _AutoGeneratePassword: <li>"YES"代表选择自动生成密码，这时不指定Password字段。</li>
 <li>"NO"代表选择自定义密码，这时要指定Password字段。</li>
         :type AutoGeneratePassword: str
         :param _Password: 实例登录密码。具体按照操作系统的复杂度要求。 
-WINDOWS 实例密码必须 12-30 位，不能以“/”开头且不包括用户名, 至少包含以下字符中的三种不同字符 
-<li>小写字母：[a-z]</li>
-<li>大写字母：[A-Z]</li>
-<li>数字： 0-9</li>
-<li>特殊字符：()`~!@#$%^&*-+=_|{}[]:;' <>,.?/</li>
+`LINUX_UNIX` 实例密码必须 8-30 位，推荐使用 12 位以上密码，不能包含空格, 不能以“/”开头，至少包含以下字符中的三种不同字符，字符种类：<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字：0-9<br><li>特殊字符： ()\`\~!@#$%^&\*-+=\_|{}[]:;' <>,.?/</li>
+`WINDOWS` 实例密码必须 12-30 位，不能包含空格, 不能以“/”开头且不包括用户名，至少包含以下字符中的三种不同字符<br><li>小写字母：[a-z]<br><li>大写字母：[A-Z]<br><li>数字： 0-9<br><li>特殊字符：()\`~!@#$%^&\*-+=\_|{}[]:;' <>,.?/
         :type Password: str
         """
         self._AutoGeneratePassword = None
         self._Password = None
 
     @property
     def AutoGeneratePassword(self):
```

### Comparing `tencentcloud-sdk-python-lighthouse-3.0.930/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-lighthouse-3.0.931/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

