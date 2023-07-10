# Comparing `tmp/bump_pydantic-0.1.0.tar.gz` & `tmp/bump_pydantic-0.2.0.tar.gz`

## Comparing `bump_pydantic-0.1.0.tar` & `bump_pydantic-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,44 @@
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/__main__.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/py.typed
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/add_default_none.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/class_def_visitor.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/field.py
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/replace_config.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/replace_generic_model.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/replace_imports.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/root_model.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/codemods/validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/markers/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/bump_pydantic/markers/find_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/integration/__init__.py
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_add_default_none.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_class_def_visitor.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_field.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_generic_model.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_replace_config.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_replace_imports.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_root_model.py
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/tests/unit/test_validator.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/README.md
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 bump_pydantic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/__main__.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/py.typed
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/__init__.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/add_default_none.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/field.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/mypy_visitor.py
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/replace_config.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/replace_generic_model.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/replace_imports.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/root_model.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/bump_pydantic/codemods/validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/case.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/file.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/folder.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/__init__.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/add_none.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/base_settings.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/config_to_model.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/folder_inside_folder.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/generic_model.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/is_base_model.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/replace_validator.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/integration/cases/root_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_add_default_none.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_class_def_visitor.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_field.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_generic_model.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_replace_config.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_replace_imports.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_root_model.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/tests/unit/test_validator.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/README.md
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 bump_pydantic-0.2.0/PKG-INFO
```

### Comparing `bump_pydantic-0.1.0/.github/workflows/main.yml` & `bump_pydantic-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/.github/workflows/ci.yml` & `bump_pydantic-0.2.0/bump_pydantic/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/__init__.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/__init__.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/add_default_none.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/add_default_none.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import CodemodContext, VisitorBasedCodemodCommand
 from libcst.metadata import FullyQualifiedNameProvider, QualifiedName
 
