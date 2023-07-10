# Comparing `tmp/vfsfusepy-0.2.2.tar.gz` & `tmp/vfsfusepy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfsfusepy-0.2.2.tar", last modified: Mon Jul 10 08:35:50 2023, max compression
+gzip compressed data, was "vfsfusepy-0.3.0.tar", last modified: Mon Jul 10 09:03:28 2023, max compression
```

## Comparing `vfsfusepy-0.2.2.tar` & `vfsfusepy-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:35:50.686020 vfsfusepy-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 08:35:50.686020 vfsfusepy-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 08:35:50.686020 vfsfusepy-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:35:50.682021 vfsfusepy-0.2.2/vfsfusepy/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/vfsfusepy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/vfsfusepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/vfsfusepy/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/vfsfusepy/git_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/vfsfusepy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 08:35:37.000000 vfsfusepy-0.2.2/vfsfusepy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-10 08:35:36.000000 vfsfusepy-0.2.2/vfsfusepy/vfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:35:50.686020 vfsfusepy-0.2.2/vfsfusepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 08:35:50.000000 vfsfusepy-0.2.2/vfsfusepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 08:35:50.000000 vfsfusepy-0.2.2/vfsfusepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:35:50.000000 vfsfusepy-0.2.2/vfsfusepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:35:50.000000 vfsfusepy-0.2.2/vfsfusepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 08:35:50.000000 vfsfusepy-0.2.2/vfsfusepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 08:35:50.000000 vfsfusepy-0.2.2/vfsfusepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/vfsfusepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/git_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 09:03:13.000000 vfsfusepy-0.3.0/vfsfusepy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-10 09:03:12.000000 vfsfusepy-0.3.0/vfsfusepy/vfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:03:28.295715 vfsfusepy-0.3.0/vfsfusepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:03:28.000000 vfsfusepy-0.3.0/vfsfusepy.egg-info/top_level.txt
```

### Comparing `vfsfusepy-0.2.2/LICENSE` & `vfsfusepy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.2/PKG-INFO` & `vfsfusepy-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfsfusepy
-Version: 0.2.2
+Version: 0.3.0
 Summary: A versioned file system based on FUSE and Git.
 Home-page: https://github.com/nero19960329/VFS-FUSE
 Author: Zhao Wang
 Author-email: wangzhao2013tsinghua@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `vfsfusepy-0.2.2/README.md` & `vfsfusepy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.2/setup.cfg` & `vfsfusepy-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.2/vfsfusepy/__main__.py` & `vfsfusepy-0.3.0/vfsfusepy/__main__.py`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.2/vfsfusepy/file_operations.py` & `vfsfusepy-0.3.0/vfsfusepy/file_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,7 +41,40 @@
         f.seek(offset)
         return f.write(data)
 
 
 def truncate(path: str, length: int, fh: Optional[int] = None) -> None:
     with open(path, "rb+") as f:
         f.truncate(length)
+
+
+def access(path: str, mode: int) -> None:
+    if not os.access(path, mode):
+        raise PermissionError(path)
+
+
+def readlink(path: str) -> str:
+    pathname = os.readlink(path)
+    if pathname.startswith("/"):
+        # Path name is absolute, sanitize it.
+        return os.path.relpath(pathname, os.path.dirname(path))
+    else:
+        return pathname
+
+
+def statfs(path: str) -> Dict[str, Any]:
+    stv = os.statvfs(path)
+    return {
+        key: getattr(stv, key)
+        for key in (
+            "f_bavail",
+            "f_bfree",
+            "f_blocks",
+            "f_bsize",
+            "f_favail",
+            "f_ffree",
+            "f_files",
+            "f_flag",
+            "f_frsize",
+            "f_namemax",
+        )
+    }
```

### Comparing `vfsfusepy-0.2.2/vfsfusepy/utils.py` & `vfsfusepy-0.3.0/vfsfusepy/utils.py`

 * *Files identical despite different names*

### Comparing `vfsfusepy-0.2.2/vfsfusepy/vfs.py` & `vfsfusepy-0.3.0/vfsfusepy/vfs.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     @handle_os_errors
     def create(self, path: str, mode: int) -> int:
         full_path = file_path(self.repo.working_dir, path)
         file_operations.create(full_path, mode)
         if is_git_path(path):
             return 0
