# Comparing `tmp/SempCode-0.3.7.5-py3-none-any.whl.zip` & `tmp/SempCode-0.5.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 4713 bytes, number of entries: 8
+Zip file size: 5550 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1750 b- defN 23-Jul-08 11:17 Semp/Command.py
 -rw-rw-rw-  2.0 fat     2390 b- defN 23-Jul-08 10:25 Semp/SempWrite.py
--rw-rw-rw-  2.0 fat     3738 b- defN 23-Jul-08 12:16 Semp/__init__.py
+-rw-rw-rw-  2.0 fat     3700 b- defN 23-Jul-10 10:58 Semp/__init__.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jul-08 11:54 Semp/about.py
--rw-rw-rw-  2.0 fat     1116 b- defN 23-Jul-08 12:39 SempCode-0.3.7.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-08 12:39 SempCode-0.3.7.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-08 12:39 SempCode-0.3.7.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      597 b- defN 23-Jul-08 12:39 SempCode-0.3.7.5.dist-info/RECORD
-8 files, 10058 bytes uncompressed, 3681 bytes compressed:  63.4%
+-rw-rw-rw-  2.0 fat     2660 b- defN 23-Jul-10 10:57 Semp/EasyTkinter/__init__.py
+-rw-rw-rw-  2.0 fat      750 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      681 b- defN 23-Jul-10 10:58 SempCode-0.5.0.1.dist-info/RECORD
+9 files, 12398 bytes uncompressed, 4386 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: Semp/__init__.py
 Comment: 
 
 Filename: Semp/about.py
 Comment: 
 
-Filename: SempCode-0.3.7.5.dist-info/METADATA
+Filename: Semp/EasyTkinter/__init__.py
 Comment: 
 
-Filename: SempCode-0.3.7.5.dist-info/WHEEL
+Filename: SempCode-0.5.0.1.dist-info/METADATA
 Comment: 
 
-Filename: SempCode-0.3.7.5.dist-info/top_level.txt
+Filename: SempCode-0.5.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: SempCode-0.3.7.5.dist-info/RECORD
+Filename: SempCode-0.5.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: SempCode-0.5.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Semp/__init__.py

```diff
@@ -1,20 +1,20 @@
 """
     Semp Python Tool by Win12Home
-    Version:0.3.7.5 Alpha
+    Version:0.5.0.1 Alpha
     
 """
 from PIL import Image,ImageTk
 from requests import *
 from sys import set_int_max_str_digits as max
 
 
 max(0)
-BINARY_TRUE="binary_true_T_WriteBinary"
-BINARY_FALSE="binary_false_F_OnlyWrite"
+BINARY_TRUE="BTRUE"
+BINARY_FALSE="BFALSE"
 
 class NumberError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 class BoolError(Exception):
     def __init__(self, *args, **kwargs):
         pass
```

## Comparing `SempCode-0.3.7.5.dist-info/RECORD` & `SempCode-0.5.0.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Semp/Command.py,sha256=Q3WpZq_YKORo-Ab8ZStGmLvZ3jdE7Yr7QyQgUXtwWTU,1750
 Semp/SempWrite.py,sha256=RDlzqY7yFAZjXh5w8LlGtoaDHJ9U9czvO5p_MW7N3sc,2390
-Semp/__init__.py,sha256=rHeZV4NMnxEO8st2ikTRb_1wZL8nFkRVJ4w3DpnFka4,3738
+Semp/__init__.py,sha256=ic6pWzshGY6G2oMS7925Qi9O7v9NvpzKhSPzlfxy2QQ,3700
 Semp/about.py,sha256=6dnRbFTZdDyFoMssu3qYmZtdWQhjDqU2VgN4jryIwpk,370
-SempCode-0.3.7.5.dist-info/METADATA,sha256=O0qxocnYo5BqMGdY0cBM-NC1uFOgD6do3ns2JBRlUh0,1116
-SempCode-0.3.7.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-SempCode-0.3.7.5.dist-info/top_level.txt,sha256=Di-SqoMJG3xW7CoY0ksMcZ_26p4QE8NuQV9einW_26k,5
-SempCode-0.3.7.5.dist-info/RECORD,,
+Semp/EasyTkinter/__init__.py,sha256=KV31i47ZKcfBx44odfiSLiw307MXxIyXtk_NS6u9pYw,2660
+SempCode-0.5.0.1.dist-info/METADATA,sha256=_0XVwBbJI4NDPOn49V0bsQltgXu4qfH2_8gAkZUIOWU,750
+SempCode-0.5.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+SempCode-0.5.0.1.dist-info/top_level.txt,sha256=Di-SqoMJG3xW7CoY0ksMcZ_26p4QE8NuQV9einW_26k,5
+SempCode-0.5.0.1.dist-info/RECORD,,
```

