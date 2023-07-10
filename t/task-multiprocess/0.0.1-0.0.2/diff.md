# Comparing `tmp/task_multiprocess-0.0.1.tar.gz` & `tmp/task_multiprocess-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task_multiprocess-0.0.1.tar", last modified: Mon Jul 10 06:16:59 2023, max compression
+gzip compressed data, was "task_multiprocess-0.0.2.tar", last modified: Mon Jul 10 06:31:10 2023, max compression
```

## Comparing `task_multiprocess-0.0.1.tar` & `task_multiprocess-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:16:59.336000 task_multiprocess-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-07-07 07:05:10.000000 task_multiprocess-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 06:16:59.336000 task_multiprocess-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 15:20:42.000000 task_multiprocess-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 06:16:59.336000 task_multiprocess-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-10 06:14:52.000000 task_multiprocess-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:16:59.336000 task_multiprocess-0.0.1/task_multiprocess/
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-07 15:18:02.000000 task_multiprocess-0.0.1/task_multiprocess/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-10 05:53:55.000000 task_multiprocess-0.0.1/task_multiprocess/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:16:59.336000 task_multiprocess-0.0.1/task_multiprocess.egg-info/
--rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 06:16:59.000000 task_multiprocess-0.0.1/task_multiprocess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-10 06:16:59.000000 task_multiprocess-0.0.1/task_multiprocess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 06:16:59.000000 task_multiprocess-0.0.1/task_multiprocess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 06:16:59.000000 task_multiprocess-0.0.1/task_multiprocess.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:31:10.700000 task_multiprocess-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-07 07:05:10.000000 task_multiprocess-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 06:31:10.700000 task_multiprocess-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 15:20:42.000000 task_multiprocess-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 06:31:10.700000 task_multiprocess-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-10 06:30:52.000000 task_multiprocess-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:31:10.700000 task_multiprocess-0.0.2/task_multiprocess/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-07 15:18:02.000000 task_multiprocess-0.0.2/task_multiprocess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-07-10 06:30:37.000000 task_multiprocess-0.0.2/task_multiprocess/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:31:10.700000 task_multiprocess-0.0.2/task_multiprocess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 06:31:10.000000 task_multiprocess-0.0.2/task_multiprocess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-10 06:31:10.000000 task_multiprocess-0.0.2/task_multiprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 06:31:10.000000 task_multiprocess-0.0.2/task_multiprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 06:31:10.000000 task_multiprocess-0.0.2/task_multiprocess.egg-info/top_level.txt
```

### Comparing `task_multiprocess-0.0.1/LICENSE` & `task_multiprocess-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `task_multiprocess-0.0.1/setup.py` & `task_multiprocess-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="task_multiprocess",
-    version="0.0.1",
+    version="0.0.2",
     author="raymond",
     author_email="lei20190123@gmail.com",
     description="run tasks in parallel",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=['task_multiprocess'],
```

### Comparing `task_multiprocess-0.0.1/task_multiprocess/main.py` & `task_multiprocess-0.0.2/task_multiprocess/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,21 +32,22 @@
         #         return  # 不需要子进程函数执行结果
         return main
 
     return wrapper
 
 
 @multiprocess_decorator(cpu_num)
-def common_multiprocess(fun, q_num, cpu_num=os.cpu_count(), q=None, q_size=0, lock=None):
+def common_multiprocess(fun, q_num, cpu_num=os.cpu_count(), q=None, q_size=0,
+                        lock=None, block=True, timeout=2):
     from tqdm import tqdm
     pbar = tqdm(total=q_size, position=0, desc='')
     try:
         while q.qsize():
             lock.acquire()
-            q_element_list = [q.get() for i in range(q_num)]
+            q_element_list = [q.get(block=block, timeout=timeout) for i in range(q_num)]
             lock.release()
             # print(q_element_list)
             fun(q_element_list)
             # process_id_list.append(os.getpid())
             pbar.update(q_num * cpu_num)
     except Exception as e:
         print(e)
```

