# Comparing `tmp/BREWasm-0.0.tar.gz` & `tmp/BREWasm-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BREWasm-0.0.tar", last modified: Mon Jul 10 03:47:52 2023, max compression
+gzip compressed data, was "BREWasm-0.2.tar", last modified: Sat Jul  8 15:00:21 2023, max compression
```

## Comparing `BREWasm-0.0.tar` & `BREWasm-0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ping       (501) staff       (20)        0 2023-07-10 03:47:52.530197 BREWasm-0.0/
-drwxr-xr-x   0 ping       (501) staff       (20)        0 2023-07-10 03:47:52.525967 BREWasm-0.0/BREWasm/
--rw-r--r--   0 ping       (501) staff       (20)      228 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/__init__.py
-drwxr-xr-x   0 ping       (501) staff       (20)        0 2023-07-10 03:47:52.528125 BREWasm-0.0/BREWasm/parser/
--rw-r--r--   0 ping       (501) staff       (20)       12 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/__init__.py
--rw-r--r--   0 ping       (501) staff       (20)      562 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/errors.py
--rw-r--r--   0 ping       (501) staff       (20)      892 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/instruction.py
--rw-r--r--   0 ping       (501) staff       (20)     1996 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/leb128.py
--rw-r--r--   0 ping       (501) staff       (20)     5355 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/module.py
--rw-r--r--   0 ping       (501) staff       (20)     2845 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/opcodes.py
--rw-r--r--   0 ping       (501) staff       (20)     5778 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/opnames.py
--rw-r--r--   0 ping       (501) staff       (20)    24366 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/reader.py
--rw-r--r--   0 ping       (501) staff       (20)     3108 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/parser/types.py
-drwxr-xr-x   0 ping       (501) staff       (20)        0 2023-07-10 03:47:52.529677 BREWasm-0.0/BREWasm/rewriter/
--rw-r--r--   0 ping       (501) staff       (20)      160 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/BREWasm.py
--rw-r--r--   0 ping       (501) staff       (20)      226 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/__init__.py
--rw-r--r--   0 ping       (501) staff       (20)     4777 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/defination.py
--rw-r--r--   0 ping       (501) staff       (20)     4957 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/indices_fixer.py
--rw-r--r--   0 ping       (501) staff       (20)    51052 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/modify_binary.py
--rw-r--r--   0 ping       (501) staff       (20)    57672 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/section_rewriter.py
--rw-r--r--   0 ping       (501) staff       (20)    19510 2023-07-10 03:41:49.000000 BREWasm-0.0/BREWasm/rewriter/semantics_rewriter.py
-drwxr-xr-x   0 ping       (501) staff       (20)        0 2023-07-10 03:47:52.526581 BREWasm-0.0/BREWasm.egg-info/
--rw-r--r--   0 ping       (501) staff       (20)     3440 2023-07-10 03:47:52.000000 BREWasm-0.0/BREWasm.egg-info/PKG-INFO
--rw-r--r--   0 ping       (501) staff       (20)      646 2023-07-10 03:47:52.000000 BREWasm-0.0/BREWasm.egg-info/SOURCES.txt
--rw-r--r--   0 ping       (501) staff       (20)        1 2023-07-10 03:47:52.000000 BREWasm-0.0/BREWasm.egg-info/dependency_links.txt
--rw-r--r--   0 ping       (501) staff       (20)        8 2023-07-10 03:47:52.000000 BREWasm-0.0/BREWasm.egg-info/top_level.txt
--rw-r--r--   0 ping       (501) staff       (20)     3440 2023-07-10 03:47:52.530086 BREWasm-0.0/PKG-INFO
--rw-r--r--   0 ping       (501) staff       (20)     6404 2023-07-10 03:46:22.000000 BREWasm-0.0/README.md
-drwxr-xr-x   0 ping       (501) staff       (20)        0 2023-07-10 03:47:52.529873 BREWasm-0.0/doc/
--rw-r--r--   0 ping       (501) staff       (20)   123854 2023-07-10 03:42:21.000000 BREWasm-0.0/doc/Definition.png
--rw-r--r--   0 ping       (501) staff       (20)       38 2023-07-10 03:47:52.530240 BREWasm-0.0/setup.cfg
--rw-r--r--   0 ping       (501) staff       (20)      649 2023-07-10 03:45:38.000000 BREWasm-0.0/setup.py
+drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 15:00:21.137958 BREWasm-0.2/
+drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 15:00:21.129957 BREWasm-0.2/BREWasm/
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      144 2023-07-08 14:13:39.000000 BREWasm-0.2/BREWasm/__init__.py
+drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 15:00:21.133957 BREWasm-0.2/BREWasm/parser/
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 14:14:35.000000 BREWasm-0.2/BREWasm/parser/__init__.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      581 2023-07-08 13:57:21.000000 BREWasm-0.2/BREWasm/parser/errors.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     1515 2023-07-08 13:57:21.000000 BREWasm-0.2/BREWasm/parser/instruction.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     2189 2023-07-08 13:57:21.000000 BREWasm-0.2/BREWasm/parser/leb128.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     5367 2023-07-08 13:57:21.000000 BREWasm-0.2/BREWasm/parser/module.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     2845 2023-07-08 13:22:42.000000 BREWasm-0.2/BREWasm/parser/opcodes.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     5778 2023-07-08 13:26:01.000000 BREWasm-0.2/BREWasm/parser/opnames.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)    24422 2023-07-08 13:57:21.000000 BREWasm-0.2/BREWasm/parser/reader.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     3266 2023-07-08 13:57:21.000000 BREWasm-0.2/BREWasm/parser/types.py
+drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 15:00:21.137958 BREWasm-0.2/BREWasm/rewriter/
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)      160 2023-07-08 14:12:36.000000 BREWasm-0.2/BREWasm/rewriter/BREWasm.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)        0 2023-06-30 09:02:47.000000 BREWasm-0.2/BREWasm/rewriter/__init__.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)    51172 2023-07-08 14:00:26.000000 BREWasm-0.2/BREWasm/rewriter/change_binary.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     4787 2023-07-08 14:00:26.000000 BREWasm-0.2/BREWasm/rewriter/defination.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     4957 2023-07-08 14:01:07.000000 BREWasm-0.2/BREWasm/rewriter/indices_fixer.py
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)    59198 2023-07-08 14:14:18.000000 BREWasm-0.2/BREWasm/rewriter/section_rewriter.py
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)    19510 2023-07-08 14:02:41.000000 BREWasm-0.2/BREWasm/rewriter/semantics_rewriter.py
+drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 15:00:21.129957 BREWasm-0.2/BREWasm.egg-info/
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)     3612 2023-07-08 15:00:21.000000 BREWasm-0.2/BREWasm.egg-info/PKG-INFO
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)      646 2023-07-08 15:00:21.000000 BREWasm-0.2/BREWasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)        1 2023-07-08 15:00:21.000000 BREWasm-0.2/BREWasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)        8 2023-07-08 15:00:21.000000 BREWasm-0.2/BREWasm.egg-info/top_level.txt
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)     3612 2023-07-08 15:00:21.137958 BREWasm-0.2/PKG-INFO
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)     6750 2023-07-08 14:23:27.000000 BREWasm-0.2/README.md
+drwxrwxr-x   0 obfuscator  (1000) obfuscator  (1000)        0 2023-07-08 15:00:21.137958 BREWasm-0.2/doc/
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)   123854 2023-07-08 02:18:35.000000 BREWasm-0.2/doc/Definition.png
+-rw-rw-r--   0 obfuscator  (1000) obfuscator  (1000)       38 2023-07-08 15:00:21.137958 BREWasm-0.2/setup.cfg
+-rw-r--r--   0 obfuscator  (1000) obfuscator  (1000)      649 2023-07-08 15:00:04.000000 BREWasm-0.2/setup.py
```

### Comparing `BREWasm-0.0/BREWasm/parser/leb128.py` & `BREWasm-0.2/BREWasm/parser/leb128.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,63 +2,63 @@
 
 
 def decode_var_uint(reader, size: int):
     result = 0
     i = 0
     while True:
         a = reader.read(1)
