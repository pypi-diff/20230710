# Comparing `tmp/ixoncdkingress-0.0.7.tar.gz` & `tmp/ixoncdkingress-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixoncdkingress-0.0.7.tar", last modified: Thu Jun 22 09:01:13 2023, max compression
+gzip compressed data, was "ixoncdkingress-0.0.8.tar", last modified: Mon Jul 10 09:55:59 2023, max compression
```

## Comparing `ixoncdkingress-0.0.7.tar` & `ixoncdkingress-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress/cbc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8106 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/caller.py
--rw-rw-rw-   0 root         (0) root         (0)     2547 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/cbc/context.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/types.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress/webserver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 09:00:47.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4208 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7398 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/request.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/response.py
--rw-rw-rw-   0 root         (0) root         (0)     4445 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/servlet.py
--rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/ixoncdkingress/webserver/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      800 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/ixoncdkingress.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-22 09:01:13.000000 ixoncdkingress-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:01:13.211183 ixoncdkingress-0.0.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1055 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/tests/test___main__.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-06-22 08:16:19.000000 ixoncdkingress-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.469914 ixoncdkingress-0.0.8/ixoncdkingress/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/ixoncdkingress/cbc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/caller.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/cbc/document_db_client.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/ixoncdkingress/webserver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 09:55:24.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4208 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4445 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/servlet.py
+-rw-rw-rw-   0 root         (0) root         (0)     6425 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/ixoncdkingress/webserver/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      841 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/ixoncdkingress.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-10 09:55:59.000000 ixoncdkingress-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:55:59.473914 ixoncdkingress-0.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/tests/test___main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-10 09:18:40.000000 ixoncdkingress-0.0.8/tests/test_utils.py
```

### Comparing `ixoncdkingress-0.0.7/README.md` & `ixoncdkingress-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/__main__.py` & `ixoncdkingress-0.0.8/ixoncdkingress/__main__.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/cbc/api_client.py` & `ixoncdkingress-0.0.8/ixoncdkingress/cbc/api_client.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/cbc/caller.py` & `ixoncdkingress-0.0.8/ixoncdkingress/cbc/caller.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/cbc/context.py` & `ixoncdkingress-0.0.8/ixoncdkingress/cbc/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Context.
 """
 from typing import Any, Dict, Optional, Set
 
 from ixoncdkingress.cbc.api_client import ApiClient
+from ixoncdkingress.cbc.document_db_client import DocumentDBClient
 
-class CbcIxapiResource:
+class CbcResource:
     """
     Describes an IXAPI resource.
     """
     public_id: str
     name: str
     custom_properties: Dict[str, Any]
     permissions: Optional[Set[str]]
@@ -37,60 +38,59 @@
         )
 
 class CbcContext:
     """
     The context for a backend component.
     """
     config: Dict[str, str]
-
     api_client: ApiClient
-
-    user: Optional[CbcIxapiResource] = None
-
-    company: Optional[CbcIxapiResource] = None
-
-    asset: Optional[CbcIxapiResource] = None
-
-    agent: Optional[CbcIxapiResource] = None
+    document_db_client: Optional[DocumentDBClient] = None
+    user: Optional[CbcResource] = None
+    company: Optional[CbcResource] = None
+    asset: Optional[CbcResource] = None
+    agent: Optional[CbcResource] = None
 
     @property
-    def agent_or_asset(self) -> CbcIxapiResource:
+    def agent_or_asset(self) -> CbcResource:
         """
         Return either an Agent or an Asset resource, depending on what's available. If both are
         available in the context, returns the Asset resource.
         """
         if self.asset:
             return self.asset
 
         assert self.agent
         return self.agent
 
     def __init__(
             self,
             config: Dict[str, str],
             api_client: ApiClient,
-            user: Optional[CbcIxapiResource] = None,
-            company: Optional[CbcIxapiResource] = None,
-            asset: Optional[CbcIxapiResource] = None,
-            agent: Optional[CbcIxapiResource] = None,
+            document_db_client: Optional[DocumentDBClient] = None,
+            user: Optional[CbcResource] = None,
+            company: Optional[CbcResource] = None,
+            asset: Optional[CbcResource] = None,
+            agent: Optional[CbcResource] = None,
             **kwargs: Any
         ) -> None:
         del kwargs
 
         self.config = config
         self.api_client = api_client
+        self.document_db_client = document_db_client
         self.user = user
         self.company = company
         self.asset = asset
         self.agent = agent
 
     def __repr__(self) -> str:
         return (
             f'<CbcContext'
             f' config={repr(self.config)},'
             f' api_client={repr(self.api_client)},'
+            f' document_db_client={repr(self.document_db_client)},'
             f' user={repr(self.user)},'
             f' company={repr(self.company)},'
             f' asset={repr(self.asset)},'
             f' agent={repr(self.agent)},'
             f'>'
         )
```

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/types.py` & `ixoncdkingress-0.0.8/ixoncdkingress/types.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/config.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/config.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/form.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/form.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 HTML form generator
 """
 from typing import Optional, Dict, Set, Tuple, TYPE_CHECKING
 from urllib.parse import parse_qs
 
 from ixoncdkingress.cbc.api_client import ApiClient
