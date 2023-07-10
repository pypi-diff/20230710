# Comparing `tmp/magic-admin-0.3.3.tar.gz` & `tmp/magic-admin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic-admin-0.3.3.tar", last modified: Tue May  2 19:03:50 2023, max compression
+gzip compressed data, was "dist/magic-admin-1.0.0.tar", last modified: Mon Jul 10 17:47:01 2023, max compression
```

## Comparing `magic-admin-0.3.3.tar` & `magic-admin-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.607137 magic-admin-0.3.3/
--rw-r--r--   0 ben        (501) staff       (20)     1081 2023-05-02 16:31:00.000000 magic-admin-0.3.3/LICENSE.txt
--rw-r--r--   0 ben        (501) staff       (20)     3712 2023-05-02 19:03:50.607211 magic-admin-0.3.3/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     3100 2023-05-02 16:31:00.000000 magic-admin-0.3.3/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.604067 magic-admin-0.3.3/magic_admin/
--rw-r--r--   0 ben        (501) staff       (20)      199 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)      449 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/config.py
--rw-r--r--   0 ben        (501) staff       (20)     2196 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/error.py
--rw-r--r--   0 ben        (501) staff       (20)     4550 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/http_client.py
--rw-r--r--   0 ben        (501) staff       (20)     1110 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/magic.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.606301 magic-admin-0.3.3/magic_admin/resources/
--rw-r--r--   0 ben        (501) staff       (20)      142 2023-05-02 16:36:19.000000 magic-admin-0.3.3/magic_admin/resources/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     1488 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/base.py
--rw-r--r--   0 ben        (501) staff       (20)     5230 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/token.py
--rw-r--r--   0 ben        (501) staff       (20)     1778 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/user.py
--rw-r--r--   0 ben        (501) staff       (20)      496 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/wallet.py
--rw-r--r--   0 ben        (501) staff       (20)      187 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/response.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.606949 magic-admin-0.3.3/magic_admin/utils/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)      745 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/did_token.py
--rw-r--r--   0 ben        (501) staff       (20)      371 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/http.py
--rw-r--r--   0 ben        (501) staff       (20)      199 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/time.py
--rw-r--r--   0 ben        (501) staff       (20)       18 2023-05-02 16:32:49.000000 magic-admin-0.3.3/magic_admin/version.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.605184 magic-admin-0.3.3/magic_admin.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     3712 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      680 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/not-zip-safe
--rw-r--r--   0 ben        (501) staff       (20)       35 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      106 2023-05-02 19:03:50.607457 magic-admin-0.3.3/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)     1696 2023-05-02 16:31:00.000000 magic-admin-0.3.3/setup.py
+drwxr-xr-x   0 ravibhankharia   (501) staff       (20)        0 2023-07-10 17:47:01.000000 magic-admin-1.0.0/
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     4581 2023-07-10 17:47:01.000000 magic-admin-1.0.0/PKG-INFO
+drwxr-xr-x   0 ravibhankharia   (501) staff       (20)        0 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin/
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     1495 2023-07-10 17:44:53.000000 magic-admin-1.0.0/magic_admin/magic.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      449 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/config.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)       18 2023-07-10 17:44:53.000000 magic-admin-1.0.0/magic_admin/version.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     2196 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/error.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     4550 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/http_client.py
+drwxr-xr-x   0 ravibhankharia   (501) staff       (20)        0 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin/resources/
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     1778 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/resources/user.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     5446 2023-07-10 17:44:53.000000 magic-admin-1.0.0/magic_admin/resources/token.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      142 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/resources/__init__.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     1488 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/resources/base.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      496 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/resources/wallet.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      199 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/__init__.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      187 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/response.py
+drwxr-xr-x   0 ravibhankharia   (501) staff       (20)        0 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin/utils/
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      199 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/utils/time.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      745 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/utils/did_token.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)        0 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/utils/__init__.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      371 2023-06-26 20:23:36.000000 magic-admin-1.0.0/magic_admin/utils/http.py
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     3100 2023-06-26 20:23:36.000000 magic-admin-1.0.0/README.md
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     1696 2023-06-26 20:23:36.000000 magic-admin-1.0.0/setup.py
+drwxr-xr-x   0 ravibhankharia   (501) staff       (20)        0 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin.egg-info/
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     4581 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin.egg-info/PKG-INFO
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)        1 2023-07-05 19:21:51.000000 magic-admin-1.0.0/magic_admin.egg-info/not-zip-safe
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      680 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)       35 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin.egg-info/requires.txt
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)       12 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin.egg-info/top_level.txt
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)        1 2023-07-10 17:47:01.000000 magic-admin-1.0.0/magic_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)      106 2023-07-10 17:47:01.000000 magic-admin-1.0.0/setup.cfg
+-rw-r--r--   0 ravibhankharia   (501) staff       (20)     1081 2023-06-26 20:23:36.000000 magic-admin-1.0.0/LICENSE.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `magic-admin-0.3.3/LICENSE.txt` & `magic-admin-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/PKG-INFO` & `magic-admin-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: magic-admin
-Version: 0.3.3
-Summary: Magic Python Library
-Home-page: https://magic.link
-Author: Magic
-Author-email: support@magic.link
-License: MIT
-Project-URL: Website, https://magic.link
-Keywords: magic python sdk
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Magic Admin Python SDK
 
 The Magic Admin Python SDK provides convenient ways for developers to interact with Magic API endpoints and an array of utilities to handle [DID Token](https://magic.link/docs/auth/introduction/decentralized-id).
 
 ## Table of Contents
 
 * [Documentation](#documentation)
```

### Comparing `magic-admin-0.3.3/magic_admin/error.py` & `magic-admin-1.0.0/magic_admin/error.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/magic_admin/http_client.py` & `magic-admin-1.0.0/magic_admin/http_client.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/magic_admin/resources/base.py` & `magic-admin-1.0.0/magic_admin/resources/base.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/magic_admin/resources/token.py` & `magic-admin-1.0.0/magic_admin/resources/token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 import json
 
 from eth_account.messages import defunct_hash_message
 from web3.auto import w3
 
+import magic_admin
 from magic_admin.error import DIDTokenExpired
 from magic_admin.error import DIDTokenInvalid
 from magic_admin.error import DIDTokenMalformed
 from magic_admin.resources.base import ResourceComponent
 from magic_admin.utils.did_token import parse_public_address_from_issuer
 from magic_admin.utils.time import apply_did_token_nbf_grace_period
 from magic_admin.utils.time import epoch_time_now
@@ -168,7 +169,12 @@
 
         if current_time_in_s < apply_did_token_nbf_grace_period(claim['nbf']):
             raise DIDTokenInvalid(
                 message='Given DID token cannot be used at this time. Please '
                 'check the "nbf" field and regenerate a new token with a suitable '
                 'value.',
             )
+
+        if claim['aud'] != magic_admin.client_id:
+            raise DIDTokenInvalid(
+                message='"aud" field does not match your client. Please check your secret key.',
+            )
```

### Comparing `magic-admin-0.3.3/magic_admin/resources/user.py` & `magic-admin-1.0.0/magic_admin/resources/user.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/magic_admin/utils/did_token.py` & `magic-admin-1.0.0/magic_admin/utils/did_token.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/magic_admin.egg-info/SOURCES.txt` & `magic-admin-1.0.0/magic_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.3/setup.py` & `magic-admin-1.0.0/setup.py`

 * *Files identical despite different names*

