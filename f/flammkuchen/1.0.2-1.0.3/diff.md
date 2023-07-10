# Comparing `tmp/flammkuchen-1.0.2.tar.gz` & `tmp/flammkuchen-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flammkuchen-1.0.2.tar", last modified: Tue Jun 14 08:56:09 2022, max compression
+gzip compressed data, was "flammkuchen-1.0.3.tar", last modified: Mon Jul 10 16:55:49 2023, max compression
```

## Comparing `flammkuchen-1.0.2.tar` & `flammkuchen-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 08:56:09.625415 flammkuchen-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 08:56:09.621415 flammkuchen-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 08:56:09.621415 flammkuchen-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-06-14 08:56:09.625415 flammkuchen-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 08:56:09.621415 flammkuchen-1.0.2/flammkuchen/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/flammkuchen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/flammkuchen/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    27054 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/flammkuchen/hdf5io.py
--rw-r--r--   0 runner    (1001) docker     (121)    26899 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/flammkuchen/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 08:56:09.625415 flammkuchen-1.0.2/flammkuchen/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/flammkuchen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12425 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/flammkuchen/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 08:56:09.625415 flammkuchen-1.0.2/flammkuchen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-06-14 08:56:08.000000 flammkuchen-1.0.2/flammkuchen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-06-14 08:56:09.000000 flammkuchen-1.0.2/flammkuchen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 08:56:09.000000 flammkuchen-1.0.2/flammkuchen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-14 08:56:09.000000 flammkuchen-1.0.2/flammkuchen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-14 08:56:09.000000 flammkuchen-1.0.2/flammkuchen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16799 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/io.rst
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-06-14 08:56:09.625415 flammkuchen-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-06-14 08:55:59.000000 flammkuchen-1.0.2/test.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:49.214596 flammkuchen-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:49.206596 flammkuchen-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:49.210596 flammkuchen-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-10 16:55:49.214596 flammkuchen-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:49.214596 flammkuchen-1.0.3/flammkuchen/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/flammkuchen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/flammkuchen/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27051 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/flammkuchen/hdf5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/flammkuchen/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:49.214596 flammkuchen-1.0.3/flammkuchen/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/flammkuchen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/flammkuchen/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:55:49.214596 flammkuchen-1.0.3/flammkuchen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-10 16:55:49.000000 flammkuchen-1.0.3/flammkuchen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 16:55:49.000000 flammkuchen-1.0.3/flammkuchen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:55:49.000000 flammkuchen-1.0.3/flammkuchen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 16:55:49.000000 flammkuchen-1.0.3/flammkuchen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 16:55:49.000000 flammkuchen-1.0.3/flammkuchen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-10 16:55:49.214596 flammkuchen-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-10 16:55:39.000000 flammkuchen-1.0.3/test.h5
```

### Comparing `flammkuchen-1.0.2/.github/workflows/main.yml` & `flammkuchen-1.0.3/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
           flake8
   test:
     needs: lint
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.7, 3.8.6]
+        python-version: [3.7, 3.8]
         exclude:
           - os: macos-latest
             python-version: 3.7
           - os: windows-latest
             python-version: 3.7
     steps:
       - uses: actions/checkout@v2
```

### Comparing `flammkuchen-1.0.2/.gitignore` & `flammkuchen-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flammkuchen-1.0.2/CHANGELOG.rst` & `flammkuchen-1.0.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `flammkuchen-1.0.2/LICENSE` & `flammkuchen-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flammkuchen-1.0.2/PKG-INFO` & `flammkuchen-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flammkuchen
-Version: 1.0.2
+Version: 1.0.3
 Summary: Easy saving and loading of hdf5 files in python (forked from DeepDish)
 Home-page: https://github.com/portugueslab/flammkuchen
 Maintainer: Luigi Petrucco, Vilim Stih @portugueslab
 Maintainer-email: luigi.petrucco@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `flammkuchen-1.0.2/README.rst` & `flammkuchen-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `flammkuchen-1.0.2/flammkuchen/hdf5io.py` & `flammkuchen-1.0.3/flammkuchen/hdf5io.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         itemsize = x.itemsize // 4
         atom = tables.UInt8Atom()
         x = x.view(dtype=np.uint8)
     elif np.issubdtype(x.dtype, np.string_):
         strtype = b"ascii"
         itemsize = x.itemsize
         atom = tables.StringAtom(itemsize)
-    elif x.dtype == np.object:
+    elif x.dtype == object:
         # Not supported by HDF5, force pickling
         _save_pickled(handler, group, x, name=name)
         return
     else:
         atom = tables.Atom.from_dtype(x.dtype)
         strtype = None
         itemsize = None
```

### Comparing `flammkuchen-1.0.2/flammkuchen/ls.py` & `flammkuchen-1.0.3/flammkuchen/ls.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,14 @@
     colorize=True,
     file=sys.stdout,
     unpack=False,
     settings={},
     parent_color="darkgray",
     key_color="white",
 ):
-
     s = "{}{}".format(
         paint(parent, parent_color, colorize=colorize),
         paint(key, key_color, colorize=colorize),
     )
     s_raw = "{}{}".format(parent, key)
     if "filter" in settings:
         if not re.search(settings["filter"], s_raw):
@@ -412,15 +411,14 @@
         level=0,
         parent="/",
         colorize=True,
         max_level=None,
         file=sys.stdout,
         settings={},
     ):
-
         if level < max_level:
             for i, v in enumerate(self.children):
                 k = str(i)
                 final = level + 1 == max_level
                 print_row(
                     k,
                     v.info(colorize=colorize, final_level=final),
```

### Comparing `flammkuchen-1.0.2/flammkuchen/tests/test_io.py` & `flammkuchen-1.0.3/flammkuchen/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `flammkuchen-1.0.2/flammkuchen.egg-info/PKG-INFO` & `flammkuchen-1.0.3/flammkuchen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flammkuchen
-Version: 1.0.2
+Version: 1.0.3
 Summary: Easy saving and loading of hdf5 files in python (forked from DeepDish)
 Home-page: https://github.com/portugueslab/flammkuchen
 Maintainer: Luigi Petrucco, Vilim Stih @portugueslab
 Maintainer-email: luigi.petrucco@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `flammkuchen-1.0.2/io.rst` & `flammkuchen-1.0.3/io.rst`

 * *Files identical despite different names*

### Comparing `flammkuchen-1.0.2/setup.py` & `flammkuchen-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
 ]
 
 args = dict(
     name="flammkuchen",
-    version="1.0.2",
+    version="1.0.3",
     url="https://github.com/portugueslab/flammkuchen",
     description="Easy saving and loading of hdf5 files in python (forked from DeepDish)",
     maintainer="Luigi Petrucco, Vilim Stih @portugueslab",
     maintainer_email="luigi.petrucco@gmail.com",
     install_requires=required,
     extras_require=dict(dev=required_dev),
     packages=[
```

### Comparing `flammkuchen-1.0.2/test.h5` & `flammkuchen-1.0.3/test.h5`

 * *Files identical despite different names*

