# Comparing `tmp/Req_http_vpn-1.0.0.tar.gz` & `tmp/Req_http_vpn-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Req_http_vpn-1.0.0.tar", last modified: Mon Jul 10 19:40:56 2023, max compression
+gzip compressed data, was "Req_http_vpn-2.0.0.tar", last modified: Mon Jul 10 21:29:02 2023, max compression
```

## Comparing `Req_http_vpn-1.0.0.tar` & `Req_http_vpn-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 19:40:56.433618 Req_http_vpn-1.0.0/
--rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2021 2023-07-10 19:40:56.434619 Req_http_vpn-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-07-10 19:39:51.000000 Req_http_vpn-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 19:40:56.334592 Req_http_vpn-1.0.0/Req_http_vpn/
--rw-rw-rw-   0        0        0     6485 2023-07-10 19:39:29.000000 Req_http_vpn-1.0.0/Req_http_vpn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 19:40:56.427615 Req_http_vpn-1.0.0/Req_http_vpn.egg-info/
--rw-rw-rw-   0        0        0     2021 2023-07-10 19:40:56.000000 Req_http_vpn-1.0.0/Req_http_vpn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-10 19:40:56.000000 Req_http_vpn-1.0.0/Req_http_vpn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 19:40:56.000000 Req_http_vpn-1.0.0/Req_http_vpn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-10 19:40:56.000000 Req_http_vpn-1.0.0/Req_http_vpn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-10 19:40:56.000000 Req_http_vpn-1.0.0/Req_http_vpn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       81 2023-07-10 19:40:56.442618 Req_http_vpn-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-10 19:40:11.000000 Req_http_vpn-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:29:02.498884 Req_http_vpn-2.0.0/
+-rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2297 2023-07-10 21:29:02.500913 Req_http_vpn-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1936 2023-07-10 21:14:54.000000 Req_http_vpn-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 21:29:02.323853 Req_http_vpn-2.0.0/Req_http_vpn/
+-rw-rw-rw-   0        0        0     7101 2023-07-10 21:11:58.000000 Req_http_vpn-2.0.0/Req_http_vpn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:29:02.493878 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/
+-rw-rw-rw-   0        0        0     2297 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-10 21:29:02.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-10 21:29:01.000000 Req_http_vpn-2.0.0/Req_http_vpn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2023-07-10 21:29:02.556895 Req_http_vpn-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-07-10 21:27:34.000000 Req_http_vpn-2.0.0/setup.py
```

### Comparing `Req_http_vpn-1.0.0/LICENSE` & `Req_http_vpn-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-1.0.0/PKG-INFO` & `Req_http_vpn-2.0.0/Req_http_vpn.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: Req_http_vpn
-Version: 1.0.0
+Name: Req-http-vpn
+Version: 2.0.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
 Keywords: http
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
- ____                       _      _    _
-|  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
-| |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
-|  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
-|_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
-                 |_||_____|                 |_|    |_____|       |_|
+# ____                       _      _    _
+# |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
+# | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
+# |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
+# |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
+#                  |_||_____|                 |_|    |_____|       |_|
 
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
@@ -42,12 +42,26 @@
     ```
     And this class has **three functions** >>>
     ```python
     filter_req_GET() #To send http request with GET method
     filter_req_POST() #To send http request with POST method
     filter_req_HEAD() #To send an http request to get website headers
     ```
+
+    ```python
+   from Req_http_vpn import *
+   import os
+
+   os.environ['print_access_request_library_Req_http_vpn'] = '0' #1
+
+   app = Requests_filter(Url=f'https://youtube.com')
+
+   app = app.filter_req_GET()
+
+   print(app.get('content'))
+    ```
+
     `The author and developer of this light and simple library:` ÙŽ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
```

