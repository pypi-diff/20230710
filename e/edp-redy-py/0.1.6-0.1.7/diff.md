# Comparing `tmp/edp_redy_py-0.1.6.tar.gz` & `tmp/edp_redy_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edp_redy_py-0.1.6.tar", last modified: Sat Jul  8 18:06:04 2023, max compression
+gzip compressed data, was "edp_redy_py-0.1.7.tar", last modified: Sun Jul  9 22:05:38 2023, max compression
```

## Comparing `edp_redy_py-0.1.6.tar` & `edp_redy_py-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.285747 edp_redy_py-0.1.6/
--rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      283 2023-07-08 18:06:04.286253 edp_redy_py-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.6/README.md
--rw-rw-rw-   0        0        0      111 2023-07-08 18:06:04.287315 edp_redy_py-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-07-08 18:05:16.000000 edp_redy_py-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.259000 edp_redy_py-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.269145 edp_redy_py-0.1.6/src/edp_redy/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.6/src/edp_redy/__init__.py
--rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.6/src/edp_redy/authenticate.py
--rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.6/src/edp_redy/consts.py
--rw-rw-rw-   0        0        0     2549 2023-07-08 18:05:54.000000 edp_redy_py-0.1.6/src/edp_redy/edp_mqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.271450 edp_redy_py-0.1.6/src/edp_redy/equipment/
--rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.6/src/edp_redy/equipment/__init__.py
--rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.6/src/edp_redy/equipment/equipment.py
--rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.6/src/edp_redy/helpers.py
--rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.6/src/edp_redy/redy.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.273568 edp_redy_py-0.1.6/src/edp_redy/usermanagement/
--rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.6/src/edp_redy/usermanagement/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.6/src/edp_redy/usermanagement/usermanagement.py
-drwxrwxrwx   0        0        0        0 2023-07-08 18:06:04.284479 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/
--rw-rw-rw-   0        0        0      283 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-08 18:06:04.000000 edp_redy_py-0.1.6/src/edp_redy_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 22:05:38.933971 edp_redy_py-0.1.7/
+-rw-rw-rw-   0        0        0    11556 2023-07-08 16:56:32.000000 edp_redy_py-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-07-09 22:05:38.933971 edp_redy_py-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-08 17:07:46.000000 edp_redy_py-0.1.7/README.md
+-rw-rw-rw-   0        0        0      111 2023-07-09 22:05:38.935576 edp_redy_py-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-07-09 22:05:22.000000 edp_redy_py-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:05:38.903720 edp_redy_py-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 22:05:38.917814 edp_redy_py-0.1.7/src/edp_redy/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:14:43.000000 edp_redy_py-0.1.7/src/edp_redy/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-07-08 17:53:36.000000 edp_redy_py-0.1.7/src/edp_redy/authenticate.py
+-rw-rw-rw-   0        0        0      204 2023-07-08 16:51:43.000000 edp_redy_py-0.1.7/src/edp_redy/consts.py
+-rw-rw-rw-   0        0        0     2549 2023-07-08 18:05:54.000000 edp_redy_py-0.1.7/src/edp_redy/edp_mqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:05:38.919935 edp_redy_py-0.1.7/src/edp_redy/equipment/
+-rw-rw-rw-   0        0        0        0 2023-07-08 16:25:40.000000 edp_redy_py-0.1.7/src/edp_redy/equipment/__init__.py
+-rw-rw-rw-   0        0        0     7618 2023-07-08 17:33:47.000000 edp_redy_py-0.1.7/src/edp_redy/equipment/equipment.py
+-rw-rw-rw-   0        0        0     1003 2023-07-08 16:51:43.000000 edp_redy_py-0.1.7/src/edp_redy/helpers.py
+-rw-rw-rw-   0        0        0      721 2023-07-08 17:37:45.000000 edp_redy_py-0.1.7/src/edp_redy/redy.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:05:38.922618 edp_redy_py-0.1.7/src/edp_redy/usermanagement/
+-rw-rw-rw-   0        0        0        0 2023-07-08 15:24:38.000000 edp_redy_py-0.1.7/src/edp_redy/usermanagement/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-07-08 17:33:51.000000 edp_redy_py-0.1.7/src/edp_redy/usermanagement/usermanagement.py
+drwxrwxrwx   0        0        0        0 2023-07-09 22:05:38.932895 edp_redy_py-0.1.7/src/edp_redy_py.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-07-09 22:05:38.000000 edp_redy_py-0.1.7/src/edp_redy_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-07-09 22:05:38.000000 edp_redy_py-0.1.7/src/edp_redy_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 22:05:38.000000 edp_redy_py-0.1.7/src/edp_redy_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-07-09 22:05:38.000000 edp_redy_py-0.1.7/src/edp_redy_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 22:05:38.000000 edp_redy_py-0.1.7/src/edp_redy_py.egg-info/top_level.txt
```

### Comparing `edp_redy_py-0.1.6/LICENSE` & `edp_redy_py-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.6/src/edp_redy/authenticate.py` & `edp_redy_py-0.1.7/src/edp_redy/authenticate.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.6/src/edp_redy/edp_mqtt.py` & `edp_redy_py-0.1.7/src/edp_redy/edp_mqtt.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.6/src/edp_redy/equipment/equipment.py` & `edp_redy_py-0.1.7/src/edp_redy/equipment/equipment.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.6/src/edp_redy/helpers.py` & `edp_redy_py-0.1.7/src/edp_redy/helpers.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.6/src/edp_redy/redy.py` & `edp_redy_py-0.1.7/src/edp_redy/redy.py`

 * *Files identical despite different names*

### Comparing `edp_redy_py-0.1.6/src/edp_redy/usermanagement/usermanagement.py` & `edp_redy_py-0.1.7/src/edp_redy/usermanagement/usermanagement.py`

 * *Files identical despite different names*

