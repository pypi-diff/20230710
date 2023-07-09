# Comparing `tmp/pytest_embedded_serial-1.3.3.tar.gz` & `tmp/pytest_embedded_serial-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_serial-1.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_serial-1.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_serial-1.3.3.tar` & `pytest_embedded_serial-1.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/LICENSE
--rw-r--r--   0        0        0      195 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/README.md
--rw-r--r--   0        0        0     2898 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      176 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/pytest_embedded_serial/__init__.py
--rw-r--r--   0        0        0     1271 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/pytest_embedded_serial/dut.py
--rw-r--r--   0        0        0     6113 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/pytest_embedded_serial/serial.py
--rw-r--r--   0        0        0     1653 2023-07-05 01:18:10.855964 pytest_embedded_serial-1.3.3/tests/test_serial.py
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/LICENSE
+-rw-r--r--   0        0        0      195 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/README.md
+-rw-r--r--   0        0        0     2898 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/pytest_embedded_serial/__init__.py
+-rw-r--r--   0        0        0     1271 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/pytest_embedded_serial/dut.py
+-rw-r--r--   0        0        0     6113 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/pytest_embedded_serial/serial.py
+-rw-r--r--   0        0        0     1653 2023-07-09 23:36:39.756581 pytest_embedded_serial-1.3.4/tests/test_serial.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.3.4/PKG-INFO
```

### Comparing `pytest_embedded_serial-1.3.3/LICENSE` & `pytest_embedded_serial-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.3.3/pyproject.toml` & `pytest_embedded_serial-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.3.3",
+    "pytest-embedded~=1.3.4",
     "pyserial~=3.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
```

### Comparing `pytest_embedded_serial-1.3.3/pytest_embedded_serial/dut.py` & `pytest_embedded_serial-1.3.4/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.3.3/pytest_embedded_serial/serial.py` & `pytest_embedded_serial-1.3.4/pytest_embedded_serial/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.3.3/tests/test_serial.py` & `pytest_embedded_serial-1.3.4/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.3.3/PKG-INFO` & `pytest_embedded_serial-1.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-serial
-Version: 1.3.3
+Version: 1.3.4
 Summary: Make pytest-embedded plugin work with Serial.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.3.3
+Requires-Dist: pytest-embedded~=1.3.4
 Requires-Dist: pyserial~=3.0
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 
 ### pytest-embedded-serial
```