-from bump_pydantic.codemods.class_def_visitor import ClassDefVisitor
-from bump_pydantic.markers.find_base_model import CONTEXT_KEY as BASE_MODEL_CONTEXT_KEY
-from bump_pydantic.markers.find_base_model import find_base_model
+from bump_pydantic.codemods.mypy_visitor import CONTEXT_KEY
 
 
 class AddDefaultNoneCommand(VisitorBasedCodemodCommand):
     """This codemod adds the default value `None` to all fields of a pydantic model that
     are either type `Optional[T]`, `Union[T, None]` or `Any`.
 
     Example::
@@ -47,15 +45,15 @@
     def visit_ClassDef(self, node: cst.ClassDef) -> None:
         fqn_set = self.get_metadata(FullyQualifiedNameProvider, node)
 
         if not fqn_set:
             return None
 
         fqn: QualifiedName = next(iter(fqn_set))  # type: ignore
-        if fqn.name in self.context.scratch[BASE_MODEL_CONTEXT_KEY]:
+        if self.context.scratch[CONTEXT_KEY].get(fqn.name, False):
             self.inside_base_model = True
 
     def leave_ClassDef(self, original_node: cst.ClassDef, updated_node: cst.ClassDef) -> cst.ClassDef:
         self.inside_base_model = False
         return updated_node
 
     def visit_AnnAssign(self, node: cst.AnnAssign) -> bool | None:
@@ -90,15 +88,14 @@
 if __name__ == "__main__":
     import os
     import textwrap
     from pathlib import Path
     from tempfile import TemporaryDirectory
 
     from libcst.metadata import FullRepoManager
-    from rich.pretty import pprint
 
     with TemporaryDirectory(dir=os.getcwd()) as tmpdir:
         package_dir = f"{tmpdir}/package"
         os.mkdir(package_dir)
         module_path = f"{package_dir}/a.py"
         with open(module_path, "w") as f:
             content = textwrap.dedent(
@@ -119,16 +116,13 @@
             )
             f.write(content)
         module = str(Path(module_path).relative_to(tmpdir))
         mrg = FullRepoManager(tmpdir, {module}, providers={FullyQualifiedNameProvider})
         wrapper = mrg.get_metadata_wrapper_for_path(module)
         context = CodemodContext(wrapper=wrapper)
 
-        command = ClassDefVisitor(context=context)
-        mod = wrapper.visit(command)
-
-        find_base_model(scratch=context.scratch)
-        pprint(context.scratch)
+        # classes = run_mypy_visitor(context=context)
+        # mod = wrapper.visit(command)
 
         command = AddDefaultNoneCommand(context=context)  # type: ignore[assignment]
         mod = wrapper.visit(command)
         print(mod.code)
```

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/field.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/field.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,28 @@
                 m.ZeroOrMore(),
             ],
         ),
         m.ZeroOrMore(),
     ]
 )
 
+ANN_ASSIGN_WITH_FIELD = m.AnnAssign(
+    value=m.Call(func=m.Name("Field")),
+) | m.AnnAssign(
+    annotation=m.Annotation(
+        annotation=m.Subscript(
+            slice=[
+                m.ZeroOrMore(),
+                m.SubscriptElement(slice=m.Index(value=m.Call(func=m.Name("Field")))),
+                m.ZeroOrMore(),
+            ]
+        )
+    )
+)
+
 
 class FieldCodemod(VisitorBasedCodemodCommand):
     def __init__(self, context: CodemodContext) -> None:
         super().__init__(context)
 
         self.has_field_import = False
         self.inside_field_assign = False
@@ -56,20 +70,20 @@
         self.has_field_import = True
 
     @m.leave(IMPORT_FIELD)
     def leave_field_import(self, original_node: cst.Module, updated_node: cst.Module) -> cst.Module:
         self.has_field_import = False
         return updated_node
 
-    @m.visit(m.AnnAssign(value=m.Call(func=m.Name("Field"))))
+    @m.visit(ANN_ASSIGN_WITH_FIELD)
     def visit_field_assign(self, node: cst.AnnAssign) -> None:
         self.inside_field_assign = True
         self._const: Union[cst.Arg, None] = None
 
-    @m.leave(m.AnnAssign(value=m.Call(func=m.Name("Field"))))
+    @m.leave(ANN_ASSIGN_WITH_FIELD)
     def leave_field_assign(self, original_node: cst.AnnAssign, updated_node: cst.AnnAssign) -> cst.AnnAssign:
         self.inside_field_assign = False
 
         if self._const is None:
             return updated_node
 
         AddImportsVisitor.add_needed_import(self.context, "typing", "Literal")
@@ -96,15 +110,23 @@
         if not self.has_field_import or not self.inside_field_assign:
             return updated_node
 
         new_args: List[cst.Arg] = []
         for arg in updated_node.args:
             if m.matches(arg, m.Arg(keyword=m.Name())):
                 keyword = RENAMED_KEYWORDS.get(arg.keyword.value, arg.keyword.value)  # type: ignore
-                new_args.append(arg.with_changes(keyword=arg.keyword.with_changes(value=keyword)))  # type: ignore
+                value = arg.value
+                # The `allow_mutation` keyword argument is a special case. It's the negative of `frozen`.
+                if arg.keyword and arg.keyword.value == "allow_mutation":
+                    if m.matches(arg.value, m.Name(value="False")):
+                        value = cst.Name("True")
+                    elif m.matches(arg.value, m.Name(value="True")):
+                        value = cst.Name("False")
+                new_arg = arg.with_changes(keyword=arg.keyword.with_changes(value=keyword), value=value)  # type: ignore
+                new_args.append(new_arg)  # type: ignore
             else:
                 new_args.append(arg)
 
         return updated_node.with_changes(args=new_args)
 
 
 if __name__ == "__main__":
@@ -112,18 +134,20 @@
 
     from rich.console import Console
 
     console = Console()
 
     source = textwrap.dedent(
         """
+        from typing import Annotated
+
         from pydantic import BaseModel, Field
 
         class A(BaseModel):
