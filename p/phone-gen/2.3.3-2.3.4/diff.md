# Comparing `tmp/phone_gen-2.3.3.tar.gz` & `tmp/phone_gen-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_gen-2.3.3.tar", last modified: Fri Jun 23 09:12:11 2023, max compression
+gzip compressed data, was "phone_gen-2.3.4.tar", last modified: Mon Jul 10 09:33:40 2023, max compression
```

## Comparing `phone_gen-2.3.3.tar` & `phone_gen-2.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.195633 phone_gen-2.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.195633 phone_gen-2.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 09:11:55.000000 phone_gen-2.3.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-23 09:11:55.000000 phone_gen-2.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-23 09:11:55.000000 phone_gen-2.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 09:11:55.000000 phone_gen-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-23 09:12:11.199633 phone_gen-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-23 09:11:55.000000 phone_gen-2.3.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-23 09:11:55.000000 phone_gen-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-23 09:11:55.000000 phone_gen-2.3.3/dev_tools/patterns_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-23 09:11:55.000000 phone_gen-2.3.3/dev_tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/phone_gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/iso3.py
--rw-r--r--   0 runner    (1001) docker     (123)    87966 2023-06-23 09:11:55.000000 phone_gen-2.3.3/phone_gen/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/phone_gen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 09:12:11.000000 phone_gen-2.3.3/phone_gen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 09:12:11.203633 phone_gen-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-23 09:11:55.000000 phone_gen-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:12:11.199633 phone_gen-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_alt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_load_alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-23 09:11:55.000000 phone_gen-2.3.3/tests/test_phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.444941 phone_gen-2.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.440941 phone_gen-2.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.440941 phone_gen-2.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-10 09:33:29.000000 phone_gen-2.3.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-10 09:33:29.000000 phone_gen-2.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-10 09:33:29.000000 phone_gen-2.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-10 09:33:29.000000 phone_gen-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-10 09:33:40.444941 phone_gen-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 09:33:29.000000 phone_gen-2.3.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-10 09:33:29.000000 phone_gen-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.440941 phone_gen-2.3.4/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-10 09:33:29.000000 phone_gen-2.3.4/dev_tools/patterns_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-10 09:33:29.000000 phone_gen-2.3.4/dev_tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.440941 phone_gen-2.3.4/phone_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 09:33:40.000000 phone_gen-2.3.4/phone_gen/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/iso3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87972 2023-07-10 09:33:29.000000 phone_gen-2.3.4/phone_gen/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.440941 phone_gen-2.3.4/phone_gen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-10 09:33:40.000000 phone_gen-2.3.4/phone_gen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-10 09:33:40.000000 phone_gen-2.3.4/phone_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:33:40.000000 phone_gen-2.3.4/phone_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 09:33:40.000000 phone_gen-2.3.4/phone_gen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:33:40.000000 phone_gen-2.3.4/phone_gen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 09:33:40.444941 phone_gen-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-10 09:33:29.000000 phone_gen-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:40.444941 phone_gen-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 09:33:29.000000 phone_gen-2.3.4/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-10 09:33:29.000000 phone_gen-2.3.4/tests/test_alt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-10 09:33:29.000000 phone_gen-2.3.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-10 09:33:29.000000 phone_gen-2.3.4/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-10 09:33:29.000000 phone_gen-2.3.4/tests/test_load_alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-10 09:33:29.000000 phone_gen-2.3.4/tests/test_phone.py
```

### Comparing `phone_gen-2.3.3/.github/workflows/python-package.yml` & `phone_gen-2.3.4/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 jobs:
   build:
 
     runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
       matrix:
-        python-version: [ "3.7", "3.8", "3.9", "3.10", "3.11" ]
+        python-version: [ "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev" ]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.15
+          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.16
           python -m pip install -e .
       - name: Flake8
         run: |
           flake8 phone_gen
       - name: Black
         run: |
           black --check phone_gen
