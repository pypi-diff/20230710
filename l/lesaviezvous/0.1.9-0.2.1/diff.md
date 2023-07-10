# Comparing `tmp/lesaviezvous-0.1.9.tar.gz` & `tmp/lesaviezvous-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.1.9.tar", last modified: Mon Jul 10 17:44:34 2023, max compression
+gzip compressed data, was "lesaviezvous-0.2.1.tar", last modified: Mon Jul 10 17:52:38 2023, max compression
```

## Comparing `lesaviezvous-0.1.9.tar` & `lesaviezvous-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.9/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      501 2023-07-10 17:27:03.000000 lesaviezvous-0.1.9/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.9/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79461 2023-07-10 17:37:05.000000 lesaviezvous-0.1.9/lesaviezvous/db.py
--rw-r--r--   0 runner    (1000) runner    (1000)       97 2023-07-10 17:41:41.000000 lesaviezvous-0.1.9/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:44:34.000000 lesaviezvous-0.1.9/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:44:34.502527 lesaviezvous-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 17:44:31.000000 lesaviezvous-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:52:38.581602 lesaviezvous-0.2.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1304 2023-07-10 17:52:38.581602 lesaviezvous-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-07-10 17:52:10.000000 lesaviezvous-0.2.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:52:38.577602 lesaviezvous-0.2.1/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.2.1/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79461 2023-07-10 17:37:05.000000 lesaviezvous-0.2.1/lesaviezvous/db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      100 2023-07-10 17:50:14.000000 lesaviezvous-0.2.1/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:52:38.581602 lesaviezvous-0.2.1/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1304 2023-07-10 17:52:38.000000 lesaviezvous-0.2.1/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      258 2023-07-10 17:52:38.000000 lesaviezvous-0.2.1/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:52:38.000000 lesaviezvous-0.2.1/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:52:38.000000 lesaviezvous-0.2.1/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:52:38.581602 lesaviezvous-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 17:51:17.000000 lesaviezvous-0.2.1/setup.py
```

### Comparing `lesaviezvous-0.1.9/LICENSE` & `lesaviezvous-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.9/PKG-INFO` & `lesaviezvous-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.9
+Version: 0.2.1
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
@@ -16,18 +16,17 @@
 <p>Un package Python pour obtenir des informations intéressantes à partir de l'API Lesaviezvous.</p>
 <h2>Installation</h2>
 <p>Installez le package à l'aide de <code>pip</code> :</p>
 <pre lang="bash">pip<span class="w"> </span>install<span class="w"> </span>lesaviezvous
 </pre>
 <h2>Utilisation</h2>
 <p>Importez le package dans votre script Python et appelez la fonction infos() pour obtenir des informations intéressantes :</p>
-<pre lang="bash">import<span class="w"> </span>lesaviezvous
-from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>infos
+<pre lang="bash">from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>get_infos
 
-<span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>infos<span class="o">()</span>
+<span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>get_infos<span class="o">()</span>
 print<span class="o">(</span>fact<span class="o">)</span>
 </pre>
 <h2>Exigences</h2>
 <ul>
 <li>Python3</li>
 </ul>
 <h2>Quoi de neuf</h2>
```

### Comparing `lesaviezvous-0.1.9/lesaviezvous/db.py` & `lesaviezvous-0.2.1/lesaviezvous/db.py`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.9/lesaviezvous.egg-info/PKG-INFO` & `lesaviezvous-0.2.1/lesaviezvous.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.9
+Version: 0.2.1
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
@@ -16,18 +16,17 @@
 <p>Un package Python pour obtenir des informations intéressantes à partir de l'API Lesaviezvous.</p>
 <h2>Installation</h2>
 <p>Installez le package à l'aide de <code>pip</code> :</p>
 <pre lang="bash">pip<span class="w"> </span>install<span class="w"> </span>lesaviezvous
 </pre>
 <h2>Utilisation</h2>
 <p>Importez le package dans votre script Python et appelez la fonction infos() pour obtenir des informations intéressantes :</p>
-<pre lang="bash">import<span class="w"> </span>lesaviezvous
-from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>infos
+<pre lang="bash">from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>get_infos
 
-<span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>infos<span class="o">()</span>
+<span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>get_infos<span class="o">()</span>
 print<span class="o">(</span>fact<span class="o">)</span>
 </pre>
 <h2>Exigences</h2>
 <ul>
 <li>Python3</li>
 </ul>
 <h2>Quoi de neuf</h2>
```

### Comparing `lesaviezvous-0.1.9/pyproject.toml` & `lesaviezvous-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.9/setup.py` & `lesaviezvous-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name="lesaviezvous",
-    version="0.1.9",
+    version="0.2.1",
     author="Coding Team",
     author_email="codingteam@telegmail.com",
     license='MIT',
     description='Un package Python pour obtenir des informations intéressantes du monde.',
     long_description=render(long_description),
     long_description_content_type="text/markdown",
     url="https://github.com/codingtuto/lesaviezvouspkg/",
```

