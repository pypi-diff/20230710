# Comparing `tmp/HALchemy-0.1.7-py3-none-any.whl.zip` & `tmp/HALchemy-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5500 bytes, number of entries: 7
+Zip file size: 5493 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-04 01:21 halchemy/__init__.py
--rw-rw-rw-  2.0 fat     6308 b- defN 23-Jul-06 16:47 halchemy/api.py
+-rw-rw-rw-  2.0 fat     6301 b- defN 23-Jul-10 01:34 halchemy/api.py
 -rw-rw-rw-  2.0 fat     2548 b- defN 23-Jul-01 18:46 halchemy/requests_helper.py
--rw-rw-rw-  2.0 fat     1976 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      532 b- defN 23-Jul-09 03:41 HALchemy-0.1.7.dist-info/RECORD
-7 files, 11538 bytes uncompressed, 4558 bytes compressed:  60.5%
+-rw-rw-rw-  2.0 fat     1969 b- defN 23-Jul-10 03:37 HALchemy-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 03:37 HALchemy-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-10 03:37 HALchemy-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      532 b- defN 23-Jul-10 03:37 HALchemy-0.1.8.dist-info/RECORD
+7 files, 11524 bytes uncompressed, 4551 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: halchemy/api.py
 Comment: 
 
 Filename: halchemy/requests_helper.py
 Comment: 
 
-Filename: HALchemy-0.1.7.dist-info/METADATA
+Filename: HALchemy-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: HALchemy-0.1.7.dist-info/WHEEL
+Filename: HALchemy-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: HALchemy-0.1.7.dist-info/top_level.txt
+Filename: HALchemy-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: HALchemy-0.1.7.dist-info/RECORD
+Filename: HALchemy-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## halchemy/api.py

```diff
@@ -135,15 +135,15 @@
             response.raise_for_status()
             return response.json()
         except:
             message = f'{response.status_code} {response.reason}'
             details = response.text
             raise RuntimeError(f'PUT {url}\n{headers}\n{message}\n{details}\n\n{data}')
 
-    def delete_collection(self, url):
+    def delete_url(self, url):
         response = self._api.delete(url)
 
         try:
             response.raise_for_status()
         except:
             message = f'{response.status_code} {response.reason}'
             details = response.text
```

## Comparing `HALchemy-0.1.7.dist-info/METADATA` & `HALchemy-0.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HALchemy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Toolkit for creating clients of HAL based Hypermedia APIs.
 Home-page: https://github.com/pointw-dev/HALchemy
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
@@ -51,12 +51,12 @@
 
 * **get**(self, url='/')
 * **get_from_rel**(self, resource, rel='self', parameters={}, template={})
 * **get_from_rel_with_lookup**(self, resource, rel, lookup, parameters={})
 * **post_to_rel**(self, resource, rel, data, parameters={}, template={})
 * **patch_resource**(self, resource, data)
 * **put_to_rel**(self, resource, data, rel='self')
-* **delete_collection**(self, url)
+* **delete_url**(self, url)
 * **delete_resource**(self, resource)
 * **url_from_rel**(resource, rel, parameters={}, template={})
 * **post_to_url**(self, url, data)
```

