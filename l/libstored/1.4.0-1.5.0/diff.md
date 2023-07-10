# Comparing `tmp/libstored-1.4.0.tar.gz` & `tmp/libstored-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libstored-1.4.0.tar", last modified: Thu Apr  6 20:53:42 2023, max compression
+gzip compressed data, was "libstored-1.5.0.tar", last modified: Mon Jul 10 07:12:24 2023, max compression
```

## Comparing `libstored-1.4.0.tar` & `libstored-1.5.0.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.558987 libstored-1.4.0/
--rw-r--r--   0 jochem     (501) staff       (20)    16727 2023-04-06 20:44:32.000000 libstored-1.4.0/LICENSE
--rw-r--r--   0 jochem     (501) staff       (20)        0 2023-04-06 20:44:32.000000 libstored-1.4.0/MANIFEST.in
--rw-r--r--   0 jochem     (501) staff       (20)     2178 2023-04-06 20:53:42.558625 libstored-1.4.0/PKG-INFO
--rw-r--r--   0 jochem     (501) staff       (20)     1562 2021-08-24 22:50:38.000000 libstored-1.4.0/README.md
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.548460 libstored-1.4.0/libstored/
--rw-r--r--   0 jochem     (501) staff       (20)      625 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/__init__.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.551070 libstored-1.4.0/libstored/cli/
--rw-r--r--   0 jochem     (501) staff       (20)        0 2021-08-24 22:50:38.000000 libstored-1.4.0/libstored/cli/__init__.py
--rw-r--r--   0 jochem     (501) staff       (20)     1402 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/cli/__main__.py
--rw-r--r--   0 jochem     (501) staff       (20)     6596 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/csv.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.554127 libstored-1.4.0/libstored/gui/
--rw-r--r--   0 jochem     (501) staff       (20)        0 2021-08-24 22:50:38.000000 libstored-1.4.0/libstored/gui/__init__.py
--rw-r--r--   0 jochem     (501) staff       (20)    17207 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/gui/__main__.py
--rw-r--r--   0 jochem     (501) staff       (20)    28055 2023-04-06 20:53:41.000000 libstored-1.4.0/libstored/gui/gui_qrc.py
--rw-r--r--   0 jochem     (501) staff       (20)    17238 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/protocol.py
--rw-r--r--   0 jochem     (501) staff       (20)     3285 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/serial2zmq.py
--rw-r--r--   0 jochem     (501) staff       (20)     2881 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/stdio2zmq.py
--rw-r--r--   0 jochem     (501) staff       (20)     4891 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/stream2zmq.py
--rw-r--r--   0 jochem     (501) staff       (20)      345 2023-04-06 20:46:30.000000 libstored-1.4.0/libstored/version.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.555659 libstored-1.4.0/libstored/visu/
--rw-r--r--   0 jochem     (501) staff       (20)        0 2021-08-24 22:50:38.000000 libstored-1.4.0/libstored/visu/__init__.py
--rw-r--r--   0 jochem     (501) staff       (20)     3636 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/visu/__main__.py
--rw-r--r--   0 jochem     (501) staff       (20)    10496 2023-04-06 20:53:41.000000 libstored-1.4.0/libstored/visu/visu_example.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.556048 libstored-1.4.0/libstored/wrapper/
--rw-r--r--   0 jochem     (501) staff       (20)        0 2021-08-24 22:50:38.000000 libstored-1.4.0/libstored/wrapper/__init__.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.556641 libstored-1.4.0/libstored/wrapper/serial/
--rw-r--r--   0 jochem     (501) staff       (20)        0 2021-08-24 22:50:38.000000 libstored-1.4.0/libstored/wrapper/serial/__init__.py
--rw-r--r--   0 jochem     (501) staff       (20)     1887 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/wrapper/serial/__main__.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.557903 libstored-1.4.0/libstored/wrapper/stdio/
--rw-r--r--   0 jochem     (501) staff       (20)        0 2021-08-24 22:50:38.000000 libstored-1.4.0/libstored/wrapper/stdio/__init__.py
--rw-r--r--   0 jochem     (501) staff       (20)     1515 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/wrapper/stdio/__main__.py
--rw-r--r--   0 jochem     (501) staff       (20)    65941 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/zmq_client.py
--rw-r--r--   0 jochem     (501) staff       (20)     4247 2023-04-06 20:44:32.000000 libstored-1.4.0/libstored/zmq_server.py
-drwxr-xr-x   0 jochem     (501) staff       (20)        0 2023-04-06 20:53:42.550427 libstored-1.4.0/libstored.egg-info/
--rw-r--r--   0 jochem     (501) staff       (20)     2178 2023-04-06 20:53:42.000000 libstored-1.4.0/libstored.egg-info/PKG-INFO
--rw-r--r--   0 jochem     (501) staff       (20)      793 2023-04-06 20:53:42.000000 libstored-1.4.0/libstored.egg-info/SOURCES.txt
--rw-r--r--   0 jochem     (501) staff       (20)        1 2023-04-06 20:53:42.000000 libstored-1.4.0/libstored.egg-info/dependency_links.txt
--rw-r--r--   0 jochem     (501) staff       (20)       77 2023-04-06 20:53:42.000000 libstored-1.4.0/libstored.egg-info/requires.txt
--rw-r--r--   0 jochem     (501) staff       (20)       14 2023-04-06 20:53:42.000000 libstored-1.4.0/libstored.egg-info/top_level.txt
--rw-r--r--   0 jochem     (501) staff       (20)       38 2023-04-06 20:53:42.559109 libstored-1.4.0/setup.cfg
--rw-r--r--   0 jochem     (501) staff       (20)     1564 2023-04-06 20:44:32.000000 libstored-1.4.0/setup.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)    16727 2022-10-20 11:21:51.000000 libstored-1.5.0/LICENSE
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2022-03-28 13:51:58.000000 libstored-1.5.0/MANIFEST.in
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     2399 2023-07-10 07:12:24.486424 libstored-1.5.0/PKG-INFO
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     1783 2023-07-10 07:11:39.000000 libstored-1.5.0/README.md
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.482424 libstored-1.5.0/libstored/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)      625 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/__init__.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/cli/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2021-09-16 07:22:32.000000 libstored-1.5.0/libstored/cli/__init__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     1425 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/cli/__main__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     7917 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/csv.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/gui/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2021-09-16 07:22:32.000000 libstored-1.5.0/libstored/gui/__init__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)    17394 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/gui/__main__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)    28093 2023-07-10 07:11:58.000000 libstored-1.5.0/libstored/gui/gui_qrc.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/log/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/log/__init__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     4306 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/log/__main__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)    17238 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/protocol.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     3285 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/serial2zmq.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     2920 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/stdio2zmq.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     4891 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/stream2zmq.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)      345 2023-07-07 09:25:23.000000 libstored-1.5.0/libstored/version.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/visu/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2021-09-16 07:22:32.000000 libstored-1.5.0/libstored/visu/__init__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     3678 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/visu/__main__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)    10519 2023-07-10 07:11:58.000000 libstored-1.5.0/libstored/visu/visu_example.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/wrapper/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2021-09-16 07:22:32.000000 libstored-1.5.0/libstored/wrapper/__init__.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/wrapper/serial/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2021-09-16 07:22:32.000000 libstored-1.5.0/libstored/wrapper/serial/__init__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     1909 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/wrapper/serial/__main__.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored/wrapper/stdio/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        0 2021-09-16 07:22:32.000000 libstored-1.5.0/libstored/wrapper/stdio/__init__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     1538 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/wrapper/stdio/__main__.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)    66386 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/zmq_client.py
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     4247 2023-07-10 07:11:39.000000 libstored-1.5.0/libstored/zmq_server.py
+drwxrwxr-x   0 jrt       (1000) jrt       (1000)        0 2023-07-10 07:12:24.486424 libstored-1.5.0/libstored.egg-info/
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     2399 2023-07-10 07:12:24.000000 libstored-1.5.0/libstored.egg-info/PKG-INFO
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)      909 2023-07-10 07:12:24.000000 libstored-1.5.0/libstored.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        1 2023-07-10 07:12:24.000000 libstored-1.5.0/libstored.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)      341 2023-07-10 07:12:24.000000 libstored-1.5.0/libstored.egg-info/entry_points.txt
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)       77 2023-07-10 07:12:24.000000 libstored-1.5.0/libstored.egg-info/requires.txt
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)       10 2023-07-10 07:12:24.000000 libstored-1.5.0/libstored.egg-info/top_level.txt
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)       94 2023-07-10 07:11:39.000000 libstored-1.5.0/pyproject.toml
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)     1183 2023-07-10 07:12:24.486424 libstored-1.5.0/setup.cfg
+-rw-rw-r--   0 jrt       (1000) jrt       (1000)        6 2023-07-07 09:25:23.000000 libstored-1.5.0/version.txt
```

### Comparing `libstored-1.4.0/LICENSE` & `libstored-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libstored-1.4.0/PKG-INFO` & `libstored-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libstored
-Version: 1.4.0
+Version: 1.5.0
 Summary: Embedded Debugger client for libstored's debug protocol
 Home-page: https://github.com/DEMCON/libstored
 Author: Jochem Rutgers
 Author-email: jochem.rutgers@demcon.com
 License: MPLv2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -38,14 +38,17 @@
 - `libstored.cli`: a command line interface that connects to a debug target.
 - `libstored.wrapper.stdio`: a stdin/stdout wrapper, which is a bridge between
   Embedded Debugger messages within the stdin/stdout streams of the application
   to a ZeroMQ socket interface, which in turn can be used to connect
   `libstored.gui` or `libstored.cli` to.
 - `libstored.wrapper.serial`: like `libstored.wrapper.stdio`, but using
   `pyserial` instead of stdin/stdout.
