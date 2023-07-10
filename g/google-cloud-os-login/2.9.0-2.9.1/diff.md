# Comparing `tmp/google-cloud-os-login-2.9.0.tar.gz` & `tmp/google-cloud-os-login-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-os-login-2.9.0.tar", last modified: Wed Jan 11 15:59:09 2023, max compression
+gzip compressed data, was "google-cloud-os-login-2.9.1.tar", last modified: Mon Jan 23 16:10:04 2023, max compression
```

## Comparing `google-cloud-os-login-2.9.0.tar` & `google-cloud-os-login-2.9.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.267224 google-cloud-os-login-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4587 2023-01-11 15:59:09.267224 google-cloud-os-login-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3669 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.255222 google-cloud-os-login-2.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.255222 google-cloud-os-login-2.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.259222 google-cloud-os-login-2.9.0/google/cloud/oslogin/
--rw-rw-r--   0 root         (0)     1003     1590 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.259222 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/
--rw-rw-r--   0 root         (0)     1003     1445 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.259222 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/
--rw-rw-r--   0 root         (0)     1003      758 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/__init__.py
--rw-rw-r--   0 root         (0)     1003      243 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       88 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.259222 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/types/
--rw-rw-r--   0 root         (0)     1003      750 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3875 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/types/common.py
--rw-rw-r--   0 root         (0)     1003     2393 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.259222 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    42611 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    50660 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11389 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18989 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19335 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/types/
--rw-rw-r--   0 root         (0)     1003     1180 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7438 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/types/oslogin.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/
--rw-r--r--   0 root         (0)     1003     4587 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1623 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-11 15:59:09.000000 google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-11 15:59:09.267224 google-cloud-os-login-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2976 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.263223 google-cloud-os-login-2.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-11 15:59:09.267224 google-cloud-os-login-2.9.0/tests/unit/gapic/oslogin_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/tests/unit/gapic/oslogin_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   114011 2023-01-11 15:55:49.000000 google-cloud-os-login-2.9.0/tests/unit/gapic/oslogin_v1/test_os_login_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.783951 google-cloud-os-login-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4587 2023-01-23 16:10:04.783951 google-cloud-os-login-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3669 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.771953 google-cloud-os-login-2.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.771953 google-cloud-os-login-2.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.775953 google-cloud-os-login-2.9.1/google/cloud/oslogin/
+-rw-rw-r--   0 root         (0)     1003     1590 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.775953 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/
+-rw-rw-r--   0 root         (0)     1003     1445 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.775953 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/
+-rw-rw-r--   0 root         (0)     1003      758 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/__init__.py
+-rw-rw-r--   0 root         (0)     1003      243 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       88 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.775953 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/types/
+-rw-rw-r--   0 root         (0)     1003      750 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3875 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/types/common.py
+-rw-rw-r--   0 root         (0)     1003     2393 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    42611 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    50686 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11389 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18989 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19335 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1180 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7438 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/types/oslogin.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/
+-rw-r--r--   0 root         (0)     1003     4587 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1623 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:10:04.000000 google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:10:04.783951 google-cloud-os-login-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.779952 google-cloud-os-login-2.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:10:04.783951 google-cloud-os-login-2.9.1/tests/unit/gapic/oslogin_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/tests/unit/gapic/oslogin_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   114011 2023-01-23 16:06:35.000000 google-cloud-os-login-2.9.1/tests/unit/gapic/oslogin_v1/test_os_login_service.py
```

### Comparing `google-cloud-os-login-2.9.0/LICENSE` & `google-cloud-os-login-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/MANIFEST.in` & `google-cloud-os-login-2.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/PKG-INFO` & `google-cloud-os-login-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-os-login
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Os Login API client library
 Home-page: https://github.com/googleapis/python-oslogin
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-os-login-2.9.0/README.rst` & `google-cloud-os-login-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin/gapic_version.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/types/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/common/types/common.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/common/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/gapic_metadata.json` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/gapic_version.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.9.0"  # {x-release-please-version}
+__version__ = "2.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/async_client.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/client.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,15 +1209,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "OsLoginServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/base.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/grpc.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/services/os_login_service/transports/grpc_asyncio.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/services/os_login_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/types/__init__.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google/cloud/oslogin_v1/types/oslogin.py` & `google-cloud-os-login-2.9.1/google/cloud/oslogin_v1/types/oslogin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/PKG-INFO` & `google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-os-login
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Cloud Os Login API client library
 Home-page: https://github.com/googleapis/python-oslogin
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-os-login-2.9.0/google_cloud_os_login.egg-info/SOURCES.txt` & `google-cloud-os-login-2.9.1/google_cloud_os_login.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/setup.py` & `google-cloud-os-login-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/tests/__init__.py` & `google-cloud-os-login-2.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/tests/unit/__init__.py` & `google-cloud-os-login-2.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/tests/unit/gapic/__init__.py` & `google-cloud-os-login-2.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/tests/unit/gapic/oslogin_v1/__init__.py` & `google-cloud-os-login-2.9.1/tests/unit/gapic/oslogin_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-os-login-2.9.0/tests/unit/gapic/oslogin_v1/test_os_login_service.py` & `google-cloud-os-login-2.9.1/tests/unit/gapic/oslogin_v1/test_os_login_service.py`

 * *Files identical despite different names*

