# Comparing `tmp/azure_storage_helper-0.1.2.tar.gz` & `tmp/azure_storage_helper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_storage_helper-0.1.2.tar", max compression
+gzip compressed data, was "azure_storage_helper-0.1.3.tar", max compression
```

## Comparing `azure_storage_helper-0.1.2.tar` & `azure_storage_helper-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-23 06:04:39.516677 azure_storage_helper-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-23 06:04:51.606033 azure_storage_helper-0.1.2/README.md
--rw-r--r--   0        0        0      137 2023-06-23 06:18:18.233783 azure_storage_helper-0.1.2/azure/gen1/__init__.py
--rw-r--r--   0        0        0    10215 2023-06-26 07:26:42.964073 azure_storage_helper-0.1.2/azure/gen1/gen1.py
--rw-r--r--   0        0        0     2760 2023-06-26 07:26:51.109685 azure_storage_helper-0.1.2/azure/gen1/helper.py
--rw-r--r--   0        0        0      177 2023-06-23 06:18:18.248482 azure_storage_helper-0.1.2/azure/gen2/__init__.py
--rw-r--r--   0        0        0    17089 2023-06-26 07:26:13.491820 azure_storage_helper-0.1.2/azure/gen2/gen2.py
--rw-r--r--   0        0        0     2822 2023-06-26 07:26:28.520023 azure_storage_helper-0.1.2/azure/gen2/helper.py
--rw-r--r--   0        0        0      459 2023-06-26 07:28:12.292110 azure_storage_helper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.2/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-23 06:04:39.516677 azure_storage_helper-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-23 06:04:51.606033 azure_storage_helper-0.1.3/README.md
+-rw-r--r--   0        0        0      137 2023-06-23 06:18:18.233783 azure_storage_helper-0.1.3/azure/gen1/__init__.py
+-rw-r--r--   0        0        0    10363 2023-07-10 06:05:35.768373 azure_storage_helper-0.1.3/azure/gen1/gen1.py
+-rw-r--r--   0        0        0     2760 2023-06-26 07:26:51.109685 azure_storage_helper-0.1.3/azure/gen1/helper.py
+-rw-r--r--   0        0        0      177 2023-06-23 06:18:18.248482 azure_storage_helper-0.1.3/azure/gen2/__init__.py
+-rw-r--r--   0        0        0    17373 2023-07-10 06:05:42.653002 azure_storage_helper-0.1.3/azure/gen2/gen2.py
+-rw-r--r--   0        0        0     2822 2023-06-26 07:26:28.520023 azure_storage_helper-0.1.3/azure/gen2/helper.py
+-rw-r--r--   0        0        0      459 2023-07-10 06:07:06.379394 azure_storage_helper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.3/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.3/PKG-INFO
```

### Comparing `azure_storage_helper-0.1.2/azure/gen1/gen1.py` & `azure_storage_helper-0.1.3/azure/gen1/gen1.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,14 +153,19 @@
         """
         try:
             self.client.create_container(**kwargs)
         except ResourceExistsError as err:
             if not exist_ok:
                 raise err
 
+    def delete(self, **kwargs) -> None:
+        """현재 container를 삭제합니다.
+        """
+        self.client.delete_container(**kwargs)
+
     def glob(self, path: str = None, name_starts_with: str = None) -> list:
         """컨테이너에 존재하는 Blob을 검색합니다.
 
         Args:
             path (str, optional): 현재 컨테이너로부터 검색하려는 디렉토리의 상대 경로.
             Defaults to None.
             name_starts_with (str, optional): Blob 이름의 접두사. Defaults to None.
```

### Comparing `azure_storage_helper-0.1.2/azure/gen1/helper.py` & `azure_storage_helper-0.1.3/azure/gen1/helper.py`

 * *Files identical despite different names*

### Comparing `azure_storage_helper-0.1.2/azure/gen2/gen2.py` & `azure_storage_helper-0.1.3/azure/gen2/gen2.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,19 @@
         """
         try:
             self.client.create_file_system(**kwargs)
         except ResourceExistsError as err:
             if not exist_ok:
                 raise err
 
+    def delete(self, **kwargs) -> None:
+        """Container를 삭제합니다.
+        """
+        self.client.delete_file_system(**kwargs)
+
     def glob(
         self,
         path: str = None,
         name_starts_with: str = None,
         recursive: bool = True,
     ) -> list:
         """컨테이너에 존재하는 Blob을 검색합니다.
@@ -327,14 +332,19 @@
         """
         try:
             self.client.create_directory(**kwargs)
         except ResourceExistsError as err:
             if not exist_ok:
                 raise err
 
+    def delete(self, **kwargs) -> None:
+        """Directory를 삭제합니다.
+        """
+        self.client.delete_directory(**kwargs)
+
     def glob(
         self, name_start_with: str = None, recursive: bool = True
     ) -> list:
         """현재 디렉토리 내 blob을 검색합니다.
 
         Args:
             name_start_with (str, optional): Blob의 접두사 필터. Defaults to None.
```

### Comparing `azure_storage_helper-0.1.2/azure/gen2/helper.py` & `azure_storage_helper-0.1.3/azure/gen2/helper.py`

 * *Files identical despite different names*

### Comparing `azure_storage_helper-0.1.2/setup.py` & `azure_storage_helper-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'azure-storage-file-datalake>=12.9.1,<13.0.0',
  'joblib>=1.2.0,<2.0.0',
  'pandas>=1.5.2',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'azure-storage-helper',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '',
     'author': 'gbhwang',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `azure_storage_helper-0.1.2/PKG-INFO` & `azure_storage_helper-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-storage-helper
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: gbhwang
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

