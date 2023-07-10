# Comparing `tmp/groupdocs-viewer-cloud-23.3.tar.gz` & `tmp/groupdocs-viewer-cloud-23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-viewer-cloud-23.3.tar", last modified: Thu Mar 16 09:25:30 2023, max compression
+gzip compressed data, was "dist\groupdocs-viewer-cloud-23.7.tar", last modified: Mon Jul 10 06:34:27 2023, max compression
```

## Comparing `groupdocs-viewer-cloud-23.3.tar` & `groupdocs-viewer-cloud-23.7.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/
--rw-rw-rw-   0        0        0     1105 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/LICENSE
--rw-rw-rw-   0        0        0     2836 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/PKG-INFO
--rw-rw-rw-   0        0        0     2005 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/
--rw-rw-rw-   0        0        0     5194 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/__init__.py
--rw-rw-rw-   0        0        0    26221 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/
--rw-rw-rw-   0        0        0      439 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    38644 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36254 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    11877 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     6594 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0    26570 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0    14020 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/view_api.py
--rw-rw-rw-   0        0        0     3303 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/auth.py
--rw-rw-rw-   0        0        0     7677 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/
--rw-rw-rw-   0        0        0     3950 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     6122 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/archive_options.py
--rw-rw-rw-   0        0        0     4227 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/archive_view_info.py
--rw-rw-rw-   0        0        0     4071 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/attachment_info.py
--rw-rw-rw-   0        0        0     4306 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/attachment_view.py
--rw-rw-rw-   0        0        0    10268 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/cad_options.py
--rw-rw-rw-   0        0        0     4980 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/cad_view_info.py
--rw-rw-rw-   0        0        0     3730 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/character.py
--rw-rw-rw-   0        0        0     5129 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     5068 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/delete_view_options.py
--rw-rw-rw-   0        0        0     5187 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0    13603 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/email_options.py
--rw-rw-rw-   0        0        0     6291 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     4761 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/field_label.py
--rw-rw-rw-   0        0        0     6354 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5409 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     4876 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/format.py
--rw-rw-rw-   0        0        0     4211 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0    17155 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/html_options.py
--rw-rw-rw-   0        0        0     4402 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/html_resource.py
--rw-rw-rw-   0        0        0    10331 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/image_options.py
--rw-rw-rw-   0        0        0    11378 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/info_result.py
--rw-rw-rw-   0        0        0     4906 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/layer.py
--rw-rw-rw-   0        0        0     5663 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/layout.py
--rw-rw-rw-   0        0        0     4394 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/line.py
--rw-rw-rw-   0        0        0     6261 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/mail_storage_options.py
--rw-rw-rw-   0        0        0     5178 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     7158 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/outlook_options.py
--rw-rw-rw-   0        0        0     4258 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/outlook_view_info.py
--rw-rw-rw-   0        0        0     7555 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/page_info.py
--rw-rw-rw-   0        0        0     5807 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/page_rotation.py
--rw-rw-rw-   0        0        0     5200 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/page_view.py
--rw-rw-rw-   0        0        0    12395 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/pdf_document_options.py
--rw-rw-rw-   0        0        0    12476 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/pdf_options.py
--rw-rw-rw-   0        0        0     4531 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/pdf_view_info.py
--rw-rw-rw-   0        0        0     8156 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/project_management_options.py
--rw-rw-rw-   0        0        0     5373 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/project_management_view_info.py
--rw-rw-rw-   0        0        0    27431 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/render_options.py
--rw-rw-rw-   0        0        0     4878 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/resource.py
--rw-rw-rw-   0        0        0    17039 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/spreadsheet_options.py
--rw-rw-rw-   0        0        0     4276 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0     7677 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/text_element.py
--rw-rw-rw-   0        0        0     5615 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/text_options.py
--rw-rw-rw-   0        0        0     7139 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/tile.py
--rw-rw-rw-   0        0        0     8891 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/view_options.py
--rw-rw-rw-   0        0        0     5561 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/view_result.py
--rw-rw-rw-   0        0        0     5662 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/visio_rendering_options.py
--rw-rw-rw-   0        0        0     7064 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/watermark.py
--rw-rw-rw-   0        0        0     9859 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/web_document_options.py
--rw-rw-rw-   0        0        0     4519 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/word.py
--rw-rw-rw-   0        0        0     8556 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/word_processing_options.py
--rw-rw-rw-   0        0        0    13735 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/
--rw-rw-rw-   0        0        0     2836 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/setup.cfg
--rw-rw-rw-   0        0        0     1679 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/test/
--rw-rw-rw-   0        0        0        0 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 09:25:30.000000 groupdocs-viewer-cloud-23.3/test/apis/
--rw-rw-rw-   0        0        0        0 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3001 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0     3798 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3135 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     2731 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     9101 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_viewer_create_view_api.py
--rw-rw-rw-   0        0        0     2294 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_viewer_delete_view_api.py
--rw-rw-rw-   0        0        0     2028 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_viewer_formats_api.py
--rw-rw-rw-   0        0        0     8350 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/apis/test_viewer_get_info_api.py
--rw-rw-rw-   0        0        0     4733 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/test_context.py
--rw-rw-rw-   0        0        0     3964 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/test_file.py
--rw-rw-rw-   0        0        0     1702 2023-03-16 09:24:55.000000 groupdocs-viewer-cloud-23.3/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/
+-rw-rw-rw-   0        0        0     1105 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/LICENSE
+-rw-rw-rw-   0        0        0     2836 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2005 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/
+-rw-rw-rw-   0        0        0     5194 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/__init__.py
+-rw-rw-rw-   0        0        0    26221 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/
+-rw-rw-rw-   0        0        0      439 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    38644 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36254 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    11877 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     6594 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0    26570 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0    14020 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/view_api.py
+-rw-rw-rw-   0        0        0     3303 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/auth.py
+-rw-rw-rw-   0        0        0     7677 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/
+-rw-rw-rw-   0        0        0     3950 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     6122 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/archive_options.py
+-rw-rw-rw-   0        0        0     4227 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/archive_view_info.py
+-rw-rw-rw-   0        0        0     4071 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/attachment_info.py
+-rw-rw-rw-   0        0        0     4306 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/attachment_view.py
+-rw-rw-rw-   0        0        0    10268 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/cad_options.py
+-rw-rw-rw-   0        0        0     4980 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/cad_view_info.py
+-rw-rw-rw-   0        0        0     3730 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/character.py
+-rw-rw-rw-   0        0        0     5129 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     5068 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/delete_view_options.py
+-rw-rw-rw-   0        0        0     5187 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0    13603 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/email_options.py
+-rw-rw-rw-   0        0        0     6291 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     4761 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/field_label.py
+-rw-rw-rw-   0        0        0     6354 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5409 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     4876 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4211 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0    17155 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/html_options.py
+-rw-rw-rw-   0        0        0     4402 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/html_resource.py
+-rw-rw-rw-   0        0        0    10331 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/image_options.py
+-rw-rw-rw-   0        0        0    11378 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/info_result.py
+-rw-rw-rw-   0        0        0     4906 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/layer.py
+-rw-rw-rw-   0        0        0     5663 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/layout.py
+-rw-rw-rw-   0        0        0     4394 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/line.py
+-rw-rw-rw-   0        0        0     6261 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/mail_storage_options.py
+-rw-rw-rw-   0        0        0     5178 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     7158 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/outlook_options.py
+-rw-rw-rw-   0        0        0     4258 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/outlook_view_info.py
+-rw-rw-rw-   0        0        0     7555 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/page_info.py
+-rw-rw-rw-   0        0        0     5807 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/page_rotation.py
+-rw-rw-rw-   0        0        0     5200 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/page_view.py
+-rw-rw-rw-   0        0        0    12395 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/pdf_document_options.py
+-rw-rw-rw-   0        0        0    12476 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/pdf_options.py
+-rw-rw-rw-   0        0        0     4531 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/pdf_view_info.py
+-rw-rw-rw-   0        0        0     8156 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/project_management_options.py
+-rw-rw-rw-   0        0        0     5373 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/project_management_view_info.py
+-rw-rw-rw-   0        0        0    27431 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/render_options.py
+-rw-rw-rw-   0        0        0     4878 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/resource.py
+-rw-rw-rw-   0        0        0    17039 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/spreadsheet_options.py
+-rw-rw-rw-   0        0        0     4276 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     7677 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/text_element.py
+-rw-rw-rw-   0        0        0     5615 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/text_options.py
+-rw-rw-rw-   0        0        0     7139 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/tile.py
+-rw-rw-rw-   0        0        0     8891 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/view_options.py
+-rw-rw-rw-   0        0        0     5561 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/view_result.py
+-rw-rw-rw-   0        0        0     5662 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/visio_rendering_options.py
+-rw-rw-rw-   0        0        0     7064 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/watermark.py
+-rw-rw-rw-   0        0        0     9859 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/web_document_options.py
+-rw-rw-rw-   0        0        0     4519 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/word.py
+-rw-rw-rw-   0        0        0     8556 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/word_processing_options.py
+-rw-rw-rw-   0        0        0    13735 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/
+-rw-rw-rw-   0        0        0     2836 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3759 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/setup.cfg
+-rw-rw-rw-   0        0        0     1679 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/test/
+-rw-rw-rw-   0        0        0        0 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:34:27.000000 groupdocs-viewer-cloud-23.7/test/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3001 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0     3798 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3135 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     2731 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     9101 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_viewer_create_view_api.py
+-rw-rw-rw-   0        0        0     2294 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_viewer_delete_view_api.py
+-rw-rw-rw-   0        0        0     2028 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_viewer_formats_api.py
+-rw-rw-rw-   0        0        0     8350 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/apis/test_viewer_get_info_api.py
+-rw-rw-rw-   0        0        0     4733 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/test_context.py
+-rw-rw-rw-   0        0        0     3964 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/test_file.py
+-rw-rw-rw-   0        0        0     1702 2023-07-10 06:33:55.000000 groupdocs-viewer-cloud-23.7/test/test_settings.py
```

### Comparing `groupdocs-viewer-cloud-23.3/LICENSE` & `groupdocs-viewer-cloud-23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/PKG-INFO` & `groupdocs-viewer-cloud-23.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-viewer-cloud
-Version: 23.3
+Version: 23.7
 Summary: GroupDocs.Viewer Cloud Python SDK
 Home-page: http://github.com/groupdocs-viewer-cloud/groupdocs-viewer-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,viewer,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-viewer-cloud-23.3/README.md` & `groupdocs-viewer-cloud-23.7/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/__init__.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/api_client.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.3'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.7'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 23.3'
