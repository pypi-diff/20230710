# Comparing `tmp/deadpool_executor-2023.7.1.tar.gz` & `tmp/deadpool_executor-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpool_executor-2023.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deadpool_executor-2023.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deadpool_executor-2023.7.1.tar` & `deadpool_executor-2023.7.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/.coveragerc
--rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.1/LICENSE
--rw-r--r--   0        0        0    20242 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/README.rst
--rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/covstart.pth
--rw-r--r--   0        0        0    22051 2023-07-06 00:57:38.760330 deadpool_executor-2023.7.1/deadpool.py
--rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/examples/callbacks.py
--rw-r--r--   0        0        0      516 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/examples/entrypoint.py
--rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/examples/priorities.py
--rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/noxfile.py
--rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/tests/conftest.py
--rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/tests/test_deadpool.py
--rw-r--r--   0        0        0    21321 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/.coveragerc
+-rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.2/LICENSE
+-rw-r--r--   0        0        0    22826 2023-07-10 00:05:36.185684 deadpool_executor-2023.7.2/README.rst
+-rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/covstart.pth
+-rw-r--r--   0        0        0    22394 2023-07-10 00:01:01.439799 deadpool_executor-2023.7.2/deadpool.py
+-rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/examples/callbacks.py
+-rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.2/examples/entrypoint.py
+-rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/examples/priorities.py
+-rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/noxfile.py
+-rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/tests/conftest.py
+-rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.2/tests/test_deadpool.py
+-rw-r--r--   0        0        0    23905 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.2/PKG-INFO
```

### Comparing `deadpool_executor-2023.7.1/LICENSE` & `deadpool_executor-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.1/README.rst` & `deadpool_executor-2023.7.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,32 +28,36 @@
     :alt: This project uses the "black" style formatter for Python code
     :target: https://github.com/python/black
 
 .. image:: https://api.securityscorecards.dev/projects/github.com/cjrh/deadpool/badge
     :alt: OpenSSF Scorecard
     :target: https://api.securityscorecards.dev/projects/github.com/cjrh/deadpool
 
-deadpool
-========
+
+Deadpool
+--------
 
 ``Deadpool`` is a process pool that is really hard to kill.
 
 ``Deadpool`` is an implementation of the ``Executor`` interface
 in the ``concurrent.futures`` standard library. ``Deadpool`` is
 a process pool executor, quite similar to the stdlib's
 `ProcessPoolExecutor`_.
 
 This document assumes that you are familiar with the stdlib
 `ProcessPoolExecutor`_. If you are not, it is important
 to understand that ``Deadpool`` makes very specific tradeoffs that
 can result in quite different behaviour to the stdlib
 implementation.
 
+.. sectnum::
+
 .. contents::
    :local:
+   :depth: 2
    :backlinks: entry
 
 Installation
 ------------
 
 The python package name is *deadpool-executor*, so to install
 you must type ``$ pip install deadpool-executor``. The import
@@ -73,59 +77,72 @@
 task, which the stdlib executor doesn't provide.
 
 You might wonder, isn't it bad to just kill a task like that?
 In my use-case, we had extensive logging and monitoring to alert
 us if any tasks failed; but it was paramount that our services
 continue to operate even when tasks got killed in OOM scenarios,
 or specific tasks took too long. This is the primary trade-off
-that ``Deadpool`` offers.
+that ``Deadpool`` offers: the pool will not break, but tasks
+can receive SIGKILL under certain conditions. This trade-off
+is likely fine if you've seen many OOMs break your pools.
 
 I also tried using the `Pebble <https://github.com/noxdafox/pebble>`_
 community process pool. This is a cool project, featuring several
 of the properties I've been looking for such as timeouts, and
 more resilient operation. However, during testing I found several
 occurrences of a mysterious `RuntimeError`_ that caused the Pebble
 pool to become broken and no longer accept new tasks.
 
-My goal with ``Deadpool`` is to make a process pool executor that
-is impossible to break. The tradeoffs are that I care less about:
-
-- being cross-platform
-- optimizing per-task latency
+My goal with ``Deadpool`` is that **the pool must never enter
+a broken state**. Any means by which that can happen will be
+considered a bug.
 
 What differs from `ProcessPoolExecutor`_?
 -----------------------------------------
 
 ``Deadpool`` is generally similar to `ProcessPoolExecutor`_ since it executes
 tasks in subprocesses, and implements the standard ``Executor`` abstract