+- `libstored.log`: command line tool that connects to a debug target and logs
+  samples to CSV.  It is equivalent to passing `-f` to `libstored.gui`, but
+  this tool allows easier automation of a specific set of samples.
 
 ## Interesting classes
 
 The following classes are particularly interesting:
 
 - `libstored.ZmqClient`
 - `libstored.ZmqServer`
```

### Comparing `libstored-1.4.0/README.md` & `libstored-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 - `libstored.cli`: a command line interface that connects to a debug target.
 - `libstored.wrapper.stdio`: a stdin/stdout wrapper, which is a bridge between
   Embedded Debugger messages within the stdin/stdout streams of the application
   to a ZeroMQ socket interface, which in turn can be used to connect
   `libstored.gui` or `libstored.cli` to.
 - `libstored.wrapper.serial`: like `libstored.wrapper.stdio`, but using
   `pyserial` instead of stdin/stdout.
+- `libstored.log`: command line tool that connects to a debug target and logs
+  samples to CSV.  It is equivalent to passing `-f` to `libstored.gui`, but
+  this tool allows easier automation of a specific set of samples.
 
 ## Interesting classes
 
 The following classes are particularly interesting:
 
 - `libstored.ZmqClient`
 - `libstored.ZmqServer`
```

### Comparing `libstored-1.4.0/libstored/__init__.py` & `libstored-1.5.0/libstored/__init__.py`

 * *Files identical despite different names*

### Comparing `libstored-1.4.0/libstored/cli/__main__.py` & `libstored-1.5.0/libstored/cli/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys
 import argparse
 import logging
 
 from ..zmq_client import ZmqClient
 from ..zmq_server import ZmqServer
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser(description='ZMQ command line client')
     parser.add_argument('-s', dest='server', type=str, default='localhost', help='ZMQ server to connect to')
     parser.add_argument('-p', dest='port', type=int, default=ZmqServer.default_port, help='port')
     parser.add_argument('-v', dest='verbose', default=False, help='Enable verbose output', action='store_true')
 
     args = parser.parse_args()
 
