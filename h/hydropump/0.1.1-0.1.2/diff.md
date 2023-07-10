# Comparing `tmp/hydropump-0.1.1.tar.gz` & `tmp/hydropump-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydropump-0.1.1.tar", max compression
+gzip compressed data, was "hydropump-0.1.2.tar", max compression
```

## Comparing `hydropump-0.1.1.tar` & `hydropump-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-07-10 01:52:29.959752 hydropump-0.1.1/LICENSE
--rw-r--r--   0        0        0     2573 2023-07-10 01:52:29.959752 hydropump-0.1.1/README.md
--rw-r--r--   0        0        0      214 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/__init__.py
--rw-r--r--   0        0        0    11223 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/backend.py
--rw-r--r--   0        0        0     4742 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/instruction.py
--rw-r--r--   0        0        0     6260 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/service.py
--rw-r--r--   0        0        0     3292 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/TESTING.md
--rw-r--r--   0        0        0        0 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/__init__.py
--rw-r--r--   0        0        0     1398 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/conftest.py
--rw-r--r--   0        0        0        0 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/test_instructions.py
--rw-r--r--   0        0        0       13 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/test_root/base/.gitignore
--rw-r--r--   0        0        0       13 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/test_root/template/.gitignore
--rw-r--r--   0        0        0      740 2023-07-10 01:52:29.959752 hydropump-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 hydropump-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-10 12:51:19.925666 hydropump-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2623 2023-07-10 12:51:19.925666 hydropump-0.1.2/README.md
+-rw-r--r--   0        0        0      214 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/__init__.py
+-rw-r--r--   0        0        0    11271 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/backend.py
+-rw-r--r--   0        0        0     4742 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/instruction.py
+-rw-r--r--   0        0        0     6278 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/service.py
+-rw-r--r--   0        0        0     3292 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/TESTING.md
+-rw-r--r--   0        0        0        0 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/__init__.py
+-rw-r--r--   0        0        0     1398 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/test_instructions.py
+-rw-r--r--   0        0        0       13 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/test_root/base/.gitignore
+-rw-r--r--   0        0        0       13 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/test_root/template/.gitignore
+-rw-r--r--   0        0        0      740 2023-07-10 12:51:19.925666 hydropump-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 hydropump-0.1.2/PKG-INFO
```

### Comparing `hydropump-0.1.1/LICENSE` & `hydropump-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.1/README.md` & `hydropump-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,55 +30,51 @@
     "backend_type": "FileSystem",
     "file_extension": "json",
 }
 
 service = Service(config=service_config)
 
 template_id1 = "example_template1"
-template1 = {
-    "sqlEngine": "mysql"
-}
+template1 = {"sqlEngine": "mysql"}
 service.create_template(metadata={}, source=template1, template_id=template_id1)
 
 template_id2 = "example_template2"
 template2 = {
-    "sqlEngine": "postgres"
-    "cloudProvider": "AWS"
+    "sqlEngine": "postgres",
+    "cloudProvider": "AWS",
 }
 service.create_template(metadata={}, source=template2, template_id=template_id2)
 
 instruction_id = "client-12345"
 metadata = {
     "createdBy": "mvecchione145",
-
     # templates are compiled from left to right
     # (common keys in example_template1 will be
     # overridden by values in example_template2)
-    "templates": ["example_template1", "example_template2"]
-}
-source = {
-    "system": "darwin"
+    "templates": ["example_template1", "example_template2"],
 }
+source = {"system": "darwin"}
 
 service.create_instruction(
-    instruction_id=instruction_id,
-    metadata=metadata,
-    source=source)
+    instruction_id=instruction_id, metadata=metadata, source=source
+)
 
 instruction = service.get_instruction(instruction_id=instruction_id)
 
-print(returned_payload)
+print(instruction)
 # {
 #   "instruction": {
 #     "cloudProvider": "AWS",
 #     "sqlEngine": "postgres",
 #     "system": "darwin"
 #   },
 #   "metadata": {
+#     "compiled": True,
 #     "createdBy": "mvecchione145",
