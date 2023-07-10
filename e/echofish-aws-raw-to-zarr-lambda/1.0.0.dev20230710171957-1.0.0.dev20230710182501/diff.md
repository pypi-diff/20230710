# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957.tar", last modified: Mon Jul 10 17:21:02 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501.tar", last modified: Mon Jul 10 18:26:05 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:21:02.680351 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 17:21:02.680351 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 17:21:02.680351 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-10 17:20:57.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:21:02.676351 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:21:02.676351 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15503 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-07-10 17:19:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:21:02.680351 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 17:21:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-10 17:21:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:21:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 17:21:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 17:21:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:26:05.399083 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 18:26:05.399083 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 18:26:05.399083 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-10 18:26:00.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:26:05.395084 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:26:05.399083 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15503 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5577 2023-07-10 18:24:56.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:26:05.399083 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 18:26:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-10 18:26:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:26:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 18:26:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 18:26:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230710171957
+Version: 1.0.0.dev20230710182501
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230710171957",
+  version="1.0.0.dev20230710182501",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,49 +4,60 @@
 class S3Operations:
     #####################################################################
     def __get_client(
         self,
         access_key_id=None,
         secret_access_key=None
     ):
-        # client = None
         if access_key_id:
-            print('there is an access_key_id')
-            client = boto3.Session().client(
-                service_name='s3',
+            session = boto3.Session(
                 aws_access_key_id=access_key_id,
                 aws_secret_access_key=secret_access_key
             )
+            client = session.client(
+                service_name='s3',
+                # aws_access_key_id=access_key_id,
+                # aws_secret_access_key=secret_access_key
+            )
         else:
             client = boto3.Session().client('s3')
-        print('testing client...')
-        print(client.list_objects(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow/HB0707')['Contents'][0])
+        # print('testing client...')
+        # print(client.list_objects(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow/HB0707')['Contents'][0])
         return client
 
     #####################################################################
     def list_objects(  # analog to "find_children_objects"
         self,
         bucket_name,
         prefix,
         access_key_id=None,
         secret_access_key=None
     ):
-
         keys = []
         s3_client = self.__get_client(
             access_key_id=access_key_id,
             secret_access_key=secret_access_key
         )
+        #######################################################
+        print('start test')
+        s3 = boto3.Session().client(
+            service_name='s3',
+            aws_access_key_id="AKIA2KSLXHVML5SEVCGJ",
+            aws_secret_access_key="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",
+        )
+        print('testing w hard coded credentials')
+        print(len(s3.list_objects(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow/HB0707')['Contents'][0]))
+        print('end test')
+        ########################################################
         s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds')
-        print(s3_client.meta.endpoint_url)
-        print(s3_client.meta.region_name)
         print(s3_client.meta.config.signature_version)  # s3v4
         print(s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds'))
         print('listing files')
-        len(s3_client.list_objects_v2(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow')['Contents'])
+        print(len(s3_client.list_objects(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow')['Contents'][0]))
+        print(len(s3_client.list_objects_v2(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow')['Contents'][0]))
         print('other')
         for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             # problem here
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230710171957
+Version: 1.0.0.dev20230710182501
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710171957/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710182501/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

