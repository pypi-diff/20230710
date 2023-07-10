# Comparing `tmp/swanapi-0.1.9-py3-none-any.whl.zip` & `tmp/swanapi-0.1.9b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11119 bytes, number of entries: 15
+Zip file size: 11147 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      158 b- defN 23-Jul-10 19:07 swanapi/__init__.py
 -rw-r--r--  2.0 unx    10349 b- defN 23-Jul-10 20:37 swanapi/base_inference.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
 -rw-r--r--  2.0 unx     2759 b- defN 23-Jul-10 19:56 swanapi/server.py
 -rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
 -rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 07:52 swanapi/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
 -rw-r--r--  2.0 unx     3889 b- defN 23-Jul-09 18:35 swanapi/docker_builder/config.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1419 b- defN 23-Jul-09 18:39 swanapi/docker_builder/runner.py
--rw-r--r--  2.0 unx      347 b- defN 23-Jul-10 20:44 swanapi-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 20:44 swanapi-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-10 20:44 swanapi-0.1.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-10 20:44 swanapi-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1218 b- defN 23-Jul-10 20:44 swanapi-0.1.9.dist-info/RECORD
-15 files, 26127 bytes uncompressed, 9097 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      349 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1228 b- defN 23-Jul-10 20:37 swanapi-0.1.9b2.dist-info/RECORD
+15 files, 26139 bytes uncompressed, 9105 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: swanapi/docker_builder/generate_dockerfile.py
 Comment: 
 
 Filename: swanapi/docker_builder/runner.py
 Comment: 
 
-Filename: swanapi-0.1.9.dist-info/METADATA
+Filename: swanapi-0.1.9b2.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.1.9.dist-info/WHEEL
+Filename: swanapi-0.1.9b2.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.1.9.dist-info/entry_points.txt
+Filename: swanapi-0.1.9b2.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.1.9.dist-info/top_level.txt
+Filename: swanapi-0.1.9b2.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.1.9.dist-info/RECORD
+Filename: swanapi-0.1.9b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `swanapi-0.1.9.dist-info/RECORD` & `swanapi-0.1.9b2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 swanapi/server.py,sha256=_8CvGMp69-WSvNr6zfZlAb6-Mnxi1b-H9daH2vkXEpE,2759
 swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
 swanapi/utils.py,sha256=VE09kmCHcSnPzCgCRdumEu5vnKjMwFAzWl29FoU6vs0,1065
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/docker_builder/config.py,sha256=CspWGMAyxZz_rd2JecCrsC4nL75Zh3o7XGAXMVHa32o,3889
 swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
 swanapi/docker_builder/runner.py,sha256=uDToZ5UfgshahcnKbu8Eb7enLLry2pVHn7e2bJB56vk,1419
-swanapi-0.1.9.dist-info/METADATA,sha256=MiP4x-pIYb-Sop6s8CsA5BGink5V7y7YlRcgU-ZSkLM,347
-swanapi-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.1.9.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.1.9.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.1.9.dist-info/RECORD,,
+swanapi-0.1.9b2.dist-info/METADATA,sha256=xQB2b5pTSJxvPa-OBXu8KJ51kMLan0jMKDwmWcjv3tw,349
+swanapi-0.1.9b2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.1.9b2.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.1.9b2.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.1.9b2.dist-info/RECORD,,
```

