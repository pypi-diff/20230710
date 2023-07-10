# Comparing `tmp/recon_lw-2.0.0.dev5484773776.tar.gz` & `tmp/recon_lw-2.0.0.dev5506899890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5484773776.tar", last modified: Fri Jul  7 09:13:35 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5506899890.tar", last modified: Mon Jul 10 10:20:32 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5484773776.tar` & `recon_lw-2.0.0.dev5506899890.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-07 09:13:09.000000 recon_lw-2.0.0.dev5484773776/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    35110 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-10 10:20:14.000000 recon_lw-2.0.0.dev5506899890/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35229 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 10:20:32.000000 recon_lw-2.0.0.dev5506899890/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-10 10:19:51.000000 recon_lw-2.0.0.dev5506899890/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,14 +345,18 @@
     else:
         reset_aggr_seq(order_book)
 
     old_side, old_price, old_size = find_order_position(order_id, order_book)
     if old_side is None:
         return {"error": order_id + " not found"}, []
 
+    if price == old_price and size == old_size:
+        return {"error": "order update to identical parameters"}, []
+
+
     log = []
     if price == old_price:
         order_book[old_side][old_price][order_id] = size
         reflect_price_update_in_version(old_side, old_price, str_time_of_event, order_book)
         log.append(copy.deepcopy(order_book))
     else:
         # should no get here but will monitor
```

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw/recon_oe_ob.py` & `recon_lw-2.0.0.dev5506899890/recon_lw/recon_oe_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5506899890/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/setup.py` & `recon_lw-2.0.0.dev5506899890/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5484773776/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5506899890/test/test_recon_ob.py`

 * *Files identical despite different names*

