# Comparing `tmp/syncari-sdk-1.3.7.tar.gz` & `tmp/syncari-sdk-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/syncari-sdk-1.3.7.tar", last modified: Tue May  9 19:34:30 2023, max compression
+gzip compressed data, was "syncari-sdk-1.3.8.tar", last modified: Mon Jul 10 03:33:59 2023, max compression
```

## Comparing `syncari-sdk-1.3.7.tar` & `syncari-sdk-1.3.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/
--rw-r--r--   0 vraman     (501) staff       (20)      373 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/PKG-INFO
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/__init__.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/models/
--rw-r--r--   0 vraman     (501) staff       (20)     2505 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/models/request.py
--rw-r--r--   0 vraman     (501) staff       (20)       64 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/models/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)     3935 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/models/core.py
--rw-r--r--   0 vraman     (501) staff       (20)     2273 2023-05-09 06:49:08.000000 syncari-sdk-1.3.7/syncari/models/schema.py
--rw-r--r--   0 vraman     (501) staff       (20)      699 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/logger.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/synapse/
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/synapse/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)    10308 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/synapse/abstract_synapse.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari/rest/
--rw-r--r--   0 vraman     (501) staff       (20)     3938 2023-05-09 18:36:03.000000 syncari-sdk-1.3.7/syncari/rest/client.py
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/syncari/rest/__init__.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/unit_tests/
--rw-r--r--   0 vraman     (501) staff       (20)     7319 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/unit_tests/test_mock_synapse.py
--rw-r--r--   0 vraman     (501) staff       (20)        0 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/unit_tests/__init__.py
--rw-r--r--   0 vraman     (501) staff       (20)     6299 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/unit_tests/test_response_validations.py
--rw-r--r--   0 vraman     (501) staff       (20)     2809 2023-05-09 18:36:58.000000 syncari-sdk-1.3.7/unit_tests/test_rest_client.py
--rw-r--r--   0 vraman     (501) staff       (20)       78 2023-03-23 20:00:03.000000 syncari-sdk-1.3.7/README.md
--rwxr-xr-x   0 vraman     (501) staff       (20)      562 2023-05-09 15:33:05.000000 syncari-sdk-1.3.7/setup.py
-drwxr-xr-x   0 vraman     (501) staff       (20)        0 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/
--rw-r--r--   0 vraman     (501) staff       (20)      373 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vraman     (501) staff       (20)      569 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vraman     (501) staff       (20)       47 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/requires.txt
--rw-r--r--   0 vraman     (501) staff       (20)       19 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/top_level.txt
--rw-r--r--   0 vraman     (501) staff       (20)        1 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/syncari_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vraman     (501) staff       (20)       38 2023-05-09 19:34:30.000000 syncari-sdk-1.3.7/setup.cfg
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.434896 syncari-sdk-1.3.8/
+-rw-r--r--   0 blesson    (501) staff       (20)      338 2023-07-10 03:33:59.434789 syncari-sdk-1.3.8/PKG-INFO
+-rw-r--r--   0 blesson    (501) staff       (20)       78 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/README.md
+-rw-r--r--   0 blesson    (501) staff       (20)       38 2023-07-10 03:33:59.434934 syncari-sdk-1.3.8/setup.cfg
+-rwxr-xr-x   0 blesson    (501) staff       (20)      562 2023-07-07 16:46:08.000000 syncari-sdk-1.3.8/setup.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.432085 syncari-sdk-1.3.8/syncari/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)      699 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/logger.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.432877 syncari-sdk-1.3.8/syncari/models/
+-rw-r--r--   0 blesson    (501) staff       (20)       64 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/models/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)     3969 2023-07-07 15:56:51.000000 syncari-sdk-1.3.8/syncari/models/core.py
+-rw-r--r--   0 blesson    (501) staff       (20)     2505 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/models/request.py
+-rw-r--r--   0 blesson    (501) staff       (20)     2273 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/models/schema.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.433100 syncari-sdk-1.3.8/syncari/rest/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/rest/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)     3938 2023-06-15 14:32:04.000000 syncari-sdk-1.3.8/syncari/rest/client.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.433409 syncari-sdk-1.3.8/syncari/synapse/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/synapse/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)    10308 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/synapse/abstract_synapse.py
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.433970 syncari-sdk-1.3.8/syncari_sdk.egg-info/
+-rw-r--r--   0 blesson    (501) staff       (20)      338 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 blesson    (501) staff       (20)      569 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 blesson    (501) staff       (20)        1 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 blesson    (501) staff       (20)       47 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/requires.txt
+-rw-r--r--   0 blesson    (501) staff       (20)       19 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.434527 syncari-sdk-1.3.8/unit_tests/
+-rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/unit_tests/__init__.py
+-rw-r--r--   0 blesson    (501) staff       (20)     7319 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/unit_tests/test_mock_synapse.py
+-rw-r--r--   0 blesson    (501) staff       (20)     6299 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/unit_tests/test_response_validations.py
+-rw-r--r--   0 blesson    (501) staff       (20)     2809 2023-06-15 14:32:04.000000 syncari-sdk-1.3.8/unit_tests/test_rest_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `syncari-sdk-1.3.7/syncari/models/request.py` & `syncari-sdk-1.3.8/syncari/models/request.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/syncari/models/core.py` & `syncari-sdk-1.3.8/syncari/models/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     name: str
     category: str
     metadata: UIMetadata
     supportedAuthTypes: List[AuthMetadata]
     configuredFields: Optional[List[AuthField]]
     disabledMessage: Optional[str]
     oauthInfo: Optional[dict[str, str]]
+    apiMaxCrudSize: Optional[int]
 
 class AuthConfig(BaseModel):
     """
         The authentication configuration for auth mechanism.
     """
     endpoint: Optional[str]
     userName: Optional[str]
```

### Comparing `syncari-sdk-1.3.7/syncari/models/schema.py` & `syncari-sdk-1.3.8/syncari/models/schema.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/syncari/logger.py` & `syncari-sdk-1.3.8/syncari/logger.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/syncari/synapse/abstract_synapse.py` & `syncari-sdk-1.3.8/syncari/synapse/abstract_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/syncari/rest/client.py` & `syncari-sdk-1.3.8/syncari/rest/client.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/unit_tests/test_mock_synapse.py` & `syncari-sdk-1.3.8/unit_tests/test_mock_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/unit_tests/test_response_validations.py` & `syncari-sdk-1.3.8/unit_tests/test_response_validations.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/unit_tests/test_rest_client.py` & `syncari-sdk-1.3.8/unit_tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.7/setup.py` & `syncari-sdk-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='syncari-sdk',
-    version='1.3.7',
+    version='1.3.8',
     description='Syncari Synapse Development Kit',
     author='Syncari',
     author_email='dev@syncari.com',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='TBD',
     packages=find_packages(exclude=('unittests')),
```

### Comparing `syncari-sdk-1.3.7/syncari_sdk.egg-info/SOURCES.txt` & `syncari-sdk-1.3.8/syncari_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

