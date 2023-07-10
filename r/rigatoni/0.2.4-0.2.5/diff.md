# Comparing `tmp/rigatoni-0.2.4.tar.gz` & `tmp/rigatoni-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigatoni-0.2.4.tar", last modified: Sat Jul  8 17:35:03 2023, max compression
+gzip compressed data, was "rigatoni-0.2.5.tar", last modified: Mon Jul 10 15:00:16 2023, max compression
```

## Comparing `rigatoni-0.2.4.tar` & `rigatoni-0.2.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     3506 2023-06-20 19:54:44.942275 rigatoni-0.2.4/.github/workflows/continuous_integration.yml
--rw-r--r--   0        0        0     1421 2023-05-05 15:45:08.191319 rigatoni-0.2.4/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1047 2023-05-05 15:45:08.191768 rigatoni-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1119 2023-06-20 19:54:44.945276 rigatoni-0.2.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     3135 2023-06-13 16:27:24.044950 rigatoni-0.2.4/.gitignore
--rw-r--r--   0        0        0     1101 2022-08-12 15:03:40.714647 rigatoni-0.2.4/LICENSE
--rw-r--r--   0        0        0     1945 2023-06-21 19:05:15.039195 rigatoni-0.2.4/README.md
--rw-r--r--   0        0        0      115 2023-06-15 19:54:17.470002 rigatoni-0.2.4/docs/.pages
--rw-r--r--   0        0        0       58 2023-06-15 15:57:38.411606 rigatoni-0.2.4/docs/api_reference/.pages
--rw-r--r--   0        0        0      352 2023-06-15 18:27:29.368893 rigatoni-0.2.4/docs/api_reference/components.md
--rw-r--r--   0        0        0      368 2023-06-26 21:08:32.850540 rigatoni-0.2.4/docs/api_reference/geometry.md
--rw-r--r--   0        0        0      231 2023-06-14 18:11:17.854247 rigatoni-0.2.4/docs/api_reference/server.md
--rw-r--r--   0        0        0     1206 2023-06-15 18:47:51.441171 rigatoni-0.2.4/docs/api_reference/support_objects.md
--rw-r--r--   0        0        0    40440 2023-06-15 19:28:11.494980 rigatoni-0.2.4/docs/assets/concepts.svg
--rw-r--r--   0        0        0      968 2023-06-15 14:35:12.652491 rigatoni-0.2.4/docs/assets/favicon.png
--rw-r--r--   0        0        0     1254 2023-06-15 14:35:10.529923 rigatoni-0.2.4/docs/assets/logo.svg
--rw-r--r--   0        0        0     3321 2023-06-21 14:17:01.116762 rigatoni-0.2.4/docs/basic_usage.md
--rw-r--r--   0        0        0     3077 2023-06-21 14:50:48.227826 rigatoni-0.2.4/docs/index.md
--rw-r--r--   0        0        0      824 2023-06-14 23:48:11.136509 rigatoni-0.2.4/docs/install.md
--rw-r--r--   0        0        0     1592 2023-06-15 19:56:42.301700 rigatoni-0.2.4/docs/noodles.md
--rw-r--r--   0        0        0      808 2023-06-14 21:17:16.319749 rigatoni-0.2.4/docs/quick_start.md
--rw-r--r--   0        0        0     1464 2023-06-20 19:39:07.963858 rigatoni-0.2.4/mkdocs.yml
--rw-r--r--   0        0        0      942 2023-06-20 19:55:39.438455 rigatoni-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       45 2023-07-07 17:41:39.859872 rigatoni-0.2.4/requirements.txt
--rw-r--r--   0        0        0      947 2023-07-08 17:33:49.679166 rigatoni-0.2.4/rigatoni/__init__.py
--rw-r--r--   0        0        0     4804 2023-06-20 19:51:39.651166 rigatoni-0.2.4/rigatoni/byte_server.py
--rw-r--r--   0        0        0    43479 2023-07-08 17:05:47.244627 rigatoni-0.2.4/rigatoni/core.py
--rw-r--r--   0        0        0      467 2023-06-26 21:08:32.836421 rigatoni-0.2.4/rigatoni/geometry/__init__.py
--rw-r--r--   0        0        0    31969 2023-06-28 15:14:39.539867 rigatoni-0.2.4/rigatoni/geometry/methods.py
--rw-r--r--   0        0        0     1498 2023-06-22 21:03:55.102593 rigatoni-0.2.4/rigatoni/geometry/objects.py
--rw-r--r--   0        0        0    30416 2023-07-08 17:33:04.117093 rigatoni-0.2.4/rigatoni/noodle_objects.py
--rw-r--r--   0        0        0        0 2023-05-05 15:45:08.200874 rigatoni-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     8622 2023-06-14 20:03:53.431955 rigatoni-0.2.4/tests/clients.py
--rw-r--r--   0        0        0        0 2023-05-05 15:45:08.201078 rigatoni-0.2.4/tests/examples/__init__.py
--rw-r--r--   0        0        0     8158 2023-06-21 17:44:26.776995 rigatoni-0.2.4/tests/examples/basic_server.py
--rw-r--r--   0        0        0    11872 2023-07-07 17:33:30.120374 rigatoni-0.2.4/tests/examples/geometry_server.py
--rw-r--r--   0        0        0  2309522 2023-05-05 15:45:08.213596 rigatoni-0.2.4/tests/mesh_data/boot.obj
--rw-r--r--   0        0        0     2898 2023-06-20 13:49:01.077673 rigatoni-0.2.4/tests/mesh_data/box.gltf
--rw-r--r--   0        0        0      648 2023-06-20 13:48:02.901111 rigatoni-0.2.4/tests/mesh_data/box0.bin
--rw-r--r--   0        0        0   205922 2023-05-05 15:45:08.216659 rigatoni-0.2.4/tests/mesh_data/data.csv
--rw-r--r--   0        0        0  2408417 2023-05-05 15:45:08.232076 rigatoni-0.2.4/tests/mesh_data/stanford-bunny.obj
--rw-r--r--   0        0        0  3645817 2023-07-07 17:36:00.242186 rigatoni-0.2.4/tests/mesh_data/test_mesh.obj
--rw-r--r--   0        0        0     3106 2023-07-07 17:35:56.388919 rigatoni-0.2.4/tests/mesh_data/test_sphere.obj
--rw-r--r--   0        0        0     3347 2023-06-20 18:13:41.376089 rigatoni-0.2.4/tests/servers.py
--rw-r--r--   0        0        0      795 2023-07-07 18:02:05.023194 rigatoni-0.2.4/tests/test_byte_server.py
--rw-r--r--   0        0        0    12489 2023-06-20 22:05:38.111108 rigatoni-0.2.4/tests/test_core.py
--rw-r--r--   0        0        0    12643 2023-07-07 17:28:51.869864 rigatoni-0.2.4/tests/test_geometry_creation.py
--rw-r--r--   0        0        0     5183 2023-06-20 19:28:59.553008 rigatoni-0.2.4/tests/test_noodle_objects.py
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3506 2023-06-20 19:54:44.942275 rigatoni-0.2.5/.github/workflows/continuous_integration.yml
+-rw-r--r--   0        0        0     1421 2023-05-05 15:45:08.191319 rigatoni-0.2.5/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1047 2023-05-05 15:45:08.191768 rigatoni-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1119 2023-06-20 19:54:44.945276 rigatoni-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3135 2023-06-13 16:27:24.044950 rigatoni-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1101 2022-08-12 15:03:40.714647 rigatoni-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1945 2023-06-21 19:05:15.039195 rigatoni-0.2.5/README.md
+-rw-r--r--   0        0        0      115 2023-06-15 19:54:17.470002 rigatoni-0.2.5/docs/.pages
+-rw-r--r--   0        0        0       58 2023-06-15 15:57:38.411606 rigatoni-0.2.5/docs/api_reference/.pages
+-rw-r--r--   0        0        0      352 2023-06-15 18:27:29.368893 rigatoni-0.2.5/docs/api_reference/components.md
+-rw-r--r--   0        0        0      368 2023-06-26 21:08:32.850540 rigatoni-0.2.5/docs/api_reference/geometry.md
+-rw-r--r--   0        0        0      231 2023-06-14 18:11:17.854247 rigatoni-0.2.5/docs/api_reference/server.md
+-rw-r--r--   0        0        0     1206 2023-06-15 18:47:51.441171 rigatoni-0.2.5/docs/api_reference/support_objects.md
+-rw-r--r--   0        0        0    40440 2023-06-15 19:28:11.494980 rigatoni-0.2.5/docs/assets/concepts.svg
+-rw-r--r--   0        0        0      968 2023-06-15 14:35:12.652491 rigatoni-0.2.5/docs/assets/favicon.png
+-rw-r--r--   0        0        0     1254 2023-06-15 14:35:10.529923 rigatoni-0.2.5/docs/assets/logo.svg
+-rw-r--r--   0        0        0     3321 2023-06-21 14:17:01.116762 rigatoni-0.2.5/docs/basic_usage.md
+-rw-r--r--   0        0        0     3077 2023-06-21 14:50:48.227826 rigatoni-0.2.5/docs/index.md
+-rw-r--r--   0        0        0      824 2023-06-14 23:48:11.136509 rigatoni-0.2.5/docs/install.md
+-rw-r--r--   0        0        0     1592 2023-06-15 19:56:42.301700 rigatoni-0.2.5/docs/noodles.md
+-rw-r--r--   0        0        0      808 2023-06-14 21:17:16.319749 rigatoni-0.2.5/docs/quick_start.md
+-rw-r--r--   0        0        0     1464 2023-06-20 19:39:07.963858 rigatoni-0.2.5/mkdocs.yml
+-rw-r--r--   0        0        0      942 2023-06-20 19:55:39.438455 rigatoni-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-07-07 17:41:39.859872 rigatoni-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      947 2023-07-10 15:00:05.271752 rigatoni-0.2.5/rigatoni/__init__.py
+-rw-r--r--   0        0        0     4804 2023-06-20 19:51:39.651166 rigatoni-0.2.5/rigatoni/byte_server.py
+-rw-r--r--   0        0        0    43479 2023-07-08 17:05:47.244627 rigatoni-0.2.5/rigatoni/core.py
+-rw-r--r--   0        0        0      467 2023-06-26 21:08:32.836421 rigatoni-0.2.5/rigatoni/geometry/__init__.py
+-rw-r--r--   0        0        0    31969 2023-06-28 15:14:39.539867 rigatoni-0.2.5/rigatoni/geometry/methods.py
+-rw-r--r--   0        0        0     1498 2023-06-22 21:03:55.102593 rigatoni-0.2.5/rigatoni/geometry/objects.py
+-rw-r--r--   0        0        0    30202 2023-07-10 14:42:48.220576 rigatoni-0.2.5/rigatoni/noodle_objects.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:45:08.200874 rigatoni-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     8622 2023-06-14 20:03:53.431955 rigatoni-0.2.5/tests/clients.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:45:08.201078 rigatoni-0.2.5/tests/examples/__init__.py
+-rw-r--r--   0        0        0     8158 2023-06-21 17:44:26.776995 rigatoni-0.2.5/tests/examples/basic_server.py
+-rw-r--r--   0        0        0    11872 2023-07-07 17:33:30.120374 rigatoni-0.2.5/tests/examples/geometry_server.py
+-rw-r--r--   0        0        0  2309522 2023-05-05 15:45:08.213596 rigatoni-0.2.5/tests/mesh_data/boot.obj
+-rw-r--r--   0        0        0     2898 2023-06-20 13:49:01.077673 rigatoni-0.2.5/tests/mesh_data/box.gltf
+-rw-r--r--   0        0        0      648 2023-06-20 13:48:02.901111 rigatoni-0.2.5/tests/mesh_data/box0.bin
+-rw-r--r--   0        0        0   205922 2023-05-05 15:45:08.216659 rigatoni-0.2.5/tests/mesh_data/data.csv
+-rw-r--r--   0        0        0  2408417 2023-05-05 15:45:08.232076 rigatoni-0.2.5/tests/mesh_data/stanford-bunny.obj
+-rw-r--r--   0        0        0  3645817 2023-07-07 17:36:00.242186 rigatoni-0.2.5/tests/mesh_data/test_mesh.obj
+-rw-r--r--   0        0        0     3106 2023-07-07 17:35:56.388919 rigatoni-0.2.5/tests/mesh_data/test_sphere.obj
+-rw-r--r--   0        0        0     3347 2023-06-20 18:13:41.376089 rigatoni-0.2.5/tests/servers.py
+-rw-r--r--   0        0        0      795 2023-07-07 18:02:05.023194 rigatoni-0.2.5/tests/test_byte_server.py
+-rw-r--r--   0        0        0    12489 2023-06-20 22:05:38.111108 rigatoni-0.2.5/tests/test_core.py
+-rw-r--r--   0        0        0    12643 2023-07-07 17:28:51.869864 rigatoni-0.2.5/tests/test_geometry_creation.py
+-rw-r--r--   0        0        0     5183 2023-06-20 19:28:59.553008 rigatoni-0.2.5/tests/test_noodle_objects.py
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.5/PKG-INFO
```

### Comparing `rigatoni-0.2.4/.github/workflows/continuous_integration.yml` & `rigatoni-0.2.5/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/.github/workflows/coverage.yml` & `rigatoni-0.2.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/.github/workflows/python-publish.yml` & `rigatoni-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/.github/workflows/test.yml` & `rigatoni-0.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/.gitignore` & `rigatoni-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/LICENSE` & `rigatoni-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/README.md` & `rigatoni-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/api_reference/support_objects.md` & `rigatoni-0.2.5/docs/api_reference/support_objects.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/assets/concepts.svg` & `rigatoni-0.2.5/docs/assets/concepts.svg`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/assets/favicon.png` & `rigatoni-0.2.5/docs/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/assets/logo.svg` & `rigatoni-0.2.5/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/basic_usage.md` & `rigatoni-0.2.5/docs/basic_usage.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/index.md` & `rigatoni-0.2.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/install.md` & `rigatoni-0.2.5/docs/install.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/noodles.md` & `rigatoni-0.2.5/docs/noodles.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/docs/quick_start.md` & `rigatoni-0.2.5/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/mkdocs.yml` & `rigatoni-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/pyproject.toml` & `rigatoni-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/rigatoni/__init__.py` & `rigatoni-0.2.5/rigatoni/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         objects.py
     delegates.py
     noodle_objects.py
     server.py
 """
 
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 from .core import Server
 from .noodle_objects import *
 from .byte_server import ByteServer
 
 # Ensure that dependencies are installed for optional module
 try:
```

