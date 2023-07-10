# Comparing `tmp/cryptol-3.0.0.tar.gz` & `tmp/cryptol-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptol-3.0.0.tar", max compression
+gzip compressed data, was "cryptol-3.0.1.tar", max compression
```

## Comparing `cryptol-3.0.0.tar` & `cryptol-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2022-03-17 13:58:42.893837 cryptol-3.0.0/LICENSE
--rw-r--r--   0        0        0     6969 2023-06-22 14:12:12.001591 cryptol-3.0.0/README.md
--rw-r--r--   0        0        0     1242 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/__init__.py
--rw-r--r--   0        0        0    21302 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/bitvector.py
--rw-r--r--   0        0        0    12494 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/commands.py
--rw-r--r--   0        0        0    26865 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/connection.py
--rw-r--r--   0        0        0    18605 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/cryptoltypes.py
--rw-r--r--   0        0        0     4476 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/custom_fstring.py
--rw-r--r--   0        0        0      355 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/file_deps.py
--rw-r--r--   0        0        0      561 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/opaque.py
--rw-r--r--   0        0        0        0 2022-03-17 13:58:42.897837 cryptol-3.0.0/cryptol/py.typed
--rw-r--r--   0        0        0     3900 2022-05-18 13:09:19.916614 cryptol-3.0.0/cryptol/quoting.py
--rw-r--r--   0        0        0    12665 2023-06-22 14:12:12.001591 cryptol-3.0.0/cryptol/single_connection.py
--rw-r--r--   0        0        0     3178 2023-06-22 14:12:12.005591 cryptol-3.0.0/cryptol/solver.py
--rw-r--r--   0        0        0    19875 2023-06-22 14:12:12.005591 cryptol-3.0.0/cryptol/synchronous.py
--rw-r--r--   0        0        0      228 2022-03-17 13:58:42.897837 cryptol-3.0.0/mypy.ini
--rw-r--r--   0        0        0      584 2023-06-26 17:51:42.962079 cryptol-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 cryptol-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-11 21:07:40.690001 cryptol-3.0.1/LICENSE
+-rw-r--r--   0        0        0     6969 2023-04-11 21:07:40.690240 cryptol-3.0.1/README.md
+-rw-r--r--   0        0        0     1242 2023-04-11 21:07:40.691768 cryptol-3.0.1/cryptol/__init__.py
+-rw-r--r--   0        0        0    21322 2023-07-06 18:21:37.983493 cryptol-3.0.1/cryptol/bitvector.py
+-rw-r--r--   0        0        0    12827 2023-07-06 19:36:02.338078 cryptol-3.0.1/cryptol/commands.py
+-rw-r--r--   0        0        0    27251 2023-07-06 19:38:17.555027 cryptol-3.0.1/cryptol/connection.py
+-rw-r--r--   0        0        0    18605 2023-05-08 18:36:02.272059 cryptol-3.0.1/cryptol/cryptoltypes.py
+-rw-r--r--   0        0        0     4476 2023-04-11 21:07:40.698051 cryptol-3.0.1/cryptol/custom_fstring.py
+-rw-r--r--   0        0        0      355 2023-07-06 18:21:37.985704 cryptol-3.0.1/cryptol/file_deps.py
+-rw-r--r--   0        0        0      561 2023-04-11 21:07:40.699860 cryptol-3.0.1/cryptol/opaque.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:07:40.700029 cryptol-3.0.1/cryptol/py.typed
+-rw-r--r--   0        0        0     4115 2023-07-06 18:21:47.085220 cryptol-3.0.1/cryptol/quoting.py
+-rw-r--r--   0        0        0    12886 2023-07-06 19:32:21.926342 cryptol-3.0.1/cryptol/single_connection.py
+-rw-r--r--   0        0        0     3178 2023-04-11 21:07:40.703748 cryptol-3.0.1/cryptol/solver.py
+-rw-r--r--   0        0        0    21146 2023-07-10 17:06:58.583113 cryptol-3.0.1/cryptol/synchronous.py
+-rw-r--r--   0        0        0      228 2023-04-20 18:17:17.417167 cryptol-3.0.1/mypy.ini
+-rw-r--r--   0        0        0      584 2023-07-10 19:36:36.853447 cryptol-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 cryptol-3.0.1/PKG-INFO
```

### Comparing `cryptol-3.0.0/LICENSE` & `cryptol-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/README.md` & `cryptol-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/cryptol/__init__.py` & `cryptol-3.0.1/cryptol/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/cryptol/bitvector.py` & `cryptol-3.0.1/cryptol/bitvector.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
     def to_int(self) -> int:
         """Return the unsigned integer the ``BV`` represents (equivalent to ``self.value()``)."""
         return self.__value
 
     def to_signed_int(self) -> int:
         """Return the signed (i.e., two's complement) integer the ``BV`` represents."""
