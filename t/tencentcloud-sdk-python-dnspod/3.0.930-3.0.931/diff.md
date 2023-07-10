# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.930.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.930.tar", last modified: Fri Jul  7 00:22:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.931.tar", last modified: Mon Jul 10 00:39:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.930.tar` & `tencentcloud-sdk-python-dnspod-3.0.931.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/setup.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    23664 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60713 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)   334940 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:22:36.000000 tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    23664 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60713 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)   340184 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.931/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.931/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.931/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.930
+Version: 3.0.931
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/dnspod/v20210323/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1354,18 +1354,24 @@
         r"""
         :param _Domain: 域名
         :type Domain: str
         :param _GroupId: 域名分组ID。可以通过接口DescribeDomainGroupList查看当前域名分组信息
         :type GroupId: int
         :param _IsMark: 是否星标域名，”yes”、”no” 分别代表是和否。
         :type IsMark: str
+        :param _TransferSubDomain: 添加子域名时，是否迁移相关父域名的解析记录。不传默认为 true
+        :type TransferSubDomain: bool
+        :param _Tags: 域名绑定的标签
+        :type Tags: list of TagItem
         """
         self._Domain = None
         self._GroupId = None
         self._IsMark = None
+        self._TransferSubDomain = None
+        self._Tags = None
 
     @property
     def Domain(self):
         return self._Domain
 
     @Domain.setter
     def Domain(self, Domain):
@@ -1383,19 +1389,42 @@
     def IsMark(self):
         return self._IsMark
 
     @IsMark.setter
     def IsMark(self, IsMark):
         self._IsMark = IsMark
 
+    @property
+    def TransferSubDomain(self):
+        return self._TransferSubDomain
+
+    @TransferSubDomain.setter
+    def TransferSubDomain(self, TransferSubDomain):
+        self._TransferSubDomain = TransferSubDomain
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
 
     def _deserialize(self, params):
         self._Domain = params.get("Domain")
         self._GroupId = params.get("GroupId")
         self._IsMark = params.get("IsMark")
+        self._TransferSubDomain = params.get("TransferSubDomain")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = TagItem()
+                obj._deserialize(item)
+                self._Tags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3617,14 +3646,16 @@
         :type UpdatedAtEnd: str
         :param _RecordCountBegin: 要获取域名的记录数查询区间起点。
         :type RecordCountBegin: int
         :param _RecordCountEnd: 要获取域名的记录数查询区间终点。
         :type RecordCountEnd: int
         :param _ProjectId: 项目ID
         :type ProjectId: int
+        :param _Tags: 标签过滤
+        :type Tags: list of TagItemFilter
         """
         self._Type = None
         self._Offset = None
         self._Limit = None
         self._GroupId = None
         self._Keyword = None
         self._SortField = None
@@ -3633,14 +3664,15 @@
         self._Package = None
         self._Remark = None
         self._UpdatedAtBegin = None
         self._UpdatedAtEnd = None
         self._RecordCountBegin = None
         self._RecordCountEnd = None
         self._ProjectId = None
+        self._Tags = None
 
     @property
     def Type(self):
         return self._Type
 
     @Type.setter
     def Type(self, Type):
@@ -3754,14 +3786,22 @@
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
         self._ProjectId = ProjectId
 
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
 
     def _deserialize(self, params):
         self._Type = params.get("Type")
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
         self._GroupId = params.get("GroupId")
         self._Keyword = params.get("Keyword")
@@ -3771,14 +3811,20 @@
         self._Package = params.get("Package")
         self._Remark = params.get("Remark")
         self._UpdatedAtBegin = params.get("UpdatedAtBegin")
         self._UpdatedAtEnd = params.get("UpdatedAtEnd")
         self._RecordCountBegin = params.get("RecordCountBegin")
         self._RecordCountEnd = params.get("RecordCountEnd")
         self._ProjectId = params.get("ProjectId")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = TagItemFilter()
+                obj._deserialize(item)
+                self._Tags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -3902,20 +3948,23 @@
         :type Offset: int
         :param _Limit: 要获取的域名数量, 比如获取20个, 则为20。默认值为3000。
         :type Limit: int
         :param _GroupId: 分组ID, 获取指定分组的域名
         :type GroupId: int
         :param _Keyword: 根据关键字搜索域名
         :type Keyword: str
+        :param _Tags: 标签过滤
+        :type Tags: list of TagItemFilter
         """
         self._Type = None
         self._Offset = None
         self._Limit = None
         self._GroupId = None
         self._Keyword = None
+        self._Tags = None
 
     @property
     def Type(self):
         return self._Type
 
     @Type.setter
     def Type(self, Type):
@@ -3949,21 +3998,35 @@
     def Keyword(self):
         return self._Keyword
 
     @Keyword.setter
     def Keyword(self, Keyword):
         self._Keyword = Keyword
 
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
 
     def _deserialize(self, params):
         self._Type = params.get("Type")
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
         self._GroupId = params.get("GroupId")
         self._Keyword = params.get("Keyword")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = TagItemFilter()
+                obj._deserialize(item)
+                self._Tags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -6950,14 +7013,17 @@
         :type VipAutoRenew: str
         :param _VipResourceId: VIP套餐资源ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type VipResourceId: str
         :param _IsSubDomain: 是否是子域名。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsSubDomain: bool
