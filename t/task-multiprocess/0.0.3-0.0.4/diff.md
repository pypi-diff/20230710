# Comparing `tmp/task_multiprocess-0.0.3.tar.gz` & `tmp/task_multiprocess-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task_multiprocess-0.0.3.tar", last modified: Mon Jul 10 06:41:49 2023, max compression
+gzip compressed data, was "task_multiprocess-0.0.4.tar", last modified: Mon Jul 10 14:16:56 2023, max compression
```

## Comparing `task_multiprocess-0.0.3.tar` & `task_multiprocess-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:49.540000 task_multiprocess-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-07-07 07:05:10.000000 task_multiprocess-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 06:41:49.540000 task_multiprocess-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 15:20:42.000000 task_multiprocess-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 06:41:49.540000 task_multiprocess-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-10 06:39:54.000000 task_multiprocess-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:49.536000 task_multiprocess-0.0.3/task_multiprocess/
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-07 15:18:02.000000 task_multiprocess-0.0.3/task_multiprocess/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2039 2023-07-10 06:35:19.000000 task_multiprocess-0.0.3/task_multiprocess/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:49.540000 task_multiprocess-0.0.3/task_multiprocess.egg-info/
--rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 06:41:49.000000 task_multiprocess-0.0.3/task_multiprocess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-10 06:41:49.000000 task_multiprocess-0.0.3/task_multiprocess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 06:41:49.000000 task_multiprocess-0.0.3/task_multiprocess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 06:41:49.000000 task_multiprocess-0.0.3/task_multiprocess.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:56.244000 task_multiprocess-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-07 07:05:10.000000 task_multiprocess-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-07-10 14:16:56.244000 task_multiprocess-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      896 2023-07-10 07:37:23.000000 task_multiprocess-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:16:56.244000 task_multiprocess-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-10 14:16:16.000000 task_multiprocess-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:56.244000 task_multiprocess-0.0.4/task_multiprocess/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-07 15:18:02.000000 task_multiprocess-0.0.4/task_multiprocess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-10 14:16:16.000000 task_multiprocess-0.0.4/task_multiprocess/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:16:56.244000 task_multiprocess-0.0.4/task_multiprocess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-07-10 14:16:56.000000 task_multiprocess-0.0.4/task_multiprocess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-10 14:16:56.000000 task_multiprocess-0.0.4/task_multiprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:16:56.000000 task_multiprocess-0.0.4/task_multiprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 14:16:56.000000 task_multiprocess-0.0.4/task_multiprocess.egg-info/top_level.txt
```

### Comparing `task_multiprocess-0.0.3/LICENSE` & `task_multiprocess-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `task_multiprocess-0.0.3/task_multiprocess/main.py` & `task_multiprocess-0.0.4/task_multiprocess/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 import os
 
-cpu_num = 10
 
+class TaskMultiprocess:
+    cpu_num = os.cpu_count()
 
-# 配合多进程使用的队列
-def generate_queue(queue_list, num=2, desc='generate_queue'):
-    # queue_list 将列表形式的数据存放在队列中，返回队列,队列的大小,进程共享的list,子进程的Process_id_list
-    from multiprocessing import Manager
-    from tqdm import tqdm
-    lock = Manager().Lock()
-    q = Manager().Queue()
-    for i in tqdm(queue_list, position=0, desc=desc):
-        q.put(str(i))
-    q_size = q.qsize()
-    return q, q_size, lock, [Manager().list() for i in range(num)]
-
-
-# 多进程装饰器
-def multiprocess_decorator(cpu_num=os.cpu_count()):
-    def wrapper(func):
-        from multiprocessing import Process
-        def main(*args, **kwargs):
-            process_list = []
-            for _ in range(cpu_num):  # 开启多个子进程执行func函数
-                p = Process(target=func, args=(*args,), kwargs=kwargs)  # 实例化进程对象
-                p.start()
-                process_list.append(p)
-            for p in process_list:
-                p.join()
-
-        #         return  # 不需要子进程函数执行结果
-        return main
-
-    return wrapper
-
-
-@multiprocess_decorator(cpu_num)
-def common_multiprocess(fun, q_num, cpu_num=os.cpu_count(), q=None, q_size=0,
-                        lock=None, block=True, timeout=2):
-    from tqdm import tqdm
-    pbar = tqdm(total=q_size, position=0, desc='')
-    try:
-        while q.qsize():
-            lock.acquire()
-            # q_element_list = [q.get(block=block, timeout=timeout) for i in range(q_num)]
-            q_element_list = [q.get_nowait() for i in range(q_num)]
-            lock.release()
-            # print(q_element_list)
-            fun(q_element_list)
-            # process_id_list.append(os.getpid())
-            pbar.update(q_num * cpu_num)
-    except Exception as e:
-        print(e)
-        pass
+    # 配合多进程使用的队列
+    def generate_queue(self, queue_list, num=2, desc='generate_queue'):
+        # queue_list 将列表形式的数据存放在队列中，返回队列,队列的大小,进程共享的list
+        from multiprocessing import Manager
+        from tqdm import tqdm
+        lock = Manager().Lock()
+        q = Manager().Queue()
+        for i in tqdm(queue_list, position=0, desc=desc):
+            q.put(str(i))
+        q_size = q.qsize()
+        return q, q_size, lock, [Manager().list() for i in range(num)]
+
+    # 多进程装饰器
+    @staticmethod
+    def multiprocess_decorator(cpu_num=os.cpu_count()):
+        def wrapper(func):
+            from multiprocessing import Process
+            def main(*args, **kwargs):
+                process_list = []
+                for _ in range(cpu_num):  # 开启多个子进程执行func函数
+                    p = Process(target=func, args=(*args,), kwargs=kwargs)  # 实例化进程对象
+                    p.start()
+                    process_list.append(p)
+                for p in process_list:
+                    p.join()
+
+            #         return  # 不需要子进程函数执行结果
+            return main
+
+        return wrapper
+
+    @multiprocess_decorator(cpu_num)
+    def common_multiprocess(self, fun, q_num, cpu_num=os.cpu_count(), q=None, q_size=0,
+                            lock=None, block=True, timeout=2):
+        from tqdm import tqdm
+        pbar = tqdm(total=q_size, position=0, desc='')
+        try:
+            while q.qsize():
+                lock.acquire()
+                # q_element_list = [q.get(block=block, timeout=timeout) for i in range(q_num)]
+                q_element_list = [q.get_nowait() for i in range(q_num)]
+                lock.release()
+                # print(q_element_list)
+                fun(q_element_list)
+                # process_id_list.append(os.getpid())
+                pbar.update(q_num * cpu_num)
+        except Exception as e:
+            print(e)
+            pass
 
 
 """
 sample_list = list(range(10))[:]
 q, q_size, lock, public_list = generate_queue(sample_list,num=2)
 """
```