-        if not self.msb():
+        if self.__size == 0 or not self.msb():
             n = self.__value
         else:
             n = 0 - ((2 ** self.__size) - self.__value)
         return n
 
     def msb(self) -> bool:
         """Returns ``True`` if the most significant bit is 1, else returns ``False``."""
```

### Comparing `cryptol-3.0.0/cryptol/commands.py` & `cryptol-3.0.1/cryptol/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,26 @@
             timeout=timeout
         )
 
     def process_result(self, res : Any) -> Any:
         return res
 
 
+class CryptolVersion(argo.Command):
+    def __init__(self, connection : HasProtocolState, timeout: Optional[float]) -> None:
+        super(CryptolVersion, self).__init__(
+            'version',
+            {},
+            connection,
+            timeout=timeout)
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
+
 class CryptolReset(argo.Notification):
     def __init__(self, connection : HasProtocolState) -> None:
         super(CryptolReset, self).__init__(
             'clear state',
             {'state to clear': connection.protocol_state()},
             connection
         )
```

### Comparing `cryptol-3.0.0/cryptol/connection.py` & `cryptol-3.0.1/cryptol/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,22 @@
         """Return the name of the currently-focused module.
 
         :param timeout: Optional timeout for this request (in seconds)."""
         timeout = timeout if timeout is not None else self.timeout
         self.most_recent_result = CryptolFocusedModule(self, timeout)
         return self.most_recent_result
 
+    def version(self, *, timeout:Optional[float] = None) -> argo.Command:
+        """Returns version information about the Cryptol server.
+
+        :param timeout: Optional timeout for this request (in seconds)."""
+        timeout = timeout if timeout is not None else self.timeout
+        self.most_recent_result = CryptolVersion(self, timeout)
+        return self.most_recent_result
+
     def reset(self) -> None:
         """Resets the connection, causing its unique state on the server to be freed (if applicable).
 
         After a reset a connection may be treated as if it were a fresh connection with the server if desired."""
         CryptolReset(self)
         self.most_recent_result = None
```

### Comparing `cryptol-3.0.0/cryptol/cryptoltypes.py` & `cryptol-3.0.1/cryptol/cryptoltypes.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/cryptol/custom_fstring.py` & `cryptol-3.0.1/cryptol/custom_fstring.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/cryptol/opaque.py` & `cryptol-3.0.1/cryptol/opaque.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/cryptol/quoting.py` & `cryptol-3.0.1/cryptol/quoting.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 
 def to_cryptol_str(val : Union[CryptolValue, str, CryptolJSON]) -> str:
     """Converts a ``CryptolValue``, string literal, or ``CryptolJSON`` into
        a string of Cryptol syntax."""
     if isinstance(val, bool):
         return 'True' if val else 'False'
     elif isinstance(val, tuple):
+        if len(val) == 1:
+            raise TypeError("Unable to convert 1-tuple to Cryptol syntax: " + str(val))
         return '(' + ', '.join(to_cryptol_str(x) for x in val) + ')'
     elif isinstance(val, dict):
         return '{' + ', '.join(f'{k} = {to_cryptol_str(v)}' for k,v in val.items()) + '}'
     elif isinstance(val, int):
         return str(val)
     elif isinstance(val, list):
         return '[' + ', '.join(to_cryptol_str(x) for x in val) + ']'
     elif isinstance(val, BV):
-        if val.size() % 4 == 0:
+        if val.size() > 0 and val.size() % 4 == 0:
             return val.hex()
         else:
             return f'({val.to_signed_int()} : [{val.size()}])'
     elif isinstance(val, OpaqueValue):
         return str(val)
     elif isinstance(val, str):
-        return f'"{val}"'
+        chars = list(val.encode('latin-1'))
+        return f'({to_cryptol_str(chars)} : [{len(chars)}][8])'
     elif hasattr(val, '__to_cryptol_str__'):
         return parenthesize(val.__to_cryptol_str__())
     else:
         raise TypeError("Unable to convert value to Cryptol syntax: " + str(val))
 
 def to_cryptol_str_customf(s : str, *, frames : int = 0,
                                        filename : str = "<cry_f>") -> str:
```

### Comparing `cryptol-3.0.0/cryptol/single_connection.py` & `cryptol-3.0.1/cryptol/single_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing_extensions import Literal
 
 from .custom_fstring import *
 from .quoting import *
 from .solver import OfflineSmtQuery, Solver, OnlineSolver, OfflineSolver, Z3
 from .connection import CryptolValue, CheckReport
 from . import synchronous
