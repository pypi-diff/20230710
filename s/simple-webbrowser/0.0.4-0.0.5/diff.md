# Comparing `tmp/simple_webbrowser-0.0.4.tar.gz` & `tmp/simple_webbrowser-0.0.5.tar.gz`

## Comparing `simple_webbrowser-0.0.4.tar` & `simple_webbrowser-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/src/simple_webbrowser/__init__.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/src/simple_webbrowser/simple_webbrowser.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/archive/0-0-3/simple_webbrowser-0.0.3-py3-none-any.whl
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/archive/0-0-3/simple_webbrowser-0.0.3.tar.gz
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/archive/0-0-4/simple_webbrowser-0.0.4-py3-none-any.whl
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/archive/0-0-4/simple_webbrowser-0.0.4.tar.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/src/simple_webbrowser/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/src/simple_webbrowser/simple_webbrowser.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/LICENSE
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/README.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 simple_webbrowser-0.0.5/PKG-INFO
```

### Comparing `simple_webbrowser-0.0.4/src/simple_webbrowser/simple_webbrowser.py` & `simple_webbrowser-0.0.5/src/simple_webbrowser/simple_webbrowser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import webbrowser
 from sys import platform
 
 # simple_webbrowser.py by MF366
 # Based on built-in module: webbrowser
 # Also uses the platform variable from sys module
 
-def Website(url):
+def Website(url, new: int = 0):
     if platform == "win32":
-        webbrowser.open(url)
+        webbrowser.open(url, new=new)
         # trust me: this part is not a total waste
     elif platform == "linux" or "darwin":
-        webbrowser.open(url)
+        webbrowser.open(url, new=new)
         
 def Google(query):
     query = str(query)
     for i in query:
         typed = query.replace(' ', '+')
     webbrowser.open('https://www.google.com/search?q='+typed)
 
@@ -78,8 +78,22 @@
         typed = query.replace(' ', '+')
     webbrowser.open("https://www.qwant.com/?q="+typed)
                 
 def SpotifyOnline(query):
     query = str(query)
     for i in query:
         typed = query.replace(' ', '%20')
-    webbrowser.open("https://open.spotify.com/search/"+typed)
+    webbrowser.open("https://open.spotify.com/search/"+typed)
+    
+def GitLab(query):
+    # requires a GitLab account
+    query = str(query)
+    for i in query:
+        typed = query.replace(' ', '%20')
+    webbrowser.open("https://gitlab.com/search?search="+typed)
+    
+def GitHub(query):
+    # requires a GitHub account
+    query = str(query)
+    for i in query:
+        typed = query.replace(' ', '+')
+    webbrowser.open("https://github.com/search?q="+typed)
```

### Comparing `simple_webbrowser-0.0.4/LICENSE` & `simple_webbrowser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_webbrowser-0.0.4/pyproject.toml` & `simple_webbrowser-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple_webbrowser"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="MF366", email="real_mf366@yahoo.com" },
 ]
 description = "A better webbrowser. Just. For. You."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_webbrowser-0.0.4/PKG-INFO` & `simple_webbrowser-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_webbrowser
-Version: 0.0.4
+Version: 0.0.5
 Summary: A better webbrowser. Just. For. You.
 Project-URL: Homepage, https://github.com/MF366-Coding/simple_webbrowser
 Project-URL: Bug Tracker, https://github.com/MF366-Coding/simple_webbrowser/issues
 Author-email: MF366 <real_mf366@yahoo.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,23 +14,30 @@
 
 # simple_webbrowser
 `simple_webbrowser` is a module that makes `webbrowser` module way more simple to work with.
 
 # License
 This module is licensed under the MIT License.
 
-# PyPI
-This module is also available on PyPI.
-
 # How to install?
 Use the following command on the commandline:
 ```
 pip install simple_webbrowser
 ```
 
+Or, for Windows (if Python is on ``PATH``, but ``pip`` isn't):
+```
+python -m pip install simple_webbrowser
+```
+
 # How to use?
 Import it like this:
 ```
 from simple_webbrowser import simple_webbrowser
 
 # Afterwards, just use it :)
 ```
+
+# Projects where this module is used... (GitHub)
+Search query: [simple_webbrowser language:Python](https://github.com/search?q=simple_webbrowser+language%3APython&type=code)
+
+Filters: code
```

