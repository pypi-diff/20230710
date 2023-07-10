# Comparing `tmp/pydaraja-0.1.1.tar.gz` & `tmp/pydaraja-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydaraja-0.1.1.tar", last modified: Sun Jul  9 22:07:36 2023, max compression
+gzip compressed data, was "pydaraja-0.1.2.tar", last modified: Mon Jul 10 02:43:14 2023, max compression
```

## Comparing `pydaraja-0.1.1.tar` & `pydaraja-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:07:36.901302 pydaraja-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-09 22:07:25.000000 pydaraja-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-09 22:07:36.901302 pydaraja-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-09 22:07:25.000000 pydaraja-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:07:36.901302 pydaraja-0.1.1/pydaraja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:07:25.000000 pydaraja-0.1.1/pydaraja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:07:25.000000 pydaraja-0.1.1/pydaraja/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-09 22:07:25.000000 pydaraja-0.1.1/pydaraja/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-09 22:07:25.000000 pydaraja-0.1.1/pydaraja/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:07:36.901302 pydaraja-0.1.1/pydaraja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-09 22:07:36.000000 pydaraja-0.1.1/pydaraja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-09 22:07:36.000000 pydaraja-0.1.1/pydaraja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:07:36.000000 pydaraja-0.1.1/pydaraja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 22:07:36.000000 pydaraja-0.1.1/pydaraja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 22:07:36.000000 pydaraja-0.1.1/pydaraja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-09 22:07:25.000000 pydaraja-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:07:36.901302 pydaraja-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:14.045783 pydaraja-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 02:43:02.000000 pydaraja-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 02:43:14.041782 pydaraja-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-10 02:43:02.000000 pydaraja-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:14.041782 pydaraja-0.1.2/pydaraja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:14.041782 pydaraja-0.1.2/pydaraja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:43:14.045783 pydaraja-0.1.2/setup.cfg
```

### Comparing `pydaraja-0.1.1/LICENSE` & `pydaraja-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydaraja-0.1.1/PKG-INFO` & `pydaraja-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pydaraja
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for Mpesa Daraja API
 Author-email: Raymond Kipkorir <raykipkorir02@gmail.com>
 Project-URL: Homepage, https://github.com/raykipkorir/pydaraja
 Project-URL: Bug Tracker, https://github.com/raykipkorir/pydaraja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydaraja
 
 ## Description
-This is a python wrapper that handles payment requests through th Daraja Mpesa API.
+This is a python wrapper that handles payment requests through the Daraja Mpesa API.
 
 Daraja API services offered by pydaraja are:
 - Lipa na M-PESA online API also known as M-PESA express (STK Push/NI push)
 - STK push query API -> Used to check the status of Lipa na Mpesa online payment
 
 More services will come soon.
 
@@ -39,12 +39,17 @@
 payment.CALLBACK_URL = "YOUR_CALLBACK_URL"
 
 payment.ACCOUNT_REFERENCE = "YOUR_ACCOUNT_REFERENCE"
 payment.TRANSACTION_DESC = "YOUR_TRANSACTION_DESCRIPTION"
 
 response = payment.trigger_stk_push(phone_number="+254700000000", amount=1)
 print(response.json())
+
+# use checkout_request_id from the above stk push as parameter for the function below
+stk_query = payment.query_stk_push(your_checkout_request_id)
+print(stk_query.json())
+
 ```
 
 ## Contribute
 
 Read the [CONTRIBUTING.md](https://github.com/raykipkorir/pydaraja/blob/main/CONTRIBUTING.md) file.
```

### Comparing `pydaraja-0.1.1/README.md` & `pydaraja-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pydaraja
 
 ## Description
-This is a python wrapper that handles payment requests through th Daraja Mpesa API.
+This is a python wrapper that handles payment requests through the Daraja Mpesa API.
 
 Daraja API services offered by pydaraja are:
 - Lipa na M-PESA online API also known as M-PESA express (STK Push/NI push)
 - STK push query API -> Used to check the status of Lipa na Mpesa online payment
 
 More services will come soon.
 
@@ -25,12 +25,17 @@
 payment.CALLBACK_URL = "YOUR_CALLBACK_URL"
 
 payment.ACCOUNT_REFERENCE = "YOUR_ACCOUNT_REFERENCE"
 payment.TRANSACTION_DESC = "YOUR_TRANSACTION_DESCRIPTION"
 
 response = payment.trigger_stk_push(phone_number="+254700000000", amount=1)
 print(response.json())
+
+# use checkout_request_id from the above stk push as parameter for the function below
+stk_query = payment.query_stk_push(your_checkout_request_id)
+print(stk_query.json())
+
 ```
 
 ## Contribute
 
 Read the [CONTRIBUTING.md](https://github.com/raykipkorir/pydaraja/blob/main/CONTRIBUTING.md) file.
```

### Comparing `pydaraja-0.1.1/pydaraja/payment.py` & `pydaraja-0.1.2/pydaraja/payment.py`

 * *Files identical despite different names*

### Comparing `pydaraja-0.1.1/pydaraja/utils.py` & `pydaraja-0.1.2/pydaraja/utils.py`

 * *Files identical despite different names*

### Comparing `pydaraja-0.1.1/pydaraja.egg-info/PKG-INFO` & `pydaraja-0.1.2/pydaraja.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pydaraja
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for Mpesa Daraja API
 Author-email: Raymond Kipkorir <raykipkorir02@gmail.com>
 Project-URL: Homepage, https://github.com/raykipkorir/pydaraja
 Project-URL: Bug Tracker, https://github.com/raykipkorir/pydaraja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydaraja
 
 ## Description
-This is a python wrapper that handles payment requests through th Daraja Mpesa API.
+This is a python wrapper that handles payment requests through the Daraja Mpesa API.
 
 Daraja API services offered by pydaraja are:
 - Lipa na M-PESA online API also known as M-PESA express (STK Push/NI push)
 - STK push query API -> Used to check the status of Lipa na Mpesa online payment
 
 More services will come soon.
 
@@ -39,12 +39,17 @@
 payment.CALLBACK_URL = "YOUR_CALLBACK_URL"
 
 payment.ACCOUNT_REFERENCE = "YOUR_ACCOUNT_REFERENCE"
 payment.TRANSACTION_DESC = "YOUR_TRANSACTION_DESCRIPTION"
 
 response = payment.trigger_stk_push(phone_number="+254700000000", amount=1)
 print(response.json())
+
+# use checkout_request_id from the above stk push as parameter for the function below
+stk_query = payment.query_stk_push(your_checkout_request_id)
+print(stk_query.json())
+
 ```
 
 ## Contribute
 
 Read the [CONTRIBUTING.md](https://github.com/raykipkorir/pydaraja/blob/main/CONTRIBUTING.md) file.
```

### Comparing `pydaraja-0.1.1/pyproject.toml` & `pydaraja-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydaraja"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Raymond Kipkorir", email="raykipkorir02@gmail.com" },
 ]
 description = "Python wrapper for Mpesa Daraja API"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