-        b = int.from_bytes(a, "little")
+        b = int.from_bytes(a, "little")  # bytes转int，否则没法&
 
         if i == size / 7:
             if b & 0x80 != 0:
                 raise ErrIntTooLong
             if b >> (size - i * 7) > 0:
                 raise ErrIntTooLarge
-        result |= (b & 0x7f) << (i * 7)
+        result |= (b & 0x7f) << (i * 7)  # 取低7位并左移七位
         if b & 0x80 == 0:
             return result, i + 1
         i += 1
     raise ErrUnexpectedEnd
 
 
 def decode_var_uint111(data, size: int):
     result = 0
     i = 0
     while True:
-        b = int.from_bytes(data[:1], "little")
+        b = int.from_bytes(data[:1], "little")  # bytes转int，否则没法&
         data = data[1:]
 
         if i == size / 7:
             if b & 0x80 != 0:
                 raise ErrIntTooLong
             if b >> (size - i * 7) > 0:
                 raise ErrIntTooLarge
-        result |= (b & 0x7f) << (i * 7)
+        result |= (b & 0x7f) << (i * 7)  # 取低7位并左移七位
         if b & 0x80 == 0:
             return result, i + 1
         i += 1
     raise ErrUnexpectedEnd
 
 
 def decode_var_int(reader, size):
     result = 0
     i = 0
     while True:
-        b = int.from_bytes(reader.read(1), "little")
+        b = int.from_bytes(reader.read(1), "little")  # bytes转int，否则没法&
 
         if i == size / 7:
             if b & 0x80 != 0:
                 raise ErrIntTooLong
             if b & 0x40 == 0 and b >> (size - i * 7 - 1) != 0 or \
                     b & 0x40 != 0 and int(b | 0x80) >> (size - i * 7 - 1) != -1:
                 raise ErrIntTooLarge
         result |= (b & 0x7f) << (i * 7)
         if b & 0x80 == 0:
-            if (i * 7 < size) and (b & 0x40 != 0):
-                result |= -1 << ((i + 1) * 7)
+            if (i * 7 < size) and (b & 0x40 != 0):  # 判断是否为负数
+                result |= -1 << ((i + 1) * 7)  # 前几位补1
             return result, i + 1
         i += 1
     raise ErrUnexpectedEnd
 
 
 def decode_var_uint_from_data(data, size: int):
     result = 0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `BREWasm-0.0/BREWasm/parser/module.py` & `BREWasm-0.2/BREWasm/parser/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..parser.types import BlockTypeI32, BlockTypeI64, BlockTypeF32, BlockTypeF64, BlockTypeEmpty, FuncType, \
-    I32, I64, F32, F64
+    ValTypeI32, ValTypeI64, ValTypeF32, ValTypeF64
 
 MagicNumber = 0x6D736100
 
 Version = 0x00000001
 
 SecCustomID = 0
 
@@ -51,17 +51,15 @@
 LocalIdx = int
 
 LabelIdx = int
 
 
 class Module:
 
-    def __init__(self, path=None):
-
-        self.path = path
+    def __init__(self):
 
         self.magic = 0
 
         self.version = 0
 
         self.custom_secs = []
 
@@ -91,21 +89,21 @@
         self.section_range.append([])
         for i in range(11):
             self.section_range.append(SectionRange())
 
     def get_block_type(self, bt):
 
         if bt == BlockTypeI32:
-            return FuncType(result_types=[I32])
+            return FuncType(result_types=[ValTypeI32])
         elif bt == BlockTypeI64:
             return FuncType(result_types=[ValTypeI64])
         elif bt == BlockTypeF32:
-            return FuncType(result_types=[F32])
+            return FuncType(result_types=[ValTypeF32])
         elif bt == BlockTypeF64:
-            return FuncType(result_types=[F64])
+            return FuncType(result_types=[ValTypeF64])
         elif bt == BlockTypeEmpty:
             return FuncType()
         else:
             return self.type_sec[bt]
 
 
 class SectionRange:
```

### Comparing `BREWasm-0.0/BREWasm/parser/opcodes.py` & `BREWasm-0.2/BREWasm/parser/opcodes.py`

 * *Files identical despite different names*

### Comparing `BREWasm-0.0/BREWasm/parser/opnames.py` & `BREWasm-0.2/BREWasm/parser/opnames.py`

 * *Files identical despite different names*

### Comparing `BREWasm-0.0/BREWasm/parser/reader.py` & `BREWasm-0.2/BREWasm/parser/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..parser.leb128 import *
 from ..parser.module import Import, ImportDesc, ImportTagFunc, ImportTagTable, ImportTagMem, ImportTagGlobal, \
     Global, Export, ExportDesc, ExportTagFunc, ExportTagTable, ExportTagMem, ExportTagGlobal, Elem, Code, Locals, \
     Data, MagicNumber, Version, Module, SecCustomID, SecDataID, CustomSec, SecTypeID, SecImportID, SecFuncID, \
     SecTableID, SecMemID, SecGlobalID, SecExportID, SecStartID, SecElemID, SecCodeID, NameData, SectionRange
 from ..parser.opcodes import *
 from ..parser.opnames import opnames
-from ..parser.types import I32, I64, F32, F64, FuncType, FtTag, TableType, FuncRef, \
+from ..parser.types import ValTypeI32, ValTypeI64, ValTypeF32, ValTypeF64, FuncType, FtTag, TableType, FuncRef, \
     GlobalType, MutConst, MutVar, Limits, BlockTypeI32, BlockTypeI64, BlockTypeF32, BlockTypeF64, BlockTypeEmpty, \
     NameAssoc
 
 
 def decode_file(file_name: str):
     data, err = None, None
     try:
@@ -536,15 +536,15 @@
         vec = []
         for _ in range(self.read_var_u32()):
             vec.append(self.read_val_type())
         return vec
 
     def read_val_type(self):
         vt = self.read_byte()
-        if vt not in [I32, I64, F32, F64]:
+        if vt not in [ValTypeI32, ValTypeI64, ValTypeF32, ValTypeF64]:
             raise Exception("malformed value type: %d" % vt)
         return vt
 
     def read_block_type(self):
         bt = self.read_var_s32()
         if bt < 0:
             if bt not in [BlockTypeI32, BlockTypeI64, BlockTypeF32, BlockTypeF64, BlockTypeEmpty]:
```

### Comparing `BREWasm-0.0/BREWasm/parser/types.py` & `BREWasm-0.2/BREWasm/parser/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-I32 = 0x7F
+ValTypeI32 = 0x7F
 
