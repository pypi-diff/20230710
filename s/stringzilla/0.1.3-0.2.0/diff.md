# Comparing `tmp/stringzilla-0.1.3-cp39-cp39-win_amd64.whl.zip` & `tmp/stringzilla-0.2.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 97823 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   241152 b- defN 23-Jul-08 00:09 stringzilla.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     4019 b- defN 23-Jul-08 00:09 stringzilla-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-08 00:09 stringzilla-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-08 00:09 stringzilla-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      404 b- defN 23-Jul-08 00:09 stringzilla-0.1.3.dist-info/RECORD
-5 files, 245687 bytes uncompressed, 97073 bytes compressed:  60.5%
+Zip file size: 99257 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   244224 b- defN 23-Jul-09 23:16 stringzilla.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     4564 b- defN 23-Jul-09 23:16 stringzilla-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-09 23:16 stringzilla-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-09 23:16 stringzilla-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      404 b- defN 23-Jul-09 23:16 stringzilla-0.2.0.dist-info/RECORD
+5 files, 249304 bytes uncompressed, 98507 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: stringzilla.cp39-win_amd64.pyd
 Comment: 
 
-Filename: stringzilla-0.1.3.dist-info/METADATA
+Filename: stringzilla-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: stringzilla-0.1.3.dist-info/WHEEL
+Filename: stringzilla-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: stringzilla-0.1.3.dist-info/top_level.txt
+Filename: stringzilla-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: stringzilla-0.1.3.dist-info/RECORD
+Filename: stringzilla-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `stringzilla-0.1.3.dist-info/METADATA` & `stringzilla-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stringzilla
-Version: 0.1.3
+Version: 0.2.0
 Summary: Crunch 100+ GB Strings in Python with ease
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -79,15 +79,15 @@
 ```sh
 pip install stringzilla
 ```
 
 There are two classes you can use interchangibly:
 
 ```python
-from stringzilla import Str, File, Slices
+from stringzilla import Str, File, Strs
 
 text: str = 'some-string'
 text: Str = Str('some-string')
 text: File = File('some-file.txt')
 ```
 
 Once constructed, following interfaces are supported:
@@ -117,34 +117,56 @@
     allowoverlap=False, # optional
 ) -> int
 
 text.splitlines(
     keeplinebreaks=False, # optional
     **, # non-traditional arguments:
     separator='\n', # optional
-) -> Slices # similar to list[str]
+) -> Strs # similar to list[str]
 
 text.split(
     separator=' ', # optional
     maxsplit=9223372036854775807, # optional
     **, # non-traditional arguments:
     keepseparator=False, # optional
-) -> Slices # similar to list[str]
+) -> Strs # similar to list[str]
 ```
 
 ## Development
 
 ```sh
 rm -rf build && pip install -e . && pytest scripts/test.py -s -x
+
+pip install -e . --no-index --no-deps
 ```
 
 To benchmark on some custom file and pattern combination:
 
 ```sh
-python scripts/bench.py --path "your file" --pattern "your pattern"
+python scripts/bench.py --haystack_path "your file" --needle "your pattern"
+```
+
+To benchmark on syntetic data:
+
+```sh
+python scripts/bench.py --haystack_pattern "abcd" --haystack_length 1e9 --needle "abce"
 ```
 
 To validate packaging:
 
 ```sh
 cibuildwheel --platform linux
 ```
+
+Compilin C++ tests:
+
+
+```sh
+brew install libomp llvm
+cmake -B ./build_release \
+    -DCMAKE_C_COMPILER="/opt/homebrew/opt/llvm/bin/clang" \
+    -DCMAKE_CXX_COMPILER="/opt/homebrew/opt/llvm/bin/clang++" \
+    -DSTRINGZILLA_USE_OPENMP=1 \
+    -DSTRINGZILLA_BUILD_TEST=1 \
+    && \
+    make -C ./build_release -j && ./build_release/stringzilla_test
+```
```

