# Comparing `tmp/moby_distribution-0.5.4.tar.gz` & `tmp/moby_distribution-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moby_distribution-0.5.4.tar", max compression
+gzip compressed data, was "moby_distribution-0.5.5.tar", max compression
```

## Comparing `moby_distribution-0.5.4.tar` & `moby_distribution-0.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/LICENSE
--rw-r--r--   0        0        0     7006 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/README.md
--rw-r--r--   0        0        0      895 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/__init__.py
--rw-r--r--   0        0        0     5441 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/auth.py
--rw-r--r--   0        0        0     6351 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/client.py
--rw-r--r--   0        0        0      917 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/exceptions.py
--rw-r--r--   0        0        0      574 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/resources/__init__.py
--rw-r--r--   0        0        0    10776 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/resources/blobs.py
--rw-r--r--   0        0        0    13969 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/resources/image.py
--rw-r--r--   0        0        0     4645 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/resources/manifests.py
--rw-r--r--   0        0        0      967 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/resources/tags.py
--rw-r--r--   0        0        0     3868 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/registry/utils.py
--rw-r--r--   0        0        0        0 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/spec/__init__.py
--rw-r--r--   0        0        0     1140 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/spec/auth.py
--rw-r--r--   0        0        0     1070 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/spec/base.py
--rw-r--r--   0        0        0     2688 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/spec/endpoint.py
--rw-r--r--   0        0        0     3757 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/spec/image_json.py
--rw-r--r--   0        0        0     4594 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/moby_distribution/spec/manifest.py
--rw-r--r--   0        0        0      914 2023-03-28 03:57:03.122250 moby_distribution-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     7976 1970-01-01 00:00:00.000000 moby_distribution-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 09:07:08.233722 moby_distribution-0.5.5/LICENSE
+-rw-r--r--   0        0        0     7006 2023-07-10 09:07:08.233722 moby_distribution-0.5.5/README.md
+-rw-r--r--   0        0        0      895 2023-07-10 09:07:08.233722 moby_distribution-0.5.5/moby_distribution/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:07:08.233722 moby_distribution-0.5.5/moby_distribution/registry/__init__.py
+-rw-r--r--   0        0        0     5582 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/auth.py
+-rw-r--r--   0        0        0     6351 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/client.py
+-rw-r--r--   0        0        0      917 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/exceptions.py
+-rw-r--r--   0        0        0      574 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/resources/__init__.py
+-rw-r--r--   0        0        0    10776 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/resources/blobs.py
+-rw-r--r--   0        0        0    13969 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/resources/image.py
+-rw-r--r--   0        0        0     4645 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/resources/manifests.py
+-rw-r--r--   0        0        0      967 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/resources/tags.py
+-rw-r--r--   0        0        0     3868 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/registry/utils.py
+-rw-r--r--   0        0        0        0 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/spec/__init__.py
+-rw-r--r--   0        0        0     1140 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/spec/auth.py
+-rw-r--r--   0        0        0     1070 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/spec/base.py
+-rw-r--r--   0        0        0     2688 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/spec/endpoint.py
+-rw-r--r--   0        0        0     3757 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/spec/image_json.py
+-rw-r--r--   0        0        0     4594 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/moby_distribution/spec/manifest.py
+-rw-r--r--   0        0        0      914 2023-07-10 09:07:08.237722 moby_distribution-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     7976 1970-01-01 00:00:00.000000 moby_distribution-0.5.5/PKG-INFO
```

### Comparing `moby_distribution-0.5.4/LICENSE` & `moby_distribution-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/README.md` & `moby_distribution-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/__init__.py` & `moby_distribution-0.5.5/moby_distribution/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from moby_distribution.registry.resources.image import ImageRef, LayerRef
 from moby_distribution.registry.resources.manifests import ManifestRef
 from moby_distribution.registry.resources.tags import Tags
 from moby_distribution.spec.endpoint import OFFICIAL_ENDPOINT, APIEndpoint
 from moby_distribution.spec.image_json import ImageJSON
 from moby_distribution.spec.manifest import ManifestSchema1, ManifestSchema2, OCIManifestSchema1
 
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 __ALL__ = [
     "DockerRegistryV2Client",
     "Blob",
     "ManifestRef",
     "Tags",
     "APIEndpoint",
     "ManifestSchema1",
```

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/auth.py` & `moby_distribution-0.5.5/moby_distribution/registry/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import requests
 from www_authenticate import parse
 
 from moby_distribution.registry.exceptions import AuthFailed
 from moby_distribution.spec.auth import TokenResponse
 
+AUTH_TIMEOUT = 60 * 3
 logger = logging.getLogger(__name__)
 
 
 class AuthorizationProvider:
     def provide(self) -> str:
         """Provide the 'Authorization' used in HTTP Headers
 
@@ -124,15 +125,16 @@
         headers = {}
         if username and password:
             auth = base64.b64encode(f"{username}:{password}".encode()).decode()
             headers["Authorization"] = f"Basic {auth}"
         elif any([username, password]) and not all([username, password]):
             logger.warning("请同时提供 username 和 password!")
 
-        resp = requests.get(self.backend, headers=headers, params=params)
+        logger.info("sending authentication request to authorization service<%s>", self.backend)
+        resp = requests.get(self.backend, headers=headers, params=params, timeout=AUTH_TIMEOUT)
         if resp.status_code != 200:
             raise AuthFailed(
                 message="用户凭证校验失败, 请检查用户信息和操作权限",
                 status_code=resp.status_code,
                 response=resp,
             )
         return TokenAuthorizationProvider(TokenResponse(**resp.json()))
```

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/client.py` & `moby_distribution-0.5.5/moby_distribution/registry/client.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/exceptions.py` & `moby_distribution-0.5.5/moby_distribution/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/resources/__init__.py` & `moby_distribution-0.5.5/moby_distribution/registry/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/resources/blobs.py` & `moby_distribution-0.5.5/moby_distribution/registry/resources/blobs.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/resources/image.py` & `moby_distribution-0.5.5/moby_distribution/registry/resources/image.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/resources/manifests.py` & `moby_distribution-0.5.5/moby_distribution/registry/resources/manifests.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/resources/tags.py` & `moby_distribution-0.5.5/moby_distribution/registry/resources/tags.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/registry/utils.py` & `moby_distribution-0.5.5/moby_distribution/registry/utils.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/spec/auth.py` & `moby_distribution-0.5.5/moby_distribution/spec/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/spec/base.py` & `moby_distribution-0.5.5/moby_distribution/spec/base.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/spec/endpoint.py` & `moby_distribution-0.5.5/moby_distribution/spec/endpoint.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/spec/image_json.py` & `moby_distribution-0.5.5/moby_distribution/spec/image_json.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/moby_distribution/spec/manifest.py` & `moby_distribution-0.5.5/moby_distribution/spec/manifest.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.5.4/pyproject.toml` & `moby_distribution-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moby-distribution"
-version = "0.5.4"
+version = "0.5.5"
 description = "Yet another moby(docker) distribution implement by python."
 authors = ["shabbywu <shabbywu@qq.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/distribution"
 homepage = "https://github.com/shabbywu/distribution"
```

### Comparing `moby_distribution-0.5.4/PKG-INFO` & `moby_distribution-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moby-distribution
-Version: 0.5.4
+Version: 0.5.5
 Summary: Yet another moby(docker) distribution implement by python.
 Home-page: https://github.com/shabbywu/distribution
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