-interface. However, it differs in the following ways:
+interface. We can draw a few comparisons to the stdlib pool to guide
+your decision process about whether this makes sense for your use-case:
 
-- ``Deadpool`` makes a new subprocess for every task submitted to
-  the pool (up to the ``max_workers`` limit). It is like having
-  ``max_tasks_per_child == 1`` (a new feature in
+- ``Deadpool`` precreates all subprocesses up to the pool size.
+- ``Deadpool`` also supports the
+  ``max_tasks_per_child`` parameter (a new feature in
   Python 3.11, although it was available in `multiprocessing.Pool`_
-  since Python 3.2). I have ideas about making this configurable, but
-  for now this is a much less important than overall resilience of
-  the pool. This also means that ``Deadpool`` doesn't suffer from
-  long-lived subprocesses being affected by memory leaks, usually
-  created by native extensions.
+  since Python 3.2).
+- ``Deadpool`` tasks can have priorities. When the executor chooses
+  the next pending task to schedule to a subprocess, it chooses the
+  pending task with the highest priority. This gives you a way of
+  prioritizing certain kinds of tasks. For example, you might give
+  UI-sensitive tasks a higher priority to deliver a more snappy
+  user experience to your users.
 - ``Deadpool`` defaults to the `forkserver <https://docs.python.org/3.11/library/multiprocessing.html#contexts-and-start-methods>`_ multiprocessing
   context, unlike the stdlib pool which defaults to ``fork`` on
   Linux. It's just a setting though, you can change it in the same way as
-  with the stdlib pool.
-- ``Deadpool`` does not keep a pool of processes around indefinitely.
-  There will only be as many concurrent processes running as there
-  is work to be done, up to the limit set by the ``max_workers``
-  parameter; but if there are fewer tasks to be executed, there will
-  be fewer active subprocesses. When there are no pending or active
-  tasks, there will be *no subprocesses present*. They are created
-  on demand as necessary and disappear when not required.
+  with the stdlib pool. Like the stdlib, I strongly advise you to avoid
+  using ``fork`` because propagation threads and locks via fork is
+  going to ruin your day eventually.
+- ``Deadpool`` can ask the system allocator (Linux only) to return
+  unused memory back to the OS based on exceeding a max threshold RSS.
+  For long-running pools and modern
+  kernels, the system memory allocator can hold onto unused memory
+  for a surprisingly long time, and coupled with bloat due to
+  memory fragmentation, this can result in carrying very large
+  RSS values in your pool. The ``max_tasks_per_child`` helps with
+  this because a subprocess is entirely erased when the max is
+  reached, but it does mean that periodically there will be a small
+  latency penalty from constructing the replacement subprocess. In
+  my opinion, ``max_tasks_per_child`` is appropriate for when you
+  know or suspect there's a real memory leak somewhere in your code
+  (or a 3rd-party package!), and the easiest way to deal with that
+  right now is just to periodically remove a process.
 - ``Deadpool`` tasks can have timeouts. When a task hits the timeout,
   the underlying subprocess in the pool is killed with ``SIGKILL``.
-  The entire process tree of that subprocess is killed.
+  The entire process tree of that subprocess is killed. Your application
+  logic needs to handle this. The ``finalizer`` will not run.
 - ``Deadpool`` tasks can have priorities. The priority is set in the
   ``submit()`` call. See the examples later in this document for further
   discussion on priorities.
 - The shutdown parameters ``wait`` and ``cancel_futures`` can behave
   differently to how they work in the _ProcessPoolExecutor. This is
   discussed in more detail later in this document.
 - If a ``Deadpool`` subprocess in the pool is killed by some
@@ -142,15 +159,16 @@
   Just like the ``initializer`` callable, the ``finalizer``
   callable is executed inside the subprocess. It is not guaranteed that
   the finalizer will always run. If a process is killed, e.g. due to a
   timeout or any other reason, the finalizer will not run. The finalizer
   could be used for things like flushing pending monitoring messages,
   such as traces and so on.
 - ``Deadpool`` currently only works on Linux. There isn't any specific