@@ -39,7 +39,9 @@
             sys.stdout.flush()
 
     except KeyboardInterrupt:
         pass
 
     client.close()
 
+if __name__ == '__main__':
+    main()
```

### Comparing `libstored-1.4.0/libstored/gui/__main__.py` & `libstored-1.5.0/libstored/gui/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,21 @@
 
     def _remove(self, o):
         if o not in self._data:
             return
 
         data = self._data[o]
         QObject.disconnect(data.connection)
-        self._ax.lines.remove(data.line)
+        try:
+            self._ax.lines.remove(data.line)
+        except AttributeError:
+            # This is a newer MPL, apparently.
+            data.line.remove()
+            pass
+
         del self._data[o]
 
         if len(self._data) > 0:
             self.update_legend()
         else:
             self.plottingChanged.emit()
             self._timer.stop()
@@ -480,15 +486,17 @@
 
 def signal_handler(sig, stk, app):
     app.exit(1)
     signal.signal(sig, signal.SIG_DFL)
 
 
 
-if __name__ == '__main__':
+def main():
+    global logger
+
     logger = logging.getLogger('gui')
     qInstallMessageHandler(msgHandler)
 
     QCoreApplication.setApplicationName("Embedded Debugger")
     QCoreApplication.setApplicationVersion(__version__)
     try:
         QGuiApplication.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