### Comparing `Req_http_vpn-1.0.0/README.md` & `Req_http_vpn-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
- ____                       _      _    _
-|  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
-| |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
-|  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
-|_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
-                 |_||_____|                 |_|    |_____|       |_|
+# ____                       _      _    _
+# |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
+# | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
+# |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
+# |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
+#                  |_||_____|                 |_|    |_____|       |_|
 
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
@@ -30,12 +30,26 @@
     ```
     And this class has **three functions** >>>
     ```python
     filter_req_GET() #To send http request with GET method
     filter_req_POST() #To send http request with POST method
     filter_req_HEAD() #To send an http request to get website headers
     ```
+
+    ```python
+   from Req_http_vpn import *
+   import os
+
+   os.environ['print_access_request_library_Req_http_vpn'] = '0' #1
+
+   app = Requests_filter(Url=f'https://youtube.com')
+
+   app = app.filter_req_GET()
+
+   print(app.get('content'))
+    ```
+
     `The author and developer of this light and simple library:` َ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
```

### Comparing `Req_http_vpn-1.0.0/Req_http_vpn/__init__.py` & `Req_http_vpn-2.0.0/Req_http_vpn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,25 @@
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 """
 
 import sys
 sys.dont_write_bytecode = True
 
+__version__ = ['1.0.0']
+
+this : list = []
+
+Req_Vpn_print = '0'
+
 from typing import Any, overload
 from requests import post, head, RequestException
 import os
+from ColorTER import *
+from MusicBGX import *
 
 class Requests_filter:
     """
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
     ### How to create an object from this class:
     ```python
@@ -45,16 +53,25 @@
     filter_req_HEAD() #To send an http request to get website headers
     ```
     `The author and developer of this light and simple library:` َ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
     """
+    
     def __init__(self, Url : str):
         self.url = Url
+        global Req_Vpn_print
+        if 'print_access_request_library_Req_http_vpn' not in os.environ:
+            os.environ['print_access_request_library_Req_http_vpn'] = Req_Vpn_print
+        if os.environ['print_access_request_library_Req_http_vpn'] == '0':
+            Print.printY(f'You are using Req_http_vpn library :')
+            Print.printM(f'\t version: {__version__[0]} (:')
+            bgx = BackGround(paths=['ss.mp3'])
+            bgx.play_background_music(Vol=50.0)
         
     # =======================================================================================
     
     @overload
     def filter_req_GET(
         self,
         Content_type : str = 'text/html',
```

### Comparing `Req_http_vpn-1.0.0/Req_http_vpn.egg-info/PKG-INFO` & `Req_http_vpn-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: Req-http-vpn
-Version: 1.0.0
+Name: Req_http_vpn
+Version: 2.0.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
 Keywords: http
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
- ____                       _      _    _
-|  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
-| |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
-|  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
-|_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
-                 |_||_____|                 |_|    |_____|       |_|
+# ____                       _      _    _
+# |  _ \   ___   __ _        | |__  | |_ | |_  _ __         __   __ _ __   _ __  
+# | |_) | / _ \ / _` |       | '_ \ | __|| __|| '_ \        \ \ / /| '_ \ | '_ \ 
+# |  _ < |  __/| (_| |       | | | || |_ | |_ | |_) |        \ V / | |_) || | | |
+# |_| \_\ \___| \__, | _____ |_| |_| \__| \__|| .__/  _____   \_/  | .__/ |_| |_|
+#                  |_||_____|                 |_|    |_____|       |_|
 
 """
 Req_http_vpn Library
 ~~~~~~~~~~~~~~~~~~~~~
 
 Req_http_vpn Library is an HTTP library, written in Python, for human beings.
 Basic GET usage:
@@ -42,12 +42,26 @@
     ```
     And this class has **three functions** >>>
     ```python
     filter_req_GET() #To send http request with GET method
     filter_req_POST() #To send http request with POST method
     filter_req_HEAD() #To send an http request to get website headers
     ```
+
+    ```python
+   from Req_http_vpn import *
+   import os
+
+   os.environ['print_access_request_library_Req_http_vpn'] = '0' #1
+
+   app = Requests_filter(Url=f'https://youtube.com')
+
+   app = app.filter_req_GET()
+
+   print(app.get('content'))
+    ```
+
     `The author and developer of this light and simple library:` ÙŽ**Amin Rngbr**
     **and over (:**
     
     **GitHub address**: [aminrngbr1122](https://github.com/aminrngbr1122)
```

