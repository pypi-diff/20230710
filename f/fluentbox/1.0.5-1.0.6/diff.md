# Comparing `tmp/fluentbox-1.0.5.tar.gz` & `tmp/fluentbox-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluentbox-1.0.5.tar", last modified: Thu Mar 23 19:33:30 2023, max compression
+gzip compressed data, was "fluentbox-1.0.6.tar", last modified: Mon Jul 10 10:02:32 2023, max compression
```

## Comparing `fluentbox-1.0.5.tar` & `fluentbox-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-03-23 19:33:30.292039 fluentbox-1.0.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-03-23 19:33:30.292039 fluentbox-1.0.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)       90 2023-01-27 09:33:21.000000 fluentbox-1.0.5/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-03-23 19:33:30.292039 fluentbox-1.0.5/setup.cfg
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-03-23 19:33:30.288038 fluentbox-1.0.5/src/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-03-23 19:33:30.292039 fluentbox-1.0.5/src/fluentbox/
--rw-rw-r--   0 alex      (1000) alex      (1000)      239 2023-01-27 09:52:59.000000 fluentbox-1.0.5/src/fluentbox/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14225 2023-03-23 19:32:26.000000 fluentbox-1.0.5/src/fluentbox/fluentbox.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-03-23 19:33:30.292039 fluentbox-1.0.5/src/fluentbox.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-03-23 19:33:30.000000 fluentbox-1.0.5/src/fluentbox.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      249 2023-03-23 19:33:30.000000 fluentbox-1.0.5/src/fluentbox.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-03-23 19:33:30.000000 fluentbox-1.0.5/src/fluentbox.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       10 2023-03-23 19:33:30.000000 fluentbox-1.0.5/src/fluentbox.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-03-23 19:33:30.292039 fluentbox-1.0.5/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)    14996 2023-01-30 16:45:01.000000 fluentbox-1.0.5/tests/test_fluentbox.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-10 10:02:32.756944 fluentbox-1.0.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)       90 2023-03-23 19:38:01.000000 fluentbox-1.0.6/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-07-10 10:02:32.756944 fluentbox-1.0.6/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/src/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/src/fluentbox/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      239 2023-01-27 09:52:59.000000 fluentbox-1.0.6/src/fluentbox/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14836 2023-07-10 09:59:12.000000 fluentbox-1.0.6/src/fluentbox/fluentbox.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/src/fluentbox.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      249 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       10 2023-07-10 10:02:32.000000 fluentbox-1.0.6/src/fluentbox.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-10 10:02:32.756944 fluentbox-1.0.6/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14996 2023-01-30 16:45:01.000000 fluentbox-1.0.6/tests/test_fluentbox.py
```

### Comparing `fluentbox-1.0.5/src/fluentbox/fluentbox.py` & `fluentbox-1.0.6/src/fluentbox/fluentbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,35 @@
         :param operation: The operation to use when evaluating.
         :param value: The value to evaluate the item's attribute or key against.
         :return: The first item that satisfies the condition.
         :raises IndexError: When no item could be found that satisfies the condition.
         """
         return self.first_where(key, operation, value, or_fail=True)
 
+    def group_by(self, key: str | abc.Callable[[Any], abc.Hashable]) -> MutableMappingBox:
+        result = {}
+
+        callback: abc.Callable[[Any], abc.Hashable]
+        if isinstance(key, str):
+            callback = lambda value: self.__get_attribute_or_key(value, key, raise_on_error=True)
+
+        else:
+            callback = key
+
+        for value in self:
+            result_key = callback(value)
+
+            if result_key in result:
+                result[result_key].append(value)
+
+            else:
+                result[result_key] = [value]
+
+        return cast(MutableMappingBox, box(result))
+
     def key_by(self, key: str | abc.Callable[[Any], abc.Hashable]) -> MutableMappingBox:
         if isinstance(key, str):
             return self.map_and_key_by(lambda value: (self.__get_attribute_or_key(value, cast(str, key), raise_on_error=True), value))
 
         return self.map_and_key_by(lambda value: (key(value), value))  # type: ignore
 
     def map(self, callback: abc.Callable) -> Box:
```

### Comparing `fluentbox-1.0.5/tests/test_fluentbox.py` & `fluentbox-1.0.6/tests/test_fluentbox.py`

 * *Files identical despite different names*

