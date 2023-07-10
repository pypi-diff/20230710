# Comparing `tmp/vfsfusepy-0.3.0.tar.gz` & `tmp/vfsfusepy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfsfusepy-0.3.0.tar", last modified: Mon Jul 10 09:03:28 2023, max compression
+gzip compressed data, was "vfsfusepy-0.4.0.tar", last modified: Mon Jul 10 09:07:02 2023, max compression
```

## Comparing `vfsfusepy-0.3.0.tar` & `vfsfusepy-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/vfsfusepy/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/git_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 09:03:13.000000 vfsfusepy-0.3.0/vfsfusepy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/vfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/vfsfusepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:07:02.365424 vfsfusepy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 09:07:02.365424 vfsfusepy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 09:07:02.365424 vfsfusepy-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:07:02.365424 vfsfusepy-0.4.0/vfsfusepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/vfsfusepy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/vfsfusepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/vfsfusepy/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/vfsfusepy/git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/vfsfusepy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 09:06:48.000000 vfsfusepy-0.4.0/vfsfusepy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-10 09:06:47.000000 vfsfusepy-0.4.0/vfsfusepy/vfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:07:02.365424 vfsfusepy-0.4.0/vfsfusepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 09:07:02.000000 vfsfusepy-0.4.0/vfsfusepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 09:07:02.000000 vfsfusepy-0.4.0/vfsfusepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:07:02.000000 vfsfusepy-0.4.0/vfsfusepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 09:07:02.000000 vfsfusepy-0.4.0/vfsfusepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:07:02.000000 vfsfusepy-0.4.0/vfsfusepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:07:02.000000 vfsfusepy-0.4.0/vfsfusepy.egg-info/top_level.txt
```

### Comparing `vfsfusepy-0.3.0/LICENSE` & `vfsfusepy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.3.0/PKG-INFO` & `vfsfusepy-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfsfusepy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A versioned file system based on FUSE and Git.
 Home-page: https://github.com/nero19960329/VFS-FUSE
 Author: Zhao Wang
 Author-email: wangzhao2013tsinghua@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `vfsfusepy-0.3.0/README.md` & `vfsfusepy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.3.0/setup.cfg` & `vfsfusepy-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.3.0/vfsfusepy/__main__.py` & `vfsfusepy-0.4.0/vfsfusepy/__main__.py`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.3.0/vfsfusepy/file_operations.py` & `vfsfusepy-0.4.0/vfsfusepy/file_operations.py`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.3.0/vfsfusepy/utils.py` & `vfsfusepy-0.4.0/vfsfusepy/utils.py`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.3.0/vfsfusepy/vfs.py` & `vfsfusepy-0.4.0/vfsfusepy/vfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,14 @@
     @handle_os_errors
     def mkdir(self, path: str, mode: int) -> None:
         full_path = file_path(self.repo.working_dir, path)
         os.mkdir(full_path, mode)
         if is_git_path(path):
             return
 
-        gitkeep_path = os.path.join(full_path, ".gitkeep")
-        # Create .gitkeep file to track empty directories in Git
-        with open(gitkeep_path, "w") as f:
-            pass
         git_operations.add(self.repo, full_path)
         git_operations.commit(self.repo, "-m", f"create directory {path}")
 
     @handle_os_errors
     def rmdir(self, path: str) -> None:
         full_path = file_path(self.repo.working_dir, path)
         if os.path.exists(full_path):
```

### Comparing `vfsfusepy-0.3.0/vfsfusepy.egg-info/PKG-INFO` & `vfsfusepy-0.4.0/vfsfusepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfsfusepy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A versioned file system based on FUSE and Git.
 Home-page: https://github.com/nero19960329/VFS-FUSE
 Author: Zhao Wang
 Author-email: wangzhao2013tsinghua@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