@@ -592,7 +600,10 @@
     logger.info('Exiting...')
 
     client.saveState()
     client.close()
     gc.collect()
 
     sys.exit(res)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `libstored-1.4.0/libstored/gui/gui_qrc.py` & `libstored-1.5.0/libstored/gui/gui_qrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.5.0
+# Created by: The Resource Compiler for Qt version 6.5.1
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x04\xc3\
 /\
@@ -742,15 +742,15 @@
 odule Libstored.\
 Components\x0aInput\
  1.0 Input.qml\x0aM\
 easurement 1.0 M\
 easurement.qml\x0aS\
 toreObject 1.0 S\
 toreObject.qml\x0a\
-\x00\x00\x06\xb3\
+\x00\x00\x06\xbb\
 /\
 *\x0a * libstored, \
 distributed debu\
 ggable data stor\
 es.\x0a * Copyright\
  (C) 2020-2023  \
 Jochem Rutgers\x0a \
@@ -794,72 +794,72 @@
  {\x0a            o\
 bj = client.obj(\
 ref)\x0a        }\x0a \
    }\x0a\x0a    onObjC\
 hanged: {\x0a      \
   if(obj) {\x0a    \
         value = \
-obj.value\x0a\x0a     \
-       if(!obj.p\
-olling) {\x0a      \
-          if(pol\
-lInterval > 0)\x0a \
-                \
-   obj.poll(poll\
-Interval)\x0a      \
-          else i\
-f(autoReadOnInit\
-)\x0a              \
-      obj.asyncR\
-ead()\x0a          \
-  } else if(poll\
-Interval > 0 && \
-obj.pollInterval\
- > pollInterval)\
- {\x0a             \
-   // Prefer the\
- faster setting,\
- if there are mu\
-ltiple.\x0a        \
-        obj.poll\
-(pollInterval)\x0a \
-           }\x0a   \
-     } else {\x0a  \
-          value \
-= null\x0a        }\
-\x0a    }\x0a\x0a    prop\
-erty string valu\
-eString: obj ? o\
-bj.valueString :\
- ''\x0a    property\
- var value: null\
-\x0a\x0a    property b\
-ool refreshed: f\
-alse\x0a\x0a    Timer \
-{\x0a        id: up\
-datedTimer\x0a     \
-   interval: 110\
-0\x0a        onTrig\
-gered: comp.refr\
-eshed = false\x0a  \
-  }\x0a\x0a    onValue\
-StringChanged: {\
-\x0a        if(obj)\
-\x0a            val\
-ue = obj.value\x0a\x0a\
-        comp.ref\
-reshed = true\x0a  \
-      updatedTim\
-er.restart()\x0a   \
- }\x0a\x0a    function\
- set(x) {\x0a      \
-  if(obj)\x0a      \
-      obj.valueS\
-tring = x\x0a    }\x0a\
-}\x0a\
+obj.valueSafe\x0a\x0a \
+           if(!o\
+bj.polling) {\x0a  \
+              if\
+(pollInterval > \
+0)\x0a             \
+       obj.poll(\
+pollInterval)\x0a  \
+              el\
+se if(autoReadOn\
+Init)\x0a          \
+          obj.as\
+yncRead()\x0a      \
+      } else if(\
+pollInterval > 0\
+ && obj.pollInte\
+rval > pollInter\
+val) {\x0a         \
+       // Prefer\
+ the faster sett\
+ing, if there ar\
+e multiple.\x0a    \
+            obj.\
+poll(pollInterva\
+l)\x0a            }\
+\x0a        } else \
+{\x0a            va\
+lue = null\x0a     \
+   }\x0a    }\x0a\x0a    \
+property string \
+valueString: obj\
+ ? obj.valueStri\
+ng : ''\x0a    prop\
+erty var value: \
+null\x0a\x0a    proper\
+ty bool refreshe\
+d: false\x0a\x0a    Ti\
+mer {\x0a        id\
+: updatedTimer\x0a \
+       interval:\
+ 1100\x0a        on\
+Triggered: comp.\
+refreshed = fals\
+e\x0a    }\x0a\x0a    onV\
+alueStringChange\
+d: {\x0a        if(\
+obj)\x0a           \
+ value = obj.val\
+ueSafe\x0a\x0a        \
+comp.refreshed =\
+ true\x0a        up\
+datedTimer.resta\
+rt()\x0a    }\x0a\x0a    \
+function set(x) \
+{\x0a        if(obj\
+)\x0a            ob\
+j.valueString = \
+x\x0a    }\x0a}\x0a\
 "
 
 qt_resource_name = b"\
 \x00\x0c\
 \x00V'\xdc\
 \x00C\
 \x00h\x00e\x00c\x00k\x00B\x00o\x00x\x00.\x00q\x00m\x00l\
@@ -911,37 +911,37 @@
 \x00t\x00o\x00r\x00e\x00O\x00b\x00j\x00e\x00c\x00t\x00.\x00q\x00m\x00l\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x07\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x87XPW\x17\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x04\xc7\
-\x00\x00\x01\x87XPW\x18\
+\x00\x00\x01\x7f\xd0\xcc7s\
 \x00\x00\x00\x80\x00\x01\x00\x00\x00\x01\x00\x00\x0dy\
-\x00\x00\x01\x87XPW\x17\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\xd4\x00\x01\x00\x00\x00\x01\x00\x00\x16\x0e\
-\x00\x00\x01\x87XPW\x18\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\xbc\x00\x02\x00\x00\x00\x01\x00\x00\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00f\x00\x00\x00\x00\x00\x01\x00\x00\x08\x01\
-\x00\x00\x01\x87XPW\x17\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x13\x90\
-\x00\x00\x01\x87XPW\x17\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\xea\x00\x02\x00\x00\x00\x04\x00\x00\x00\x09\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x01R\x00\x00\x00\x00\x00\x01\x00\x00,\xf3\
-\x00\x00\x01\x87XPW\x1a\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x01@\x00\x00\x00\x00\x00\x01\x00\x00,\x7f\
-\x00\x00\x01\x87XPW\x1a\
+\x00\x00\x01\x7f\xd0\xcc7s\
 \x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00&\x1d\
-\x00\x00\x01\x87XPW\x19\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x01\x04\x00\x00\x00\x00\x00\x01\x00\x00\x1f\xd8\
-\x00\x00\x01\x87XPW\x1a\
+\x00\x00\x01\x89>\xa4A\x13\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `libstored-1.4.0/libstored/protocol.py` & `libstored-1.5.0/libstored/protocol.py`

 * *Files identical despite different names*

### Comparing `libstored-1.4.0/libstored/serial2zmq.py` & `libstored-1.5.0/libstored/serial2zmq.py`

 * *Files identical despite different names*

### Comparing `libstored-1.4.0/libstored/stdio2zmq.py` & `libstored-1.5.0/libstored/stdio2zmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """A stdin/stdout frame grabber to ZmqServer bridge."""
 
     def __init__(self, args, stack='ascii,term', listen='*', port=Stream2Zmq.default_port, **kwargs):
         super().__init__(stack=stack, listen=listen, port=port)
         self.process = subprocess.Popen(
             args=args, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
             preexec_fn = set_pdeathsig() if os.name == 'posix' else None,
-            shell=not os.path.exists(args),
+            shell=not os.path.exists(args[0] if isinstance(args, list) else args),
             **kwargs)
         self.stdout_socket = self.registerStream(self.process.stdout)
         self.stdin_socket = self.registerStream(sys.stdin)
         self.rep_queue = []
 
     def poll(self, timeout_s = None):
         # We need to check if the process still runs once in a while.
