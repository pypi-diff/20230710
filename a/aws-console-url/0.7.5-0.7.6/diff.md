# Comparing `tmp/aws_console_url-0.7.5.tar.gz` & `tmp/aws_console_url-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_console_url-0.7.5.tar", last modified: Fri May 12 17:57:30 2023, max compression
+gzip compressed data, was "aws_console_url-0.7.6.tar", last modified: Mon Jul 10 20:53:35 2023, max compression
```

## Comparing `aws_console_url-0.7.5.tar` & `aws_console_url-0.7.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.234783 aws_console_url-0.7.5/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-12 17:57:30.234646 aws_console_url-0.7.5/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)    15928 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/Public-API.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     2905 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.229656 aws_console_url-0.7.5/aws_console_url/
--rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 01:36:58.000000 aws_console_url-0.7.5/aws_console_url/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/compat.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3555 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/console.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.230399 aws_console_url-0.7.5/aws_console_url/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6758 2023-05-12 01:33:30.000000 aws_console_url-0.7.5/aws_console_url/model.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1213 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/resource.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.233652 aws_console_url-0.7.5/aws_console_url/srv/
--rw-r--r--   0 sanhehu    (501) staff       (20)       45 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2769 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/a2i.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5747 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/awslambda.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    14455 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/cloudformation.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4619 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/cloudwatch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5455 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/codebuild.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4116 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/codecommit.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1831 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1553 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/ecr.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4386 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/glue.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1596 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/ground_truth.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4917 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/iam.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2502 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/s3.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1207 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/sagemaker.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/secretmanager.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1834 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/sqs.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1607 2023-05-09 19:38:31.000000 aws_console_url-0.7.5/aws_console_url/srv/ssm.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5552 2023-05-09 19:36:47.000000 aws_console_url-0.7.5/aws_console_url/srv/step_function.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2810 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/srv/vpc.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.234043 aws_console_url-0.7.5/aws_console_url/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/aws_console_url/tests/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.230275 aws_console_url-0.7.5/aws_console_url.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1322 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      300 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-05-12 17:57:30.000000 aws_console_url-0.7.5/aws_console_url.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2606 2023-05-12 01:36:51.000000 aws_console_url-0.7.5/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      297 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      117 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 17:57:30.234824 aws_console_url-0.7.5/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7661 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 17:57:30.234386 aws_console_url-0.7.5/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      290 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/tests/test_builder.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1658 2023-05-09 19:32:30.000000 aws_console_url-0.7.5/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.778494 aws_console_url-0.7.6/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-07-10 20:53:35.778349 aws_console_url-0.7.6/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15928 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/Public-API.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2905 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.773028 aws_console_url-0.7.6/aws_console_url/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-10 20:51:11.000000 aws_console_url-0.7.6/aws_console_url/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3555 2023-07-10 20:51:01.000000 aws_console_url-0.7.6/aws_console_url/console.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.773821 aws_console_url-0.7.6/aws_console_url/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6758 2023-05-12 01:33:30.000000 aws_console_url-0.7.6/aws_console_url/model.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1213 2023-07-10 20:51:01.000000 aws_console_url-0.7.6/aws_console_url/resource.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.777212 aws_console_url-0.7.6/aws_console_url/srv/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       45 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2991 2023-07-10 20:36:00.000000 aws_console_url-0.7.6/aws_console_url/srv/a2i.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5747 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/awslambda.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    14455 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/cloudformation.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4619 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/cloudwatch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5455 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/codebuild.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4116 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/codecommit.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1831 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1553 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/ecr.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4386 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/glue.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1596 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/ground_truth.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4917 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/iam.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2502 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1207 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/sagemaker.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/secretmanager.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1834 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/sqs.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1607 2023-05-09 19:38:31.000000 aws_console_url-0.7.6/aws_console_url/srv/ssm.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5552 2023-05-09 19:36:47.000000 aws_console_url-0.7.6/aws_console_url/srv/step_function.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2810 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/srv/vpc.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.777610 aws_console_url-0.7.6/aws_console_url/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      352 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1215 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      370 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/aws_console_url/tests/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.773698 aws_console_url-0.7.6/aws_console_url.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3983 2023-07-10 20:53:35.000000 aws_console_url-0.7.6/aws_console_url.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1322 2023-07-10 20:53:35.000000 aws_console_url-0.7.6/aws_console_url.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-10 20:53:35.000000 aws_console_url-0.7.6/aws_console_url.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      330 2023-07-10 20:53:35.000000 aws_console_url-0.7.6/aws_console_url.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-07-10 20:53:35.000000 aws_console_url-0.7.6/aws_console_url.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2797 2023-07-10 20:52:17.000000 aws_console_url-0.7.6/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      297 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      189 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      147 2023-07-10 20:47:19.000000 aws_console_url-0.7.6/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-10 20:53:35.778541 aws_console_url-0.7.6/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7661 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:53:35.778017 aws_console_url-0.7.6/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      290 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/tests/test_builder.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1658 2023-05-09 19:32:30.000000 aws_console_url-0.7.6/tests/test_import.py
```

### Comparing `aws_console_url-0.7.5/LICENSE.txt` & `aws_console_url-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/PKG-INFO` & `aws_console_url-0.7.6/aws_console_url.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: aws_console_url
-Version: 0.7.5
+Name: aws-console-url
+Version: 0.7.6
 Summary: Build AWS Console Url for debugging.
 Home-page: https://github.com/MacHu-GWU/aws_console_url-project
-Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.5#downloads
+Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.6#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_console_url-0.7.5/Public-API.rst` & `aws_console_url-0.7.6/Public-API.rst`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/README.rst` & `aws_console_url-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/console.py` & `aws_console_url-0.7.6/aws_console_url/console.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/model.py` & `aws_console_url-0.7.6/aws_console_url/model.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/resource.py` & `aws_console_url-0.7.6/aws_console_url/resource.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/a2i.py` & `aws_console_url-0.7.6/aws_console_url/srv/a2i.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,47 +19,54 @@
 @dataclasses.dataclass(frozen=True)
 class A2IHumanLoop(BaseSageMakerResource):
     _RESOURCE_TYPE = "human-loop"
 
 
 @dataclasses.dataclass(frozen=True)
 class A2I(Service):
-    _AWS_SERVICE = "a2i"
+    _AWS_SERVICE = "sagemaker/groundtruth"
 
     # --- Human Review Workflows
     @property
     def human_review_workflows(self) -> str:
         return (
-            f"{self._service_root}/home?region={self._region}#/human-review-workflows"
+            f"{self._service_root}?region={self._region}#/a2i/human-review-workflows"
         )
 
     def get_human_review_workflow_arn(self, name: str) -> str:
         return A2IFlowDefinition.make(self._account_id, self._region, name=name).arn
 
     def _human_review_workflow_arn_to_name(self, arn: str) -> str:
         return A2IFlowDefinition.from_arn(arn).name
 
     def get_human_review_workflow(self, name_or_arn: str) -> str:
         name = self._ensure_name(name_or_arn, self._human_review_workflow_arn_to_name)
-        return f"{self._service_root}/home?region={self._region}#/human-review-workflows/{name}"
+        return f"{self._service_root}?region={self._region}#/a2i/human-review-workflows/{name}"
 
     # --- Worker Task Templates
     @property
     def worker_task_templates(self) -> str:
-        return f"{self._service_root}/home?region={self._region}#/worker-task-templates"
+        return f"{self._service_root}?region={self._region}#/a2i/worker-task-templates"
 
     def get_worker_task_template_arn(self, name: str) -> str:
         return A2IHumanTaskUI.make(self._account_id, self._region, name=name).arn
 
     def _worker_task_template_arn_to_name(self, arn: str) -> str:
         return A2IHumanTaskUI.from_arn(arn).name
 
     def get_worker_task_template(self, name_or_arn: str) -> str:
         name = self._ensure_name(name_or_arn, self._worker_task_template_arn_to_name)