### Comparing `rigatoni-0.2.4/rigatoni/byte_server.py` & `rigatoni-0.2.5/rigatoni/byte_server.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/rigatoni/core.py` & `rigatoni-0.2.5/rigatoni/core.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/rigatoni/geometry/methods.py` & `rigatoni-0.2.5/rigatoni/geometry/methods.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/rigatoni/geometry/objects.py` & `rigatoni-0.2.5/rigatoni/geometry/objects.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/rigatoni/noodle_objects.py` & `rigatoni-0.2.5/rigatoni/noodle_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -507,26 +507,20 @@
         plot (Optional[PlotID]): Plot to invoke signal on
     """
     entity: Optional[EntityID] = None
     table: Optional[TableID] = None
     plot: Optional[PlotID] = None
 
     @model_validator(mode="after")
-    def one_of_three(cls, values):
-        already_found = False
-        for field in values:
-            if values[field] and already_found:
-                raise ValueError("More than one field entered")
-            elif values[field]:
-                already_found = True
-
-        if not already_found:
-            raise ValueError("No field provided")
-        else:
-            return values
+    def one_of_three(cls, model):
+        """Ensure only one of the three attributes is set"""
+        selected = bool(model.entity) + bool(model.table) + bool(model.plot)
+        if selected != 1:
+            raise ValueError("Must select exactly one of entity, table, or plot")
+        return model
 
 
 class TableColumnInfo(NoodleObject):
     """Information about a column in a table
 
     Attributes:
         name (str): Name of column
