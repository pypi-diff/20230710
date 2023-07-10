# Comparing `tmp/xtor-0.4.0.tar.gz` & `tmp/xtor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtor-0.4.0.tar", max compression
+gzip compressed data, was "xtor-0.4.1.tar", max compression
```

## Comparing `xtor-0.4.0.tar` & `xtor-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1216 2023-07-01 22:45:48.270665 xtor-0.4.0/README.md
--rw-r--r--   0        0        0      685 2023-07-10 16:23:28.606873 xtor-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-07-10 16:23:36.210843 xtor-0.4.0/xtor/__init__.py
--rw-r--r--   0        0        0      901 2023-07-10 16:22:17.519132 xtor-0.4.0/xtor/cli.py
--rw-r--r--   0        0        0     5740 2023-07-10 16:22:38.299060 xtor-0.4.0/xtor/tor.py
--rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.4.0/xtor/utils.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 xtor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1216 2023-07-01 22:45:48.270665 xtor-0.4.1/README.md
+-rw-r--r--   0        0        0      685 2023-07-10 16:28:10.373529 xtor-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-07-10 16:28:17.673489 xtor-0.4.1/xtor/__init__.py
+-rw-r--r--   0        0        0      997 2023-07-10 16:26:30.862052 xtor-0.4.1/xtor/cli.py
+-rw-r--r--   0        0        0     5740 2023-07-10 16:22:38.299060 xtor-0.4.1/xtor/tor.py
+-rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.4.1/xtor/utils.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 xtor-0.4.1/PKG-INFO
```

### Comparing `xtor-0.4.0/README.md` & `xtor-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xtor-0.4.0/pyproject.toml` & `xtor-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtor"
-version = "0.4.0"
+version = "0.4.1"
 description = "Manage Tor instances"
 authors = ["khalidelborai <elboraikhalid@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/khalidelborai/xtor"
 license = "GNU Version 3"
 keywords = [
     "tor",
```

### Comparing `xtor-0.4.0/xtor/cli.py` & `xtor-0.4.1/xtor/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     port: int = typer.Option(9052, help="Port to listen on"),
     host: str = typer.Option("127.0.0.1", help="Host to listen on"),
     control_port: int = typer.Option(9053, help="Port to control tor"),
     password: str = typer.Option("password", help="Password to control tor"),
     own: bool = typer.Option(True, help="Own tor process"),
     path: str = typer.Option("tor", help="Path to tor binary"),
     countries: list = typer.Option([], help="Countries to use for tor"),
+    max_time: int = typer.Option(0, help="Max time to run tor"),
 ):
     """Start a tor server"""
-    tor = Tor.startTor(port=port, host=host, control_port=control_port, password=password, own=own, path=path, countries=countries)
+    tor = Tor.startTor(port=port, host=host, control_port=control_port, password=password, own=own, path=path, countries=countries,max_circuit_dirtiness=max_time)
     typer.echo(f"Tor started on {tor.host}:{tor.port}")
 
     if own:
         typer.pause(
             "Press any key to stop tor server. "
         )
```

### Comparing `xtor-0.4.0/xtor/tor.py` & `xtor-0.4.1/xtor/tor.py`

 * *Files identical despite different names*

### Comparing `xtor-0.4.0/xtor/utils.py` & `xtor-0.4.1/xtor/utils.py`

 * *Files identical despite different names*

### Comparing `xtor-0.4.0/PKG-INFO` & `xtor-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Manage Tor instances
 Home-page: https://github.com/khalidelborai/xtor
 License: GNU Version 3
 Keywords: tor,torrc,torrc manager,tor manager,tor instance,proxy
 Author: khalidelborai
 Author-email: elboraikhalid@gmail.com
 Requires-Python: >=3.7,<4.0
```