```

### Comparing `phone_gen-2.3.3/.github/workflows/python-publish.yml` & `phone_gen-2.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/.gitignore` & `phone_gen-2.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/LICENSE` & `phone_gen-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/PKG-INFO` & `phone_gen-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.3.3
+Version: 2.3.4
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Communications :: Telephony
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phone_gen-2.3.3/README.md` & `phone_gen-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/dev_tools/patterns_generator.py` & `phone_gen-2.3.4/dev_tools/patterns_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/dev_tools/update.py` & `phone_gen-2.3.4/dev_tools/update.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/__init__.py` & `phone_gen-2.3.4/phone_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/_generator.py` & `phone_gen-2.3.4/phone_gen/_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/alt_patterns.py` & `phone_gen-2.3.4/phone_gen/alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/cli.py` & `phone_gen-2.3.4/phone_gen/cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/country_name.py` & `phone_gen-2.3.4/phone_gen/country_name.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/iso3.py` & `phone_gen-2.3.4/phone_gen/iso3.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/phone_gen/patterns.py` & `phone_gen-2.3.4/phone_gen/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2023-06-23 09:05:07 UTC
-Resource: https://github.com/google/libphonenumber v8.13.15
+Auto-generated file 2023-07-10 09:22:21 UTC
+Resource: https://github.com/google/libphonenumber v8.13.16
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.13.15",
+    "info": "libphonenumber v8.13.16",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -171,15 +171,15 @@
         "BT": {
             "code": "975",
             "pattern": "(((2[3-6])|([34][5-7])|(5[236])|(6[2-46])|(7[246])|(8[2-4])[\\d]{5}))",
             "mobile": "(((1[67])|(77)[\\d]{6}))",
         },
         "BW": {
             "code": "267",
-            "pattern": "(((2(4[0-48])|(6[0-24])|(9[0578]))|(3(1[0-35-9])|(55)|([69][\\d])|(7[013]))|(4(6[03])|(7[1267])|(9[0-5]))|(5(3[03489])|(4[0489])|(7[1-47])|(88)|(9[0-49]))|(6(2[1-35])|(5[149])|(8[067]))[\\d]{4}))",
+            "pattern": "(((2(4[0-48])|(6[0-24])|(9[0578]))|(3(1[0-35-9])|(55)|([69][\\d])|(7[013])|(81))|(4(6[03])|(7[1267])|(9[0-5]))|(5(3[03489])|(4[0489])|(7[1-47])|(88)|(9[0-49]))|(6(2[1-35])|(5[149])|(8[067]))[\\d]{4}))",
             "mobile": "(((321)|(7([1-7][\\d])|(8[0-4]))[\\d]{5}))",
         },
         "BY": {
             "code": "375",
             "pattern": "(((1(5(1[1-5])|([24][\\d])|(6[2-4])|(9[1-7]))|(6([235][\\d])|(4[1-7]))|(7[\\d][\\d]))|(2(1([246][\\d])|(3[0-35-9])|(5[1-9]))|(2([235][\\d])|(4[0-8]))|(3([26][\\d])|(3[02-79])|(4[024-7])|(5[03-7])))[\\d]{5}))",
             "mobile": "(((2(5[5-79])|(9[1-9]))|((33)|(44)[\\d])[\\d]{6}))",
         },
