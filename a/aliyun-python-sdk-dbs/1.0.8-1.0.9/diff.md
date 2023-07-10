# Comparing `tmp/aliyun-python-sdk-dbs-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-dbs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dbs-1.0.8.tar", last modified: Tue May 28 17:00:15 2019, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dbs-1.0.9.tar", last modified: Wed Jun 12 10:30:00 2019, max compression
```

## Comparing `aliyun-python-sdk-dbs-1.0.8.tar` & `aliyun-python-sdk-dbs-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 jenkins    (498) jenkins    (496)        0 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/
--rw-r--r--   0 jenkins    (498) jenkins    (496)      361 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/README.rst
--rw-r--r--   0 jenkins    (498) jenkins    (496)        0 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/MANIFEST.in
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1331 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (496)     2529 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/setup.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (496)        0 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/
--rw-r--r--   0 jenkins    (498) jenkins    (496)       21 2019-05-28 16:53:55.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (496)        0 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/
--rw-r--r--   0 jenkins    (498) jenkins    (496)        0 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/__init__.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (496)        0 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1711 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/ModifyBackupObjectsRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1841 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeFullBackupListRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)        0 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/__init__.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1487 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeNodeCidrListRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     5319 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/CreateRestoreTaskRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     5881 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/ConfigureBackupPlanRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1521 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/StartRestoreTaskRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1851 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeIncrementBackupListRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1989 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeBackupPlanListRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1683 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/StopBackupPlanRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1513 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/StartBackupPlanRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1983 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeBackupGatewayListRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     2345 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/CreateBackupPlanRequest.py
--rw-r--r--   0 jenkins    (498) jenkins    (496)     2033 2019-05-28 16:53:53.000000 aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeRestoreTaskListRequest.py
-drwxr-xr-x   0 jenkins    (498) jenkins    (496)        0 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1331 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (498) jenkins    (496)       31 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (498) jenkins    (496)     1157 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (498) jenkins    (496)        1 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (498) jenkins    (496)       13 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (498) jenkins    (496)       38 2019-05-28 17:00:15.000000 aliyun-python-sdk-dbs-1.0.8/setup.cfg
+drwxrwxr-x   0 admin      (696) admin      (696)        0 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/
+-rw-rw-r--   0 admin      (696) admin      (696)     1321 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/PKG-INFO
+-rw-rw-r--   0 admin      (696) admin      (696)     2452 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/setup.py
+-rw-rw-r--   0 admin      (696) admin      (696)      351 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/README.rst
+drwxrwxr-x   0 admin      (696) admin      (696)        0 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/
+drwxrwxr-x   0 admin      (696) admin      (696)        0 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/
+drwxrwxr-x   0 admin      (696) admin      (696)        0 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/
+-rw-rw-r--   0 admin      (696) admin      (696)     2010 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeRestoreTaskListRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1818 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeFullBackupListRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     2322 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/CreateBackupPlanRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1828 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeIncrementBackupListRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     5858 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/ConfigureBackupPlanRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     5296 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/CreateRestoreTaskRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1798 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/RenewBackupPlanRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1966 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeBackupPlanListRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1688 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/ModifyBackupObjectsRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1490 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/StartBackupPlanRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1464 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeNodeCidrListRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1498 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/StartRestoreTaskRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1660 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/StopBackupPlanRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)     1960 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeBackupGatewayListRequest.py
+-rw-rw-r--   0 admin      (696) admin      (696)        0 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/__init__.py
+-rw-rw-r--   0 admin      (696) admin      (696)        0 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/__init__.py
+-rw-rw-r--   0 admin      (696) admin      (696)       21 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/__init__.py
+drwxrwxr-x   0 admin      (696) admin      (696)        0 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/
+-rw-rw-r--   0 admin      (696) admin      (696)     1321 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/PKG-INFO
+-rw-rw-r--   0 admin      (696) admin      (696)       13 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/top_level.txt
+-rw-rw-r--   0 admin      (696) admin      (696)     1214 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin      (696) admin      (696)        1 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin      (696) admin      (696)       30 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/requires.txt
+-rw-rw-r--   0 admin      (696) admin      (696)        0 2019-06-12 10:29:59.000000 aliyun-python-sdk-dbs-1.0.9/MANIFEST.in
+-rw-rw-r--   0 admin      (696) admin      (696)       59 2019-06-12 10:30:00.000000 aliyun-python-sdk-dbs-1.0.9/setup.cfg
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/PKG-INFO` & `aliyun-python-sdk-dbs-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dbs
-Version: 1.0.8
+Version: 1.0.9
 Summary: The dbs module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
