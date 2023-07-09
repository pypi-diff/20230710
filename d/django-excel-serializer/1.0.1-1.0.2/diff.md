# Comparing `tmp/django-excel-serializer-1.0.1.tar.gz` & `tmp/django-excel-serializer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-excel-serializer-1.0.1.tar", last modified: Sun Jul  9 22:56:51 2023, max compression
+gzip compressed data, was "django-excel-serializer-1.0.2.tar", last modified: Sun Jul  9 23:10:59 2023, max compression
```

## Comparing `django-excel-serializer-1.0.1.tar` & `django-excel-serializer-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 22:56:51.004191 django-excel-serializer-1.0.1/
--rw-r--r--   0 kamil      (501) staff       (20)     1075 2023-07-09 21:11:27.000000 django-excel-serializer-1.0.1/LICENSE
--rw-r--r--   0 kamil      (501) staff       (20)      284 2023-07-09 22:56:51.003694 django-excel-serializer-1.0.1/PKG-INFO
--rw-r--r--   0 kamil      (501) staff       (20)       82 2023-07-09 21:21:23.000000 django-excel-serializer-1.0.1/README.md
-drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 22:56:51.002252 django-excel-serializer-1.0.1/django_excel_serializer.egg-info/
--rw-r--r--   0 kamil      (501) staff       (20)      284 2023-07-09 22:56:50.000000 django-excel-serializer-1.0.1/django_excel_serializer.egg-info/PKG-INFO
--rw-r--r--   0 kamil      (501) staff       (20)      249 2023-07-09 22:56:50.000000 django-excel-serializer-1.0.1/django_excel_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 kamil      (501) staff       (20)        1 2023-07-09 22:56:50.000000 django-excel-serializer-1.0.1/django_excel_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 kamil      (501) staff       (20)       17 2023-07-09 22:56:50.000000 django-excel-serializer-1.0.1/django_excel_serializer.egg-info/top_level.txt
-drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 22:56:51.002824 django-excel-serializer-1.0.1/excel_serializer/
--rw-r--r--   0 kamil      (501) staff       (20)       22 2023-07-09 22:56:43.000000 django-excel-serializer-1.0.1/excel_serializer/__init__.py
--rw-r--r--   0 kamil      (501) staff       (20)      410 2023-07-09 22:50:41.000000 django-excel-serializer-1.0.1/pyproject.toml
--rw-r--r--   0 kamil      (501) staff       (20)       38 2023-07-09 22:56:51.004360 django-excel-serializer-1.0.1/setup.cfg
+drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:10:59.262904 django-excel-serializer-1.0.2/
+-rw-r--r--   0 kamil      (501) staff       (20)     1075 2023-07-09 21:11:27.000000 django-excel-serializer-1.0.2/LICENSE
+-rw-r--r--   0 kamil      (501) staff       (20)      458 2023-07-09 23:10:59.262648 django-excel-serializer-1.0.2/PKG-INFO
+-rw-r--r--   0 kamil      (501) staff       (20)       82 2023-07-09 21:21:23.000000 django-excel-serializer-1.0.2/README.md
+drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:10:59.261713 django-excel-serializer-1.0.2/django_excel_serializer.egg-info/
+-rw-r--r--   0 kamil      (501) staff       (20)      458 2023-07-09 23:10:59.000000 django-excel-serializer-1.0.2/django_excel_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 kamil      (501) staff       (20)      312 2023-07-09 23:10:59.000000 django-excel-serializer-1.0.2/django_excel_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 kamil      (501) staff       (20)        1 2023-07-09 23:10:59.000000 django-excel-serializer-1.0.2/django_excel_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       21 2023-07-09 23:10:59.000000 django-excel-serializer-1.0.2/django_excel_serializer.egg-info/requires.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       17 2023-07-09 23:10:59.000000 django-excel-serializer-1.0.2/django_excel_serializer.egg-info/top_level.txt
+drwxr-xr-x   0 kamil      (501) staff       (20)        0 2023-07-09 23:10:59.262120 django-excel-serializer-1.0.2/excel_serializer/
+-rw-r--r--   0 kamil      (501) staff       (20)       22 2023-07-09 23:10:53.000000 django-excel-serializer-1.0.2/excel_serializer/__init__.py
+-rw-r--r--   0 kamil      (501) staff       (20)      607 2023-07-09 23:09:51.000000 django-excel-serializer-1.0.2/pyproject.toml
+-rw-r--r--   0 kamil      (501) staff       (20)       23 2023-07-09 23:06:22.000000 django-excel-serializer-1.0.2/requirements.txt
+-rw-r--r--   0 kamil      (501) staff       (20)       38 2023-07-09 23:10:59.262985 django-excel-serializer-1.0.2/setup.cfg
```

### Comparing `django-excel-serializer-1.0.1/LICENSE` & `django-excel-serializer-1.0.2/LICENSE`

 * *Files identical despite different names*