-        self.repo.git.add(full_path)
+        git_operations.add(self.repo, full_path)
         git_operations.commit(self.repo, "-m", f"create file {path}")
         return 0
 
     @handle_os_errors
     def read(self, path: str, size: int, offset: int, fh: int) -> bytes:
         return file_operations.read(
             file_path(self.repo.working_dir, path), size, offset, fh
@@ -46,50 +46,50 @@
     def write(self, path: str, data: bytes, offset: int, fh: int) -> int:
         full_path = file_path(self.repo.working_dir, path)
         size = file_operations.write(full_path, data, offset, fh)
         if is_git_path(path):
             return size
 
         full_path = file_path(self.repo.working_dir, path)
-        self.repo.git.add(full_path)
+        git_operations.add(self.repo, full_path)
         git_operations.commit(self.repo, "-m", f"write file {path}")
         return size
 
     @handle_os_errors
     def truncate(self, path: str, length: int, fh: Optional[int] = None) -> int:
         full_path = file_path(self.repo.working_dir, path)
         file_operations.truncate(full_path, length, fh)
         if is_git_path(path):
             return 0
 
-        self.repo.git.add(full_path)
+        git_operations.add(self.repo, full_path)
         git_operations.commit(self.repo, "-m", f"truncate file {path}")
 
     @handle_os_errors
     def unlink(self, path: str) -> None:
         full_path = file_path(self.repo.working_dir, path)
         os.unlink(full_path)
         if is_git_path(path):
             return
 
-        self.repo.git.rm(full_path)
+        git_operations.add(self.repo, full_path)
         git_operations.commit(self.repo, "-m", f"remove file {path}")
 
     @handle_os_errors
     def mkdir(self, path: str, mode: int) -> None:
         full_path = file_path(self.repo.working_dir, path)
         os.mkdir(full_path, mode)
         if is_git_path(path):
             return
 
         gitkeep_path = os.path.join(full_path, ".gitkeep")
         # Create .gitkeep file to track empty directories in Git
         with open(gitkeep_path, "w") as f:
             pass
-        self.repo.git.add(full_path)
+        git_operations.add(self.repo, full_path)
         git_operations.commit(self.repo, "-m", f"create directory {path}")
 
     @handle_os_errors
     def rmdir(self, path: str) -> None:
         full_path = file_path(self.repo.working_dir, path)
         if os.path.exists(full_path):
             os.rmdir(full_path)
@@ -98,18 +98,65 @@
     def rename(self, old_path: str, new_path: str) -> None:
         old_full_path = file_path(self.repo.working_dir, old_path)
         new_full_path = file_path(self.repo.working_dir, new_path)
         os.rename(old_full_path, new_full_path)
         if is_git_path(old_path) and is_git_path(new_path):
             return
         if is_git_path(old_path):
-            self.repo.git.add(new_full_path)
+            git_operations.add(self.repo, new_full_path)
             git_operations.commit(self.repo, "-m", f"create file {new_path}")
             return
         if is_git_path(new_path):
             self.repo.git.rm(old_full_path)
             git_operations.commit(self.repo, "-m", f"remove file {old_path}")
             return
 
-        self.repo.git.add(old_full_path)
-        self.repo.git.add(new_full_path)
+        git_operations.add(self.repo, old_full_path)
+        git_operations.add(self.repo, new_full_path)
         git_operations.commit(self.repo, "-m", f"rename from {old_path} to {new_path}")
+
+    @handle_os_errors
+    def access(self, path: str, mode: int) -> None:
+        file_operations.access(file_path(self.repo.working_dir, path), mode)
+
+    @handle_os_errors
+    def chmod(self, path: str, mode: int) -> None:
+        full_path = file_path(self.repo.working_dir, path)
+        os.chmod(full_path, mode)
+        if is_git_path(path):
+            return
+
+        git_operations.add(self.repo, full_path)
+        git_operations.commit(self.repo, "-m", f"change mode of {path}")
+
+    @handle_os_errors
+    def readlink(self, path: str) -> str:
+        full_path = file_path(self.repo.working_dir, path)
+        pathname = os.readlink(full_path)
+        if pathname.startswith("/"):
+            # Path name is absolute, sanitize it.
+            return os.path.relpath(pathname, self.repo.working_dir)
+        return pathname
+
+    @handle_os_errors
+    def mknod(self, path: str, mode: int, dev: int) -> None:
+        os.mknod(file_path(self.repo.working_dir, path), mode, dev)
+
+    @handle_os_errors
+    def symlink(self, target: str, source: str) -> None:
+        full_path = file_path(self.repo.working_dir, target)
+        os.symlink(file_path(self.repo.working_dir, source), full_path)
+        if is_git_path(target):
+            return
+
+        git_operations.add(self.repo, full_path)
+        git_operations.commit(self.repo, "-m", f"create file {target}")
+
+    @handle_os_errors
+    def link(self, target: str, source: str) -> None:
+        full_path = file_path(self.repo.working_dir, target)
+        os.link(file_path(self.repo.working_dir, source), full_path)
+        if is_git_path(target):
+            return
+
+        git_operations.add(self.repo, full_path)
+        git_operations.commit(self.repo, "-m", f"create file {target}")
```

### Comparing `vfsfusepy-0.2.2/vfsfusepy.egg-info/PKG-INFO` & `vfsfusepy-0.3.0/vfsfusepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfsfusepy
-Version: 0.2.2
+Version: 0.3.0
 Summary: A versioned file system based on FUSE and Git.
 Home-page: https://github.com/nero19960329/VFS-FUSE
 Author: Zhao Wang
 Author-email: wangzhao2013tsinghua@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

