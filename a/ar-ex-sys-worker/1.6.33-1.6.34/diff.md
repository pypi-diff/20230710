# Comparing `tmp/ar_ex_sys_worker-1.6.33-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.34-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16330 bytes, number of entries: 11
+Zip file size: 16348 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    29452 b- defN 23-Jun-05 10:29 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    29611 b- defN 23-Jul-10 07:24 ar_external_sys_worker/main.py
 -rw-rw-rw-  2.0 fat    19901 b- defN 23-Jun-05 10:30 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Jun-05 10:30 ar_ex_sys_worker-1.6.33.dist-info/RECORD
-11 files, 64229 bytes uncompressed, 14614 bytes compressed:  77.2%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-Jul-10 07:25 ar_ex_sys_worker-1.6.34.dist-info/RECORD
+11 files, 64388 bytes uncompressed, 14632 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.33.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.34.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.33.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.34.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.33.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.34.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.33.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.34.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.33.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.34.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -503,14 +503,18 @@
             return
         if signal_id.strip() == 'this carrier was not found':
             self.delete_act_from_send_reports(record_id)
             return {
                 'error': {f'Act has not been delivered cos {signal_id}. '
                           f'Deleted from log...'}}
         if not self.is_valid_uuid(signal_id):
+            try:
+                self.delete_act_from_send_reports(record_id)
+            except:
+                return {'error': traceback.format_exc()}
             return {'error': f'act not found in signall_id ({signal_id})'}
         return self.update_act(
             signall_id=signal_id,
             car_number=car_number,
             transporter_inn=transporter_inn,
             trash_cat=trash_cat,
             trash_type=trash_type,
```

## Comparing `ar_ex_sys_worker-1.6.33.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.34.dist-info/LICENSE`

 * *Files identical despite different names*