-            a: List[str] = Field(..., description="My description", min_items=1)
+            a: Annotated[List[str], Field(..., description="My description", min_items=1)]
         """
     )
     console.print(source)
     console.print("=" * 80)
 
     mod = cst.parse_module(source)
     context = CodemodContext(filename="main.py")
```

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/replace_config.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/replace_generic_model.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/replace_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/replace_imports.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/root_model.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/bump_pydantic/codemods/validator.py` & `bump_pydantic-0.2.0/bump_pydantic/codemods/validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/tests/unit/test_add_default_none.py` & `bump_pydantic-0.2.0/tests/unit/test_add_default_none.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,34 +5,32 @@
 import pytest
 from libcst import MetadataWrapper, parse_module
 from libcst.codemod import CodemodContext, CodemodTest
 from libcst.metadata import FullyQualifiedNameProvider
 from libcst.testing.utils import UnitTest
 
 from bump_pydantic.codemods.add_default_none import AddDefaultNoneCommand
-from bump_pydantic.codemods.class_def_visitor import ClassDefVisitor
-from bump_pydantic.markers.find_base_model import find_base_model
+from bump_pydantic.codemods.mypy_visitor import CONTEXT_KEY, run_mypy_visitor
 
 
+@pytest.mark.skip(reason="The file needs to exists for the test to pass.")
 class TestClassDefVisitor(UnitTest):
     def add_default_none(self, file_path: str, code: str) -> cst.Module:
         mod = MetadataWrapper(
             parse_module(CodemodTest.make_fixture_data(code)),
             cache={
                 FullyQualifiedNameProvider: FullyQualifiedNameProvider.gen_cache(Path(""), [file_path], None).get(
                     file_path, ""
                 )
             },
         )
         mod.resolve_many(AddDefaultNoneCommand.METADATA_DEPENDENCIES)
         context = CodemodContext(wrapper=mod)
-        instance = ClassDefVisitor(context=context)
-        mod.visit(instance)
-
-        find_base_model(scratch=context.scratch)
+        classes = run_mypy_visitor(arg_files=[file_path])
+        context.scratch.update({CONTEXT_KEY: classes})
 
         instance = AddDefaultNoneCommand(context=context)  # type: ignore[assignment]
         return mod.visit(instance)
 
     def test_no_annotations(self) -> None:
         source = textwrap.dedent(
             """class Potato:
```

### Comparing `bump_pydantic-0.1.0/tests/unit/test_class_def_visitor.py` & `bump_pydantic-0.2.0/tests/unit/test_class_def_visitor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,75 @@
-from pathlib import Path
+# from pathlib import Path
 
