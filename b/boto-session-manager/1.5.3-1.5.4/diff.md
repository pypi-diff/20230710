# Comparing `tmp/boto_session_manager-1.5.3.tar.gz` & `tmp/boto_session_manager-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto_session_manager-1.5.3.tar", last modified: Fri May 26 02:46:52 2023, max compression
+gzip compressed data, was "boto_session_manager-1.5.4.tar", last modified: Mon Jul 10 20:01:16 2023, max compression
```

## Comparing `boto_session_manager-1.5.3.tar` & `boto_session_manager-1.5.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 02:46:52.553268 boto_session_manager-1.5.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      607 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)    11387 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      318 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     8872 2023-05-26 02:46:52.553069 boto_session_manager-1.5.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     7641 2023-05-11 21:55:49.000000 boto_session_manager-1.5.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 02:46:52.551487 boto_session_manager-1.5.3/boto_session_manager/
--rw-r--r--   0 sanhehu    (501) staff       (20)      803 2023-05-12 01:07:20.000000 boto_session_manager-1.5.3/boto_session_manager/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 02:15:49.000000 boto_session_manager-1.5.3/boto_session_manager/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)   113267 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/boto_session_manager/clients.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 02:46:52.552249 boto_session_manager-1.5.3/boto_session_manager/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/boto_session_manager/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       79 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/boto_session_manager/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    16756 2023-05-26 02:41:48.000000 boto_session_manager-1.5.3/boto_session_manager/manager.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2435 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/boto_session_manager/sentinel.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    11542 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/boto_session_manager/services.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 02:46:52.552125 boto_session_manager-1.5.3/boto_session_manager.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     8872 2023-05-26 02:46:52.000000 boto_session_manager-1.5.3/boto_session_manager.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      680 2023-05-26 02:46:52.000000 boto_session_manager-1.5.3/boto_session_manager.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 02:46:52.000000 boto_session_manager-1.5.3/boto_session_manager.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      190 2023-05-26 02:46:52.000000 boto_session_manager-1.5.3/boto_session_manager.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       21 2023-05-26 02:46:52.000000 boto_session_manager-1.5.3/boto_session_manager.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     4793 2023-05-26 02:44:04.000000 boto_session_manager-1.5.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      338 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      196 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        6 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 02:46:52.553319 boto_session_manager-1.5.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     5398 2023-05-11 21:23:12.000000 boto_session_manager-1.5.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 02:46:52.552742 boto_session_manager-1.5.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      309 2023-04-26 23:54:08.000000 boto_session_manager-1.5.3/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5930 2023-05-26 02:42:35.000000 boto_session_manager-1.5.3/tests/test_manager.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:01:16.175822 boto_session_manager-1.5.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      607 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11387 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      318 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8872 2023-07-10 20:01:16.175575 boto_session_manager-1.5.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7641 2023-05-11 21:55:49.000000 boto_session_manager-1.5.4/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:01:16.173693 boto_session_manager-1.5.4/boto_session_manager/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      803 2023-05-12 01:07:20.000000 boto_session_manager-1.5.4/boto_session_manager/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-10 19:57:20.000000 boto_session_manager-1.5.4/boto_session_manager/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)   116597 2023-07-10 19:56:47.000000 boto_session_manager-1.5.4/boto_session_manager/clients.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:01:16.174519 boto_session_manager-1.5.4/boto_session_manager/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/boto_session_manager/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       79 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/boto_session_manager/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16756 2023-05-26 02:41:48.000000 boto_session_manager-1.5.4/boto_session_manager/manager.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2435 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/boto_session_manager/sentinel.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11885 2023-07-10 19:52:16.000000 boto_session_manager-1.5.4/boto_session_manager/services.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:01:16.174385 boto_session_manager-1.5.4/boto_session_manager.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8872 2023-07-10 20:01:16.000000 boto_session_manager-1.5.4/boto_session_manager.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      680 2023-07-10 20:01:16.000000 boto_session_manager-1.5.4/boto_session_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-10 20:01:16.000000 boto_session_manager-1.5.4/boto_session_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      190 2023-07-10 20:01:16.000000 boto_session_manager-1.5.4/boto_session_manager.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       21 2023-07-10 20:01:16.000000 boto_session_manager-1.5.4/boto_session_manager.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5168 2023-07-10 19:59:20.000000 boto_session_manager-1.5.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      338 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      196 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        6 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-10 20:01:16.175884 boto_session_manager-1.5.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5398 2023-05-11 21:23:12.000000 boto_session_manager-1.5.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-10 20:01:16.175337 boto_session_manager-1.5.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      309 2023-04-26 23:54:08.000000 boto_session_manager-1.5.4/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5930 2023-05-26 02:42:35.000000 boto_session_manager-1.5.4/tests/test_manager.py
```

### Comparing `boto_session_manager-1.5.3/AUTHORS.rst` & `boto_session_manager-1.5.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/LICENSE.txt` & `boto_session_manager-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/PKG-INFO` & `boto_session_manager-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: boto_session_manager
-Version: 1.5.3
+Version: 1.5.4
 Summary: Provides an alternative, or maybe a more user friendly way to use the native boto3 API.
 Home-page: https://github.com/aws-samples/boto_session_manager-project
-Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.5.3#downloads
+Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.5.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: Apache License, Version 2.0
 Platform: Windows
 Platform: MacOS
```

### Comparing `boto_session_manager-1.5.3/README.rst` & `boto_session_manager-1.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/boto_session_manager/__init__.py` & `boto_session_manager-1.5.4/boto_session_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/boto_session_manager/clients.py` & `boto_session_manager-1.5.4/boto_session_manager/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     import mypy_boto3_amplifybackend
     import mypy_boto3_amplifyuibuilder
     import mypy_boto3_apigateway
     import mypy_boto3_apigatewaymanagementapi
     import mypy_boto3_apigatewayv2
     import mypy_boto3_appconfig
     import mypy_boto3_appconfigdata
+    import mypy_boto3_appfabric
     import mypy_boto3_appflow
     import mypy_boto3_appintegrations
     import mypy_boto3_application_autoscaling
     import mypy_boto3_application_insights
     import mypy_boto3_applicationcostprofiler
     import mypy_boto3_appmesh
     import mypy_boto3_apprunner
@@ -63,14 +64,15 @@
     import mypy_boto3_cloudwatch
     import mypy_boto3_codeartifact
     import mypy_boto3_codebuild
     import mypy_boto3_codecatalyst
     import mypy_boto3_codecommit
     import mypy_boto3_codedeploy
     import mypy_boto3_codeguru_reviewer
+    import mypy_boto3_codeguru_security
     import mypy_boto3_codeguruprofiler
     import mypy_boto3_codepipeline
     import mypy_boto3_codestar
     import mypy_boto3_codestar_connections
     import mypy_boto3_codestar_notifications
     import mypy_boto3_cognito_identity
     import mypy_boto3_cognito_idp
@@ -168,14 +170,15 @@
     import mypy_boto3_iotfleetwise
     import mypy_boto3_iotsecuretunneling
     import mypy_boto3_iotsitewise
     import mypy_boto3_iotthingsgraph
     import mypy_boto3_iottwinmaker
     import mypy_boto3_iotwireless
     import mypy_boto3_ivs
+    import mypy_boto3_ivs_realtime
     import mypy_boto3_ivschat
     import mypy_boto3_kafka
     import mypy_boto3_kafkaconnect
     import mypy_boto3_kendra
     import mypy_boto3_kendra_ranking
     import mypy_boto3_keyspaces
     import mypy_boto3_kinesis
@@ -211,14 +214,15 @@
     import mypy_boto3_marketplace_entitlement
     import mypy_boto3_marketplacecommerceanalytics
     import mypy_boto3_mediaconnect
     import mypy_boto3_mediaconvert
     import mypy_boto3_medialive
     import mypy_boto3_mediapackage
     import mypy_boto3_mediapackage_vod
