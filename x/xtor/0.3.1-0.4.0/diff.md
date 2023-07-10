# Comparing `tmp/xtor-0.3.1.tar.gz` & `tmp/xtor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtor-0.3.1.tar", max compression
+gzip compressed data, was "xtor-0.4.0.tar", max compression
```

## Comparing `xtor-0.3.1.tar` & `xtor-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1216 2023-07-01 22:45:48.270665 xtor-0.3.1/README.md
--rw-r--r--   0        0        0      685 2023-07-01 22:45:10.749672 xtor-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       67 2023-07-01 22:45:07.066969 xtor-0.3.1/xtor/__init__.py
--rw-r--r--   0        0        0      807 2023-06-30 12:47:55.419073 xtor-0.3.1/xtor/cli.py
--rw-r--r--   0        0        0     5380 2023-07-01 22:44:59.450642 xtor-0.3.1/xtor/tor.py
--rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.3.1/xtor/utils.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 xtor-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1216 2023-07-01 22:45:48.270665 xtor-0.4.0/README.md
+-rw-r--r--   0        0        0      685 2023-07-10 16:23:28.606873 xtor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-07-10 16:23:36.210843 xtor-0.4.0/xtor/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-10 16:22:17.519132 xtor-0.4.0/xtor/cli.py
+-rw-r--r--   0        0        0     5740 2023-07-10 16:22:38.299060 xtor-0.4.0/xtor/tor.py
+-rw-r--r--   0        0        0     1844 2023-06-28 16:26:22.537395 xtor-0.4.0/xtor/utils.py
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 xtor-0.4.0/PKG-INFO
```

### Comparing `xtor-0.3.1/README.md` & `xtor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xtor-0.3.1/pyproject.toml` & `xtor-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtor"
-version = "0.3.1"
+version = "0.4.0"
 description = "Manage Tor instances"
 authors = ["khalidelborai <elboraikhalid@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/khalidelborai/xtor"
 license = "GNU Version 3"
 keywords = [
     "tor",
```

### Comparing `xtor-0.3.1/xtor/cli.py` & `xtor-0.4.0/xtor/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 def start(
     port: int = typer.Option(9052, help="Port to listen on"),
     host: str = typer.Option("127.0.0.1", help="Host to listen on"),
     control_port: int = typer.Option(9053, help="Port to control tor"),
     password: str = typer.Option("password", help="Password to control tor"),
     own: bool = typer.Option(True, help="Own tor process"),
     path: str = typer.Option("tor", help="Path to tor binary"),
+    countries: list = typer.Option([], help="Countries to use for tor"),
 ):
     """Start a tor server"""
-    tor = Tor.startTor(port=port, host=host, control_port=control_port, password=password, own=own, path=path)
+    tor = Tor.startTor(port=port, host=host, control_port=control_port, password=password, own=own, path=path, countries=countries)
     typer.echo(f"Tor started on {tor.host}:{tor.port}")
 
     if own:
         typer.pause(
             "Press any key to stop tor server. "
         )
```

### Comparing `xtor-0.3.1/xtor/tor.py` & `xtor-0.4.0/xtor/tor.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         control_port: int,
         host: str,
         password: Optional[str] = None,
         client_options: Optional[dict] = {},
         config: Optional[dict] = {},
         path: Optional[str] = None,
         own: Optional[bool] = True,
+        max_circuit_dirtiness: Optional[int] = None,
+        countries: Optional[list] = None,
         *args,
         **kwargs,
     ) -> "Tor":
         """
         Start Tor
 
         Args:
@@ -90,16 +92,24 @@
             "ControlPort": str(control_port),
             **config,
         }
 
         if password is not None:
             config["HashedControlPassword"] = getTorPassHash(password)
 
+        if max_circuit_dirtiness is not None and max_circuit_dirtiness >= 10:
+            config["MaxCircuitDirtiness"] = str(max_circuit_dirtiness)
+
+        if countries is not None:
+            config["ExitNodes"] = "{" + ",".join(countries) + "}"
+            
         
 
+
+
         tor: Popen = launch_tor_with_config(
             config=config,
             take_ownership=own,
             *args,
             **kwargs,
         )
```

### Comparing `xtor-0.3.1/xtor/utils.py` & `xtor-0.4.0/xtor/utils.py`

 * *Files identical despite different names*

### Comparing `xtor-0.3.1/PKG-INFO` & `xtor-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtor
-Version: 0.3.1
+Version: 0.4.0
 Summary: Manage Tor instances
 Home-page: https://github.com/khalidelborai/xtor
 License: GNU Version 3
 Keywords: tor,torrc,torrc manager,tor manager,tor instance,proxy
 Author: khalidelborai
 Author-email: elboraikhalid@gmail.com
 Requires-Python: >=3.7,<4.0
```