@@ -317,15 +317,15 @@
             "code": "593",
             "pattern": "(([2-7][2-7][\\d]{6}))",
             "mobile": "((964[0-2][\\d]{5})|(9(39)|([57][89])|(6[0-36-9])|([89][\\d])[\\d]{6}))",
         },
         "EE": {
             "code": "372",
             "pattern": "(((3[23589])|(4[3-8])|(6[\\d])|(7[1-9])|(88)[\\d]{5}))",
-            "mobile": "(((5[\\d]{5})|(8(1(0(000)|([3-9][\\d][\\d]))|((1(0[236])|(1[\\d]))|((2[0-59])|([3-79][\\d])[\\d])[\\d]))|(2(0(000)|((19)|([2-7][\\d])[\\d]))|((([124-6][\\d])|(3[5-9])[\\d])|(7([0-3679][\\d])|(8[13-9]))|(8([2-6][\\d])|(7[01]))[\\d]))|([349][\\d]{4}))[\\d][\\d])|(5(([02][\\d])|(5[0-478])[\\d])|(1([0-8][\\d])|(95))|(6(4[0-4])|(5[1-589]))[\\d]{3}))",
+            "mobile": "(((5[\\d]{5})|(8(1(0(000)|([3-9][\\d][\\d]))|((1(0[236])|(1[\\d]))|((2[0-59])|([3-79][\\d])[\\d])[\\d]))|(2(0(000)|((19)|([2-7][\\d])[\\d]))|((([124-6][\\d])|(3[5-9])[\\d])|(7([0-79][\\d])|(8[13-9]))|(8([2-6][\\d])|(7[01]))[\\d]))|([349][\\d]{4}))[\\d][\\d])|(5(([02][\\d])|(5[0-478])[\\d])|(1([0-8][\\d])|(95))|(6(4[0-4])|(5[1-589]))[\\d]{3}))",
         },
         "EG": {
             "code": "20",
             "pattern": "((13[23][\\d]{6})|((15)|(57)[\\d]{6:7})|((2[2-4])|(3)|(4[05-8])|(5[05])|(6[24-689])|(8[2468])|(9[235-7])[\\d]{7}))",
             "mobile": "((1[0-25][\\d]{8}))",
         },
         "EH": {
@@ -542,15 +542,15 @@
         "JE": {
             "code": "44",
             "pattern": "((1534[0-24-8][\\d]{5}))",
             "mobile": "((7(((50)|(82)9)|(937)[\\d])|(7(00[378])|(97[7-9]))[\\d]{5}))",
         },
         "JM": {
             "code": "1",
-            "pattern": "((8766060[\\d]{3})|((658(2([0-8][\\d])|(9[0-46-9]))|([3-9][\\d][\\d]))|(876(52[35])|(6(0[1-3579])|(1[0235-9])|([23][\\d])|(40)|(5[06])|(6[2-589])|(7[025-9])|(8[04])|(9[4-9]))|(7(0[2-689])|([1-6][\\d])|(8[056])|(9[45]))|(9(0[1-8])|(1[02378])|([2-8][\\d])|(9[2-468])))[\\d]{4}))",
+            "pattern": "((8766060[\\d]{3})|((658(2([0-8][\\d])|(9[0-46-9]))|([3-9][\\d][\\d]))|(876(52[35])|(6(0[1-3579])|(1[0235-9])|([23][\\d])|(40)|(5[06])|(6[2-589])|(7[0-25-9])|(8[04])|(9[4-9]))|(7(0[2-689])|([1-6][\\d])|(8[056])|(9[45]))|(9(0[1-8])|(1[02378])|([2-8][\\d])|(9[2-468])))[\\d]{4}))",
             "mobile": "(((658295)|(876(2(0[1-9])|([13-9][\\d])|(2[013-9]))|([348][\\d][\\d])|(5(0[1-9])|([1-9][\\d]))|(6(4[89])|(6[67]))|(7(0[07])|(7[\\d])|(8[1-47-9])|(9[0-36-9]))|(9([01]9)|(9[0579])))[\\d]{4}))",
         },
         "JO": {
             "code": "962",
             "pattern": "((87(000)|(90[01])[\\d]{3})|((2(6(2[0-35-9])|(3[0-578])|(4[24-7])|(5[0-24-8])|([6-8][023])|(9[0-3]))|(7(0[1-79])|(10)|(2[014-7])|(3[0-689])|(4[019])|(5[0-3578])))|(32(0[1-69])|(1[1-35-7])|(2[024-7])|(3[\\d])|(4[0-3])|([5-7][023]))|(53(0[0-3])|([13][023])|(2[0-59])|(49)|(5[0-35-9])|(6[15])|(7[45])|(8[1-6])|(9[0-36-9]))|(6(2([05]0)|(22))|(3(00)|(33))|(4(0[0-25])|(1[2-7])|(2[0569])|([38][07-9])|(4[025689])|(6[0-589])|(7[\\d])|(9[0-2]))|(5([01][056])|(2[034])|(3[0-57-9])|(4[178])|(5[0-69])|(6[0-35-9])|(7[1-379])|(8[0-68])|(9[0239])))|(87(20)|(7[078])|(99))[\\d]{4}))",
             "mobile": "((7([78][0-25-9])|(9[\\d])[\\d]{6}))",
         },
@@ -563,15 +563,15 @@
             "code": "254",
             "pattern": "(((4[245])|(5[1-79])|(6[01457-9])[\\d]{5:7})|((4[136])|(5[08])|(62)[\\d]{7})|(([24]0)|(66)[\\d]{6:7}))",
             "mobile": "(((1(0[0-6])|(1[0-5])|(2[014])|(30))|(7[\\d][\\d])[\\d]{6}))",
         },
         "KG": {
             "code": "996",
             "pattern": "((312(5[0-79][\\d])|(9([0-689][\\d])|(7[0-24-9]))[\\d]{3})|((3(1(2[0-46-8])|(3[1-9])|(47)|([56][\\d]))|(2(22)|(3[0-479])|(6[0-7]))|(4(22)|(5[6-9])|(6[\\d]))|(5(22)|(3[4-7])|(59)|(6[\\d]))|(6(22)|(5[35-7])|(6[\\d]))|(7(22)|(3[468])|(4[1-9])|(59)|([67][\\d]))|(9(22)|(4[1-8])|(6[\\d])))|(6(09)|(12)|(2[2-4])[\\d])[\\d]{5}))",
-            "mobile": "((312(58[\\d])|(973)[\\d]{3})|((2(0[0-35])|(2[\\d]))|(5[0-24-7][\\d])|(600)|(7([07][\\d])|(55))|(88[08])|(99[05-9])[\\d]{6}))",
+            "mobile": "((312(58[\\d])|(973)[\\d]{3})|((2(0[0-35])|(2[\\d]))|(5[0-24-7][\\d])|(600)|(7([07][\\d])|(55))|(88[08])|(9(12)|(9[05-9]))[\\d]{6}))",
         },
         "KH": {
             "code": "855",
             "pattern": "((23(4([2-4])|([56][\\d]))|([568][\\d][\\d])[\\d]{4})|(23[236-9][\\d]{5})|((2[4-6])|(3[2-6])|(4[2-4])|([5-7][2-5])(([237-9])|(4[56])|(5[\\d])[\\d]{5})|(6[\\d]{5:6})))",
             "mobile": "((((1[28])|(3[18])|(9[67])[\\d])|(6[016-9])|(7([07-9])|([16][\\d]))|(8([013-79])|(8[\\d]))[\\d]{6})|((1[\\d])|(9[0-57-9])[\\d]{6})|((2[3-6])|(3[2-6])|(4[2-4])|([5-7][2-5])48[\\d]{5}))",
         },
         "KI": {
@@ -878,15 +878,15 @@
         "PL": {
             "code": "48",
             "pattern": "((47[\\d]{7})|((1[2-8])|(2[2-69])|(3[2-4])|(4[1-468])|(5[24-689])|(6[1-3578])|(7[14-7])|(8[1-79])|(9[145])([02-9][\\d]{6})|(1([0-8][\\d]{5})|(9[\\d]{3}([\\d]{2})?))))",
             "mobile": "((21(1([145][\\d])|(3[1-5]))|(2[0-4][\\d])[\\d]{4})|((45)|(5[0137])|(6[069])|(7[2389])|(88)[\\d]{7}))",
         },
         "PM": {
             "code": "508",
-            "pattern": "(((4[1-356])|(50)[\\d]{4}))",
+            "pattern": "(((4[1-35-7])|(5[01])[\\d]{4}))",
             "mobile": "(((4[02-4])|(5[056])|(708[45][0-5])[\\d]{4}))",
         },
         "PR": {
             "code": "1",
             "pattern": "(((787)|(939)[2-9][\\d]{6}))",
             "mobile": "(((787)|(939)[2-9][\\d]{6}))",
         },
@@ -964,15 +964,15 @@
             "code": "46",
             "pattern": "(((([12][136])|(3[356])|(4[0246])|(6[03])|(8[\\d])[\\d])|(90[1-9])[\\d]{4:6})|((1(2[0-35])|(4[0-4])|(5[0-25-9])|(7[13-6])|([89][\\d]))|(2(2[0-7])|(4[0136-8])|(5[0138])|(7[018])|(8[01])|(9[0-57]))|(3(0[0-4])|(1[\\d])|(2[0-25])|(4[056])|(7[0-2])|(8[0-3])|(9[023]))|(4(1[013-8])|(3[0135])|(5[14-79])|(7[0-246-9])|(8[0156])|(9[0-689]))|(5(0[0-6])|([15][0-5])|(2[0-68])|(3[0-4])|(4[\\d])|(6[03-5])|(7[013])|(8[0-79])|(9[01]))|(6(1[1-3])|(2[0-4])|(4[02-57])|(5[0-37])|(6[0-3])|(7[0-2])|(8[0247])|(9[0-356]))|(9(1[0-68])|(2[\\d])|(3[02-5])|(4[0-3])|(5[0-4])|([68][01])|(7[0135-8]))[\\d]{5:6}))",
             "mobile": "((7[02369][\\d]{7}))",
         },
         "SG": {
             "code": "65",
             "pattern": "((662[0-24-9][\\d]{4})|(6([0-578][\\d])|(6[013-57-9])|(9[0-35-9])[\\d]{5}))",
-            "mobile": "((8(06[0-689])|(95[0-2])[\\d]{4})|((8(0[1-5])|([1-8][\\d])|(9[0-4]))|(9[0-8][\\d])[\\d]{5}))",
+            "mobile": "((8(07[01])|(95[0-2])[\\d]{4})|((8(0[1-6])|([1-8][\\d])|(9[0-4]))|(9[0-8][\\d])[\\d]{5}))",
         },
         "SH": {
             "code": "290",
             "pattern": "((2([0-57-9][\\d])|(6[4-9])[\\d][\\d]))",
             "mobile": "(([56][\\d]{4}))",
         },
         "SI": {
@@ -1023,16 +1023,16 @@
         "ST": {
             "code": "239",
             "pattern": "((22[\\d]{5}))",
             "mobile": "((900[5-9][\\d]{3})|(9(0[1-9])|([89][\\d])[\\d]{4}))",
         },
         "SV": {
             "code": "503",
-            "pattern": "((2(([1-6][\\d][\\d])|(990)[\\d])|(790[034])|(890[0245])[\\d]{3}))",
-            "mobile": "((66([02-9][\\d][\\d])|(1([02-9][\\d])|(16))[\\d]{3})|((6[0-57-9])|(7[\\d])[\\d]{6}))",
+            "pattern": "((2(79(0[0347-9])|([1-9][\\d]))|(89(0[024589])|([1-9][\\d]))[\\d]{3})|(2([1-69][\\d])|([78][0-8])[\\d]{5}))",
+            "mobile": "(([67][\\d]{7}))",
         },
         "SX": {
             "code": "1",
             "pattern": "((7215(4[2-8])|(8[239])|(9[056])[\\d]{4}))",
             "mobile": "((7215(1[02])|(2[\\d])|(5[034679])|(8[014-8])[\\d]{4}))",
         },
         "SY": {
@@ -1065,15 +1065,15 @@
             "code": "66",
             "pattern": "(((1[0689])|(2[\\d])|(3[2-9])|(4[2-5])|(5[2-6])|(7[3-7])[\\d]{6}))",
             "mobile": "((671[0-8][\\d]{5})|((14)|(6[1-6])|([89][\\d])[\\d]{7}))",
         },
         "TJ": {
             "code": "992",
             "pattern": "(((3(1[3-5])|(2[245])|(3[12])|(4[24-7])|(5[25])|(72))|(4(46)|(74)|(87))[\\d]{6}))",
-            "mobile": "((41[18][\\d]{6})|((0[0-27])|(1[017])|(2[02])|([34]0)|(5[05])|(7[0178])|(8[078])|(9[\\d])[\\d]{7}))",
+            "mobile": "(((0[348]0)|(41[18])|(81[1-9])[\\d]{6})|((0[0-27])|(1[017])|(2[02])|([34]0)|(5[05])|(7[0178])|(8[078])|(9[\\d])[\\d]{7}))",
         },
         "TK": {
             "code": "690",
             "pattern": "(((2[2-4])|([34][\\d])[\\d]{2:5}))",
             "mobile": "((7[2-4][\\d]{2:5}))",
         },
         "TL": {
```

### Comparing `phone_gen-2.3.3/phone_gen.egg-info/PKG-INFO` & `phone_gen-2.3.4/phone_gen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone-gen
-Version: 2.3.3
+Version: 2.3.4
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Communications :: Telephony
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phone_gen-2.3.3/phone_gen.egg-info/SOURCES.txt` & `phone_gen-2.3.4/phone_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/setup.py` & `phone_gen-2.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,14 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Testing",
         "Topic :: Communications :: Telephony",
     ],
 )
```

### Comparing `phone_gen-2.3.3/tests/test_alt_pattern.py` & `phone_gen-2.3.4/tests/test_alt_pattern.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/tests/test_cli.py` & `phone_gen-2.3.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/tests/test_generator.py` & `phone_gen-2.3.4/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/tests/test_load_alt_patterns.py` & `phone_gen-2.3.4/tests/test_load_alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.3/tests/test_phone.py` & `phone_gen-2.3.4/tests/test_phone.py`

 * *Files identical despite different names*