@@ -548,23 +542,23 @@
     columns: List[TableColumnInfo]
     keys: List[int]
     data: List[List[Any]]  # Originally tried union, but currently order is used to coerce by pydantic
     selections: Optional[List[Selection]] = None
 
     # too much overhead? - strict mode
     @model_validator(mode="after")
-    def types_match(cls, values):
-        for row in values['data']:
-            for col, i in zip(values['columns'], range(len(row))):
+    def types_match(cls, model):
+        for row in model.data:
+            for col, i in zip(model.columns, range(len(row))):
                 text_mismatch = isinstance(row[i], str) and col.type != "TEXT"
                 real_mismatch = isinstance(row[i], float) and col.type != "REAL"
                 int_mismatch = isinstance(row[i], int) and col.type != "INTEGER"
                 if text_mismatch or real_mismatch or int_mismatch:
                     raise ValueError(f"Column Info doesn't match type in data: {col, row[i]}")
-        return values
+        return model
 
 
 """ ====================== NOODLE COMPONENTS / DELEGATES ====================== """
 
 
 class Method(Delegate):
     """A method that clients can request the server to call.
@@ -661,17 +655,17 @@
     simple_plot: Optional[str] = None
     url_plot: Optional[str] = None
 
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
     @model_validator(mode="after")
-    def one_of(cls, values):
-        if bool(values['simple_plot']) != bool(values['url_plot']):
-            return values
+    def one_of(cls, model):
+        if bool(model.simple_plot) != bool(model.url_plot):
+            return model
         else:
             raise ValueError("One plot type must be specified")
 
 
 class Buffer(Delegate):
     """A buffer of bytes containing data for an image or a mesh.
 
