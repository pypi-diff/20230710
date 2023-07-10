# Comparing `tmp/multikeyiterdict-0.11.tar.gz` & `tmp/multikeyiterdict-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multikeyiterdict-0.11.tar", last modified: Thu Jul  6 18:37:14 2023, max compression
+gzip compressed data, was "multikeyiterdict-0.12.tar", last modified: Mon Jul 10 20:33:50 2023, max compression
```

## Comparing `multikeyiterdict-0.11.tar` & `multikeyiterdict-0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:37:14.248327 multikeyiterdict-0.11/
--rw-rw-rw-   0        0        0     1148 2023-07-06 18:37:05.000000 multikeyiterdict-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      119 2023-07-06 18:37:03.000000 multikeyiterdict-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     6958 2023-07-06 18:37:14.248327 multikeyiterdict-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     6192 2023-07-06 18:18:09.000000 multikeyiterdict-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 18:37:14.243340 multikeyiterdict-0.11/multikeyiterdict/
--rw-rw-rw-   0        0        0     6192 2023-07-06 18:18:09.000000 multikeyiterdict-0.11/multikeyiterdict/README.MD
--rw-rw-rw-   0        0        0     3910 2023-07-06 18:36:13.000000 multikeyiterdict-0.11/multikeyiterdict/__init__.py
--rw-rw-rw-   0        0        0       87 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/multikeyiterdict/requirements.txt
--rw-rw-rw-   0        0        0     5030 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/multikeyiterdict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-06 18:37:14.247329 multikeyiterdict-0.11/multikeyiterdict.egg-info/
--rw-rw-rw-   0        0        0     6958 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/multikeyiterdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-06 18:37:14.000000 multikeyiterdict-0.11/multikeyiterdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/multikeyiterdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/multikeyiterdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/multikeyiterdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-06 18:37:14.249324 multikeyiterdict-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1589 2023-07-06 18:37:13.000000 multikeyiterdict-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 20:33:50.950173 multikeyiterdict-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-07-10 20:33:43.000000 multikeyiterdict-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      119 2023-07-10 20:33:42.000000 multikeyiterdict-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     6958 2023-07-10 20:33:50.950173 multikeyiterdict-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     6192 2023-07-06 18:38:08.000000 multikeyiterdict-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 20:33:50.947180 multikeyiterdict-0.12/multikeyiterdict/
+-rw-rw-rw-   0        0        0     6192 2023-07-06 18:38:08.000000 multikeyiterdict-0.12/multikeyiterdict/README.MD
+-rw-rw-rw-   0        0        0     3836 2023-07-10 20:28:56.000000 multikeyiterdict-0.12/multikeyiterdict/__init__.py
+-rw-rw-rw-   0        0        0       87 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict/requirements.txt
+-rw-rw-rw-   0        0        0     5030 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-10 20:33:50.950173 multikeyiterdict-0.12/multikeyiterdict.egg-info/
+-rw-rw-rw-   0        0        0     6958 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/multikeyiterdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-10 20:33:50.951171 multikeyiterdict-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1589 2023-07-10 20:33:50.000000 multikeyiterdict-0.12/setup.py
```

### Comparing `multikeyiterdict-0.11/LICENSE.rst` & `multikeyiterdict-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `multikeyiterdict-0.11/PKG-INFO` & `multikeyiterdict-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multikeyiterdict
-Version: 0.11
+Version: 0.12
 Summary: MultiKeyIterDict enhances the capabilities of the standard dictionary by supporting multiple keys, nested searches, and operations such as updates and merges (without loosing data) on dicts
 Home-page: https://github.com/hansalemaos/multikeyiterdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested
 Classifier: Development Status :: 4 - Beta
```

### Comparing `multikeyiterdict-0.11/README.md` & `multikeyiterdict-0.12/README.md`

 * *Files identical despite different names*

