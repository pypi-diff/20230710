# Comparing `tmp/pubtools-content-gateway-0.4.0.tar.gz` & `tmp/pubtools-content-gateway-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubtools-content-gateway-0.4.0.tar", last modified: Wed Feb  1 08:14:11 2023, max compression
+gzip compressed data, was "pubtools-content-gateway-0.5.1.tar", last modified: Mon Jul 10 07:29:36 2023, max compression
```

## Comparing `pubtools-content-gateway-0.4.0.tar` & `pubtools-content-gateway-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 08:14:11.236576 pubtools-content-gateway-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-01 08:14:11.236576 pubtools-content-gateway-0.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 08:14:11.232576 pubtools-content-gateway-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/_content_gateway.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/entrypoints_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/push_base.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/push_cgw.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/docs/push_staged_cgw.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 08:14:11.232576 pubtools-content-gateway-0.4.0/pubtools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 08:14:11.232576 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/cgw_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/cgw_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/cgw_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    29843 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/push_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/push_cgw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/push_staged_cgw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/pubtools/_content_gateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 08:14:11.236576 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-01 08:14:11.000000 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-01 08:14:11.000000 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 08:14:11.000000 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-01 08:14:11.000000 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-01 08:14:11.000000 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-01 08:14:11.000000 pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-01 08:14:11.236576 pubtools-content-gateway-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-01 08:14:01.000000 pubtools-content-gateway-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/_content_gateway.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/entrypoints_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/push_base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/push_cgw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/docs/push_staged_cgw.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/pubtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29726 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_cgw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_staged_cgw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/pubtools/_content_gateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 07:29:36.000000 pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 07:29:36.435650 pubtools-content-gateway-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-10 07:29:26.000000 pubtools-content-gateway-0.5.1/setup.py
```

### Comparing `pubtools-content-gateway-0.4.0/LICENSE` & `pubtools-content-gateway-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/PKG-INFO` & `pubtools-content-gateway-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pubtools-content-gateway
-Version: 0.4.0
+Version: 0.5.1
 Summary: Automate pushing to Content Gateway
 Home-page: https://github.com/release-engineering/pubtools-content-gateway
 Author: Javed Alam
 Author-email: jalam@redhat.com
 Project-URL: Changelog, https://release-engineering.github.io/pubtools-content-gateway/CHANGELOG.html
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-content-gateway/
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pubtools-content-gateway-0.4.0/docs/Makefile` & `pubtools-content-gateway-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/docs/README.rst` & `pubtools-content-gateway-0.5.1/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 --------------------------------
 
 
 Requirements
 ============
 
-- Python 3.5+
+- Python 3.9+
 
 --------------------------------
 
 
 Setup
 =====
```

### Comparing `pubtools-content-gateway-0.4.0/docs/_content_gateway.rst` & `pubtools-content-gateway-0.5.1/docs/_content_gateway.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/docs/conf.py` & `pubtools-content-gateway-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/docs/entrypoints_reference.rst` & `pubtools-content-gateway-0.5.1/docs/entrypoints_reference.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/docs/index.rst` & `pubtools-content-gateway-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/docs/push_cgw.rst` & `pubtools-content-gateway-0.5.1/docs/push_cgw.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/docs/push_staged_cgw.rst` & `pubtools-content-gateway-0.5.1/docs/push_staged_cgw.rst`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/cgw_authentication.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_authentication.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/cgw_client.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_client.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/cgw_session.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/cgw_session.py`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/push_base.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from .cgw_client import CGWClient
 from .cgw_authentication import CGWBasicAuth
 import logging
 
 LOG = logging.getLogger("pubtools.cgw")
-LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(message)s"
-logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT)
 
 
 class CGWError(Exception):
     """Custom exception class to handle Content Gateway errors."""
 
     def __init__(self, msg):
         super(CGWError, self).__init__(msg)
