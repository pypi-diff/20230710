# Comparing `tmp/tencentcloud-sdk-python-tse-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-tse-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tse-3.0.930.tar", last modified: Fri Jul  7 00:35:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tse-3.0.931.tar", last modified: Mon Jul 10 00:55:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tse-3.0.930.tar` & `tencentcloud-sdk-python-tse-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud_sdk_python_tse.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud_sdk_python_tse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud_sdk_python_tse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud_sdk_python_tse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud_sdk_python_tse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/v20201207/
--rw-r--r--   0 root         (0) root         (0)     3508 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/v20201207/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    97961 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/v20201207/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/v20201207/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10224 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/v20201207/tse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:35:42.000000 tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud_sdk_python_tse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud_sdk_python_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud_sdk_python_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud_sdk_python_tse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud_sdk_python_tse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/v20201207/
+-rw-r--r--   0 root         (0) root         (0)     4625 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/v20201207/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   210902 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/v20201207/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/v20201207/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31417 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/v20201207/tse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:55:46.000000 tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/__init__.py
```

### Comparing `tencentcloud-sdk-python-tse-3.0.930/setup.py` & `tencentcloud-sdk-python-tse-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tse-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-tse-3.0.931/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tse
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Tse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tse-3.0.930/README.rst` & `tencentcloud-sdk-python-tse-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tse-3.0.930/tencentcloud_sdk_python_tse.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tse-3.0.931/tencentcloud_sdk_python_tse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tse
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Tse SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tse-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tse-3.0.931/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tse-3.0.930/tencentcloud/tse/v20201207/errorcodes.py` & `tencentcloud-sdk-python-tse-3.0.931/tencentcloud/tse/v20201207/errorcodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,29 @@
 
 # 未授权操作错误。
 AUTHFAILURE_UNAUTHORIZEDOPERATION = 'AuthFailure.UnauthorizedOperation'
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
+# 操作失败。
+FAILEDOPERATION_FAILEDOPERATION = 'FailedOperation.FailedOperation'
+
+# 操作失败，内部错误。
+FAILEDOPERATION_INTERNALERROR = 'FailedOperation.InternalError'
+
+# 获取临时密钥失败
+FAILEDOPERATION_ROLE = 'FailedOperation.Role'
+
+# 调用VPC服务失败
+FAILEDOPERATION_VPC = 'FailedOperation.Vpc'
+
+# 内部错误。
+INTERNALERROR = 'InternalError'
+
 # 创建内部错误。
 INTERNALERROR_CREATEERROR = 'InternalError.CreateError'
 
 # 获取凭证失败。
 INTERNALERROR_GETCREDENTIAL = 'InternalError.GetCredential'
 
 # 角色获取错误。
@@ -73,23 +88,41 @@
 
 # 无效请求参数导致操作失败。
 INVALIDPARAMETERVALUE_OPERATIONFAILED = 'InvalidParameterValue.OperationFailed'
 
 # 无效请求参数，查询失败。
 INVALIDPARAMETERVALUE_QUERYERROR = 'InvalidParameterValue.QueryError'
 
+# 无效的Region。
+INVALIDPARAMETERVALUE_REGION = 'InvalidParameterValue.Region'
+
+# 资源已经存在。
+INVALIDPARAMETERVALUE_RESOURCEALREADYEXIST = 'InvalidParameterValue.ResourceAlreadyExist'
+
+# 网关规格参数内容错误
+INVALIDPARAMETERVALUE_SPECIFICATION = 'InvalidParameterValue.Specification'
+
+# 网关类型参数内容错误
+INVALIDPARAMETERVALUE_TYPE = 'InvalidParameterValue.Type'
+
 # 无效请求参数导致更新失败。
 INVALIDPARAMETERVALUE_UPDATEERROR = 'InvalidParameterValue.UpdateError'
 
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
+# 缺少参数错误。
+MISSINGPARAMETER = 'MissingParameter'
+
 # 缺失参数导致创建失败。
 MISSINGPARAMETER_CREATEERROR = 'MissingParameter.CreateError'
 
+# 缺少参数。
+MISSINGPARAMETER_MISSPARAMETER = 'MissingParameter.MissParameter'
+
 # 缺失参数导致更新失败。
 MISSINGPARAMETER_UPDATEERROR = 'MissingParameter.UpdateError'
 
 # 操作被拒绝。
 OPERATIONDENIED = 'OperationDenied'
 
 # 资源不存在。
@@ -105,7 +138,13 @@
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # cam认证失败。
 UNAUTHORIZEDOPERATION_CAMNOAUTH = 'UnauthorizedOperation.CamNoAuth'
 
 # 子账号缺少passRole权限。
 UNAUTHORIZEDOPERATION_CAMPASSROLENOTEXIST = 'UnauthorizedOperation.CamPassRoleNotExist'
+
+# Uin未授权
+UNAUTHORIZEDOPERATION_UIN = 'UnauthorizedOperation.Uin'
+
+# 未授权的操作。
+UNAUTHORIZEDOPERATION_UNAUTHORIZEDOPERATION = 'UnauthorizedOperation.UnauthorizedOperation'
```

