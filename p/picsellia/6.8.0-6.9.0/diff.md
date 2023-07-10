# Comparing `tmp/picsellia-6.8.0.tar.gz` & `tmp/picsellia-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picsellia-6.8.0.tar", max compression
+gzip compressed data, was "picsellia-6.9.0.tar", max compression
```

## Comparing `picsellia-6.8.0.tar` & `picsellia-6.9.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0    11046 2023-06-16 13:11:39.208475 picsellia-6.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.8.0/LICENSE
--rw-r--r--   0        0        0     1660 2023-05-10 08:40:15.009117 picsellia-6.8.0/README.md
--rw-r--r--   0        0        0     2590 2023-06-16 13:11:39.208475 picsellia-6.8.0/picsellia/__init__.py
--rw-r--r--   0        0        0    38919 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/client.py
--rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.8.0/picsellia/colors.py
--rw-r--r--   0        0        0     1706 2023-05-10 08:40:15.013117 picsellia-6.8.0/picsellia/decorators.py
--rw-r--r--   0        0        0     4918 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/exceptions.py
--rw-r--r--   0        0        0     3410 2023-05-10 08:40:15.013117 picsellia-6.8.0/picsellia/pxl_multithreading.py
--rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.8.0/picsellia/sdk/__init__.py
--rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.8.0/picsellia/sdk/annotation.py
--rw-r--r--   0        0        0     3227 2023-05-10 08:40:15.013117 picsellia-6.8.0/picsellia/sdk/artifact.py
--rw-r--r--   0        0        0    17063 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/sdk/asset.py
--rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.8.0/picsellia/sdk/classification.py
--rw-r--r--   0        0        0    19558 2023-06-16 07:22:12.477468 picsellia-6.8.0/picsellia/sdk/connexion.py
--rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.8.0/picsellia/sdk/dao.py
--rw-r--r--   0        0        0     9259 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/sdk/data.py
--rw-r--r--   0        0        0    18002 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/sdk/datalake.py
--rw-r--r--   0        0        0     7203 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/dataset.py
--rw-r--r--   0        0        0    60790 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/sdk/dataset_version.py
--rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.8.0/picsellia/sdk/datasource.py
--rw-r--r--   0        0        0    37431 2023-05-16 15:31:25.511144 picsellia-6.8.0/picsellia/sdk/deployment.py
--rw-r--r--   0        0        0     3485 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/downloadable.py
--rw-r--r--   0        0        0     4219 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/evaluation.py
--rw-r--r--   0        0        0    40734 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/sdk/experiment.py
--rw-r--r--   0        0        0     8130 2023-06-16 13:05:20.597718 picsellia-6.8.0/picsellia/sdk/job.py
--rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/label.py
--rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/line.py
--rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/log.py
--rw-r--r--   0        0        0     2872 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/logging_file.py
--rw-r--r--   0        0        0     8681 2023-06-16 07:21:46.345339 picsellia-6.8.0/picsellia/sdk/model.py
--rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/model_context.py
--rw-r--r--   0        0        0     2311 2023-05-10 08:40:15.017117 picsellia-6.8.0/picsellia/sdk/model_file.py
--rw-r--r--   0        0        0    12878 2023-06-16 07:21:46.349339 picsellia-6.8.0/picsellia/sdk/model_version.py
--rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.8.0/picsellia/sdk/multi_object.py
--rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/point.py
--rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.8.0/picsellia/sdk/polygon.py
--rw-r--r--   0        0        0    16844 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/sdk/project.py
--rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/rectangle.py
--rw-r--r--   0        0        0     5374 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/run.py
--rw-r--r--   0        0        0     6923 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/sdk/scan.py
--rw-r--r--   0        0        0     3103 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/sdk/scan_file.py
--rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/tag.py
--rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/taggable.py
--rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/sdk/worker.py
--rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/services/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/asset_splitter.py
--rw-r--r--   0        0        0     5988 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/services/coco_file_builder.py
--rw-r--r--   0        0        0     3558 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/coco_importer.py
--rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.8.0/picsellia/services/datasource.py
--rw-r--r--   0        0        0      798 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/error_manager.py
--rw-r--r--   0        0        0      974 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/splitter.py
--rw-r--r--   0        0        0     2658 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/voc_importer.py
--rw-r--r--   0        0        0     8268 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/services/yolo_importer.py
--rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.8.0/picsellia/types/__init__.py
--rw-r--r--   0        0        0     4572 2023-06-16 07:21:46.349339 picsellia-6.8.0/picsellia/types/enums.py
--rw-r--r--   0        0        0     4588 2023-06-16 13:11:15.864325 picsellia-6.8.0/picsellia/types/schemas.py
--rw-r--r--   0        0        0     3658 2023-05-10 08:40:15.021117 picsellia-6.8.0/picsellia/types/schemas_prediction.py
--rw-r--r--   0        0        0     8498 2023-05-10 08:40:15.025117 picsellia-6.8.0/picsellia/utils.py
--rw-r--r--   0        0        0     1368 2023-06-16 13:11:39.208475 picsellia-6.8.0/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.8.0/setup.py
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11678 2023-07-10 14:26:30.067305 picsellia-6.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.9.0/LICENSE
+-rw-r--r--   0        0        0     1660 2023-05-10 08:40:15.009117 picsellia-6.9.0/README.md
+-rw-r--r--   0        0        0     2590 2023-07-10 14:26:30.067305 picsellia-6.9.0/picsellia/__init__.py
+-rw-r--r--   0        0        0    39378 2023-07-10 14:02:19.237641 picsellia-6.9.0/picsellia/client.py
+-rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.9.0/picsellia/colors.py
+-rw-r--r--   0        0        0     1706 2023-05-10 08:40:15.013117 picsellia-6.9.0/picsellia/decorators.py
+-rw-r--r--   0        0        0     4918 2023-06-16 13:05:20.597718 picsellia-6.9.0/picsellia/exceptions.py
+-rw-r--r--   0        0        0     3342 2023-07-10 14:02:19.237641 picsellia-6.9.0/picsellia/exif.py
+-rw-r--r--   0        0        0     3410 2023-05-10 08:40:15.013117 picsellia-6.9.0/picsellia/pxl_multithreading.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.9.0/picsellia/sdk/__init__.py
+-rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.9.0/picsellia/sdk/annotation.py
+-rw-r--r--   0        0        0     3227 2023-05-10 08:40:15.013117 picsellia-6.9.0/picsellia/sdk/artifact.py
+-rw-r--r--   0        0        0    17063 2023-06-16 13:11:15.864325 picsellia-6.9.0/picsellia/sdk/asset.py
+-rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.9.0/picsellia/sdk/classification.py
+-rw-r--r--   0        0        0    19558 2023-06-16 07:22:12.477468 picsellia-6.9.0/picsellia/sdk/connexion.py
+-rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.9.0/picsellia/sdk/dao.py
+-rw-r--r--   0        0        0     9259 2023-06-16 13:11:15.864325 picsellia-6.9.0/picsellia/sdk/data.py
+-rw-r--r--   0        0        0    18388 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/datalake.py
+-rw-r--r--   0        0        0     7203 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/dataset.py
+-rw-r--r--   0        0        0    60790 2023-07-06 07:37:34.607828 picsellia-6.9.0/picsellia/sdk/dataset_version.py
+-rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.9.0/picsellia/sdk/datasource.py
+-rw-r--r--   0        0        0    38557 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/deployment.py
+-rw-r--r--   0        0        0     3485 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/downloadable.py
+-rw-r--r--   0        0        0     4219 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/evaluation.py
+-rw-r--r--   0        0        0    40734 2023-06-21 12:38:00.020248 picsellia-6.9.0/picsellia/sdk/experiment.py
+-rw-r--r--   0        0        0     8130 2023-06-16 13:05:20.597718 picsellia-6.9.0/picsellia/sdk/job.py
+-rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/label.py
+-rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/line.py
+-rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/log.py
+-rw-r--r--   0        0        0     2872 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/logging_file.py
+-rw-r--r--   0        0        0     8755 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/model.py
+-rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/model_context.py
+-rw-r--r--   0        0        0     2311 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/model_file.py
+-rw-r--r--   0        0        0    12952 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/model_version.py
+-rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.9.0/picsellia/sdk/multi_object.py
+-rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/point.py
+-rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/polygon.py
+-rw-r--r--   0        0        0    16844 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/sdk/project.py
+-rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/rectangle.py
+-rw-r--r--   0        0        0     5374 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/run.py
+-rw-r--r--   0        0        0     6923 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/sdk/scan.py
+-rw-r--r--   0        0        0     3103 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/sdk/scan_file.py
+-rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/tag.py
+-rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/taggable.py
+-rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/worker.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/services/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/asset_splitter.py
+-rw-r--r--   0        0        0     5988 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/services/coco_file_builder.py
+-rw-r--r--   0        0        0     3558 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/coco_importer.py
+-rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/services/datasource.py
+-rw-r--r--   0        0        0      798 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/error_manager.py
+-rw-r--r--   0        0        0      974 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/splitter.py
+-rw-r--r--   0        0        0     2658 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/voc_importer.py
+-rw-r--r--   0        0        0     8268 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/yolo_importer.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.9.0/picsellia/types/__init__.py
+-rw-r--r--   0        0        0     4572 2023-06-16 07:21:46.349339 picsellia-6.9.0/picsellia/types/enums.py
+-rw-r--r--   0        0        0     4588 2023-06-16 13:11:15.864325 picsellia-6.9.0/picsellia/types/schemas.py
+-rw-r--r--   0        0        0     3658 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/types/schemas_prediction.py
+-rw-r--r--   0        0        0     7735 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-10 14:26:30.067305 picsellia-6.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.9.0/setup.py
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.9.0/PKG-INFO
```

### Comparing `picsellia-6.8.0/CHANGELOG.md` & `picsellia-6.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 
 # Changelog
 
 Picsellia SDK Python is a library that allows users to connect to Picsellia backend.
 
 All notable changes to this project will be documented in this file.
 