+        self.user_agent = 'python sdk 23.7'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/api_exception.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/api_exception.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/file_api.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/folder_api.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/info_api.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/license_api.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/license_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/storage_api.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/apis/view_api.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/apis/view_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/auth.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/auth.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/configuration.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.3\n"\
-               "SDK Package Version: 23.3".\
+               "Version of the API: 23.7\n"\
+               "SDK Package Version: 23.7".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/__init__.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/archive_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/archive_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/archive_view_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/archive_view_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/attachment_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/attachment_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/attachment_view.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/attachment_view.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/cad_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/cad_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/cad_view_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/cad_view_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/character.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/character.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/consumption_result.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/consumption_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/delete_view_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/delete_view_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/disc_usage.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/email_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/email_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/error.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/error.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/error_details.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/field_label.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/field_label.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/file_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/file_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/file_version.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/file_versions.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/files_list.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/files_upload_result.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/format.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/format.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/formats_result.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/formats_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/html_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/html_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/html_resource.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/html_resource.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/image_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/image_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/info_result.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/info_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/layer.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/layer.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/layout.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/layout.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/line.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/line.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/mail_storage_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/mail_storage_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/object_exist.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/outlook_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/outlook_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/outlook_view_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/outlook_view_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/page_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/page_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/page_rotation.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/page_rotation.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/page_view.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/page_view.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/pdf_document_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/pdf_document_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/pdf_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/pdf_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/pdf_view_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/pdf_view_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/project_management_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/project_management_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/project_management_view_info.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/project_management_view_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/render_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/render_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/resource.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/resource.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/spreadsheet_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/spreadsheet_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/storage_exist.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/storage_file.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/text_element.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/text_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/text_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/tile.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/tile.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/view_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/view_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/view_result.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/view_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/visio_rendering_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/visio_rendering_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/watermark.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/watermark.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/web_document_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/web_document_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/word.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/word.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/models/word_processing_options.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/models/word_processing_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud/rest.py` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/PKG-INFO` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-viewer-cloud
-Version: 23.3
+Version: 23.7
 Summary: GroupDocs.Viewer Cloud Python SDK
 Home-page: http://github.com/groupdocs-viewer-cloud/groupdocs-viewer-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,viewer,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `groupdocs-viewer-cloud-23.3/groupdocs_viewer_cloud.egg-info/SOURCES.txt` & `groupdocs-viewer-cloud-23.7/groupdocs_viewer_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/setup.py` & `groupdocs-viewer-cloud-23.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-viewer-cloud"
-VERSION = "23.3"
+VERSION = "23.7"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_auth_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_file_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_folder_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_storage_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_viewer_create_view_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_viewer_create_view_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_viewer_delete_view_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_viewer_delete_view_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_viewer_formats_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_viewer_formats_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/apis/test_viewer_get_info_api.py` & `groupdocs-viewer-cloud-23.7/test/apis/test_viewer_get_info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/test_context.py` & `groupdocs-viewer-cloud-23.7/test/test_context.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/test_file.py` & `groupdocs-viewer-cloud-23.7/test/test_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-viewer-cloud-23.3/test/test_settings.py` & `groupdocs-viewer-cloud-23.7/test/test_settings.py`

 * *Files identical despite different names*

