# Comparing `tmp/rigatoni-0.2.5.tar.gz` & `tmp/rigatoni-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigatoni-0.2.5.tar", last modified: Mon Jul 10 15:00:16 2023, max compression
+gzip compressed data, was "rigatoni-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rigatoni-0.2.5.tar` & `rigatoni-0.2.6.tar`

### file list

```diff
@@ -1,49 +1,10 @@
--rw-r--r--   0        0        0     3506 2023-06-20 19:54:44.942275 rigatoni-0.2.5/.github/workflows/continuous_integration.yml
--rw-r--r--   0        0        0     1421 2023-05-05 15:45:08.191319 rigatoni-0.2.5/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1047 2023-05-05 15:45:08.191768 rigatoni-0.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1119 2023-06-20 19:54:44.945276 rigatoni-0.2.5/.github/workflows/test.yml
--rw-r--r--   0        0        0     3135 2023-06-13 16:27:24.044950 rigatoni-0.2.5/.gitignore
--rw-r--r--   0        0        0     1101 2022-08-12 15:03:40.714647 rigatoni-0.2.5/LICENSE
--rw-r--r--   0        0        0     1945 2023-06-21 19:05:15.039195 rigatoni-0.2.5/README.md
--rw-r--r--   0        0        0      115 2023-06-15 19:54:17.470002 rigatoni-0.2.5/docs/.pages
--rw-r--r--   0        0        0       58 2023-06-15 15:57:38.411606 rigatoni-0.2.5/docs/api_reference/.pages
--rw-r--r--   0        0        0      352 2023-06-15 18:27:29.368893 rigatoni-0.2.5/docs/api_reference/components.md
--rw-r--r--   0        0        0      368 2023-06-26 21:08:32.850540 rigatoni-0.2.5/docs/api_reference/geometry.md
--rw-r--r--   0        0        0      231 2023-06-14 18:11:17.854247 rigatoni-0.2.5/docs/api_reference/server.md
--rw-r--r--   0        0        0     1206 2023-06-15 18:47:51.441171 rigatoni-0.2.5/docs/api_reference/support_objects.md
--rw-r--r--   0        0        0    40440 2023-06-15 19:28:11.494980 rigatoni-0.2.5/docs/assets/concepts.svg
--rw-r--r--   0        0        0      968 2023-06-15 14:35:12.652491 rigatoni-0.2.5/docs/assets/favicon.png
--rw-r--r--   0        0        0     1254 2023-06-15 14:35:10.529923 rigatoni-0.2.5/docs/assets/logo.svg
--rw-r--r--   0        0        0     3321 2023-06-21 14:17:01.116762 rigatoni-0.2.5/docs/basic_usage.md
--rw-r--r--   0        0        0     3077 2023-06-21 14:50:48.227826 rigatoni-0.2.5/docs/index.md
--rw-r--r--   0        0        0      824 2023-06-14 23:48:11.136509 rigatoni-0.2.5/docs/install.md
--rw-r--r--   0        0        0     1592 2023-06-15 19:56:42.301700 rigatoni-0.2.5/docs/noodles.md
--rw-r--r--   0        0        0      808 2023-06-14 21:17:16.319749 rigatoni-0.2.5/docs/quick_start.md
--rw-r--r--   0        0        0     1464 2023-06-20 19:39:07.963858 rigatoni-0.2.5/mkdocs.yml
--rw-r--r--   0        0        0      942 2023-06-20 19:55:39.438455 rigatoni-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       45 2023-07-07 17:41:39.859872 rigatoni-0.2.5/requirements.txt
--rw-r--r--   0        0        0      947 2023-07-10 15:00:05.271752 rigatoni-0.2.5/rigatoni/__init__.py
--rw-r--r--   0        0        0     4804 2023-06-20 19:51:39.651166 rigatoni-0.2.5/rigatoni/byte_server.py
--rw-r--r--   0        0        0    43479 2023-07-08 17:05:47.244627 rigatoni-0.2.5/rigatoni/core.py
--rw-r--r--   0        0        0      467 2023-06-26 21:08:32.836421 rigatoni-0.2.5/rigatoni/geometry/__init__.py
--rw-r--r--   0        0        0    31969 2023-06-28 15:14:39.539867 rigatoni-0.2.5/rigatoni/geometry/methods.py
--rw-r--r--   0        0        0     1498 2023-06-22 21:03:55.102593 rigatoni-0.2.5/rigatoni/geometry/objects.py
--rw-r--r--   0        0        0    30202 2023-07-10 14:42:48.220576 rigatoni-0.2.5/rigatoni/noodle_objects.py
--rw-r--r--   0        0        0        0 2023-05-05 15:45:08.200874 rigatoni-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     8622 2023-06-14 20:03:53.431955 rigatoni-0.2.5/tests/clients.py
--rw-r--r--   0        0        0        0 2023-05-05 15:45:08.201078 rigatoni-0.2.5/tests/examples/__init__.py
--rw-r--r--   0        0        0     8158 2023-06-21 17:44:26.776995 rigatoni-0.2.5/tests/examples/basic_server.py
--rw-r--r--   0        0        0    11872 2023-07-07 17:33:30.120374 rigatoni-0.2.5/tests/examples/geometry_server.py
--rw-r--r--   0        0        0  2309522 2023-05-05 15:45:08.213596 rigatoni-0.2.5/tests/mesh_data/boot.obj
--rw-r--r--   0        0        0     2898 2023-06-20 13:49:01.077673 rigatoni-0.2.5/tests/mesh_data/box.gltf
--rw-r--r--   0        0        0      648 2023-06-20 13:48:02.901111 rigatoni-0.2.5/tests/mesh_data/box0.bin
--rw-r--r--   0        0        0   205922 2023-05-05 15:45:08.216659 rigatoni-0.2.5/tests/mesh_data/data.csv
--rw-r--r--   0        0        0  2408417 2023-05-05 15:45:08.232076 rigatoni-0.2.5/tests/mesh_data/stanford-bunny.obj
--rw-r--r--   0        0        0  3645817 2023-07-07 17:36:00.242186 rigatoni-0.2.5/tests/mesh_data/test_mesh.obj
--rw-r--r--   0        0        0     3106 2023-07-07 17:35:56.388919 rigatoni-0.2.5/tests/mesh_data/test_sphere.obj
--rw-r--r--   0        0        0     3347 2023-06-20 18:13:41.376089 rigatoni-0.2.5/tests/servers.py
--rw-r--r--   0        0        0      795 2023-07-07 18:02:05.023194 rigatoni-0.2.5/tests/test_byte_server.py
--rw-r--r--   0        0        0    12489 2023-06-20 22:05:38.111108 rigatoni-0.2.5/tests/test_core.py
--rw-r--r--   0        0        0    12643 2023-07-07 17:28:51.869864 rigatoni-0.2.5/tests/test_geometry_creation.py
--rw-r--r--   0        0        0     5183 2023-06-20 19:28:59.553008 rigatoni-0.2.5/tests/test_noodle_objects.py
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1945 2023-07-10 20:45:16.440916 rigatoni-0.2.6/README.md
+-rw-r--r--   0        0        0      942 2023-07-10 20:45:16.440916 rigatoni-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      947 2023-07-10 20:45:16.440916 rigatoni-0.2.6/rigatoni/__init__.py
+-rw-r--r--   0        0        0     4804 2023-07-10 20:45:16.440916 rigatoni-0.2.6/rigatoni/byte_server.py
+-rw-r--r--   0        0        0    43539 2023-07-10 20:45:16.440916 rigatoni-0.2.6/rigatoni/core.py
+-rw-r--r--   0        0        0      467 2023-07-10 20:45:16.444916 rigatoni-0.2.6/rigatoni/geometry/__init__.py
+-rw-r--r--   0        0        0    31969 2023-07-10 20:45:16.444916 rigatoni-0.2.6/rigatoni/geometry/methods.py
+-rw-r--r--   0        0        0     1498 2023-07-10 20:45:16.444916 rigatoni-0.2.6/rigatoni/geometry/objects.py
+-rw-r--r--   0        0        0    30041 2023-07-10 20:45:16.444916 rigatoni-0.2.6/rigatoni/noodle_objects.py
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 rigatoni-0.2.6/PKG-INFO
```