-  reason it can't work on other platforms.
+  reason it can't work on other platforms. The malloc trim feature also
+  requires a glibc system, so probably won't work on Alpine.
 
 Show me some code
 -----------------
 
 Simple case
 ^^^^^^^^^^^
 
@@ -217,24 +235,26 @@
         except deadpool.ProcessError:
             print("Oh no someone killed my task!")
 
 
 As long as the OOM killer terminates the subprocess (and not the main process),
 which is likely because it'll be your subprocess that is using too much
 memory, this will not hurt the pool, and it will be able to receive and
-process more tasks.
+process more tasks. Note that this event will show up as a ``ProcessError``
+exception when accessing the future, so you have a way of at least tracking
+these events.
 
 Design Details
 --------------
 
 Typical Example - with timeouts
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Here's a typical example of how code using Deadpool might look. The
-output of this code should be similar to the following:
+output of the code further below should be similar to the following:
 
 .. code-block:: bash
 
     $ python examples/entrypoint.py
     ...................xxxxxxxxxxx.xxxxxxx.x.xxxxxxx.x
     $
 
@@ -339,15 +359,15 @@
 - I also specified the ``max_backlog`` parameter when creating the
   Deadpool instance. This is discussed in more detail next, but quickly:
   task priority can only be enforced on what is in the submitted backlog
   of tasks, and the ``max_backlog`` parameter controls the depth of that
   queue. If ``max_backlog`` is too low, then the window of prioritization
   will not include tasks submitted later which might have higher priorities
   than earlier-submitted tasks. The ``submit`` call will in fact block
-  if the ``max_backlog`` depth has been reached.
+  once the ``max_backlog`` depth has been reached.
 
 Controlling the backlog of submitted tasks
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 By default, the ``max_backlog`` parameter is set to 5. This parameter is
 used to create the "submit queue" size. The submit queue is the place
 where submitted tasks are held before they are executed in background
@@ -424,14 +444,23 @@
         f = exe.submit(work)
 
         def cb(fut: deadpool.Future):
             print(f"My task is running on process {fut.pid}")
 
         f.add_pid_callback(cb)
 
+Obviously, both kinds of callbacks can be added:
+
+.. code-block:: python
+
+    with deadpool.Deadpool() as exe:
+        f = exe.submit(work)
+        f.add_pid_callback(lambda fut: f"Started on {fut.pid=}")
+        f.add_done_callback(lambda fut: f"Completed {fut.pid=}")
+
 More about shutdown
 ^^^^^^^^^^^^^^^^^^^
 
 In the documentation for ProcessPoolExecutor_, the following function
 signature is given for the shutdown_ method of the executor interface:
 
 .. code-block:: python
@@ -528,15 +557,51 @@
 
 To apply style fixes, and check for any remaining lints,
 
 .. code-block:: shell
 
    $ nox -t style
 
+docs
+^^^^
+
+The only docs currently are this README, which uses RST. Github 
+uses `docutils <https://docutils.sourceforge.io/docs/ref/rst/directives.html>`_
+to render RST.
+
+release
+^^^^^^^
+
+This project uses flit to release the package to pypi. The whole
+process isn't as automated as I would like, but this is what
+I currently do:
+
+1. Ensure that ``main`` branch is fully up to date with all to
+   be released, and all the tests succeed.
+2. Change the ``__version__`` field in ``deadpool.py``. Flit
+   uses this to stamp the version.
+3. Verify that ``flit build`` succeeds. This will produce a
+   wheel in the ``dist/`` directory. You can inspect this
+   wheel to ensure it contains only what is necessary. This
+   wheel will be what is uploaded to PyPI.
+4. **Commit the changed ``__version__``**. Easy to forget this
+   step, resulting in multiple awkward releases to try to
+   get the state all correct again.
+5. Now create the git tag and push to github:
+
+   .. code-block:: shell
+
+        $ git tag YYYY.MM.patch
+        $ git push --tags origin main
+
+6. Now deploy to PyPI:
+
+   .. code-block:: shell
 