-Description: aliyun-python-sdk-dbs
-        This is the dbs module of Aliyun Python SDK.
-        
-        Aliyun Python SDK is the official software development kit. It makes things easy to integrate your Python application, library, or script with Aliyun services.
-        
-        This module works on Python versions:
-        
-        2.6.5 and greater
-        Documentation:
-        
+Description: aliyun-python-sdk-dbs
+        This is the dbs module of Aliyun Python SDK.
+        
+        Aliyun Python SDK is the official software development kit. It makes things easy to integrate your Python application, library, or script with Aliyun services.
+        
+        This module works on Python versions:
+        
+        2.6.5 and greater
+        Documentation:
+        
         Please visit http://develop.aliyun.com/sdk/python
 Keywords: aliyun,sdk,dbs
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/ModifyBackupObjectsRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/ModifyBackupObjectsRequest.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class ModifyBackupObjectsRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class ModifyBackupObjectsRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'ModifyBackupObjects','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeFullBackupListRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeBackupPlanListRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class DescribeFullBackupListRequest(RpcRequest):
-
-	def __init__(self):
-		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeFullBackupList','cbs')
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class DescribeBackupPlanListRequest(RpcRequest):
+
+	def __init__(self):
+		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeBackupPlanList','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
@@ -37,14 +37,20 @@
 
 	def get_BackupPlanId(self):
 		return self.get_query_params().get('BackupPlanId')
 
 	def set_BackupPlanId(self,BackupPlanId):
 		self.add_query_param('BackupPlanId',BackupPlanId)
 
+	def get_Region(self):
+		return self.get_query_params().get('Region')
+
+	def set_Region(self,Region):
+		self.add_query_param('Region',Region)
+
 	def get_PageNum(self):
 		return self.get_query_params().get('PageNum')
 
 	def set_PageNum(self,PageNum):
 		self.add_query_param('PageNum',PageNum)
 
 	def get_OwnerId(self):
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeNodeCidrListRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeNodeCidrListRequest.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class DescribeNodeCidrListRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class DescribeNodeCidrListRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeNodeCidrList','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/CreateRestoreTaskRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/CreateRestoreTaskRequest.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class CreateRestoreTaskRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class CreateRestoreTaskRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'CreateRestoreTask','cbs')
 
 	def get_BackupGatewayId(self):
 		return self.get_query_params().get('BackupGatewayId')
 
 	def set_BackupGatewayId(self,BackupGatewayId):
 		self.add_query_param('BackupGatewayId',BackupGatewayId)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/ConfigureBackupPlanRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/ConfigureBackupPlanRequest.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class ConfigureBackupPlanRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class ConfigureBackupPlanRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'ConfigureBackupPlan','cbs')
 
 	def get_SourceEndpointRegion(self):
 		return self.get_query_params().get('SourceEndpointRegion')
 
 	def set_SourceEndpointRegion(self,SourceEndpointRegion):
 		self.add_query_param('SourceEndpointRegion',SourceEndpointRegion)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/StartRestoreTaskRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/StartRestoreTaskRequest.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class StartRestoreTaskRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class StartRestoreTaskRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'StartRestoreTask','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeIncrementBackupListRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeIncrementBackupListRequest.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class DescribeIncrementBackupListRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class DescribeIncrementBackupListRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeIncrementBackupList','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeBackupPlanListRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeRestoreTaskListRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class DescribeBackupPlanListRequest(RpcRequest):
-
-	def __init__(self):
-		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeBackupPlanList','cbs')
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class DescribeRestoreTaskListRequest(RpcRequest):
+
+	def __init__(self):
+		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeRestoreTaskList','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
+	def get_RestoreTaskId(self):
+		return self.get_query_params().get('RestoreTaskId')
+
+	def set_RestoreTaskId(self,RestoreTaskId):
+		self.add_query_param('RestoreTaskId',RestoreTaskId)
+
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
 	def get_BackupPlanId(self):
 		return self.get_query_params().get('BackupPlanId')
 
 	def set_BackupPlanId(self,BackupPlanId):
 		self.add_query_param('BackupPlanId',BackupPlanId)
 
-	def get_Region(self):
-		return self.get_query_params().get('Region')
-
-	def set_Region(self,Region):
-		self.add_query_param('Region',Region)
-
 	def get_PageNum(self):
 		return self.get_query_params().get('PageNum')
 
 	def set_PageNum(self,PageNum):
 		self.add_query_param('PageNum',PageNum)
 
 	def get_OwnerId(self):
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/StopBackupPlanRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/StartBackupPlanRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class StopBackupPlanRequest(RpcRequest):
-
-	def __init__(self):
-		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'StopBackupPlan','cbs')
-
-	def get_StopMethod(self):
-		return self.get_query_params().get('StopMethod')
-
-	def set_StopMethod(self,StopMethod):
-		self.add_query_param('StopMethod',StopMethod)
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class StartBackupPlanRequest(RpcRequest):
+
+	def __init__(self):
+		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'StartBackupPlan','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/StartBackupPlanRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/RenewBackupPlanRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class RenewBackupPlanRequest(RpcRequest):
+
+	def __init__(self):
+		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'RenewBackupPlan','cbs')
 
