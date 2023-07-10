# Comparing `tmp/lesaviezvous-0.2.4.tar.gz` & `tmp/lesaviezvous-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.2.4.tar", last modified: Mon Jul 10 19:28:39 2023, max compression
+gzip compressed data, was "lesaviezvous-0.2.5.tar", last modified: Mon Jul 10 19:42:00 2023, max compression
```

## Comparing `lesaviezvous-0.2.4.tar` & `lesaviezvous-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:28:39.701962 lesaviezvous-0.2.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.2.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 19:28:39.701962 lesaviezvous-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      501 2023-07-10 19:27:33.000000 lesaviezvous-0.2.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:28:39.697962 lesaviezvous-0.2.4/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-10 19:26:59.000000 lesaviezvous-0.2.4/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79538 2023-07-10 19:25:06.000000 lesaviezvous-0.2.4/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:28:39.701962 lesaviezvous-0.2.4/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1339 2023-07-10 19:28:39.000000 lesaviezvous-0.2.4/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      239 2023-07-10 19:28:39.000000 lesaviezvous-0.2.4/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 19:28:39.000000 lesaviezvous-0.2.4/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 19:28:39.000000 lesaviezvous-0.2.4/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 19:28:39.701962 lesaviezvous-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 19:27:47.000000 lesaviezvous-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1539 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-07-10 19:41:27.000000 lesaviezvous-0.2.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-10 19:26:59.000000 lesaviezvous-0.2.5/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79538 2023-07-10 19:25:06.000000 lesaviezvous-0.2.5/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1539 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      239 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 19:42:00.000000 lesaviezvous-0.2.5/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 lesaviezvous-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 19:42:00.993203 lesaviezvous-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      769 2023-07-10 19:41:38.000000 lesaviezvous-0.2.5/setup.py
```

### Comparing `lesaviezvous-0.2.4/LICENSE` & `lesaviezvous-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.2.4/PKG-INFO` & `lesaviezvous-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.2.4
+Version: 0.2.5
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
@@ -17,18 +17,23 @@
 <h2>Installation</h2>
 <p>Installez le package à l'aide de <code>pip</code> :</p>
 <pre lang="bash">pip<span class="w"> </span>install<span class="w"> </span>lesaviezvous
 </pre>
 <h2>Utilisation</h2>
 <p>Importez le package dans votre script Python et appelez la fonction infos() pour obtenir des informations intéressantes :</p>
 <pre lang="bash">import<span class="w"> </span>lesaviezvous
-from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>faits
+from<span class="w"> </span>lesaviezvous.lesaviezvous<span class="w"> </span>import<span class="w"> </span>faits
 
 <span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>faits<span class="o">()</span>
 print<span class="o">(</span>fact<span class="o">)</span>
 </pre>
 <h2>Exigences</h2>
 <ul>
 <li>Python3</li>
 </ul>
 <h2>Quoi de neuf</h2>
-<p>Version plus rapide</p>
+<h3>Version 0.2.5:</h3>
+<ul>
+<li>Amélioration des performances pour une génération plus rapide des faits.</li>
+<li>Ajout de nouveaux faits à la base de données.</li>
+<li>Correction de bugs mineurs.</li>
+</ul>
```

### Comparing `lesaviezvous-0.2.4/lesaviezvous/lesaviezvous.py` & `lesaviezvous-0.2.5/lesaviezvous/lesaviezvous.py`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.2.4/lesaviezvous.egg-info/PKG-INFO` & `lesaviezvous-0.2.5/lesaviezvous.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.2.4
+Version: 0.2.5
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
@@ -17,18 +17,23 @@
 <h2>Installation</h2>
 <p>Installez le package à l'aide de <code>pip</code> :</p>
 <pre lang="bash">pip<span class="w"> </span>install<span class="w"> </span>lesaviezvous
 </pre>
 <h2>Utilisation</h2>
 <p>Importez le package dans votre script Python et appelez la fonction infos() pour obtenir des informations intéressantes :</p>
 <pre lang="bash">import<span class="w"> </span>lesaviezvous
-from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>faits
+from<span class="w"> </span>lesaviezvous.lesaviezvous<span class="w"> </span>import<span class="w"> </span>faits
 
 <span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>faits<span class="o">()</span>
 print<span class="o">(</span>fact<span class="o">)</span>
 </pre>
 <h2>Exigences</h2>
 <ul>
 <li>Python3</li>
 </ul>
 <h2>Quoi de neuf</h2>
-<p>Version plus rapide</p>
+<h3>Version 0.2.5:</h3>
+<ul>
+<li>Amélioration des performances pour une génération plus rapide des faits.</li>
+<li>Ajout de nouveaux faits à la base de données.</li>
+<li>Correction de bugs mineurs.</li>
+</ul>
```

### Comparing `lesaviezvous-0.2.4/pyproject.toml` & `lesaviezvous-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.2.4/setup.py` & `lesaviezvous-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name="lesaviezvous",
-    version="0.2.4",
+    version="0.2.5",
     author="Coding Team",
     author_email="codingteam@telegmail.com",
     license='MIT',
     description='Un package Python pour obtenir des informations intéressantes du monde.',
     long_description=render(long_description),
     long_description_content_type="text/markdown",
     url="https://github.com/codingtuto/lesaviezvouspkg/",
```

