# Comparing `tmp/pipedi-0.0.1.tar.gz` & `tmp/pipedi-0.0.2.tar.gz`

## Comparing `pipedi-0.0.1.tar` & `pipedi-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pipedi-0.0.1/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pipedi-0.0.1/src/pipedi/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pipedi-0.0.1/src/pipedi/pipy.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pipedi-0.0.1/src/pipedi/util/text.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pipedi-0.0.1/tests/test.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pipedi-0.0.1/tests/test_pipable.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pipedi-0.0.1/tests/test_piped.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pipedi-0.0.1/tests/test_util_text.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pipedi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pipedi-0.0.1/LICENCE
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 pipedi-0.0.1/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pipedi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pipedi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 pipedi-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pipedi-0.0.2/src/pipedi/__init__.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pipedi-0.0.2/src/pipedi/pipy.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pipedi-0.0.2/src/pipedi/util/text.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pipedi-0.0.2/tests/test.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pipedi-0.0.2/tests/test_pipable.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pipedi-0.0.2/tests/test_piped.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pipedi-0.0.2/tests/test_util_text.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pipedi-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pipedi-0.0.2/LICENCE
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pipedi-0.0.2/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pipedi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pipedi-0.0.2/PKG-INFO
```

### Comparing `pipedi-0.0.1/requirements.txt` & `pipedi-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/src/pipedi/util/text.py` & `pipedi-0.0.2/src/pipedi/util/text.py`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/tests/test.py` & `pipedi-0.0.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/tests/test_pipable.py` & `pipedi-0.0.2/tests/test_pipable.py`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/tests/test_piped.py` & `pipedi-0.0.2/tests/test_piped.py`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/tests/test_util_text.py` & `pipedi-0.0.2/tests/test_util_text.py`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/.gitignore` & `pipedi-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/LICENCE` & `pipedi-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pipedi-0.0.1/README.md` & `pipedi-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pipy
+# Pipedi
 
 A simple Python package that enables piping iterables to functions with the pipe `|` character like in a shell.
 
 ```python
 with open('input.txt', 'r') as input_file:
     res = list(input_file \
                 | strip('\n') \
@@ -90,33 +90,25 @@
 ```
 
 
 ## Building
 
 ```bash
 # Clone this repository
-$ git clone git@github.com:akupar/pipy.git
-$ cd pipy
+$ git clone git@github.com:akupar/pipedi.git
+$ cd pipedi
 # Create virtual environment
-.../pipy$ python -m venv venv
+.../pipedi$ python -m venv venv
 # Activate virtual environment
-.../pipy$ . venv/bin/activate
+.../pipedi$ . venv/bin/activate
 # Install requirements
-(venv) .../pipy$ pip install -r requirements.txt
-# Install the pipy package in editable mode
-(venv) .../pipy$ pip install -e .
+(venv) .../pipedi$ pip install -r requirements.txt
+# Install the pipedi package in editable mode
+(venv) .../pipedi$ pip install -e .
 # Run tests
-(venv) .../pipy$ python -m pytest
+(venv) .../pipedi$ python -m pytest
 # Preview readme
-(venv) .../pipy$ grip -b README.md
+(venv) .../pipedi$ grip -b README.md
 # Build package
-(venv) .../pipy$ python -m build
-
-# Upload package (for myself)
-(venv) .../pipy$ python -m twine upload --repository testpypi dist/*
-
-# Test package
-.../testpipy$ python -m venv venv
-.../testpipy$ . venv/bin/activate
-(venv) .../testpipy$ pip install --index-url https://test.pypi.org/simple/ --no-deps pipy
+(venv) .../pipedi$ python -m build
 
 ``´
```

### Comparing `pipedi-0.0.1/pyproject.toml` & `pipedi-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pipedi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Antti Kuparinen", email="teknovelho@gmail.com" },
 ]
 description = "Enables piping iterables to functions with the pipe character"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pipedi-0.0.1/PKG-INFO` & `pipedi-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pipedi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Enables piping iterables to functions with the pipe character
 Project-URL: Homepage, https://github.com/akupar/pipy
 Project-URL: Bug Tracker, https://github.com/akupar/pipy/issues
 Author-email: Antti Kuparinen <teknovelho@gmail.com>
 License-File: LICENCE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# Pipy
+# Pipedi
 
 A simple Python package that enables piping iterables to functions with the pipe `|` character like in a shell.
 
 ```python
 with open('input.txt', 'r') as input_file:
     res = list(input_file \
                 | strip('\n') \
@@ -106,33 +106,25 @@
 ```
 
 
 ## Building
 
 ```bash
 # Clone this repository
-$ git clone git@github.com:akupar/pipy.git
-$ cd pipy
+$ git clone git@github.com:akupar/pipedi.git
+$ cd pipedi
 # Create virtual environment
-.../pipy$ python -m venv venv
+.../pipedi$ python -m venv venv
 # Activate virtual environment
-.../pipy$ . venv/bin/activate
+.../pipedi$ . venv/bin/activate
 # Install requirements
-(venv) .../pipy$ pip install -r requirements.txt
-# Install the pipy package in editable mode
-(venv) .../pipy$ pip install -e .
+(venv) .../pipedi$ pip install -r requirements.txt
+# Install the pipedi package in editable mode
+(venv) .../pipedi$ pip install -e .
 # Run tests
-(venv) .../pipy$ python -m pytest
+(venv) .../pipedi$ python -m pytest
 # Preview readme
-(venv) .../pipy$ grip -b README.md
+(venv) .../pipedi$ grip -b README.md
 # Build package
-(venv) .../pipy$ python -m build
-
-# Upload package (for myself)
-(venv) .../pipy$ python -m twine upload --repository testpypi dist/*
-
-# Test package
-.../testpipy$ python -m venv venv
-.../testpipy$ . venv/bin/activate
-(venv) .../testpipy$ pip install --index-url https://test.pypi.org/simple/ --no-deps pipy
+(venv) .../pipedi$ python -m build
 
 ``´
```