### Comparing `rigatoni-0.2.5/README.md` & `rigatoni-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.5/pyproject.toml` & `rigatoni-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.5/rigatoni/__init__.py` & `rigatoni-0.2.6/rigatoni/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         objects.py
     delegates.py
     noodle_objects.py
     server.py
 """
 
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 from .core import Server
 from .noodle_objects import *
 from .byte_server import ByteServer
 
 # Ensure that dependencies are installed for optional module
 try:
```

### Comparing `rigatoni-0.2.5/rigatoni/byte_server.py` & `rigatoni-0.2.6/rigatoni/byte_server.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.5/rigatoni/core.py` & `rigatoni-0.2.6/rigatoni/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
             else:  # Normal update, include id, and any field in delta
                 delta = set() if not delta else delta
                 delta.add("id")
                 contents = noodle_object.model_dump(exclude_none=True, include=delta)
 
         elif action == "delete":
             try:
-                contents["id"] = noodle_object.id
+                contents["id"] = tuple(noodle_object.id)
             except AttributeError:
                 raise Exception(f"Cannot delete a {noodle_object}")
 
         return contents
 
     def _prepare_message(self, action: str, noodle_object: NoodleObject = None, delta: set[str] = None):
         """Given object and action, get id and message contents as dict
@@ -800,14 +800,16 @@
             name (str): name of the signal
             doc (str, optional): documentation for the signal
             arg_doc (list[MethodArg], optional): list of arguments and documentation for the signal
 
         Returns:
             Signal: signal delegate that was created
         """
+        if arg_doc is None:
+            arg_doc = []
         return self.create_component(Signal, name=name, doc=doc, arg_doc=arg_doc)
 
     def create_entity(self, name: Optional[str],
                       parent: Optional[EntityID] = None,
                       transform: Optional[Mat4] = None,
                       text_rep: Optional[TextRepresentation] = None,
                       web_rep: Optional[WebRepresentation] = None,
```

### Comparing `rigatoni-0.2.5/rigatoni/geometry/methods.py` & `rigatoni-0.2.6/rigatoni/geometry/methods.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.5/rigatoni/geometry/objects.py` & `rigatoni-0.2.6/rigatoni/geometry/objects.py`

 * *Files identical despite different names*

### Comparing `rigatoni-0.2.5/rigatoni/noodle_objects.py` & `rigatoni-0.2.6/rigatoni/noodle_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,33 +134,28 @@
         server (Server): server delegate is attached to
         id: (ID): Unique identifier for delegate
         name (Optional[str]): Name of delegate
         signals (Optional[dict]): Signals that can be called on delegate, method name to callable
     """
 
     server: object  # Better way to annotate this without introducing circular imports?
