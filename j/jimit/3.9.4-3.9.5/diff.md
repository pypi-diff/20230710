# Comparing `tmp/jimit-3.9.4-py3-none-any.whl.zip` & `tmp/jimit-3.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 25593 bytes, number of entries: 24
--rw-r--r--  2.0 unx      975 b- defN 23-Apr-02 14:09 jimit/__init__.py
+Zip file size: 25604 bytes, number of entries: 24
+-rw-r--r--  2.0 unx      975 b- defN 23-Jul-10 09:27 jimit/__init__.py
 -rw-r--r--  2.0 unx     6927 b- defN 21-Apr-30 10:16 jimit/check.py
 -rw-r--r--  2.0 unx     7082 b- defN 22-Oct-23 07:28 jimit/common.py
 -rw-r--r--  2.0 unx     1221 b- defN 19-Sep-09 06:13 jimit/convert.py
 -rw-r--r--  2.0 unx     4462 b- defN 22-Jan-22 20:54 jimit/downloader.py
 -rw-r--r--  2.0 unx      261 b- defN 17-Oct-25 12:05 jimit/ji_exceptions.py
 -rw-r--r--  2.0 unx     4442 b- defN 21-Apr-16 08:18 jimit/ji_time.py
 -rw-r--r--  2.0 unx     8114 b- defN 21-Apr-17 08:41 jimit/keep_read.py
 -rw-r--r--  2.0 unx     4636 b- defN 23-Mar-19 12:59 jimit/net_utils.py
 -rw-r--r--  2.0 unx      495 b- defN 17-Oct-25 12:08 jimit/regex.py
 -rw-r--r--  2.0 unx      581 b- defN 16-Nov-04 21:14 jimit/router.py
 -rw-r--r--  2.0 unx     4399 b- defN 21-Jun-04 18:35 jimit/security.py
 -rw-r--r--  2.0 unx     4391 b- defN 21-Apr-17 18:20 jimit/state_code.py
 -rw-r--r--  2.0 unx     1269 b- defN 21-Apr-16 08:14 jimit/transaction_serial_number.py
 -rw-r--r--  2.0 unx      322 b- defN 21-Apr-17 19:31 jimit/orm/__init__.py
--rw-r--r--  2.0 unx     3265 b- defN 23-Apr-02 14:08 jimit/orm/filter.py
+-rw-r--r--  2.0 unx     3304 b- defN 23-Jul-10 09:25 jimit/orm/filter.py
 -rw-r--r--  2.0 unx    14573 b- defN 22-Apr-01 17:54 jimit/orm/orm.py
 -rw-r--r--  2.0 unx      294 b- defN 21-Apr-17 18:54 jimit/orm/orm_exceptions.py
 -rw-r--r--  2.0 unx      175 b- defN 16-Jun-27 06:42 jimit/terminal/__init__.py
 -rw-r--r--  2.0 unx     3031 b- defN 16-Jun-27 09:16 jimit/terminal/color.py
--rw-r--r--  2.0 unx     3592 b- defN 23-Apr-02 14:09 jimit-3.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-02 14:09 jimit-3.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-02 14:09 jimit-3.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1809 b- defN 23-Apr-02 14:09 jimit-3.9.4.dist-info/RECORD
-24 files, 76414 bytes uncompressed, 22735 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx     3592 b- defN 23-Jul-10 09:27 jimit-3.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 09:27 jimit-3.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-10 09:27 jimit-3.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1809 b- defN 23-Jul-10 09:27 jimit-3.9.5.dist-info/RECORD
+24 files, 76453 bytes uncompressed, 22746 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: jimit/terminal/__init__.py
 Comment: 
 
 Filename: jimit/terminal/color.py
 Comment: 
 
-Filename: jimit-3.9.4.dist-info/METADATA
+Filename: jimit-3.9.5.dist-info/METADATA
 Comment: 
 
-Filename: jimit-3.9.4.dist-info/WHEEL
+Filename: jimit-3.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: jimit-3.9.4.dist-info/top_level.txt
+Filename: jimit-3.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: jimit-3.9.4.dist-info/RECORD
+Filename: jimit-3.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jimit/__init__.py

```diff
@@ -54,14 +54,14 @@
 )
 
 from .downloader import (
     DownloaderProxyType,
     Downloader
 )
 
-__version__ = "3.9.4"
+__version__ = "3.9.5"
 
 __all__ = [
     'index_state', 'Common', 'Check', 'Convert', 'JITime', 'Router', 'Security', 'NetUtils', 'KeepRead',
     'TransactionSerialNumber', 'JITError', 'PreviewingError', 'DownloaderProxyType', 'Downloader'
 ]
```

## jimit/orm/filter.py