+## [6.9.0] - 2023-07-10
+
+### Added
+- `Datalake.upload()` can now be called with parameter `fill_metadata`. On upload, set this parameter to True to read exif metadata flags and push metadata to Picsellia. By default, `fill_metadata` is False.
+- `Client.get_datalake()` can now be called with parameter `id` or `name` to retrieve the Datalake you want. If nothing is given, this method will retrieve your default datalake.
+- `Deployment.predict_bytes()` can now be called if you want to send image as bytes on Serving service
+- `ModelVersion.update()` and `Model.create_version()` can now be called with `docker_tag` parameter
+
+
 ## [6.8.0] - 2023-06-12
 
 ### Added
 - `Datalake.upload_data()` now accept parameter `metadata` which is a dict (or a list of dict if there are multiple filepaths) matching common metadata allowed by Picsellia.
 - `DatasetVersion.fork()` can now be called with parameters `with_annotations` and `with_labels` as web application
 - `DatasetVersion.export_annotation_file()` can now be called with `AnnotationFileType.YOLO` to retrieve a zip with yolo files
-- `Dataset.create_model` and `DatasetVersion.update` have parameter `description` to update description of a ModelVersion
+- `Dataset.create_model()` and `DatasetVersion.update()` have parameter `description` to update description of a ModelVersion
 
 
 ### Fixed
 - When adding evaluation, allow empty list to be sent as a list of shape
 
 ## [6.7.1] - 2023-05-15
 Some changes on `monitor()` following an update of our monitoring stack.
