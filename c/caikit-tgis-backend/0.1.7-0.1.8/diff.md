# Comparing `tmp/caikit_tgis_backend-0.1.7.tar.gz` & `tmp/caikit_tgis_backend-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit_tgis_backend-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit_tgis_backend-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit_tgis_backend-0.1.7.tar` & `caikit_tgis_backend-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       65 2023-06-22 16:30:19.008058 caikit_tgis_backend-0.1.7/.coveragerc
--rw-r--r--   0        0        0      676 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      105 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/dependabot.yml
--rw-r--r--   0        0        0     1280 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1144 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      183 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.gitignore
--rw-r--r--   0        0        0      318 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.isort.cfg
--rw-r--r--   0        0        0      440 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       24 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.prettierignore
--rw-r--r--   0        0        0       12 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.prettierrc.yaml
--rw-r--r--   0        0        0    21406 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.pylintrc
--rw-r--r--   0        0        0       78 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/.whitesource
--rw-r--r--   0        0        0      362 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/CODEOWNERS
--rw-r--r--   0        0        0     7269 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/LICENSE
--rw-r--r--   0        0        0      138 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/README.md
--rw-r--r--   0        0        0      152 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/SECURITY.md
--rw-r--r--   0        0        0      723 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/__init__.py
--rw-r--r--   0        0        0     5727 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/generation.proto
--rw-r--r--   0        0        0    15375 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/managed_tgis_subprocess.py
--rw-r--r--   0        0        0      840 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/protobufs/__init__.py
--rw-r--r--   0        0        0    13426 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/protobufs/generation_pb2.py
--rw-r--r--   0        0        0     5685 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/protobufs/generation_pb2_grpc.py
--rw-r--r--   0        0        0     9861 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/caikit_tgis_backend/tgis_backend.py
--rw-r--r--   0        0        0      169 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/code-of-conduct.md
--rw-r--r--   0        0        0      656 2023-06-22 16:30:22.200118 caikit_tgis_backend-0.1.7/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/scripts/fmt.sh
--rwxr-xr-x   0        0        0      393 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/scripts/gen_tgis_protos.sh
--rw-r--r--   0        0        0       33 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/setup_requirements.txt
--rw-r--r--   0        0        0        0 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      342 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0    12193 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/tests/test_tgis_backend.py
--rw-r--r--   0        0        0     9004 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/tests/tgis_mock.py
--rw-r--r--   0        0        0     1209 2023-06-22 16:30:19.012058 caikit_tgis_backend-0.1.7/tox.ini
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 caikit_tgis_backend-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.coveragerc
+-rw-r--r--   0        0        0      676 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      105 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1280 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1144 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      183 2023-07-10 17:28:20.528057 caikit_tgis_backend-0.1.8/.gitignore
+-rw-r--r--   0        0        0      318 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/.isort.cfg
+-rw-r--r--   0        0        0      440 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       24 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/.prettierignore
+-rw-r--r--   0        0        0       12 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/.prettierrc.yaml
+-rw-r--r--   0        0        0    21406 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/.pylintrc
+-rw-r--r--   0        0        0       78 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/.whitesource
+-rw-r--r--   0        0        0      362 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/CODEOWNERS
+-rw-r--r--   0        0        0     7269 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/LICENSE
+-rw-r--r--   0        0        0      138 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/README.md
+-rw-r--r--   0        0        0      152 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/SECURITY.md
+-rw-r--r--   0        0        0      723 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/__init__.py
+-rw-r--r--   0        0        0     5727 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/generation.proto
+-rw-r--r--   0        0        0    15375 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/managed_tgis_subprocess.py
+-rw-r--r--   0        0        0      840 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/protobufs/__init__.py
+-rw-r--r--   0        0        0    13426 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/protobufs/generation_pb2.py
+-rw-r--r--   0        0        0     5685 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/protobufs/generation_pb2_grpc.py
+-rw-r--r--   0        0        0     9861 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/caikit_tgis_backend/tgis_backend.py
+-rw-r--r--   0        0        0      169 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/code-of-conduct.md
+-rw-r--r--   0        0        0      656 2023-07-10 17:28:23.672090 caikit_tgis_backend-0.1.8/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/scripts/fmt.sh
+-rwxr-xr-x   0        0        0      393 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/scripts/gen_tgis_protos.sh
+-rw-r--r--   0        0        0       33 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/setup_requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      342 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0    12193 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/tests/test_tgis_backend.py
+-rw-r--r--   0        0        0     9004 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/tests/tgis_mock.py
+-rw-r--r--   0        0        0     1209 2023-07-10 17:28:20.532057 caikit_tgis_backend-0.1.8/tox.ini
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 caikit_tgis_backend-0.1.8/PKG-INFO
```

### Comparing `caikit_tgis_backend-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit_tgis_backend-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit_tgis_backend-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/.github/ISSUE_TEMPLATE/user_story.md` & `caikit_tgis_backend-0.1.8/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/.github/workflows/build-library.yml` & `caikit_tgis_backend-0.1.8/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/.github/workflows/lint-code.yml` & `caikit_tgis_backend-0.1.8/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/.github/workflows/publish-library.yml` & `caikit_tgis_backend-0.1.8/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/.pylintrc` & `caikit_tgis_backend-0.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/CONTRIBUTING.md` & `caikit_tgis_backend-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/LICENSE` & `caikit_tgis_backend-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/__init__.py` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/generation.proto` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/generation.proto`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/managed_tgis_subprocess.py` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/managed_tgis_subprocess.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/protobufs/__init__.py` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/protobufs/generation_pb2.py` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/protobufs/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/protobufs/generation_pb2_grpc.py` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/protobufs/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/caikit_tgis_backend/tgis_backend.py` & `caikit_tgis_backend-0.1.8/caikit_tgis_backend/tgis_backend.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/pyproject.toml` & `caikit_tgis_backend-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit-tgis-backend"
 # Not the actual current version: overwritten by CI
-version = "0.1.7"
+version = "0.1.8"
 description = "Caikit module backend for models run in TGIS"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
-    "caikit>=0.2.0,<0.10.0", # Core abstractions
+    "caikit>=0.2.0,<0.11.0", # Core abstractions
     "grpcio>=1.35.0,<2.0", # Client calls to TGIS
     "requests>=2.28.2,<3", # Health check calls to TGIS
 ]
 
 [project.urls]
 Source = "https://github.com/caikit/caikit-tgis-backend"
```

### Comparing `caikit_tgis_backend-0.1.7/scripts/fmt.sh` & `caikit_tgis_backend-0.1.8/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/tests/test_tgis_backend.py` & `caikit_tgis_backend-0.1.8/tests/test_tgis_backend.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/tests/tgis_mock.py` & `caikit_tgis_backend-0.1.8/tests/tgis_mock.py`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/tox.ini` & `caikit_tgis_backend-0.1.8/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit_tgis_backend-0.1.7/PKG-INFO` & `caikit_tgis_backend-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: caikit-tgis-backend
-Version: 0.1.7
+Version: 0.1.8
 Summary: Caikit module backend for models run in TGIS
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: caikit>=0.2.0,<0.10.0
+Requires-Dist: caikit>=0.2.0,<0.11.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: requests>=2.28.2,<3
 Project-URL: Source, https://github.com/caikit/caikit-tgis-backend
 
 ## Caikit Text Generation Inference Service (TGIS) Backend
 
 This project provides a Caikit module backend that manages models run in TGIS
```