```diff
@@ -33,15 +33,15 @@
 
     def __init__(self):
         pass
 
     @staticmethod
     def get_fit_statement(field_type=None, value=''):
         if field_type == FilterFieldType.INT.value:
-            if not value.lstrip('-').isdigit():
+            if not value.lstrip('-').isdigit() and not value.split('.')[-1].isdigit():
                 raise TypeError(''.join(['Value: ', str(value), ' should be digit']))
             return value
 
         elif field_type == FilterFieldType.STR.value:
             _s = regex_sql_str.sub('"', str(value)).strip('"')
             return ''.join(['"', _s.replace('"', '\\"'), '"'])
```

## Comparing `jimit-3.9.4.dist-info/METADATA` & `jimit-3.9.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jimit
-Version: 3.9.4
+Version: 3.9.5
 Summary: James Iter's common library by python.
 Home-page: https://github.com/jamesiter/jimitlib-py.git
 Author: James Iter
 Author-email: james.iter.cn@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

## Comparing `jimit-3.9.4.dist-info/RECORD` & `jimit-3.9.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-jimit/__init__.py,sha256=lj3igy9n_BbpRvUUtS0XDTyXhN-SJkuSTKk8e3WYc-0,975
+jimit/__init__.py,sha256=R839q4H6wx0VvFc8xwrtNbIGZhtILLZ2fWdc_1BlAtI,975
 jimit/check.py,sha256=JqYrJIQlF7psBRUd_7A0BpwpSyWE6VNqNvaF0IY9zew,6927
 jimit/common.py,sha256=mbKLK2roYtdozQaDvsTlrlmKh7fAlIzP6vE2Gux0ReY,7082
 jimit/convert.py,sha256=nVe3tDzWO9Vn_F-GNaT__xSdEe0LggOObnT8T_epdds,1221
 jimit/downloader.py,sha256=NJRWbgfDucGqLKdkJXLJ4EwE-prMXUOtttx16yvhLzk,4462
 jimit/ji_exceptions.py,sha256=0rMZMS2F2un_Tes_TIVfjOuZd3IDYEAm8F8eH6G4lro,261
 jimit/ji_time.py,sha256=xUvlqHcZyHEL_ZJXFmOhs6ZVXLQx4YAZ5QesW8q2iog,4442
 jimit/keep_read.py,sha256=Ob0_r2a02g7zIH80UGYNwIABhZgyz_rK84--wDBxAQg,8114
 jimit/net_utils.py,sha256=qPeDbp1_S5-DaLJOwvuuOFs49GGIy5aWsnqH9LSmjHI,4636
 jimit/regex.py,sha256=q25Nbhyp1s7f343HlJiATqHyQL4nKUWBzgJtZzuQybw,495
 jimit/router.py,sha256=9JPQh44I8GGYS-55uzUhTOiQISaDVt93l0T2vuLbxtU,581
 jimit/security.py,sha256=VZQIIcRP6DRBiJZ_vZ5NKX4CNew4IjAuERR_pMpOLPo,4399
 jimit/state_code.py,sha256=JHRwv3WJalwG-PF07ZsUsr1KIndCqZeN797B7k1QOwA,4391
 jimit/transaction_serial_number.py,sha256=Mk8j7ELA9WhG27bOxZ-U43HfEuggNAYngm_mWiHEBnA,1269
 jimit/orm/__init__.py,sha256=Ma1V-TWB7GIRcI7WWS0Gbi0KzXLQGBGcwN6OLSQcjz4,322
-jimit/orm/filter.py,sha256=bZnS35n26A1cNAprRU-ARQwp0cwacM3Nu6n7Ox_hzc8,3265
+jimit/orm/filter.py,sha256=UrWKV30EVVq16p3ZTPTsGmsF5pWb4KObA1wqLGMkiLs,3304
 jimit/orm/orm.py,sha256=NzvTJ-jfeRv7RUZNu593_QuM0xVRMBOc0ri3Oc-Nw3Q,14573
 jimit/orm/orm_exceptions.py,sha256=Acceen9JdCBN3KNeNDR8zcWqhAVf8SPxRVqMJGtIhss,294
 jimit/terminal/__init__.py,sha256=ZLy39AJVDCIanqEzTT-wRPBrabI9upHGr9z7XO8N2YY,175
 jimit/terminal/color.py,sha256=U79rJVCutqKzF5qLcKZpU73qfm9-Awso8__N027K2eA,3031
-jimit-3.9.4.dist-info/METADATA,sha256=LW0-aJ3UhoinHaSu2bR5JetUYsxC-Wi2tNGDkiBIHKE,3592
-jimit-3.9.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-jimit-3.9.4.dist-info/top_level.txt,sha256=DQl6cL_STApKhpROz0WE2poFLSTKXmStDcibvXVoWYc,6
-jimit-3.9.4.dist-info/RECORD,,
+jimit-3.9.5.dist-info/METADATA,sha256=57phodedZU6uTRdm3Ahk2yOl4M9bRBogIrALnMNCDb4,3592
+jimit-3.9.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+jimit-3.9.5.dist-info/top_level.txt,sha256=DQl6cL_STApKhpROz0WE2poFLSTKXmStDcibvXVoWYc,6
+jimit-3.9.5.dist-info/RECORD,,
```