```

### Comparing `picsellia-6.8.0/LICENSE` & `picsellia-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/README.md` & `picsellia-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/__init__.py` & `picsellia-6.9.0/picsellia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "6.8.0"
+__version__ = "6.9.0"
 
 import logging.config
 import os
 
 from picsellia.client import Client
 from picsellia.sdk.annotation import Annotation
 from picsellia.sdk.artifact import Artifact
```

### Comparing `picsellia-6.8.0/picsellia/client.py` & `picsellia-6.9.0/picsellia/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,27 +172,39 @@
             Url on Platform for this resource
         """
 
         return f"{self.connexion.host}/organization/{self.id}"
 
     @exception_handler
     @beartype
-    def get_datalake(self) -> Datalake:
-        """Retrieve default datalake of this organization
+    def get_datalake(
+        self, id: Optional[Union[str, UUID]] = None, name: Optional[str] = None
+    ) -> Datalake:
+        """Retrieve a datalake of your organization.
+        By default, is nothing is given, this will return your default datalake.
 
         Examples:
             ```python
             datalake = client.get_datalake()
+            datalake = client.get_datalake(name="default")
+            datalake = client.get_datalake(id="0188e773-db65-7546-8e3e-b38fe5bed6d2")
             ```
 
         Returns:
             The (Datalake) of the client that you are using
         """
