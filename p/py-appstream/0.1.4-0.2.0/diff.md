# Comparing `tmp/py-appstream-0.1.4.tar.gz` & `tmp/py-appstream-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-appstream-0.1.4.tar", last modified: Fri Mar 25 14:57:46 2022, max compression
+gzip compressed data, last modified: Mon Jul 10 19:45:07 2023, from Unix
```

## Comparing `py-appstream-0.1.4.tar` & `py-appstream-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-25 14:57:46.812743 py-appstream-0.1.4/
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-25 14:57:46.805466 py-appstream-0.1.4/LICENSES/
--rwxrwxrwx   0 root         (0) root         (0)    18375 2021-03-31 15:07:53.000000 py-appstream-0.1.4/LICENSES/CC-BY-SA-4.0.txt
--rwxrwxrwx   0 root         (0) root         (0)     7048 2021-03-31 15:07:53.000000 py-appstream-0.1.4/LICENSES/CC0-1.0.txt
--rwxrwxrwx   0 root         (0) root         (0)    25967 2021-03-31 15:07:53.000000 py-appstream-0.1.4/LICENSES/LGPL-2.1-or-later.txt
--rwxrwxrwx   0 root         (0) root         (0)     1040 2022-03-25 14:57:46.812924 py-appstream-0.1.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      272 2022-03-11 21:29:06.000000 py-appstream-0.1.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-25 14:57:46.809038 py-appstream-0.1.4/py_appstream/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-03-11 06:26:48.000000 py-appstream-0.1.4/py_appstream/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6089 2022-03-19 16:37:52.000000 py-appstream-0.1.4/py_appstream/component.py
--rwxrwxrwx   0 root         (0) root         (0)      165 2022-03-11 15:49:44.000000 py-appstream-0.1.4/py_appstream/exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)     9366 2022-03-19 16:35:24.000000 py-appstream-0.1.4/py_appstream/subcomponent.py
--rwxrwxrwx   0 root         (0) root         (0)      623 2022-03-19 16:35:24.000000 py-appstream-0.1.4/py_appstream/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-03-25 14:57:46.812255 py-appstream-0.1.4/py_appstream.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1040 2022-03-25 14:57:46.000000 py-appstream-0.1.4/py_appstream.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      464 2022-03-25 14:57:46.000000 py-appstream-0.1.4/py_appstream.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-03-25 14:57:46.000000 py-appstream-0.1.4/py_appstream.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-03-11 18:03:59.000000 py-appstream-0.1.4/py_appstream.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       16 2022-03-25 14:57:46.000000 py-appstream-0.1.4/py_appstream.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2022-03-25 14:57:46.000000 py-appstream-0.1.4/py_appstream.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      212 2022-03-11 17:36:47.000000 py-appstream-0.1.4/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      910 2022-03-25 14:57:46.813621 py-appstream-0.1.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      146 2022-03-11 17:29:31.000000 py-appstream-0.1.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 19:43:15.000000 py-appstream-0.2.0/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 19:43:15.000000 py-appstream-0.2.0/LICENSES/
+-rwxrwxrwx   0 root         (0) root         (0)    18375 2021-03-31 15:07:53.000000 py-appstream-0.2.0/LICENSES/CC-BY-SA-4.0.txt
+-rwxrwxrwx   0 root         (0) root         (0)     7048 2021-03-31 15:07:53.000000 py-appstream-0.2.0/LICENSES/CC0-1.0.txt
+-rwxrwxrwx   0 root         (0) root         (0)    25967 2021-03-31 15:07:53.000000 py-appstream-0.2.0/LICENSES/LGPL-2.1-or-later.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1020 2023-07-10 19:43:15.000000 py-appstream-0.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      272 2022-03-11 21:29:06.000000 py-appstream-0.2.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-03-11 06:26:48.000000 py-appstream-0.2.0/py_appstream/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7048 2023-07-10 15:14:34.000000 py-appstream-0.2.0/py_appstream/component.py
+-rwxrwxrwx   0 root         (0) root         (0)      165 2022-03-11 15:49:44.000000 py-appstream-0.2.0/py_appstream/exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)     9366 2022-03-19 16:35:24.000000 py-appstream-0.2.0/py_appstream/subcomponent.py
+-rwxrwxrwx   0 root         (0) root         (0)      623 2022-03-19 16:35:24.000000 py-appstream-0.2.0/py_appstream/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1020 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2022-03-11 18:03:59.000000 py-appstream-0.2.0/py_appstream.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       16 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 19:43:15.000000 py-appstream-0.2.0/py_appstream.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      212 2022-03-11 17:36:47.000000 py-appstream-0.2.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      910 2023-07-10 19:43:15.000000 py-appstream-0.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      146 2022-03-11 17:29:31.000000 py-appstream-0.2.0/setup.py
```

### Comparing `py-appstream-0.1.4/LICENSES/CC-BY-SA-4.0.txt` & `py-appstream-0.2.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `py-appstream-0.1.4/LICENSES/CC0-1.0.txt` & `py-appstream-0.2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `py-appstream-0.1.4/LICENSES/LGPL-2.1-or-later.txt` & `py-appstream-0.2.0/LICENSES/LGPL-2.1-or-later.txt`

 * *Files identical despite different names*

### Comparing `py-appstream-0.1.4/PKG-INFO` & `py-appstream-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: py-appstream
-Version: 0.1.4
+Version: 0.2.0
 Summary: Pure Python library to parse AppStream files
 Home-page: https://github.com/phunh/py-appstream
 Author: Phu Hung Nguyen
 Author-email: phuhnguyen@outlook.com
 License: LGPLv2+
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
@@ -31,9 +30,7 @@
 (Partly) compliant with AppStream 0.15.
 
 ### Install
 
 ```bash
 pip install py-appstream
 ```
