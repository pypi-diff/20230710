# Comparing `tmp/linlangleyprime-0.7.tar.gz` & `tmp/linlangleyprime-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linlangleyprime-0.7.tar", last modified: Tue Apr 27 22:36:13 2021, max compression
+gzip compressed data, was "linlangleyprime-0.8.tar", last modified: Mon Jul 10 16:34:59 2023, max compression
```

## Comparing `linlangleyprime-0.7.tar` & `linlangleyprime-0.8.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.659640 linlangleyprime-0.7/
--rw-r--r--   0 lchen      (501) staff       (20)     1077 2021-04-26 18:35:38.000000 linlangleyprime-0.7/LICENSE
--rw-r--r--   0 lchen      (501) staff       (20)       79 2021-04-26 19:04:35.000000 linlangleyprime-0.7/MANIFEST.in
--rw-r--r--   0 lchen      (501) staff       (20)     1146 2021-04-27 22:36:13.659798 linlangleyprime-0.7/PKG-INFO
--rw-r--r--   0 lchen      (501) staff       (20)      152 2021-04-26 18:35:12.000000 linlangleyprime-0.7/README.md
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.618141 linlangleyprime-0.7/doc/
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.618284 linlangleyprime-0.7/doc/_build/
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.631709 linlangleyprime-0.7/doc/_build/html/
--rw-r--r--   0 lchen      (501) staff       (20)      230 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/.buildinfo
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.634345 linlangleyprime-0.7/doc/_build/html/_sources/
--rw-r--r--   0 lchen      (501) staff       (20)      434 2021-04-27 20:43:59.000000 linlangleyprime-0.7/doc/_build/html/_sources/index.rst.txt
--rw-r--r--   0 lchen      (501) staff       (20)       60 2021-04-27 21:08:07.000000 linlangleyprime-0.7/doc/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 lchen      (501) staff       (20)      492 2021-04-27 20:33:45.000000 linlangleyprime-0.7/doc/_build/html/_sources/primepackage.rst.txt
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.652146 linlangleyprime-0.7/doc/_build/html/_static/
--rw-r--r--   0 lchen      (501) staff       (20)    13647 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/_static/basic.css
--rw-r--r--   0 lchen      (501) staff       (20)     4256 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/_static/classic.css
--rw-r--r--   0 lchen      (501) staff       (20)     9592 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/doctools.js
--rw-r--r--   0 lchen      (501) staff       (20)      350 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/_static/documentation_options.js
--rw-r--r--   0 lchen      (501) staff       (20)      286 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/file.png
--rw-r--r--   0 lchen      (501) staff       (20)   287630 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 lchen      (501) staff       (20)    89476 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/jquery.js
--rw-r--r--   0 lchen      (501) staff       (20)    10854 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/_static/language_data.js
--rw-r--r--   0 lchen      (501) staff       (20)       90 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/minus.png
--rw-r--r--   0 lchen      (501) staff       (20)       90 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/plus.png
--rw-r--r--   0 lchen      (501) staff       (20)    25240 2021-04-27 20:58:28.000000 linlangleyprime-0.7/doc/_build/html/_static/prime.jpeg
--rw-r--r--   0 lchen      (501) staff       (20)     4846 2021-04-27 21:08:11.000000 linlangleyprime-0.7/doc/_build/html/_static/pygments.css
--rw-r--r--   0 lchen      (501) staff       (20)    16582 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/searchtools.js
--rw-r--r--   0 lchen      (501) staff       (20)     4803 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/_static/sidebar.js
--rw-r--r--   0 lchen      (501) staff       (20)    67692 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/underscore-1.12.0.js
--rw-r--r--   0 lchen      (501) staff       (20)    19358 2021-02-22 19:51:20.000000 linlangleyprime-0.7/doc/_build/html/_static/underscore.js
--rw-r--r--   0 lchen      (501) staff       (20)     5648 2021-04-27 21:08:11.000000 linlangleyprime-0.7/doc/_build/html/genindex.html
--rw-r--r--   0 lchen      (501) staff       (20)     5456 2021-04-27 21:08:11.000000 linlangleyprime-0.7/doc/_build/html/index.html
--rw-r--r--   0 lchen      (501) staff       (20)     5025 2021-04-27 21:08:11.000000 linlangleyprime-0.7/doc/_build/html/modules.html
--rw-r--r--   0 lchen      (501) staff       (20)      362 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/objects.inv
--rw-r--r--   0 lchen      (501) staff       (20)    10809 2021-04-27 21:00:13.000000 linlangleyprime-0.7/doc/_build/html/primepackage.html
--rw-r--r--   0 lchen      (501) staff       (20)     4106 2021-04-27 21:08:11.000000 linlangleyprime-0.7/doc/_build/html/py-modindex.html
--rw-r--r--   0 lchen      (501) staff       (20)     3411 2021-04-27 21:08:11.000000 linlangleyprime-0.7/doc/_build/html/search.html
--rw-r--r--   0 lchen      (501) staff       (20)     1628 2021-04-27 21:08:12.000000 linlangleyprime-0.7/doc/_build/html/searchindex.js
--rw-r--r--   0 lchen      (501) staff       (20)      104 2021-04-27 21:25:13.000000 linlangleyprime-0.7/pyproject.toml
--rw-r--r--   0 lchen      (501) staff       (20)       19 2021-04-26 18:36:47.000000 linlangleyprime-0.7/requirements.txt
--rw-r--r--   0 lchen      (501) staff       (20)       63 2021-04-27 22:36:13.660244 linlangleyprime-0.7/setup.cfg
--rw-r--r--   0 lchen      (501) staff       (20)     1588 2021-04-27 22:35:32.000000 linlangleyprime-0.7/setup.py
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.653079 linlangleyprime-0.7/src/
--rw-r--r--   0 lchen      (501) staff       (20)      647 2021-04-26 18:34:28.000000 linlangleyprime-0.7/src/generator
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.655507 linlangleyprime-0.7/src/linlangleyprime.egg-info/
--rw-r--r--   0 lchen      (501) staff       (20)     1146 2021-04-27 22:36:13.000000 linlangleyprime-0.7/src/linlangleyprime.egg-info/PKG-INFO
--rw-r--r--   0 lchen      (501) staff       (20)     1429 2021-04-27 22:36:13.000000 linlangleyprime-0.7/src/linlangleyprime.egg-info/SOURCES.txt
--rw-r--r--   0 lchen      (501) staff       (20)        1 2021-04-27 22:36:13.000000 linlangleyprime-0.7/src/linlangleyprime.egg-info/dependency_links.txt
--rw-r--r--   0 lchen      (501) staff       (20)       19 2021-04-27 22:36:13.000000 linlangleyprime-0.7/src/linlangleyprime.egg-info/requires.txt
--rw-r--r--   0 lchen      (501) staff       (20)       13 2021-04-27 22:36:13.000000 linlangleyprime-0.7/src/linlangleyprime.egg-info/top_level.txt
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.657261 linlangleyprime-0.7/src/primepackage/
--rw-r--r--   0 lchen      (501) staff       (20)      118 2021-04-26 18:29:28.000000 linlangleyprime-0.7/src/primepackage/__init__.py
--rw-r--r--   0 lchen      (501) staff       (20)     1434 2021-04-26 18:30:18.000000 linlangleyprime-0.7/src/primepackage/primeio.py
--rw-r--r--   0 lchen      (501) staff       (20)     1479 2021-04-26 18:30:43.000000 linlangleyprime-0.7/src/primepackage/primemodule.py
-drwxr-xr-x   0 lchen      (501) staff       (20)        0 2021-04-27 22:36:13.658900 linlangleyprime-0.7/test/
--rw-r--r--   0 lchen      (501) staff       (20)      824 2021-04-27 21:22:52.000000 linlangleyprime-0.7/test/test_is_prime.py
--rw-r--r--   0 lchen      (501) staff       (20)     1303 2021-04-27 21:23:56.000000 linlangleyprime-0.7/test/test_suit.py
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.782246 linlangleyprime-0.8/
+-rw-r--r--   0 linchen    (502) staff       (20)      589 2023-07-10 15:56:37.000000 linlangleyprime-0.8/LICENSE
+-rw-r--r--   0 linchen    (502) staff       (20)       79 2023-07-07 18:20:33.000000 linlangleyprime-0.8/MANIFEST.in
+-rw-r--r--   0 linchen    (502) staff       (20)     1803 2023-07-10 16:34:59.782520 linlangleyprime-0.8/PKG-INFO
+-rw-r--r--   0 linchen    (502) staff       (20)      957 2023-07-10 16:01:08.000000 linlangleyprime-0.8/README.md
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.759299 linlangleyprime-0.8/doc/
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.759419 linlangleyprime-0.8/doc/_build/
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.765553 linlangleyprime-0.8/doc/_build/html/
+-rw-r--r--   0 linchen    (502) staff       (20)      230 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/.buildinfo
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.766587 linlangleyprime-0.8/doc/_build/html/_sources/
+-rw-r--r--   0 linchen    (502) staff       (20)      434 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 linchen    (502) staff       (20)       60 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 linchen    (502) staff       (20)      492 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_sources/primepackage.rst.txt
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.774808 linlangleyprime-0.8/doc/_build/html/_static/
+-rw-r--r--   0 linchen    (502) staff       (20)    13647 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/basic.css
+-rw-r--r--   0 linchen    (502) staff       (20)     4256 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/classic.css
+-rw-r--r--   0 linchen    (502) staff       (20)     9592 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 linchen    (502) staff       (20)      350 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/documentation_options.js
+-rw-r--r--   0 linchen    (502) staff       (20)      286 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/file.png
+-rw-r--r--   0 linchen    (502) staff       (20)   287630 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 linchen    (502) staff       (20)    89476 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/jquery.js
+-rw-r--r--   0 linchen    (502) staff       (20)    10854 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/language_data.js
+-rw-r--r--   0 linchen    (502) staff       (20)       90 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/minus.png
+-rw-r--r--   0 linchen    (502) staff       (20)       90 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/plus.png
+-rw-r--r--   0 linchen    (502) staff       (20)    25240 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/prime.jpeg
+-rw-r--r--   0 linchen    (502) staff       (20)     4846 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 linchen    (502) staff       (20)    16582 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 linchen    (502) staff       (20)     4803 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/sidebar.js
+-rw-r--r--   0 linchen    (502) staff       (20)    67692 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/underscore-1.12.0.js
+-rw-r--r--   0 linchen    (502) staff       (20)    19358 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/_static/underscore.js
+-rw-r--r--   0 linchen    (502) staff       (20)     5648 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/genindex.html
+-rw-r--r--   0 linchen    (502) staff       (20)     5456 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/index.html
+-rw-r--r--   0 linchen    (502) staff       (20)     5025 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/modules.html
+-rw-r--r--   0 linchen    (502) staff       (20)      362 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/objects.inv
+-rw-r--r--   0 linchen    (502) staff       (20)    10809 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/primepackage.html
+-rw-r--r--   0 linchen    (502) staff       (20)     4106 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/py-modindex.html
+-rw-r--r--   0 linchen    (502) staff       (20)     3411 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/search.html
+-rw-r--r--   0 linchen    (502) staff       (20)     1628 2023-07-07 18:20:33.000000 linlangleyprime-0.8/doc/_build/html/searchindex.js
+-rw-r--r--   0 linchen    (502) staff       (20)      104 2023-07-07 18:20:33.000000 linlangleyprime-0.8/pyproject.toml
+-rw-r--r--   0 linchen    (502) staff       (20)       19 2023-07-07 18:20:33.000000 linlangleyprime-0.8/requirements.txt
+-rw-r--r--   0 linchen    (502) staff       (20)       63 2023-07-10 16:34:59.783362 linlangleyprime-0.8/setup.cfg
+-rw-r--r--   0 linchen    (502) staff       (20)     1472 2023-07-10 16:34:29.000000 linlangleyprime-0.8/setup.py
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.775330 linlangleyprime-0.8/src/
+-rw-r--r--   0 linchen    (502) staff       (20)      647 2023-07-07 18:20:33.000000 linlangleyprime-0.8/src/generator
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.777887 linlangleyprime-0.8/src/linlangleyprime.egg-info/
+-rw-r--r--   0 linchen    (502) staff       (20)     1803 2023-07-10 16:34:59.000000 linlangleyprime-0.8/src/linlangleyprime.egg-info/PKG-INFO
+-rw-r--r--   0 linchen    (502) staff       (20)     1467 2023-07-10 16:34:59.000000 linlangleyprime-0.8/src/linlangleyprime.egg-info/SOURCES.txt
+-rw-r--r--   0 linchen    (502) staff       (20)        1 2023-07-10 16:34:59.000000 linlangleyprime-0.8/src/linlangleyprime.egg-info/dependency_links.txt
+-rw-r--r--   0 linchen    (502) staff       (20)       19 2023-07-10 16:34:59.000000 linlangleyprime-0.8/src/linlangleyprime.egg-info/requires.txt
+-rw-r--r--   0 linchen    (502) staff       (20)       13 2023-07-10 16:34:59.000000 linlangleyprime-0.8/src/linlangleyprime.egg-info/top_level.txt
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.779336 linlangleyprime-0.8/src/primepackage/
+-rw-r--r--   0 linchen    (502) staff       (20)      118 2023-07-07 18:20:33.000000 linlangleyprime-0.8/src/primepackage/__init__.py
+-rw-r--r--   0 linchen    (502) staff       (20)     1434 2023-07-07 18:20:33.000000 linlangleyprime-0.8/src/primepackage/primeio.py
+-rw-r--r--   0 linchen    (502) staff       (20)     1479 2023-07-07 18:20:33.000000 linlangleyprime-0.8/src/primepackage/primemodule.py
+drwxr-xr-x   0 linchen    (502) staff       (20)        0 2023-07-10 16:34:59.781581 linlangleyprime-0.8/test/
+-rw-r--r--   0 linchen    (502) staff       (20)      189 2023-07-07 18:20:33.000000 linlangleyprime-0.8/test/test_assert.py
+-rw-r--r--   0 linchen    (502) staff       (20)      824 2023-07-07 18:20:33.000000 linlangleyprime-0.8/test/test_is_prime.py
+-rw-r--r--   0 linchen    (502) staff       (20)      132 2023-07-07 18:20:33.000000 linlangleyprime-0.8/test/test_nose.py
+-rw-r--r--   0 linchen    (502) staff       (20)     1303 2023-07-07 18:20:33.000000 linlangleyprime-0.8/test/test_suit.py
```

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/basic.css` & `linlangleyprime-0.8/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/classic.css` & `linlangleyprime-0.8/doc/_build/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/doctools.js` & `linlangleyprime-0.8/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/jquery-3.5.1.js` & `linlangleyprime-0.8/doc/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/jquery.js` & `linlangleyprime-0.8/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/language_data.js` & `linlangleyprime-0.8/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/prime.jpeg` & `linlangleyprime-0.8/doc/_build/html/_static/prime.jpeg`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/pygments.css` & `linlangleyprime-0.8/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/searchtools.js` & `linlangleyprime-0.8/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/sidebar.js` & `linlangleyprime-0.8/doc/_build/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/underscore-1.12.0.js` & `linlangleyprime-0.8/doc/_build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/_static/underscore.js` & `linlangleyprime-0.8/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/genindex.html` & `linlangleyprime-0.8/doc/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/index.html` & `linlangleyprime-0.8/doc/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/modules.html` & `linlangleyprime-0.8/doc/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/primepackage.html` & `linlangleyprime-0.8/doc/_build/html/primepackage.html`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/py-modindex.html` & `linlangleyprime-0.8/doc/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/search.html` & `linlangleyprime-0.8/doc/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/doc/_build/html/searchindex.js` & `linlangleyprime-0.8/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/setup.py` & `linlangleyprime-0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import setuptools
- 
+
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
- 
+
 setuptools.setup(
     setup_requires=[
         'pytest-runner',
     ],
     tests_require=['pytest'],
     name='linlangleyprime', # a unique name for PyPI
-    version='0.7',
+    version='0.8',
     author='Lin Chen, Yanhua Feng',
     author_email='lin.chen@ieee.org, yf@vims.edu',
     description='Demo for building a Python project',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='http://lin-chen-langley.github.io',
     project_urls = {
         'PyPI': 'https://pypi.org/manage/project/linlangleyprime/releases/',
-        'Conda': 'https://anaconda.org/linchenVA/linlangleyprime'
         },
     classifiers=[
-      'Development Status :: 4 - Beta',
+      'Development Status :: 1 - Planning',
       'Environment :: X11 Applications :: GTK',
       'Intended Audience :: End Users/Desktop',
       'Intended Audience :: Developers',
-      'License :: OSI Approved :: GNU General Public License (GPL)',
+      'License :: OSI Approved :: Apache Software License',
       'Operating System :: POSIX :: Linux',
       'Programming Language :: Python',
       'Topic :: Desktop Environment',
       'Topic :: Text Processing :: Fonts'
       ],
     install_requires=requirements,
     package_dir={'':'src'}, # location to find the packages
     packages=setuptools.find_packages(where="src"),
     #packages=['primepackage', ], # packages and subpackages containing .py files
-    python_requires=">=3.9",
+    python_requires=">=3.11",
     scripts=['src/generator',], # the executable files will be installed for user
-    license='Creative Commons Attribution-Noncommercial-Share Alike license',
+    license='Apache License 2.0',
 )
```

### Comparing `linlangleyprime-0.7/src/generator` & `linlangleyprime-0.8/src/generator`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/src/linlangleyprime.egg-info/SOURCES.txt` & `linlangleyprime-0.8/src/linlangleyprime.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,9 +38,11 @@
 src/linlangleyprime.egg-info/SOURCES.txt
 src/linlangleyprime.egg-info/dependency_links.txt
 src/linlangleyprime.egg-info/requires.txt
 src/linlangleyprime.egg-info/top_level.txt
 src/primepackage/__init__.py
 src/primepackage/primeio.py
 src/primepackage/primemodule.py
+test/test_assert.py
 test/test_is_prime.py
+test/test_nose.py
 test/test_suit.py
```

### Comparing `linlangleyprime-0.7/src/primepackage/primeio.py` & `linlangleyprime-0.8/src/primepackage/primeio.py`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/src/primepackage/primemodule.py` & `linlangleyprime-0.8/src/primepackage/primemodule.py`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/test/test_is_prime.py` & `linlangleyprime-0.8/test/test_is_prime.py`

 * *Files identical despite different names*

### Comparing `linlangleyprime-0.7/test/test_suit.py` & `linlangleyprime-0.8/test/test_suit.py`

 * *Files identical despite different names*

