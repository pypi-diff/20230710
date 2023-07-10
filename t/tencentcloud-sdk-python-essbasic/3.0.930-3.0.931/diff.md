# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.930.tar", last modified: Fri Jul  7 00:23:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.931.tar", last modified: Mon Jul 10 00:40:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.930.tar` & `tencentcloud-sdk-python-essbasic-3.0.931.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/essbasic_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   375355 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52742 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/essbasic_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   375558 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52742 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:40:39.000000 tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.931/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         r"""
         :param _AppId: 应用的唯一标识。不同的业务系统可以采用不同的AppId，不同AppId下的数据是隔离的。可以由控制台开发者中心-应用集成自主生成。
         :type AppId: str
         :param _ProxyOrganizationOpenId: 第三方应用平台自定义，对应第三方平台子客企业的唯一标识。一个第三方平台子客企业主体与子客企业ProxyOrganizationOpenId是一一对应的，不可更改，不可重复使用。（例如，可以使用企业名称的hash值，或者社会统一信用代码的hash值，或者随机hash值，需要第三方应用平台保存），最大64位字符串
         :type ProxyOrganizationOpenId: str
         :param _ProxyOperator: 第三方平台子客企业中的员工/经办人，通过第三方应用平台进入电子签完成实名、且被赋予相关权限后，可以参与到企业资源的管理或签署流程中。
         :type ProxyOperator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
-        :param _ProxyAppId: 在第三方平台子客企业开通电子签后，会生成唯一的子客应用Id（ProxyAppId）用于代理调用时的鉴权，在子客开通的回调中获取。
+        :param _ProxyAppId: 非必需参数，在第三方平台子客企业开通电子签后，会生成唯一的子客应用Id（ProxyAppId）用于代理调用时的鉴权，在子客开通的回调中获取。
         :type ProxyAppId: str
         :param _ProxyOrganizationId: 内部参数，暂未开放使用
         :type ProxyOrganizationId: str
         """
         self._AppId = None
         self._ProxyOrganizationOpenId = None
         self._ProxyOperator = None
@@ -2404,17 +2404,17 @@
         :type ResourceId: str
         :param _ResourceType: 资源类型，1：模板，目前仅支持模板，与ResourceId对应
         :type ResourceType: int
         :param _FlowInfo: 合同流程基础信息
         :type FlowInfo: :class:`tencentcloud.essbasic.v20210526.models.BaseFlowInfo`
         :param _FlowApproverList: 合同签署人信息
         :type FlowApproverList: list of CommonFlowApprover
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param _FlowOption: 合同流程配置信息
+        :param _FlowOption: 合同流程配置信息，用于配置发起合同时定制化
         :type FlowOption: :class:`tencentcloud.essbasic.v20210526.models.CreateFlowOption`
         :param _FlowId: 通过flowid快速获得之前成功通过页面发起的合同生成链接
         :type FlowId: str
         :param _NeedPreview: 该参数不可用，请通过获取 web 可嵌入接口获取合同流程预览 URL
         :type NeedPreview: bool
         :param _Organization: 企业机构信息，不用传
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
@@ -2486,18 +2486,22 @@
 
     @FlowId.setter
     def FlowId(self, FlowId):
         self._FlowId = FlowId
 
     @property
     def NeedPreview(self):
+        warnings.warn("parameter `NeedPreview` is deprecated", DeprecationWarning) 
+
         return self._NeedPreview
 
     @NeedPreview.setter
     def NeedPreview(self, NeedPreview):
+        warnings.warn("parameter `NeedPreview` is deprecated", DeprecationWarning) 
+
         self._NeedPreview = NeedPreview
 
     @property
     def Organization(self):
         warnings.warn("parameter `Organization` is deprecated", DeprecationWarning) 
 
         return self._Organization
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.931/tencentcloud/__init__.py`

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