-I64 = 0x7E
+ValTypeI64 = 0x7E
 
-F32 = 0x7D
+ValTypeF32 = 0x7D
 
-F64 = 0x7C
+ValTypeF64 = 0x7C
 
 BlockTypeI32 = -1
 BlockTypeI64 = -2
 BlockTypeF32 = -3
 BlockTypeF64 = -4
 BlockTypeEmpty = -64
 
 FtTag = 0x60
 FuncRef = 0x70
 
 MutConst = 0
 MutVar = 1
 
+FunctionName = 0
+GlobalName = 1
+DataName = 2
+
 
 class FuncType:
 
     def __init__(self, tag=0, param_types=None, result_types=None):
         if result_types is None:
             result_types = []
         if param_types is None:
@@ -52,30 +56,30 @@
         sb += ")"
         return sb
 
     def get_signature(self):
         arg_types = []
         ret_types = []
         for valtype in self.param_types:
-            if valtype == I32:
+            if valtype == ValTypeI32:
                 arg_types.append("i32")
-            elif valtype == I64:
+            elif valtype == ValTypeI64:
                 arg_types.append("i64")
-            elif valtype == F32:
+            elif valtype == ValTypeF32:
                 arg_types.append("f32")
-            elif valtype == F64:
+            elif valtype == ValTypeF64:
                 arg_types.append("f64")
         for valtype in self.result_types:
-            if valtype == I32:
+            if valtype == ValTypeI32:
                 ret_types.append("i32")
-            elif valtype == I64:
+            elif valtype == ValTypeI64:
                 ret_types.append("i64")
-            elif valtype == F32:
+            elif valtype == ValTypeF32:
                 ret_types.append("f32")
-            elif valtype == F64:
+            elif valtype == ValTypeF64:
                 ret_types.append("f64")
         return arg_types, ret_types
 
     def __str__(self):
         return self.print_signature()
 
 
@@ -120,17 +124,17 @@
         self.name = name
 
     def __str__(self):
         return "{id: %d, name: %s}" % (self.idx, self.name)
 
 
 def val_type_to_str(vt) -> str:
-    if vt == I32:
+    if vt == ValTypeI32:
         return "i32"
-    elif vt == I64:
+    elif vt == ValTypeI64:
         return "i64"
-    elif vt == F32:
+    elif vt == ValTypeF32:
         return "f32"
-    elif vt == F64:
+    elif vt == ValTypeF64:
         return "f64"
     else:
         raise Exception("invalid valtype: %d" % vt)
```

### Comparing `BREWasm-0.0/BREWasm/rewriter/defination.py` & `BREWasm-0.2/BREWasm/rewriter/defination.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 from ..parser.module import ExportDesc
 from ..parser.module import Global as OriginGlobal
 from ..parser.module import Import as OriginImport
 from ..parser.module import ImportDesc
 from ..parser.module import Locals
 from ..parser.types import *
 
-FunctionName = 0
-GlobalName = 1
-DataName = 2
-
 
 class SectionName(Enum):
     CustomSec = 0
     TypeSec = 1
     ImportSec = 2
     FuncSec = 3
     TableSec = 4
@@ -51,33 +47,33 @@
     def convert(self):
         param_types = []
         result_types = []
         if self.arg_types is not None:
             for arg in self.arg_types:
                 match arg:
                     case "i32":
-                        param_types.append(I32)
+                        param_types.append(ValTypeI32)
                     case "i64":
-                        param_types.append(I64)
+                        param_types.append(ValTypeI64)
                     case "f32":
-                        param_types.append(F32)
+                        param_types.append(ValTypeF32)
                     case "f64":
-                        param_types.append(F64)
+                        param_types.append(ValTypeF64)
 
         if self.ret_types is not None:
             for arg in self.ret_types:
                 match arg:
                     case "i32":
-                        result_types.append(I32)
+                        result_types.append(ValTypeI32)
                     case "i64":
-                        result_types.append(I64)
+                        result_types.append(ValTypeI64)
                     case "f32":
-                        result_types.append(F32)
+                        result_types.append(ValTypeF32)
                     case "f64":
-                        result_types.append(F64)
+                        result_types.append(ValTypeF64)
 
         return FuncType(FtTag, param_types, result_types)
 
 
 class Import:
 
     def __init__(self, importidx=None, module=None, name=None, typeidx=None):
```

### Comparing `BREWasm-0.0/BREWasm/rewriter/indices_fixer.py` & `BREWasm-0.2/BREWasm/rewriter/indices_fixer.py`

 * *Files identical despite different names*

### Comparing `BREWasm-0.0/BREWasm/rewriter/modify_binary.py` & `BREWasm-0.2/BREWasm/rewriter/change_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,71 @@
 import os
 import struct
 
 from leb128 import LEB128U, LEB128S
-from shutil import copyfile
+
 from BREWasm.parser import reader
 from BREWasm.parser.instruction import Instruction
 from BREWasm.parser.module import *
 from BREWasm.parser.opcodes import *
 from BREWasm.parser.types import val_type_to_str, GlobalType
 
 
-class ModifyBinary:
+class ChangeBinary:
+
+    def __init__(self, path: str):
+        module, err = reader.decode_file(path)
+        if err is not None:
+            print(err.args)
+            print("=================================")
+            raise Exception("Failed to read the wasm file!")
+        self.path = path
+        self.module = module
+
+        self.func_name = []
+        for custom in self.module.custom_secs:
+            if custom.name == "name":
+                if custom.name_data.funcNameSubSec is not None:
+
+                    for func_name_item in custom.name_data.funcNameSubSec[self.get_import_func_num():]:
+                        self.func_name.append(func_name_item.name)
 
-    def __init__(self, module: Module, path: str):
+    def __init__(self, path: str, module: Module):
         if module is None:
             module, err = reader.decode_file(path)
             if err is not None:
                 print(err.args)
                 print("=================================")
                 raise Exception("Failed to read the wasm file!")
-
+            self.path = path
             self.module = module
-            self.module.path = path
 
             self.func_name = []
             for custom in self.module.custom_secs:
                 if custom.name == "name":
                     if custom.name_data.funcNameSubSec is not None:
 
                         for func_name_item in custom.name_data.funcNameSubSec[self.get_import_func_num():]:
                             self.func_name.append(func_name_item.name)
         else:
             self.module = module
-            self.module.path = path
+            self.path = path
 
-    def emit_binary(self, path):
-        file_path = self.module.path
-        if not os.path.samefile(self.module.path, path):
-            if os.path.isfile(path):
-                os.remove(path)
-            copyfile(self.module.path, path)
-            file_path = path
-
-        self.change_custom_name_section(self.module.custom_secs, file_path)
-        self.change_type_section(self.module.type_sec, file_path)
-        self.change_import_section(self.module.import_sec, file_path)
-        self.change_export_section(self.module.export_sec, file_path)
-        self.change_func_section(self.module.func_sec, file_path)
-        self.change_code_section(self.module.code_sec, file_path)
-        self.change_table_section(self.module.table_sec, file_path)
-        self.change_elem_section(self.module.elem_sec, file_path)
-        self.change_memory_section(self.module.mem_sec, file_path)
-        self.change_data_section(self.module.data_sec, file_path)
-        self.change_global_section(self.module.global_sec, file_path)
+    def emit_binary(self):
+        self.change_custom_name_section(self.module.custom_secs)
+        self.change_type_section(self.module.type_sec)
+        self.change_import_section(self.module.import_sec)
+        self.change_export_section(self.module.export_sec)
+        self.change_func_section(self.module.func_sec)
+        self.change_code_section(self.module.code_sec)
+        self.change_table_section(self.module.table_sec)
+        self.change_elem_section(self.module.elem_sec)
+        self.change_memory_section(self.module.mem_sec)
+        self.change_data_section(self.module.data_sec)
+        self.change_global_section(self.module.global_sec)
 
     def get_import_func_list(self):
         import_func_list = []
         for import_item in self.module.import_sec:
             if import_item.desc.func_type is not None:
                 import_func_list.append(import_item)
 