-from libcst import MetadataWrapper, parse_module
-from libcst.codemod import CodemodContext, CodemodTest
-from libcst.metadata import FullyQualifiedNameProvider
-from libcst.testing.utils import UnitTest
-
-from bump_pydantic.codemods.class_def_visitor import ClassDefVisitor
-
-
-class TestClassDefVisitor(UnitTest):
-    def gather_class_def(self, file_path: str, code: str) -> ClassDefVisitor:
-        mod = MetadataWrapper(
-            parse_module(CodemodTest.make_fixture_data(code)),
-            cache={
-                FullyQualifiedNameProvider: FullyQualifiedNameProvider.gen_cache(Path(""), [file_path], None).get(
-                    file_path, ""
-                )
-            },
-        )
-        mod.resolve_many(ClassDefVisitor.METADATA_DEPENDENCIES)
-        instance = ClassDefVisitor(CodemodContext(wrapper=mod))
-        mod.visit(instance)
-        return instance
-
-    def test_no_annotations(self) -> None:
-        visitor = self.gather_class_def(
-            "some/test/module.py",
-            """
-            def foo() -> None:
-                pass
-            """,
-        )
-        results = visitor.context.scratch[ClassDefVisitor.CONTEXT_KEY]
-        self.assertEqual(results, {})
-
-    def test_without_bases(self) -> None:
-        visitor = self.gather_class_def(
-            "some/test/module.py",
-            """
-            class Foo:
-                pass
-            """,
-        )
-        results = visitor.context.scratch[ClassDefVisitor.CONTEXT_KEY]
-        self.assertEqual(results, {})
-
-    def test_with_class_defs(self) -> None:
-        visitor = self.gather_class_def(
-            "some/test/module.py",
-            """
-            from pydantic import BaseModel
-
-            class Foo(BaseModel):
-                pass
-
-            class Bar(Foo):
-                pass
-            """,
-        )
-        results = visitor.context.scratch[ClassDefVisitor.CONTEXT_KEY]
-        self.assertEqual(
-            results,
-            {
-                "some.test.module.Foo": {"pydantic.BaseModel"},
-                "some.test.module.Bar": {"some.test.module.Foo"},
-            },
-        )
-
-    def test_with_pydantic_base_model(self) -> None:
-        visitor = self.gather_class_def(
-            "some/test/module.py",
-            """
-            import pydantic
-
-            class Foo(pydantic.BaseModel):
-                ...
-            """,
-        )
-        results = visitor.context.scratch[ClassDefVisitor.CONTEXT_KEY]
-        self.assertEqual(
-            results,
-            {"some.test.module.Foo": {"pydantic.BaseModel"}},
-        )
+# from libcst import MetadataWrapper, parse_module
+# from libcst.codemod import CodemodContext, CodemodTest
+# from libcst.metadata import FullyQualifiedNameProvider
+# from libcst.testing.utils import UnitTest
+
+
+# class TestClassDefVisitor(UnitTest):
+#     def gather_class_def(self, file_path: str, code: str) -> ClassDefVisitor:
+#         mod = MetadataWrapper(
+#             parse_module(CodemodTest.make_fixture_data(code)),
+#             cache={
+#                 FullyQualifiedNameProvider: FullyQualifiedNameProvider.gen_cache(Path(""), [file_path], None).get(
+#                     file_path, ""
+#                 )
+#             },
+#         )
+#         mod.resolve_many(ClassDefVisitor.METADATA_DEPENDENCIES)
+#         instance = ClassDefVisitor(CodemodContext(wrapper=mod))
+#         mod.visit(instance)
+#         return instance
+
+#     def test_no_annotations(self) -> None:
+#         visitor = self.gather_class_def(
+#             "some/test/module.py",
+#             """
+#             def foo() -> None:
+#                 pass
+#             """,
+#         )
+#         results = visitor.context.scratch[ClassDefVisitor.BASE_MODEL_CONTEXT_KEY]
+#         self.assertEqual(results, {"pydantic.BaseModel", "pydantic.main.BaseModel"})
+
+#     def test_without_bases(self) -> None:
+#         visitor = self.gather_class_def(
+#             "some/test/module.py",
+#             """
+#             class Foo:
+#                 pass
+#             """,
+#         )
+#         results = visitor.context.scratch[ClassDefVisitor.BASE_MODEL_CONTEXT_KEY]
+#         self.assertEqual(results, {"pydantic.BaseModel", "pydantic.main.BaseModel"})
+
+#     def test_with_class_defs(self) -> None:
+#         visitor = self.gather_class_def(
+#             "some/test/module.py",
+#             """
+#             from pydantic import BaseModel
+
+#             class Foo(BaseModel):
+#                 pass
+
+#             class Bar(Foo):
+#                 pass
+#             """,
+#         )
+#         results = visitor.context.scratch[ClassDefVisitor.BASE_MODEL_CONTEXT_KEY]
+#         self.assertEqual(
+#             results, {"pydantic.BaseModel", "pydantic.main.BaseModel", "some.test.module.Foo", "some.test.module.Bar"}
+#         )
+
+#     def test_with_pydantic_base_model(self) -> None:
+#         visitor = self.gather_class_def(
+#             "some/test/module.py",
+#             """
+#             import pydantic
+
+#             class Foo(pydantic.BaseModel):
+#                 ...
+#             """,
+#         )
+#         results = visitor.context.scratch[ClassDefVisitor.BASE_MODEL_CONTEXT_KEY]
+#         self.assertEqual(results, {"pydantic.BaseModel", "pydantic.main.BaseModel", "some.test.module.Foo"})
```

### Comparing `bump_pydantic-0.1.0/tests/unit/test_field.py` & `bump_pydantic-0.2.0/tests/unit/test_field.py`

 * *Files 22% similar despite different names*

```diff
@@ -98,7 +98,41 @@
         class MyEnum(Enum):
             POTATO = "potato"
 
         class Potato(BaseModel):
             potato: Literal[MyEnum.POTATO] = MyEnum.POTATO
         """
         self.assertCodemod(before, after)
+
+    def test_flip_frozen_boolean(self) -> None:
+        before = """
+        from pydantic import BaseSettings, Field
+
+        class Settings(BaseSettings):
+            potato: int = Field(..., allow_mutation=False)
+            strawberry: int = Field(..., allow_mutation=True)
+        """
+        after = """
+        from pydantic import BaseSettings, Field
+
+        class Settings(BaseSettings):
+            potato: int = Field(..., frozen=True)
+            strawberry: int = Field(..., frozen=False)
+        """
+        self.assertCodemod(before, after)
+
+    def test_annotated_field(self) -> None:
+        before = """
+        from pydantic import BaseModel, Field
+        from typing import Annotated
+
+        class Potato(BaseModel):
+            potato: Annotated[List[int], Field(..., min_items=1, max_items=10)]
+        """
+        after = """
+        from pydantic import BaseModel, Field
+        from typing import Annotated
+
+        class Potato(BaseModel):
+            potato: Annotated[List[int], Field(..., min_length=1, max_length=10)]
+        """
+        self.assertCodemod(before, after)
```

### Comparing `bump_pydantic-0.1.0/tests/unit/test_generic_model.py` & `bump_pydantic-0.2.0/tests/unit/test_generic_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/tests/unit/test_replace_config.py` & `bump_pydantic-0.2.0/tests/unit/test_replace_config.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/tests/unit/test_replace_imports.py` & `bump_pydantic-0.2.0/tests/unit/test_replace_imports.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/tests/unit/test_root_model.py` & `bump_pydantic-0.2.0/tests/unit/test_root_model.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/tests/unit/test_validator.py` & `bump_pydantic-0.2.0/tests/unit/test_validator.py`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/.gitignore` & `bump_pydantic-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/LICENSE.txt` & `bump_pydantic-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bump_pydantic-0.1.0/README.md` & `bump_pydantic-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: bump-pydantic
+Version: 0.2.0
+Summary: Convert Pydantic from V1 to V2 ♻
+Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
+Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
+Project-URL: Source, https://github.com/pydantic/bump-pydantic
+Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
+License-Expression: MIT
+License-File: LICENSE.txt
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pydantic
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Requires-Dist: libcst
+Requires-Dist: mypy
+Requires-Dist: rich
+Requires-Dist: typer>=0.7.0
+Requires-Dist: typing-extensions
+Description-Content-Type: text/markdown
+
 # Bump Pydantic ♻️
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - License](https://img.shields.io/pypi/l/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 
 
@@ -20,29 +47,28 @@
     - [Check diff before applying changes](#check-diff-before-applying-changes)
     - [Apply changes](#apply-changes)
   - [Rules](#rules)
     - [BP001: Add default `None` to `Optional[T]`, `Union[T, None]` and `Any` fields](#bp001-add-default-none-to-optionalt-uniont-none-and-any-fields)
     - [BP002: Replace `Config` class by `model_config` attribute](#bp002-replace-config-class-by-model_config-attribute)
     - [BP003: Replace `Field` old parameters to new ones](#bp003-replace-field-old-parameters-to-new-ones)
     - [BP004: Replace imports](#bp004-replace-imports)
-    - [BP003: Replace `Config` class by `model_config`](#bp003-replace-config-class-by-model_config)
     - [BP005: Replace `GenericModel` by `BaseModel`](#bp005-replace-genericmodel-by-basemodel)
     - [BP006: Replace `__root__` by `RootModel`](#bp006-replace-__root__-by-rootmodel)
     - [BP007: Replace decorators](#bp007-replace-decorators)
-    - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter)
+    <!-- - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter) -->
   - [License](#license)
 
 ---
 
 ## Installation
 
 The installation is as simple as:
 
 ```bash
-pip install "bump-pydantic @ git+https://github.com/pydantic/bump-pydantic@main"
+pip install bump-pydantic
 ```
 
 ---
 
 ## Usage
 
 `bump-pydantic` is a CLI tool, hence you can use it from your terminal.
@@ -155,37 +181,14 @@
 ```
 
 ### BP004: Replace imports
 
 - ✅ Replace `BaseSettings` from `pydantic` to `pydantic_settings`.
 - ✅ Replace `Color` and `PaymentCardNumber` from `pydantic` to `pydantic_extra_types`.
 
-### BP003: Replace `Config` class by `model_config`
-
-- ✅ Replace `Config` class by `model_config = ConfigDict()`.
-
-The following code will be transformed:
-
-```py
-class User(BaseModel):
-    name: str
-
-    class Config:
-        extra = 'forbid'
-```
-
-Into:
-
-```py
-class User(BaseModel):
-    name: str
-
-    model_config = ConfigDict(extra='forbid')
-```
-
 ### BP005: Replace `GenericModel` by `BaseModel`
 
 - ✅ Replace `GenericModel` by `BaseModel`.
 
 The following code will be transformed:
 
 ```py
@@ -280,14 +283,15 @@
         return v
 
     @model_validator(mode='before')
     def validate_root(cls, values):
         return values
 ```
 
+<!--
 ### BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
 
 - ✅ Replace `pydantic.parse_obj_as(T, obj)` to `pydantic.TypeAdapter(T).validate_python(obj)`.
 
 
 The following code will be transformed:
 
@@ -322,13 +326,14 @@
 
 class Users(BaseModel):
     users: List[User]
 
 
 users = TypeAdapter(Users).validate_python({'users': [{'name': 'John'}]})
 ```
+-->
 
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `bump_pydantic-0.1.0/pyproject.toml` & `bump_pydantic-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Framework :: Pydantic",
 ]
-dependencies = ["typer>=0.7.0", "libcst", "rich", "typing_extensions"]
+dependencies = ["typer>=0.7.0", "libcst", "rich", "typing_extensions", "mypy"]
 
 [project.urls]
 Documentation = "https://github.com/pydantic/bump-pydantic#readme"
 Issues = "https://github.com/pydantic/bump-pydantic/issues"
 Source = "https://github.com/pydantic/bump-pydantic"
 
 [project.scripts]
```

### Comparing `bump_pydantic-0.1.0/PKG-INFO` & `bump_pydantic-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: bump-pydantic
-Version: 0.1.0
-Summary: Convert Pydantic from V1 to V2 ♻
-Project-URL: Documentation, https://github.com/pydantic/bump-pydantic#readme
-Project-URL: Issues, https://github.com/pydantic/bump-pydantic/issues
-Project-URL: Source, https://github.com/pydantic/bump-pydantic
-Author-email: Marcelo Trylesinski <marcelotryle@gmail.com>
-License-Expression: MIT
-License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Pydantic
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Requires-Dist: libcst
-Requires-Dist: rich
-Requires-Dist: typer>=0.7.0
-Requires-Dist: typing-extensions
-Description-Content-Type: text/markdown
-
 # Bump Pydantic ♻️
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 [![PyPI - License](https://img.shields.io/pypi/l/bump-pydantic.svg)](https://pypi.org/project/bump-pydantic)
 
 
@@ -46,29 +20,28 @@
     - [Check diff before applying changes](#check-diff-before-applying-changes)
     - [Apply changes](#apply-changes)
   - [Rules](#rules)
     - [BP001: Add default `None` to `Optional[T]`, `Union[T, None]` and `Any` fields](#bp001-add-default-none-to-optionalt-uniont-none-and-any-fields)
     - [BP002: Replace `Config` class by `model_config` attribute](#bp002-replace-config-class-by-model_config-attribute)
     - [BP003: Replace `Field` old parameters to new ones](#bp003-replace-field-old-parameters-to-new-ones)
     - [BP004: Replace imports](#bp004-replace-imports)
-    - [BP003: Replace `Config` class by `model_config`](#bp003-replace-config-class-by-model_config)
     - [BP005: Replace `GenericModel` by `BaseModel`](#bp005-replace-genericmodel-by-basemodel)
     - [BP006: Replace `__root__` by `RootModel`](#bp006-replace-__root__-by-rootmodel)
     - [BP007: Replace decorators](#bp007-replace-decorators)
-    - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter)
+    <!-- - [BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`](#bp008-replace-pydanticparse_obj_as-by-pydantictypeadapter) -->
   - [License](#license)
 
 ---
 
 ## Installation
 
 The installation is as simple as:
 
 ```bash
-pip install "bump-pydantic @ git+https://github.com/pydantic/bump-pydantic@main"
+pip install bump-pydantic
 ```
 
 ---
 
 ## Usage
 
 `bump-pydantic` is a CLI tool, hence you can use it from your terminal.
@@ -181,37 +154,14 @@
 ```
 
 ### BP004: Replace imports
 
 - ✅ Replace `BaseSettings` from `pydantic` to `pydantic_settings`.
 - ✅ Replace `Color` and `PaymentCardNumber` from `pydantic` to `pydantic_extra_types`.
 
-### BP003: Replace `Config` class by `model_config`
-
-- ✅ Replace `Config` class by `model_config = ConfigDict()`.
-
-The following code will be transformed:
-
-```py
-class User(BaseModel):
-    name: str
-
-    class Config:
-        extra = 'forbid'
-```
-
-Into:
-
-```py
-class User(BaseModel):
-    name: str
-
-    model_config = ConfigDict(extra='forbid')
-```
-
 ### BP005: Replace `GenericModel` by `BaseModel`
 
 - ✅ Replace `GenericModel` by `BaseModel`.
 
 The following code will be transformed:
 
 ```py
@@ -306,14 +256,15 @@
         return v
 
     @model_validator(mode='before')
     def validate_root(cls, values):
         return values
 ```
 
+<!--
 ### BP008: Replace `pydantic.parse_obj_as` by `pydantic.TypeAdapter`
 
 - ✅ Replace `pydantic.parse_obj_as(T, obj)` to `pydantic.TypeAdapter(T).validate_python(obj)`.
 
 
 The following code will be transformed:
 
@@ -348,13 +299,14 @@
 
 class Users(BaseModel):
     users: List[User]
 
 
 users = TypeAdapter(Users).validate_python({'users': [{'name': 'John'}]})
 ```
+-->
 
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

