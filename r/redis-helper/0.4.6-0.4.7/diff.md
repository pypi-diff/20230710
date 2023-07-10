# Comparing `tmp/redis_helper-0.4.6-py3-none-any.whl.zip` & `tmp/redis_helper-0.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 29526 bytes, number of entries: 17
+Zip file size: 30719 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx     4891 b- defN 22-Mar-13 03:29 redis_helper/__init__.py
--rw-rw-r--  2.0 unx    60010 b- defN 22-Aug-09 04:22 redis_helper/collection.py
+-rw-rw-r--  2.0 unx    61383 b- defN 23-Jun-21 15:14 redis_helper/collection.py
 -rw-rw-r--  2.0 unx      290 b- defN 22-Mar-12 14:52 redis_helper/settings.ini
 -rw-rw-r--  2.0 unx        0 b- defN 20-Aug-08 21:00 redis_helper/scripts/__init__.py
+-rw-rw-r--  2.0 unx      372 b- defN 23-Jun-21 15:14 redis_helper/scripts/clear_locks.py
+-rw-rw-r--  2.0 unx      361 b- defN 23-Jun-21 15:14 redis_helper/scripts/collection_reports.py
 -rw-rw-r--  2.0 unx      773 b- defN 20-Aug-08 21:00 redis_helper/scripts/download_examples.py
 -rw-rw-r--  2.0 unx      797 b- defN 20-Aug-08 21:00 redis_helper/scripts/download_scripts.py
 -rw-rw-r--  2.0 unx     1646 b- defN 20-Aug-08 21:00 redis_helper/scripts/notes.py
 -rw-rw-r--  2.0 unx      552 b- defN 20-Oct-05 04:18 redis_helper/scripts/shell.py
 -rw-rw-r--  2.0 unx       43 b- defN 20-Oct-04 14:12 tests/__init__.py
 -rw-rw-r--  2.0 unx     8973 b- defN 22-Apr-12 16:38 tests/test_collection.py
 -rw-rw-r--  2.0 unx      299 b- defN 22-Mar-13 05:58 tests/test_settings.py
--rw-rw-r--  2.0 unx      608 b- defN 22-Aug-09 04:34 redis_helper-0.4.6.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx    24878 b- defN 22-Aug-09 04:34 redis_helper-0.4.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-09 04:34 redis_helper-0.4.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx      236 b- defN 22-Aug-09 04:34 redis_helper-0.4.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       19 b- defN 22-Aug-09 04:34 redis_helper-0.4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1443 b- defN 22-Aug-09 04:34 redis_helper-0.4.6.dist-info/RECORD
-17 files, 105550 bytes uncompressed, 27128 bytes compressed:  74.3%
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jul-10 05:03 redis_helper-0.4.7.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx    24901 b- defN 23-Jul-10 05:03 redis_helper-0.4.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 05:03 redis_helper-0.4.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      364 b- defN 23-Jul-10 05:03 redis_helper-0.4.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       19 b- defN 23-Jul-10 05:03 redis_helper-0.4.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1632 b- defN 23-Jul-10 05:03 redis_helper-0.4.7.dist-info/RECORD
+19 files, 107996 bytes uncompressed, 28015 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -6,14 +6,20 @@
 
 Filename: redis_helper/settings.ini
 Comment: 
 
 Filename: redis_helper/scripts/__init__.py
 Comment: 
 
+Filename: redis_helper/scripts/clear_locks.py
+Comment: 
+
+Filename: redis_helper/scripts/collection_reports.py
+Comment: 
+
 Filename: redis_helper/scripts/download_examples.py
 Comment: 
 
 Filename: redis_helper/scripts/download_scripts.py
 Comment: 
 
 Filename: redis_helper/scripts/notes.py
@@ -27,26 +33,26 @@
 
 Filename: tests/test_collection.py
 Comment: 
 
 Filename: tests/test_settings.py
 Comment: 
 
-Filename: redis_helper-0.4.6.dist-info/LICENSE.txt
+Filename: redis_helper-0.4.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: redis_helper-0.4.6.dist-info/METADATA
+Filename: redis_helper-0.4.7.dist-info/METADATA
 Comment: 
 
-Filename: redis_helper-0.4.6.dist-info/WHEEL
+Filename: redis_helper-0.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: redis_helper-0.4.6.dist-info/entry_points.txt
+Filename: redis_helper-0.4.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: redis_helper-0.4.6.dist-info/top_level.txt
+Filename: redis_helper-0.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: redis_helper-0.4.6.dist-info/RECORD
+Filename: redis_helper-0.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## redis_helper/collection.py

