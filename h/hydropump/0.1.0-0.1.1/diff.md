# Comparing `tmp/hydropump-0.1.0.tar.gz` & `tmp/hydropump-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydropump-0.1.0.tar", max compression
+gzip compressed data, was "hydropump-0.1.1.tar", max compression
```

## Comparing `hydropump-0.1.0.tar` & `hydropump-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-07-08 15:17:11.235752 hydropump-0.1.0/LICENSE
--rw-r--r--   0        0        0     3546 2023-07-09 18:35:40.847509 hydropump-0.1.0/README.md
--rw-r--r--   0        0        0      214 2023-07-09 00:52:35.220448 hydropump-0.1.0/hydropump/__init__.py
--rw-r--r--   0        0        0    11173 2023-07-10 00:53:01.631306 hydropump-0.1.0/hydropump/backend.py
--rw-r--r--   0        0        0     4742 2023-07-10 00:56:48.719844 hydropump-0.1.0/hydropump/instruction.py
--rw-r--r--   0        0        0     6284 2023-07-10 00:58:51.044297 hydropump-0.1.0/hydropump/service.py
--rw-r--r--   0        0        0     3292 2023-07-09 18:37:38.782053 hydropump-0.1.0/hydropump/test/TESTING.md
--rw-r--r--   0        0        0        0 2023-07-09 00:43:11.686090 hydropump-0.1.0/hydropump/test/__init__.py
--rw-r--r--   0        0        0     1398 2023-07-10 00:59:22.389807 hydropump-0.1.0/hydropump/test/conftest.py
--rw-r--r--   0        0        0        0 2023-07-09 00:44:25.748468 hydropump-0.1.0/hydropump/test/unit/__init__.py
--rw-r--r--   0        0        0     1468 2023-07-10 00:39:52.153530 hydropump-0.1.0/hydropump/test/unit/test_instructions.py
--rw-r--r--   0        0        0       13 2023-07-09 21:40:44.625173 hydropump-0.1.0/hydropump/test/unit/test_root/base/.gitignore
--rw-r--r--   0        0        0       13 2023-07-09 21:40:47.513645 hydropump-0.1.0/hydropump/test/unit/test_root/template/.gitignore
--rw-r--r--   0        0        0      745 2023-07-09 23:58:47.428825 hydropump-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 hydropump-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-10 01:52:29.959752 hydropump-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2573 2023-07-10 01:52:29.959752 hydropump-0.1.1/README.md
+-rw-r--r--   0        0        0      214 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/__init__.py
+-rw-r--r--   0        0        0    11223 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/backend.py
+-rw-r--r--   0        0        0     4742 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/instruction.py
+-rw-r--r--   0        0        0     6260 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/service.py
+-rw-r--r--   0        0        0     3292 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/TESTING.md
+-rw-r--r--   0        0        0        0 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/__init__.py
+-rw-r--r--   0        0        0     1398 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/test_instructions.py
+-rw-r--r--   0        0        0       13 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/test_root/base/.gitignore
+-rw-r--r--   0        0        0       13 2023-07-10 01:52:29.959752 hydropump-0.1.1/hydropump/test/unit/test_root/template/.gitignore
+-rw-r--r--   0        0        0      740 2023-07-10 01:52:29.959752 hydropump-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 hydropump-0.1.1/PKG-INFO
```

### Comparing `hydropump-0.1.0/LICENSE` & `hydropump-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.0/hydropump/backend.py` & `hydropump-0.1.1/hydropump/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,32 +56,32 @@
             output = child
         for k, v in parent.items():
             if isinstance(v, (str, int, float, bool)):
                 output[k] = v
             elif isinstance(v, list):
                 output[k] = output.get(k, []) + v
             elif isinstance(v, dict):
-                output[k] = self._compile(v, child.get(k, {}), output.get())
+                output[k] = self._compile(v, child.get(k, {}), output.get(k, {}))
         return output
 
     def compile_instruction(self, instruction: Instruction) -> Instruction:
         """
         Compile the instruction by applying templates.
 
         Args:
             instruction (Instruction): The instruction object.
 
         Returns:
             Instruction: The compiled instruction.
         """
+        template = {}
         for template_id in instruction.metadata.get("templates", []):
             template_instruction = self.get_template(template_id)
-            instruction.source = self._compile(
-                instruction.source, template_instruction["template"]
-            )
+            template = self._compile(template_instruction["template"], template)
+        instruction.source = self._compile(instruction.source, template)
         instruction.set_source()
         return instruction
 
     def set_dump_load(self):
         """
         Set the dump and load functions based on the file extension.
         """
```

### Comparing `hydropump-0.1.0/hydropump/instruction.py` & `hydropump-0.1.1/hydropump/instruction.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.0/hydropump/service.py` & `hydropump-0.1.1/hydropump/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         Returns:
             Instruction: The retrieved instruction.
 
         Raises:
             NotImplementedError: If debug mode is not enabled and compilation is requested.
         """
         instruction = self.backend.get_base(instruction_id=instruction_id)
-        if not self.debug and compile:
-            raise NotImplementedError("Compilation is not supported in non-debug mode.")
+        if compile:
+            instruction = self.backend.compile_instruction(instruction=instruction)
         return instruction
 
     def get_template(self, template_id: str) -> Template:
         """
         Get a template by its ID.
 
         Args:
```

### Comparing `hydropump-0.1.0/hydropump/test/TESTING.md` & `hydropump-0.1.1/hydropump/test/TESTING.md`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.0/hydropump/test/conftest.py` & `hydropump-0.1.1/hydropump/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.0/hydropump/test/unit/test_instructions.py` & `hydropump-0.1.1/hydropump/test/unit/test_instructions.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     expected_compiled_result: dict,
 ) -> None:
     test_service.create_instruction(
         instruction_id=test_instruction_id,
         metadata=test_metadata,
         source=test_source,
     )
-    instruction = test_service.get_instruction(test_instruction_id)
+    instruction = test_service.get_instruction(instruction_id=test_instruction_id)
     assert instruction == expected_compiled_result
 
 
 @pytest.mark.run(order=3)
 def test_delete_instruction(
     test_service: Service,
     test_instruction_id: str,
```

### Comparing `hydropump-0.1.0/pyproject.toml` & `hydropump-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydropump"
-version = "0.1.0"
+version = "0.1.1"
 description = "Configuration Management Library"
 authors = ["Michael Vecchione <51305946+mvecchione145@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
@@ -22,16 +22,16 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [project.urls]
-"Homepage" = "https://github.com/mvecchione145/HydroPump-python"
-"Bug Tracker" = "https://github.com/mvecchione145/HydroPump-python/issues"
+homepage = "https://github.com/mvecchione145/HydroPump-python"
+bugtracker = "https://github.com/mvecchione145/HydroPump-python/issues"
 
 
 [tool.pytest]
 testpaths = [
     "hydropump/test"
 ]
```

