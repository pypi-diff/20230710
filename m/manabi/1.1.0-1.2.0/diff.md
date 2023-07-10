# Comparing `tmp/manabi-1.1.0.tar.gz` & `tmp/manabi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manabi-1.1.0.tar", max compression
+gzip compressed data, was "manabi-1.2.0.tar", max compression
```

## Comparing `manabi-1.1.0.tar` & `manabi-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2716 2023-07-03 13:09:03.092631 manabi-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-31 17:06:59.165102 manabi-1.1.0/LICENSE
--rw-r--r--   0        0        0     5260 2023-06-19 16:02:10.707837 manabi-1.1.0/README.md
--rw-r--r--   0        0        0     1372 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/__init__.py
--rw-r--r--   0        0        0     4300 2023-06-16 14:47:50.897983 manabi-1.1.0/manabi/auth.py
--rw-r--r--   0        0        0     4277 2023-06-21 14:54:48.018204 manabi-1.1.0/manabi/filesystem.py
--rw-r--r--   0        0        0    10021 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/lock.py
--rw-r--r--   0        0        0     2681 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/log.py
--rw-r--r--   0        0        0      273 2023-06-15 12:40:23.020940 manabi-1.1.0/manabi/mypy_fix.py
--rw-r--r--   0        0        0     4401 2023-06-16 14:27:26.837088 manabi-1.1.0/manabi/token.py
--rw-r--r--   0        0        0      524 2023-06-21 14:54:48.024870 manabi-1.1.0/manabi/type_alias.py
--rw-r--r--   0        0        0     2763 2023-06-19 16:02:10.707837 manabi-1.1.0/manabi/util.py
--rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/__init__.py
--rw-r--r--   0        0        0      165 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/apps.py
--rw-r--r--   0        0        0      532 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/migrations/__init__.py
--rw-r--r--   0        0        0      200 2023-05-31 17:07:00.845155 manabi-1.1.0/manabi_django/manabi_migrations/models.py
--rw-r--r--   0        0        0     2428 2023-07-03 13:06:49.898682 manabi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6510 1970-01-01 00:00:00.000000 manabi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3043 2023-07-10 11:49:52.293035 manabi-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-07-10 11:49:52.293035 manabi-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5507 2023-07-10 11:49:52.293035 manabi-1.2.0/README.md
+-rw-r--r--   0        0        0     1372 2023-07-10 11:49:52.293035 manabi-1.2.0/manabi/__init__.py
+-rw-r--r--   0        0        0     4300 2023-07-10 11:49:52.293035 manabi-1.2.0/manabi/auth.py
+-rw-r--r--   0        0        0     5080 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/filesystem.py
+-rw-r--r--   0        0        0    10021 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/lock.py
+-rw-r--r--   0        0        0     2681 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/log.py
+-rw-r--r--   0        0        0      273 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/mypy_fix.py
+-rw-r--r--   0        0        0     5263 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/token.py
+-rw-r--r--   0        0        0      521 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/type_alias.py
+-rw-r--r--   0        0        0     2763 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi/util.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi_django/manabi_migrations/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi_django/manabi_migrations/apps.py
+-rw-r--r--   0        0        0      532 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi_django/manabi_migrations/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi_django/manabi_migrations/migrations/__init__.py
+-rw-r--r--   0        0        0      200 2023-07-10 11:49:52.297035 manabi-1.2.0/manabi_django/manabi_migrations/models.py
+-rw-r--r--   0        0        0     2428 2023-07-10 11:49:52.297035 manabi-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6757 1970-01-01 00:00:00.000000 manabi-1.2.0/PKG-INFO
```

### Comparing `manabi-1.1.0/CHANGELOG.md` & `manabi-1.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+### Feature
+* Add post-write-hook/callback ([`80cbf38`](https://github.com/projectcaluma/manabi/commit/80cbf387a775e1a417e3a44bcfb884e926d5bf08))
+
+### Fix
+* **token:** Handle errors from msgpack by creating a invalid token ([`81a5ccf`](https://github.com/projectcaluma/manabi/commit/81a5ccff740112947c8fb67b97d17d6e640eedfb))
+
 ## v1.1.0 (2023-07-03)
 
 ### Feature
 * Add pre_write_callback and hook/callback approve write ([`08b6a6f`](https://github.com/projectcaluma/manabi/commit/08b6a6fe2ea76e006de17cc0a7f0be35f2b1e1f6))
 
 ## v1.0.0 (2023-06-20)
```

### Comparing `manabi-1.1.0/LICENSE` & `manabi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/README.md` & `manabi-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -37,22 +37,21 @@
 - Manabi retrieves the token from the request URI, checks its validity, and
   proceeds to open the document if the token is verified.
 - The token is updated and stored as a cookie within Word/LO for future reference.
 - Due to the ephemeral WebDAV lock, Word/LO must regularly contact Manabi to
   refresh the lock. Consequently, we leverage this mechanism to also refresh the
   token.
 
-**pre_write_hook**: We provide an optional pre-write-hook feature that enhances
-the API's capabilities by adding a versioning system. The hook is invoked with
-the token as an argument **prior** to the document being saved using WebDAV-PUT.
-The API has the ability to verify this token and subsequently create a new
-version of the document. Once the hook operation is successfully completed,
-Manabi takes over and saves the document.
-
-A post-write-hook is not implemented, if you need one, please open an issue.
+**cb_hook_config**: We provide an optional write-hooks/callbacks feature that
+enhances the API's capabilities by adding a versioning system. The pre-write-
+hook/callback is invoked with the token as an argument **prior** to the document
+being saved using WebDAV-PUT. The API has the ability to verify this token and
+subsequently create a new version of the document. Once the hook operation is
+successfully completed, Manabi takes over and saves the document. Manabi then
+continues and invokes the post-write-hook/callback.
 
 ## Install
 
 Make sure libsodium exists on the system, for example execute:
 
 ```bash
 apk add --no-cache libsodium
@@ -98,20 +97,28 @@
 The time from the token being generated till it has to be refreshed the first
 time, we recommend 1 minues: `60`. In case tokens leak, for example via cache on
 a computer, tokens should be expired by the time an adversary gets them.
 
 ```python
 from manabi import ManabiDAVApp
 
+# All hooks and callbacks are optional
+cb_hook_config = CallbackHookConfig(
+    pre_write_hook=_pre_write_hook,
+    pre_write_callback=_pre_write_callback,
+    post_write_hook=_post_write_hook,
+    post_write_callback=_post_write_callback,
+)
+
 postgres_dsn = "dbname=manabi user=manabi host=localhost password=manabi"
 config = {
     "mount_path": "/dav",
     "lock_storage": ManabiDbLockStorage(refresh, postgres_dsn),
     "provider_mapping": {
-        "/": ManabiProvider(settings.MEDIA_ROOT, pre_write_hook="http://127.0.0.1/hook"),
+        "/": ManabiProvider(settings.MEDIA_ROOT, cb_hook_config=cb_hook_config),
     },
     "middleware_stack": [
         WsgiDavDebugFilter,
         ErrorPrinter,
         ManabiAuthenticator,
         WsgiDavDirBrowser,
         RequestResolver,
```

### Comparing `manabi-1.1.0/manabi/__init__.py` & `manabi-1.2.0/manabi/__init__.py`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/manabi/auth.py` & `manabi-1.2.0/manabi/auth.py`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/manabi/lock.py` & `manabi-1.2.0/manabi/lock.py`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/manabi/log.py` & `manabi-1.2.0/manabi/log.py`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/manabi/token.py` & `manabi-1.2.0/manabi/token.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 from attr import Factory, dataclass
 from branca import Branca  # type: ignore
 
 from .type_alias import OptionalProp, PropType
 from .util import cattrib, from_string
 
 
+class DecodingError(Exception):
+    pass
+
+
+class EncodingError(Exception):
+    pass
+
+
 def now() -> int:
     return calendar.timegm(datetime.utcnow().timetuple())
 
 
 @dataclass
 class TTL:
     initial: int = cattrib(int)
@@ -100,15 +108,16 @@
         branca = Branca(key.data)
         try:
             timestamp = branca.timestamp(ciphertext)
         except (struct.error, ValueError):
             return cls(key, None, None)
         try:
             token_path, token_payload = _decode(branca, ciphertext)
-        except RuntimeError:
+        except DecodingError:
+            # Handle decoding errors by creating a invalid token
             return cls(key, None, timestamp)
         return cls(key, token_path, token_payload, timestamp, ciphertext)
 
     def check(self, ttl: Optional[int] = None) -> State:
         if self.path is None or self.timestamp is None:
             return State.invalid
         if ttl is not None:
@@ -131,24 +140,44 @@
 def _encode(
     key: bytes,
     path: str,
     payload: OptionalProp = None,
     now: Optional[int] = None,
 ) -> str:
     f = Branca(key)
-    p = umsgpack.packb((path.encode("UTF-8"), payload))
-    ciphertext = f.encode(p, now)
+    try:
+        path_bytes = path.encode("UTF-8")
+    except Exception as e:
+        raise EncodingError("Could not UTF-8 encode the path") from e
+    try:
+        p = umsgpack.packb((path_bytes, payload))
+    except Exception as e:
+        raise EncodingError("Could not msg-pack the payload") from e
+    try:
+        ciphertext = f.encode(p, now)
+    except Exception as e:
+        raise EncodingError("Could not encode the branca token") from e
     return ciphertext
 
 
 def _decode(
     key: Union[bytes, Branca],
     ciphertext: str,
     ttl=None,
 ) -> Tuple[Path, PropType]:
     if isinstance(key, Branca):
         f = key
     else:
         f = Branca(key)
-    tpb, token_payload = umsgpack.unpackb(f.decode(ciphertext, ttl))
-    token_path = tpb.decode("UTF-8")
+    try:
+        token = f.decode(ciphertext, ttl)
+    except Exception as e:
+        raise DecodingError("Could not decode the branca token") from e
+    try:
+        tpb, token_payload = umsgpack.unpackb(token)
+    except Exception as e:
+        raise DecodingError("Could not msg-unpack the payload") from e
+    try:
+        token_path = tpb.decode("UTF-8")
+    except Exception as e:
+        raise DecodingError("Could not UTF-8 decode the path") from e
     return Path(token_path), token_payload
```

### Comparing `manabi-1.1.0/manabi/type_alias.py` & `manabi-1.2.0/manabi/type_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
     str,
     None,
     Dict[str, "PropType"],
     Tuple["PropType"],
     bool,
 ]
 OptionalProp = Optional[PropType]
-PreWriteType = Callable[["Token"], bool]
+WriteType = Callable[["Token"], bool]
```

### Comparing `manabi-1.1.0/manabi/util.py` & `manabi-1.2.0/manabi/util.py`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/manabi_django/manabi_migrations/migrations/0001_initial.py` & `manabi-1.2.0/manabi_django/manabi_migrations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `manabi-1.1.0/pyproject.toml` & `manabi-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manabi"
-version = "1.1.0"
+version = "1.2.0"
 description = "Provide WebDAV access for documents."
 homepage = "https://github.com/projectcaluma/manabi"
 repository = "https://github.com/projectcaluma/manabi"
 authors = ["Adfinis AG"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
```

### Comparing `manabi-1.1.0/PKG-INFO` & `manabi-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manabi
-Version: 1.1.0
+Version: 1.2.0
 Summary: Provide WebDAV access for documents.
 Home-page: https://github.com/projectcaluma/manabi
 License: AGPL-3.0-or-later
 Author: Adfinis AG
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -66,22 +66,21 @@
 - Manabi retrieves the token from the request URI, checks its validity, and
   proceeds to open the document if the token is verified.
 - The token is updated and stored as a cookie within Word/LO for future reference.
 - Due to the ephemeral WebDAV lock, Word/LO must regularly contact Manabi to
   refresh the lock. Consequently, we leverage this mechanism to also refresh the
   token.
 
-**pre_write_hook**: We provide an optional pre-write-hook feature that enhances
-the API's capabilities by adding a versioning system. The hook is invoked with
-the token as an argument **prior** to the document being saved using WebDAV-PUT.
-The API has the ability to verify this token and subsequently create a new
-version of the document. Once the hook operation is successfully completed,
-Manabi takes over and saves the document.
-
-A post-write-hook is not implemented, if you need one, please open an issue.
+**cb_hook_config**: We provide an optional write-hooks/callbacks feature that
+enhances the API's capabilities by adding a versioning system. The pre-write-
+hook/callback is invoked with the token as an argument **prior** to the document
+being saved using WebDAV-PUT. The API has the ability to verify this token and
+subsequently create a new version of the document. Once the hook operation is
+successfully completed, Manabi takes over and saves the document. Manabi then
+continues and invokes the post-write-hook/callback.
 
 ## Install
 
 Make sure libsodium exists on the system, for example execute:
 
 ```bash
 apk add --no-cache libsodium
@@ -127,20 +126,28 @@
 The time from the token being generated till it has to be refreshed the first
 time, we recommend 1 minues: `60`. In case tokens leak, for example via cache on
 a computer, tokens should be expired by the time an adversary gets them.
 
 ```python
 from manabi import ManabiDAVApp
 
+# All hooks and callbacks are optional
+cb_hook_config = CallbackHookConfig(
+    pre_write_hook=_pre_write_hook,
+    pre_write_callback=_pre_write_callback,
+    post_write_hook=_post_write_hook,
+    post_write_callback=_post_write_callback,
+)
+
 postgres_dsn = "dbname=manabi user=manabi host=localhost password=manabi"
 config = {
     "mount_path": "/dav",
     "lock_storage": ManabiDbLockStorage(refresh, postgres_dsn),
     "provider_mapping": {
-        "/": ManabiProvider(settings.MEDIA_ROOT, pre_write_hook="http://127.0.0.1/hook"),
+        "/": ManabiProvider(settings.MEDIA_ROOT, cb_hook_config=cb_hook_config),
     },
     "middleware_stack": [
         WsgiDavDebugFilter,
         ErrorPrinter,
         ManabiAuthenticator,
         WsgiDavDirBrowser,
         RequestResolver,
```