```diff
@@ -10,15 +10,15 @@
 from functools import partial
 from itertools import chain
 from io import StringIO
 from pprint import pprint
 from redis import ResponseError
 try:
     from ujson import dumps, loads
-except ImportError:
+except (ImportError, ModuleNotFoundError):
     from json import dumps, loads
 
 
 META_FIELDS = {'_id', '_ts'}
 _CURLY_MATCHER = ih.matcher.CurlyMatcher()
 
 
@@ -98,14 +98,16 @@
         self._next_id_string_key = self._make_key(self._base_key, '_next_id')
         self._ts_zset_key = self._make_key(self._base_key, '_ts')
         self._id_zset_key = self._make_key(self._base_key, '_id')
         self._in_zset_key = self._make_key(self._base_key, '_in')
         self._get_id_stats_hash_key = self._make_key(self._base_key, '_get_id_stats')
         self._get_field_stats_hash_key = self._make_key(self._base_key, '_get_field_stats')
         self._lock_string_key = self._make_key(self._base_key, '_LOCK')
+        self._lock_time_string_key = self._make_key(self._base_key, '_LOCK_TIME')
+        self._lock_durations_list_key = self._make_key(self._base_key, '_LOCK_DURATIONS')
         self._find_base_key = self._make_key(self._base_key, '_find')
         self._find_next_id_string_key = self._make_key(self._find_base_key, '_next_id')
         self._find_stats_hash_key = self._make_key(self._find_base_key, '_stats')
         self._find_searches_zset_key = self._make_key(self._find_base_key, '_searches')
 
         ref_errors = []
         for f in self._reference_fields:
@@ -208,19 +210,30 @@
         return self._make_key(base_key, int(result[1]))
 
     def _get_next_find_key(self):
         return self._get_next_key(self._find_next_id_string_key, self._find_base_key)
 
     def _lock(self):
         """Lock the collection from being modified"""
-        rh.REDIS.set(self._lock_string_key, 'True')
+        pipe = rh.REDIS.pipeline()
+        pipe.set(self._lock_string_key, 'True')
+        pipe.set(self._lock_time_string_key, dh.utc_now_float_string())
+        pipe.execute()
 
     def _unlock(self):
         """Unlock the collection and allow modifications"""
-        rh.REDIS.set(self._lock_string_key, 'False')
+        lock_start = ih.from_string(ih.decode(rh.REDIS.get(self._lock_time_string_key)))
+        pipe = rh.REDIS.pipeline()
+        pipe.set(self._lock_string_key, 'False')
+        if lock_start:
+            now_string = dh.utc_now_float_string()
+            duration = round(ih.from_string(now_string) - lock_start, 5)
+            pipe.delete(self._lock_time_string_key)
+            pipe.lpush(self._lock_durations_list_key, '{}--{}'.format(now_string, duration))
+        pipe.execute()
 
     @property
     def is_locked(self):
         """Return True if the collection is locked"""
         return ih.from_string(ih.decode(rh.REDIS.get(self._lock_string_key))) is True
 
     def wait_for_unlock(self, sleeptime=.5):
@@ -603,15 +616,15 @@
         """A class method to select previously created model instance"""
         models = cls.select_models()
         if models:
             return models[0]
 
     @classmethod
     def report_all(cls):
-        """A class method to show some info about the classes"""
+        """A class method to show some info about the Collections"""
         pprint(rh.REDIS.hgetall('_REDIS_HELPER_COLLECTION'))
 
     @property
     def last_update(self):
         """Return the last time the collection was updated"""
         return ih.decode(rh.REDIS.hget(
             '_REDIS_HELPER_COLLECTION',
@@ -715,14 +728,30 @@
         ])
 
     def clear_keyspace(self):
         """Delete all Redis keys under self._base_key"""
         for key in rh.REDIS.scan_iter('{}*'.format(self._base_key)):
             rh.REDIS.delete(key)
 
+    @classmethod
+    def clear_all_collection_locks(cls):
+        """Clear all Collection locks"""
+        lock_keys = []
+        lock_time_keys = []
+        for base_key in cls.init_stats()['init_args'].keys():
+            lock_keys.append(rh.REDIS.scan_iter('{}:_LOCK'.format(base_key)))
+            lock_time_keys.append(rh.REDIS.scan_iter('{}:_LOCK_TIME'.format(base_key)))
+
+        pipe = rh.REDIS.pipeline()
+        for lock_key in chain(*lock_keys):
+            pipe.set(lock_key, 'False')
+        for lock_time_key in chain(*lock_time_keys):
+            pipe.delete(lock_time_key)
+        pipe.execute()
+
     def delete(self, hash_id, pipe=None):
         """Delete a specific hash_id's data and remove from indexes it is in
 
         - hash_id: hash_id to remove
         - pipe: if a redis pipeline object is passed in, just add more
           operations to the pipe
         """
```

