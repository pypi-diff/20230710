# Comparing `tmp/tencentcloud-sdk-python-soe-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-soe-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.930.tar", last modified: Fri Jul  7 00:31:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.931.tar", last modified: Mon Jul 10 00:51:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-soe-3.0.930.tar` & `tencentcloud-sdk-python-soe-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud_sdk_python_soe.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud_sdk_python_soe.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/
--rw-r--r--   0 root         (0) root         (0)    14652 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65787 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)     5903 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/soe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:31:05.000000 tencentcloud-sdk-python-soe-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/
+-rw-r--r--   0 root         (0) root         (0)    14652 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67959 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/soe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-soe-3.0.930/setup.py` & `tencentcloud-sdk-python-soe-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.931/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.930/README.rst` & `tencentcloud-sdk-python-soe-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.930/tencentcloud_sdk_python_soe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/errorcodes.py` & `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/models.py` & `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -901,14 +901,74 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Tone(AbstractModel):
+    """中文声调检测结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Valid: 检测结果是否有效
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Valid: bool
+        :param _RefTone: 文本标准声调，数值范围[-1,1,2,3,4]
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RefTone: int
+        :param _HypothesisTone: 实际发音声调，数值范围[-1,1,2,3,4]
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HypothesisTone: int
+        """
+        self._Valid = None
+        self._RefTone = None
+        self._HypothesisTone = None
+
+    @property
+    def Valid(self):
+        return self._Valid
+
+    @Valid.setter
+    def Valid(self, Valid):
+        self._Valid = Valid
+
+    @property
+    def RefTone(self):
+        return self._RefTone
+
+    @RefTone.setter
+    def RefTone(self, RefTone):
+        self._RefTone = RefTone
+
+    @property
+    def HypothesisTone(self):
+        return self._HypothesisTone
+
+    @HypothesisTone.setter
+    def HypothesisTone(self, HypothesisTone):
+        self._HypothesisTone = HypothesisTone
+
+
+    def _deserialize(self, params):
+        self._Valid = params.get("Valid")
+        self._RefTone = params.get("RefTone")
+        self._HypothesisTone = params.get("HypothesisTone")
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
 class TransmitOralProcessRequest(AbstractModel):
     """TransmitOralProcess请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1705,24 +1765,28 @@
         :param _PhoneInfos: 音节评估详情
         :type PhoneInfos: list of PhoneInfo
         :param _ReferenceWord: 参考词，目前为保留字段。
         :type ReferenceWord: str
         :param _KeywordTag: 主题词命中标志，0表示没命中，1表示命中
 注意：此字段可能返回 null，表示取不到有效值。
         :type KeywordTag: int
+        :param _Tone: 声调检测结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tone: :class:`tencentcloud.soe.v20180724.models.Tone`
         """
         self._MemBeginTime = None
         self._MemEndTime = None
         self._PronAccuracy = None
         self._PronFluency = None
         self._Word = None
         self._MatchTag = None
         self._PhoneInfos = None
         self._ReferenceWord = None
         self._KeywordTag = None
+        self._Tone = None
 
     @property
     def MemBeginTime(self):
         return self._MemBeginTime
 
     @MemBeginTime.setter
     def MemBeginTime(self, MemBeginTime):
@@ -1788,14 +1852,22 @@
     def KeywordTag(self):
         return self._KeywordTag
 
     @KeywordTag.setter
     def KeywordTag(self, KeywordTag):
         self._KeywordTag = KeywordTag
 
+    @property
+    def Tone(self):
+        return self._Tone
+
+    @Tone.setter
+    def Tone(self, Tone):
+        self._Tone = Tone
+
 
     def _deserialize(self, params):
         self._MemBeginTime = params.get("MemBeginTime")
         self._MemEndTime = params.get("MemEndTime")
         self._PronAccuracy = params.get("PronAccuracy")
         self._PronFluency = params.get("PronFluency")
         self._Word = params.get("Word")
@@ -1804,14 +1876,17 @@
             self._PhoneInfos = []
             for item in params.get("PhoneInfos"):
                 obj = PhoneInfo()
                 obj._deserialize(item)
                 self._PhoneInfos.append(obj)
         self._ReferenceWord = params.get("ReferenceWord")
         self._KeywordTag = params.get("KeywordTag")
+        if params.get("Tone") is not None:
+            self._Tone = Tone()
+            self._Tone._deserialize(params.get("Tone"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-soe-3.0.930/tencentcloud/soe/v20180724/soe_client.py` & `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/soe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/__init__.py`

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