+        $ flit publish
 
 
 .. _shutdown: https://docs.python.org/3/library/concurrent.futures.html?highlight=brokenprocesspool#concurrent.futures.Executor.shutdown
 .. _ProcessPoolExecutor: https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#processpoolexecutor
 .. _RuntimeError: https://github.com/noxdafox/pebble/issues/42#issuecomment-551245730
 .. _OOM killer: https://en.wikipedia.org/wiki/Out_of_memory#Out_of_memory_management
 .. _multiprocessing.Pool: https://docs.python.org/3.11/library/multiprocessing.html#multiprocessing.pool.Pool
```

### Comparing `deadpool_executor-2023.7.1/deadpool.py` & `deadpool_executor-2023.7.2/deadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 from dataclasses import dataclass, field
 from multiprocessing.connection import Connection
 from queue import Empty, PriorityQueue, Queue, SimpleQueue
 from typing import Callable, Optional, Tuple
 
 import psutil
 
-__version__ = "2023.7.1"
+__version__ = "2023.7.2"
 __all__ = [
     "Deadpool",
     "Future",
     "CancelledError",
     "TimeoutError",
     "ProcessError",
     "PoolClosed",
     "as_completed",
 ]
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("deadpool")
 
 
 @dataclass(order=True)
 class PrioritizedItem:
     priority: int
     item: typing.Any = field(compare=False)
 
@@ -51,14 +51,15 @@
     # Stats
     tasks_ran_counter: int
     # Controls
     # If the subprocess RSS memory is above this threshold,
     # ask the system allocator to release unused memory back
     # to the OS.
     malloc_trim_rss_memory_threshold_bytes: Optional[int] = None
+    ok: bool = True
 
     def __init__(
         self,
         initializer=None,
         initargs=(),
         finalizer=None,
         finargs=(),
@@ -89,14 +90,15 @@
         )
 
         p.start()
         self.process = p
         self.connection_receive_msgs_from_process = conn_receiver
         self.connection_send_msgs_to_process = conn_sender2
         self.tasks_ran_counter = 0
+        self.ok = True
 
     def __hash__(self):
         return hash(self.process.pid)
 
     @property
     def pid(self):
         return self.process.pid
@@ -323,14 +325,18 @@
 
         if self.max_worker_memory_bytes is not None:
             if wp.get_rss_bytes() >= self.max_worker_memory_bytes:
                 wp.shutdown(wait=False)
                 self.add_worker_to_pool()
                 return
 
+        if not wp.ok:
+            self.add_worker_to_pool()
+            return
+
         self.workers.put(wp)
 
     def run_task(self, fn, args, kwargs, timeout, fut: Future):
         try:
             worker: WorkerProcess = self.get_process()
             worker.submit_job((fn, args, kwargs, timeout))
             fut.pid = worker.pid
@@ -348,14 +354,20 @@
                         logger.debug(f"Unexpected exception from worker: {e}")
                         fut.set_exception(e)
                     else:
                         if isinstance(results, BaseException):
                             fut.set_exception(results)
                         else:
                             fut.set_result(results)
+
+                        if isinstance(results, TimeoutError):
+                            logger.debug(
+                                f"TimeoutError on {worker.pid}, setting ok=False"
+                            )
+                            worker.ok = False
                     finally:
                         break
                 elif not worker.is_alive():
                     logger.debug(f"p is no longer alive: {worker.process}")
                     try:
                         signame = signal.strsignal(-worker.process.exitcode)
                     except ValueError:  # pragma: no cover
@@ -515,15 +527,14 @@
     parent_pid,
     initializer,
     initargs,
     finitializer: Optional[Callable] = None,
     finitargs: Optional[Tuple] = None,
     mem_clear_threshold_bytes: Optional[int] = None,
 ):
-    logging.basicConfig(level=logging.DEBUG)
     proc = psutil.Process()
     pid = proc.pid
     lock = threading.Lock()
 
     def conn_send_safe(obj):
         try:
             with lock:
```

### Comparing `deadpool_executor-2023.7.1/examples/entrypoint.py` & `deadpool_executor-2023.7.2/examples/priorities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import random
 import time
 
 import deadpool
 
 
-def work():
+def work(symbol):
     time.sleep(random.random() * 4.0)
-    print(".", end="", flush=True)
+    print(symbol, end="", flush=True)
     return 1
 
 
 def main():
