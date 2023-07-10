# Comparing `tmp/tone-0.0.4.tar.gz` & `tmp/tone-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tone-0.0.4.tar", last modified: Fri Apr 30 07:00:43 2021, max compression
+gzip compressed data, was "tone-0.0.5.tar", last modified: Mon Jul 10 20:41:48 2023, max compression
```

## Comparing `tone-0.0.4.tar` & `tone-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2021-04-30 07:00:43.890259 tone-0.0.4/
--rw-r--r--   0 steven    (1000) root         (0)       38 2021-04-30 06:38:11.000000 tone-0.0.4/MANIFEST.in
--rw-r--r--   0 steven    (1000) root         (0)      556 2021-04-30 07:00:43.890259 tone-0.0.4/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)      105 2021-04-30 07:00:13.000000 tone-0.0.4/README
--rw-r--r--   0 steven    (1000) root         (0)       38 2021-04-30 07:00:43.890259 tone-0.0.4/setup.cfg
--rw-r--r--   0 steven    (1000) root         (0)     1257 2021-04-30 07:00:13.000000 tone-0.0.4/setup.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2021-04-30 07:00:43.886925 tone-0.0.4/tone/
--rw-r--r--   0 steven    (1000) root         (0)       90 2021-04-30 07:00:25.000000 tone-0.0.4/tone/__init__.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2021-04-30 07:00:43.890259 tone-0.0.4/tone/utils/
--rw-r--r--   0 steven    (1000) root         (0)       90 2021-04-30 06:38:11.000000 tone-0.0.4/tone/utils/__init__.py
--rw-r--r--   0 steven    (1000) root         (0)     1564 2021-04-30 06:38:11.000000 tone-0.0.4/tone/utils/attrdict.py
--rw-r--r--   0 steven    (1000) root         (0)     1073 2021-04-30 06:38:11.000000 tone-0.0.4/tone/utils/logger.py
-drwxr-xr-x   0 steven    (1000) root         (0)        0 2021-04-30 07:00:43.890259 tone-0.0.4/tone.egg-info/
--rw-r--r--   0 steven    (1000) root         (0)      556 2021-04-30 07:00:43.000000 tone-0.0.4/tone.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) root         (0)      246 2021-04-30 07:00:43.000000 tone-0.0.4/tone.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2021-04-30 07:00:43.000000 tone-0.0.4/tone.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) root         (0)        5 2021-04-30 07:00:43.000000 tone-0.0.4/tone.egg-info/top_level.txt
--rw-r--r--   0 steven    (1000) root         (0)        1 2021-04-30 07:00:43.000000 tone-0.0.4/tone.egg-info/zip-safe
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/
+-rw-r--r--   0 steven    (1000) root         (0)     1063 2023-07-10 20:38:25.000000 tone-0.0.5/LICENSE
+-rw-r--r--   0 steven    (1000) root         (0)       36 2023-07-10 20:38:25.000000 tone-0.0.5/MANIFEST.in
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 20:41:48.548729 tone-0.0.5/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)       98 2023-07-10 20:38:25.000000 tone-0.0.5/README
+-rw-r--r--   0 steven    (1000) root         (0)       38 2023-07-10 20:41:48.548729 tone-0.0.5/setup.cfg
+-rw-r--r--   0 steven    (1000) root         (0)     1209 2023-07-10 20:38:25.000000 tone-0.0.5/setup.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tests/
+-rw-r--r--   0 steven    (1000) root         (0)      421 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_all.py
+-rw-r--r--   0 steven    (1000) root         (0)      402 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_base.py
+-rw-r--r--   0 steven    (1000) root         (0)      266 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_tone.py
+-rw-r--r--   0 steven    (1000) root         (0)     3904 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_utils_attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      554 2023-07-10 20:38:25.000000 tone-0.0.5/tests/test_utils_logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tone/
+-rw-r--r--   0 steven    (1000) root         (0)       84 2023-07-10 20:40:01.000000 tone-0.0.5/tone/__init__.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tone/utils/
+-rw-r--r--   0 steven    (1000) root         (0)      108 2023-07-10 20:41:10.000000 tone-0.0.5/tone/utils/__init__.py
+-rw-r--r--   0 steven    (1000) root         (0)     1502 2023-07-10 20:38:25.000000 tone-0.0.5/tone/utils/attrdict.py
+-rw-r--r--   0 steven    (1000) root         (0)      618 2023-07-10 20:40:50.000000 tone-0.0.5/tone/utils/ipython.py
+-rw-r--r--   0 steven    (1000) root         (0)     1029 2023-07-10 20:38:25.000000 tone-0.0.5/tone/utils/logger.py
+drwxr-xr-x   0 steven    (1000) root         (0)        0 2023-07-10 20:41:48.548729 tone-0.0.5/tone.egg-info/
+-rw-r--r--   0 steven    (1000) root         (0)      510 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/PKG-INFO
+-rw-r--r--   0 steven    (1000) root         (0)      388 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/SOURCES.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/dependency_links.txt
+-rw-r--r--   0 steven    (1000) root         (0)        5 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/top_level.txt
+-rw-r--r--   0 steven    (1000) root         (0)        1 2023-07-10 20:41:48.000000 tone-0.0.5/tone.egg-info/zip-safe
```

### Comparing `tone-0.0.4/setup.py` & `tone-0.0.5/setup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# from __future__ import absolute_import
-import os
-import sys
-from setuptools import setup
-
-NAME = "tone"
-INSTALL_REQUIRES = [
-]
-
-dirname = os.path.dirname(os.path.abspath(__file__))
-if dirname not in sys.path:
-    sys.path.insert(0, dirname)
-try:
-    import tone
-    version = tone.__version__
-except Exception:
-    print("import project error")
-    exit(-1)
-
-readme = os.path.join(dirname, "README")
-
-setup(
-    name=NAME,
-    version=tone.__version__,
-    description="Deal with tone",
-    long_description=open(readme).read(),
-    packages=[NAME],
-    install_requires=INSTALL_REQUIRES,
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3',
-    ],
-    author="StevenKang",
-    author_email="kangweibaby@163.com",
-    url="https://github.com/StevenBaby/tone",
-    license="MIT",
-    include_package_data=True,
-    zip_safe=True,
-    platforms="any",
-)
-
-
-# python setup.py sdist bdist_wheel --universal
-# twine upload dist/*
-# pip2 install dandan --upgrade -i https://pypi.python.org/simple
-# pip3 install dandan --upgrade -i https://pypi.python.org/simple
+# from __future__ import absolute_import
+import os
+import sys
+from setuptools import setup
+
+NAME = "tone"
+INSTALL_REQUIRES = [
+]
+
+dirname = os.path.dirname(os.path.abspath(__file__))
+if dirname not in sys.path:
+    sys.path.insert(0, dirname)
+try:
+    import tone
+    version = tone.__version__
+except Exception:
+    print("import project error")
+    exit(-1)
+
+readme = os.path.join(dirname, "README")
+
+setup(
+    name=NAME,
+    version=tone.__version__,
+    description="Deal with tone",
+    long_description=open(readme).read(),
+    packages=[NAME],
+    install_requires=INSTALL_REQUIRES,
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Intended Audience :: Developers',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3',
+    ],
+    author="StevenKang",
+    author_email="kangweibaby@163.com",
+    url="https://github.com/StevenBaby/tone",
+    license="MIT",
+    include_package_data=True,
+    zip_safe=True,
+    platforms="any",
+)
+
+
+# python setup.py sdist bdist_wheel --universal
+# twine upload dist/*
+# pip2 install dandan --upgrade -i https://pypi.python.org/simple
+# pip3 install dandan --upgrade -i https://pypi.python.org/simple
```

### Comparing `tone-0.0.4/tone/utils/attrdict.py` & `tone-0.0.5/tone/utils/attrdict.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# coding=utf-8
-
-
-class attrdict(dict):
-
-    '''
-    Use dict key as attribute if available
-    '''
-
-    def __init__(self, *args, **kwargs):
-        super(attrdict, self).__init__(*args, **kwargs)
-        self.__dict__ = self
-
-    def __getattr__(self, key):
-        try:
-            return self[key]
-        except KeyError as e:
-            raise AttributeError(e)
-
-    @classmethod
-    def loads(cls, value):
-        if type(value) is dict:
-            result = cls()
-            result.update(value)
-            for k, v in result.items():
-                result[k] = cls.loads(v)
-
-        elif type(value) is list:
-            for index, item in enumerate(value):
-                if type(item) in (list, dict):
-                    value[index] = cls.loads(item)
-            result = value
-        else:
-            result = value
-        return result
-
-    @classmethod
-    def json_loads(cls, value):
-        import json
-        data = json.loads(value)
-        return cls.loads(data)
-
-
-class defaultattrdict(attrdict):
-
-    '''
-    like attrdict but if key not exists, then create a empty defaultattrdict.
-    '''
-
-    def __getattr__(self, key):
-        try:
-            return super(defaultattrdict, self).__getattr__(key)
-        except AttributeError:
-            self[key] = defaultattrdict()
-            return self[key]
-
-    def get(self, key):
-        try:
-            return self[key]
-        except KeyError as e:
-            self[key] = defaultattrdict()
-            return self[key]
+# coding=utf-8
+
+
+class attrdict(dict):
+
+    '''
+    Use dict key as attribute if available
+    '''
+
+    def __init__(self, *args, **kwargs):
+        super(attrdict, self).__init__(*args, **kwargs)
+        self.__dict__ = self
+
+    def __getattr__(self, key):
+        try:
+            return self[key]
+        except KeyError as e:
+            raise AttributeError(e)
+
+    @classmethod
+    def loads(cls, value):
+        if type(value) is dict:
+            result = cls()
+            result.update(value)
+            for k, v in result.items():
+                result[k] = cls.loads(v)
+
+        elif type(value) is list:
+            for index, item in enumerate(value):
+                if type(item) in (list, dict):
+                    value[index] = cls.loads(item)
+            result = value
+        else:
+            result = value
+        return result
+
+    @classmethod
+    def json_loads(cls, value):
+        import json
+        data = json.loads(value)
+        return cls.loads(data)
+
+
+class defaultattrdict(attrdict):
+
+    '''
+    like attrdict but if key not exists, then create a empty defaultattrdict.
+    '''
+
+    def __getattr__(self, key):
+        try:
+            return super(defaultattrdict, self).__getattr__(key)
+        except AttributeError:
+            self[key] = defaultattrdict()
+            return self[key]
+
+    def get(self, key):
+        try:
+            return self[key]
+        except KeyError as e:
+            self[key] = defaultattrdict()
+            return self[key]
```

