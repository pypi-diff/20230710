# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045.tar", last modified: Mon Jul 10 06:41:44 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010.tar", last modified: Mon Jul 10 07:51:10 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:43.997756 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 06:41:43.997756 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 06:41:43.997756 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-10 06:41:39.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:43.997756 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:43.997756 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15663 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-07-10 06:40:41.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 06:41:43.997756 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 06:41:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-10 06:41:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 06:41:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 06:41:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 06:41:43.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:51:10.074775 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 07:51:10.074775 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 07:51:10.074775 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-10 07:51:05.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:51:10.074775 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:51:10.074775 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15663 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2023-07-10 07:50:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 07:51:10.074775 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-10 07:51:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-10 07:51:10.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 07:51:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 07:51:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 07:51:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230710064045
+Version: 1.0.0.dev20230710075010
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230710064045",
+  version="1.0.0.dev20230710075010",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             secret_access_key=secret_access_key
         )
         s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds')
         print(s3_client.meta.endpoint_url)
         print(s3_client.meta.region_name)
         print(s3_client.meta.config.signature_version)  # s3v4
         print(s3_client.get_bucket_policy(Bucket='noaa-wcsd-zarr-pds'))
+        print('listing files')
+        len(s3_client.list_objects_v2(Bucket='noaa-wcsd-zarr-pds', Prefix='level_2/Henry_B._Bigelow')['Contents'])
         for page in s3_client.get_paginator('list_objects_v2').paginate(Bucket=bucket_name, Prefix=prefix):
             # problem here
             if 'Contents' in page.keys():
                 keys.extend(page['Contents'])
         return keys
 
     #####################################################################
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230710064045
+Version: 1.0.0.dev20230710075010
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710064045/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230710075010/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