-from ixoncdkingress.cbc.context import CbcContext, CbcIxapiResource
+from ixoncdkingress.cbc.context import CbcContext, CbcResource
 from ixoncdkingress.types import FunctionLocation, FunctionArguments
 from ixoncdkingress.webserver.config import Config
 from ixoncdkingress.webserver.utils import parse_function_location
 
 try:
     from dominate.document import document
     from dominate.tags import h1, form, div, label, input_, h3, table, thead, \
@@ -143,61 +143,69 @@
     """
 
     in_put = parse_qs(body)
 
     context = CbcContext(
         context_config,
         api_client=ApiClient(config.api_client_base_url),
+        document_db_client=None,
         user=_parse_resource('user__', in_put, False),
         company=_parse_resource('company__', in_put, True),
         asset=_parse_resource('asset__', in_put, True),
         agent=_parse_resource('agent__', in_put, True)
     )
 
     function_location = parse_function_location(in_put.get('function', [''])[0])
     function_arguments = _parse_function_args(in_put)
 
     return context, function_location, function_arguments
 
 def _parse_function_args(in_put: dict[str, list[str]]) -> FunctionArguments:
     function_arguments = {}
-    i = 0
-    while in_put.get(f'function_args__key{i}') and in_put.get(f'function_args__value{i}'):
-        function_arguments[in_put[f'function_args__key{i}'][0]] = \
-            in_put[f'function_args__value{i}'][0]
-        i += 1
+    for in_put_key, in_put_value in in_put.items():
+        if not in_put_key.startswith('function_args__key'):
+            continue
+
+        key_argument_value = f'function_args__value{in_put_key[18:]}'
+        if key_argument_value not in in_put:
+            continue
+
+        function_arguments[in_put_value[0]] = in_put[key_argument_value][0]
 
     return function_arguments
 
 def _parse_resource(
         prefix: str,
         in_put: dict[str, list[str]],
         has_permissions: bool
-    ) -> Optional[CbcIxapiResource]:
+    ) -> Optional[CbcResource]:
     """
     Reads a resource description from the in_put and returns it as a CbcResource.
     """
     props = {}
-    permissions: Optional[Set[str]] = None
+    permissions: Optional[Set[str]] = set() if has_permissions else None
     if not in_put.get(f'{prefix}public_id') or not in_put.get(f'{prefix}name'):
         return None
 
-    prop_iterator = 0
-    prop_prefix = f'{prefix}custom_properties__'
-    while (in_put.get(f'{prop_prefix}key{prop_iterator}')
-           and in_put.get(f'{prop_prefix}value{prop_iterator}')):
-        permission = in_put[f'{prop_prefix}value{prop_iterator}'][0]
-        props[in_put[f'{prop_prefix}key{prop_iterator}'][0]] = permission
-        prop_iterator += 1
-
-    if has_permissions:
-        permissions = set()
-        permission_iterator = 0
-        permission_prefix = f'{prefix}permissions__'
-        while in_put.get(f'{permission_prefix}value{permission_iterator}'):
-            permissions.add(in_put[f'{permission_prefix}value{permission_iterator}'][0])
-            permission_iterator += 1
+    custom_property_prefix = f'{prefix}custom_properties__'
+    permission_prefix = f'{prefix}permissions__value'
+    for in_put_key, in_put_value in in_put.items():
+
+        # Process custom property
+        if in_put_key.startswith(f'{custom_property_prefix}key'):
+            custom_property_index = in_put_key[len(f'{custom_property_prefix}key'):]
+            key_custom_property_value = f'{custom_property_prefix}value{custom_property_index}'
+            if key_custom_property_value not in in_put:
+                continue
+
+            props[in_put_value[0]] = in_put[key_custom_property_value][0]
+            continue
+
+        # Process permission
+        if has_permissions and in_put_key.startswith(permission_prefix):
+            assert isinstance(permissions, set) # type hint
+            permissions.add(in_put_value[0])
 
-    return CbcIxapiResource(in_put[f'{prefix}public_id'][0],
+    return CbcResource(in_put[f'{prefix}public_id'][0],
                             in_put[f'{prefix}name'][0],
                             props,
                             permissions)
```

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/request.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/request.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/response.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/response.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/servlet.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/servlet.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/utils.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,22 @@
 """
 import json
 
 from typing import Any, Dict, Tuple
 from urllib.parse import parse_qs
 
 from ixoncdkingress.cbc.api_client import ApiClient, Query
-from ixoncdkingress.cbc.context import CbcIxapiResource, CbcContext
+from ixoncdkingress.cbc.context import CbcResource, CbcContext
 from ixoncdkingress.types import FunctionLocation, FunctionArguments
 from ixoncdkingress.webserver.config import Config
 