-    with deadpool.Deadpool() as exe:
-        futs = (exe.submit(work, deadpool_timeout=2.0) for _ in range(50))
+    with deadpool.Deadpool(max_backlog=100) as exe:
+        futs = []
+        for _ in range(25):
+            fut = exe.submit(work, ".", deadpool_timeout=2.0, deadpool_priority=10)
+            futs.append(fut)
+            fut = exe.submit(work, "!", deadpool_timeout=2.0, deadpool_priority=0)
+            futs.append(fut)
+
         for fut in deadpool.as_completed(futs):
             try:
                 assert fut.result() == 1
             except deadpool.TimeoutError:
                 print("x", end="", flush=True)
```

### Comparing `deadpool_executor-2023.7.1/noxfile.py` & `deadpool_executor-2023.7.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.1/pyproject.toml` & `deadpool_executor-2023.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.1/tests/test_deadpool.py` & `deadpool_executor-2023.7.2/tests/test_deadpool.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.1/PKG-INFO` & `deadpool_executor-2023.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpool-executor
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Deadpool
 Author-email: Caleb Hattingh <caleb.hattingh@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
@@ -53,32 +53,36 @@
     :alt: This project uses the "black" style formatter for Python code
     :target: https://github.com/python/black
 
 .. image:: https://api.securityscorecards.dev/projects/github.com/cjrh/deadpool/badge
     :alt: OpenSSF Scorecard
     :target: https://api.securityscorecards.dev/projects/github.com/cjrh/deadpool
 
-deadpool
-========
+
+Deadpool
+--------
 
 ``Deadpool`` is a process pool that is really hard to kill.
 
 ``Deadpool`` is an implementation of the ``Executor`` interface
 in the ``concurrent.futures`` standard library. ``Deadpool`` is
 a process pool executor, quite similar to the stdlib's
 `ProcessPoolExecutor`_.
 
 This document assumes that you are familiar with the stdlib
 `ProcessPoolExecutor`_. If you are not, it is important
 to understand that ``Deadpool`` makes very specific tradeoffs that
 can result in quite different behaviour to the stdlib
 implementation.
 
+.. sectnum::
+
 .. contents::
    :local:
+   :depth: 2
    :backlinks: entry
 
 Installation
 ------------
 
 The python package name is *deadpool-executor*, so to install
 you must type ``$ pip install deadpool-executor``. The import
@@ -98,59 +102,72 @@
 task, which the stdlib executor doesn't provide.
 
 You might wonder, isn't it bad to just kill a task like that?
 In my use-case, we had extensive logging and monitoring to alert
 us if any tasks failed; but it was paramount that our services
 continue to operate even when tasks got killed in OOM scenarios,
 or specific tasks took too long. This is the primary trade-off
-that ``Deadpool`` offers.
+that ``Deadpool`` offers: the pool will not break, but tasks
+can receive SIGKILL under certain conditions. This trade-off
+is likely fine if you've seen many OOMs break your pools.
 
 I also tried using the `Pebble <https://github.com/noxdafox/pebble>`_
 community process pool. This is a cool project, featuring several
 of the properties I've been looking for such as timeouts, and
 more resilient operation. However, during testing I found several
 occurrences of a mysterious `RuntimeError`_ that caused the Pebble
 pool to become broken and no longer accept new tasks.
 
-My goal with ``Deadpool`` is to make a process pool executor that
-is impossible to break. The tradeoffs are that I care less about:
-
-- being cross-platform
-- optimizing per-task latency
+My goal with ``Deadpool`` is that **the pool must never enter
+a broken state**. Any means by which that can happen will be
+considered a bug.
 
 What differs from `ProcessPoolExecutor`_?
 -----------------------------------------
 
 ``Deadpool`` is generally similar to `ProcessPoolExecutor`_ since it executes
 tasks in subprocesses, and implements the standard ``Executor`` abstract
-interface. However, it differs in the following ways:
+interface. We can draw a few comparisons to the stdlib pool to guide
+your decision process about whether this makes sense for your use-case:
 
