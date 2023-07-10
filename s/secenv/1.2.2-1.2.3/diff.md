# Comparing `tmp/secenv-1.2.2.tar.gz` & `tmp/secenv-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secenv-1.2.2.tar", last modified: Wed May  3 16:17:52 2023, max compression
+gzip compressed data, was "secenv-1.2.3.tar", last modified: Mon Jul 10 09:00:23 2023, max compression
```

## Comparing `secenv-1.2.2.tar` & `secenv-1.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:17:52.825157 secenv-1.2.2/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-03 16:17:16.000000 secenv-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    50212 2023-05-03 16:17:52.825157 secenv-1.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8953 2023-05-03 16:17:16.000000 secenv-1.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-03 16:17:17.000000 secenv-1.2.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:17:52.821158 secenv-1.2.2/secenv/
--rw-rw-rw-   0 root         (0) root         (0)    11962 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3750 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:17:52.821158 secenv-1.2.2/secenv/contexts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/contexts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/contexts/aws_assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:17:52.821158 secenv-1.2.2/secenv/stores/
--rw-rw-rw-   0 root         (0) root         (0)     4446 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/aws.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/azure.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/bitwarden.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/env.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/gcp.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/pass.py
--rw-rw-rw-   0 root         (0) root         (0)     2733 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/scaleway.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/stores/vault.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-05-03 16:17:16.000000 secenv-1.2.2/secenv/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:17:52.821158 secenv-1.2.2/secenv.egg-info/
--rw-r--r--   0 root         (0) root         (0)    50212 2023-05-03 16:17:52.000000 secenv-1.2.2/secenv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-05-03 16:17:52.000000 secenv-1.2.2/secenv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:17:52.000000 secenv-1.2.2/secenv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-03 16:17:52.000000 secenv-1.2.2/secenv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-03 16:17:52.000000 secenv-1.2.2/secenv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 16:17:52.000000 secenv-1.2.2/secenv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 16:17:52.825157 secenv-1.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-03 16:17:16.000000 secenv-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:17:52.825157 secenv-1.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5623 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_config_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_context_output.py
--rw-rw-rw-   0 root         (0) root         (0)     5754 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_fill_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_gen_context.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_list_contexts.py
--rw-rw-rw-   0 root         (0) root         (0)    10980 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-03 16:17:16.000000 secenv-1.2.2/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.015214 secenv-1.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-10 08:59:43.000000 secenv-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-07-10 09:00:23.015214 secenv-1.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8953 2023-07-10 08:59:43.000000 secenv-1.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-07-10 08:59:44.000000 secenv-1.2.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.011214 secenv-1.2.3/secenv/
+-rw-rw-rw-   0 root         (0) root         (0)    11962 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3750 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.011214 secenv-1.2.3/secenv/contexts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/contexts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/contexts/aws_assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.015214 secenv-1.2.3/secenv/stores/
+-rw-rw-rw-   0 root         (0) root         (0)     4446 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/aws.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/azure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/bitwarden.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/pass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2701 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/scaleway.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/stores/vault.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-10 08:59:43.000000 secenv-1.2.3/secenv/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.011214 secenv-1.2.3/secenv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    50212 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-07-10 09:00:23.000000 secenv-1.2.3/secenv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-10 09:00:22.000000 secenv-1.2.3/secenv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 09:00:23.015214 secenv-1.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-10 08:59:43.000000 secenv-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:00:23.015214 secenv-1.2.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5623 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_config_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_context_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     5754 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_fill_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_gen_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_list_contexts.py
+-rw-rw-rw-   0 root         (0) root         (0)    10980 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-07-10 08:59:43.000000 secenv-1.2.3/tests/test_utils.py
```

### Comparing `secenv-1.2.2/LICENSE` & `secenv-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/PKG-INFO` & `secenv-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.2.2
+Version: 1.2.3
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.2.2/README.md` & `secenv-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/pyproject.toml` & `secenv-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "secenv"
-version = "1.2.2"
+version = "1.2.3"
 description = "An utility tool to list, read and fill secrets from multiple stores."
 readme = "README.md"
 authors = [{ name = "Keltio Labs", email = "labs@keltio.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `secenv-1.2.2/secenv/__init__.py` & `secenv-1.2.3/secenv/__init__.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/context.py` & `secenv-1.2.3/secenv/context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/contexts/aws_assume_role.py` & `secenv-1.2.3/secenv/contexts/aws_assume_role.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/__init__.py` & `secenv-1.2.3/secenv/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/aws.py` & `secenv-1.2.3/secenv/stores/aws.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/azure.py` & `secenv-1.2.3/secenv/stores/azure.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/bitwarden.py` & `secenv-1.2.3/secenv/stores/bitwarden.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/env.py` & `secenv-1.2.3/secenv/stores/env.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/gcp.py` & `secenv-1.2.3/secenv/stores/gcp.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/pass.py` & `secenv-1.2.3/secenv/stores/pass.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/stores/scaleway.py` & `secenv-1.2.3/secenv/stores/scaleway.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,15 @@
         elif generate:
             secret_value = generate_secret(generate)
         else:
             secret_value = ask_secret(self.name, secret)
 
         try:
             uid = self._name_to_uid(secret)
-        except Exception:
-            # except SecretNotFoundError:
+        except SecretNotFoundError:
             ret = self._post(
                 "secrets", {"name": secret, "project_id": self.project_id, "tags": []}
             )
             uid = json.loads(ret)["id"]
 
         url = f"secrets/{uid}/versions"
         data = {"data": base64.b64encode(secret_value.encode()).decode()}
```

### Comparing `secenv-1.2.2/secenv/stores/vault.py` & `secenv-1.2.3/secenv/stores/vault.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv/utils.py` & `secenv-1.2.3/secenv/utils.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/secenv.egg-info/PKG-INFO` & `secenv-1.2.3/secenv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secenv
-Version: 1.2.2
+Version: 1.2.3
 Summary: An utility tool to list, read and fill secrets from multiple stores.
 Author-email: Keltio Labs <labs@keltio.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `secenv-1.2.2/secenv.egg-info/SOURCES.txt` & `secenv-1.2.3/secenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/tests/test_config_file.py` & `secenv-1.2.3/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/tests/test_context_output.py` & `secenv-1.2.3/tests/test_context_output.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/tests/test_fill_secrets.py` & `secenv-1.2.3/tests/test_fill_secrets.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/tests/test_gen_context.py` & `secenv-1.2.3/tests/test_gen_context.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/tests/test_stores.py` & `secenv-1.2.3/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `secenv-1.2.2/tests/test_utils.py` & `secenv-1.2.3/tests/test_utils.py`

 * *Files identical despite different names*