-    id: ID = None
+    id: ID
     name: Optional[str] = "No-Name"
     signals: Optional[dict] = {}
 
     def __str__(self):
         return f"{self.name} - {type(self).__name__} - {self.id.compact_str()}"
 
 
 """ ====================== Common Definitions ====================== """
 
-Vec3 = Tuple[float, float, float]
-Vec4 = Tuple[float, float, float, float]
-Mat3 = Tuple[float, float, float,
-             float, float, float,
-             float, float, float]
-Mat4 = Tuple[float, float, float, float,
-             float, float, float, float,
-             float, float, float, float,
-             float, float, float, float]
+Vec3 = List[float]  # Length 3
+Vec4 = List[float]  # Length 4
+Mat3 = List[float]  # Length 9
+Mat4 = List[float]  # Length 16
 
 RGB = Vec3
 RGBA = Vec4
 
 
 class AttributeSemantic(Enum):
     """String indicating type of attribute, used in Attribute inside of geometry patch
@@ -587,15 +582,15 @@
         doc: Documentation for the signal
         arg_doc: Documentation for the arguments
     """
 
     id: SignalID
     name: str
     doc: Optional[str] = None
-    arg_doc: List[MethodArg] = None
+    arg_doc: List[MethodArg] = []
 
 
 class Entity(Delegate):
     """Container for other entities, possibly renderable, has associated methods and signals
 
     Attributes:
         id: ID for the entity
@@ -674,18 +669,18 @@
         name: Name of the buffer
         size: Size of the buffer in bytes
         inline_bytes: Bytes of the buffer
         uri_bytes: URI for the bytes
     """
     id: BufferID
     name: Optional[str] = None
-    size: int = None
+    size: int
 
-    inline_bytes: bytes = None
-    uri_bytes: str = None
+    inline_bytes: Optional[bytes] = None
+    uri_bytes: Optional[str] = None
 
     @model_validator(mode="after")
     def one_of(cls, model):
         if bool(model.inline_bytes) != bool(model.uri_bytes):
             return model
         else:
             raise ValueError("One plot type must be specified")
@@ -753,16 +748,16 @@
         name: Name of the image
         buffer_source: Buffer that the image is stored in
         uri_source: URI for the bytes if they are hosted externally
     """
     id: ImageID
     name: Optional[str] = None
 
-    buffer_source: BufferID = None
-    uri_source: str = None
+    buffer_source: Optional[BufferID] = None
+    uri_source: Optional[str] = None
 
     @model_validator(mode="after")
     def one_of(cls, model):
         if bool(model.buffer_source) != bool(model.uri_source):
             return model
         else:
             raise ValueError("One plot type must be specified")
@@ -818,17 +813,17 @@
     """
     id: LightID
     name: Optional[str] = None
 
     color: Optional[RGB] = [1.0, 1.0, 1.0]
     intensity: Optional[float] = 1.0
 
-    point: PointLight = None
-    spot: SpotLight = None
-    directional: DirectionalLight = None
+    point: Optional[PointLight] = None
+    spot: Optional[SpotLight] = None
+    directional: Optional[DirectionalLight] = None
 
     @model_validator(mode="after")
     def one_of(cls, model):
         num_selected = bool(model.point) + bool(model.spot) + bool(model.directional)
         if num_selected > 1:
             raise ValueError("Only one light type can be selected")
         elif num_selected == 0:
@@ -901,15 +896,15 @@
         pass
 
     def table_selection_updated(self, selection: Selection):
         """Invoke table selection updated signal"""
         pass
 
 
-# TODO: need to work this in to specify which methods are avaiable in which contexts
+# TODO: need to work this in to specify which methods are available in which contexts
 class Document(Delegate):
     """Represents the scope of the whole session
 
     Attributes:
         name (str): name will be "Document"
         methods_list (list[MethodID]): list of methods available on the document
         signals_list (list[SignalID]): list of signals available on the document
```

### Comparing `rigatoni-0.2.5/PKG-INFO` & `rigatoni-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigatoni
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python Server Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,server,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