-- ``Deadpool`` makes a new subprocess for every task submitted to
-  the pool (up to the ``max_workers`` limit). It is like having
-  ``max_tasks_per_child == 1`` (a new feature in
+- ``Deadpool`` precreates all subprocesses up to the pool size.
+- ``Deadpool`` also supports the
+  ``max_tasks_per_child`` parameter (a new feature in
   Python 3.11, although it was available in `multiprocessing.Pool`_
-  since Python 3.2). I have ideas about making this configurable, but
-  for now this is a much less important than overall resilience of
-  the pool. This also means that ``Deadpool`` doesn't suffer from
-  long-lived subprocesses being affected by memory leaks, usually
-  created by native extensions.
+  since Python 3.2).
+- ``Deadpool`` tasks can have priorities. When the executor chooses
+  the next pending task to schedule to a subprocess, it chooses the
+  pending task with the highest priority. This gives you a way of
+  prioritizing certain kinds of tasks. For example, you might give
+  UI-sensitive tasks a higher priority to deliver a more snappy
+  user experience to your users.
 - ``Deadpool`` defaults to the `forkserver <https://docs.python.org/3.11/library/multiprocessing.html#contexts-and-start-methods>`_ multiprocessing
   context, unlike the stdlib pool which defaults to ``fork`` on
   Linux. It's just a setting though, you can change it in the same way as
-  with the stdlib pool.
-- ``Deadpool`` does not keep a pool of processes around indefinitely.
-  There will only be as many concurrent processes running as there
-  is work to be done, up to the limit set by the ``max_workers``
-  parameter; but if there are fewer tasks to be executed, there will
-  be fewer active subprocesses. When there are no pending or active
-  tasks, there will be *no subprocesses present*. They are created
-  on demand as necessary and disappear when not required.
+  with the stdlib pool. Like the stdlib, I strongly advise you to avoid
+  using ``fork`` because propagation threads and locks via fork is
+  going to ruin your day eventually.
+- ``Deadpool`` can ask the system allocator (Linux only) to return
+  unused memory back to the OS based on exceeding a max threshold RSS.
+  For long-running pools and modern
+  kernels, the system memory allocator can hold onto unused memory
+  for a surprisingly long time, and coupled with bloat due to
+  memory fragmentation, this can result in carrying very large
+  RSS values in your pool. The ``max_tasks_per_child`` helps with
+  this because a subprocess is entirely erased when the max is
+  reached, but it does mean that periodically there will be a small
+  latency penalty from constructing the replacement subprocess. In
+  my opinion, ``max_tasks_per_child`` is appropriate for when you
+  know or suspect there's a real memory leak somewhere in your code
+  (or a 3rd-party package!), and the easiest way to deal with that
+  right now is just to periodically remove a process.
 - ``Deadpool`` tasks can have timeouts. When a task hits the timeout,
   the underlying subprocess in the pool is killed with ``SIGKILL``.
-  The entire process tree of that subprocess is killed.
+  The entire process tree of that subprocess is killed. Your application
+  logic needs to handle this. The ``finalizer`` will not run.
 - ``Deadpool`` tasks can have priorities. The priority is set in the
   ``submit()`` call. See the examples later in this document for further
   discussion on priorities.
 - The shutdown parameters ``wait`` and ``cancel_futures`` can behave
   differently to how they work in the _ProcessPoolExecutor. This is
   discussed in more detail later in this document.
 - If a ``Deadpool`` subprocess in the pool is killed by some
@@ -167,15 +184,16 @@
   Just like the ``initializer`` callable, the ``finalizer``
   callable is executed inside the subprocess. It is not guaranteed that
   the finalizer will always run. If a process is killed, e.g. due to a
   timeout or any other reason, the finalizer will not run. The finalizer
   could be used for things like flushing pending monitoring messages,
   such as traces and so on.
 - ``Deadpool`` currently only works on Linux. There isn't any specific
-  reason it can't work on other platforms.
+  reason it can't work on other platforms. The malloc trim feature also
+  requires a glibc system, so probably won't work on Alpine.
 
 Show me some code
 -----------------
 
 Simple case
 ^^^^^^^^^^^
 
@@ -242,24 +260,26 @@
         except deadpool.ProcessError:
             print("Oh no someone killed my task!")
 
 
 As long as the OOM killer terminates the subprocess (and not the main process),
 which is likely because it'll be your subprocess that is using too much
 memory, this will not hurt the pool, and it will be able to receive and