```

### Comparing `libstored-1.4.0/libstored/stream2zmq.py` & `libstored-1.5.0/libstored/stream2zmq.py`

 * *Files identical despite different names*

### Comparing `libstored-1.4.0/libstored/visu/__main__.py` & `libstored-1.5.0/libstored/visu/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     elif msgType == QtMsgType.QtWarningMsg:
         logger.warning(msg)
     elif msgType == QtMsgType.QtCriticalMsg:
         logger.error(msg)
     else:
         logger.critical(msg)
 
-if __name__ == '__main__':
+def main():
+    global logger
+
     logger = logging.getLogger('visu')
     qInstallMessageHandler(msgHandler)
 
     QCoreApplication.setApplicationName("Embedded Debugger visu")
 
     parser = argparse.ArgumentParser(description='ZMQ visu', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-s', dest='server', type=str, default='localhost', help='ZMQ server to connect to')
@@ -94,7 +96,9 @@
     if not engine.rootObjects():
         sys.exit(-1)
 
     res = app.exec()
     client.close()
     sys.exit(res)
 
+if __name__ == '__main__':
+    main()
```

### Comparing `libstored-1.4.0/libstored/visu/visu_example.py` & `libstored-1.5.0/libstored/visu/visu_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.5.0
+# Created by: The Resource Compiler for Qt version 6.5.1
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x06\xbc\
 /\
@@ -328,15 +328,15 @@
 odule Libstored.\
 Components\x0aInput\
  1.0 Input.qml\x0aM\
 easurement 1.0 M\
 easurement.qml\x0aS\
 toreObject 1.0 S\
 toreObject.qml\x0a\
-\x00\x00\x06\xb3\
+\x00\x00\x06\xbb\
 /\
 *\x0a * libstored, \
 distributed debu\
 ggable data stor\
 es.\x0a * Copyright\
  (C) 2020-2023  \
 Jochem Rutgers\x0a \
@@ -380,72 +380,72 @@
  {\x0a            o\
 bj = client.obj(\
 ref)\x0a        }\x0a \
    }\x0a\x0a    onObjC\
 hanged: {\x0a      \
   if(obj) {\x0a    \
         value = \
-obj.value\x0a\x0a     \
-       if(!obj.p\
-olling) {\x0a      \
-          if(pol\
-lInterval > 0)\x0a \
-                \
-   obj.poll(poll\
-Interval)\x0a      \
-          else i\
-f(autoReadOnInit\
-)\x0a              \
-      obj.asyncR\
-ead()\x0a          \
-  } else if(poll\
-Interval > 0 && \
-obj.pollInterval\
- > pollInterval)\
- {\x0a             \
-   // Prefer the\
- faster setting,\
- if there are mu\
-ltiple.\x0a        \
-        obj.poll\
-(pollInterval)\x0a \
-           }\x0a   \
-     } else {\x0a  \
-          value \
-= null\x0a        }\
-\x0a    }\x0a\x0a    prop\
-erty string valu\
-eString: obj ? o\
-bj.valueString :\
- ''\x0a    property\
- var value: null\
-\x0a\x0a    property b\
-ool refreshed: f\
-alse\x0a\x0a    Timer \
-{\x0a        id: up\
-datedTimer\x0a     \
-   interval: 110\
-0\x0a        onTrig\
-gered: comp.refr\
-eshed = false\x0a  \
-  }\x0a\x0a    onValue\
-StringChanged: {\
-\x0a        if(obj)\
-\x0a            val\
-ue = obj.value\x0a\x0a\
-        comp.ref\
-reshed = true\x0a  \
-      updatedTim\
-er.restart()\x0a   \
- }\x0a\x0a    function\
- set(x) {\x0a      \
-  if(obj)\x0a      \
-      obj.valueS\
-tring = x\x0a    }\x0a\
-}\x0a\
+obj.valueSafe\x0a\x0a \
+           if(!o\
+bj.polling) {\x0a  \
+              if\
+(pollInterval > \
+0)\x0a             \
+       obj.poll(\
+pollInterval)\x0a  \
+              el\
+se if(autoReadOn\
+Init)\x0a          \
+          obj.as\
+yncRead()\x0a      \
+      } else if(\
+pollInterval > 0\
+ && obj.pollInte\
+rval > pollInter\
+val) {\x0a         \
+       // Prefer\
+ the faster sett\
+ing, if there ar\
+e multiple.\x0a    \
+            obj.\
+poll(pollInterva\
+l)\x0a            }\
+\x0a        } else \
+{\x0a            va\
+lue = null\x0a     \
+   }\x0a    }\x0a\x0a    \
+property string \
+valueString: obj\
+ ? obj.valueStri\
+ng : ''\x0a    prop\
+erty var value: \
+null\x0a\x0a    proper\
+ty bool refreshe\
+d: false\x0a\x0a    Ti\
+mer {\x0a        id\
+: updatedTimer\x0a \
+       interval:\
+ 1100\x0a        on\
+Triggered: comp.\
+refreshed = fals\
+e\x0a    }\x0a\x0a    onV\
+alueStringChange\
+d: {\x0a        if(\
+obj)\x0a           \
+ value = obj.val\
+ueSafe\x0a\x0a        \
+comp.refreshed =\
+ true\x0a        up\
+datedTimer.resta\
+rt()\x0a    }\x0a\x0a    \
+function set(x) \
+{\x0a        if(obj\
+)\x0a            ob\
+j.valueString = \
+x\x0a    }\x0a}\x0a\
 "
 
 qt_resource_name = b"\
 \x00\x09\
 \x09\xab\xcdT\
 \x00L\
 \x00i\x00b\x00s\x00t\x00o\x00r\x00e\x00d\
@@ -475,27 +475,27 @@
 \x00t\x00o\x00r\x00e\x00O\x00b\x00j\x00e\x00c\x00t\x00.\x00q\x00m\x00l\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x18\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x87XPW\x19\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x03\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00.\x00\x02\x00\x00\x00\x04\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x96\x00\x00\x00\x00\x00\x01\x00\x00\x13\xdb\