+#     "createdAt": "YYYY-MM-DD HH:MM:SS.NNNNNN"
 #     "templates": [
 #       "example_template",
 #       "example_template2"
 #     ]
 #   }
 ```
```

### Comparing `hydropump-0.1.1/hydropump/backend.py` & `hydropump-0.1.2/hydropump/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             Instruction: The compiled instruction.
         """
         template = {}
         for template_id in instruction.metadata.get("templates", []):
             template_instruction = self.get_template(template_id)
             template = self._compile(template_instruction["template"], template)
         instruction.source = self._compile(instruction.source, template)
+        instruction.metadata["compiled"] = True
         instruction.set_source()
         return instruction
 
     def set_dump_load(self):
         """
         Set the dump and load functions based on the file extension.
         """
```

### Comparing `hydropump-0.1.1/hydropump/instruction.py` & `hydropump-0.1.2/hydropump/instruction.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.1/hydropump/service.py` & `hydropump-0.1.2/hydropump/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         if self.backend is None and config is None:
             self.backend = FileSystemBackend()
         if config is not None and self.backend is None:
             self.backend = self._set_backend(config)
         if not isinstance(self.backend, Backend):
             raise ValueError("Backend is not of type Backend.")
 
+    @staticmethod
     def _set_backend(config: dict) -> Backend:
         """
         Set the backend based on the provided configuration.
 
         Args:
             config (dict): The configuration options for the backend.
```

### Comparing `hydropump-0.1.1/hydropump/test/TESTING.md` & `hydropump-0.1.2/hydropump/test/TESTING.md`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.1/hydropump/test/conftest.py` & `hydropump-0.1.2/hydropump/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.1/hydropump/test/unit/test_instructions.py` & `hydropump-0.1.2/hydropump/test/unit/test_instructions.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.1/pyproject.toml` & `hydropump-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydropump"
-version = "0.1.1"
+version = "0.1.2"
 description = "Configuration Management Library"
 authors = ["Michael Vecchione <51305946+mvecchione145@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `hydropump-0.1.1/PKG-INFO` & `hydropump-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydropump
-Version: 0.1.1
+Version: 0.1.2
 Summary: Configuration Management Library
 License: MIT
 Author: Michael Vecchione
 Author-email: 51305946+mvecchione145@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -45,55 +45,51 @@
     "backend_type": "FileSystem",
     "file_extension": "json",
 }
 
 service = Service(config=service_config)
 
 template_id1 = "example_template1"
-template1 = {
-    "sqlEngine": "mysql"
-}
+template1 = {"sqlEngine": "mysql"}
 service.create_template(metadata={}, source=template1, template_id=template_id1)
 
 template_id2 = "example_template2"
 template2 = {
-    "sqlEngine": "postgres"
-    "cloudProvider": "AWS"
+    "sqlEngine": "postgres",
+    "cloudProvider": "AWS",
 }
 service.create_template(metadata={}, source=template2, template_id=template_id2)
 
 instruction_id = "client-12345"
 metadata = {
     "createdBy": "mvecchione145",
-
     # templates are compiled from left to right
     # (common keys in example_template1 will be
     # overridden by values in example_template2)
-    "templates": ["example_template1", "example_template2"]
-}
-source = {
-    "system": "darwin"
+    "templates": ["example_template1", "example_template2"],
 }
+source = {"system": "darwin"}
 
 service.create_instruction(
-    instruction_id=instruction_id,
-    metadata=metadata,
-    source=source)
+    instruction_id=instruction_id, metadata=metadata, source=source
+)
 
 instruction = service.get_instruction(instruction_id=instruction_id)
 
-print(returned_payload)
+print(instruction)
 # {
 #   "instruction": {
 #     "cloudProvider": "AWS",
 #     "sqlEngine": "postgres",
 #     "system": "darwin"
 #   },
 #   "metadata": {
+#     "compiled": True,
 #     "createdBy": "mvecchione145",
+#     "createdAt": "YYYY-MM-DD HH:MM:SS.NNNNNN"
 #     "templates": [
 #       "example_template",
 #       "example_template2"
 #     ]
 #   }
 ```
```

