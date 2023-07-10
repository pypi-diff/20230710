# Comparing `tmp/lesaviezvous-0.1.3.tar.gz` & `tmp/lesaviezvous-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.1.3.tar", last modified: Mon Jul 10 16:50:23 2023, max compression
+gzip compressed data, was "lesaviezvous-0.1.4.tar", last modified: Mon Jul 10 17:00:45 2023, max compression
```

## Comparing `lesaviezvous-0.1.3.tar` & `lesaviezvous-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1947 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      865 2023-07-10 07:15:22.000000 lesaviezvous-0.1.3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.3/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      243 2023-07-10 16:45:22.000000 lesaviezvous-0.1.3/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1947 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 16:50:23.000000 lesaviezvous-0.1.3/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      499 2023-07-10 16:44:12.000000 lesaviezvous-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 16:50:23.912023 lesaviezvous-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      815 2023-07-10 16:46:27.000000 lesaviezvous-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2997 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1103 2023-07-10 16:59:17.000000 lesaviezvous-0.1.4/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.4/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      243 2023-07-10 16:45:22.000000 lesaviezvous-0.1.4/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2997 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 17:00:44.000000 lesaviezvous-0.1.4/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      499 2023-07-10 16:44:12.000000 lesaviezvous-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 17:00:45.300675 lesaviezvous-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      777 2023-07-10 17:00:04.000000 lesaviezvous-0.1.4/setup.py
```

### Comparing `lesaviezvous-0.1.3/LICENSE` & `lesaviezvous-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lesaviezvous-0.1.3/PKG-INFO` & `lesaviezvous-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.3
+Version: 0.1.4
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1>Lesaviezvous</h1>
 <p>Un package Python pour obtenir des informations intéressantes à partir de l'API Lesaviezvous.</p>
@@ -22,15 +21,26 @@
 <h2>Utilisation</h2>
 <p>Importez le package dans votre script Python et appelez la fonction get_info() pour obtenir des informations intéressantes :</p>
 <pre lang="bash">import<span class="w"> </span>lesaviezvous
 from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>get_info
 
 <span class="nv">info</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>get_info<span class="o">()</span>
 <span class="k">if</span><span class="w"> </span>info:
-<span class="w">    </span>print<span class="o">(</span>info<span class="o">)</span>
+<span class="w">    </span><span class="nv">info_text</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>info<span class="o">[</span><span class="s1">&#39;infos&#39;</span><span class="o">]</span>
+<span class="w">    </span>print<span class="o">(</span>info_text<span class="o">)</span>
+<span class="k">else</span>:
+<span class="w">    </span>print<span class="o">(</span><span class="s2">&quot;Impossible de récupérer les informations.&quot;</span><span class="o">)</span>
+</pre>
+<p>ou</p>
+<pre lang="bash">import<span class="w"> </span>lesaviezvous
+
+<span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>lesaviezvous.get_info<span class="o">()</span>
+<span class="k">if</span><span class="w"> </span>fact<span class="w"> </span>is<span class="w"> </span>not<span class="w"> </span>None:
+<span class="w">    </span><span class="nv">fact_text</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>fact<span class="o">[</span><span class="s1">&#39;infos&#39;</span><span class="o">]</span>
+<span class="w">    </span>print<span class="o">(</span>fact_text<span class="o">)</span>
 <span class="k">else</span>:
 <span class="w">    </span>print<span class="o">(</span><span class="s2">&quot;Impossible de récupérer les informations.&quot;</span><span class="o">)</span>
 </pre>
 <h2>Exigences</h2>
 <ul>
 <li>Python3</li>
 <li>Request</li>
```

### Comparing `lesaviezvous-0.1.3/README.md` & `lesaviezvous-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,31 @@
 Importez le package dans votre script Python et appelez la fonction get_info() pour obtenir des informations intéressantes :
 ```bash
 import lesaviezvous
 from lesaviezvous import get_info
 
 info = get_info()
 if info:
-    print(info)
+    info_text = info['infos']
+    print(info_text)
 else:
     print("Impossible de récupérer les informations.")
 ```
+ou 
 
+```bash
+import lesaviezvous
+
+fact = lesaviezvous.get_info()
+if fact is not None:
+    fact_text = fact['infos']
+    print(fact_text)
+else:
+    print("Impossible de récupérer les informations.")
+```
 ## Exigences
 - Python3
 - Request
 
 ## Problème connu
 Il est possible de rencontrer un délai lors de l'affichage de la réponse du serveur. Cela peut être dû à divers facteurs, tels que la vitesse du réseau ou le temps de réponse de l'API Lesaviezvous. Veuillez prendre en compte cette possibilité lors de l'utilisation du package.
```

### Comparing `lesaviezvous-0.1.3/lesaviezvous.egg-info/PKG-INFO` & `lesaviezvous-0.1.4/lesaviezvous.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: lesaviezvous
-Version: 0.1.3
+Version: 0.1.4
 Summary: Un package Python pour obtenir des informations intéressantes du monde.
 Home-page: https://github.com/codingtuto/lesaviezvouspkg/
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1>Lesaviezvous</h1>
 <p>Un package Python pour obtenir des informations intéressantes à partir de l'API Lesaviezvous.</p>
@@ -22,15 +21,26 @@
 <h2>Utilisation</h2>
 <p>Importez le package dans votre script Python et appelez la fonction get_info() pour obtenir des informations intéressantes :</p>
 <pre lang="bash">import<span class="w"> </span>lesaviezvous
 from<span class="w"> </span>lesaviezvous<span class="w"> </span>import<span class="w"> </span>get_info
 
 <span class="nv">info</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>get_info<span class="o">()</span>
 <span class="k">if</span><span class="w"> </span>info:
-<span class="w">    </span>print<span class="o">(</span>info<span class="o">)</span>
+<span class="w">    </span><span class="nv">info_text</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>info<span class="o">[</span><span class="s1">&#39;infos&#39;</span><span class="o">]</span>
+<span class="w">    </span>print<span class="o">(</span>info_text<span class="o">)</span>
+<span class="k">else</span>:
+<span class="w">    </span>print<span class="o">(</span><span class="s2">&quot;Impossible de récupérer les informations.&quot;</span><span class="o">)</span>
+</pre>
+<p>ou</p>
+<pre lang="bash">import<span class="w"> </span>lesaviezvous
+
+<span class="nv">fact</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>lesaviezvous.get_info<span class="o">()</span>
+<span class="k">if</span><span class="w"> </span>fact<span class="w"> </span>is<span class="w"> </span>not<span class="w"> </span>None:
+<span class="w">    </span><span class="nv">fact_text</span><span class="w"> </span><span class="o">=</span><span class="w"> </span>fact<span class="o">[</span><span class="s1">&#39;infos&#39;</span><span class="o">]</span>
+<span class="w">    </span>print<span class="o">(</span>fact_text<span class="o">)</span>
 <span class="k">else</span>:
 <span class="w">    </span>print<span class="o">(</span><span class="s2">&quot;Impossible de récupérer les informations.&quot;</span><span class="o">)</span>
 </pre>
 <h2>Exigences</h2>
 <ul>
 <li>Python3</li>
 <li>Request</li>
```

### Comparing `lesaviezvous-0.1.3/setup.py` & `lesaviezvous-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 
 long_description = ""
 with open('README.md', encoding='utf-8') as file:
   long_description = file.read()
 
 setup(
   name = "lesaviezvous",
-  version = "0.1.3",
+  version = "0.1.4",
   author="Coding Team",
   author_email="codingteam@telegmail.com",
   license='MIT',
   description='Un package Python pour obtenir des informations intéressantes du monde.',
   long_description=render(long_description),
   long_description_content_type="text/markdown",
   url="https://github.com/codingtuto/lesaviezvouspkg/",
   packages=find_packages(exclude=["testing"]),
   install_requires=[
     'requests'
   ],
   python_requires='>=3.7',
   classifiers=[
     "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
     "Topic :: Utilities"
   ],
 )
```