## Comparing `redis_helper-0.4.6.dist-info/LICENSE.txt` & `redis_helper-0.4.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `redis_helper-0.4.6.dist-info/METADATA` & `redis_helper-0.4.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: redis-helper
-Version: 0.4.6
+Version: 0.4.7
 Summary: Easily store, index, and modify Python dicts in Redis (with flexible searching)
 Home-page: https://github.com/kenjyco/redis-helper
-Download-URL: https://github.com/kenjyco/redis-helper/tarball/v0.4.6
+Download-URL: https://github.com/kenjyco/redis-helper/tarball/v0.4.7
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
 Keywords: redis,cli,command-line,dictionary,data,database,secondary index,model,prototype,event logging,dashboard,easy modeling,helper,kenjyco
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -389,15 +389,15 @@
 project. In cases like this you can do the following:
 
 ::
 
    try:
        import redis_helper as rh
        from redis import ConnectionError as RedisConnectionError
-   except ImportError:
+   except (ImportError, ModuleNotFoundError):
        SomeCollection = None
    else:
        try:
            SomeCollection = rh.Collection(
                ...
            )
        except RedisConnectionError:
```

## Comparing `redis_helper-0.4.6.dist-info/RECORD` & `redis_helper-0.4.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 redis_helper/__init__.py,sha256=deazilqxw3EBFkYk-BNlAoQTCNRgbIgj7n0QiDl7dH0,4891
-redis_helper/collection.py,sha256=9rNfkJDajxaqihB642mJ29HZKv3Npqw0cJcntrRAryE,60010
+redis_helper/collection.py,sha256=qqgvieC9LL_voxaKjVJ8z0R18oFdJViBNPyyHBbZqwI,61383
 redis_helper/settings.ini,sha256=NETRCY9P2xGGgciF_76rtYCsx0bXQvXFP0GzWXzDXcg,290
 redis_helper/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+redis_helper/scripts/clear_locks.py,sha256=vBqqTnT-DH0l-9bBUjWXjO7KjDD8AN7dktIxujCsBV8,372
+redis_helper/scripts/collection_reports.py,sha256=OQRjdd55fPIo1-oDqJ8HZOVE0Us2fnWHhaBiEs6MZ9U,361
 redis_helper/scripts/download_examples.py,sha256=VhM3Vkegrvi5zcV8q_1kVbcL5w0E0bhuDa4nt4WJQXE,773
 redis_helper/scripts/download_scripts.py,sha256=2jgpt9mjQ5A8ZRsafLZ8FOKQAz4cT67Pjy-BQQCQhFU,797
 redis_helper/scripts/notes.py,sha256=h99QhnAdiQzCoDyJleVZsuWemDtajhGYSnzvzcqHAQ8,1646
 redis_helper/scripts/shell.py,sha256=fWwXJ9d0No_EPJPemkq5-HGwuH9JnSpJXXzSalG7cLc,552
 tests/__init__.py,sha256=jci-DFyrUeT4kU4vCgkmGeFgq6wfxwEtoyRQcBSuM_8,43
 tests/test_collection.py,sha256=Ujo5LllD75Ifex5XvAyhnN2NiGpn26mSzO0gyDj4q5I,8973
 tests/test_settings.py,sha256=4L2udKlKJvZZ3KRP9RM60Dwj6mhtfBvkwgt299WRuTY,299
-redis_helper-0.4.6.dist-info/LICENSE.txt,sha256=2JijE8Cf8mYr8FsfWCqTUAgVlMrGmzp1NssckIGh5Hc,608
-redis_helper-0.4.6.dist-info/METADATA,sha256=EfTN7QfxPOtl2VquhNbgtDGKrLysNFQ2JqsopP3Ybq8,24878
-redis_helper-0.4.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-redis_helper-0.4.6.dist-info/entry_points.txt,sha256=RMRqFrpH7FENiGKRPowuLtdvaT4tYr5l3xinxE5ROK4,236
-redis_helper-0.4.6.dist-info/top_level.txt,sha256=lvNePSKTlPiIP7X5x2l3qePtKm30YeY-BjrtkkwvGdY,19
-redis_helper-0.4.6.dist-info/RECORD,,
+redis_helper-0.4.7.dist-info/LICENSE.txt,sha256=2JijE8Cf8mYr8FsfWCqTUAgVlMrGmzp1NssckIGh5Hc,608
+redis_helper-0.4.7.dist-info/METADATA,sha256=ai9vmTPUIhP9Or1Qza523sX3HhuN1A1xBRj6TKnRr8U,24901
+redis_helper-0.4.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+redis_helper-0.4.7.dist-info/entry_points.txt,sha256=LXEi1Ywmrwe5nt7dFKmfulNEBKp7Ffrn53SlGH3PW_A,364
+redis_helper-0.4.7.dist-info/top_level.txt,sha256=lvNePSKTlPiIP7X5x2l3qePtKm30YeY-BjrtkkwvGdY,19
+redis_helper-0.4.7.dist-info/RECORD,,
```

