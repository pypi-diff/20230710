# Comparing `tmp/regress-0.2.2.tar.gz` & `tmp/regress-0.2.3.tar.gz`

## Comparing `regress-0.2.2.tar` & `regress-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 regress-0.2.2/Cargo.toml
--rw-r--r--   0        0        0      219 2023-07-10 10:02:28.000000 regress-0.2.2/.github/dependabot.yml
--rw-r--r--   0        0        0       81 2023-07-10 10:02:28.000000 regress-0.2.2/.github/release.yml
--rw-r--r--   0        0        0     4321 2023-07-10 10:02:28.000000 regress-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-07-10 10:02:28.000000 regress-0.2.2/.gitignore
--rw-r--r--   0        0        0     1039 2023-07-10 10:02:28.000000 regress-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-07-10 10:02:28.000000 regress-0.2.2/LICENSE
--rw-r--r--   0        0        0      799 2023-07-10 10:02:28.000000 regress-0.2.2/README.rst
--rw-r--r--   0        0        0     1849 2023-07-10 10:02:28.000000 regress-0.2.2/noxfile.py
--rw-r--r--   0        0        0     1164 2023-07-10 10:02:28.000000 regress-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      407 2023-07-10 10:02:28.000000 regress-0.2.2/regress.pyi
--rw-r--r--   0        0        0     1976 2023-07-10 10:02:28.000000 regress-0.2.2/src/lib.rs
--rw-r--r--   0        0        0        8 2023-07-10 10:02:28.000000 regress-0.2.2/tests/requirements.in
--rw-r--r--   0        0        0      352 2023-07-10 10:02:28.000000 regress-0.2.2/tests/requirements.txt
--rw-r--r--   0        0        0     1230 2023-07-10 10:02:28.000000 regress-0.2.2/tests/test_regress.py
--rw-r--r--   0        0        0     9087 2023-07-10 10:02:28.000000 regress-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 regress-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 regress-0.2.3/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-10 14:50:18.000000 regress-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-10 14:50:18.000000 regress-0.2.3/.github/release.yml
+-rw-r--r--   0        0        0     5148 2023-07-10 14:50:18.000000 regress-0.2.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-10 14:50:18.000000 regress-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1039 2023-07-10 14:50:18.000000 regress-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-10 14:50:18.000000 regress-0.2.3/LICENSE
+-rw-r--r--   0        0        0      799 2023-07-10 14:50:18.000000 regress-0.2.3/README.rst
+-rw-r--r--   0        0        0     1849 2023-07-10 14:50:18.000000 regress-0.2.3/noxfile.py
+-rw-r--r--   0        0        0     1164 2023-07-10 14:50:18.000000 regress-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-07-10 14:50:18.000000 regress-0.2.3/regress.pyi
+-rw-r--r--   0        0        0     1976 2023-07-10 14:50:18.000000 regress-0.2.3/src/lib.rs
+-rw-r--r--   0        0        0        8 2023-07-10 14:50:18.000000 regress-0.2.3/tests/requirements.in
+-rw-r--r--   0        0        0      352 2023-07-10 14:50:18.000000 regress-0.2.3/tests/requirements.txt
+-rw-r--r--   0        0        0     1230 2023-07-10 14:50:18.000000 regress-0.2.3/tests/test_regress.py
+-rw-r--r--   0        0        0     9087 2023-07-10 14:50:18.000000 regress-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 regress-0.2.3/PKG-INFO
```

### Comparing `regress-0.2.2/.github/workflows/CI.yml` & `regress-0.2.3/.github/workflows/CI.yml`

 * *Files 10% similar despite different names*

```diff
@@ -65,37 +65,63 @@
         with:
           python-version: "3.x"
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
-  linux:
+  manylinux:
     needs: test
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 pypy3.8 pypy3.9'
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 3.12 pypy3.8 pypy3.9 pypy3.10'
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
+  musllinux:
+    needs: test
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        target:
+          - aarch64-unknown-linux-musl
+          - i686-unknown-linux-musl
+          - x86_64-unknown-linux-musl
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.x"
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.target }}
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 3.12 pypy3.8 pypy3.9 pypy3.10'
+          manylinux: musllinux_1_2
+      - name: Upload wheels
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
+
   windows:
     needs: test
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
     steps:
@@ -126,26 +152,26 @@
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
+          args: --release --out dist --interpreter '3.8 3.9 3.10 3.11 3.12 pypy3.8 pypy3.9 pypy3.10'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos]
+    needs: [manylinux, musllinux, windows, macos]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
```

### Comparing `regress-0.2.2/.gitignore` & `regress-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/.pre-commit-config.yaml` & `regress-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/LICENSE` & `regress-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/README.rst` & `regress-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/noxfile.py` & `regress-0.2.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/pyproject.toml` & `regress-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/src/lib.rs` & `regress-0.2.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/tests/test_regress.py` & `regress-0.2.3/tests/test_regress.py`

 * *Files identical despite different names*

### Comparing `regress-0.2.2/Cargo.lock` & `regress-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 dependencies = [
  "hashbrown",
  "memchr",
 ]
 
 [[package]]
 name = "regress-py"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "pyo3",
  "regress",
 ]
 
 [[package]]
 name = "scopeguard"
```

### Comparing `regress-0.2.2/PKG-INFO` & `regress-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regress
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

