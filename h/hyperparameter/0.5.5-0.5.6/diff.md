# Comparing `tmp/hyperparameter-0.5.5.tar.gz` & `tmp/hyperparameter-0.5.6.tar.gz`

## Comparing `hyperparameter-0.5.5.tar` & `hyperparameter-0.5.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 hyperparameter-0.5.5/Cargo.toml
--rw-r--r--   0     1001      123      834 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      126 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0     1001      123      595 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      706 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/workflows/codecov.yml
--rw-r--r--   0     1001      123      845 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/workflows/mkdocs.yml
--rw-r--r--   0     1001      123     1262 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      123     2001 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.gitignore
--rw-r--r--   0     1001      123      356 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     5202 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    25260 2023-07-06 11:54:56.000000 hyperparameter-0.5.5/Cargo.lock
--rw-r--r--   0     1001      123    11356 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/LICENSE
--rw-r--r--   0     1001      123     3027 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/README.md
--rw-r--r--   0     1001      123     2871 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/README.zh.md
--rw-r--r--   0     1001      123     2846 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/examples/optimization.md
--rw-r--r--   0     1001      123     2868 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/examples/optimization.zh.md
--rw-r--r--   0     1001      123     3027 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/index.md
--rw-r--r--   0     1001      123     2871 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/index.zh.md
--rw-r--r--   0     1001      123     3000 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/quick_start.md
--rw-r--r--   0     1001      123     3000 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/quick_start.zh.md
--rw-r--r--   0     1001      123       48 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/reference.md
--rw-r--r--   0     1001      123      110 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/requirements.txt
--rw-r--r--   0     1001      123     6738 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/docs/structured_parameter.md
--rw-r--r--   0     1001      123      337 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/application/README.md
--rw-r--r--   0     1001      123      789 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/application/app.py
--rw-r--r--   0     1001      123       46 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/application/cfg.json
--rw-r--r--   0     1001      123     4733 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/automl_optuna_mnist/automl_mnist.py
--rw-r--r--   0     1001      123     2737 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/cpp/cxx_test.cc
--rw-r--r--   0     1001      123      436 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/cpp/cxx_test.py
--rw-r--r--   0     1001      123      237 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/cpp/cxx_test.sh
--rw-r--r--   0     1001      123      152 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/README.md
--rw-r--r--   0     1001      123     5625 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/main.py
--rw-r--r--   0     1001      123     5899 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/main_with_hp.py
--rw-r--r--   0     1001      123     6202 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/main_with_hp_with_mlflow.py
--rw-r--r--   0     1001      123       18 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/mnist/requirements.txt
--rw-r--r--   0     1001      123     2846 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/README.md
--rw-r--r--   0     1001      123      230 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/example.py
--rw-r--r--   0     1001      123      527 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/example_hp.py
--rw-r--r--   0     1001      123      727 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/optuna/example_hp_nested.py
--rw-r--r--   0     1001      123     1650 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/README.md
--rw-r--r--   0     1001      123      581 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/example_1.py
--rw-r--r--   0     1001      123      934 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/example_2.py
--rw-r--r--   0     1001      123     1059 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/example_mlflow.py
--rw-r--r--   0     1001      123      867 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/sparse_lr/model.py
--rw-r--r--   0     1001      123     1631 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/examples/storage.rs
--rw-r--r--   0     1001      123        0 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hparam/__init__.py
--rw-r--r--   0     1001      123     3710 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hparam/__main__.py
--rw-r--r--   0     1001      123      320 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/__init__.py
--rw-r--r--   0     1001      123    17127 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/api.py
--rw-r--r--   0     1001      123     7715 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/hyperparameter.h
--rw-r--r--   0     1001      123      828 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/loader.py
--rw-r--r--   0     1001      123     4202 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/storage.py
--rw-r--r--   0     1001      123     2223 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/hyperparameter/tune.py
--rw-r--r--   0     1001      123     1249 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/mkdocs.yml
--rw-r--r--   0     1001      123      941 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/pyproject.toml
--rwxr-xr-x   0     1001      123      814 2023-07-06 11:54:36.000000 hyperparameter-0.5.5/run-maturin-action.sh
--rw-r--r--   0     1001      123     6151 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/entry.rs
--rw-r--r--   0     1001      123     6583 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/ext.rs
--rw-r--r--   0     1001      123     2038 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/ffi.rs
--rw-r--r--   0     1001      123      106 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/lib.rs
--rw-r--r--   0     1001      123     8129 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/storage.rs
--rw-r--r--   0     1001      123     4528 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/src/xxh.rs
--rwxr-xr-x   0     1001      123    40754 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/a.out
--rw-r--r--   0     1001      123      912 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_auto_param.py
--rw-r--r--   0     1001      123     3769 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_param_scope.py
--rw-r--r--   0     1001      123      697 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_param_scope_thread.py
--rw-r--r--   0     1001      123     2991 2023-07-06 11:53:55.000000 hyperparameter-0.5.5/tests/test_rust_backend.py
--rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 hyperparameter-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 hyperparameter-0.5.6/Cargo.toml
+-rw-r--r--   0     1001      123      834 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      126 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0     1001      123      595 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      706 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.github/workflows/codecov.yml
+-rw-r--r--   0     1001      123      845 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.github/workflows/mkdocs.yml
+-rw-r--r--   0     1001      123     1262 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      123     2001 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.gitignore
+-rw-r--r--   0     1001      123      356 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5202 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    25263 2023-07-10 02:49:56.000000 hyperparameter-0.5.6/Cargo.lock
+-rw-r--r--   0     1001      123    11356 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/LICENSE
+-rw-r--r--   0     1001      123     3027 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/README.md
+-rw-r--r--   0     1001      123     2871 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/README.zh.md
+-rw-r--r--   0     1001      123      320 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/build.rs
+-rw-r--r--   0     1001      123     2846 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/examples/optimization.md
+-rw-r--r--   0     1001      123     2868 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/examples/optimization.zh.md
+-rw-r--r--   0     1001      123     3027 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/index.md
+-rw-r--r--   0     1001      123     2871 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/index.zh.md
+-rw-r--r--   0     1001      123     3000 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/quick_start.md
+-rw-r--r--   0     1001      123     3000 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/quick_start.zh.md
+-rw-r--r--   0     1001      123       48 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/reference.md
+-rw-r--r--   0     1001      123      110 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/requirements.txt
+-rw-r--r--   0     1001      123     6738 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/docs/structured_parameter.md
+-rw-r--r--   0     1001      123      337 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/application/README.md
+-rw-r--r--   0     1001      123      789 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/application/app.py
+-rw-r--r--   0     1001      123       46 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/application/cfg.json
+-rw-r--r--   0     1001      123     4733 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/automl_optuna_mnist/automl_mnist.py
+-rw-r--r--   0     1001      123     2737 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/cpp/cxx_test.cc
+-rw-r--r--   0     1001      123      436 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/cpp/cxx_test.py
+-rw-r--r--   0     1001      123      237 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/cpp/cxx_test.sh
+-rw-r--r--   0     1001      123      152 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/mnist/README.md
+-rw-r--r--   0     1001      123     5625 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/mnist/main.py
+-rw-r--r--   0     1001      123     5899 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/mnist/main_with_hp.py
+-rw-r--r--   0     1001      123     6202 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/mnist/main_with_hp_with_mlflow.py
+-rw-r--r--   0     1001      123       18 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/mnist/requirements.txt
+-rw-r--r--   0     1001      123     2846 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/optuna/README.md
+-rw-r--r--   0     1001      123      230 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/optuna/example.py
+-rw-r--r--   0     1001      123      527 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/optuna/example_hp.py
+-rw-r--r--   0     1001      123      727 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/optuna/example_hp_nested.py
+-rw-r--r--   0     1001      123     1650 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/sparse_lr/README.md
+-rw-r--r--   0     1001      123      581 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/sparse_lr/example_1.py
+-rw-r--r--   0     1001      123      934 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/sparse_lr/example_2.py
+-rw-r--r--   0     1001      123     1059 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/sparse_lr/example_mlflow.py
+-rw-r--r--   0     1001      123      867 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/sparse_lr/model.py
+-rw-r--r--   0     1001      123     1631 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/examples/storage.rs
+-rw-r--r--   0     1001      123        0 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hparam/__init__.py
+-rw-r--r--   0     1001      123     3710 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hparam/__main__.py
+-rw-r--r--   0     1001      123      320 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hyperparameter/__init__.py
+-rw-r--r--   0     1001      123    17127 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hyperparameter/api.py
+-rw-r--r--   0     1001      123     7715 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hyperparameter/hyperparameter.h
+-rw-r--r--   0     1001      123      828 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hyperparameter/loader.py
+-rw-r--r--   0     1001      123     4202 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hyperparameter/storage.py
+-rw-r--r--   0     1001      123     2223 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/hyperparameter/tune.py
+-rw-r--r--   0     1001      123     1249 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/mkdocs.yml
+-rw-r--r--   0     1001      123      941 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/pyproject.toml
+-rw-r--r--   0     1001      123     6151 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/src/entry.rs
+-rw-r--r--   0     1001      123     6583 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/src/ext.rs
+-rw-r--r--   0     1001      123     2038 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/src/ffi.rs
+-rw-r--r--   0     1001      123      106 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/src/lib.rs
+-rw-r--r--   0     1001      123     8129 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/src/storage.rs
+-rw-r--r--   0     1001      123     4528 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/src/xxh.rs
+-rwxr-xr-x   0     1001      123    40754 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/tests/a.out
+-rw-r--r--   0     1001      123      912 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/tests/test_auto_param.py
+-rw-r--r--   0     1001      123     3769 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/tests/test_param_scope.py
+-rw-r--r--   0     1001      123      697 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/tests/test_param_scope_thread.py
+-rw-r--r--   0     1001      123     2991 2023-07-10 02:48:56.000000 hyperparameter-0.5.6/tests/test_rust_backend.py
+-rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 hyperparameter-0.5.6/PKG-INFO
```

### Comparing `hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md` & `hyperparameter-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md` & `hyperparameter-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/.github/workflows/codecov.yml` & `hyperparameter-0.5.6/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/.github/workflows/mkdocs.yml` & `hyperparameter-0.5.6/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/.github/workflows/python-publish.yml` & `hyperparameter-0.5.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/.gitignore` & `hyperparameter-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/CODE_OF_CONDUCT.md` & `hyperparameter-0.5.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/Cargo.lock` & `hyperparameter-0.5.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -102,39 +102,39 @@
 checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.98"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd99fdd577aa186de8a711654cfabc63a7b2024e8d392f87153af428deaa4f71"
