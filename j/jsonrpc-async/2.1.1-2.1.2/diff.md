# Comparing `tmp/jsonrpc-async-2.1.1.tar.gz` & `tmp/jsonrpc-async-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonrpc-async-2.1.1.tar", last modified: Tue May  3 16:33:22 2022, max compression
+gzip compressed data, was "jsonrpc-async-2.1.2.tar", last modified: Mon Jul 10 16:00:19 2023, max compression
```

## Comparing `jsonrpc-async-2.1.1.tar` & `jsonrpc-async-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/
--rw-r--r--   0 emilylovemills   (502) staff       (20)     6725 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/PKG-INFO
--rw-r--r--   0 emilylovemills   (502) staff       (20)      135 2022-05-03 16:26:36.000000 jsonrpc-async-2.1.1/requirements-test.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)       20 2021-11-21 16:06:47.000000 jsonrpc-async-2.1.1/MANIFEST.in
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async.egg-info/
--rw-r--r--   0 emilylovemills   (502) staff       (20)     6725 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async.egg-info/PKG-INFO
--rw-r--r--   0 emilylovemills   (502) staff       (20)      300 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async.egg-info/SOURCES.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)       35 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async.egg-info/requires.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)       14 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async.egg-info/top_level.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)        1 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async.egg-info/dependency_links.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)     1158 2022-05-03 16:33:07.000000 jsonrpc-async-2.1.1/setup.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)       38 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/setup.cfg
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:33:22.000000 jsonrpc-async-2.1.1/jsonrpc_async/
--rw-r--r--   0 emilylovemills   (502) staff       (20)      144 2021-11-21 16:06:47.000000 jsonrpc-async-2.1.1/jsonrpc_async/__init__.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     1873 2021-11-21 16:06:47.000000 jsonrpc-async-2.1.1/jsonrpc_async/jsonrpc.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     4855 2022-05-03 16:32:04.000000 jsonrpc-async-2.1.1/README.rst
--rw-r--r--   0 emilylovemills   (502) staff       (20)     1468 2021-11-21 16:06:47.000000 jsonrpc-async-2.1.1/LICENSE.txt
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-07-10 16:00:19.593402 jsonrpc-async-2.1.2/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     1468 2023-07-10 15:48:32.000000 jsonrpc-async-2.1.2/LICENSE.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       20 2023-07-10 15:48:32.000000 jsonrpc-async-2.1.2/MANIFEST.in
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5549 2023-07-10 16:00:19.593186 jsonrpc-async-2.1.2/PKG-INFO
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     4817 2023-07-10 15:58:31.000000 jsonrpc-async-2.1.2/README.rst
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-07-10 16:00:19.591055 jsonrpc-async-2.1.2/jsonrpc_async/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      144 2023-07-10 15:48:32.000000 jsonrpc-async-2.1.2/jsonrpc_async/__init__.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     2080 2023-07-10 15:48:32.000000 jsonrpc-async-2.1.2/jsonrpc_async/jsonrpc.py
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-07-10 16:00:19.592819 jsonrpc-async-2.1.2/jsonrpc_async.egg-info/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5549 2023-07-10 16:00:19.000000 jsonrpc-async-2.1.2/jsonrpc_async.egg-info/PKG-INFO
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      300 2023-07-10 16:00:19.000000 jsonrpc-async-2.1.2/jsonrpc_async.egg-info/SOURCES.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)        1 2023-07-10 16:00:19.000000 jsonrpc-async-2.1.2/jsonrpc_async.egg-info/dependency_links.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       35 2023-07-10 16:00:19.000000 jsonrpc-async-2.1.2/jsonrpc_async.egg-info/requires.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       14 2023-07-10 16:00:19.000000 jsonrpc-async-2.1.2/jsonrpc_async.egg-info/top_level.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      135 2023-07-10 15:48:32.000000 jsonrpc-async-2.1.2/requirements-test.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       38 2023-07-10 16:00:19.593462 jsonrpc-async-2.1.2/setup.cfg
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     1153 2023-07-10 15:58:47.000000 jsonrpc-async-2.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsonrpc-async-2.1.1/PKG-INFO` & `jsonrpc-async-2.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,161 +1,155 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: jsonrpc-async
-Version: 2.1.1
+Version: 2.1.2
 Summary: A JSON-RPC client library for asyncio
 Home-page: http://github.com/emlove/jsonrpc-async