+    import mypy_boto3_mediapackagev2
     import mypy_boto3_mediastore
     import mypy_boto3_mediastore_data
     import mypy_boto3_mediatailor
     import mypy_boto3_memorydb
     import mypy_boto3_meteringmarketplace
     import mypy_boto3_mgh
     import mypy_boto3_mgn
@@ -237,16 +241,19 @@
     import mypy_boto3_oam
     import mypy_boto3_omics
     import mypy_boto3_opensearch
     import mypy_boto3_opensearchserverless
     import mypy_boto3_opsworks
     import mypy_boto3_opsworkscm
     import mypy_boto3_organizations
+    import mypy_boto3_osis
     import mypy_boto3_outposts
     import mypy_boto3_panorama
+    import mypy_boto3_payment_cryptography
+    import mypy_boto3_payment_cryptography_data
     import mypy_boto3_personalize
     import mypy_boto3_personalize_events
     import mypy_boto3_personalize_runtime
     import mypy_boto3_pi
     import mypy_boto3_pinpoint
     import mypy_boto3_pinpoint_email
     import mypy_boto3_pinpoint_sms_voice
@@ -304,15 +311,14 @@
     import mypy_boto3_servicediscovery
     import mypy_boto3_ses
     import mypy_boto3_sesv2
     import mypy_boto3_shield
     import mypy_boto3_signer
     import mypy_boto3_simspaceweaver
     import mypy_boto3_sms
-    import mypy_boto3_sms_voice
     import mypy_boto3_snow_device_management
     import mypy_boto3_snowball
     import mypy_boto3_sns
     import mypy_boto3_sqs
     import mypy_boto3_ssm
     import mypy_boto3_ssm_contacts
     import mypy_boto3_ssm_incidents
@@ -330,15 +336,17 @@
     import mypy_boto3_textract
     import mypy_boto3_timestream_query
     import mypy_boto3_timestream_write
     import mypy_boto3_tnb
     import mypy_boto3_transcribe
     import mypy_boto3_transfer
     import mypy_boto3_translate
+    import mypy_boto3_verifiedpermissions
     import mypy_boto3_voice_id
+    import mypy_boto3_vpc_lattice
     import mypy_boto3_waf
     import mypy_boto3_waf_regional
     import mypy_boto3_wafv2
     import mypy_boto3_wellarchitected
     import mypy_boto3_wisdom
     import mypy_boto3_workdocs
     import mypy_boto3_worklink
@@ -445,14 +453,21 @@
     def appconfigdata_client(self: "BotoSesManager") -> "mypy_boto3_appconfigdata.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html
         """
         return self.get_client(AwsServiceEnum.AppConfigData)
     
     @property
+    def appfabric_client(self: "BotoSesManager") -> "mypy_boto3_appfabric.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html
+        """
+        return self.get_client(AwsServiceEnum.AppFabric)
+    
+    @property
     def appflow_client(self: "BotoSesManager") -> "mypy_boto3_appflow.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html
         """
         return self.get_client(AwsServiceEnum.Appflow)
     
     @property
@@ -774,14 +789,21 @@
     def codegurureviewer_client(self: "BotoSesManager") -> "mypy_boto3_codeguru_reviewer.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html
         """
         return self.get_client(AwsServiceEnum.CodeGuruReviewer)
     
     @property
+    def codegurusecurity_client(self: "BotoSesManager") -> "mypy_boto3_codeguru_security.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html
+        """
+        return self.get_client(AwsServiceEnum.CodeGuruSecurity)
+    
+    @property
     def codeguruprofiler_client(self: "BotoSesManager") -> "mypy_boto3_codeguruprofiler.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html
         """
         return self.get_client(AwsServiceEnum.CodeGuruProfiler)
     
     @property