-\x00\x00\x01\x87XPW\x1a\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00\x84\x00\x00\x00\x00\x00\x01\x00\x00\x13g\
-\x00\x00\x01\x87XPW\x1a\
+\x00\x00\x01\x7f\xd0\xcc7s\
 \x00\x00\x00l\x00\x00\x00\x00\x00\x01\x00\x00\x0d\x05\
-\x00\x00\x01\x87XPW\x19\
+\x00\x00\x01\x89>\xa4A\x13\
 \x00\x00\x00H\x00\x00\x00\x00\x00\x01\x00\x00\x06\xc0\
-\x00\x00\x01\x87XPW\x1a\
+\x00\x00\x01\x89>\xa4A\x13\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `libstored-1.4.0/libstored/wrapper/serial/__main__.py` & `libstored-1.5.0/libstored/wrapper/serial/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import re
 import serial
 
 from ...zmq_server import ZmqServer
 from ...serial2zmq import Serial2Zmq
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser(description='serial wrapper to ZMQ server',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-l', dest='zmqlisten', type=str, default='*', help='ZMQ listen address')
     parser.add_argument('-p', dest='zmqport', type=int, default=ZmqServer.default_port, help='ZMQ port')
     parser.add_argument('port', help='serial port')
     parser.add_argument('baud', nargs='?', type=int, default=115200, help='baud rate')
     parser.add_argument('-r', dest='rtscts', default=False, help='RTS/CTS flow control', action='store_true')
@@ -39,8 +39,9 @@
         while True:
             bridge.poll()
     except KeyboardInterrupt:
         pass
 
     bridge.close()
 
-
+if __name__ == '__main__':
+    main()
```

