# Comparing `tmp/estratega-utils-1.1.tar.gz` & `tmp/estratega-utils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estratega-utils-1.1.tar", last modified: Thu Jul  6 15:04:32 2023, max compression
+gzip compressed data, was "estratega-utils-1.2.tar", last modified: Mon Jul 10 18:06:06 2023, max compression
```

## Comparing `estratega-utils-1.1.tar` & `estratega-utils-1.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:04:32.843763 estratega-utils-1.1/
--rw-rw-rw-   0        0        0      578 2023-07-06 15:04:32.843763 estratega-utils-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 15:04:32.821823 estratega-utils-1.1/estratega_utils.egg-info/
--rw-rw-rw-   0        0        0      578 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 15:04:32.000000 estratega-utils-1.1/estratega_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 15:04:32.844761 estratega-utils-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-07-06 14:50:13.000000 estratega-utils-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:04:32.841770 estratega-utils-1.1/utils/
--rw-rw-rw-   0        0        0       78 2023-07-06 15:01:30.000000 estratega-utils-1.1/utils/__init__.py
--rw-rw-rw-   0        0        0      822 2023-07-06 13:42:40.000000 estratega-utils-1.1/utils/objetos.py
--rw-rw-rw-   0        0        0      403 2023-07-06 14:57:10.000000 estratega-utils-1.1/utils/strings.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.041013 estratega-utils-1.2/
+-rw-rw-rw-   0        0        0      479 2023-07-10 18:06:06.037979 estratega-utils-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-07-07 15:48:13.000000 estratega-utils-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.027671 estratega-utils-1.2/estratega_utils.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 18:06:05.000000 estratega-utils-1.2/estratega_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:06:06.041968 estratega-utils-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-07-10 13:20:00.000000 estratega-utils-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.033991 estratega-utils-1.2/utils/
+-rw-rw-rw-   0        0        0      202 2023-07-07 17:18:39.000000 estratega-utils-1.2/utils/PRUEBAS.py
+-rw-rw-rw-   0        0        0      228 2023-07-07 18:48:55.000000 estratega-utils-1.2/utils/__init__.py
+-rw-rw-rw-   0        0        0     1188 2023-07-07 17:18:39.000000 estratega-utils-1.2/utils/dicts.py
+-rw-rw-rw-   0        0        0      160 2023-07-07 18:48:27.000000 estratega-utils-1.2/utils/lists.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:06:06.035985 estratega-utils-1.2/utils/query_builder/
+-rw-rw-rw-   0        0        0      119 2023-07-07 18:40:39.000000 estratega-utils-1.2/utils/query_builder/__init__.py
+-rw-rw-rw-   0        0        0     7836 2023-07-10 18:03:44.000000 estratega-utils-1.2/utils/query_builder/mysql.py
+-rw-rw-rw-   0        0        0      403 2023-07-06 14:57:10.000000 estratega-utils-1.2/utils/strings.py
```

### Comparing `estratega-utils-1.1/setup.py` & `estratega-utils-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = 'Utilidades varias'
 LONG_DESCRIPTION = 'Funciones y clases con utiliddades para agilizar y optimizar la escritura de código'
 
 # Configurando
 setup(
     # el nombre debe coincidir con el nombre de la carpeta
     # 'modulomuysimple'
@@ -12,20 +12,18 @@
     version=VERSION,
     author="Ivan Sayavedra",
     author_email="<isayavedra@estrategasoftware.com.ar>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # añade cualquier paquete adicional que debe ser
-    install_requires=['pydantic'],
+    install_requires=['pydantic', 'pymysql'],
     # instalado junto con tu paquete. Ej: 'caer'
 
     keywords=['python', 'estratega utils'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

