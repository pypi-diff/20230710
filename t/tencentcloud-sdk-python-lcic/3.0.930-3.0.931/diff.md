# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.930.tar", last modified: Fri Jul  7 00:26:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.931.tar", last modified: Mon Jul 10 00:43:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.930.tar` & `tencentcloud-sdk-python-lcic-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4414 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   227598 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    48649 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:26:52.000000 tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229078 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    48649 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:43:24.000000 tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/setup.py` & `tencentcloud-sdk-python-lcic-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.931/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.931/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/README.rst` & `tencentcloud-sdk-python-lcic-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5414,20 +5414,23 @@
         :type StartTime: int
         :param _EndTime: 结束时间。默认以当前时间加上半小时作为结束时间。
         :type EndTime: int
         :param _Page: 分页查询当前页数，从1开始递增
         :type Page: int
         :param _Limit: 默认是10条
         :type Limit: int
+        :param _Status: 课堂状态。默认展示所有课堂，0为未开始，1为正在上课，2为已结束，3为已过期
+        :type Status: list of int non-negative
         """
         self._SdkAppId = None
         self._StartTime = None
         self._EndTime = None
         self._Page = None
         self._Limit = None
+        self._Status = None
 
     @property
     def SdkAppId(self):
         return self._SdkAppId
 
     @SdkAppId.setter
     def SdkAppId(self, SdkAppId):
@@ -5461,21 +5464,30 @@
     def Limit(self):
         return self._Limit
 
     @Limit.setter
     def Limit(self, Limit):
         self._Limit = Limit
 
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
 
     def _deserialize(self, params):
         self._SdkAppId = params.get("SdkAppId")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._Page = params.get("Page")
         self._Limit = params.get("Limit")
+        self._Status = params.get("Status")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7512,28 +7524,36 @@
         :type RecordUrl: str
         :param _MaxMicNumber: 最高房间内人数（包括老师），0表示不限制，默认为0
 注意：此字段可能返回 null，表示取不到有效值。
         :type MaxMicNumber: int
         :param _EnableDirectControl: 打开学生麦克风/摄像头的授权开关 
 注意：此字段可能返回 null，表示取不到有效值。
         :type EnableDirectControl: int
+        :param _InteractionMode: 开启专注模式。 0 收看全部角色音视频(默认) 1 只看老师和助教
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InteractionMode: int
+        :param _VideoOrientation: 横竖屏。0：横屏开播（默认值）; 1：竖屏开播，当前仅支持移动端的纯视频类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VideoOrientation: int
         """
         self._Name = None
         self._RoomId = None
         self._Status = None
         self._StartTime = None
         self._EndTime = None
         self._RealStartTime = None
         self._RealEndTime = None
         self._Resolution = None
         self._MaxRTCMember = None
         self._ReplayUrl = None
         self._RecordUrl = None
         self._MaxMicNumber = None
         self._EnableDirectControl = None
+        self._InteractionMode = None
+        self._VideoOrientation = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -7631,14 +7651,30 @@
     def EnableDirectControl(self):
         return self._EnableDirectControl
 
     @EnableDirectControl.setter
     def EnableDirectControl(self, EnableDirectControl):
         self._EnableDirectControl = EnableDirectControl
 
+    @property
+    def InteractionMode(self):
+        return self._InteractionMode
+
+    @InteractionMode.setter
+    def InteractionMode(self, InteractionMode):
+        self._InteractionMode = InteractionMode
+
+    @property
+    def VideoOrientation(self):
+        return self._VideoOrientation
+
+    @VideoOrientation.setter
+    def VideoOrientation(self, VideoOrientation):
+        self._VideoOrientation = VideoOrientation
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._RoomId = params.get("RoomId")
         self._Status = params.get("Status")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
@@ -7646,14 +7682,16 @@
         self._RealEndTime = params.get("RealEndTime")
         self._Resolution = params.get("Resolution")
         self._MaxRTCMember = params.get("MaxRTCMember")
         self._ReplayUrl = params.get("ReplayUrl")
         self._RecordUrl = params.get("RecordUrl")
         self._MaxMicNumber = params.get("MaxMicNumber")
         self._EnableDirectControl = params.get("EnableDirectControl")
+        self._InteractionMode = params.get("InteractionMode")
+        self._VideoOrientation = params.get("VideoOrientation")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.931/tencentcloud/__init__.py`

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