### Comparing `libstored-1.4.0/libstored/wrapper/stdio/__main__.py` & `libstored-1.5.0/libstored/wrapper/stdio/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import argparse
 import logging
 import re
 
 from ...zmq_server import ZmqServer
 from ...stdio2zmq import Stdio2Zmq
 
-if __name__ == '__main__':
+def main():
     parser = argparse.ArgumentParser(description='stdin/stdout wrapper to ZMQ server',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-l', dest='listen', type=str, default='*', help='listen address')
     parser.add_argument('-p', dest='port', type=int, default=ZmqServer.default_port, help='port')
     parser.add_argument('-S', dest='stack', type=str, default='ascii,pubterm', help='protocol stack')
     parser.add_argument('-v', dest='verbose', default=False, help='Enable verbose output', action='store_true')
     parser.add_argument('command')
@@ -36,7 +36,9 @@
         while True:
             bridge.poll()
     except KeyboardInterrupt:
         pass
 
     bridge.close()
 
+if __name__ == '__main__':
+    main()
```

### Comparing `libstored-1.4.0/libstored/zmq_client.py` & `libstored-1.5.0/libstored/zmq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,20 +300,20 @@
         return res
 
     def _decode(self, rep):
         dtype = self._type & ~self.FlagFunction
         try:
             if self.isFixed():
                 binint = int(rep.decode(), 16)
-                if sys.version_info.major <= 3 and sys.version_info.minor < 9:
-                    # If binint >= 2^63 for Uint64, we run into problems in libshiboken.
-                    # See https://bugreports.qt.io/browse/PYSIDE-648
-                    # Force to Int64 in that case.
-                    if binint >= 1 << 63:
-                        binint -= 1 << 64
+                # If binint >= 2^63 for Uint64, we run into problems in libshiboken.
+                # See https://bugreports.qt.io/browse/PYSIDE-648
+                # Force to Int64 in that case.
+#                if binint >= 1 << 63:
+#                    binint -= 1 << 64
+
                 if self.isInt() and not self.isSigned():
                     return binint
                 elif dtype == self.Int8:
                     return self.sign_extend(binint, 8)
                 elif dtype == self.Int16:
                     return self.sign_extend(binint, 16)
                 elif dtype == self.Int32:
@@ -525,27 +525,41 @@
             }.get(self._type & ~self.FlagFunction, lambda x: x)(value)
         return value
 
     # Returns the currently known value (without an actual read())
     def _value_get(self):
         return self._value
 
+    def _value_getSafe(self):
+        value = self._value_get()
+
+        if value is not None:
+            if self._type & self.FlagInt:
+                # If value >= 2^63 for Uint64, we run into problems in
+                # libshiboken.  See https://bugreports.qt.io/browse/PYSIDE-648
+                # Force to Int64 in that case.
+                if value >= 1 << 63:
+                    value = (value % (1 << 64)) - (1 << 64)
+
+        return value
+
     # Writes the value to the server.
     def _value_set(self, v):
         try:
             v = self.interpret(v)
             if self._client and self._client.useEventLoop:
                 self.asyncWrite(v)
                 return True
             else:
                 return self.write(v)
         except ValueError:
             return False
 
     value = _Property('QVariant', _value_get, _value_set, notify=valueChanged)
+    valueSafe = _Property('QVariant', _value_getSafe, _value_set, notify=valueChanged)
 
     def _valueString_get(self):
         v = self._value
         if v is None:
             return ""
         else:
             try:
```

### Comparing `libstored-1.4.0/libstored/zmq_server.py` & `libstored-1.5.0/libstored/zmq_server.py`

 * *Files identical despite different names*

### Comparing `libstored-1.4.0/libstored.egg-info/PKG-INFO` & `libstored-1.5.0/libstored.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libstored
-Version: 1.4.0
+Version: 1.5.0
 Summary: Embedded Debugger client for libstored's debug protocol
 Home-page: https://github.com/DEMCON/libstored
 Author: Jochem Rutgers
 Author-email: jochem.rutgers@demcon.com
 License: MPLv2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -38,14 +38,17 @@
 - `libstored.cli`: a command line interface that connects to a debug target.
 - `libstored.wrapper.stdio`: a stdin/stdout wrapper, which is a bridge between
   Embedded Debugger messages within the stdin/stdout streams of the application
   to a ZeroMQ socket interface, which in turn can be used to connect
   `libstored.gui` or `libstored.cli` to.
 - `libstored.wrapper.serial`: like `libstored.wrapper.stdio`, but using
   `pyserial` instead of stdin/stdout.