-        # Retrieve default datalake
-        r = self.connexion.get(f"/sdk/organization/{self.id}/datalake").json()
+        params = {}
+        if id:
+            params["id"] = UUID(id) if isinstance(id, str) else id
+        elif name:
+            params["name"] = name
+
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/datalake", params=params
+        ).json()
 
         return Datalake(self.connexion, self.id, r)
 
     @exception_handler
     @beartype
     def list_datalakes(self) -> List[Datalake]:
         """Retrieve all datalakes linked to this organization
```

### Comparing `picsellia-6.8.0/picsellia/decorators.py` & `picsellia-6.9.0/picsellia/decorators.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/exceptions.py` & `picsellia-6.9.0/picsellia/exceptions.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/pxl_multithreading.py` & `picsellia-6.9.0/picsellia/pxl_multithreading.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/annotation.py` & `picsellia-6.9.0/picsellia/sdk/annotation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/artifact.py` & `picsellia-6.9.0/picsellia/sdk/artifact.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/asset.py` & `picsellia-6.9.0/picsellia/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/classification.py` & `picsellia-6.9.0/picsellia/sdk/classification.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/connexion.py` & `picsellia-6.9.0/picsellia/sdk/connexion.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/dao.py` & `picsellia-6.9.0/picsellia/sdk/dao.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/data.py` & `picsellia-6.9.0/picsellia/sdk/data.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/datalake.py` & `picsellia-6.9.0/picsellia/sdk/datalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 from picsellia.exceptions import (
     BadRequestError,
     NoConnectorFound,
     NoDataError,
     NothingDoneError,
     UploadError,
 )
+from picsellia.exif import read_image_metadata
 from picsellia.sdk.connexion import Connexion
 from picsellia.sdk.dao import Dao
 from picsellia.sdk.data import Data, MultiData
 from picsellia.sdk.datasource import DataSource
 from picsellia.sdk.tag import Tag
 from picsellia.services.datasource import DataSourceService
 from picsellia.services.error_manager import ErrorManager
 from picsellia.types.enums import DataType, TagTarget
 from picsellia.types.schemas import DatalakeSchema
 from picsellia.utils import (
     combine_two_ql,
     convert_tag_list_to_query_language,
     filter_payload,
-    get_image_shape_with_exif_transpose,
 )
 
 logger = logging.getLogger("picsellia")
 warnings.filterwarnings("ignore", category=BeartypeDecorHintPep585DeprecationWarning)
 
 
 class Datalake(Dao):
@@ -104,14 +104,15 @@
         self,
         filepaths: Union[str, Path, List[Union[str, Path]]],
         tags: Optional[List[Union[str, Tag]]] = None,
         source: Union[str, DataSource, None] = None,
         max_workers: Optional[int] = None,
         error_manager: Optional[ErrorManager] = None,
         metadata: Union[None, Dict, List[Dict]] = None,
+        fill_metadata: Optional[bool] = False,
     ) -> Union[Data, MultiData]:
         """Upload data into this datalake.
 
         Upload files representing data, into a datalake.
         You can give some tags as a list.
         You can give a source for your data.
 
@@ -125,15 +126,15 @@
             tag_car = client.get_data_tag("car")
             tag_huge_car = client.get_data_tag("huge-car")
             source_camera_one = client.get_datasource("camera-one")
             source_camera_two = client.get_datasource("camera-two")
 
             lake = client.get_datalake()
             lake.upload_data(filepaths=["porsche.png", "ferrari.png"], tags=[tag_car], source=source_camera_one)
