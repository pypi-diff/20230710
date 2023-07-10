# Comparing `tmp/vfsfusepy-0.2.0.tar.gz` & `tmp/vfsfusepy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfsfusepy-0.2.0.tar", last modified: Fri Jul  7 07:52:37 2023, max compression
+gzip compressed data, was "vfsfusepy-0.2.1.tar", last modified: Mon Jul 10 08:25:22 2023, max compression
```

## Comparing `vfsfusepy-0.2.0.tar` & `vfsfusepy-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:52:37.315151 vfsfusepy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 07:52:24.000000 vfsfusepy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-07 07:52:37.315151 vfsfusepy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-07 07:52:24.000000 vfsfusepy-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 07:52:24.000000 vfsfusepy-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 07:52:24.000000 vfsfusepy-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 07:52:37.315151 vfsfusepy-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:52:37.311151 vfsfusepy-0.2.0/vfsfusepy/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 07:52:24.000000 vfsfusepy-0.2.0/vfsfusepy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6679 2023-07-07 07:52:24.000000 vfsfusepy-0.2.0/vfsfusepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 07:52:25.000000 vfsfusepy-0.2.0/vfsfusepy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:52:37.315151 vfsfusepy-0.2.0/vfsfusepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-07 07:52:37.000000 vfsfusepy-0.2.0/vfsfusepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-07 07:52:37.000000 vfsfusepy-0.2.0/vfsfusepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:52:37.000000 vfsfusepy-0.2.0/vfsfusepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-07 07:52:37.000000 vfsfusepy-0.2.0/vfsfusepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 07:52:37.000000 vfsfusepy-0.2.0/vfsfusepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 07:52:37.000000 vfsfusepy-0.2.0/vfsfusepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:22.851619 vfsfusepy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 08:25:22.851619 vfsfusepy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 08:25:22.851619 vfsfusepy-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:22.851619 vfsfusepy-0.2.1/vfsfusepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/vfsfusepy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/vfsfusepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/vfsfusepy/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/vfsfusepy/git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/vfsfusepy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 08:25:08.000000 vfsfusepy-0.2.1/vfsfusepy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-10 08:25:07.000000 vfsfusepy-0.2.1/vfsfusepy/vfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:25:22.851619 vfsfusepy-0.2.1/vfsfusepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 08:25:22.000000 vfsfusepy-0.2.1/vfsfusepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 08:25:22.000000 vfsfusepy-0.2.1/vfsfusepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:25:22.000000 vfsfusepy-0.2.1/vfsfusepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:25:22.000000 vfsfusepy-0.2.1/vfsfusepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 08:25:22.000000 vfsfusepy-0.2.1/vfsfusepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 08:25:22.000000 vfsfusepy-0.2.1/vfsfusepy.egg-info/top_level.txt
```

### Comparing `vfsfusepy-0.2.0/LICENSE` & `vfsfusepy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.0/PKG-INFO` & `vfsfusepy-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfsfusepy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A versioned file system based on FUSE and Git.
 Home-page: https://github.com/nero19960329/VFS-FUSE
 Author: Zhao Wang
 Author-email: wangzhao2013tsinghua@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -86,16 +86,28 @@
 
 # Create a new file
 echo "Hello, World!" > test.txt
 
 # View the file
 cat test.txt
 
+# Rename the file
+mv test.txt test2.txt
+
 # Remove the file
-rm test.txt
+rm test2.txt
+
+# Create a new directory
+mkdir test_dir
+
+# Rename the directory
+mv test_dir test_dir2
+
+# Remove the directory
+rm -rf test_dir2
 
 # View the commit history
 git log
 ```
 
 In this example, when you write to test.txt, the file system automatically commits the changes to the Git repository located at `/data/vfs-root`. You can then use standard Git commands to view the commit history and checkout previous versions of the file.
```

### Comparing `vfsfusepy-0.2.0/README.md` & `vfsfusepy-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,28 @@
 
 # Create a new file
 echo "Hello, World!" > test.txt
 
 # View the file
 cat test.txt
 
+# Rename the file
+mv test.txt test2.txt
+
 # Remove the file
-rm test.txt
+rm test2.txt
+
+# Create a new directory
+mkdir test_dir
+
+# Rename the directory
+mv test_dir test_dir2
+
+# Remove the directory
+rm -rf test_dir2
 
 # View the commit history
 git log
 ```
 
 In this example, when you write to test.txt, the file system automatically commits the changes to the Git repository located at `/data/vfs-root`. You can then use standard Git commands to view the commit history and checkout previous versions of the file.
```

### Comparing `vfsfusepy-0.2.0/setup.cfg` & `vfsfusepy-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.0/vfsfusepy.egg-info/PKG-INFO` & `vfsfusepy-0.2.1/vfsfusepy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfsfusepy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A versioned file system based on FUSE and Git.
 Home-page: https://github.com/nero19960329/VFS-FUSE
 Author: Zhao Wang
 Author-email: wangzhao2013tsinghua@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -86,16 +86,28 @@
 
 # Create a new file
 echo "Hello, World!" > test.txt
 
 # View the file
 cat test.txt
 
+# Rename the file
+mv test.txt test2.txt
+
 # Remove the file
-rm test.txt
+rm test2.txt
+
+# Create a new directory
+mkdir test_dir
+
+# Rename the directory
+mv test_dir test_dir2
+
+# Remove the directory
+rm -rf test_dir2
 
 # View the commit history
 git log
 ```
 
 In this example, when you write to test.txt, the file system automatically commits the changes to the Git repository located at `/data/vfs-root`. You can then use standard Git commands to view the commit history and checkout previous versions of the file.
```

