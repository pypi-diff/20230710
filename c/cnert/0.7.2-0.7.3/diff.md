# Comparing `tmp/cnert-0.7.2.tar.gz` & `tmp/cnert-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.7.2.tar", max compression
+gzip compressed data, was "cnert-0.7.3.tar", max compression
```

## Comparing `cnert-0.7.2.tar` & `cnert-0.7.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.2/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.2/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.2/LICENSE.mit
--rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.2/README.md
--rw-r--r--   0        0        0     3150 2023-07-03 15:17:00.331762 cnert-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    26269 2023-07-03 15:17:00.361496 cnert-0.7.2/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.2/src/cnert/py.typed
--rw-r--r--   0        0        0     9312 1970-01-01 00:00:00.000000 cnert-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.7.3/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.7.3/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.7.3/LICENSE.mit
+-rw-r--r--   0        0        0     7748 2023-05-10 14:30:59.900805 cnert-0.7.3/README.md
+-rw-r--r--   0        0        0     3150 2023-07-10 07:20:22.974432 cnert-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0    26744 2023-07-10 07:20:23.003925 cnert-0.7.3/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.7.3/src/cnert/py.typed
+-rw-r--r--   0        0        0     9312 1970-01-01 00:00:00.000000 cnert-0.7.3/PKG-INFO
```

### Comparing `cnert-0.7.2/LICENSE.apache2` & `cnert-0.7.3/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.7.2/LICENSE.mit` & `cnert-0.7.3/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.7.2/README.md` & `cnert-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cnert-0.7.2/pyproject.toml` & `cnert-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.7.2"
+version = "0.7.3"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
```

### Comparing `cnert-0.7.2/src/cnert/__init__.py` & `cnert-0.7.3/src/cnert/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.x509.oid import ExtendedKeyUsageOID, NameOID
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
@@ -535,14 +535,32 @@
 
         Returns:
             An RSA private key.
         """
         return self.private_key.public_key()
 
     @property
+    def public_key_pem(self) -> bytes:
+        """
+        Examples:
+            >>> cert = CA().issue_cert()
+            >>> cert.public_key_pem
+            b'-----BEGIN PUBLIC KEY-----
+            ...
+
+
+        Returns:
+            PEM encoded serialized key in RSAPublicKey format.
+        """
+        return self.public_key.public_bytes(
+            serialization.Encoding.PEM,
+            format=serialization.PublicFormat.SubjectPublicKeyInfo,
+        )
+
+    @property
     def MD5(self) -> str:
         """
         Examples:
             >>> cert = cnert.CA().issue_cert()
             >>> cert.MD5
             'A03D37486DD47BE3E9C7EC1624073856'
```

### Comparing `cnert-0.7.2/PKG-INFO` & `cnert-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnert
-Version: 0.7.2
+Version: 0.7.3
 Summary: Cnert is trying to be a simple API for creating TLS Certificates testing purposes.
 Home-page: https://github.com/maartenq/cnert
 License: MIT
 Keywords: certificate,X.509,TLS,cryptography,testing
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 Requires-Python: >=3.9,<4.0
```

