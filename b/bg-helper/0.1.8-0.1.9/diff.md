# Comparing `tmp/bg_helper-0.1.8-py3-none-any.whl.zip` & `tmp/bg_helper-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 4671 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4449 b- defN 18-Dec-27 12:37 bg_helper/__init__.py
--rw-r--r--  2.0 unx      608 b- defN 18-Dec-27 12:41 bg_helper-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4360 b- defN 18-Dec-27 12:41 bg_helper-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 18-Dec-27 12:41 bg_helper-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 18-Dec-27 12:41 bg_helper-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      477 b- defN 18-Dec-27 12:41 bg_helper-0.1.8.dist-info/RECORD
-6 files, 9996 bytes uncompressed, 3805 bytes compressed:  61.9%
+Zip file size: 10369 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     4965 b- defN 20-Sep-28 01:21 bg_helper/__init__.py
+-rw-rw-r--  2.0 unx       38 b- defN 20-Aug-08 20:59 bg_helper/tools/__init__.py
+-rw-rw-r--  2.0 unx    16755 b- defN 20-Sep-28 01:21 bg_helper/tools/_docker.py
+-rw-rw-r--  2.0 unx      608 b- defN 20-Sep-28 06:15 bg_helper-0.1.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx    15272 b- defN 20-Sep-28 06:15 bg_helper-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 20-Sep-28 06:15 bg_helper-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 20-Sep-28 06:15 bg_helper-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      644 b- defN 20-Sep-28 06:15 bg_helper-0.1.9.dist-info/RECORD
+8 files, 38384 bytes uncompressed, 9245 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: bg_helper/__init__.py
 Comment: 
 
-Filename: bg_helper-0.1.8.dist-info/LICENSE.txt
+Filename: bg_helper/tools/__init__.py
 Comment: 
 
-Filename: bg_helper-0.1.8.dist-info/METADATA
+Filename: bg_helper/tools/_docker.py
 Comment: 
 
-Filename: bg_helper-0.1.8.dist-info/WHEEL
+Filename: bg_helper-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: bg_helper-0.1.8.dist-info/top_level.txt
+Filename: bg_helper-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: bg_helper-0.1.8.dist-info/RECORD
+Filename: bg_helper-0.1.9.dist-info/WHEEL
+Comment: 
+
+Filename: bg_helper-0.1.9.dist-info/top_level.txt
+Comment: 
+
+Filename: bg_helper-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bg_helper/__init__.py

```diff
@@ -58,20 +58,40 @@
         handler.baseFilename
         for handler in logger.handlers
         if hasattr(handler, 'baseFilename')
     ]
 
 
 def call_func(func, *args, **kwargs):
-    """Call a function and pass *args and **kwargs to it; return a dict
+    """Call a func with arbitrary args/kwargs and capture uncaught exceptions
 
     The following kwargs will be popped and used internally:
 
     - logger: logger object to use
-    - verbose: if True (default), print line separator and tracebacks when caught
+    - verbose: if True (default), print line separator & tracebacks when caught
+
+    The returned dict will always have at least the following keys:
+
+    - `func_name`
+    - `args`
+    - `kwargs`
+    - `status` (ok/error)
+
+    If the function call was successful, there will also be a `value` key. If
+    there was an uncaught exception, the following additional keys will be
+    provided in the return dict
+
+    - `error_type`
+    - `error_value`
+    - `fqdn`
+    - `func_doc`
+    - `func_module`
+    - `time_epoch`
+    - `time_string`
+    - `traceback_string`
     """
     _logger = kwargs.pop('logger', logger)
     verbose = kwargs.pop('verbose', True)
     try:
         _logfile = get_logger_filenames(_logger)[0]
     except IndexError:
         _logfile = None
@@ -146,7 +166,10 @@
         # Setup the daemonized thread and start running it
         thread = threading.Thread(target=self.run)
         thread.daemon = True
         thread.start()
 
     def run(self):
         call_func(self._func, *self._args, **self._kwargs)
+
+
+from bg_helper import tools
```

## Comparing `bg_helper-0.1.8.dist-info/LICENSE.txt` & `bg_helper-0.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