-Author: Emily Love Mills
+Author: Emily Mills
 Author-email: emily@emlove.me
 License: BSD
-Description: jsonrpc-async: a compact JSON-RPC client library for asyncio
-        =======================================================================================================
-        
-        .. image:: https://img.shields.io/pypi/v/jsonrpc-async.svg
-                :target: https://pypi.python.org/pypi/jsonrpc-async
-        .. image:: https://github.com/emlove/jsonrpc-async/workflows/tests/badge.svg
-                :target: https://github.com/emlove/jsonrpc-async/actions
-        .. image:: https://coveralls.io/repos/emlove/jsonrpc-async/badge.svg
-            :target: https://coveralls.io/r/emlove/jsonrpc-async
-        
-        This is a compact and simple JSON-RPC client implementation for asyncio python code. This code is forked from https://github.com/gciotta/jsonrpc-requests
-        
-        Main Features
-        -------------
-        
-        * Supports nested namespaces (eg. `app.users.getUsers()`)
-        * 100% test coverage
-        
-        Usage
-        -----
-        It is recommended to manage the aiohttp ClientSession object externally and pass it to the Server constructor. `(See the aiohttp documentation.) <https://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession>`_ If not passed to Server, a ClientSession object will be created automatically.
-        
-        Execute remote JSON-RPC functions
-        
-        .. code-block:: python
-        
-            import asyncio
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server('http://localhost:8080')
-                try:
-                    await server.foo(1, 2)
-                    await server.foo(bar=1, baz=2)
-                    await server.foo({'foo': 'bar'})
-                    await server.foo.bar(baz=1, qux=2)
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        A notification
-        
-        .. code-block:: python
-        
-            import asyncio
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server('http://localhost:8080')
-                try:
-                    await server.foo(bar=1, _notification=True)
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        Pass through arguments to aiohttp (see also `aiohttp  documentation <http://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession.request>`_)
-        
-        .. code-block:: python
-        
-            import asyncio
-            import aiohttp
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server(
-                    'http://localhost:8080',
-                    auth=aiohttp.BasicAuth('user', 'pass'),
-                    headers={'x-test2': 'true'})
-                try:
-                    await server.foo()
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        Pass through aiohttp exceptions
-        
-        .. code-block:: python
-        
-            import asyncio
-            import aiohttp
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server('http://unknown-host')
-                try:
-                    await server.foo()
-                except TransportError as transport_error:
-                    print(transport_error.args[1]) # this will hold a aiohttp exception instance
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        Tests
-        -----
-        Install the Python tox package and run ``tox``, it'll test this package with various versions of Python.
-        
-        Changelog
-        ---------
-        2.1.1 (2022-05-03)
-        ~~~~~~~~~~~~~~~~~~
-        - Unpin test dependencies and fix tests
-        
-        2.1.0 (2021-05-03)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 2.1.0
-        
-        2.0.0 (2021-03-16)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 2.0.0
-        - BREAKING CHANGE: `Allow single mapping as a positional parameter. <https://github.com/emlove/jsonrpc-base/pull/6>`_
-          Previously, when calling with a single dict as a parameter (example: ``server.foo({'bar': 0})``), the mapping was used as the JSON-RPC keyword parameters. This made it impossible to send a mapping as the first and only positional parameter. If you depended on the old behavior, you can recreate it by spreading the mapping as your method's kwargs. (example: ``server.foo(**{'bar': 0})``)
-        
-        1.1.1 (2019-11-12)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 1.0.3
-        
-        1.1.0 (2018-09-04)
-        ~~~~~~~~~~~~~~~~~~
-        - Added support for using a custom json.loads method `(#1) <https://github.com/emlove/jsonrpc-async/pull/1>`_ `@tdivis <https://github.com/tdivis>`_
-        
-        1.0.1 (2018-08-23)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 1.0.2
-        
-        1.0.0 (2018-07-06)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped minimum aiohttp version to 3.0.0
-        - Bumped jsonrpc-base to version 1.0.1
-        
-        Credits
-        -------
-        `@gciotta <https://github.com/gciotta>`_ for creating the base project `jsonrpc-requests <https://github.com/gciotta/jsonrpc-requests>`_.
-        
-        `@mbroadst <https://github.com/mbroadst>`_ for providing full support for nested method calls, JSON-RPC RFC
-        compliance and other improvements.
-        
-        `@vaab <https://github.com/vaab>`_ for providing api and tests improvements, better RFC compliance.
-        
 Keywords: json-rpc async asyncio
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.txt
+
+jsonrpc-async: a compact JSON-RPC client library for asyncio
+=======================================================================================================
+
+.. image:: https://img.shields.io/pypi/v/jsonrpc-async.svg
+        :target: https://pypi.python.org/pypi/jsonrpc-async
+.. image:: https://github.com/emlove/jsonrpc-async/workflows/tests/badge.svg
+        :target: https://github.com/emlove/jsonrpc-async/actions
+.. image:: https://coveralls.io/repos/emlove/jsonrpc-async/badge.svg
+    :target: https://coveralls.io/r/emlove/jsonrpc-async
+
+This is a compact and simple JSON-RPC client implementation for asyncio python code. This code is forked from https://github.com/gciotta/jsonrpc-requests
+
+Main Features
+-------------
+
+* Supports nested namespaces (eg. `app.users.getUsers()`)
+* 100% test coverage
+
+Usage
+-----
+It is recommended to manage the aiohttp ClientSession object externally and pass it to the Server constructor. `(See the aiohttp documentation.) <https://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession>`_ If not passed to Server, a ClientSession object will be created automatically.
+
+Execute remote JSON-RPC functions
+
+.. code-block:: python
+
+    import asyncio
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server('http://localhost:8080') as server:
+            await server.foo(1, 2)
+            await server.foo(bar=1, baz=2)
+            await server.foo({'foo': 'bar'})
+            await server.foo.bar(baz=1, qux=2)
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+A notification
+
+.. code-block:: python
+
+    import asyncio
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server('http://localhost:8080') as server:
+            await server.foo(bar=1, _notification=True)
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+Pass through arguments to aiohttp (see also `aiohttp  documentation <http://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession.request>`_)
+
+.. code-block:: python
+
+    import asyncio
+    import aiohttp
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server(
+            'http://localhost:8080',
+            auth=aiohttp.BasicAuth('user', 'pass'),
+            headers={'x-test2': 'true'}
+        ) as server:
+            await server.foo()
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+Pass through aiohttp exceptions
+
+.. code-block:: python
+
+    import asyncio
+    import aiohttp
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server('http://unknown-host') as server:
+            try:
+                await server.foo()
+            except TransportError as transport_error:
+                print(transport_error.args[1]) # this will hold a aiohttp exception instance
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+Tests
+-----
+Install the Python tox package and run ``tox``, it'll test this package with various versions of Python.
+
+Changelog
+---------
+2.1.2 (2023-07-10)
+~~~~~~~~~~~~~~~~~~
+- Add support for `async with` `(#10) <https://github.com/emlove/jsonrpc-async/pull/10>`_ `@lieryan <https://github.com/lieryan>`_
+
+2.1.1 (2022-05-03)
+~~~~~~~~~~~~~~~~~~
+- Unpin test dependencies
+
+2.1.0 (2021-05-03)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 2.1.0
+
+2.0.0 (2021-03-16)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 2.0.0
+- BREAKING CHANGE: `Allow single mapping as a positional parameter. <https://github.com/emlove/jsonrpc-base/pull/6>`_
+  Previously, when calling with a single dict as a parameter (example: ``server.foo({'bar': 0})``), the mapping was used as the JSON-RPC keyword parameters. This made it impossible to send a mapping as the first and only positional parameter. If you depended on the old behavior, you can recreate it by spreading the mapping as your method's kwargs. (example: ``server.foo(**{'bar': 0})``)
+
+1.1.1 (2019-11-12)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 1.0.3
+
+1.1.0 (2018-09-04)
+~~~~~~~~~~~~~~~~~~
+- Added support for using a custom json.loads method `(#1) <https://github.com/emlove/jsonrpc-async/pull/1>`_ `@tdivis <https://github.com/tdivis>`_
+
+1.0.1 (2018-08-23)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 1.0.2
+
+1.0.0 (2018-07-06)
+~~~~~~~~~~~~~~~~~~
+- Bumped minimum aiohttp version to 3.0.0
+- Bumped jsonrpc-base to version 1.0.1
+
+Credits
+-------
+`@gciotta <https://github.com/gciotta>`_ for creating the base project `jsonrpc-requests <https://github.com/gciotta/jsonrpc-requests>`_.
+
+`@mbroadst <https://github.com/mbroadst>`_ for providing full support for nested method calls, JSON-RPC RFC
+compliance and other improvements.
+
+`@vaab <https://github.com/vaab>`_ for providing api and tests improvements, better RFC compliance.
```

### Comparing `jsonrpc-async-2.1.1/jsonrpc_async.egg-info/PKG-INFO` & `jsonrpc-async-2.1.2/jsonrpc_async.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,161 +1,155 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: jsonrpc-async
-Version: 2.1.1
+Version: 2.1.2
 Summary: A JSON-RPC client library for asyncio
 Home-page: http://github.com/emlove/jsonrpc-async