-from aliyunsdkcore.request import RpcRequest
-class StartBackupPlanRequest(RpcRequest):
+	def get_Period(self):
+		return self.get_query_params().get('Period')
 
-	def __init__(self):
-		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'StartBackupPlan','cbs')
+	def set_Period(self,Period):
+		self.add_query_param('Period',Period)
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
@@ -35,8 +41,14 @@
 	def set_BackupPlanId(self,BackupPlanId):
 		self.add_query_param('BackupPlanId',BackupPlanId)
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_UsedTime(self):
+		return self.get_query_params().get('UsedTime')
+
+	def set_UsedTime(self,UsedTime):
+		self.add_query_param('UsedTime',UsedTime)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeBackupGatewayListRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeBackupGatewayListRequest.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class DescribeBackupGatewayListRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class DescribeBackupGatewayListRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeBackupGatewayList','cbs')
 
 	def get_Identifier(self):
 		return self.get_query_params().get('Identifier')
 
 	def set_Identifier(self,Identifier):
 		self.add_query_param('Identifier',Identifier)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/CreateBackupPlanRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/CreateBackupPlanRequest.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class CreateBackupPlanRequest(RpcRequest):
-
-	def __init__(self):
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class CreateBackupPlanRequest(RpcRequest):
+
+	def __init__(self):
 		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'CreateBackupPlan','cbs')
 
 	def get_BackupMethod(self):
 		return self.get_query_params().get('BackupMethod')
 
 	def set_BackupMethod(self,BackupMethod):
 		self.add_query_param('BackupMethod',BackupMethod)
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyunsdkdbs/request/v20190306/DescribeRestoreTaskListRequest.py` & `aliyun-python-sdk-dbs-1.0.9/aliyunsdkdbs/request/v20190306/DescribeFullBackupListRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-#
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-
-from aliyunsdkcore.request import RpcRequest
-class DescribeRestoreTaskListRequest(RpcRequest):
-
-	def __init__(self):
-		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeRestoreTaskList','cbs')
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+#
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+from aliyunsdkcore.request import RpcRequest
+class DescribeFullBackupListRequest(RpcRequest):
+
+	def __init__(self):
+		RpcRequest.__init__(self, 'Dbs', '2019-03-06', 'DescribeFullBackupList','cbs')
 
 	def get_ClientToken(self):
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self,ClientToken):
 		self.add_query_param('ClientToken',ClientToken)
 
-	def get_RestoreTaskId(self):
-		return self.get_query_params().get('RestoreTaskId')
-
-	def set_RestoreTaskId(self,RestoreTaskId):
-		self.add_query_param('RestoreTaskId',RestoreTaskId)
-
 	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self,PageSize):
 		self.add_query_param('PageSize',PageSize)
 
 	def get_BackupPlanId(self):
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/PKG-INFO` & `aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dbs
-Version: 1.0.8
+Version: 1.0.9
 Summary: The dbs module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
-Description: aliyun-python-sdk-dbs
-        This is the dbs module of Aliyun Python SDK.
-        
-        Aliyun Python SDK is the official software development kit. It makes things easy to integrate your Python application, library, or script with Aliyun services.
-        
-        This module works on Python versions:
-        
-        2.6.5 and greater
-        Documentation:
-        
+Description: aliyun-python-sdk-dbs
+        This is the dbs module of Aliyun Python SDK.
+        
+        Aliyun Python SDK is the official software development kit. It makes things easy to integrate your Python application, library, or script with Aliyun services.
+        
+        This module works on Python versions:
+        
+        2.6.5 and greater
+        Documentation:
+        
         Please visit http://develop.aliyun.com/sdk/python
 Keywords: aliyun,sdk,dbs
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `aliyun-python-sdk-dbs-1.0.8/aliyun_python_sdk_dbs.egg-info/SOURCES.txt` & `aliyun-python-sdk-dbs-1.0.9/aliyun_python_sdk_dbs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 aliyunsdkdbs/request/v20190306/DescribeBackupGatewayListRequest.py
 aliyunsdkdbs/request/v20190306/DescribeBackupPlanListRequest.py
 aliyunsdkdbs/request/v20190306/DescribeFullBackupListRequest.py
 aliyunsdkdbs/request/v20190306/DescribeIncrementBackupListRequest.py
 aliyunsdkdbs/request/v20190306/DescribeNodeCidrListRequest.py
 aliyunsdkdbs/request/v20190306/DescribeRestoreTaskListRequest.py
 aliyunsdkdbs/request/v20190306/ModifyBackupObjectsRequest.py
+aliyunsdkdbs/request/v20190306/RenewBackupPlanRequest.py
 aliyunsdkdbs/request/v20190306/StartBackupPlanRequest.py
 aliyunsdkdbs/request/v20190306/StartRestoreTaskRequest.py
 aliyunsdkdbs/request/v20190306/StopBackupPlanRequest.py
 aliyunsdkdbs/request/v20190306/__init__.py
```