+from ixoncdkingress.cbc.document_db_client import (
+    DocumentDBAuthentication, DocumentDBClient, DocumentDBConnection
+)
+
 def read_qs_as_dict(in_put: bytes) -> Dict[str, str]:
     """
     Reads and parses the URL query string, returns it as a dict with for each value only the first
     occurrence.
     """
     body = in_put.decode('utf-8')
 
@@ -34,41 +38,41 @@
     if not function_path:
         return 'functions', function_name
 
     return module_name, function_name
 
 def _parse_context_values(context_items: Dict[str, Any]) -> Dict[str, Any]:
     """
-    Parses expected context_items into CbcIxapiResources
+    Parses expected context_items into CbcResources
     and discards any unexpected context_items.
     """
     context_values = {}
     for context_name, context_resource in context_items.items():
         # context_values.apiApplication and .accessToken will be sent to the CbcContext
         # but are unused, they are only used to create the ApiClient.
         if (context_name not in
                 ['user', 'company', 'agent', 'asset', 'apiApplication', 'accessToken']):
             continue
 
         if context_resource is None:
             continue
 
-        # accessToken is not a CbcIxapiResource because it doesn't have
+        # accessToken is not a CbcResource because it doesn't have
         # a publicId, name and custom field.
         if context_name == 'accessToken':
             context_values[context_name] = context_resource.get('headerValue')
             continue
 
         permissions = None
         if context_name in ['company', 'agent', 'asset']:
             permissions = set()
             if 'permissions' in context_resource:
                 permissions.update(context_resource['permissions'])
 
-        context_values[context_name] = CbcIxapiResource(
+        context_values[context_name] = CbcResource(
             context_resource['publicId'],
             context_resource['name'],
             context_resource['custom'],
             permissions,
         )
 
     return context_values
@@ -140,12 +144,25 @@
                         query=query,
                     )
                     api_data['asset'] = asset_res['data']
 
             # Overwrite existing context_values
             context_values = _parse_context_values(api_data)
 
-    context = CbcContext(context_config, api_client, **context_values)
+    document_db_client = None
+    if ((db_config := in_put.get('internalConfig', {}).get('dbConfig'))
+            and context_values.get('company')
+        ):
+        # The database name is the public id of the company
+        # The collection name is the public id of the backend component template
+        document_db_client = DocumentDBClient(
+            DocumentDBConnection(host=db_config['host'], port=int(db_config['port'])),
+            context_values['company'].public_id,
+            in_put['internalConfig']['publicId'],
+            DocumentDBAuthentication(username=db_config['username'], password=db_config['password'])
+        )
+
+    context = CbcContext(context_config, api_client, document_db_client, **context_values)
 
     function_arguments = in_put.get('arguments', {})
 
     return context, function_location, function_arguments
```

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress/webserver/wsgi.py` & `ixoncdkingress-0.0.8/ixoncdkingress/webserver/wsgi.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/ixoncdkingress.egg-info/SOURCES.txt` & `ixoncdkingress-0.0.8/ixoncdkingress.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ixoncdkingress.egg-info/dependency_links.txt
 ixoncdkingress.egg-info/requires.txt
 ixoncdkingress.egg-info/top_level.txt
 ixoncdkingress/cbc/__init__.py
 ixoncdkingress/cbc/api_client.py
 ixoncdkingress/cbc/caller.py
 ixoncdkingress/cbc/context.py
+ixoncdkingress/cbc/document_db_client.py
 ixoncdkingress/webserver/__init__.py
 ixoncdkingress/webserver/config.py
 ixoncdkingress/webserver/form.py
 ixoncdkingress/webserver/request.py
 ixoncdkingress/webserver/response.py
 ixoncdkingress/webserver/servlet.py
 ixoncdkingress/webserver/utils.py
```

### Comparing `ixoncdkingress-0.0.7/setup.py` & `ixoncdkingress-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,24 +15,25 @@
     'pytest-mock==3.8.2',
     'types-requests>=2.28.11.5',
     'wouter==0.0.3',
 ]
 
 setup(
     name='ixoncdkingress',
-    version='0.0.7',
+    version='0.0.8',
     description='IXON CDK Ingress used in Custom Backend Components(CBC) for the IXON Cloud',
     author='IXON',
     author_email='development@ixon.cloud',
     url='https://www.ixon.cloud/',
     packages=find_packages(exclude=['tests*', ]),
     package_data={
         '': ['py.typed', 'assets/*'],
     },
     python_requires='>=3.9',
     install_requires=[
+        'pymongo>=4.4.0',
         'requests>=2.28.1',
     ],
     extras_require={
         'development': development_requires,
     },
 )
```

### Comparing `ixoncdkingress-0.0.7/tests/test___main__.py` & `ixoncdkingress-0.0.8/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `ixoncdkingress-0.0.7/tests/test_utils.py` & `ixoncdkingress-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