+checksum = "e928d50d5858b744d1ea920b790641129c347a770d1530c3a85b77705a5ee031"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.98"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9204071a5d00b4da785ebe22f863cffd365f3357b6dba4070177bfe2e75f160"
+checksum = "5966a5a87b6e9bb342f5fab7170a93c77096efe199872afffc4b477cfeb86957"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.98"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59f6a87b1e7f773ec602b9af278e06da3d1b46c98bc0ee09751c2477d97d3b0b"
+checksum = "81b2dab6991c7ab1572fea8cb049db819b1aeea1e2dac74c0869f244d9f21a7c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "darling"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d706e75d87e35569db781a9b5e2416cff1236a47ed380831f959382ccd5f858"
@@ -270,17 +270,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
  "hermit-abi",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
@@ -415,15 +415,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
@@ -435,17 +435,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -621,27 +621,27 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.166"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01b7404f9d441d3ad40e6a636a7782c377d2abdbe4fa2440e2edcc2f4f10db8"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.166"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5dd83d6dde2b6b2d466e14d9d1acce8816dedee94f735eac6395808b3483c6d6"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
@@ -751,17 +751,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.23"
+version = "2.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
+checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -843,15 +843,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -865,15 +865,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.23",
+ "syn 2.0.25",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
```

### Comparing `hyperparameter-0.5.5/LICENSE` & `hyperparameter-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/README.md` & `hyperparameter-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/README.zh.md` & `hyperparameter-0.5.6/README.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/examples/optimization.md` & `hyperparameter-0.5.6/docs/examples/optimization.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/examples/optimization.zh.md` & `hyperparameter-0.5.6/docs/examples/optimization.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/index.md` & `hyperparameter-0.5.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/index.zh.md` & `hyperparameter-0.5.6/docs/index.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/quick_start.md` & `hyperparameter-0.5.6/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/quick_start.zh.md` & `hyperparameter-0.5.6/docs/quick_start.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/docs/structured_parameter.md` & `hyperparameter-0.5.6/docs/structured_parameter.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/application/app.py` & `hyperparameter-0.5.6/examples/application/app.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/automl_optuna_mnist/automl_mnist.py` & `hyperparameter-0.5.6/examples/automl_optuna_mnist/automl_mnist.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/cpp/cxx_test.cc` & `hyperparameter-0.5.6/examples/cpp/cxx_test.cc`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/mnist/main.py` & `hyperparameter-0.5.6/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/mnist/main_with_hp.py` & `hyperparameter-0.5.6/examples/mnist/main_with_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/mnist/main_with_hp_with_mlflow.py` & `hyperparameter-0.5.6/examples/mnist/main_with_hp_with_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/optuna/README.md` & `hyperparameter-0.5.6/examples/optuna/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/optuna/example_hp.py` & `hyperparameter-0.5.6/examples/optuna/example_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/optuna/example_hp_nested.py` & `hyperparameter-0.5.6/examples/optuna/example_hp_nested.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/sparse_lr/README.md` & `hyperparameter-0.5.6/examples/sparse_lr/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/sparse_lr/example_1.py` & `hyperparameter-0.5.6/examples/sparse_lr/example_1.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/sparse_lr/example_2.py` & `hyperparameter-0.5.6/examples/sparse_lr/example_2.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/sparse_lr/example_mlflow.py` & `hyperparameter-0.5.6/examples/sparse_lr/example_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/sparse_lr/model.py` & `hyperparameter-0.5.6/examples/sparse_lr/model.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/examples/storage.rs` & `hyperparameter-0.5.6/examples/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/hparam/__main__.py` & `hyperparameter-0.5.6/hparam/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/hyperparameter/api.py` & `hyperparameter-0.5.6/hyperparameter/api.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/hyperparameter/hyperparameter.h` & `hyperparameter-0.5.6/hyperparameter/hyperparameter.h`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/hyperparameter/loader.py` & `hyperparameter-0.5.6/hyperparameter/loader.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/hyperparameter/storage.py` & `hyperparameter-0.5.6/hyperparameter/storage.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/hyperparameter/tune.py` & `hyperparameter-0.5.6/hyperparameter/tune.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/mkdocs.yml` & `hyperparameter-0.5.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/pyproject.toml` & `hyperparameter-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "hyperparameter"
-version = "0.5.5"
+version = "0.5.6"
 authors = [{ name = "Reiase", email = "reiase@gmail.com" }]
 description = "A hyper-parameter library for researchers, data scientists and machine learning engineers."
 requires-python = ">=3.7"
 readme = "README.md"
 license = { text = "Apache License Version 2.0" }
 
 [tool.maturin]
```

### Comparing `hyperparameter-0.5.5/src/entry.rs` & `hyperparameter-0.5.6/src/entry.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/src/ext.rs` & `hyperparameter-0.5.6/src/ext.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/src/ffi.rs` & `hyperparameter-0.5.6/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/src/storage.rs` & `hyperparameter-0.5.6/src/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/src/xxh.rs` & `hyperparameter-0.5.6/src/xxh.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/tests/a.out` & `hyperparameter-0.5.6/tests/a.out`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/tests/test_auto_param.py` & `hyperparameter-0.5.6/tests/test_auto_param.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/tests/test_param_scope.py` & `hyperparameter-0.5.6/tests/test_param_scope.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/tests/test_param_scope_thread.py` & `hyperparameter-0.5.6/tests/test_param_scope_thread.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/tests/test_rust_backend.py` & `hyperparameter-0.5.6/tests/test_rust_backend.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.5/PKG-INFO` & `hyperparameter-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter
-Version: 0.5.5
+Version: 0.5.6
 License-File: LICENSE
 Summary: A hyper-parameter library for researchers, data scientists and machine learning engineers.
 Author-email: Reiase <reiase@gmail.com>
 License: Apache License Version 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