-process more tasks.
+process more tasks. Note that this event will show up as a ``ProcessError``
+exception when accessing the future, so you have a way of at least tracking
+these events.
 
 Design Details
 --------------
 
 Typical Example - with timeouts
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Here's a typical example of how code using Deadpool might look. The
-output of this code should be similar to the following:
+output of the code further below should be similar to the following:
 
 .. code-block:: bash
 
     $ python examples/entrypoint.py
     ...................xxxxxxxxxxx.xxxxxxx.x.xxxxxxx.x
     $
 
@@ -364,15 +384,15 @@
 - I also specified the ``max_backlog`` parameter when creating the
   Deadpool instance. This is discussed in more detail next, but quickly:
   task priority can only be enforced on what is in the submitted backlog
   of tasks, and the ``max_backlog`` parameter controls the depth of that
   queue. If ``max_backlog`` is too low, then the window of prioritization
   will not include tasks submitted later which might have higher priorities
   than earlier-submitted tasks. The ``submit`` call will in fact block
-  if the ``max_backlog`` depth has been reached.
+  once the ``max_backlog`` depth has been reached.
 
 Controlling the backlog of submitted tasks
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 By default, the ``max_backlog`` parameter is set to 5. This parameter is
 used to create the "submit queue" size. The submit queue is the place
 where submitted tasks are held before they are executed in background
@@ -449,14 +469,23 @@
         f = exe.submit(work)
 
         def cb(fut: deadpool.Future):
             print(f"My task is running on process {fut.pid}")
 
         f.add_pid_callback(cb)
 
+Obviously, both kinds of callbacks can be added:
+
+.. code-block:: python
+
+    with deadpool.Deadpool() as exe:
+        f = exe.submit(work)
+        f.add_pid_callback(lambda fut: f"Started on {fut.pid=}")
+        f.add_done_callback(lambda fut: f"Completed {fut.pid=}")
+
 More about shutdown
 ^^^^^^^^^^^^^^^^^^^
 
 In the documentation for ProcessPoolExecutor_, the following function
 signature is given for the shutdown_ method of the executor interface:
 
 .. code-block:: python
@@ -553,15 +582,51 @@
 
 To apply style fixes, and check for any remaining lints,
 
 .. code-block:: shell
 
    $ nox -t style
 
+docs
+^^^^
+
+The only docs currently are this README, which uses RST. Github 
+uses `docutils <https://docutils.sourceforge.io/docs/ref/rst/directives.html>`_
+to render RST.
+
+release
+^^^^^^^
+
+This project uses flit to release the package to pypi. The whole
+process isn't as automated as I would like, but this is what
+I currently do:
+
+1. Ensure that ``main`` branch is fully up to date with all to
+   be released, and all the tests succeed.
+2. Change the ``__version__`` field in ``deadpool.py``. Flit
+   uses this to stamp the version.
+3. Verify that ``flit build`` succeeds. This will produce a
+   wheel in the ``dist/`` directory. You can inspect this
+   wheel to ensure it contains only what is necessary. This
+   wheel will be what is uploaded to PyPI.
+4. **Commit the changed ``__version__``**. Easy to forget this
+   step, resulting in multiple awkward releases to try to
+   get the state all correct again.
+5. Now create the git tag and push to github:
+
+   .. code-block:: shell
+
+        $ git tag YYYY.MM.patch
+        $ git push --tags origin main
+
+6. Now deploy to PyPI:
+
+   .. code-block:: shell
 
+        $ flit publish
 
 
 .. _shutdown: https://docs.python.org/3/library/concurrent.futures.html?highlight=brokenprocesspool#concurrent.futures.Executor.shutdown
 .. _ProcessPoolExecutor: https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#processpoolexecutor
 .. _RuntimeError: https://github.com/noxdafox/pebble/issues/42#issuecomment-551245730
 .. _OOM killer: https://en.wikipedia.org/wiki/Out_of_memory#Out_of_memory_management
 .. _multiprocessing.Pool: https://docs.python.org/3.11/library/multiprocessing.html#multiprocessing.pool.Pool
```