-Author: Emily Love Mills
+Author: Emily Mills
 Author-email: emily@emlove.me
 License: BSD
-Description: jsonrpc-async: a compact JSON-RPC client library for asyncio
-        =======================================================================================================
-        
-        .. image:: https://img.shields.io/pypi/v/jsonrpc-async.svg
-                :target: https://pypi.python.org/pypi/jsonrpc-async
-        .. image:: https://github.com/emlove/jsonrpc-async/workflows/tests/badge.svg
-                :target: https://github.com/emlove/jsonrpc-async/actions
-        .. image:: https://coveralls.io/repos/emlove/jsonrpc-async/badge.svg
-            :target: https://coveralls.io/r/emlove/jsonrpc-async
-        
-        This is a compact and simple JSON-RPC client implementation for asyncio python code. This code is forked from https://github.com/gciotta/jsonrpc-requests
-        
-        Main Features
-        -------------
-        
-        * Supports nested namespaces (eg. `app.users.getUsers()`)
-        * 100% test coverage
-        
-        Usage
-        -----
-        It is recommended to manage the aiohttp ClientSession object externally and pass it to the Server constructor. `(See the aiohttp documentation.) <https://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession>`_ If not passed to Server, a ClientSession object will be created automatically.
-        
-        Execute remote JSON-RPC functions
-        
-        .. code-block:: python
-        
-            import asyncio
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server('http://localhost:8080')
-                try:
-                    await server.foo(1, 2)
-                    await server.foo(bar=1, baz=2)
-                    await server.foo({'foo': 'bar'})
-                    await server.foo.bar(baz=1, qux=2)
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        A notification
-        
-        .. code-block:: python
-        
-            import asyncio
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server('http://localhost:8080')
-                try:
-                    await server.foo(bar=1, _notification=True)
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        Pass through arguments to aiohttp (see also `aiohttp  documentation <http://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession.request>`_)
-        
-        .. code-block:: python
-        
-            import asyncio
-            import aiohttp
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server(
-                    'http://localhost:8080',
-                    auth=aiohttp.BasicAuth('user', 'pass'),
-                    headers={'x-test2': 'true'})
-                try:
-                    await server.foo()
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        Pass through aiohttp exceptions
-        
-        .. code-block:: python
-        
-            import asyncio
-            import aiohttp
-            from jsonrpc_async import Server
-        
-            async def routine():
-                server = Server('http://unknown-host')
-                try:
-                    await server.foo()
-                except TransportError as transport_error:
-                    print(transport_error.args[1]) # this will hold a aiohttp exception instance
-                finally:
-                    await server.session.close()
-        
-            asyncio.get_event_loop().run_until_complete(routine())
-        
-        Tests
-        -----
-        Install the Python tox package and run ``tox``, it'll test this package with various versions of Python.
-        
-        Changelog
-        ---------
-        2.1.1 (2022-05-03)
-        ~~~~~~~~~~~~~~~~~~
-        - Unpin test dependencies and fix tests
-        
-        2.1.0 (2021-05-03)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 2.1.0
-        
-        2.0.0 (2021-03-16)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 2.0.0
-        - BREAKING CHANGE: `Allow single mapping as a positional parameter. <https://github.com/emlove/jsonrpc-base/pull/6>`_
-          Previously, when calling with a single dict as a parameter (example: ``server.foo({'bar': 0})``), the mapping was used as the JSON-RPC keyword parameters. This made it impossible to send a mapping as the first and only positional parameter. If you depended on the old behavior, you can recreate it by spreading the mapping as your method's kwargs. (example: ``server.foo(**{'bar': 0})``)
-        
-        1.1.1 (2019-11-12)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 1.0.3
-        
-        1.1.0 (2018-09-04)
-        ~~~~~~~~~~~~~~~~~~
-        - Added support for using a custom json.loads method `(#1) <https://github.com/emlove/jsonrpc-async/pull/1>`_ `@tdivis <https://github.com/tdivis>`_
-        
-        1.0.1 (2018-08-23)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped jsonrpc-base to version 1.0.2
-        
-        1.0.0 (2018-07-06)
-        ~~~~~~~~~~~~~~~~~~
-        - Bumped minimum aiohttp version to 3.0.0
-        - Bumped jsonrpc-base to version 1.0.1
-        
-        Credits
-        -------
-        `@gciotta <https://github.com/gciotta>`_ for creating the base project `jsonrpc-requests <https://github.com/gciotta/jsonrpc-requests>`_.
-        
-        `@mbroadst <https://github.com/mbroadst>`_ for providing full support for nested method calls, JSON-RPC RFC
-        compliance and other improvements.
-        
-        `@vaab <https://github.com/vaab>`_ for providing api and tests improvements, better RFC compliance.
-        
 Keywords: json-rpc async asyncio
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.txt
+
+jsonrpc-async: a compact JSON-RPC client library for asyncio
+=======================================================================================================
+
+.. image:: https://img.shields.io/pypi/v/jsonrpc-async.svg
+        :target: https://pypi.python.org/pypi/jsonrpc-async
+.. image:: https://github.com/emlove/jsonrpc-async/workflows/tests/badge.svg
+        :target: https://github.com/emlove/jsonrpc-async/actions
+.. image:: https://coveralls.io/repos/emlove/jsonrpc-async/badge.svg
+    :target: https://coveralls.io/r/emlove/jsonrpc-async
+
+This is a compact and simple JSON-RPC client implementation for asyncio python code. This code is forked from https://github.com/gciotta/jsonrpc-requests
+
+Main Features
+-------------
+
+* Supports nested namespaces (eg. `app.users.getUsers()`)
+* 100% test coverage
+
+Usage
+-----
+It is recommended to manage the aiohttp ClientSession object externally and pass it to the Server constructor. `(See the aiohttp documentation.) <https://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession>`_ If not passed to Server, a ClientSession object will be created automatically.
+
+Execute remote JSON-RPC functions
+
+.. code-block:: python
+
+    import asyncio
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server('http://localhost:8080') as server:
+            await server.foo(1, 2)
+            await server.foo(bar=1, baz=2)
+            await server.foo({'foo': 'bar'})
+            await server.foo.bar(baz=1, qux=2)
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+A notification
+
+.. code-block:: python
+
+    import asyncio
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server('http://localhost:8080') as server:
+            await server.foo(bar=1, _notification=True)
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+Pass through arguments to aiohttp (see also `aiohttp  documentation <http://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession.request>`_)
+
+.. code-block:: python
+
+    import asyncio
+    import aiohttp
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server(
+            'http://localhost:8080',
+            auth=aiohttp.BasicAuth('user', 'pass'),
+            headers={'x-test2': 'true'}
+        ) as server:
+            await server.foo()
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+Pass through aiohttp exceptions
+
+.. code-block:: python
+
+    import asyncio
+    import aiohttp
+    from jsonrpc_async import Server
+
+    async def routine():
+        async with Server('http://unknown-host') as server:
+            try:
+                await server.foo()
+            except TransportError as transport_error:
+                print(transport_error.args[1]) # this will hold a aiohttp exception instance
+
+    asyncio.get_event_loop().run_until_complete(routine())
+
+Tests
+-----
+Install the Python tox package and run ``tox``, it'll test this package with various versions of Python.
+
+Changelog
+---------
+2.1.2 (2023-07-10)
+~~~~~~~~~~~~~~~~~~
+- Add support for `async with` `(#10) <https://github.com/emlove/jsonrpc-async/pull/10>`_ `@lieryan <https://github.com/lieryan>`_
+
+2.1.1 (2022-05-03)
+~~~~~~~~~~~~~~~~~~
+- Unpin test dependencies
+
+2.1.0 (2021-05-03)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 2.1.0
+
+2.0.0 (2021-03-16)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 2.0.0
+- BREAKING CHANGE: `Allow single mapping as a positional parameter. <https://github.com/emlove/jsonrpc-base/pull/6>`_
+  Previously, when calling with a single dict as a parameter (example: ``server.foo({'bar': 0})``), the mapping was used as the JSON-RPC keyword parameters. This made it impossible to send a mapping as the first and only positional parameter. If you depended on the old behavior, you can recreate it by spreading the mapping as your method's kwargs. (example: ``server.foo(**{'bar': 0})``)
+
+1.1.1 (2019-11-12)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 1.0.3
+
+1.1.0 (2018-09-04)
+~~~~~~~~~~~~~~~~~~
+- Added support for using a custom json.loads method `(#1) <https://github.com/emlove/jsonrpc-async/pull/1>`_ `@tdivis <https://github.com/tdivis>`_
+
+1.0.1 (2018-08-23)
+~~~~~~~~~~~~~~~~~~
+- Bumped jsonrpc-base to version 1.0.2
+
+1.0.0 (2018-07-06)
+~~~~~~~~~~~~~~~~~~
+- Bumped minimum aiohttp version to 3.0.0
+- Bumped jsonrpc-base to version 1.0.1
+
+Credits
+-------
+`@gciotta <https://github.com/gciotta>`_ for creating the base project `jsonrpc-requests <https://github.com/gciotta/jsonrpc-requests>`_.
+
+`@mbroadst <https://github.com/mbroadst>`_ for providing full support for nested method calls, JSON-RPC RFC
+compliance and other improvements.
+
+`@vaab <https://github.com/vaab>`_ for providing api and tests improvements, better RFC compliance.
```

### Comparing `jsonrpc-async-2.1.1/setup.py` & `jsonrpc-async-2.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 except ImportError:
     import sys
     print("Please install the `setuptools` package in order to install this library", file=sys.stderr)
     raise
 
 setup(
     name='jsonrpc-async',
-    version='2.1.1',
-    author='Emily Love Mills',
+    version='2.1.2',
+    author='Emily Mills',
     author_email='emily@emlove.me',
     packages=('jsonrpc_async',),
     license='BSD',
     keywords='json-rpc async asyncio',
     url='http://github.com/emlove/jsonrpc-async',
     description='''A JSON-RPC client library for asyncio''',
     long_description=open('README.rst').read(),
```

### Comparing `jsonrpc-async-2.1.1/jsonrpc_async/jsonrpc.py` & `jsonrpc-async-2.1.2/jsonrpc_async/jsonrpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,7 +45,14 @@
         try:
             response_data = await response.json(**self._json_args)
         except ValueError as value_error:
             raise TransportError(
                 'Cannot deserialize response body', message, value_error)
 
         return message.parse_response(response_data)
+
+    async def __aenter__(self):
+        await self.session.__aenter__()
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        return await self.session.__aexit__(exc_type, exc, tb)
```

### Comparing `jsonrpc-async-2.1.1/README.rst` & `jsonrpc-async-2.1.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -24,89 +24,83 @@
 
 .. code-block:: python
 
     import asyncio
     from jsonrpc_async import Server
 
     async def routine():
-        server = Server('http://localhost:8080')
-        try:
+        async with Server('http://localhost:8080') as server:
             await server.foo(1, 2)
             await server.foo(bar=1, baz=2)
             await server.foo({'foo': 'bar'})
             await server.foo.bar(baz=1, qux=2)
-        finally:
-            await server.session.close()
 
     asyncio.get_event_loop().run_until_complete(routine())
 
 A notification
 
 .. code-block:: python
 
     import asyncio
     from jsonrpc_async import Server
 
     async def routine():
-        server = Server('http://localhost:8080')
-        try:
+        async with Server('http://localhost:8080') as server:
             await server.foo(bar=1, _notification=True)
-        finally:
-            await server.session.close()
 
     asyncio.get_event_loop().run_until_complete(routine())
 
 Pass through arguments to aiohttp (see also `aiohttp  documentation <http://aiohttp.readthedocs.io/en/stable/client_reference.html#aiohttp.ClientSession.request>`_)
 
 .. code-block:: python
 
     import asyncio
     import aiohttp
     from jsonrpc_async import Server
 
     async def routine():
-        server = Server(
+        async with Server(
             'http://localhost:8080',
             auth=aiohttp.BasicAuth('user', 'pass'),
-            headers={'x-test2': 'true'})
-        try:
+            headers={'x-test2': 'true'}
+        ) as server:
             await server.foo()
-        finally:
-            await server.session.close()
 
     asyncio.get_event_loop().run_until_complete(routine())
 
 Pass through aiohttp exceptions
 
 .. code-block:: python
 
     import asyncio
     import aiohttp
     from jsonrpc_async import Server
 
     async def routine():
-        server = Server('http://unknown-host')
-        try:
-            await server.foo()
-        except TransportError as transport_error:
-            print(transport_error.args[1]) # this will hold a aiohttp exception instance
-        finally:
-            await server.session.close()
+        async with Server('http://unknown-host') as server:
+            try:
+                await server.foo()
+            except TransportError as transport_error:
+                print(transport_error.args[1]) # this will hold a aiohttp exception instance
 
     asyncio.get_event_loop().run_until_complete(routine())
 
 Tests
 -----
 Install the Python tox package and run ``tox``, it'll test this package with various versions of Python.
 
 Changelog
 ---------
+2.1.2 (2023-07-10)
+~~~~~~~~~~~~~~~~~~
+- Add support for `async with` `(#10) <https://github.com/emlove/jsonrpc-async/pull/10>`_ `@lieryan <https://github.com/lieryan>`_
+
 2.1.1 (2022-05-03)
 ~~~~~~~~~~~~~~~~~~
-- Unpin test dependencies and fix tests
+- Unpin test dependencies
 
 2.1.0 (2021-05-03)
 ~~~~~~~~~~~~~~~~~~
 - Bumped jsonrpc-base to version 2.1.0
 
 2.0.0 (2021-03-16)
 ~~~~~~~~~~~~~~~~~~
```

### Comparing `jsonrpc-async-2.1.1/LICENSE.txt` & `jsonrpc-async-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

