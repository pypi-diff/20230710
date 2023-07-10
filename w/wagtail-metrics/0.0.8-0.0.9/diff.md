# Comparing `tmp/wagtail_metrics-0.0.8.tar.gz` & `tmp/wagtail_metrics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_metrics-0.0.8.tar", last modified: Wed Feb  9 17:59:11 2022, max compression
+gzip compressed data, was "wagtail_metrics-0.0.9.tar", last modified: Sat Feb 12 15:56:48 2022, max compression
```

## Comparing `wagtail_metrics-0.0.8.tar` & `wagtail_metrics-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.881280 wagtail_metrics-0.0.8/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2021-11-25 10:44:58.000000 wagtail_metrics-0.0.8/LICENSE
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      140 2022-02-04 15:22:33.000000 wagtail_metrics-0.0.8/MANIFEST.in
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    11389 2022-02-09 17:59:11.881280 wagtail_metrics-0.0.8/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    10657 2022-02-07 13:35:11.000000 wagtail_metrics-0.0.8/README.rst
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.877280 wagtail_metrics-0.0.8/app/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.8/app/__init__.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.877280 wagtail_metrics-0.0.8/app/migrations/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      604 2021-11-25 11:01:24.000000 wagtail_metrics-0.0.8/app/migrations/0001_initial.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1740 2021-11-25 12:59:47.000000 wagtail_metrics-0.0.8/app/migrations/0002_create_homepage.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      703 2022-02-02 12:35:54.000000 wagtail_metrics-0.0.8/app/migrations/0003_auto_20220202_1235.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 11:01:24.000000 wagtail_metrics-0.0.8/app/migrations/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      815 2022-02-02 13:43:51.000000 wagtail_metrics-0.0.8/app/models.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.877280 wagtail_metrics-0.0.8/app/settings/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.8/app/settings/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     4554 2022-02-04 14:56:33.000000 wagtail_metrics-0.0.8/app/settings/base.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      649 2022-02-08 18:39:17.000000 wagtail_metrics-0.0.8/app/settings/dev.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       95 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.8/app/settings/production.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.877280 wagtail_metrics-0.0.8/app/tests/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 16:01:48.000000 wagtail_metrics-0.0.8/app/tests/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     4431 2022-02-09 17:58:01.000000 wagtail_metrics-0.0.8/app/tests/test_checkup.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1198 2022-02-02 13:25:35.000000 wagtail_metrics-0.0.8/app/urls.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      387 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.8/app/wsgi.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2022-02-09 17:59:11.881280 wagtail_metrics-0.0.8/setup.cfg
--rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1163 2022-02-01 17:15:22.000000 wagtail_metrics-0.0.8/setup.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.877280 wagtail_metrics-0.0.8/wagtail_metrics/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2022-02-04 14:56:33.000000 wagtail_metrics-0.0.8/wagtail_metrics/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2367 2022-02-08 18:22:23.000000 wagtail_metrics-0.0.8/wagtail_metrics/checkup.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1248 2022-02-09 17:58:45.000000 wagtail_metrics-0.0.8/wagtail_metrics/constants.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      251 2022-02-04 10:55:15.000000 wagtail_metrics-0.0.8/wagtail_metrics/exceptions.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1057 2022-02-09 17:45:13.000000 wagtail_metrics-0.0.8/wagtail_metrics/metric.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.881280 wagtail_metrics-0.0.8/wagtail_metrics/providers/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2022-02-04 14:56:33.000000 wagtail_metrics-0.0.8/wagtail_metrics/providers/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2002 2022-02-04 15:22:33.000000 wagtail_metrics-0.0.8/wagtail_metrics/providers/google_page_speed.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      460 2022-02-07 13:57:14.000000 wagtail_metrics-0.0.8/wagtail_metrics/providers/request.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3524 2022-02-08 18:37:26.000000 wagtail_metrics-0.0.8/wagtail_metrics/providers/wagtail_page.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-09 17:59:11.877280 wagtail_metrics-0.0.8/wagtail_metrics.egg-info/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    11389 2022-02-09 17:59:11.000000 wagtail_metrics-0.0.8/wagtail_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      833 2022-02-09 17:59:11.000000 wagtail_metrics-0.0.8/wagtail_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2022-02-09 17:59:11.000000 wagtail_metrics-0.0.8/wagtail_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       20 2022-02-09 17:59:11.000000 wagtail_metrics-0.0.8/wagtail_metrics.egg-info/top_level.txt
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2021-11-25 10:44:58.000000 wagtail_metrics-0.0.9/LICENSE
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      140 2022-02-04 15:22:33.000000 wagtail_metrics-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    11389 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    10657 2022-02-07 13:35:11.000000 wagtail_metrics-0.0.9/README.rst
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.688277 wagtail_metrics-0.0.9/app/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.9/app/__init__.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/app/migrations/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      604 2021-11-25 11:01:24.000000 wagtail_metrics-0.0.9/app/migrations/0001_initial.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1740 2021-11-25 12:59:47.000000 wagtail_metrics-0.0.9/app/migrations/0002_create_homepage.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      703 2022-02-02 12:35:54.000000 wagtail_metrics-0.0.9/app/migrations/0003_auto_20220202_1235.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 11:01:24.000000 wagtail_metrics-0.0.9/app/migrations/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      815 2022-02-02 13:43:51.000000 wagtail_metrics-0.0.9/app/models.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/app/settings/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.9/app/settings/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     4554 2022-02-04 14:56:33.000000 wagtail_metrics-0.0.9/app/settings/base.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      649 2022-02-08 18:39:17.000000 wagtail_metrics-0.0.9/app/settings/dev.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       95 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.9/app/settings/production.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/app/tests/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 16:01:48.000000 wagtail_metrics-0.0.9/app/tests/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     4431 2022-02-09 17:58:01.000000 wagtail_metrics-0.0.9/app/tests/test_checkup.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1198 2022-02-02 13:25:35.000000 wagtail_metrics-0.0.9/app/urls.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      387 2021-11-25 10:52:26.000000 wagtail_metrics-0.0.9/app/wsgi.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/setup.cfg
+-rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1163 2022-02-01 17:15:22.000000 wagtail_metrics-0.0.9/setup.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/wagtail_metrics/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2022-02-04 14:56:33.000000 wagtail_metrics-0.0.9/wagtail_metrics/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2566 2022-02-12 15:55:45.000000 wagtail_metrics-0.0.9/wagtail_metrics/checkup.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1248 2022-02-09 17:58:45.000000 wagtail_metrics-0.0.9/wagtail_metrics/constants.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      251 2022-02-04 10:55:15.000000 wagtail_metrics-0.0.9/wagtail_metrics/exceptions.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1057 2022-02-09 17:45:13.000000 wagtail_metrics-0.0.9/wagtail_metrics/metric.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/wagtail_metrics/providers/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2022-02-04 14:56:33.000000 wagtail_metrics-0.0.9/wagtail_metrics/providers/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2002 2022-02-04 15:22:33.000000 wagtail_metrics-0.0.9/wagtail_metrics/providers/google_page_speed.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      460 2022-02-07 13:57:14.000000 wagtail_metrics-0.0.9/wagtail_metrics/providers/request.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3524 2022-02-08 18:37:26.000000 wagtail_metrics-0.0.9/wagtail_metrics/providers/wagtail_page.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2022-02-12 15:56:48.692277 wagtail_metrics-0.0.9/wagtail_metrics.egg-info/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    11389 2022-02-12 15:56:48.000000 wagtail_metrics-0.0.9/wagtail_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      833 2022-02-12 15:56:48.000000 wagtail_metrics-0.0.9/wagtail_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2022-02-12 15:56:48.000000 wagtail_metrics-0.0.9/wagtail_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       20 2022-02-12 15:56:48.000000 wagtail_metrics-0.0.9/wagtail_metrics.egg-info/top_level.txt
```

### Comparing `wagtail_metrics-0.0.8/LICENSE` & `wagtail_metrics-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/PKG-INFO` & `wagtail_metrics-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_metrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wagtail Metrics
 Home-page: https://github.com/Aleksi44/wagtail-metrics
 Author: Alexis Le Baron
 Author-email: hello@snoweb.io
 License: GPL-3.0
 Keywords: wagtail metrics
 Platform: linux