-        return f"{self._service_root}/home?region={self._region}#/worker-task-templates/{name}"
+        return f"{self._service_root}?region={self._region}#/a2i/worker-task-templates/{name}"
+
+    # --- Human review workforces
+    @property
+    def human_review_workforces(self) -> str:
+        return (
+            f"{self._service_root}?region={self._region}#/a2i/human-review-workforces"
+        )
 
     # --- Human Loop
     def get_human_loop_arn(self, name: str) -> str:
         return A2IHumanLoop.make(self._account_id, self._region, name=name).arn
 
     def _human_loop_arn_to_name(self, arn: str) -> str:
         return A2IHumanTaskUI.from_arn(arn).name
@@ -72,10 +79,10 @@
         flow_name = self._ensure_name(
             flow_name_or_arn, self._human_review_workflow_arn_to_name
         )
         human_loop_name = self._ensure_name(
             human_loop_name_or_arn, self._human_loop_arn_to_name
         )
         return (
-            f"{self._service_root}/home?region={self._region}#/human-review-workflows"
+            f"{self._service_root}?region={self._region}#/a2i/human-review-workflows"
             f"/{flow_name}/human-loops/{human_loop_name}"
         )
```

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/awslambda.py` & `aws_console_url-0.7.6/aws_console_url/srv/awslambda.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/cloudformation.py` & `aws_console_url-0.7.6/aws_console_url/srv/cloudformation.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/cloudwatch.py` & `aws_console_url-0.7.6/aws_console_url/srv/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/codebuild.py` & `aws_console_url-0.7.6/aws_console_url/srv/codebuild.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/codecommit.py` & `aws_console_url-0.7.6/aws_console_url/srv/codecommit.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/dynamodb.py` & `aws_console_url-0.7.6/aws_console_url/srv/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/ec2.py` & `aws_console_url-0.7.6/aws_console_url/srv/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/ecr.py` & `aws_console_url-0.7.6/aws_console_url/srv/ecr.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/glue.py` & `aws_console_url-0.7.6/aws_console_url/srv/glue.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/ground_truth.py` & `aws_console_url-0.7.6/aws_console_url/srv/ground_truth.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/iam.py` & `aws_console_url-0.7.6/aws_console_url/srv/iam.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/s3.py` & `aws_console_url-0.7.6/aws_console_url/srv/s3.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/sagemaker.py` & `aws_console_url-0.7.6/aws_console_url/srv/sagemaker.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/secretmanager.py` & `aws_console_url-0.7.6/aws_console_url/srv/secretmanager.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/sqs.py` & `aws_console_url-0.7.6/aws_console_url/srv/sqs.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/ssm.py` & `aws_console_url-0.7.6/aws_console_url/srv/ssm.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/step_function.py` & `aws_console_url-0.7.6/aws_console_url/srv/step_function.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/srv/vpc.py` & `aws_console_url-0.7.6/aws_console_url/srv/vpc.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url/tests/helper.py` & `aws_console_url-0.7.6/aws_console_url/tests/helper.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/aws_console_url.egg-info/PKG-INFO` & `aws_console_url-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: aws-console-url
-Version: 0.7.5
+Name: aws_console_url
+Version: 0.7.6
 Summary: Build AWS Console Url for debugging.
 Home-page: https://github.com/MacHu-GWU/aws_console_url-project
-Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.5#downloads
+Download-URL: https://pypi.python.org/pypi/aws_console_url/0.7.6#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_console_url-0.7.5/aws_console_url.egg-info/SOURCES.txt` & `aws_console_url-0.7.6/aws_console_url.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/release-history.rst` & `aws_console_url-0.7.6/release-history.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.7.6 (2023-07-10)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- AWS updates the augmented ai related url, so we fixed ``a2i`` related URL.
+
+
 0.7.5 (2023-05-10)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - add support to those resource name may have slash (SSM parameter)
```

### Comparing `aws_console_url-0.7.5/requirements-doc.txt` & `aws_console_url-0.7.6/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/setup.py` & `aws_console_url-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `aws_console_url-0.7.5/tests/test_import.py` & `aws_console_url-0.7.6/tests/test_import.py`

 * *Files identical despite different names*

