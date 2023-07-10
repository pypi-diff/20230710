# Comparing `tmp/atlantiscore-2.2.0.tar.gz` & `tmp/atlantiscore-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantiscore-2.2.0.tar", last modified: Thu Jun 29 15:13:06 2023, max compression
+gzip compressed data, was "atlantiscore-2.3.0.tar", last modified: Mon Jul 10 16:19:23 2023, max compression
```

## Comparing `atlantiscore-2.2.0.tar` & `atlantiscore-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.988612 atlantiscore-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-29 15:13:06.988612 atlantiscore-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.980612 atlantiscore-2.2.0/atlantiscore/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.980612 atlantiscore-2.2.0/atlantiscore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.984612 atlantiscore-2.2.0/atlantiscore/db/types/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/db/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/db/types/evm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.984612 atlantiscore-2.2.0/atlantiscore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/lib/eth.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.984612 atlantiscore-2.2.0/atlantiscore/types/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/types/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/atlantiscore/types/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.980612 atlantiscore-2.2.0/atlantiscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-29 15:13:06.000000 atlantiscore-2.2.0/atlantiscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-29 15:13:06.000000 atlantiscore-2.2.0/atlantiscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:13:06.000000 atlantiscore-2.2.0/atlantiscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-29 15:13:06.000000 atlantiscore-2.2.0/atlantiscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:13:06.000000 atlantiscore-2.2.0/atlantiscore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:13:06.988612 atlantiscore-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:13:06.984612 atlantiscore-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-29 15:12:31.000000 atlantiscore-2.2.0/tests/test_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.207250 atlantiscore-2.3.0/atlantiscore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/atlantiscore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/atlantiscore/db/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/db/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/db/types/evm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/atlantiscore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/lib/eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/atlantiscore/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/types/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/atlantiscore/types/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/atlantiscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 16:19:23.000000 atlantiscore-2.3.0/atlantiscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-10 16:19:23.000000 atlantiscore-2.3.0/atlantiscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:19:23.000000 atlantiscore-2.3.0/atlantiscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-10 16:19:23.000000 atlantiscore-2.3.0/atlantiscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 16:19:23.000000 atlantiscore-2.3.0/atlantiscore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:19:23.211250 atlantiscore-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-10 16:18:57.000000 atlantiscore-2.3.0/tests/test_finder.py
```

### Comparing `atlantiscore-2.2.0/atlantiscore/__init__.py` & `atlantiscore-2.3.0/atlantiscore/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-2.2.0/atlantiscore/db/types/evm.py` & `atlantiscore-2.3.0/atlantiscore/db/types/evm.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-2.2.0/atlantiscore/lib/eth.py` & `atlantiscore-2.3.0/atlantiscore/lib/eth.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-2.2.0/atlantiscore/types/evm.py` & `atlantiscore-2.3.0/atlantiscore/types/evm.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
     def __ne__(self, other: any) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return int(self)
 
+    def __bool__(self) -> bool:
+        return bool(int(self))
+
     @classmethod
     def __get_validators__(cls) -> Iterator[Callable]:
         yield cls.validate
 
     @classmethod
     def validate(cls, v: EVMAddress | LiteralEVMAddress) -> Self:
         try:
```

### Comparing `atlantiscore-2.2.0/pyproject.toml` & `atlantiscore-2.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlantiscore"
-version = "2.2.0"
+version = "2.3.0"
 description = "atlantiscore"
 readme = "README.md"
 authors = [{ name = "Atlantis Labs", email = "r00tail@protonmail.com" }]
 dependencies = [
     "codercore ~= 2.2",
     "coincurve ~= 18.0",
     "eth-hash[pycryptodome]~=0.5",
@@ -32,15 +32,15 @@
     "flake8 ~= 6.0",
     "isort ~= 5.12",
     "pre-commit ~= 2.21",
 ]
 
 
 [tool.bumpver]
-current_version = "2.2.0"
+current_version = "2.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `atlantiscore-2.2.0/tests/test_finder.py` & `atlantiscore-2.3.0/tests/test_finder.py`

 * *Files identical despite different names*