```

### Comparing `wagtail_metrics-0.0.8/README.rst` & `wagtail_metrics-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/migrations/0001_initial.py` & `wagtail_metrics-0.0.9/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/migrations/0002_create_homepage.py` & `wagtail_metrics-0.0.9/app/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/migrations/0003_auto_20220202_1235.py` & `wagtail_metrics-0.0.9/app/migrations/0003_auto_20220202_1235.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/models.py` & `wagtail_metrics-0.0.9/app/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/settings/base.py` & `wagtail_metrics-0.0.9/app/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/settings/dev.py` & `wagtail_metrics-0.0.9/app/settings/dev.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/tests/test_checkup.py` & `wagtail_metrics-0.0.9/app/tests/test_checkup.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/app/urls.py` & `wagtail_metrics-0.0.9/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/setup.py` & `wagtail_metrics-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics/checkup.py` & `wagtail_metrics-0.0.9/wagtail_metrics/checkup.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,18 +35,22 @@
             provider_module = self._get_provider_module(provider_name)
             provider_function = getattr(provider_module, 'run')
             try:
                 provider_function(self, page)
             except WagtailMetricsException as err:
                 logger.error(str(err))
 
-    def add_site(self, site):
+    def add_site(self, site, exclude_offline=True):
         if not isinstance(site, Site):
             return
-        for page in site.root_page.get_descendants(inclusive=True).specific():
+        if exclude_offline:
+            site_query = site.root_page.get_descendants(inclusive=True).live().public().specific()
+        else:
+            site_query = site.root_page.get_descendants(inclusive=True).specific()
+        for page in site_query:
             self.add_page(page)
             if self.i18n_enable:
                 for page_alternate in page.get_translations().exclude(alias_of__isnull=False):
                     self.add_page(page_alternate)
 
     def add_metric(self, key, value, page_url=None, initialize=False):
         if key not in constants.WAGTAIL_METRICS_DEFAULT_EXCLUDE:
```

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics/constants.py` & `wagtail_metrics-0.0.9/wagtail_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics/metric.py` & `wagtail_metrics-0.0.9/wagtail_metrics/metric.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics/providers/google_page_speed.py` & `wagtail_metrics-0.0.9/wagtail_metrics/providers/google_page_speed.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics/providers/wagtail_page.py` & `wagtail_metrics-0.0.9/wagtail_metrics/providers/wagtail_page.py`

 * *Files identical despite different names*

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics.egg-info/PKG-INFO` & `wagtail_metrics-0.0.9/wagtail_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-metrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wagtail Metrics
 Home-page: https://github.com/Aleksi44/wagtail-metrics
 Author: Alexis Le Baron
 Author-email: hello@snoweb.io
 License: GPL-3.0
 Keywords: wagtail metrics
 Platform: linux
```

### Comparing `wagtail_metrics-0.0.8/wagtail_metrics.egg-info/SOURCES.txt` & `wagtail_metrics-0.0.9/wagtail_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

