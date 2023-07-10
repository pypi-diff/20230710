# Comparing `tmp/python_redex-1.0.0.tar.gz` & `tmp/python_redex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_redex-1.0.0.tar", last modified: Fri Jul  7 18:33:51 2023, max compression
+gzip compressed data, was "python_redex-1.0.1.tar", last modified: Mon Jul 10 14:31:15 2023, max compression
```

## Comparing `python_redex-1.0.0.tar` & `python_redex-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 18:33:51.398366 python_redex-1.0.0/
--rw-rw-rw-   0        0        0      805 2023-07-07 18:32:07.000000 python_redex-1.0.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-1.0.0/LICENCE.txt
--rw-rw-rw-   0        0        0       27 2023-07-02 16:36:53.000000 python_redex-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      571 2023-07-07 18:33:51.398366 python_redex-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-1.0.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 18:33:51.319332 python_redex-1.0.0/python_redex.egg-info/
--rw-rw-rw-   0        0        0      571 2023-07-07 18:33:51.000000 python_redex-1.0.0/python_redex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-07-07 18:33:51.000000 python_redex-1.0.0/python_redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 18:33:51.000000 python_redex-1.0.0/python_redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 18:33:51.000000 python_redex-1.0.0/python_redex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 18:33:51.390952 python_redex-1.0.0/redex/
--rw-rw-rw-   0        0        0     1775 2023-07-07 18:31:43.000000 python_redex-1.0.0/redex/__init__.py
--rw-rw-rw-   0        0        0     2705 2023-07-07 18:24:48.000000 python_redex-1.0.0/redex/action.py
--rw-rw-rw-   0        0        0     2207 2023-07-07 17:46:49.000000 python_redex-1.0.0/redex/lexical_analysis.py
--rw-rw-rw-   0        0        0      581 2023-07-02 15:01:38.000000 python_redex-1.0.0/redex/split.py
--rw-rw-rw-   0        0        0      559 2023-07-02 15:02:16.000000 python_redex-1.0.0/redex/wildcards.py
-drwxrwxrwx   0        0        0        0 2023-07-07 18:33:51.398366 python_redex-1.0.0/redex.egg-info/
--rw-rw-rw-   0        0        0      177 2023-07-02 15:53:02.000000 python_redex-1.0.0/redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:53:02.000000 python_redex-1.0.0/redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 15:53:02.000000 python_redex-1.0.0/redex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 18:33:51.398366 python_redex-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      723 2023-07-07 18:32:32.000000 python_redex-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:31:15.241661 python_redex-1.0.1/
+-rw-rw-rw-   0        0        0      805 2023-07-07 18:32:07.000000 python_redex-1.0.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-1.0.1/LICENCE.txt
+-rw-rw-rw-   0        0        0       27 2023-07-02 16:36:53.000000 python_redex-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      571 2023-07-10 14:31:15.241661 python_redex-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-1.0.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 14:31:15.220774 python_redex-1.0.1/python_redex.egg-info/
+-rw-rw-rw-   0        0        0      571 2023-07-10 14:31:15.000000 python_redex-1.0.1/python_redex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-07-10 14:31:15.000000 python_redex-1.0.1/python_redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:31:15.000000 python_redex-1.0.1/python_redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 14:31:15.000000 python_redex-1.0.1/python_redex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 14:31:15.225333 python_redex-1.0.1/redex/
+-rw-rw-rw-   0        0        0     1775 2023-07-10 14:30:03.000000 python_redex-1.0.1/redex/__init__.py
+-rw-rw-rw-   0        0        0     2914 2023-07-10 14:28:42.000000 python_redex-1.0.1/redex/action.py
+-rw-rw-rw-   0        0        0     2206 2023-07-10 14:14:14.000000 python_redex-1.0.1/redex/lexical_analysis.py
+-rw-rw-rw-   0        0        0      581 2023-07-02 15:01:38.000000 python_redex-1.0.1/redex/split.py
+-rw-rw-rw-   0        0        0      559 2023-07-02 15:02:16.000000 python_redex-1.0.1/redex/wildcards.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:31:15.240458 python_redex-1.0.1/redex.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-07-02 15:53:02.000000 python_redex-1.0.1/redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:53:02.000000 python_redex-1.0.1/redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 15:53:02.000000 python_redex-1.0.1/redex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:31:15.243024 python_redex-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      723 2023-07-10 14:29:35.000000 python_redex-1.0.1/setup.py
+-rw-rw-rw-   0        0        0     1085 2023-07-10 14:28:57.000000 python_redex-1.0.1/test.py
```

### Comparing `python_redex-1.0.0/CHANGELOG.txt` & `python_redex-1.0.1/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `python_redex-1.0.0/LICENCE.txt` & `python_redex-1.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `python_redex-1.0.0/PKG-INFO` & `python_redex-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_redex
-Version: 1.0.0
+Version: 1.0.1
 Summary: User friendly version of regex.
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-1.0.0/python_redex.egg-info/PKG-INFO` & `python_redex-1.0.1/python_redex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redex
-Version: 1.0.0
+Version: 1.0.1
 Summary: User friendly version of regex.
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-1.0.0/redex/__init__.py` & `python_redex-1.0.1/redex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
         if substring:
             count += 1
     return count
 
 def info():
     print('\n')
     print('  ;,//;,    ,;/      Description:        Python library for readable regex.')