-from .synchronous import Qed, Safe, Counterexample, Satisfiable, Unsatisfiable
+from .synchronous import Qed, Safe, Counterexample, Satisfiable, Unsatisfiable, CryptolVersionInfo
 from . import cryptoltypes
 
 
 __designated_connection = None  # type: Optional[synchronous.CryptolSyncConnection]
 
 def __get_designated_connection() -> synchronous.CryptolSyncConnection:
     global __designated_connection
@@ -232,14 +232,18 @@
     The result is a subset of the list returned by `names`."""
     return __get_designated_connection().property_names(timeout=timeout)
 
 def focused_module(*, timeout:Optional[float] = None) -> cryptoltypes.CryptolModuleInfo:
     """Returns the name and other information about the currently-focused module."""
     return __get_designated_connection().focused_module(timeout=timeout)
 
+def version(*, timeout:Optional[float] = None) -> CryptolVersionInfo:
+    """Returns version information about the Cryptol server."""
+    return __get_designated_connection().version(timeout=timeout)
+
 def reset() -> None:
     """Resets the connection, causing its unique state on the server to be freed (if applicable).
     After a reset a connection may be treated as if it were a fresh connection with the server if desired."""
     __get_designated_connection().reset()
 
 def reset_server() -> None:
     """Resets the Cryptol server, clearing all states."""
```

### Comparing `cryptol-3.0.0/cryptol/solver.py` & `cryptol-3.0.1/cryptol/solver.py`

 * *Files identical despite different names*

### Comparing `cryptol-3.0.0/cryptol/synchronous.py` & `cryptol-3.0.1/cryptol/synchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,33 @@
     are falsy, i.e. evaluate to `False` in an 'if 'or 'while' statement.
     """
     def __bool__(self) -> Literal[False]:
         return False
     def __nonzero__(self) -> Literal[False]:
         return False
 
+@dataclass
+class CryptolVersionInfo:
+    """
+    Class containing version information about the Cryptol server.
+
+    :param rpc_version: The cryptol-remote-api version string.
+    :param version: The Cryptol version string.
+    :param commit_hash: The string of the git commit hash during the build of Cryptol.
+    :param commit_branch: The string of the git commit branch during the build of Cryptol.
+    :param commit_dirty: True iff non-committed files were present during the build of Cryptol.
+    :param ffi_enabled: True iff the FFI is enabled.
+    """
+    rpc_version: str
+    version: str
+    commit_hash: str
+    commit_branch: str
+    commit_dirty: bool
+    ffi_enabled: bool 
+
 
 def connect(command : Optional[str]=None,
             *,
             cryptol_path : Optional[str] = None,
             url : Optional[str] = None,
             reset_server : bool = False,
             verify : Union[bool, str] = True,
@@ -373,14 +392,26 @@
         else:
             raise ValueError("Result of `property_names()` is not a list: " + str(res))
 
     def focused_module(self, *, timeout:Optional[float] = None) -> cryptoltypes.CryptolModuleInfo:
         """Returns the name and other information about the currently-focused module."""
         return cryptoltypes.to_cryptol_module_info(self.connection.focused_module(timeout=timeout).result())
 
+    def version(self, *, timeout:Optional[float] = None) -> CryptolVersionInfo:
+        """Returns version information about the Cryptol server."""
+        res = self.connection.version(timeout=timeout).result()
+        return CryptolVersionInfo(
+                rpc_version   = res['RPC server version'],
+                version       = res['version'],
+                commit_hash   = res['commit hash'],
+                commit_branch = res['commit branch'],
+                commit_dirty  = res['commit dirty'],
+                ffi_enabled   = res['FFI enabled']
+                )
+
     def reset(self) -> None:
         """Resets the connection, causing its unique state on the server to be freed (if applicable).
         After a reset a connection may be treated as if it were a fresh connection with the server if desired."""
         self.connection.reset()
 
     def reset_server(self) -> None:
         """Resets the Cryptol server, clearing all states."""
```

### Comparing `cryptol-3.0.0/pyproject.toml` & `cryptol-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cryptol"
-version = "3.0.0"
+version = "3.0.1"
 readme = "README.md"
 keywords = ["cryptography", "verification"]
 description = "Cryptol client for the Cryptol 2.13 RPC server"
 authors = ["Galois, Inc. <cryptol-team@galois.com>"]
 
 license = "BSD License"
 include = [
```

### Comparing `cryptol-3.0.0/PKG-INFO` & `cryptol-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptol
-Version: 3.0.0
+Version: 3.0.1
 Summary: Cryptol client for the Cryptol 2.13 RPC server
 License: BSD License
 Keywords: cryptography,verification
 Author: Galois, Inc.
 Author-email: cryptol-team@galois.com
 Requires-Python: >=3.8.0,<4
 Classifier: License :: Other/Proprietary License
```

