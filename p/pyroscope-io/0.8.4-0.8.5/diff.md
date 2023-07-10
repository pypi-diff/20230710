# Comparing `tmp/pyroscope-io-0.8.4.tar.gz` & `tmp/pyroscope-io-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscope-io-0.8.4.tar", last modified: Thu Jun 15 14:36:00 2023, max compression
+gzip compressed data, was "pyroscope-io-0.8.5.tar", last modified: Mon Jul 10 05:58:37 2023, max compression
```

## Comparing `pyroscope-io-0.8.4.tar` & `pyroscope-io-0.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/.cargo/config
--rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/cbindgen.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/include/pyroscope_ffi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/pyroscope/
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/pyroscope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/pyroscope_io/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/pyroscope_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:36:00.465034 pyroscope-io-0.8.4/pyroscope_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 14:36:00.000000 pyroscope-io-0.8.4/pyroscope_io.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-15 14:36:00.469034 pyroscope-io-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-15 14:35:49.000000 pyroscope-io-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/.cargo/config
+-rw-r--r--   0 runner    (1001) docker     (123)    63646 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/cbindgen.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/include/pyroscope_ffi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/pyroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/pyroscope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/pyroscope_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/pyroscope_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/pyroscope_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 05:58:37.000000 pyroscope-io-0.8.5/pyroscope_io.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-10 05:58:37.042124 pyroscope-io-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-10 05:58:26.000000 pyroscope-io-0.8.5/setup.py
```

### Comparing `pyroscope-io-0.8.4/LICENSE` & `pyroscope-io-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.4/PKG-INFO` & `pyroscope-io-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.4
+Version: 0.8.5
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
```

### Comparing `pyroscope-io-0.8.4/README.md` & `pyroscope-io-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.4/lib/Cargo.lock` & `pyroscope-io-0.8.5/lib/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1270,17 +1270,17 @@
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "names"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7d66043b25d4a6cccb23619d10c19c25304b355a7dccd4a8e11423dd2382146"
+checksum = "7bddcd3bf5144b6392de80e04c347cd7fab2508f6df16a85fc496ecd5cec39bc"
 dependencies = [
  "clap 3.2.23",
  "rand",
 ]
 
 [[package]]
 name = "nix"
@@ -1508,27 +1508,27 @@
  "libproc 0.12.0",
  "mach2",
  "winapi",
 ]
 
 [[package]]
 name = "prost"
-version = "0.10.4"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71adf41db68aa0daaefc69bb30bcd68ded9b9abaad5d1fbb6304c4fb390e083e"
+checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.10.1"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b670f45da57fb8542ebdbb6105a925fe571b67f9e7ed9f47a06a84e72b4e7cc"
+checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
  "syn",
 ]
@@ -1566,15 +1566,15 @@
  "tempfile",
  "termios",
  "winapi",
 ]
 
 [[package]]
 name = "pyroscope"
-version = "0.5.5"
+version = "0.5.6"
 dependencies = [
  "json",
  "libc",
  "libflate",
  "log",
  "names",
  "prost",
```

### Comparing `pyroscope-io-0.8.4/lib/cbindgen.toml` & `pyroscope-io-0.8.5/lib/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.4/lib/include/pyroscope_ffi.h` & `pyroscope-io-0.8.5/lib/include/pyroscope_ffi.h`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.4/lib/src/lib.rs` & `pyroscope-io-0.8.5/lib/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use ffikit::Signal;
 use pyroscope::backend::Tag;
 use pyroscope::PyroscopeAgent;
+use pyroscope::pyroscope::ReportEncoding;
 use pyroscope_pyspy::{pyspy_backend, PyspyConfig};
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::CStr;
 use std::hash::Hasher;
 use std::os::raw::c_char;
 
 const LOG_TAG: &str = "Pyroscope::pyspy::ffi";
@@ -139,14 +140,15 @@
     let tags = string_to_tags(tags_ref);
 
     // Create the Pyspy Backend.
     let pyspy = pyspy_backend(pyspy_config);
 
     // Create the Pyroscope Agent.
     let mut agent_builder = PyroscopeAgent::builder(server_address, application_name)
+        .report_encoding(ReportEncoding::PPROF)
         .backend(pyspy)
         .tags(tags);
 
     // Add the auth token if it is not empty.
     if auth_token != "" {
         agent_builder = agent_builder.auth_token(auth_token);
     } else if basic_auth_username != "" && basic_auth_password != "" {
```

### Comparing `pyroscope-io-0.8.4/pyroscope/__init__.py` & `pyroscope-io-0.8.5/pyroscope/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroscope-io-0.8.4/pyroscope_io.egg-info/PKG-INFO` & `pyroscope-io-0.8.5/pyroscope_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscope-io
-Version: 0.8.4
+Version: 0.8.5
 Summary: Pyroscope Python integration
 Home-page: https://pyroscope.io
 Maintainer: Abid Omar
 Maintainer-email: contact@pyroscope.io
 License: Apache 2.0
 Project-URL: Documentation, https://pyroscope.io
 Project-URL: Bug Tracker, https://pyroscope.io
```

### Comparing `pyroscope-io-0.8.4/setup.cfg` & `pyroscope-io-0.8.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroscope-io
-version = 0.8.4
+version = 0.8.5
 description = Pyroscope Python integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pyroscope.io
 maintainer = Abid Omar
 maintainer_email = contact@pyroscope.io
 license = Apache 2.0
```

### Comparing `pyroscope-io-0.8.4/setup.py` & `pyroscope-io-0.8.5/setup.py`

 * *Files identical despite different names*