-    print(' o:::::::;;///       Version:            1.0.0')
+    print(' o:::::::;;///       Version:            1.0.1')
     print('>::::::::;;\\\\\\       Author:             Timo Kats')
-    print('  "\\\\\\\\\\""  \';\      Last updated:       06/07/2023', end='\n\n\n')
+    print('  "\\\\\\\\\\""  \';\      Last updated:       10/07/2023', end='\n\n\n')
```

### Comparing `python_redex-1.0.0/redex/action.py` & `python_redex-1.0.1/redex/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,44 @@
 from redex.wildcards import *
 
 # helper functions
 
 def is_in(char, string) -> bool:
     if char in wildcard.keys():
         for wchar in wildcard[char]:
-            if wchar == string[0]:
+            if wchar in string:
                 return True
     else:
         return char in string
     
-def is_in_endswith(char, string) -> bool:
+def is_in_end(char, string) -> bool:
     if char in wildcard.keys():
         for wchar in wildcard[char]:
             if wchar == string[-1]:
                 return True
     else:
-        return char in string
+        return char == string
+
+def is_in_start(char, string) -> bool:
+    if char in wildcard.keys():
+        for wchar in wildcard[char]:
+            if wchar == string[0]:
+                return True
+    else:
+        return char == string
 
 # actions
 
 def startswith(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
-    return is_in(sub_query, string[:len(sub_query)])
+    return is_in_start(sub_query, string[:len(sub_query)])
 
 def endswith(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
-    return is_in_endswith(sub_query, string[-len(sub_query):])
+    return is_in_end(sub_query, string[-len(sub_query):])
 
 def contains(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
     return is_in(sub_query, string)
 
 def count(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
@@ -73,13 +81,13 @@
         if not is_in(sequence_list[current_index], string):
             return False
     return current_index == len(sequence_list) - 1
 
 def location(sub_query, string) -> bool:
     sub_query = sub_query.split(':')[1]
     char = list(sub_query[1:-1].split(','))[0]
-    location = int(list(sub_query[1:-1].split(','))[1])
+    location = int(list(sub_query[1:-1].split(','))[1])    
     if location < len(string) - 1:
         return is_in(char, string[location])
     else:
         return False
```

### Comparing `python_redex-1.0.0/redex/lexical_analysis.py` & `python_redex-1.0.1/redex/lexical_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
         final_result = []
         for result in self.results:
             copy_query = self.query
             for sub_result in result:
                 copy_query = copy_query.replace(sub_result[0], str(sub_result[1]))
             final_result.append(eval(copy_query))
         return final_result
-
```

### Comparing `python_redex-1.0.0/redex/split.py` & `python_redex-1.0.1/redex/split.py`

 * *Files identical despite different names*

### Comparing `python_redex-1.0.0/redex/wildcards.py` & `python_redex-1.0.1/redex/wildcards.py`

 * *Files identical despite different names*

### Comparing `python_redex-1.0.0/setup.py` & `python_redex-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='python_redex',
-    version='1.0.0',
+    version='1.0.1',
     description='User friendly version of regex.',
     long_description='More information available at https://github.com/TimoKats/redex',
     url='',  
     author='Timo Kats',
     author_email='tpakats@gmail.com',
     license='MIT', 
     classifiers=classifiers,
```