+- `libstored.log`: command line tool that connects to a debug target and logs
+  samples to CSV.  It is equivalent to passing `-f` to `libstored.gui`, but
+  this tool allows easier automation of a specific set of samples.
 
 ## Interesting classes
 
 The following classes are particularly interesting:
 
 - `libstored.ZmqClient`
 - `libstored.ZmqServer`
```

### Comparing `libstored-1.4.0/libstored.egg-info/SOURCES.txt` & `libstored-1.5.0/libstored.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+setup.cfg
+version.txt
 libstored/__init__.py
 libstored/csv.py
 libstored/protocol.py
 libstored/serial2zmq.py
 libstored/stdio2zmq.py
 libstored/stream2zmq.py
 libstored/version.py
 libstored/zmq_client.py
 libstored/zmq_server.py
 libstored.egg-info/PKG-INFO
 libstored.egg-info/SOURCES.txt
 libstored.egg-info/dependency_links.txt
+libstored.egg-info/entry_points.txt
 libstored.egg-info/requires.txt
 libstored.egg-info/top_level.txt
 libstored/cli/__init__.py
 libstored/cli/__main__.py
 libstored/gui/__init__.py
 libstored/gui/__main__.py
 libstored/gui/gui_qrc.py
+libstored/log/__init__.py
+libstored/log/__main__.py
 libstored/visu/__init__.py
 libstored/visu/__main__.py
 libstored/visu/visu_example.py
 libstored/wrapper/__init__.py
 libstored/wrapper/serial/__init__.py
 libstored/wrapper/serial/__main__.py
 libstored/wrapper/stdio/__init__.py
```

### Comparing `libstored-1.4.0/setup.py` & `libstored-1.5.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,44 @@
-#!/usr/bin/env python3
-
-import os
-import re
-import setuptools
-import sys
-import libstored
-
-here = os.path.dirname(os.path.realpath(__file__))
-
-with open(os.path.join(here, "README.md"), "r") as fh:
-    long_description = fh.read()
-
-packages = setuptools.find_packages(here)
-packages += list(map(lambda p: re.sub(r'^libstored\b', 'ed2', p), packages))
-package_data = [
-]
-
-setuptools.setup(
-    name = 'libstored',
-    version = libstored.__version__,
-    description = 'Embedded Debugger client for libstored\'s debug protocol',
-    author = 'Jochem Rutgers',
-    author_email = 'jochem.rutgers@demcon.com',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url = 'https://github.com/DEMCON/libstored',
-    license = 'MPLv2.0',
-    packages = packages,
-    package_dir = {'libstored': 'libstored', 'ed2': 'libstored'},
-    package_data = {'libstored': package_data, 'ed2': package_data},
-    install_requires = [
-        'PySide6',
-        'pyserial',
-        'argparse',
-        'pyzmq',
-        'crcmod',
-        'natsort',
-        'heatshrink2',
-        'matplotlib>=3.5.0', # PySide6 support starts from 3.5.0
-#        'lognplot', # optional
-    ],
-    python_requires='>=3.6',
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Debuggers",
-        "Topic :: Software Development :: Embedded Systems",
-    ],
-    include_package_data=True,
-)
+[metadata]
+name = libstored
+version = file: version.txt
+description = Embedded Debugger client for libstored's debug protocol
+author = Jochem Rutgers
+author_email = jochem.rutgers@demcon.com
+url = https://github.com/DEMCON/libstored
+long_description = file: README.md
+long_description_content_type = text/markdown
+license = MPLv2.0
+classifiers = 
+	Programming Language :: Python :: 3
+	License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+	Intended Audience :: Developers
+	Topic :: Software Development :: Debuggers
+	Topic :: Software Development :: Embedded Systems
+
+[options]
+python_requires = >=3.6
+packages = find:
+install_requires = 
+	PySide6
+	pyserial
+	argparse
+	pyzmq
+	crcmod
+	natsort
+	heatshrink2
+	matplotlib >= 3.5.0 # PySide6 support starts from 3.5.0
+
+[options.entry_points]
+console_scripts = 
+	libstored-cli = libstored.cli.__main__:main
+	libstored-log = libstored.log.__main__:main
+	libstored-wrapper-serial = libstored.wrapper.serial.__main__:main
+	libstored-wrapper-stdio = libstored.wrapper.stdio.__main__:main
+gui_scripts = 
+	libstored-gui = libstored.gui.__main__:main
+	libstored-visu = libstored.visu.__main__:main
+
+[egg_info]
+tag_build = 
+tag_date = 0
```

