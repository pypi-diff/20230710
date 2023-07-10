# Comparing `tmp/qesdk-0.1.8.tar.gz` & `tmp/qesdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qesdk-0.1.8.tar", last modified: Sun Jun 11 13:23:30 2023, max compression
+gzip compressed data, was "qesdk-0.1.9.tar", last modified: Mon Jul 10 07:27:40 2023, max compression
```

## Comparing `qesdk-0.1.8.tar` & `qesdk-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.147007 qesdk-0.1.8/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6225 2023-06-11 13:23:30.147007 qesdk-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.8/README.md
--rw-rw-rw-   0        0        0      751 2023-06-11 13:17:44.000000 qesdk-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 13:23:30.147007 qesdk-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.130007 qesdk-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.141008 qesdk-0.1.8/src/qesdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.8/src/qesdk/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.8/src/qesdk/aio_api.py
--rw-rw-rw-   0        0        0    29394 2023-06-08 10:07:17.000000 qesdk-0.1.8/src/qesdk/api.py
--rw-rw-rw-   0        0        0     7286 2023-06-11 13:17:29.000000 qesdk-0.1.8/src/qesdk/client.py
--rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.8/src/qesdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.8/src/qesdk/qedata.thrift
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.8/src/qesdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 13:23:30.146008 qesdk-0.1.8/src/qesdk.egg-info/
--rw-rw-rw-   0        0        0     6225 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-11 13:23:30.000000 qesdk-0.1.8/src/qesdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 07:27:40.605770 qesdk-0.1.9/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6225 2023-07-10 07:27:40.605770 qesdk-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.9/README.md
+-rw-rw-rw-   0        0        0      751 2023-07-10 07:26:45.000000 qesdk-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:27:40.606769 qesdk-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 07:27:40.588771 qesdk-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 07:27:40.599772 qesdk-0.1.9/src/qesdk/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.9/src/qesdk/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.9/src/qesdk/aio_api.py
+-rw-rw-rw-   0        0        0    30044 2023-07-10 06:54:54.000000 qesdk-0.1.9/src/qesdk/api.py
+-rw-rw-rw-   0        0        0     7286 2023-07-10 07:27:09.000000 qesdk-0.1.9/src/qesdk/client.py
+-rw-rw-rw-   0        0        0      237 2023-07-10 07:04:31.000000 qesdk-0.1.9/src/qesdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.9/src/qesdk/qedata.thrift
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.9/src/qesdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:27:40.604771 qesdk-0.1.9/src/qesdk.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-07-10 07:27:40.000000 qesdk-0.1.9/src/qesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-10 07:27:40.000000 qesdk-0.1.9/src/qesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:27:40.000000 qesdk-0.1.9/src/qesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-07-10 07:27:40.000000 qesdk-0.1.9/src/qesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-10 07:27:40.000000 qesdk-0.1.9/src/qesdk.egg-info/top_level.txt
```

### Comparing `qesdk-0.1.8/LICENSE` & `qesdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.8/PKG-INFO` & `qesdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.8/README.md` & `qesdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.8/pyproject.toml` & `qesdk-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qesdk"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qesdk-0.1.8/src/qesdk/aio_api.py` & `qesdk-0.1.9/src/qesdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.8/src/qesdk/api.py` & `qesdk-0.1.9/src/qesdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
                   'volmult': 100, 'ticksize':0.2}
         return res        
     else:
         return qedataClient.instance()('get_instrument_setting', **locals())
     
 
 @assert_auth
-def get_price(security, start_date, end_date, freq='minute', fields=None, overnight=False, silent=False):
+def get_price(security, start_date, end_date, freq='minute', fields=None, overnight=False, silent=False, adjustFactor=None):
     '''
     Get the bar structure data.  
     security: such as \'AG2001.SFE\' 
     start_date/end_date: such as \'2010-02-01\'
     freq: \'minute\' as default frequecny. other choice: \'daily\' \'hour\'
           \'XT\' far X minutes, \'XB\' for X days.
     fields: None is default, get all fields. Or user could choose some of these fields.    
@@ -366,48 +366,63 @@
     '''
 
     freqtype = convert_freq(freq)
     if freqtype < 0:
         print(f"freq {freq} 不合法, 合法的频率设置如下：'minute','hour','daily','XT','XB'")
         return None
     security = convert_security(security)
+
     if security is None:
         return
-    
+    isStock = security[-3:] in ['SSE','SZE']
+
+
     if freqtype == 1:
-        dfcols = ['open','close','high','low','volume','money','position','upperlimit','lowerlimit','presett','preclose','settle']
+        if isStock:
+            dfcols = ['open', 'close', 'high', 'low', 'volume', 'money', 'upperlimit', 'lowerlimit',
+                    'preclose', 'accumAdjFactor']
+        else:
+            dfcols = ['open', 'close', 'high', 'low', 'volume', 'money', 'position', 'upperlimit', 'lowerlimit', 'presett',
+                    'preclose', 'settle']
     else:
         dfcols = ['open','close','high','low','volume','money']
     
     try:
+        if isStock :
+            if not adjustFactor is None:
+                assert adjustFactor in ['pre','post'], "adjustFactor 必须为'pre'前复权或'post'后复权"
+            else:
+                adjustFactor = 'none'    
         if fields :
            assert isinstance(fields,list) and len(fields) > 0, "fields 必须为list类型，并且不能为空."
            dfcols = [f for f in fields if f in dfcols]
         cols = json.dumps(dfcols)
         start_date = convert_start_date(start_date, freqtype, overnight)
         if not start_date:
             return None
         end_date = convert_end_date(end_date, freqtype, overnight)
         if not end_date:
             return None
     
-           
-        if len(security) >= 14:
+        if isStock:
+                dbname = "stocks_daily" if freqtype == 1 else "stocks_minu"           
+        elif len(security) >= 14:
             if security[-3:] == 'CCF':
                 dbname = "options_ccf_daily" if freqtype == 1 else "options_ccf_minu"
             else:
                 return pd.DataFrame()
         elif security[-3:] == 'SSE':
             dbname = "options_shg_daily" if freqtype == 1 else "options_shg_minu"
             
         elif security[-3:] == 'SGE':
             dbname = "sge_daily" if freqtype == 1 else "sge_minu"
         else:
             dbname = "futures_daily" if freqtype == 1 else "futures_minu"
         del dfcols
+        print(dbname)
         return qedataClient.instance()('get_price',**locals())
     except Exception as e:
         print("get_price Error:", e.__traceback__.tb_lineno,e)
         return None
```

### Comparing `qesdk-0.1.8/src/qesdk/client.py` & `qesdk-0.1.9/src/qesdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                      'port' : 6001}  
     avail_servers = [server_config]
     server_index = 0                 
 
     
 
 
-__version__='0.1.8'
+__version__='0.1.9'
 
 thrift_path = path.join(sys.modules["ROOT_DIR"], "qedata.thrift")
 thrift_path = path.abspath(thrift_path)
 #print(thrift_path)
 qedata_thrift = thriftpy2.load(thrift_path, module_name="qedata_thrift")
 loop = asyncio.get_event_loop()
 def setTimeout(client, timeout):
```

### Comparing `qesdk-0.1.8/src/qesdk/qedata.thrift` & `qesdk-0.1.9/src/qesdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.8/src/qesdk/utils.py` & `qesdk-0.1.9/src/qesdk/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.8/src/qesdk.egg-info/PKG-INFO` & `qesdk-0.1.9/src/qesdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