-            lake.upload_data(filepaths="truck.png", tags=[tag_huge_car], source=source_camera_two, metadata={"longitude": 43.6027273, "latitude": 1.4541129})
+            lake.upload_data(filepaths="truck.png", tags=[tag_huge_car], source=source_camera_two, metadata={"longitude": 43.6027273, "latitude": 1.4541129}, fill_metadata=True)
 
 
             error_manager = ErrorManager()
             lake.upload_data(filepaths=["twingo.png", "path/unknown.png", error_manager=error_manager)
 
             # This call will return a list of UploadError to see what was wrong
             error_paths = [error.path for error in error_manager.errors]
@@ -142,14 +143,16 @@
             filepaths (str or Path or List[str or Path]): Filepaths of your data
             tags (List[Tag], optional): Data Tags that will be given to data. Defaults to [].
             source (DataSource, optional): Source of your data.
             max_workers (int, optional): Number of max workers used to upload. Defaults to os.cpu_count() + 4.
             error_manager (ErrorManager, optional): Giving an ErrorManager will allow you to retrieve errors
             metadata (Dict or List[Dict], optional): Add some metadata to given data, filepaths length must match
                  this parameter. Defaults to no metadata.
+            fill_metadata (bool, optional): Whether or not read exif tags of image and add it into metadata field.
+                 If some fields are already given in metadata fields, they will be override.
 
         Returns:
             A (Data) object or a (MultiData) object that wraps a list of Data.
         """
         computed_tags_ids = []
         if tags:
             for tag in tags:
@@ -189,28 +192,30 @@
                     filename, self.connector_id
                 )
                 _, _, content_type = self.connexion.upload_file(
                     object_name, path, connector_id=self.connector_id
                 )
 
                 with Image.open(path) as image:
-                    width, height = get_image_shape_with_exif_transpose(image)
+                    image_metadatum = read_image_metadata(
+                        image, metadatum, fill_metadata
+                    )
 
                 payload = {
                     "type": DataType.IMAGE,
                     "filename": filename,
                     "object_name": object_name,
                     "content_type": content_type,
                     "meta": {
-                        "height": height,
-                        "width": width,
+                        "height": image_metadatum.height,
+                        "width": image_metadatum.width,
                     },
                     "tags": computed_tags_ids,
                     "data_source_id": source.id if source else None,
-                    "metadata": metadatum,
+                    "metadata": image_metadatum.metadata,
                 }
 
                 r = self.connexion.post(
                     f"/sdk/datalake/{self.id}/datas",
                     data=orjson.dumps(payload),
                 ).json()
                 return Data(self.connexion, self.id, r)
```

### Comparing `picsellia-6.8.0/picsellia/sdk/dataset.py` & `picsellia-6.9.0/picsellia/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/dataset_version.py` & `picsellia-6.9.0/picsellia/sdk/dataset_version.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/datasource.py` & `picsellia-6.9.0/picsellia/sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/deployment.py` & `picsellia-6.9.0/picsellia/sdk/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,17 +307,48 @@
             ```python
             deployment = client.get_deployment(
                 name="awesome-deploy"
             )
             deployment.predict('image_420.png', tags=["gonna", "give"], source="camera-1")
             ```
         Arguments:
-            tags (str, (Tag), list of str or Tag, optional): a list of tag to add to the data that will be created on the platform
+            file_path (str or Path): path to the image to predict.
+            tags (str, (Tag), list of str or Tag, optional): a list of tag to add to the data that will be created on the platform.
+            source (str or DataSource, optional): a source to attach to the data that will be created on the platform.
+
+        Returns:
+            A (dict) with information of the prediction
+        """
+        with open(file_path, "rb") as file:
+            file_data = file.read()
+            return self.predict_bytes(raw_image=file_data, tags=tags, source=source)
+
+    @exception_handler
+    @beartype
+    def predict_bytes(
+        self,
+        raw_image: bytes,
+        tags: Union[str, Tag, List[Union[Tag, str]], None] = None,
+        source: Union[str, DataSource, None] = None,
+    ) -> dict:
+        """Run a prediction on our Serving platform
+
+        Examples:
+            ```python
+            deployment = client.get_deployment(
+                name="awesome-deploy"
+            )
+            with open('image_420.png', 'rb') as img:
+                img_bytes = img.read()
+            deployment.predict_bytes(img_bytes, tags=["gonna", "give"], source="camera-1")
+            ```
+        Arguments:
+            raw_image (bytes): bytes of the image to predict.
+            tags (str, (Tag), list of str or Tag, optional): a list of tag to add to the data that will be created on the platform.
             source (str or DataSource, optional): a source to attach to the data that will be created on the platform.
-            file_path (str or Path): path to the image to predict
 
         Returns:
             A (dict) with information of the prediction
         """
 
         sent_tags = []
         if tags:
@@ -329,31 +360,30 @@
                     sent_tags.append(tag.name)
                 else:
                     sent_tags.append(tag)
 
         if isinstance(source, DataSource):
             source = source.name
 
-        with open(file_path, "rb") as file:
-            files = {"media": file}
+        payload = {"tags": sent_tags}
+        files = {"media": raw_image}
 
-            payload = {"tags": sent_tags}
-            if source:
-                payload["source"] = source
-
-            resp = self.serving_connexion.post(
-                path=f"/api/deployment/{self.id}/predict",
-                data=payload,
-                files=files,
-            )
+        if source:
+            payload["source"] = source
+
+        resp = self.serving_connexion.post(
+            path=f"/api/deployment/{self.id}/predict",
+            data=payload,
+            files=files,
+        )
 
-            if resp.status_code != 200:  # pragma: no cover
-                raise PredictionError(f"Could not predict because {resp.text}")
+        if resp.status_code != 200:  # pragma: no cover
+            raise PredictionError(f"Could not predict because {resp.text}")
 
-            return resp.json()
+        return resp.json()
 
     @exception_handler
     @beartype
     def setup_feedback_loop(self, dataset_version: DatasetVersion) -> None:
         """Set up the Feedback Loop for a Deployment.
         This way, you will be able to push reviewed predictions to given Dataset.
         This is a great option to increase your training set with quality data.
```

### Comparing `picsellia-6.8.0/picsellia/sdk/downloadable.py` & `picsellia-6.9.0/picsellia/sdk/downloadable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/evaluation.py` & `picsellia-6.9.0/picsellia/sdk/evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/experiment.py` & `picsellia-6.9.0/picsellia/sdk/experiment.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/job.py` & `picsellia-6.9.0/picsellia/sdk/job.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/label.py` & `picsellia-6.9.0/picsellia/sdk/label.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/line.py` & `picsellia-6.9.0/picsellia/sdk/line.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/log.py` & `picsellia-6.9.0/picsellia/sdk/log.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/logging_file.py` & `picsellia-6.9.0/picsellia/sdk/logging_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/model.py` & `picsellia-6.9.0/picsellia/sdk/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
         labels: Optional[dict] = None,
         base_parameters: Optional[dict] = None,
         docker_env_variables: Optional[dict] = None,
         name: Optional[str] = None,
         framework: Union[str, Framework, None] = None,
         type: Union[str, InferenceType, None] = None,
         description: Optional[str] = None,
+        docker_tag: Optional[str] = None,
     ) -> ModelVersion:
         """Create a version of a model.
 
         The version number of this model will be defined by the platform. It is incremented automatically.
 
         Examples:
             ```python
@@ -205,22 +206,23 @@
         ]:
             raise TypeError(f"Type '{type}' not supported yet for model version")
 
         payload = {
             "name": name,
             "type": type,
             "framework": framework,
-            "docker_image_name": docker_image_name,
+            "docker_image": docker_image_name,
             "docker_flags": docker_flags,
-            "thumb_object_name": thumb_object_name,
+            "thumbnail_object_name": thumb_object_name,
             "notebook_link": notebook_link,
             "labels": labels,
-            "base_parameters": base_parameters,
+            "parameters": base_parameters,
             "docker_env_variables": docker_env_variables,
             "description": description,
+            "docker_tag": docker_tag,
         }
         filtered_payload = utils.filter_payload(payload)
         r = self.connexion.post(
             f"/sdk/model/{self.id}/versions",
             data=orjson.dumps(filtered_payload),
         ).json()
         return ModelVersion(self.connexion, r)
```

### Comparing `picsellia-6.8.0/picsellia/sdk/model_context.py` & `picsellia-6.9.0/picsellia/sdk/model_context.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/model_file.py` & `picsellia-6.9.0/picsellia/sdk/model_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/model_version.py` & `picsellia-6.9.0/picsellia/sdk/model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         notebook_link: Optional[str] = None,
         base_parameters: Optional[dict] = None,
         docker_env_variables: Optional[dict] = None,
         framework: Union[str, Framework, None] = None,
         type: Union[str, InferenceType, None] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
+        docker_tag: Optional[str] = None,
     ) -> None:
         """Update this model version with some new infos.
 
         Examples:
             ```python
             model_v1.update(docker_image_name="docker.io/model1")
             ```
@@ -156,24 +157,25 @@
             InferenceType.OBJECT_DETECTION,
             InferenceType.SEGMENTATION,
         ]:
             raise TypeError(f"Type '{type}' not supported yet for model version")
 
         payload = {
             "labels": labels,
-            "docker_image_name": docker_image_name,
+            "docker_image": docker_image_name,
             "docker_flags": docker_flags,
-            "thumb_object_name": thumb_object_name,
+            "thumbnail_object_name": thumb_object_name,
             "notebook_link": notebook_link,
-            "base_parameters": base_parameters,
+            "parameters": base_parameters,
             "docker_env_variables": docker_env_variables,
             "type": type,
             "framework": framework,
             "name": name,
             "description": description,
+            "docker_tag": docker_tag,
         }
         filtered_payload = utils.filter_payload(payload)
         r = self.connexion.patch(
             f"/sdk/model/version/{self.id}",
             data=orjson.dumps(filtered_payload),
         ).json()
         self.refresh(r)
```

### Comparing `picsellia-6.8.0/picsellia/sdk/multi_object.py` & `picsellia-6.9.0/picsellia/sdk/multi_object.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/point.py` & `picsellia-6.9.0/picsellia/sdk/point.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/polygon.py` & `picsellia-6.9.0/picsellia/sdk/polygon.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/project.py` & `picsellia-6.9.0/picsellia/sdk/project.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/rectangle.py` & `picsellia-6.9.0/picsellia/sdk/rectangle.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/run.py` & `picsellia-6.9.0/picsellia/sdk/run.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/scan.py` & `picsellia-6.9.0/picsellia/sdk/scan.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/scan_file.py` & `picsellia-6.9.0/picsellia/sdk/scan_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/tag.py` & `picsellia-6.9.0/picsellia/sdk/tag.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/taggable.py` & `picsellia-6.9.0/picsellia/sdk/taggable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/sdk/worker.py` & `picsellia-6.9.0/picsellia/sdk/worker.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/asset_splitter.py` & `picsellia-6.9.0/picsellia/services/asset_splitter.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/coco_file_builder.py` & `picsellia-6.9.0/picsellia/services/coco_file_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/coco_importer.py` & `picsellia-6.9.0/picsellia/services/coco_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/datasource.py` & `picsellia-6.9.0/picsellia/services/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/error_manager.py` & `picsellia-6.9.0/picsellia/services/error_manager.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/splitter.py` & `picsellia-6.9.0/picsellia/services/splitter.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/voc_importer.py` & `picsellia-6.9.0/picsellia/services/voc_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/services/yolo_importer.py` & `picsellia-6.9.0/picsellia/services/yolo_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/types/enums.py` & `picsellia-6.9.0/picsellia/types/enums.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/types/schemas.py` & `picsellia-6.9.0/picsellia/types/schemas.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/types/schemas_prediction.py` & `picsellia-6.9.0/picsellia/types/schemas_prediction.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.8.0/picsellia/utils.py` & `picsellia-6.9.0/picsellia/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import warnings
 import zipfile
 from pathlib import Path
 from typing import Callable, Dict, List, Union
 
 from beartype import beartype
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
-from PIL import Image
 from requests import Response
 from requests.exceptions import InvalidJSONError
 
 from picsellia import exceptions as exceptions
 from picsellia.decorators import exception_handler
 
 logger = logging.getLogger("picsellia")
@@ -237,40 +236,14 @@
             return q1 + " and " + q2
 
 
 def chunk_list(items: list, chunk_size: int):
     return [(items[i : i + chunk_size], i) for i in range(0, len(items), chunk_size)]
 
 
-def get_image_shape_with_exif_transpose(image: Image):
-    """
-        This method reads exif tags of an image and invert width and height if needed.
-        Orientation flags that need inversion are : TRANSPOSE, ROTATE_90, TRANSVERSE and ROTATE_270
-
-    Args:
-        image: PIL Image to read
-
-    Returns:
-        width and height of image
-    """
-    exif = image.getexif()
-    orientation = exif.get(0x0112)
-
-    # Orientation when height and width are inverted :
-    # 5: Image.Transpose.TRANSPOSE
-    # 6: Image.Transpose.ROTATE_270
-    # 7: Image.Transpose.TRANSVERSE
-    # 8: Image.Transpose.ROTATE_90
-
-    if orientation in [5, 6, 7, 8]:
-        return image.height, image.width
-    else:
-        return image.width, image.height
-
-
 def flatten(items: List[List]) -> List:
     return [item for sublist in items for item in sublist]
 
 
 def flatten_dict(items: List[Dict], filter_value: Callable = lambda _: True) -> Dict:
     final_results = {}
     for res in items:
```

### Comparing `picsellia-6.8.0/pyproject.toml` & `picsellia-6.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["picsellia", "tests"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "picsellia"
-version = "6.8.0"
+version = "6.9.0"
 description = "Python SDK package for Picsellia MLOps platform"
 authors = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>"]
 maintainers = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>", "Lucien Haurat <lucien.haurat@picsellia.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.picsellia.com/"
 documentation = "https://documentation.picsellia.com/reference/client"
```

### Comparing `picsellia-6.8.0/setup.py` & `picsellia-6.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pydantic>=1.9.1,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'tdqm>=0.0.1,<0.0.2']
 
 setup_kwargs = {
     'name': 'picsellia',
-    'version': '6.8.0',
+    'version': '6.9.0',
     'description': 'Python SDK package for Picsellia MLOps platform',
     'long_description': '# Picsellia SDK\n\nPicsellia Python SDK is a python library that allows connecting to Picsellia platform.\n\n## Documentation\n\nReference of the SDK can be found at [reference](https://documentation.picsellia.com/reference/client)\n\n## Getting started\nDocumentation can be found at [docs](https://documentation.picsellia.com/docs/getting-started).\nStart by installing the Picsellia python package in your environment.\n```\npip install picsellia\n```\n\nThen, initialize a client\n```python\nfrom picsellia import Client\nclient = Client(api_token=<your api token>)\n```\n\nNow, use it to upload data and create a dataset !\n```python\nlake = client.get_datalake()\nuploaded_data = lake.upload_data(filepaths=["pics/twingo.png", "pics/ferrari.png"], tags=["tag_car"])\n\ndataset = client.create_dataset("cars").create_version("first")\ndataset.add_data(uploaded_data)\n```\n\n## What is Picsellia ?\n\nOur mission is to give you all the necessary tools to relieve the burden of AI projects off of your shoulders. As a data scientist / ML engineer / Researcher, you shouldn\'t have to worry about the following topics :\n\n- [💾 Data Management](https://documentation.picsellia.com/docs/data-management)\n- [📈 Experiment Tracking](https://documentation.picsellia.com/docs/experiment-tracking)\n- [📘 Model Management](https://documentation.picsellia.com/docs/export-an-experiment)\n- [🚀 Model Deployment](https://documentation.picsellia.com/docs/serverless)\n- [👀 Model Monitoring](https://documentation.picsellia.com/docs/monitor-model)\n\nPicsellia is the one-stop place for all the life-cycle of your Computer Vision projects, from ideation to production in a single platform 🚀.\n',
     'author': 'Pierre-Nicolas Tiffreau',
     'author_email': 'pierre-nicolas@picsellia.com',
     'maintainer': 'Pierre-Nicolas Tiffreau',
     'maintainer_email': 'pierre-nicolas@picsellia.com',
     'url': 'https://www.picsellia.com/',
```

### Comparing `picsellia-6.8.0/PKG-INFO` & `picsellia-6.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picsellia
-Version: 6.8.0
+Version: 6.9.0
 Summary: Python SDK package for Picsellia MLOps platform
 Home-page: https://www.picsellia.com/
 License: MIT
 Keywords: ai,picsellia,sdk,cvops
 Author: Pierre-Nicolas Tiffreau
 Author-email: pierre-nicolas@picsellia.com
 Maintainer: Pierre-Nicolas Tiffreau
```