@@ -1509,14 +1531,21 @@
     def ivs_client(self: "BotoSesManager") -> "mypy_boto3_ivs.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html
         """
         return self.get_client(AwsServiceEnum.IVS)
     
     @property
+    def ivsrealtime_client(self: "BotoSesManager") -> "mypy_boto3_ivs_realtime.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html
+        """
+        return self.get_client(AwsServiceEnum.ivsrealtime)
+    
+    @property
     def ivschat_client(self: "BotoSesManager") -> "mypy_boto3_ivschat.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html
         """
         return self.get_client(AwsServiceEnum.ivschat)
     
     @property
@@ -1810,14 +1839,21 @@
     def mediapackagevod_client(self: "BotoSesManager") -> "mypy_boto3_mediapackage_vod.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html
         """
         return self.get_client(AwsServiceEnum.MediaPackageVod)
     
     @property
+    def mediapackagev2_client(self: "BotoSesManager") -> "mypy_boto3_mediapackagev2.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html
+        """
+        return self.get_client(AwsServiceEnum.mediapackagev2)
+    
+    @property
     def mediastore_client(self: "BotoSesManager") -> "mypy_boto3_mediastore.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html
         """
         return self.get_client(AwsServiceEnum.MediaStore)
     
     @property
@@ -1992,28 +2028,49 @@
     def organizations_client(self: "BotoSesManager") -> "mypy_boto3_organizations.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html
         """
         return self.get_client(AwsServiceEnum.Organizations)
     
     @property
+    def opensearchingestion_client(self: "BotoSesManager") -> "mypy_boto3_osis.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html
+        """
+        return self.get_client(AwsServiceEnum.OpenSearchIngestion)
+    
+    @property
     def outposts_client(self: "BotoSesManager") -> "mypy_boto3_outposts.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html
         """
         return self.get_client(AwsServiceEnum.Outposts)
     
     @property
     def panorama_client(self: "BotoSesManager") -> "mypy_boto3_panorama.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html
         """
         return self.get_client(AwsServiceEnum.Panorama)
     
     @property
+    def paymentcryptographycontrolplane_client(self: "BotoSesManager") -> "mypy_boto3_payment_cryptography.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html
+        """
+        return self.get_client(AwsServiceEnum.PaymentCryptographyControlPlane)
+    
+    @property
+    def paymentcryptographydataplane_client(self: "BotoSesManager") -> "mypy_boto3_payment_cryptography_data.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html
+        """
+        return self.get_client(AwsServiceEnum.PaymentCryptographyDataPlane)
+    
+    @property
     def personalize_client(self: "BotoSesManager") -> "mypy_boto3_personalize.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html
         """
         return self.get_client(AwsServiceEnum.Personalize)
     
     @property
@@ -2461,21 +2518,14 @@
     def sms_client(self: "BotoSesManager") -> "mypy_boto3_sms.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html
         """
         return self.get_client(AwsServiceEnum.SMS)
     
     @property
-    def pinpointsmsvoice_client(self: "BotoSesManager") -> "mypy_boto3_sms_voice.Client":
-        """
-        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html
-        """
-        return self.get_client(AwsServiceEnum.PinpointSMSVoice)
-    
-    @property
     def snowdevicemanagement_client(self: "BotoSesManager") -> "mypy_boto3_snow_device_management.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html
         """
         return self.get_client(AwsServiceEnum.SnowDeviceManagement)
     
     @property
@@ -2643,21 +2693,35 @@
     def translate_client(self: "BotoSesManager") -> "mypy_boto3_translate.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html
         """
         return self.get_client(AwsServiceEnum.Translate)
     
     @property
+    def verifiedpermissions_client(self: "BotoSesManager") -> "mypy_boto3_verifiedpermissions.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html
+        """
+        return self.get_client(AwsServiceEnum.VerifiedPermissions)
+    
+    @property
     def voiceid_client(self: "BotoSesManager") -> "mypy_boto3_voice_id.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html
         """
         return self.get_client(AwsServiceEnum.VoiceID)
     
     @property
