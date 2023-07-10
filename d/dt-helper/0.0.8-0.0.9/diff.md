# Comparing `tmp/dt_helper-0.0.8-py3-none-any.whl.zip` & `tmp/dt_helper-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4842 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     8787 b- defN 22-Aug-08 10:54 dt_helper/__init__.py
+Zip file size: 4846 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     8823 b- defN 23-Jun-22 03:55 dt_helper/__init__.py
 -rw-rw-r--  2.0 unx       84 b- defN 20-Aug-08 20:59 dt_helper/settings.ini
--rw-rw-r--  2.0 unx      608 b- defN 22-Aug-08 11:35 dt_helper-0.0.8.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      967 b- defN 22-Aug-08 11:35 dt_helper-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-08 11:35 dt_helper-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 22-Aug-08 11:35 dt_helper-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      553 b- defN 22-Aug-08 11:35 dt_helper-0.0.8.dist-info/RECORD
-7 files, 11101 bytes uncompressed, 3856 bytes compressed:  65.3%
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jul-10 05:02 dt_helper-0.0.9.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-10 05:02 dt_helper-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 05:02 dt_helper-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-10 05:02 dt_helper-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      553 b- defN 23-Jul-10 05:02 dt_helper-0.0.9.dist-info/RECORD
+7 files, 11137 bytes uncompressed, 3860 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: dt_helper/__init__.py
 Comment: 
 
 Filename: dt_helper/settings.ini
 Comment: 
 
-Filename: dt_helper-0.0.8.dist-info/LICENSE.txt
+Filename: dt_helper-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dt_helper-0.0.8.dist-info/METADATA
+Filename: dt_helper-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: dt_helper-0.0.8.dist-info/WHEEL
+Filename: dt_helper-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: dt_helper-0.0.8.dist-info/top_level.txt
+Filename: dt_helper-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dt_helper-0.0.8.dist-info/RECORD
+Filename: dt_helper-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dt_helper/__init__.py

```diff
@@ -116,15 +116,16 @@
     """Return a utc_float_string for a given date_string
 
     - date_string: string form between 'YYYY' and 'YYYY-MM-DD HH:MM:SS.f'
     """
     dt = None
     s = None
     for fmt in [
-        '%Y-%m-%d %H:%M:%S', '%Y-%m-%d %H:%M', '%Y-%m-%d %H', '%Y-%m-%d', '%Y-%m', '%Y'
+        '%Y-%m-%d %H:%M:%S.%f', '%Y-%m-%d %H:%M:%S', '%Y-%m-%d %H:%M',
+        '%Y-%m-%d %H', '%Y-%m-%d', '%Y-%m', '%Y'
     ]:
         try:
             dt = datetime.strptime(str(date_string), fmt)
         except ValueError:
             continue
         else:
             break
@@ -134,15 +135,15 @@
             tz = pytz.timezone(timezone)
             dt = tz.localize(dt).astimezone(pytz.utc)
         s = dt_to_float_string(dt)
     return s
 
 
 def date_string_to_datetime(date_string, fmt='%Y-%m-%d', timezone=None):
-    """Return a date object for a string of a given format."""
+    """Return a datetime object for a string of a given format."""
     if isinstance(date_string, datetime):
         return date_string
     try:
         dt = datetime.strptime(date_string, fmt)
     except ValueError:
         # Truncate fractional seconds from string if not included in fmt
         dt = datetime.strptime(date_string.split('.')[0], fmt)
```

## Comparing `dt_helper-0.0.8.dist-info/LICENSE.txt` & `dt_helper-0.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dt_helper-0.0.8.dist-info/METADATA` & `dt_helper-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dt-helper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper funcs for doing things with datetime objects and UTC floats
 Home-page: https://github.com/kenjyco/dt-helper
-Download-URL: https://github.com/kenjyco/dt-helper/tarball/v0.0.8
+Download-URL: https://github.com/kenjyco/dt-helper/tarball/v0.0.9
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
 Keywords: datetime,date,time,utc,helper,kenjyco
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

## Comparing `dt_helper-0.0.8.dist-info/RECORD` & `dt_helper-0.0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-dt_helper/__init__.py,sha256=fi-f1wnhUP-N3MniG0JKLrm79vEF9OZ7jGNDGMN0lo4,8787
+dt_helper/__init__.py,sha256=WAxvRQDWbGvbNXcyewaACH6jmQ0dD3fEtgc0pVUHg6o,8823
 dt_helper/settings.ini,sha256=-18jkygnpZ9fUmb3hnUm3UeVPWvM_WD8JGMfBi7t3xc,84
-dt_helper-0.0.8.dist-info/LICENSE.txt,sha256=qkd6gO3_mhiG9TiDq5tJieC-1f64xFSpep3GBsIfNr0,608
-dt_helper-0.0.8.dist-info/METADATA,sha256=NVjARrfTMrTn8DMp6DGSepSV5JrWk9dxZCAHHoiP1M0,967
-dt_helper-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dt_helper-0.0.8.dist-info/top_level.txt,sha256=5c5nxN-4FAFTgtt6suNiGLISKAML-vf_TQnSFfVkHP0,10
-dt_helper-0.0.8.dist-info/RECORD,,
+dt_helper-0.0.9.dist-info/LICENSE.txt,sha256=qkd6gO3_mhiG9TiDq5tJieC-1f64xFSpep3GBsIfNr0,608
+dt_helper-0.0.9.dist-info/METADATA,sha256=PZx-CKevvuGfcHSMNYgeYpNsDpsFvuFootSnET6qiuQ,967
+dt_helper-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dt_helper-0.0.9.dist-info/top_level.txt,sha256=5c5nxN-4FAFTgtt6suNiGLISKAML-vf_TQnSFfVkHP0,10
+dt_helper-0.0.9.dist-info/RECORD,,
```

