# Comparing `tmp/clairvoyance-2.5.1.tar.gz` & `tmp/clairvoyance-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clairvoyance-2.5.1.tar", max compression
+gzip compressed data, was "clairvoyance-2.5.2.tar", max compression
```

## Comparing `clairvoyance-2.5.1.tar` & `clairvoyance-2.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/LICENSE
--rw-r--r--   0        0        0     3501 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/README.md
--rw-r--r--   0        0        0       41 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/__init__.py
--rw-r--r--   0        0        0       71 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/__main__.py
--rw-r--r--   0        0        0     4660 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/cli.py
--rw-r--r--   0        0        0     2797 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/client.py
--rw-r--r--   0        0        0      297 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/config.py
--rw-r--r--   0        0        0       55 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/entities/__init__.py
--rw-r--r--   0        0        0      659 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/entities/context.py
--rw-r--r--   0        0        0      646 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/entities/interfaces.py
--rw-r--r--   0        0        0      419 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/entities/meta.py
--rw-r--r--   0        0        0      152 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/entities/oracle.py
--rw-r--r--   0        0        0      759 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/entities/primitives.py
--rw-r--r--   0        0        0    12718 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/graphql.py
--rw-r--r--   0        0        0    22301 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/oracle.py
--rw-r--r--   0        0        0        0 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/py.typed
--rw-r--r--   0        0        0     4450 2023-03-18 12:50:21.724825 clairvoyance-2.5.1/clairvoyance/utils.py
--rw-r--r--   0        0        0    75153 2023-03-18 12:50:21.728825 clairvoyance-2.5.1/clairvoyance/wordlist.txt
--rw-r--r--   0        0        0     1491 2023-03-18 12:50:21.728825 clairvoyance-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     4408 1970-01-01 00:00:00.000000 clairvoyance-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/LICENSE
+-rw-r--r--   0        0        0     3503 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/README.md
+-rw-r--r--   0        0        0       41 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/__main__.py
+-rw-r--r--   0        0        0     4660 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/cli.py
+-rw-r--r--   0        0        0     2797 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/client.py
+-rw-r--r--   0        0        0      297 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/config.py
+-rw-r--r--   0        0        0       55 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/entities/__init__.py
+-rw-r--r--   0        0        0      659 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/entities/context.py
+-rw-r--r--   0        0        0      646 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/entities/interfaces.py
+-rw-r--r--   0        0        0      419 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/entities/meta.py
+-rw-r--r--   0        0        0      152 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/entities/oracle.py
+-rw-r--r--   0        0        0      759 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/entities/primitives.py
+-rw-r--r--   0        0        0    12718 2023-07-10 18:39:49.637856 clairvoyance-2.5.2/clairvoyance/graphql.py
+-rw-r--r--   0        0        0    22702 2023-07-10 18:39:49.641856 clairvoyance-2.5.2/clairvoyance/oracle.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:39:49.641856 clairvoyance-2.5.2/clairvoyance/py.typed
+-rw-r--r--   0        0        0     4450 2023-07-10 18:39:49.641856 clairvoyance-2.5.2/clairvoyance/utils.py
+-rw-r--r--   0        0        0    75153 2023-07-10 18:39:49.641856 clairvoyance-2.5.2/clairvoyance/wordlist.txt
+-rw-r--r--   0        0        0     1491 2023-07-10 18:39:49.641856 clairvoyance-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 clairvoyance-2.5.2/PKG-INFO
```

### Comparing `clairvoyance-2.5.1/LICENSE` & `clairvoyance-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/README.md` & `clairvoyance-2.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 LOG_LEVEL=`INFO` # A string level for logging.
 ```
 
 ## Support
 
 > Due to time constraints @nikitastupin won't be able to answer all the issues for some time but he'll do his best to review & merge PRs
 
-In case of question or issue with clairvoyance please refer to [wiki](https://github.com/nikitastupin/clairvoyance/wiki) or [issues](https://github.com/nikitastupin/clairvoyance/issues). If this doesn't solve your problem feel free to open a [new issue](https://github.com/nikitastupin/clairvoyance/issues/new).
+In case of questions or issues with Clairvoyance please refer to [wiki](https://github.com/nikitastupin/clairvoyance/wiki) or [issues](https://github.com/nikitastupin/clairvoyance/issues). If this doesn't solve your problem feel free to open a [new issue](https://github.com/nikitastupin/clairvoyance/issues/new).
 
 ## Contributing
 
 Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change. For more information about tests, internal project structure and so on refer to [Development](https://github.com/nikitastupin/clairvoyance/wiki/Development) wiki page.
 
 ## Documentation
```

### Comparing `clairvoyance-2.5.1/clairvoyance/cli.py` & `clairvoyance-2.5.2/clairvoyance/cli.py`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/clairvoyance/client.py` & `clairvoyance-2.5.2/clairvoyance/client.py`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/clairvoyance/entities/context.py` & `clairvoyance-2.5.2/clairvoyance/entities/context.py`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/clairvoyance/entities/interfaces.py` & `clairvoyance-2.5.2/clairvoyance/entities/interfaces.py`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/clairvoyance/entities/primitives.py` & `clairvoyance-2.5.2/clairvoyance/entities/primitives.py`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/clairvoyance/graphql.py` & `clairvoyance-2.5.2/clairvoyance/graphql.py`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/clairvoyance/oracle.py` & `clairvoyance-2.5.2/clairvoyance/oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,15 +418,16 @@
     results = await asyncio.gather(*tasks)
     for result in results:
         if result:
             typeref = result
 
     if not typeref and context != FuzzingContext.ARGUMENT:
         try:
-            raise Exception(f'Unable to get TypeRef for {documents} in context {context}')
+            raise Exception(f"""Unable to get TypeRef for {documents} in context {context}.
+                            It is very likely that Field Suggestion is not fully enabled on this endpoint.""")
         except Exception as e:
             raise Exception(e) from e
 
     return typeref
 
 
 async def probe_field_type(
@@ -463,30 +464,33 @@
 
 async def probe_typename(input_document: str) -> str:
 
     document = input_document.replace('FUZZ', WRONG_FIELD_EXAMPLE)
 
     response = await client().post(document=document)
     if 'errors' not in response:
-        log().debug(f'Unable to get typename from {document}')
-        sys.exit(1)
+        log().warning(f"""Unable to get typename from {document}.
+                      Field Suggestion might not be enabled on this endpoint. Using default "Query""")
+        return 'Query'
 
     errors = response['errors']
 
     match = None
     for regex in WRONG_TYPENAME:
         for error in errors:
             match = re.fullmatch(regex, error['message'])
             if match:
                 break
         if match:
             break
 
     if not match:
-        log().debug(f'Unkwon error in `probe_typename`: "{errors}" does not match any known regexes.')
+        log().debug(f"""Unkwon error in `probe_typename`: "{errors}" does not match any known regexes.
+                    Field Suggestion might not be enabled on this endpoint. Using default "Query""")
+        return 'Query'
 
     return (match.group('typename').replace('[', '').replace(']', '').replace('!', ''))
 
 
 async def fetch_root_typenames() -> Dict[str, Optional[str]]:
     documents: Dict[str, str] = {
         'queryType': 'query { __typename }',
@@ -551,14 +555,17 @@
 
 
 async def clairvoyance(
     wordlist: List[str],
     input_document: str,
     input_schema: Dict[str, Any] = None,
 ) -> str:
+
+    log().debug(f'input_document = {input_document}')
+
     if not input_schema:
         root_typenames = await fetch_root_typenames()
         schema = graphql.Schema(
             query_type=root_typenames['queryType'],
             mutation_type=root_typenames['mutationType'],
             subscription_type=root_typenames['subscriptionType'],
         )
```

### Comparing `clairvoyance-2.5.1/clairvoyance/utils.py` & `clairvoyance-2.5.2/clairvoyance/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     )
     parser.add_argument(
         '-p',
         '--profile',
         choices=['slow', 'fast'],
         default='fast',
         help='Select a speed profile. fast mod will set lot of workers to provide you quick result'
-        + ' but if the server as some rate limit you may wnat to use slow mod.',
+        + ' but if the server as some rate limit you may want to use slow mod.',
     )
     parser.add_argument(
         '--progress',
         action='store_true',
         help='Enable progress bar',
     )
     parser.add_argument('url')
```

### Comparing `clairvoyance-2.5.1/clairvoyance/wordlist.txt` & `clairvoyance-2.5.2/clairvoyance/wordlist.txt`

 * *Files identical despite different names*

### Comparing `clairvoyance-2.5.1/pyproject.toml` & `clairvoyance-2.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Clairvoyance"
-version = "2.5.1"
+version = "2.5.2"
 description = "Obtain GraphQL API Schema even if the introspection is not enabled"
 authors = [
     "Nikita Stupin <nikitastupin@protonmail.com>",
     "Swan <swan@escape.tech>"
 ]
 maintainers = [
     "Nikita Stupin <nikitastupin@protonmail.com>",
```

### Comparing `clairvoyance-2.5.1/PKG-INFO` & `clairvoyance-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clairvoyance
-Version: 2.5.1
+Version: 2.5.2
 Summary: Obtain GraphQL API Schema even if the introspection is not enabled
 Home-page: https://github.com/nikitastupin/clairvoyance
 License: MIT
 Author: Nikita Stupin
 Author-email: nikitastupin@protonmail.com
 Maintainer: Nikita Stupin
 Maintainer-email: nikitastupin@protonmail.com
@@ -84,15 +84,15 @@
 LOG_LEVEL=`INFO` # A string level for logging.
 ```
 
 ## Support
 
 > Due to time constraints @nikitastupin won't be able to answer all the issues for some time but he'll do his best to review & merge PRs
 
-In case of question or issue with clairvoyance please refer to [wiki](https://github.com/nikitastupin/clairvoyance/wiki) or [issues](https://github.com/nikitastupin/clairvoyance/issues). If this doesn't solve your problem feel free to open a [new issue](https://github.com/nikitastupin/clairvoyance/issues/new).
+In case of questions or issues with Clairvoyance please refer to [wiki](https://github.com/nikitastupin/clairvoyance/wiki) or [issues](https://github.com/nikitastupin/clairvoyance/issues). If this doesn't solve your problem feel free to open a [new issue](https://github.com/nikitastupin/clairvoyance/issues/new).
 
 ## Contributing
 
 Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change. For more information about tests, internal project structure and so on refer to [Development](https://github.com/nikitastupin/clairvoyance/wiki/Development) wiki page.
 
 ## Documentation
```

