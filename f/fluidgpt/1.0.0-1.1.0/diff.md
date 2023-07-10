# Comparing `tmp/fluidgpt-1.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/fluidgpt-1.1.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,14 @@
-Zip file size: 744831 bytes, number of entries: 17
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 14:09 fluidgpt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 14:09 fluidgpt-1.0.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 14:09 fluidgpt.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 14:09 fluidgpt/validation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-07 14:09 fluidgpt/fluidai_gpt_sdk/
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 14:09 fluidgpt/__init__.py
--rwxr-xr-x  2.0 unx   537024 b- defN 23-Jul-07 14:09 fluidgpt/validation/credentials_authentication.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   467648 b- defN 23-Jul-07 14:09 fluidgpt/validation/authentication.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      112 b- defN 23-Jul-07 14:09 fluidgpt/validation/__init__.py
--rwxr-xr-x  2.0 unx   261848 b- defN 23-Jul-07 14:09 fluidgpt/fluidai_gpt_sdk/endpoints.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    78424 b- defN 23-Jul-07 14:09 fluidgpt/fluidai_gpt_sdk/prompt_list.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   443312 b- defN 23-Jul-07 14:09 fluidgpt/fluidai_gpt_sdk/jupyter_helper.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-07 14:09 fluidgpt/fluidai_gpt_sdk/__init__.py
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-07 14:09 fluidgpt-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1204 b- defN 23-Jul-07 14:09 fluidgpt-1.0.0.dist-info/RECORD
--rw-r--r--  2.0 unx      148 b- defN 23-Jul-07 14:09 fluidgpt-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      718 b- defN 23-Jul-07 14:09 fluidgpt-1.0.0.dist-info/METADATA
-17 files, 1790552 bytes uncompressed, 742205 bytes compressed:  58.5%
+Zip file size: 145880 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-10 11:01 fluidgpt/__init__.py
+-rw-rw-rw-  2.0 fat      140 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/__init__.py
+-rw-rw-rw-  2.0 fat    55296 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/endpoints.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    89600 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/jupyter_helper.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    26624 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/prompt_list.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      113 b- defN 23-Jul-10 11:01 fluidgpt/validation/__init__.py
+-rw-rw-rw-  2.0 fat    68096 b- defN 23-Jul-10 11:01 fluidgpt/validation/authentication.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    80896 b- defN 23-Jul-10 11:01 fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      745 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1128 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/RECORD
+12 files, 322747 bytes uncompressed, 143940 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -1,52 +1,37 @@
-Filename: fluidgpt/
-Comment: 
-
-Filename: fluidgpt-1.0.0.dist-info/
-Comment: 
-
-Filename: fluidgpt.libs/
-Comment: 
-
-Filename: fluidgpt/validation/
-Comment: 
-
-Filename: fluidgpt/fluidai_gpt_sdk/
-Comment: 
-
 Filename: fluidgpt/__init__.py
 Comment: 
 
-Filename: fluidgpt/validation/credentials_authentication.cpython-39-x86_64-linux-gnu.so
+Filename: fluidgpt/fluidai_gpt_sdk/__init__.py
 Comment: 
 
-Filename: fluidgpt/validation/authentication.cpython-39-x86_64-linux-gnu.so
+Filename: fluidgpt/fluidai_gpt_sdk/endpoints.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fluidgpt/validation/__init__.py
+Filename: fluidgpt/fluidai_gpt_sdk/jupyter_helper.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fluidgpt/fluidai_gpt_sdk/endpoints.cpython-39-x86_64-linux-gnu.so
+Filename: fluidgpt/fluidai_gpt_sdk/prompt_list.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fluidgpt/fluidai_gpt_sdk/prompt_list.cpython-39-x86_64-linux-gnu.so
+Filename: fluidgpt/validation/__init__.py
 Comment: 
 
-Filename: fluidgpt/fluidai_gpt_sdk/jupyter_helper.cpython-39-x86_64-linux-gnu.so
+Filename: fluidgpt/validation/authentication.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fluidgpt/fluidai_gpt_sdk/__init__.py
+Filename: fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fluidgpt-1.0.0.dist-info/top_level.txt
+Filename: fluidgpt-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: fluidgpt-1.0.0.dist-info/RECORD
+Filename: fluidgpt-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: fluidgpt-1.0.0.dist-info/WHEEL
+Filename: fluidgpt-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fluidgpt-1.0.0.dist-info/METADATA
+Filename: fluidgpt-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## fluidgpt/validation/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-from .authentication import authenticate_secret
+from .authentication import authenticate_secret
 from .credentials_authentication import authenticate_credentials
```

## fluidgpt/fluidai_gpt_sdk/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .jupyter_helper import generate_code_completion, generate_code
+from .jupyter_helper import generate_code_completion, generate_code, generate_markdown, optimize_code
 from .endpoints import get_completion
```

## Comparing `fluidgpt-1.0.0.dist-info/METADATA` & `fluidgpt-1.1.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
-Name: fluidgpt
-Version: 1.0.0
-Summary: Run different validation tests on machine learning models.
-Home-page: https://github.com/
-Author: FluidAI
-Author-email: info@fluid.ai
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: Cython
-Requires-Dist: ipywidgets
-Requires-Dist: markdown
-Requires-Dist: mdutils
-Requires-Dist: jupyter
-Requires-Dist: ipython
-Requires-Dist: python-jose
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: fluidgpt
+Version: 1.1.0
+Summary: Run different validation tests on machine learning models.
+Home-page: https://github.com/
+Author: FluidAI
+Author-email: info@fluid.ai
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: openai
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: Cython
+Requires-Dist: ipywidgets
+Requires-Dist: markdown
+Requires-Dist: mdutils
+Requires-Dist: jupyter
+Requires-Dist: ipython
+Requires-Dist: python-jose
+
+UNKNOWN
+
```

