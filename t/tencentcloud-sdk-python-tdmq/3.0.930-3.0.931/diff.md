# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.930.tar", last modified: Fri Jul  7 00:33:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.931.tar", last modified: Mon Jul 10 00:53:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.930.tar` & `tencentcloud-sdk-python-tdmq-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   110163 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   658825 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:33:31.000000 tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   111089 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   661043 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:53:54.000000 tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.931/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,14 +870,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteRabbitMQVipInstance(self, request):
+        """删除RabbitMQ专享版实例
+
+        :param request: Request instance for DeleteRabbitMQVipInstance.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVipInstanceRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVipInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteRabbitMQVipInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteRabbitMQVipInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteRabbitMQVirtualHost(self, request):
         """删除RabbitMQ的vhost
 
         :param request: Request instance for DeleteRabbitMQVirtualHost.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVirtualHostRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.DeleteRabbitMQVirtualHostResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6552,14 +6552,98 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DeleteRabbitMQVipInstanceRequest(AbstractModel):
+    """DeleteRabbitMQVipInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例Id
+        :type InstanceId: str
+        """
+        self._InstanceId = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteRabbitMQVipInstanceResponse(AbstractModel):
+    """DeleteRabbitMQVipInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TranId: 订单号Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TranId: str
+        :param _InstanceId: 实例Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TranId = None
+        self._InstanceId = None
+        self._RequestId = None
+
+    @property
+    def TranId(self):
+        return self._TranId
+
+    @TranId.setter
+    def TranId(self, TranId):
+        self._TranId = TranId
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._TranId = params.get("TranId")
+        self._InstanceId = params.get("InstanceId")
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteRabbitMQVirtualHostRequest(AbstractModel):
     """DeleteRabbitMQVirtualHost请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.930/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.931/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

