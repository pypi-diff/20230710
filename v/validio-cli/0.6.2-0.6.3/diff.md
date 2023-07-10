# Comparing `tmp/validio_cli-0.6.2.tar.gz` & `tmp/validio_cli-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.6.2.tar", max compression
+gzip compressed data, was "validio_cli-0.6.3.tar", max compression
```

## Comparing `validio_cli-0.6.2.tar` & `validio_cli-0.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11340 2023-07-05 21:50:58.355274 validio_cli-0.6.2/LICENSE
--rw-r--r--   0        0        0      227 2023-07-05 21:50:58.355274 validio_cli-0.6.2/README_PUBLIC.md
--rw-r--r--   0        0        0     1987 2023-07-05 21:51:10.591098 validio_cli-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     6274 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/__init__.py
--rw-r--r--   0        0        0     2390 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    11640 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     4335 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     2506 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     2306 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/destinations.py
--rw-r--r--   0        0        0     7429 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/incidents.py
--rw-r--r--   0        0        0     2336 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/metrics.py
--rw-r--r--   0        0        0     2867 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3334 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     2913 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0     1902 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/segments.py
--rw-r--r--   0        0        0    26341 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1174 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     3743 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     2806 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     3259 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/bin/main.py
--rw-r--r--   0        0        0     2587 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/components.py
--rw-r--r--   0        0        0      265 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/metadata.py
--rw-r--r--   0        0        0      630 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/namespace.py
--rw-r--r--   0        0        0     1382 2023-07-05 21:50:58.355274 validio_cli-0.6.2/validio_cli/schema.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-10 07:22:31.790640 validio_cli-0.6.3/LICENSE
+-rw-r--r--   0        0        0      227 2023-07-10 07:22:31.791640 validio_cli-0.6.3/README_PUBLIC.md
+-rw-r--r--   0        0        0     1987 2023-07-10 07:22:47.882609 validio_cli-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6274 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/__init__.py
+-rw-r--r--   0        0        0     2390 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    11640 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     4335 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     2506 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     2306 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     7429 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/incidents.py
+-rw-r--r--   0        0        0     2336 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/metrics.py
+-rw-r--r--   0        0        0     2867 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3334 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     2913 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0     1902 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/segments.py
+-rw-r--r--   0        0        0    26341 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     3743 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     2806 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     3259 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     2587 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/metadata.py
+-rw-r--r--   0        0        0      630 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-07-10 07:22:31.792640 validio_cli-0.6.3/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.6.3/PKG-INFO
```

### Comparing `validio_cli-0.6.2/LICENSE` & `validio_cli-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/pyproject.toml` & `validio_cli-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-cli"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.6.2"
+version = "0.6.3"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
 readme = "README_PUBLIC.md"
```

### Comparing `validio_cli-0.6.2/validio_cli/__init__.py` & `validio_cli-0.6.3/validio_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/channels.py` & `validio_cli-0.6.3/validio_cli/bin/entities/channels.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/code.py` & `validio_cli-0.6.3/validio_cli/bin/entities/code.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/config.py` & `validio_cli-0.6.3/validio_cli/bin/entities/config.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/credentials.py` & `validio_cli-0.6.3/validio_cli/bin/entities/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/destinations.py` & `validio_cli-0.6.3/validio_cli/bin/entities/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/incidents.py` & `validio_cli-0.6.3/validio_cli/bin/entities/incidents.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/metrics.py` & `validio_cli-0.6.3/validio_cli/bin/entities/metrics.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.6.3/validio_cli/bin/entities/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.6.3/validio_cli/bin/entities/recommendations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.6.3/validio_cli/bin/entities/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/segments.py` & `validio_cli-0.6.3/validio_cli/bin/entities/segments.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/sources.py` & `validio_cli-0.6.3/validio_cli/bin/entities/sources.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/users.py` & `validio_cli-0.6.3/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/validators.py` & `validio_cli-0.6.3/validio_cli/bin/entities/validators.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/entities/windows.py` & `validio_cli-0.6.3/validio_cli/bin/entities/windows.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/bin/main.py` & `validio_cli-0.6.3/validio_cli/bin/main.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/components.py` & `validio_cli-0.6.3/validio_cli/components.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/namespace.py` & `validio_cli-0.6.3/validio_cli/namespace.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/validio_cli/schema.py` & `validio_cli-0.6.3/validio_cli/schema.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.6.2/PKG-INFO` & `validio_cli-0.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-cli
-Version: 0.6.2
+Version: 0.6.3
 Summary: CLI tool to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