### Comparing `multikeyiterdict-0.11/multikeyiterdict/README.MD` & `multikeyiterdict-0.12/multikeyiterdict/README.MD`

 * *Files identical despite different names*

### Comparing `multikeyiterdict-0.11/multikeyiterdict/__init__.py` & `multikeyiterdict-0.12/multikeyiterdict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from itertools import takewhile
 
 from dict_merger_keep_all import dict_merger
 from flatten_any_dict_iterable_or_whatsoever import fla_tu
 from mymulti_key_dict import (
     MultiKeyDict,
     convert_to_normal_dict_simple,
-    convert_to_default_dict,
 )
 from isiter import isiter
 
 
 class MultiKeyIterDict(MultiKeyDict):
     """A dictionary implementation that supports multiple keys for nested lookups."""
 
@@ -27,47 +26,47 @@
     def nested_items(self):
         """
         Generate nested items in the dictionary.
 
         Yields:
             Tuple: A tuple containing the nested key and value.
         """
-        for v, k in fla_tu(self.data):
+        for v, k in fla_tu(self):
             yield list(k), v
 
     def nested_values(self):
         """
         Generate nested values in the dictionary.
 
         Yields:
             Any: The nested value.
         """
-        for v, k in fla_tu(self.data):
+        for v, k in fla_tu(self):
             yield v
 
     def nested_keys(self):
         """
         Generate nested keys in the dictionary.
 
         Yields:
             List: The nested key.
         """
-        for v, k in fla_tu(self.data):
+        for v, k in fla_tu(self):
             yield list(k)
 
     def _check_last_item(self):
         """
         Check the last item in the nested dictionary.
 
         Yields:
             Tuple: A tuple containing the key and value of the last item.
         """
         alreadydone = []
         results = []
-        for v, k in fla_tu(self.data):
+        for v, k in fla_tu(self):
             if len(k) > 1 and k not in alreadydone:
                 qr = list(k)[:-1]
                 if isinstance(v2 := self[qr], (dict, collections.defaultdict)):
                     results.append((list(k), v))
 
                 elif isiter(v2):
                     alreadydone.append(qr)
@@ -114,15 +113,15 @@
 
         Args:
             *args: One or more dictionaries to update the current dictionary.
 
         Note:
             This method modifies the current dictionary in-place.
         """
-        self.data = convert_to_default_dict(dict_merger(self.to_dict(), *args))
+        self.update(dict_merger(self.to_dict(), *args))
 
     def nested_merge(self, *args):
         """
         Merge the dictionary with nested key-value pairs.
 
         Args:
             *args: One or more dictionaries to merge with the current dictionary.
```

### Comparing `multikeyiterdict-0.11/multikeyiterdict/thirdparty.json` & `multikeyiterdict-0.12/multikeyiterdict/thirdparty.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {'3': "{'Version': '0.13'}"}*

```diff
@@ -17,10 +17,10 @@
         "Name": "isiter",
         "Version": "0.10"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "mymulti-key-dict",
-        "Version": "0.11"
+        "Version": "0.13"
     }
 ]
```

### Comparing `multikeyiterdict-0.11/multikeyiterdict.egg-info/PKG-INFO` & `multikeyiterdict-0.12/multikeyiterdict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multikeyiterdict
-Version: 0.11
+Version: 0.12
 Summary: MultiKeyIterDict enhances the capabilities of the standard dictionary by supporting multiple keys, nested searches, and operations such as updates and merges (without loosing data) on dicts
 Home-page: https://github.com/hansalemaos/multikeyiterdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: nested
 Classifier: Development Status :: 4 - Beta
```

### Comparing `multikeyiterdict-0.11/setup.py` & `multikeyiterdict-0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''MultiKeyIterDict enhances the capabilities of the standard dictionary by supporting multiple keys, nested searches, and operations such as updates and merges (without loosing data) on dicts'''
 
 # Setting up
 setup(
     name="multikeyiterdict",
     version=VERSION,
     license='MIT',
```