+        :param _TagList: 域名关联的标签列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TagList: list of TagItem
         """
         self._DomainId = None
         self._Status = None
         self._Grade = None
         self._GroupId = None
         self._IsMark = None
         self._TTL = None
@@ -6981,14 +7047,15 @@
         self._IsGracePeriod = None
         self._VipBuffered = None
         self._VipStartAt = None
         self._VipEndAt = None
         self._VipAutoRenew = None
         self._VipResourceId = None
         self._IsSubDomain = None
+        self._TagList = None
 
     @property
     def DomainId(self):
         return self._DomainId
 
     @DomainId.setter
     def DomainId(self, DomainId):
@@ -7222,14 +7289,22 @@
     def IsSubDomain(self):
         return self._IsSubDomain
 
     @IsSubDomain.setter
     def IsSubDomain(self, IsSubDomain):
         self._IsSubDomain = IsSubDomain
 
+    @property
+    def TagList(self):
+        return self._TagList
+
+    @TagList.setter
+    def TagList(self, TagList):
+        self._TagList = TagList
+
 
     def _deserialize(self, params):
         self._DomainId = params.get("DomainId")
         self._Status = params.get("Status")
         self._Grade = params.get("Grade")
         self._GroupId = params.get("GroupId")
         self._IsMark = params.get("IsMark")
@@ -7254,14 +7329,20 @@
         self._IsGracePeriod = params.get("IsGracePeriod")
         self._VipBuffered = params.get("VipBuffered")
         self._VipStartAt = params.get("VipStartAt")
         self._VipEndAt = params.get("VipEndAt")
         self._VipAutoRenew = params.get("VipAutoRenew")
         self._VipResourceId = params.get("VipResourceId")
         self._IsSubDomain = params.get("IsSubDomain")
+        if params.get("TagList") is not None:
+            self._TagList = []
+            for item in params.get("TagList"):
+                obj = TagItem()
+                obj._deserialize(item)
+                self._TagList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7315,14 +7396,17 @@
         :type RecordCount: int
         :param _CreatedOn: 域名添加时间
         :type CreatedOn: str
         :param _UpdatedOn: 域名更新时间
         :type UpdatedOn: str
         :param _Owner: 域名所属账号
         :type Owner: str
+        :param _TagList: 域名关联的标签列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TagList: list of TagItem
         """
         self._DomainId = None
         self._Name = None
         self._Status = None
         self._TTL = None
         self._CNAMESpeedup = None
         self._DNSStatus = None
@@ -7338,14 +7422,15 @@
         self._VipStartAt = None
         self._VipEndAt = None
         self._VipAutoRenew = None
         self._RecordCount = None
         self._CreatedOn = None
         self._UpdatedOn = None
         self._Owner = None
+        self._TagList = None
 
     @property
     def DomainId(self):
         return self._DomainId
 
     @DomainId.setter
     def DomainId(self, DomainId):
@@ -7515,14 +7600,22 @@
     def Owner(self):
         return self._Owner
 
     @Owner.setter
     def Owner(self, Owner):
         self._Owner = Owner
 
+    @property
+    def TagList(self):
+        return self._TagList
+
+    @TagList.setter
+    def TagList(self, TagList):
+        self._TagList = TagList
+
 
     def _deserialize(self, params):
         self._DomainId = params.get("DomainId")
         self._Name = params.get("Name")
         self._Status = params.get("Status")
         self._TTL = params.get("TTL")
         self._CNAMESpeedup = params.get("CNAMESpeedup")
@@ -7539,14 +7632,20 @@
         self._VipStartAt = params.get("VipStartAt")
         self._VipEndAt = params.get("VipEndAt")
         self._VipAutoRenew = params.get("VipAutoRenew")
         self._RecordCount = params.get("RecordCount")
         self._CreatedOn = params.get("CreatedOn")
         self._UpdatedOn = params.get("UpdatedOn")
         self._Owner = params.get("Owner")
+        if params.get("TagList") is not None:
+            self._TagList = []
+            for item in params.get("TagList"):
+                obj = TagItem()
+                obj._deserialize(item)
+                self._TagList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -11565,14 +11664,105 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TagItem(AbstractModel):
+    """标签项
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TagKey: 标签键
+        :type TagKey: str
+        :param _TagValue: 标签值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TagValue: str
+        """
+        self._TagKey = None
+        self._TagValue = None
+
+    @property
+    def TagKey(self):
+        return self._TagKey
+
+    @TagKey.setter
+    def TagKey(self, TagKey):
+        self._TagKey = TagKey
+
+    @property
+    def TagValue(self):
+        return self._TagValue
+
+    @TagValue.setter
+    def TagValue(self, TagValue):
+        self._TagValue = TagValue
+
+
+    def _deserialize(self, params):
+        self._TagKey = params.get("TagKey")
+        self._TagValue = params.get("TagValue")
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
+class TagItemFilter(AbstractModel):
+    """标签过滤条件
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TagKey: 标签键
+        :type TagKey: str
+        :param _TagValue: 标签键
+        :type TagValue: list of str
+        """
+        self._TagKey = None
+        self._TagValue = None
+
+    @property
+    def TagKey(self):
+        return self._TagKey
+
+    @TagKey.setter
+    def TagKey(self, TagKey):
+        self._TagKey = TagKey
+
+    @property
+    def TagValue(self):
+        return self._TagValue
+
+    @TagValue.setter
+    def TagValue(self, TagValue):
+        self._TagValue = TagValue
+
+
+    def _deserialize(self, params):
+        self._TagKey = params.get("TagKey")
+        self._TagValue = params.get("TagValue")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class UserInfo(AbstractModel):
     """用户信息
 
     """
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.930/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.931/tencentcloud/__init__.py`

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

