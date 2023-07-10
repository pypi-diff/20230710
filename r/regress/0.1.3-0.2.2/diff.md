# Comparing `tmp/regress-0.1.3.tar.gz` & `tmp/regress-0.2.2.tar.gz`

## Comparing `regress-0.1.3.tar` & `regress-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 regress-0.1.3/Cargo.toml
--rw-r--r--   0        0        0      219 2023-03-17 16:30:00.000000 regress-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     4321 2023-03-17 16:30:00.000000 regress-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2023-03-17 16:30:00.000000 regress-0.1.3/.gitignore
--rw-r--r--   0        0        0     1039 2023-03-17 16:30:00.000000 regress-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1076 2023-03-17 16:30:00.000000 regress-0.1.3/LICENSE
--rw-r--r--   0        0        0      799 2023-03-17 16:30:00.000000 regress-0.1.3/README.rst
--rw-r--r--   0        0        0     1043 2023-03-17 16:30:00.000000 regress-0.1.3/noxfile.py
--rw-r--r--   0        0        0     1166 2023-03-17 16:30:00.000000 regress-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      407 2023-03-17 16:30:00.000000 regress-0.1.3/regress.pyi
--rw-r--r--   0        0        0     1976 2023-03-17 16:30:00.000000 regress-0.1.3/src/lib.rs
--rw-r--r--   0        0        0        8 2023-03-17 16:30:00.000000 regress-0.1.3/tests/requirements.in
--rw-r--r--   0        0        0      352 2023-03-17 16:30:00.000000 regress-0.1.3/tests/requirements.txt
--rw-r--r--   0        0        0     1230 2023-03-17 16:30:00.000000 regress-0.1.3/tests/test_regress.py
--rw-r--r--   0        0        0     9087 2023-03-17 16:30:00.000000 regress-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 regress-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 regress-0.2.2/Cargo.toml
+-rw-r--r--   0        0        0      219 2023-07-10 10:02:28.000000 regress-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       81 2023-07-10 10:02:28.000000 regress-0.2.2/.github/release.yml
+-rw-r--r--   0        0        0     4321 2023-07-10 10:02:28.000000 regress-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2023-07-10 10:02:28.000000 regress-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1039 2023-07-10 10:02:28.000000 regress-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1076 2023-07-10 10:02:28.000000 regress-0.2.2/LICENSE
+-rw-r--r--   0        0        0      799 2023-07-10 10:02:28.000000 regress-0.2.2/README.rst
+-rw-r--r--   0        0        0     1849 2023-07-10 10:02:28.000000 regress-0.2.2/noxfile.py
+-rw-r--r--   0        0        0     1164 2023-07-10 10:02:28.000000 regress-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-07-10 10:02:28.000000 regress-0.2.2/regress.pyi
+-rw-r--r--   0        0        0     1976 2023-07-10 10:02:28.000000 regress-0.2.2/src/lib.rs
+-rw-r--r--   0        0        0        8 2023-07-10 10:02:28.000000 regress-0.2.2/tests/requirements.in
+-rw-r--r--   0        0        0      352 2023-07-10 10:02:28.000000 regress-0.2.2/tests/requirements.txt
+-rw-r--r--   0        0        0     1230 2023-07-10 10:02:28.000000 regress-0.2.2/tests/test_regress.py
+-rw-r--r--   0        0        0     9087 2023-07-10 10:02:28.000000 regress-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 regress-0.2.2/PKG-INFO
```

### Comparing `regress-0.1.3/.github/workflows/CI.yml` & `regress-0.2.2/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
             nox --list-sessions |
             grep '^* ' |
             cut -d ' ' -f 2- |
             jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
@@ -61,15 +61,15 @@
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - name: Run nox
         run: nox -s "${{ matrix.noxenv }}"
 
   linux:
     needs: test
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `regress-0.1.3/.gitignore` & `regress-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `regress-0.1.3/.pre-commit-config.yaml` & `regress-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `regress-0.1.3/LICENSE` & `regress-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `regress-0.1.3/README.rst` & `regress-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `regress-0.1.3/pyproject.toml` & `regress-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "regress"
 description = "Python bindings to Rust's regress ECMA regular expressions library"
 readme = "README.rst"
 license = {text = "MIT"}
```

### Comparing `regress-0.1.3/src/lib.rs` & `regress-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `regress-0.1.3/tests/test_regress.py` & `regress-0.2.2/tests/test_regress.py`

 * *Files identical despite different names*

### Comparing `regress-0.1.3/Cargo.lock` & `regress-0.2.2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.17.1"
@@ -113,66 +113,66 @@
 checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -191,25 +191,25 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regress"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d995d590bd8ec096d1893f414bf3f5e8b0ee4c9eed9a5642b9766ef2c8e2e8e9"
+checksum = "82a9ecfa0cb04d0b04dddb99b8ccf4f66bc8dfd23df694b398570bd8ae3a50fb"
 dependencies = [
  "hashbrown",
  "memchr",
 ]
 
 [[package]]
 name = "regress-py"
-version = "0.1.3"
+version = "0.2.2"
 dependencies = [
  "pyo3",
  "regress",
 ]
 
 [[package]]
 name = "scopeguard"
```

### Comparing `regress-0.1.3/PKG-INFO` & `regress-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regress
-Version: 0.1.3
+Version: 0.2.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