+    def vpclattice_client(self: "BotoSesManager") -> "mypy_boto3_vpc_lattice.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html
+        """
+        return self.get_client(AwsServiceEnum.VPCLattice)
+    
+    @property
     def waf_client(self: "BotoSesManager") -> "mypy_boto3_waf.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html
         """
         return self.get_client(AwsServiceEnum.WAF)
     
     @property
@@ -2732,8 +2796,17 @@
     
     @property
     def xray_client(self: "BotoSesManager") -> "mypy_boto3_xray.Client":
         """
         Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html
         """
         return self.get_client(AwsServiceEnum.XRay)
-    
+
+    # --------------------------------------------------------------------------
+    # for backward compatibility
+    # --------------------------------------------------------------------------
+    @property
+    def sagemaker_a2i_runtime_client(self: "BotoSesManager") -> "mypy_boto3_sagemaker_a2i_runtime.Client":
+        """
+        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html
+        """
+        return self.augmentedairuntime_client
```

### Comparing `boto_session_manager-1.5.3/boto_session_manager/manager.py` & `boto_session_manager-1.5.4/boto_session_manager/manager.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/boto_session_manager/sentinel.py` & `boto_session_manager-1.5.4/boto_session_manager/sentinel.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/boto_session_manager/services.py` & `boto_session_manager-1.5.4/boto_session_manager/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     AmplifyBackend = "amplifybackend"
     AmplifyUIBuilder = "amplifyuibuilder"
     APIGateway = "apigateway"
     ApiGatewayManagementApi = "apigatewaymanagementapi"
     ApiGatewayV2 = "apigatewayv2"
     AppConfig = "appconfig"
     AppConfigData = "appconfigdata"
+    AppFabric = "appfabric"
     Appflow = "appflow"
     AppIntegrationsService = "appintegrations"
     ApplicationAutoScaling = "application-autoscaling"
     ApplicationInsights = "application-insights"
     ApplicationCostProfiler = "applicationcostprofiler"
     AppMesh = "appmesh"
     AppRunner = "apprunner"
@@ -59,14 +60,15 @@
     CloudWatch = "cloudwatch"
     CodeArtifact = "codeartifact"
     CodeBuild = "codebuild"
     CodeCatalyst = "codecatalyst"
     CodeCommit = "codecommit"
     CodeDeploy = "codedeploy"
     CodeGuruReviewer = "codeguru-reviewer"
+    CodeGuruSecurity = "codeguru-security"
     CodeGuruProfiler = "codeguruprofiler"
     CodePipeline = "codepipeline"
     CodeStar = "codestar"
     CodeStarconnections = "codestar-connections"
     CodeStarNotifications = "codestar-notifications"
     CognitoIdentity = "cognito-identity"
     CognitoIdentityProvider = "cognito-idp"
@@ -164,14 +166,15 @@
     IoTFleetWise = "iotfleetwise"
     IoTSecureTunneling = "iotsecuretunneling"
     IoTSiteWise = "iotsitewise"
     IoTThingsGraph = "iotthingsgraph"
     IoTTwinMaker = "iottwinmaker"
     IoTWireless = "iotwireless"
     IVS = "ivs"
+    ivsrealtime = "ivs-realtime"
     ivschat = "ivschat"
     Kafka = "kafka"
     KafkaConnect = "kafkaconnect"
     kendra = "kendra"
     KendraRanking = "kendra-ranking"
     Keyspaces = "keyspaces"
     Kinesis = "kinesis"
@@ -207,14 +210,15 @@
     MarketplaceEntitlementService = "marketplace-entitlement"
     MarketplaceCommerceAnalytics = "marketplacecommerceanalytics"
     MediaConnect = "mediaconnect"
     MediaConvert = "mediaconvert"
     MediaLive = "medialive"
     MediaPackage = "mediapackage"
     MediaPackageVod = "mediapackage-vod"
+    mediapackagev2 = "mediapackagev2"
     MediaStore = "mediastore"
     MediaStoreData = "mediastore-data"
     MediaTailor = "mediatailor"
     MemoryDB = "memorydb"
     MarketplaceMetering = "meteringmarketplace"
     MigrationHub = "mgh"
     mgn = "mgn"