@@ -686,17 +680,17 @@
     name: Optional[str] = None
     size: int = None
 
     inline_bytes: bytes = None
     uri_bytes: str = None
 
     @model_validator(mode="after")
-    def one_of(cls, values):
-        if bool(values['inline_bytes']) != bool(values['uri_bytes']):
-            return values
+    def one_of(cls, model):
+        if bool(model.inline_bytes) != bool(model.uri_bytes):
+            return model
         else:
             raise ValueError("One plot type must be specified")
 
 
 class BufferView(Delegate):
     """A view into a buffer, specifying a subset of the buffer and how to interpret it.
 
@@ -763,17 +757,17 @@
     id: ImageID
     name: Optional[str] = None
 
     buffer_source: BufferID = None
     uri_source: str = None
 
     @model_validator(mode="after")
-    def one_of(cls, values):
-        if bool(values['buffer_source']) != bool(values['uri_source']):
-            return values
+    def one_of(cls, model):
+        if bool(model.buffer_source) != bool(model.uri_source):
+            return model
         else:
             raise ValueError("One plot type must be specified")
 
 
 class Texture(Delegate):
     """A texture, can be used for a material
 
@@ -829,26 +823,22 @@
     intensity: Optional[float] = 1.0
 
     point: PointLight = None
     spot: SpotLight = None
     directional: DirectionalLight = None
 
     @model_validator(mode="after")