@@ -399,15 +408,15 @@
                     self.module.section_range[i].start += change
                     self.module.section_range[i].end += change
             for _, custom in enumerate(self.module.section_range[0]):
                 if _ != custom_sec_id and start <= custom.start:
                     custom.start += change
                     custom.end += change
 
-    def change_custom_name_section(self, custom_vec: list, file_path):
+    def change_custom_name_section(self, custom_vec: list):
 
         for _, custom in enumerate(custom_vec):
             if custom.name == "name":
                 name_section_bytes = bytes()
                 name_section_bytes += LEB128U.encode(len(custom.name))
                 name_section_bytes += bytes(custom.name, encoding="utf-8")
                 if custom.name_data.moduleNameSubSec != None:
@@ -465,15 +474,15 @@
                     dataname_bytes += LEB128U.encode(len(custom.name_data.dataNameSubSec))
                     for dataname in custom.name_data.dataNameSubSec:
                         dataname_bytes += LEB128U.encode(dataname.idx)
                         dataname_bytes += LEB128U.encode(len(dataname.name))
                         dataname_bytes += bytes(dataname.name, encoding="utf-8")
                     name_section_bytes += (bytes([0x09]) + LEB128U.encode(len(dataname_bytes))) + dataname_bytes
 
-                with open(os.path.abspath(file_path), "rb+") as f:
+                with open(os.path.abspath(self.path), "rb+") as f:
                     file_bytes = f.read()
                     custom = self.module.section_range[SecCustomID][_]
                     start = custom.start
                     end = custom.end
                     name_section_bytes = bytes([0x00]) + LEB128U.encode(len(name_section_bytes)) + name_section_bytes
                     file_new_bytes = file_bytes[:start] + name_section_bytes + file_bytes[end:]
                     change = len(name_section_bytes) - (end - start)
@@ -485,15 +494,15 @@
                     f.write(file_new_bytes)
             else:
                 custom_section_bytes = bytes()
                 custom_section_bytes += LEB128U.encode(len(custom.name))
                 custom_section_bytes += bytes(custom.name, encoding="utf-8")
                 custom_section_bytes += custom.custom_sec_data
 
-                with open(os.path.abspath(file_path), "rb+") as f:
+                with open(os.path.abspath(self.path), "rb+") as f:
                     file_bytes = f.read()
                     custom = self.module.section_range[SecCustomID][_]
                     start = custom.start
                     end = custom.end
                     custom_section_bytes = bytes([0x00]) + LEB128U.encode(
                         len(custom_section_bytes)) + custom_section_bytes
                     file_new_bytes = file_bytes[:start] + custom_section_bytes + file_bytes[end:]
@@ -503,15 +512,15 @@
                     self.fix_section_range(SecCustomID, change, custom.start, _)
                     f.seek(0)
                     f.truncate()
                     f.write(file_new_bytes)
 
         return None
 
-    def change_import_section(self, import_vec: list, file_path):
+    def change_import_section(self, import_vec: list):
 
         import_vec_len = len(import_vec)
         import_vec_len_bytes = LEB128U.encode(import_vec_len)
         import_vec_bytes = bytes()
         import_vec_bytes += import_vec_len_bytes
         if import_vec == []:
             return
@@ -527,15 +536,15 @@
                 import_vec_bytes += self.write_table_type(i.desc.table)
             elif i.desc.mem is not None:
                 import_vec_bytes += self.write_limits(i.desc.mem)
             elif i.desc.global_type is not None:
                 import_vec_bytes += self.write_global_type(i.desc.global_type)
         import_section_bytes = bytes([0x02]) + LEB128U.encode(len(import_vec_bytes)) + import_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[
                              :self.module.section_range[SecImportID].start] + import_section_bytes + file_bytes[
                                                                                                      self.module.section_range[
                                                                                                          SecImportID].end:]
             change = len(import_section_bytes) - (
                     self.module.section_range[SecImportID].end - self.module.section_range[SecImportID].start)
