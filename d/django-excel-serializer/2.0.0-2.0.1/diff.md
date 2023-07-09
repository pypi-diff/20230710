# Comparing `tmp/django-excel-serializer-2.0.0.tar.gz` & `tmp/django-excel-serializer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-excel-serializer-2.0.0.tar", last modified: Sun Jul  9 23:50:26 2023, max compression
+gzip compressed data, was "django-excel-serializer-2.0.1.tar", last modified: Sun Jul  9 23:55:19 2023, max compression
```

## Comparing `django-excel-serializer-2.0.0.tar` & `django-excel-serializer-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:50:26.791089 django-excel-serializer-2.0.0/
--rw-r--r--   0 kamil      (501) staff       (20)     1075 2023-07-09 21:11:27.000000 django-excel-serializer-2.0.0/LICENSE
--rw-r--r--   0 kamil      (501) staff       (20)     2396 2023-07-09 23:50:26.790795 django-excel-serializer-2.0.0/PKG-INFO
--rw-r--r--   0 kamil      (501) staff       (20)       82 2023-07-09 21:21:23.000000 django-excel-serializer-2.0.0/README.md
-drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:50:26.789684 django-excel-serializer-2.0.0/django_excel_serializer.egg-info/
--rw-r--r--   0 kamil      (501) staff       (20)     2396 2023-07-09 23:50:26.000000 django-excel-serializer-2.0.0/django_excel_serializer.egg-info/PKG-INFO
--rw-r--r--   0 kamil      (501) staff       (20)      355 2023-07-09 23:50:26.000000 django-excel-serializer-2.0.0/django_excel_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 kamil      (501) staff       (20)        1 2023-07-09 23:50:26.000000 django-excel-serializer-2.0.0/django_excel_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 kamil      (501) staff       (20)      107 2023-07-09 23:50:26.000000 django-excel-serializer-2.0.0/django_excel_serializer.egg-info/requires.txt
--rw-r--r--   0 kamil      (501) staff       (20)       17 2023-07-09 23:50:26.000000 django-excel-serializer-2.0.0/django_excel_serializer.egg-info/top_level.txt
-drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:50:26.790233 django-excel-serializer-2.0.0/excel_serializer/
--rw-r--r--   0 kamil      (501) staff       (20)       22 2023-07-09 23:50:21.000000 django-excel-serializer-2.0.0/excel_serializer/__init__.py
--rw-r--r--   0 kamil      (501) staff       (20)     1423 2023-07-09 23:47:15.000000 django-excel-serializer-2.0.0/pyproject.toml
--rw-r--r--   0 kamil      (501) staff       (20)       11 2023-07-09 23:40:03.000000 django-excel-serializer-2.0.0/requirements-dev.txt
--rw-r--r--   0 kamil      (501) staff       (20)       60 2023-07-09 23:37:44.000000 django-excel-serializer-2.0.0/requirements-test.txt
--rw-r--r--   0 kamil      (501) staff       (20)       23 2023-07-09 23:06:22.000000 django-excel-serializer-2.0.0/requirements.txt
--rw-r--r--   0 kamil      (501) staff       (20)       38 2023-07-09 23:50:26.791185 django-excel-serializer-2.0.0/setup.cfg
+drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:55:19.589601 django-excel-serializer-2.0.1/
+-rw-r--r--   0 kamil      (501) staff       (20)     1075 2023-07-09 21:11:27.000000 django-excel-serializer-2.0.1/LICENSE
+-rw-r--r--   0 kamil      (501) staff       (20)     1143 2023-07-09 23:55:19.589322 django-excel-serializer-2.0.1/PKG-INFO
+-rw-r--r--   0 kamil      (501) staff       (20)       82 2023-07-09 21:21:23.000000 django-excel-serializer-2.0.1/README.md
+drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:55:19.588377 django-excel-serializer-2.0.1/django_excel_serializer.egg-info/
+-rw-r--r--   0 kamil      (501) staff       (20)     1143 2023-07-09 23:55:19.000000 django-excel-serializer-2.0.1/django_excel_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 kamil      (501) staff       (20)      355 2023-07-09 23:55:19.000000 django-excel-serializer-2.0.1/django_excel_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 kamil      (501) staff       (20)        1 2023-07-09 23:55:19.000000 django-excel-serializer-2.0.1/django_excel_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 kamil      (501) staff       (20)      107 2023-07-09 23:55:19.000000 django-excel-serializer-2.0.1/django_excel_serializer.egg-info/requires.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       17 2023-07-09 23:55:19.000000 django-excel-serializer-2.0.1/django_excel_serializer.egg-info/top_level.txt
+drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:55:19.588793 django-excel-serializer-2.0.1/excel_serializer/
+-rw-r--r--   0 kamil      (501) staff       (20)       22 2023-07-09 23:55:07.000000 django-excel-serializer-2.0.1/excel_serializer/__init__.py
+-rw-r--r--   0 kamil      (501) staff       (20)     1394 2023-07-09 23:53:31.000000 django-excel-serializer-2.0.1/pyproject.toml
+-rw-r--r--   0 kamil      (501) staff       (20)       11 2023-07-09 23:40:03.000000 django-excel-serializer-2.0.1/requirements-dev.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       60 2023-07-09 23:37:44.000000 django-excel-serializer-2.0.1/requirements-test.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       23 2023-07-09 23:06:22.000000 django-excel-serializer-2.0.1/requirements.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       38 2023-07-09 23:55:19.589741 django-excel-serializer-2.0.1/setup.cfg
```

### Comparing `django-excel-serializer-2.0.0/LICENSE` & `django-excel-serializer-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-excel-serializer-2.0.0/pyproject.toml` & `django-excel-serializer-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [project]
 name = "django-excel-serializer"
 readme = "README.md"
-license = {file = "LICENSE"}
 authors = [
   {name = "Kamil Paduszyński", email="paduszyk@gmail.com"},
 ]
 keywords = [
   "django",
   "excel",
   "serializer",
```