-    def one_of(cls, values):
-        already_found = False
-        for field in ['point', 'spot', 'directional']:
-            if values[field] and already_found:
-                raise ValueError("More than one field entered")
-            elif values[field]:
-                already_found = True
-
-        if not already_found:
-            raise ValueError("No field provided")
+    def one_of(cls, model):
+        num_selected = bool(model.point) + bool(model.spot) + bool(model.directional)
+        if num_selected > 1:
+            raise ValueError("Only one light type can be selected")
+        elif num_selected == 0:
+            raise ValueError("No light type selected")
         else:
-            return values
+            return model
 
 
 class Geometry(Delegate):
     """Represents geometry in the scene and can be used for meshes
 
     Attributes:
         id: ID for the geometry
```

### Comparing `rigatoni-0.2.4/tests/clients.py` & `rigatoni-0.2.5/tests/clients.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/examples/basic_server.py` & `rigatoni-0.2.5/tests/examples/basic_server.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/examples/geometry_server.py` & `rigatoni-0.2.5/tests/examples/geometry_server.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/boot.obj` & `rigatoni-0.2.5/tests/mesh_data/boot.obj`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/box.gltf` & `rigatoni-0.2.5/tests/mesh_data/box.gltf`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/box0.bin` & `rigatoni-0.2.5/tests/mesh_data/box0.bin`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/data.csv` & `rigatoni-0.2.5/tests/mesh_data/data.csv`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/stanford-bunny.obj` & `rigatoni-0.2.5/tests/mesh_data/stanford-bunny.obj`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/test_mesh.obj` & `rigatoni-0.2.5/tests/mesh_data/test_mesh.obj`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/mesh_data/test_sphere.obj` & `rigatoni-0.2.5/tests/mesh_data/test_sphere.obj`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/servers.py` & `rigatoni-0.2.5/tests/servers.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/test_byte_server.py` & `rigatoni-0.2.5/tests/test_byte_server.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/test_core.py` & `rigatoni-0.2.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/test_geometry_creation.py` & `rigatoni-0.2.5/tests/test_geometry_creation.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/tests/test_noodle_objects.py` & `rigatoni-0.2.5/tests/test_noodle_objects.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.4/PKG-INFO` & `rigatoni-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigatoni
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Server Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,server,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