@@ -233,16 +237,19 @@
     CloudWatchObservabilityAccessManager = "oam"
     Omics = "omics"
     OpenSearchService = "opensearch"
     OpenSearchServiceServerless = "opensearchserverless"
     OpsWorks = "opsworks"
     OpsWorksCM = "opsworkscm"
     Organizations = "organizations"
+    OpenSearchIngestion = "osis"
     Outposts = "outposts"
     Panorama = "panorama"
+    PaymentCryptographyControlPlane = "payment-cryptography"
+    PaymentCryptographyDataPlane = "payment-cryptography-data"
     Personalize = "personalize"
     PersonalizeEvents = "personalize-events"
     PersonalizeRuntime = "personalize-runtime"
     PI = "pi"
     Pinpoint = "pinpoint"
     PinpointEmail = "pinpoint-email"
     PinpointSMSVoice = "pinpoint-sms-voice"
@@ -300,15 +307,14 @@
     ServiceDiscovery = "servicediscovery"
     SES = "ses"
     SESV2 = "sesv2"
     Shield = "shield"
     signer = "signer"
     SimSpaceWeaver = "simspaceweaver"
     SMS = "sms"
-    PinpointSMSVoice = "sms-voice"
     SnowDeviceManagement = "snow-device-management"
     Snowball = "snowball"
     SNS = "sns"
     SQS = "sqs"
     SSM = "ssm"
     SSMContacts = "ssm-contacts"
     SSMIncidents = "ssm-incidents"
@@ -326,15 +332,17 @@
     Textract = "textract"
     TimestreamQuery = "timestream-query"
     TimestreamWrite = "timestream-write"
     TelcoNetworkBuilder = "tnb"
     TranscribeService = "transcribe"
     Transfer = "transfer"
     Translate = "translate"
+    VerifiedPermissions = "verifiedpermissions"
     VoiceID = "voice-id"
+    VPCLattice = "vpc-lattice"
     WAF = "waf"
     WAFRegional = "waf-regional"
     WAFV2 = "wafv2"
     WellArchitected = "wellarchitected"
     ConnectWisdomService = "wisdom"
     WorkDocs = "workdocs"
     WorkLink = "worklink"
```

### Comparing `boto_session_manager-1.5.3/boto_session_manager.egg-info/PKG-INFO` & `boto_session_manager-1.5.4/boto_session_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: boto-session-manager
-Version: 1.5.3
+Version: 1.5.4
 Summary: Provides an alternative, or maybe a more user friendly way to use the native boto3 API.
 Home-page: https://github.com/aws-samples/boto_session_manager-project
-Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.5.3#downloads
+Download-URL: https://pypi.python.org/pypi/boto_session_manager/1.5.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: Apache License, Version 2.0
 Platform: Windows
 Platform: MacOS
```

### Comparing `boto_session_manager-1.5.3/boto_session_manager.egg-info/SOURCES.txt` & `boto_session_manager-1.5.4/boto_session_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/release-history.rst` & `boto_session_manager-1.5.4/release-history.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+1.5.4 (2023-07-14)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- AWS occasionally updates the boto3 client name on their website, making some of the old ``bsm.${service_name}_client`` unavailable. We add alias for those old service name to maintain backward compatibility.
+- Add ``sagemaker_a2i_runtime_client`` alias.
+
+
 1.5.3 (2023-05-25)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix bug that the :meth:`~boto_session_manager.manager.BotoSesManager.awscli` method doesn't work properly when using profile name, or using IAM role on EC2, lambda, etc...
```

### Comparing `boto_session_manager-1.5.3/requirements-doc.txt` & `boto_session_manager-1.5.4/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/setup.py` & `boto_session_manager-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `boto_session_manager-1.5.3/tests/test_manager.py` & `boto_session_manager-1.5.4/tests/test_manager.py`

 * *Files identical despite different names*