```

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/push_cgw.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_cgw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import logging
 from .push_base import PushBase
 from .utils import yaml_parser, validate_data, sort_items, format_cgw_items
 
 LOG = logging.getLogger("pubtools.cgw")
 LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(message)s"
-logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT)
 
 
 class PushCGW(PushBase):
     """Handle push CGW workflow."""
 
     def __init__(self, cgw_hostname, cgw_username, cgw_password, cgw_filepath):
         """
@@ -62,14 +61,15 @@
             #  we want to return full Traceback
             raise error
 
 
 def main():
     """Entrypoint for CGW Push."""
 
+    logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT)
     parser = argparse.ArgumentParser()
     parser.add_argument("-host", "--CGW_hostname", required=True, metavar="CGW-hostname", help="Hostname of the server")
     parser.add_argument(
         "-u", "--CGW_username", required=True, metavar="CGW-username", help="Username of Content Gateway"
     )
     parser.add_argument("-p", "--CGW_password", metavar="CGW-password", help="Password for Content Gateway")
     parser.add_argument(
```

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/push_staged_cgw.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/push_staged_cgw.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import json
 import logging
+import hashlib
 from .push_base import PushBase
 from .utils import yaml_parser, validate_data, sort_items, format_cgw_items
 
 try:
     import attr as attrs
 except ImportError:  # pragma: no cover
     import attrs
 
 from pubtools.pluggy import hookimpl, pm
-from pushsource import CGWPushItem
+from pushsource import CGWPushItem, DirectoryPushItem
 from pushsource import Source
 
 LOG = logging.getLogger("pubtools.cgw")
 LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(message)s"
-logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT)
 
 
 class PushStagedCGW(PushBase):
     """Handle push staged CGW workflow."""
 
     def __init__(self, source_urls, target_name, target_settings):
         """
@@ -102,34 +102,47 @@
                 try:
                     for pitem in parsed_items:
                         if pitem["type"] == "product":
                             self.process_product(pitem)
                         if pitem.get("type") == "product_version":
                             self.process_version(pitem)
                         if pitem["type"] == "file":
+                            found = None
                             for push_item in self.push_items:
-                                found = False
-                                for source_url in self.source_urls:
-                                    if (
-                                        push_item.src.replace(push_item.origin, "").lstrip("/")
-                                        == pitem["metadata"]["pushItemPath"]
-                                    ):
-                                        found = True
+                                if isinstance(push_item, DirectoryPushItem):
+                                    found = "directory_item"
+                                elif (
+                                    push_item.src.replace(push_item.origin, "").lstrip("/")
+                                    == pitem["metadata"]["pushItemPath"]
+                                ):
+                                    found = "file_item"
                                 if found:
                                     break
                             else:
                                 raise ValueError(
                                     "Unable to find push item with path:%s" % pitem["metadata"]["pushItemPath"]
                                 )
-                            pulp_push_unit = self.pulp_push_units[self.push_item_str(push_item)]
-                            pulp_push_item = self.processed_push_items[self.push_item_str(push_item)]
-                            pitem["metadata"]["downloadURL"] = pulp_push_unit.cdn_path
-                            pitem["metadata"]["md5"] = pulp_push_item.md5sum
-                            pitem["metadata"]["sha256"] = pulp_push_unit.sha256sum
-                            pitem["metadata"]["size"] = os.stat(push_item.src).st_size
+                            if found == "file_item":
+                                pulp_push_unit = self.pulp_push_units[self.push_item_str(push_item)]
+                                pulp_push_item = self.processed_push_items[self.push_item_str(push_item)]
+                                pitem["metadata"]["downloadURL"] = pulp_push_unit.cdn_path
+                                pitem["metadata"]["md5"] = pulp_push_item.md5sum
+                                pitem["metadata"]["sha256"] = pulp_push_unit.sha256sum
+                                pitem["metadata"]["size"] = os.stat(push_item.src).st_size
+                            else:
+                                filename = pitem["metadata"]["pushItemPath"].split("/")[-1]
+                                file_path = os.path.join(push_item.src, filename)
+                                with open(file_path, "rb") as f:
+                                    bytes = f.read()
+                                    pitem["metadata"]["md5"] = hashlib.md5(bytes).hexdigest()
+                                    pitem["metadata"]["sha256"] = hashlib.sha256(bytes).hexdigest()
+                                pitem["metadata"]["size"] = os.path.getsize(file_path)
+                                pitem["metadata"]["downloadURL"] = "/content/origin/files/sha256/{0}/{1}/{2}".format(
+                                    pitem["metadata"]["sha256"][:2], pitem["metadata"]["sha256"], filename
+                                )
                             self.process_file(pitem)
 
                     self.make_visible()
                     LOG.info("\n All CGW operations are successfully completed...!")
                 except Exception as error:
                     LOG.exception("Exception occurred during the CGW operation %s" % error)
                     LOG.info("Rolling back the partial operation")
@@ -138,10 +151,11 @@
                     #  raising the occurred Exception as all the exception will get caught in this except block
                     #  we want to return full Traceback
                     raise error
 
 
 def entry_point(source_urls, target_name, target_settings):
     """Entrypoint for CGW push stage."""
+    logging.basicConfig(level=logging.DEBUG, format=LOG_FORMAT)
     ret = PushStagedCGW(source_urls, target_name, target_settings)
     pm.register(ret)
     return ret
```

### Comparing `pubtools-content-gateway-0.4.0/pubtools/_content_gateway/utils.py` & `pubtools-content-gateway-0.5.1/pubtools/_content_gateway/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import yaml
 from yaml.loader import SafeLoader
 from jsonschema import validate
 import logging
 import copy
 
 LOG = logging.getLogger("pubtools.cgw")
-LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(message)s"
-logging.basicConfig(level=logging.INFO, format=LOG_FORMAT)
 
 PRODUCT_SCHEMA = {
     "type": "object",
     "properties": {
         "type": {"type": "string"},
         "action": {"type": "string", "enum": ["create", "update", "delete"]},
         "metadata": {
```

### Comparing `pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/PKG-INFO` & `pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pubtools-content-gateway
-Version: 0.4.0
+Version: 0.5.1
 Summary: Automate pushing to Content Gateway
 Home-page: https://github.com/release-engineering/pubtools-content-gateway
 Author: Javed Alam
 Author-email: jalam@redhat.com
 Project-URL: Changelog, https://release-engineering.github.io/pubtools-content-gateway/CHANGELOG.html
 Project-URL: Documentation, https://release-engineering.github.io/pubtools-content-gateway/
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pubtools-content-gateway-0.4.0/pubtools_content_gateway.egg-info/SOURCES.txt` & `pubtools-content-gateway-0.5.1/pubtools_content_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubtools-content-gateway-0.4.0/setup.py` & `pubtools-content-gateway-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,28 +64,27 @@
         return f.read().splitlines()
 
 
 # INSTALL_REQUIRES = ['urllib3', 'six', 'requests-mock', 'requests', 'mock', 'pytest', 'setuptools']
 INSTALL_REQUIRES = get_requirements()
 
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 setup(
     name="pubtools-content-gateway",
-    version="0.4.0",
+    version="0.5.1",
     description=get_description(),
     long_description_content_type="text/markdown",
     author="Javed Alam",
     author_email="jalam@redhat.com",
     url="https://github.com/release-engineering/pubtools-content-gateway",
     classifiers=classifiers,
     packages=find_packages(exclude=["tests"]),
@@ -98,14 +97,14 @@
             "push-cgw-metadata = pubtools._content_gateway.push_cgw:main"
         ],
         "target": [
             "push-staged-cgw = pubtools._content_gateway.push_staged_cgw:entry_point",
         ]
     },
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     project_urls={
         "Changelog": "https://release-engineering.github.io/pubtools-content-gateway/CHANGELOG.html",
         "Documentation": "https://release-engineering.github.io/pubtools-content-gateway/",
     },
     cmdclass={"test": Tox},
 )
```