@@ -545,30 +554,30 @@
             self.fix_section_range(SecImportID, change, self.module.section_range[SecImportID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return import_section_bytes
 
-    def change_export_section(self, export_vec: list, file_path):
+    def change_export_section(self, export_vec: list):
         export_vec_len = len(export_vec)
         export_vec_len_bytes = LEB128U.encode(export_vec_len)
         export_vec_bytes = bytes()
         export_vec_bytes += export_vec_len_bytes
         if export_vec == []:
             return
         for export_item in export_vec:
             export_vec_bytes += LEB128U.encode(len(export_item.name))
             export_vec_bytes += bytes(export_item.name, encoding="utf-8")
             export_vec_bytes += LEB128U.encode(export_item.desc.tag)
             export_vec_bytes += LEB128U.encode(export_item.desc.idx)
 
         export_section_bytes = bytes([0x07]) + LEB128U.encode(len(export_vec_bytes)) + export_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[
                              :self.module.section_range[SecExportID].start] + export_section_bytes + file_bytes[
                                                                                                      self.module.section_range[
                                                                                                          SecExportID].end:]
             change = len(export_section_bytes) - (
                     self.module.section_range[SecExportID].end - self.module.section_range[SecExportID].start)
@@ -578,30 +587,30 @@
             self.fix_section_range(SecExportID, change, self.module.section_range[SecExportID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return export_section_bytes
 
-    def change_start_section(self, export_vec: list, file_path):
+    def change_start_section(self, export_vec: list):
         export_vec_len = len(export_vec)
         export_vec_len_bytes = LEB128U.encode(export_vec_len)
         export_vec_bytes = bytes()
         export_vec_bytes += export_vec_len_bytes
         if export_vec == []:
             return
         for export_item in export_vec:
             export_vec_bytes += LEB128U.encode(len(export_item.name))
             export_vec_bytes += bytes(export_item.name, encoding="utf-8")
             export_vec_bytes += LEB128U.encode(export_item.desc.tag)
             export_vec_bytes += LEB128U.encode(export_item.desc.idx)
 
         export_section_bytes = bytes([0x07]) + LEB128U.encode(len(export_vec_bytes)) + export_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[
                              :self.module.section_range[SecExportID].start] + export_section_bytes + file_bytes[
                                                                                                      self.module.section_range[
                                                                                                          SecExportID].end:]
             change = len(export_section_bytes) - (
                     self.module.section_range[SecExportID].end - self.module.section_range[SecExportID].start)
@@ -611,15 +620,15 @@
             self.fix_section_range(SecExportID, change, self.module.section_range[SecExportID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return export_section_bytes
 
-    def change_memory_section(self, memory_vec: list, file_path):
+    def change_memory_section(self, memory_vec: list):
         memory_vec_len = len(memory_vec)
         memory_vec_len_bytes = LEB128U.encode(memory_vec_len)
         memory_vec_bytes = bytes()
         memory_vec_bytes += memory_vec_len_bytes
         if memory_vec == []:
             return
         for memory_item in memory_vec:
@@ -628,15 +637,15 @@
             memory_item_bytes += LEB128U.encode(memory_item.min)
             if memory_item.max != 0:
                 memory_item_bytes += LEB128U.encode(memory_item.max)
             memory_vec_bytes += memory_item_bytes
 
         memroy_section_bytes = bytes([SecMemID]) + LEB128U.encode(len(memory_vec_bytes)) + memory_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[
                              :self.module.section_range[SecMemID].start] + memroy_section_bytes + file_bytes[
                                                                                                   self.module.section_range[
                                                                                                       SecMemID].end:]
             change = len(memroy_section_bytes) - (
                     self.module.section_range[SecMemID].end - self.module.section_range[SecMemID].start)
@@ -646,15 +655,15 @@
             self.fix_section_range(SecMemID, change, self.module.section_range[SecMemID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return memroy_section_bytes
 
-    def change_data_section(self, data_vec: list, file_path):
+    def change_data_section(self, data_vec: list):
         data_vec_len = len(data_vec)
         data_vec_len_bytes = LEB128U.encode(data_vec_len)
         data_vec_bytes = bytes()
         data_vec_bytes += data_vec_len_bytes
         if not data_vec:
             return
         for data_item in data_vec:
@@ -664,15 +673,15 @@
             data_item_bytes += LEB128U.encode(len(data_item.init))
             data_item_bytes += data_item.init
 
             data_vec_bytes += data_item_bytes
 
         data_section_bytes = bytes([SecDataID]) + LEB128U.encode(len(data_vec_bytes)) + data_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[
                              :self.module.section_range[SecDataID].start] + data_section_bytes + file_bytes[
                                                                                                  self.module.section_range[
                                                                                                      SecDataID].end:]
             change = len(data_section_bytes) - (
                     self.module.section_range[SecDataID].end - self.module.section_range[SecDataID].start)
@@ -682,15 +691,15 @@
             self.fix_section_range(SecDataID, change, self.module.section_range[SecDataID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return data_section_bytes
 
-    def change_elem_section(self, elem_vec: list, file_path):
+    def change_elem_section(self, elem_vec: list):
 
         elem_vec_len = len(elem_vec)
         elem_vec_len_bytes = LEB128U.encode(elem_vec_len)
         elem_vec_bytes = bytes()
         elem_vec_bytes += elem_vec_len_bytes
         if elem_vec == []:
             return
@@ -698,15 +707,15 @@
             elem_vec_bytes += LEB128U.encode(elem.table)
             elem_vec_bytes += self.write_expr(elem.offset)
             elem_vec_bytes += LEB128U.encode(len(elem.init))
             for func_idx in elem.init:
                 elem_vec_bytes += LEB128U.encode(func_idx)
         elem_section_bytes = bytes([SecElemID]) + LEB128U.encode(len(elem_vec_bytes)) + elem_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             binary_start = self.module.section_range[SecElemID].start
             binary_end = self.module.section_range[SecElemID].end
             if binary_start == binary_end:
                 for i in reversed(range(SecElemID)):
                     if self.module.section_range[i].start != self.module.section_range[i].end:
                         file_new_bytes = file_bytes[
@@ -736,15 +745,15 @@
                 self.fix_section_range(SecElemID, change, self.module.section_range[SecElemID].start)
                 f.seek(0)
                 f.truncate()
                 f.write(file_new_bytes)
 
         return elem_section_bytes
 
-    def change_type_section(self, functype_vec: list, file_path):
+    def change_type_section(self, functype_vec: list):
 
         functype_vec_len = len(functype_vec)
         functype_vec_len_bytes = LEB128U.encode(functype_vec_len)
         functype_vec_bytes = bytes()
         functype_vec_bytes += functype_vec_len_bytes
         if functype_vec == []:
             return
@@ -752,15 +761,15 @@
             functype_bytes = bytes()
             functype_bytes += bytes([0x60])
             functype_bytes += self.write_val_types(functype.param_types)
             functype_bytes += self.write_val_types(functype.result_types)
             functype_vec_bytes += functype_bytes
         type_section_bytes = bytes([0x01]) + LEB128U.encode(len(functype_vec_bytes)) + functype_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[:self.module.section_range[SecTypeID].start] + type_section_bytes + file_bytes[
                                                                                                             self.module.section_range[
                                                                                                                 SecTypeID].end:]
             change = len(type_section_bytes) - (
                     self.module.section_range[SecTypeID].end - self.module.section_range[SecTypeID].start)
 
@@ -769,30 +778,30 @@
             self.fix_section_range(SecTypeID, change, self.module.section_range[SecTypeID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return type_section_bytes
 
-    def change_global_section(self, global_vec: list, file_path):
+    def change_global_section(self, global_vec: list):
 
         global_vec_len = len(global_vec)
         global_vec_len_bytes = LEB128U.encode(global_vec_len)
         global_vec_bytes = bytes()
         global_vec_bytes += global_vec_len_bytes
         if global_vec == []:
             return
         for global_item in global_vec:
             global_bytes = bytes()
             global_bytes += self.write_global(global_item)
             global_vec_bytes += global_bytes
 
         global_section_bytes = bytes([0x06]) + LEB128U.encode(len(global_vec_bytes)) + global_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             if self.module.section_range[SecGlobalID].start == 0:
                 for section in range(1, SecGlobalID):
                     if self.module.section_range[section].start != 0:
                         self.module.section_range[SecGlobalID].start = self.module.section_range[section].end
                         self.module.section_range[SecGlobalID].end = self.module.section_range[SecGlobalID].start
             file_new_bytes = file_bytes[
@@ -807,42 +816,42 @@
             self.fix_section_range(SecGlobalID, change, self.module.section_range[SecGlobalID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return global_section_bytes
 
-    def change_func_section(self, type_vec, file_path):
+    def change_func_section(self, type_vec):
 
         type_vec_len = len(type_vec)
         type_vec_len_bytes = LEB128U.encode(type_vec_len)
         type_vec_bytes = bytes()
         type_vec_bytes += type_vec_len_bytes
         if type_vec == []:
             return
         for type_item in type_vec:
             type_vec_bytes += LEB128U.encode(type_item)
 
         func_section_bytes = bytes([0x03]) + LEB128U.encode(len(type_vec_bytes)) + type_vec_bytes
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[:self.module.section_range[SecFuncID].start] + func_section_bytes + file_bytes[
                                                                                                             self.module.section_range[
                                                                                                                 SecFuncID].end:]
             change = len(func_section_bytes) - (
                     self.module.section_range[SecFuncID].end - self.module.section_range[SecFuncID].start)
 
             self.module.section_range[SecFuncID].end = self.module.section_range[SecFuncID].start + len(
                 func_section_bytes)
             self.fix_section_range(SecFuncID, change, self.module.section_range[SecFuncID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
-    def change_code_section(self, code_vec: list, file_path):
+    def change_code_section(self, code_vec: list):
 
         code_vec_len = len(code_vec)
         code_vec_len_bytes = LEB128U.encode(code_vec_len)
         code_vec_bytes = bytes()
         code_vec_bytes += code_vec_len_bytes
         if code_vec == []:
             return
@@ -860,15 +869,15 @@
                 locals_vec_bytes += bytes([local_type])
 
             expr_bytes += self.write_expr(code.expr)
             code_bytes += (locals_vec_len_bytes + locals_vec_bytes + expr_bytes)
             code_vec_bytes += LEB128U.encode(len(code_bytes)) + code_bytes
         code_section_bytes = bytes([0x0A]) + LEB128U.encode(len(code_vec_bytes)) + code_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             file_new_bytes = file_bytes[:self.module.section_range[SecCodeID].start] + code_section_bytes + file_bytes[
                                                                                                             self.module.section_range[
                                                                                                                 SecCodeID].end:]
             change = len(code_section_bytes) - (
                     self.module.section_range[SecCodeID].end - self.module.section_range[SecCodeID].start)
 
@@ -877,15 +886,15 @@
             self.fix_section_range(SecCodeID, change, self.module.section_range[SecCodeID].start)
             f.seek(0)
             f.truncate()
             f.write(file_new_bytes)
 
         return code_section_bytes
 
-    def change_table_section(self, table_vec: list, file_path):
+    def change_table_section(self, table_vec: list):
 
         table_vec_len = len(table_vec)
         table_vec_len_bytes = LEB128U.encode(table_vec_len)
         table_vec_bytes = bytes()
         table_vec_bytes += table_vec_len_bytes
         if table_vec == []:
             return
@@ -896,15 +905,15 @@
             table_type_bytes += LEB128U.encode(table_type.limits.min)
             if 0 != table_type.limits.max:
                 table_type_bytes += LEB128U.encode(table_type.limits.max)
             table_vec_bytes += table_type_bytes
 
         table_section_bytes = bytes([0x04]) + LEB128U.encode(len(table_vec_bytes)) + table_vec_bytes
 
-        with open(os.path.abspath(file_path), "rb+") as f:
+        with open(os.path.abspath(self.path), "rb+") as f:
             file_bytes = f.read()
             binary_start = self.module.section_range[SecTableID].start
             binary_end = self.module.section_range[SecTableID].end
             if binary_start == binary_end:
                 for i in reversed(range(SecTableID)):
                     if self.module.section_range[i].start != self.module.section_range[i].end:
                         file_new_bytes = file_bytes[
```

### Comparing `BREWasm-0.0/BREWasm/rewriter/section_rewriter.py` & `BREWasm-0.2/BREWasm/rewriter/section_rewriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,33 @@
+from BREWasm import Instruction
 from BREWasm.parser import module
-from BREWasm.rewriter.modify_binary import ModifyBinary
+from BREWasm.rewriter.change_binary import ChangeBinary
 from BREWasm.rewriter.defination import *
 from BREWasm.rewriter.indices_fixer import *
-from BREWasm.parser.instruction import Instruction
-from BREWasm.rewriter.indices_fixer import IndicesFixer
 
 
-# class RetInstrs:
-#     def __init__(self, index, instr, instrs):
-#         self.index = index
-#         self.instr = instr
-#         self.instrs = instrs
+class RetInstrs:
+    def __init__(self, index, instr, instrs):
+        self.index = index
+        self.instr = instr
+        self.instrs = instrs
 
 
 class SectionRewriter:
 
-    def __init__(self, module, **section):
-        """
-
-        Args:
-            module:
-            **section:
-        """
+    def __init__(self, module, **kwargs):
 
         allowed_params = ['typesec', 'importsec', 'funcsec', 'tablesec', 'memsec',
                           'globalsec', 'exportsec', 'startsec', 'elemsec', 'codesec',
                           'datasec', 'datacountsec', 'customsec']
 
-        if len(section) != 1:
+        if len(kwargs) != 1:
             raise ValueError("Only one parameter should be provided")
 
-        param_name = next(iter(section.keys()))
+        param_name = next(iter(kwargs.keys()))
         if param_name not in allowed_params:
             raise ValueError("Invalid parameter")
 
         self.module = module
         self.typesec = None
         self.importsec = None
         self.funcsec = None
@@ -46,15 +39,15 @@
         self.elemsec = None
         self.codesec = None
         self.datasec = None
         self.datacountsec = None
         self.customsec = None
         self.indices_fixer = IndicesFixer(module)
 
-        setattr(self, param_name, section[param_name])
+        setattr(self, param_name, kwargs[param_name])
 
     def select(self, query):
         if self.typesec is not None and isinstance(query, Type):
             type_list = []
             for idx, item in enumerate(self.module.type_sec):
                 param_types, result_types = item.get_signature()
                 if all(
@@ -364,21 +357,21 @@
         #                 (query.min is None or query.min == item.min,
         #                  query.max is None or query.max == item.max)
         #         ):
         #             mem_list.append(Memory(item.min, item.max))
         #     return mem_list
 
         elif self.globalsec is not None and isinstance(inserted_item, Global):
-            if inserted_item.valtype == I32:
+            if inserted_item.valtype == ValTypeI32:
                 init_value_instr = Instruction(I32Const, inserted_item.val)
-            elif inserted_item.valtype == I64:
+            elif inserted_item.valtype == ValTypeI64:
                 init_value_instr = Instruction(I64Const, inserted_item.val)
-            elif inserted_item.valtype == F32:
+            elif inserted_item.valtype == ValTypeF32:
                 init_value_instr = Instruction(F32Const, inserted_item.val)
-            elif inserted_item.valtype == F64:
+            elif inserted_item.valtype == ValTypeF64:
                 init_value_instr = Instruction(F64Const, inserted_item.val)
             else:
                 raise Exception("global type error!")
 
             if query is None:
                 self.module.global_sec.append(module.Global(GlobalType(inserted_item.valtype, inserted_item.mut),
                                                             [init_value_instr]))
@@ -805,35 +798,35 @@
             # update
             for t in type_list:
                 if new_item.arg_types is not None:
                     param_types = []
                     for arg in new_item.arg_types:
                         match arg:
                             case "i32":
-                                param_types.append(I32)
+                                param_types.append(ValTypeI32)
                             case "i64":
-                                param_types.append(I64)
+                                param_types.append(ValTypeI64)
                             case "f32":
-                                param_types.append(F32)
+                                param_types.append(ValTypeF32)
                             case "f64":
-                                param_types.append(F64)
+                                param_types.append(ValTypeF64)
                     self.module.type_sec[t.typeidx].param_types = param_types
 
                 if new_item.ret_types is not None:
                     result_types = []
                     for arg in new_item.ret_types:
                         match arg:
                             case "i32":
-                                result_types.append(I32)
+                                result_types.append(ValTypeI32)
                             case "i64":
-                                result_types.append(I64)
+                                result_types.append(ValTypeI64)
                             case "f32":
-                                result_types.append(F32)
+                                result_types.append(ValTypeF32)
                             case "f64":
-                                result_types.append(F64)
+                                result_types.append(ValTypeF64)
                     t.result_types = result_types
                     self.module.type_sec[t.typeidx].result_types = result_types
 
         elif self.importsec is not None and isinstance(query, Import):
 
             import_list = []
             for idx, item in enumerate(self.module.import_sec):
@@ -933,21 +926,21 @@
 
             for g in global_list:
                 if new_item.valtype is not None:
                     self.module.global_sec[g.globalidx].type.val_type = new_item.valtype
                 if new_item.mut is not None:
                     self.module.global_sec[g.globalidx].type.mut = new_item.mut
                 if new_item.val is not None:
-                    if self.module.global_sec[g.globalidx].type.val_type == I32:
+                    if self.module.global_sec[g.globalidx].type.val_type == ValTypeI32:
                         init_value_instr = Instruction(I32Const, new_item.val)
-                    elif self.module.global_sec[g.globalidx].type.val_type == I64:
+                    elif self.module.global_sec[g.globalidx].type.val_type == ValTypeI64:
                         init_value_instr = Instruction(I64Const, new_item.val)
-                    elif self.module.global_sec[g.globalidx].type.val_type == F32:
+                    elif self.module.global_sec[g.globalidx].type.val_type == ValTypeF32:
                         init_value_instr = Instruction(F32Const, new_item.val)
-                    elif self.module.global_sec[g.globalidx].type.val_type == F64:
+                    elif self.module.global_sec[g.globalidx].type.val_type == ValTypeF64:
                         init_value_instr = Instruction(F64Const, new_item.val)
                     self.module.global_sec[g.globalidx].init[0] = init_value_instr
 
         elif self.exportsec is not None and isinstance(query, Export):
             export_list = []
             for idx, item in enumerate(self.module.export_sec):
                 if all(
@@ -1097,15 +1090,69 @@
                         case _:
                             pass
 
         else:
             raise Exception("error")
 
     def emit_binary(self, path: str):
-        ModifyBinary(self.module, self.module.path).emit_binary(path)
+
+        ChangeBinary(self.module, path).emit_binary()
+
+    # def get_functype_idx(self, functype):
+    #     functype_id = None
+    #     for _, i in enumerate(self.module.type_sec):
+    #         if i.equal(functype) is True:
+    #             functype_id = _
+    #     return functype_id
+    #
+    # def get_funcsec_functypeidx(self, idx):
+    #     return self.module.func_sec[idx]
+    #
+    # def get_indirect_func_list(self):
+    #     indirect_func_list = []
+    #     for elem in self.module.elem_sec:
+    #         indirect_func_list.extend(elem.init)
+    #     return indirect_func_list
+    #
+    # def get_codesec_code(self, idx):
+    #     return self.module.code_sec[idx]
+    #
+    # def get_custom_list(self):
+    #     if self.module.custom_secs is None:
+    #         raise Exception("There is no custom section in this wasm module!")
+    #     return self.module.custom_secs
+    #
+    # def get_customsec_custom(self, idx=None, name=None):
+    #     if idx is not None:
+    #         return self.module.custom_secs[idx]
+    #     else:
+    #         for custom in self.get_custom_list():
+    #             if custom.name == name:
+    #                 return custom
+    #     raise Exception("No custom found")
+    #
+    # def get_codesec_code_list(self):
+    #     return self.module.code_sec
+    #
+    # def get_mem_list(self):
+    #     return self.module.mem_sec
+    #
+    # # 这里需要x
+    # def get_table_list(self):
+    #     return self.module.table_sec
+    #
+    # def get_namesec_funcname_list(self, namesec):
+    #     return namesec.name_data.funcNameSubSec
+    #
+    # def get_namesec_globalname_list(self, namesec):
+    #     return namesec.name_data.funcNameSubSec
+    #
+    # def get_namesec_dataname_list(self, namesec):
+    #     return namesec.name_data.dataNameSubSec
+    #
 
     # 这里的end没有算作指令
     def get_flat_instrs(self, instrs):
         ret_instrs = []
         for _, i in enumerate(instrs):
             if i.opcode in [Block, Loop]:
                 args = i.args
@@ -1137,81 +1184,81 @@
                 instrs[i].args.instrs2 = self.get_fold_instrs(instrs[i + 1, i + 1 + args_instrs2_length])
                 i = i + args_instrs2_length + 1
             else:
                 ret_instrs.append(instrs[i])
                 i += 1
         return ret_instrs
 
-    # def _get_instrs_instr(self, instrs, offset=None, current_offset=-1, instr=None, ret_instrs=[]):
-    #     if offset is not None:
-    #         for _, i in enumerate(instrs):
-    #             current_offset += 1
-    #             if i.opcode in [Block, Loop]:
-    #                 if offset == current_offset:
-    #                     return RetInstrs(_, i, instrs)
-    #                 args = i.args
-    #                 return self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr)
-    #                 # 将end也算一个指令
-    #                 current_offset += 1
-    #                 if offset == current_offset:
-    #                     raise Exception("end can not be get")
-    #             elif i.opcode == If:
-    #                 if offset == current_offset:
-    #                     return RetInstrs(_, i, instrs)
-    #                 args = i.args
-    #                 return self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset,
-    #                                               instr=instr)
-    #                 # 将else也算一个指令
-    #                 current_offset += 1
-    #                 if offset == current_offset:
-    #                     raise Exception("else can not be get")
-    #                 return self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset,
-    #                                               instr=instr)
-    #                 # 将end也算一个指令
-    #                 current_offset += 1
-    #                 if offset == current_offset:
-    #                     raise Exception("end can not be get")
-    #             else:
-    #                 if current_offset == offset:
-    #                     return RetInstrs(_, i, instrs)
-    #     elif instr is not None and instr.args is None:
-    #         ret_instrs = []
-    #         for _, i in enumerate(instrs):
-    #             if i.opcode in [Block, Loop]:
-    #                 if i.opcode == instr.opcode:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
-    #             elif i.opcode == If:
-    #                 if i.opcode == instr.opcode:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
-    #             else:
-    #                 if i.opcode == instr.opcode:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #         return ret_instrs
-    #     elif instr is not None:
-    #         ret_instrs = []
-    #         for _, i in enumerate(instrs):
-    #             if i.opcode in [Block, Loop]:
-    #                 if i.opcode == instr.opcode and i.args == instr.args:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
-    #             elif i.opcode == If:
-    #                 if i.opcode == instr.opcode and i.args == instr.args:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #                 args = i.args
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
-    #                 ret_instrs.extend(
-    #                     self._get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
-    #             else:
-    #                 if i.opcode == instr.opcode and i.args == instr.args:
-    #                     ret_instrs.append(RetInstrs(_, i, instrs))
-    #         return ret_instrs
+    def get_instrs_instr(self, instrs, offset=None, current_offset=-1, instr=None, ret_instrs=[]):
+        if offset is not None:
+            for _, i in enumerate(instrs):
+                current_offset += 1
+                if i.opcode in [Block, Loop]:
+                    if offset == current_offset:
+                        return RetInstrs(_, i, instrs)
+                    args = i.args
+                    return self.get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr)
+                    # 将end也算一个指令
+                    current_offset += 1
+                    if offset == current_offset:
+                        raise Exception("end can not be get")
+                elif i.opcode == If:
+                    if offset == current_offset:
+                        return RetInstrs(_, i, instrs)
+                    args = i.args
+                    return self.get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset,
+                                                 instr=instr)
+                    # 将else也算一个指令
+                    current_offset += 1
+                    if offset == current_offset:
+                        raise Exception("else can not be get")
+                    return self.get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset,
+                                                 instr=instr)
+                    # 将end也算一个指令
+                    current_offset += 1
+                    if offset == current_offset:
+                        raise Exception("end can not be get")
+                else:
+                    if current_offset == offset:
+                        return RetInstrs(_, i, instrs)
+        elif instr is not None and instr.args is None:
+            ret_instrs = []
+            for _, i in enumerate(instrs):
+                if i.opcode in [Block, Loop]:
+                    if i.opcode == instr.opcode:
+                        ret_instrs.append(RetInstrs(_, i, instrs))
+                    args = i.args
+                    ret_instrs.extend(
+                        self.get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
+                elif i.opcode == If:
+                    if i.opcode == instr.opcode:
+                        ret_instrs.append(RetInstrs(_, i, instrs))
+                    args = i.args
+                    ret_instrs.extend(
+                        self.get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
+                    ret_instrs.extend(
+                        self.get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
+                else:
+                    if i.opcode == instr.opcode:
+                        ret_instrs.append(RetInstrs(_, i, instrs))
+            return ret_instrs
+        elif instr is not None:
+            ret_instrs = []
+            for _, i in enumerate(instrs):
+                if i.opcode in [Block, Loop]:
+                    if i.opcode == instr.opcode and i.args == instr.args:
+                        ret_instrs.append(RetInstrs(_, i, instrs))
+                    args = i.args
+                    ret_instrs.extend(
+                        self.get_instrs_instr(args.instrs, offset=offset, current_offset=current_offset, instr=instr))
+                elif i.opcode == If:
+                    if i.opcode == instr.opcode and i.args == instr.args:
+                        ret_instrs.append(RetInstrs(_, i, instrs))
+                    args = i.args
+                    ret_instrs.extend(
+                        self.get_instrs_instr(args.instrs1, offset=offset, current_offset=current_offset, instr=instr))
+                    ret_instrs.extend(
+                        self.get_instrs_instr(args.instrs2, offset=offset, current_offset=current_offset, instr=instr))
+                else:
+                    if i.opcode == instr.opcode and i.args == instr.args:
+                        ret_instrs.append(RetInstrs(_, i, instrs))
+            return ret_instrs
```

### Comparing `BREWasm-0.0/BREWasm/rewriter/semantics_rewriter.py` & `BREWasm-0.2/BREWasm/rewriter/semantics_rewriter.py`

 * *Files identical despite different names*

### Comparing `BREWasm-0.0/BREWasm.egg-info/PKG-INFO` & `BREWasm-0.2/BREWasm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BREWasm
-Version: 0.0
+Version: 0.2
 Summary: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
 Home-page: https://github.com/BREWasm/brewasm-project
 Author: BREWasm
 License: MIT
 Keywords: BINARY,REWRITER,WASM
 Description-Content-Type: text/markdown
 
@@ -38,22 +38,23 @@
     - Function
     - Custom Content
 
 ## Installation
 
 ### Python package
 
-BREWasm is currently available on PIP repositories.
+BREWasm is currently not available on PIP repositories.
 
-Install BREWasm::
+To install it, you need to run at the root of the `git` repository:
 
 ```
-pip install BREWasm
+pip install --extra-index-url https://test.pypi.org/simple/ '.[all_backends]'
 ```
 
+The extra index is important, as it brings the latest version of Speculos.
 
 ## Examples
 
 ### Section Rewriter
 
 The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
 
@@ -94,8 +95,8 @@
                                            local_vec=[Local(0, I32), Local(1, I64)], funcbody)
 # Emit a new binary file
 binary.emit_binary('b.wasm')
 ```
 
 ## Documentation
 
-The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
+The complete documentation can be found [here](https://ledgerhq.github.io/ragger/).
```

### Comparing `BREWasm-0.0/BREWasm.egg-info/SOURCES.txt` & `BREWasm-0.2/BREWasm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 BREWasm/parser/module.py
 BREWasm/parser/opcodes.py
 BREWasm/parser/opnames.py
 BREWasm/parser/reader.py
 BREWasm/parser/types.py
 BREWasm/rewriter/BREWasm.py
 BREWasm/rewriter/__init__.py
+BREWasm/rewriter/change_binary.py
 BREWasm/rewriter/defination.py
 BREWasm/rewriter/indices_fixer.py
-BREWasm/rewriter/modify_binary.py
 BREWasm/rewriter/section_rewriter.py
 BREWasm/rewriter/semantics_rewriter.py
 doc/Definition.png
```

### Comparing `BREWasm-0.0/PKG-INFO` & `BREWasm-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BREWasm
-Version: 0.0
+Version: 0.2
 Summary: A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm
 Home-page: https://github.com/BREWasm/brewasm-project
 Author: BREWasm
 License: MIT
 Keywords: BINARY,REWRITER,WASM
 Description-Content-Type: text/markdown
 
@@ -38,22 +38,23 @@
     - Function
     - Custom Content
 
 ## Installation
 
 ### Python package
 
-BREWasm is currently available on PIP repositories.
+BREWasm is currently not available on PIP repositories.
 
-Install BREWasm::
+To install it, you need to run at the root of the `git` repository:
 
 ```
-pip install BREWasm
+pip install --extra-index-url https://test.pypi.org/simple/ '.[all_backends]'
 ```
 
+The extra index is important, as it brings the latest version of Speculos.
 
 ## Examples
 
 ### Section Rewriter
 
 The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
 
@@ -94,8 +95,8 @@
                                            local_vec=[Local(0, I32), Local(1, I64)], funcbody)
 # Emit a new binary file
 binary.emit_binary('b.wasm')
 ```
 
 ## Documentation
 
-The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
+The complete documentation can be found [here](https://ledgerhq.github.io/ragger/).
```

### Comparing `BREWasm-0.0/README.md` & `BREWasm-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,23 @@
     - Function
     - Custom Content
 
 ## Installation
 
 ### Python package
 
-BREWasm is currently available on PIP repositories.
+BREWasm is currently not available on PIP repositories.
 
-Install BREWasm::
+To install it, you need to run at the root of the `git` repository:
 
 ```
-pip install BREWasm
+pip install --extra-index-url https://test.pypi.org/simple/ '.[all_backends]'
 ```
 
+The extra index is important, as it brings the latest version of Speculos.
 
 ## Examples
 
 ### Section Rewriter
 
 The basic operation of the section rewriter is `select`, `insert`, `update` and `delete`.
 
@@ -84,8 +85,8 @@
                                            local_vec=[Local(0, I32), Local(1, I64)], funcbody)
 # Emit a new binary file
 binary.emit_binary('b.wasm')
 ```
 
 ## Documentation
 
-The complete documentation can be found [here](https://brewasm-project.readthedocs.io/en/latest/).
+The complete documentation can be found [here](https://ledgerhq.github.io/ragger/).
```

### Comparing `BREWasm-0.0/doc/Definition.png` & `BREWasm-0.2/doc/Definition.png`

 * *Files identical despite different names*

### Comparing `BREWasm-0.0/setup.py` & `BREWasm-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setup.py
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='UTF-16LE') as f:
   long_description = f.read()
 
 setup(name='BREWasm',
-      version='0.0',
+      version='0.2',
       description='A general purpose static binary rewriting framework for Wasm, which aims at reducing the complexity of the Wasm',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=find_packages(),
       url='https://github.com/BREWasm/brewasm-project',
       author='BREWasm',
       license='MIT',
```