-
-
```

### Comparing `py-appstream-0.1.4/py_appstream/component.py` & `py-appstream-0.2.0/py_appstream/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,15 +117,30 @@
                     self.launchable[t] = []
                 if t == 'desktop-id':
                     val = val.replace('.desktop', '') if drop_desktop_id else val
                 self.launchable[t].append(val)
             elif c1.tag == 'custom':
                 for c2 in c1:
                     if c2.tag == 'value' and 'key' in c2.attrib:
-                        self.custom[c2.get('key')] = c2.text.strip()
+                        key = c2.get('key')
+                        lang = c2.get('{http://www.w3.org/XML/1998/namespace}lang', c2.attrib.get('lang'))
+                        if lang is None and (key not in self.custom or isinstance(self.custom[key], str)):
+                            # add as simple string
+                            self.custom[key] = c2.text.strip()
+                        else:
+                            # add as language-value dict
+                            values = self.custom.get(key)
+                            if values is None:
+                                values = {}
+                            elif isinstance(values, str):
+                                # convert existing string value to dict value
+                                clang = lang_code_func('C') if lang_code_func else 'C'
+                                values = {clang: values}
+                            utils.localize(values, c2, lang_code_func=lang_code_func)
+                            self.custom[key] = values
             elif c1.tag == 'pkgname':
                 self.pkgname = val
             elif c1.tag == 'keywords':
                 lang = c1.get('{http://www.w3.org/XML/1998/namespace}lang', c1.attrib.get('lang', 'C'))
                 kw = []
                 for c2 in c1:
                     if c2.tag == 'keyword':
```

### Comparing `py-appstream-0.1.4/py_appstream/subcomponent.py` & `py-appstream-0.2.0/py_appstream/subcomponent.py`

 * *Files identical despite different names*

### Comparing `py-appstream-0.1.4/py_appstream/utils.py` & `py-appstream-0.2.0/py_appstream/utils.py`

 * *Files identical despite different names*

### Comparing `py-appstream-0.1.4/py_appstream.egg-info/PKG-INFO` & `py-appstream-0.2.0/py_appstream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: py-appstream
-Version: 0.1.4
+Version: 0.2.0
 Summary: Pure Python library to parse AppStream files
 Home-page: https://github.com/phunh/py-appstream
 Author: Phu Hung Nguyen
 Author-email: phuhnguyen@outlook.com
 License: LGPLv2+
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
@@ -31,9 +30,7 @@
 (Partly) compliant with AppStream 0.15.
 
 ### Install
 
 ```bash
 pip install py-appstream
 ```
-
-
```

### Comparing `py-appstream-0.1.4/setup.cfg` & `py-appstream-0.2.0/setup.cfg`

 * *Files identical despite different names*

