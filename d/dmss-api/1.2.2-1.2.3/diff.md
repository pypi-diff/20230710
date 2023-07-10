# Comparing `tmp/dmss-api-1.2.2.tar.gz` & `tmp/dmss-api-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmss-api-1.2.2.tar", last modified: Wed Jun 21 09:56:55 2023, max compression
+gzip compressed data, was "dmss-api-1.2.3.tar", last modified: Mon Jul 10 13:36:22 2023, max compression
```

## Comparing `dmss-api-1.2.2.tar` & `dmss-api-1.2.3.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.866175 dmss-api-1.2.2/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-21 09:56:55.870175 dmss-api-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11760 2023-06-21 09:56:54.000000 dmss-api-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.842173 dmss-api-1.2.2/dmss_api/
--rw-r--r--   0 root         (0) root         (0)      675 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.850174 dmss-api-1.2.2/dmss_api/api/
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11182 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/access_control_api.py
--rw-r--r--   0 root         (0) root         (0)     5345 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/attribute_api.py
--rw-r--r--   0 root         (0) root         (0)    10827 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/blob_api.py
--rw-r--r--   0 root         (0) root         (0)    10499 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/blueprint_api.py
--rw-r--r--   0 root         (0) root         (0)    14478 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/datasource_api.py
--rw-r--r--   0 root         (0) root         (0)   140550 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    27059 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/document_api.py
--rw-r--r--   0 root         (0) root         (0)    10544 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/entity_api.py
--rw-r--r--   0 root         (0) root         (0)    10156 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/export_api.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/health_check_api.py
--rw-r--r--   0 root         (0) root         (0)    10424 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/lookup_table_api.py
--rw-r--r--   0 root         (0) root         (0)    13697 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/personal_access_token_api.py
--rw-r--r--   0 root         (0) root         (0)    11622 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/reference_api.py
--rw-r--r--   0 root         (0) root         (0)     6429 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/search_api.py
--rw-r--r--   0 root         (0) root         (0)     5000 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/api/whoami_api.py
--rw-r--r--   0 root         (0) root         (0)    36751 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.850174 dmss-api-1.2.2/dmss_api/apis/
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17221 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5045 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.858174 dmss-api-1.2.2/dmss_api/model/
--rw-r--r--   0 root         (0) root         (0)      348 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11900 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/access_level.py
--rw-r--r--   0 root         (0) root         (0)    12074 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/acl.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/data_source_information.py
--rw-r--r--   0 root         (0) root         (0)    11544 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/data_source_request.py
--rw-r--r--   0 root         (0) root         (0)    11219 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/entity.py
--rw-r--r--   0 root         (0) root         (0)    12703 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)    12292 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/get_blueprint_response.py
--rw-r--r--   0 root         (0) root         (0)    12227 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/lookup.py
--rw-r--r--   0 root         (0) root         (0)    12532 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/pat_data.py
--rw-r--r--   0 root         (0) root         (0)    14036 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/recipe.py
--rw-r--r--   0 root         (0) root         (0)    13139 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/recipe_attribute.py
--rw-r--r--   0 root         (0) root         (0)    11750 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/reference.py
--rw-r--r--   0 root         (0) root         (0)    13481 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/repository.py
--rw-r--r--   0 root         (0) root         (0)    12059 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/repository_type.py
--rw-r--r--   0 root         (0) root         (0)    12590 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/storage_attribute.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/storage_data_types.py
--rw-r--r--   0 root         (0) root         (0)    12532 2023-06-21 09:56:54.000000 dmss-api-1.2.2/dmss_api/model/storage_recipe.py
--rw-r--r--   0 root         (0) root         (0)    80121 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.858174 dmss-api-1.2.2/dmss_api/models/
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12643 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.842173 dmss-api-1.2.2/dmss_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2287 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-21 09:56:55.000000 dmss-api-1.2.2/dmss_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-21 09:56:55.870175 dmss-api-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1011 2023-06-21 09:56:54.000000 dmss-api-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:56:55.866175 dmss-api-1.2.2/test/
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_access_control_api.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_access_level.py
--rw-r--r--   0 root         (0) root         (0)      738 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_acl.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_attribute_api.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_blob_api.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_blueprint_api.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_data_source_information.py
--rw-r--r--   0 root         (0) root         (0)      833 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_data_source_request.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_datasource_api.py
--rw-r--r--   0 root         (0) root         (0)     4437 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_default_api.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_document_api.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_entity.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_entity_api.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_export_api.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_get_blueprint_response.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_health_check_api.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_lookup.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_lookup_table_api.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_pat_data.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_personal_access_token_api.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_recipe.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_recipe_attribute.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_reference.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_reference_api.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_repository.py
--rw-r--r--   0 root         (0) root         (0)      725 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_repository_type.py
--rw-r--r--   0 root         (0) root         (0)      642 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_search_api.py
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_storage_attribute.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_storage_data_types.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_storage_recipe.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-21 09:56:54.000000 dmss-api-1.2.2/test/test_whoami_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.531063 dmss-api-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-10 13:36:22.531063 dmss-api-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12130 2023-07-10 13:36:21.000000 dmss-api-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.523063 dmss-api-1.2.3/dmss_api/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.523063 dmss-api-1.2.3/dmss_api/api/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11182 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/access_control_api.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/attribute_api.py
+-rw-r--r--   0 root         (0) root         (0)    10827 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/blob_api.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/blueprint_api.py
+-rw-r--r--   0 root         (0) root         (0)    14478 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/datasource_api.py
+-rw-r--r--   0 root         (0) root         (0)   149627 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    26969 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/document_api.py
+-rw-r--r--   0 root         (0) root         (0)    10544 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/entity_api.py
+-rw-r--r--   0 root         (0) root         (0)    10224 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/export_api.py
+-rw-r--r--   0 root         (0) root         (0)     6169 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/file_api.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/health_check_api.py
+-rw-r--r--   0 root         (0) root         (0)    10424 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/lookup_table_api.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/meta_api.py
+-rw-r--r--   0 root         (0) root         (0)    13697 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/personal_access_token_api.py
+-rw-r--r--   0 root         (0) root         (0)    10608 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/reference_api.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/search_api.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api/whoami_api.py
+-rw-r--r--   0 root         (0) root         (0)    36751 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.523063 dmss-api-1.2.3/dmss_api/apis/
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17221 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.527063 dmss-api-1.2.3/dmss_api/model/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11900 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/access_level.py
+-rw-r--r--   0 root         (0) root         (0)    12074 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/acl.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/data_source_information.py
+-rw-r--r--   0 root         (0) root         (0)    11544 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/data_source_request.py
+-rw-r--r--   0 root         (0) root         (0)    11219 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/entity.py
+-rw-r--r--   0 root         (0) root         (0)    12703 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)    12292 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/get_blueprint_response.py
+-rw-r--r--   0 root         (0) root         (0)    12227 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/lookup.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/pat_data.py
+-rw-r--r--   0 root         (0) root         (0)    14036 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/recipe.py
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/recipe_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    11768 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/reference_entity.py
+-rw-r--r--   0 root         (0) root         (0)    13481 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/repository.py
+-rw-r--r--   0 root         (0) root         (0)    12059 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/repository_type.py
+-rw-r--r--   0 root         (0) root         (0)    12590 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/storage_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/storage_data_types.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model/storage_recipe.py
+-rw-r--r--   0 root         (0) root         (0)    80121 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.527063 dmss-api-1.2.3/dmss_api/models/
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12643 2023-07-10 13:36:21.000000 dmss-api-1.2.3/dmss_api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.523063 dmss-api-1.2.3/dmss_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-10 13:36:22.000000 dmss-api-1.2.3/dmss_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-07-10 13:36:22.000000 dmss-api-1.2.3/dmss_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:36:22.000000 dmss-api-1.2.3/dmss_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-10 13:36:22.000000 dmss-api-1.2.3/dmss_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-10 13:36:22.000000 dmss-api-1.2.3/dmss_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-10 13:36:22.531063 dmss-api-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-07-10 13:36:21.000000 dmss-api-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:36:22.531063 dmss-api-1.2.3/test/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_access_control_api.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_access_level.py
+-rw-r--r--   0 root         (0) root         (0)      738 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_acl.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_attribute_api.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_blob_api.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_blueprint_api.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_data_source_information.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_data_source_request.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_datasource_api.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_default_api.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_document_api.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_entity.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_entity_api.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_export_api.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_file_api.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_get_blueprint_response.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_health_check_api.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_lookup.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_lookup_table_api.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_meta_api.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_pat_data.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_personal_access_token_api.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_recipe.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_recipe_attribute.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_reference_api.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_reference_entity.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_repository.py
+-rw-r--r--   0 root         (0) root         (0)      725 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_repository_type.py
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_search_api.py
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_storage_attribute.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_storage_data_types.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_storage_recipe.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-07-10 13:36:21.000000 dmss-api-1.2.3/test/test_whoami_api.py
```

### Comparing `dmss-api-1.2.2/README.md` & `dmss-api-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # dmss-api
 API for basic data modelling interaction
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 1.2.2
+- Package version: 1.2.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
@@ -95,68 +95,72 @@
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AccessControlApi* | [**get_acl**](docs/AccessControlApi.md#get_acl) | **GET** /api/acl/{data_source_id}/{document_id} | Get Acl
 *AccessControlApi* | [**set_acl**](docs/AccessControlApi.md#set_acl) | **PUT** /api/acl/{data_source_id}/{document_id} | Set Acl
-*AttributeApi* | [**attribute_get**](docs/AttributeApi.md#attribute_get) | **GET** /api/attribute/{reference} | Get Attribute
+*AttributeApi* | [**attribute_get**](docs/AttributeApi.md#attribute_get) | **GET** /api/attribute/{address} | Get Attribute
 *BlobApi* | [**blob_get_by_id**](docs/BlobApi.md#blob_get_by_id) | **GET** /api/blobs/{data_source_id}/{blob_id} | Get By Id
 *BlobApi* | [**blob_upload**](docs/BlobApi.md#blob_upload) | **PUT** /api/blobs/{data_source_id}/{blob_id} | Upload
 *BlueprintApi* | [**blueprint_get**](docs/BlueprintApi.md#blueprint_get) | **GET** /api/blueprint/{type_ref} | Get Blueprint
-*BlueprintApi* | [**blueprint_resolve**](docs/BlueprintApi.md#blueprint_resolve) | **GET** /api/resolve-path/{absolute_id} | Resolve Blueprint Id
+*BlueprintApi* | [**blueprint_resolve**](docs/BlueprintApi.md#blueprint_resolve) | **GET** /api/resolve-path/{address} | Resolve Blueprint Id
 *DatasourceApi* | [**data_source_get**](docs/DatasourceApi.md#data_source_get) | **GET** /api/data-sources/{data_source_id} | Get
 *DatasourceApi* | [**data_source_get_all**](docs/DatasourceApi.md#data_source_get_all) | **GET** /api/data-sources | Get All
 *DatasourceApi* | [**data_source_save**](docs/DatasourceApi.md#data_source_save) | **POST** /api/data-sources/{data_source_id} | Save
-*DefaultApi* | [**attribute_get**](docs/DefaultApi.md#attribute_get) | **GET** /api/attribute/{reference} | Get Attribute
+*DefaultApi* | [**attribute_get**](docs/DefaultApi.md#attribute_get) | **GET** /api/attribute/{address} | Get Attribute
 *DefaultApi* | [**blob_get_by_id**](docs/DefaultApi.md#blob_get_by_id) | **GET** /api/blobs/{data_source_id}/{blob_id} | Get By Id
 *DefaultApi* | [**blob_upload**](docs/DefaultApi.md#blob_upload) | **PUT** /api/blobs/{data_source_id}/{blob_id} | Upload
 *DefaultApi* | [**blueprint_get**](docs/DefaultApi.md#blueprint_get) | **GET** /api/blueprint/{type_ref} | Get Blueprint
-*DefaultApi* | [**blueprint_resolve**](docs/DefaultApi.md#blueprint_resolve) | **GET** /api/resolve-path/{absolute_id} | Resolve Blueprint Id
+*DefaultApi* | [**blueprint_resolve**](docs/DefaultApi.md#blueprint_resolve) | **GET** /api/resolve-path/{address} | Resolve Blueprint Id
 *DefaultApi* | [**create_lookup**](docs/DefaultApi.md#create_lookup) | **POST** /api/application/{application} | Create Lookup
 *DefaultApi* | [**data_source_get**](docs/DefaultApi.md#data_source_get) | **GET** /api/data-sources/{data_source_id} | Get
 *DefaultApi* | [**data_source_get_all**](docs/DefaultApi.md#data_source_get_all) | **GET** /api/data-sources | Get All
 *DefaultApi* | [**data_source_save**](docs/DefaultApi.md#data_source_save) | **POST** /api/data-sources/{data_source_id} | Save
-*DefaultApi* | [**document_add**](docs/DefaultApi.md#document_add) | **POST** /api/documents/{reference} | Add Document
+*DefaultApi* | [**document_add**](docs/DefaultApi.md#document_add) | **POST** /api/documents/{address} | Add Document
 *DefaultApi* | [**document_add_simple**](docs/DefaultApi.md#document_add_simple) | **POST** /api/documents-add-raw/{data_source_id} | Add Raw
-*DefaultApi* | [**document_get**](docs/DefaultApi.md#document_get) | **GET** /api/documents/{reference} | Get
-*DefaultApi* | [**document_remove**](docs/DefaultApi.md#document_remove) | **DELETE** /api/documents/{reference} | Remove
-*DefaultApi* | [**document_update**](docs/DefaultApi.md#document_update) | **PUT** /api/documents/{id_reference} | Update
-*DefaultApi* | [**export**](docs/DefaultApi.md#export) | **GET** /api/export/{reference} | Export
-*DefaultApi* | [**export_meta**](docs/DefaultApi.md#export_meta) | **GET** /api/export/meta/{reference} | Export Meta
+*DefaultApi* | [**document_get**](docs/DefaultApi.md#document_get) | **GET** /api/documents/{address} | Get
+*DefaultApi* | [**document_remove**](docs/DefaultApi.md#document_remove) | **DELETE** /api/documents/{address} | Remove
+*DefaultApi* | [**document_update**](docs/DefaultApi.md#document_update) | **PUT** /api/documents/{id_address} | Update
+*DefaultApi* | [**export**](docs/DefaultApi.md#export) | **GET** /api/export/{path_address} | Export
+*DefaultApi* | [**export_meta**](docs/DefaultApi.md#export_meta) | **GET** /api/export/meta/{path_address} | Export Meta
+*DefaultApi* | [**file_upload**](docs/DefaultApi.md#file_upload) | **POST** /api/files/{data_source_id} | Upload File
 *DefaultApi* | [**get_acl**](docs/DefaultApi.md#get_acl) | **GET** /api/acl/{data_source_id}/{document_id} | Get Acl
 *DefaultApi* | [**get_api_healthcheck_get**](docs/DefaultApi.md#get_api_healthcheck_get) | **GET** /api/healthcheck | Get
 *DefaultApi* | [**get_lookup**](docs/DefaultApi.md#get_lookup) | **GET** /api/application/{application} | Get Lookup
 *DefaultApi* | [**instantiate_entity**](docs/DefaultApi.md#instantiate_entity) | **POST** /api/entity | Instantiate
-*DefaultApi* | [**reference_delete**](docs/DefaultApi.md#reference_delete) | **DELETE** /api/reference/{data_source_id}/{document_dotted_id} | Delete Reference
-*DefaultApi* | [**reference_insert**](docs/DefaultApi.md#reference_insert) | **PUT** /api/reference/{data_source_id}/{document_dotted_id} | Insert Reference
+*DefaultApi* | [**meta_by_id**](docs/DefaultApi.md#meta_by_id) | **GET** /api/meta/{data_source_id}/{document_id} | Get Meta By Id
+*DefaultApi* | [**reference_delete**](docs/DefaultApi.md#reference_delete) | **DELETE** /api/reference/{address} | Delete Reference
+*DefaultApi* | [**reference_insert**](docs/DefaultApi.md#reference_insert) | **PUT** /api/reference/{address} | Insert Reference
 *DefaultApi* | [**search**](docs/DefaultApi.md#search) | **POST** /api/search | Search
 *DefaultApi* | [**set_acl**](docs/DefaultApi.md#set_acl) | **PUT** /api/acl/{data_source_id}/{document_id} | Set Acl
 *DefaultApi* | [**token_create**](docs/DefaultApi.md#token_create) | **POST** /api/token | New Personal Access Token
 *DefaultApi* | [**token_delete**](docs/DefaultApi.md#token_delete) | **DELETE** /api/token/{token_id} | Revoke Personal Access Token
 *DefaultApi* | [**token_list_all**](docs/DefaultApi.md#token_list_all) | **GET** /api/token | List All Pats
 *DefaultApi* | [**validate_entity**](docs/DefaultApi.md#validate_entity) | **POST** /api/entity/validate | Validate
 *DefaultApi* | [**whoami**](docs/DefaultApi.md#whoami) | **GET** /api/whoami | Get Information On Authenticated User
-*DocumentApi* | [**document_add**](docs/DocumentApi.md#document_add) | **POST** /api/documents/{reference} | Add Document
+*DocumentApi* | [**document_add**](docs/DocumentApi.md#document_add) | **POST** /api/documents/{address} | Add Document
 *DocumentApi* | [**document_add_simple**](docs/DocumentApi.md#document_add_simple) | **POST** /api/documents-add-raw/{data_source_id} | Add Raw
-*DocumentApi* | [**document_get**](docs/DocumentApi.md#document_get) | **GET** /api/documents/{reference} | Get
-*DocumentApi* | [**document_remove**](docs/DocumentApi.md#document_remove) | **DELETE** /api/documents/{reference} | Remove
-*DocumentApi* | [**document_update**](docs/DocumentApi.md#document_update) | **PUT** /api/documents/{id_reference} | Update
+*DocumentApi* | [**document_get**](docs/DocumentApi.md#document_get) | **GET** /api/documents/{address} | Get
+*DocumentApi* | [**document_remove**](docs/DocumentApi.md#document_remove) | **DELETE** /api/documents/{address} | Remove
+*DocumentApi* | [**document_update**](docs/DocumentApi.md#document_update) | **PUT** /api/documents/{id_address} | Update
 *EntityApi* | [**instantiate_entity**](docs/EntityApi.md#instantiate_entity) | **POST** /api/entity | Instantiate
 *EntityApi* | [**validate_entity**](docs/EntityApi.md#validate_entity) | **POST** /api/entity/validate | Validate
-*ExportApi* | [**export**](docs/ExportApi.md#export) | **GET** /api/export/{reference} | Export
-*ExportApi* | [**export_meta**](docs/ExportApi.md#export_meta) | **GET** /api/export/meta/{reference} | Export Meta
+*ExportApi* | [**export**](docs/ExportApi.md#export) | **GET** /api/export/{path_address} | Export
+*ExportApi* | [**export_meta**](docs/ExportApi.md#export_meta) | **GET** /api/export/meta/{path_address} | Export Meta
+*FileApi* | [**file_upload**](docs/FileApi.md#file_upload) | **POST** /api/files/{data_source_id} | Upload File
 *HealthCheckApi* | [**get_api_healthcheck_get**](docs/HealthCheckApi.md#get_api_healthcheck_get) | **GET** /api/healthcheck | Get
 *LookupTableApi* | [**create_lookup**](docs/LookupTableApi.md#create_lookup) | **POST** /api/application/{application} | Create Lookup
 *LookupTableApi* | [**get_lookup**](docs/LookupTableApi.md#get_lookup) | **GET** /api/application/{application} | Get Lookup
+*MetaApi* | [**meta_by_id**](docs/MetaApi.md#meta_by_id) | **GET** /api/meta/{data_source_id}/{document_id} | Get Meta By Id
 *PersonalAccessTokenApi* | [**token_create**](docs/PersonalAccessTokenApi.md#token_create) | **POST** /api/token | New Personal Access Token
 *PersonalAccessTokenApi* | [**token_delete**](docs/PersonalAccessTokenApi.md#token_delete) | **DELETE** /api/token/{token_id} | Revoke Personal Access Token
 *PersonalAccessTokenApi* | [**token_list_all**](docs/PersonalAccessTokenApi.md#token_list_all) | **GET** /api/token | List All Pats
-*ReferenceApi* | [**reference_delete**](docs/ReferenceApi.md#reference_delete) | **DELETE** /api/reference/{data_source_id}/{document_dotted_id} | Delete Reference
-*ReferenceApi* | [**reference_insert**](docs/ReferenceApi.md#reference_insert) | **PUT** /api/reference/{data_source_id}/{document_dotted_id} | Insert Reference
+*ReferenceApi* | [**reference_delete**](docs/ReferenceApi.md#reference_delete) | **DELETE** /api/reference/{address} | Delete Reference
+*ReferenceApi* | [**reference_insert**](docs/ReferenceApi.md#reference_insert) | **PUT** /api/reference/{address} | Insert Reference
 *SearchApi* | [**search**](docs/SearchApi.md#search) | **POST** /api/search | Search
 *WhoamiApi* | [**whoami**](docs/WhoamiApi.md#whoami) | **GET** /api/whoami | Get Information On Authenticated User
 
 
 ## Documentation For Models
 
  - [ACL](docs/ACL.md)
@@ -166,15 +170,15 @@
  - [Entity](docs/Entity.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [GetBlueprintResponse](docs/GetBlueprintResponse.md)
  - [Lookup](docs/Lookup.md)
  - [PATData](docs/PATData.md)
  - [Recipe](docs/Recipe.md)
  - [RecipeAttribute](docs/RecipeAttribute.md)
- - [Reference](docs/Reference.md)
+ - [ReferenceEntity](docs/ReferenceEntity.md)
  - [Repository](docs/Repository.md)
  - [RepositoryType](docs/RepositoryType.md)
  - [StorageAttribute](docs/StorageAttribute.md)
  - [StorageDataTypes](docs/StorageDataTypes.md)
  - [StorageRecipe](docs/StorageRecipe.md)
```

### Comparing `dmss-api-1.2.2/dmss_api/__init__.py` & `dmss-api-1.2.3/dmss_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     API for basic data modelling interaction  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 # import ApiClient
 from dmss_api.api_client import ApiClient
 
 # import Configuration
 from dmss_api.configuration import Configuration
```

### Comparing `dmss-api-1.2.2/dmss_api/api/access_control_api.py` & `dmss-api-1.2.3/dmss_api/api/access_control_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/attribute_api.py` & `dmss-api-1.2.3/dmss_api/api/attribute_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,28 +34,28 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         def __attribute_get(
             self,
-            reference,
+            address,
             **kwargs
         ):
             """Get Attribute  # noqa: E501
 
-            Fetch the attribute from a reference.  # noqa: E501
+            Fetch the attribute from a address.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.attribute_get(reference, async_req=True)
+            >>> thread = api.attribute_get(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -94,58 +94,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.attribute_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/attribute/{reference}',
+                'endpoint_path': '/api/attribute/{address}',
                 'operation_id': 'attribute_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
```

### Comparing `dmss-api-1.2.2/dmss_api/api/blob_api.py` & `dmss-api-1.2.3/dmss_api/api/blob_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/blueprint_api.py` & `dmss-api-1.2.3/dmss_api/api/blueprint_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -170,28 +170,28 @@
             },
             api_client=api_client,
             callable=__blueprint_get
         )
 
         def __blueprint_resolve(
             self,
-            absolute_id,
+            address,
             **kwargs
         ):
             """Resolve Blueprint Id  # noqa: E501
 
-            Resolve absolute_id of a blueprint to its type path.  - **absolute_id**: <data_source</<blueprint_uuid>  # noqa: E501
+            Resolve address of a blueprint to its type path.  - **address**: <protocol>://<data_source</$<blueprint_uuid>  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.blueprint_resolve(absolute_id, async_req=True)
+            >>> thread = api.blueprint_resolve(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_id (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -230,58 +230,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_id'] = \
-                absolute_id
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.blueprint_resolve = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/resolve-path/{absolute_id}',
+                'endpoint_path': '/api/resolve-path/{address}',
                 'operation_id': 'blueprint_resolve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_id',
+                    'address',
                 ],
                 'required': [
-                    'absolute_id',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_id':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'absolute_id': 'absolute_id',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'absolute_id': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
```

### Comparing `dmss-api-1.2.2/dmss_api/api/datasource_api.py` & `dmss-api-1.2.3/dmss_api/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/default_api.py` & `dmss-api-1.2.3/dmss_api/api/default_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from dmss_api.model.data_source_information import DataSourceInformation
 from dmss_api.model.data_source_request import DataSourceRequest
 from dmss_api.model.entity import Entity
 from dmss_api.model.error_response import ErrorResponse
 from dmss_api.model.get_blueprint_response import GetBlueprintResponse
 from dmss_api.model.lookup import Lookup
 from dmss_api.model.pat_data import PATData
-from dmss_api.model.reference import Reference
+from dmss_api.model.reference_entity import ReferenceEntity
 
 
 class DefaultApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -42,28 +42,28 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         def __attribute_get(
             self,
-            reference,
+            address,
             **kwargs
         ):
             """Get Attribute  # noqa: E501
 
-            Fetch the attribute from a reference.  # noqa: E501
+            Fetch the attribute from a address.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.attribute_get(reference, async_req=True)
+            >>> thread = api.attribute_get(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -102,58 +102,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.attribute_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/attribute/{reference}',
+                'endpoint_path': '/api/attribute/{address}',
                 'operation_id': 'attribute_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -573,28 +573,28 @@
             },
             api_client=api_client,
             callable=__blueprint_get
         )
 
         def __blueprint_resolve(
             self,
-            absolute_id,
+            address,
             **kwargs
         ):
             """Resolve Blueprint Id  # noqa: E501
 
-            Resolve absolute_id of a blueprint to its type path.  - **absolute_id**: <data_source</<blueprint_uuid>  # noqa: E501
+            Resolve address of a blueprint to its type path.  - **address**: <protocol>://<data_source</$<blueprint_uuid>  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.blueprint_resolve(absolute_id, async_req=True)
+            >>> thread = api.blueprint_resolve(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                absolute_id (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -633,58 +633,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['absolute_id'] = \
-                absolute_id
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.blueprint_resolve = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/resolve-path/{absolute_id}',
+                'endpoint_path': '/api/resolve-path/{address}',
                 'operation_id': 'blueprint_resolve',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'absolute_id',
+                    'address',
                 ],
                 'required': [
-                    'absolute_id',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'absolute_id':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'absolute_id': 'absolute_id',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'absolute_id': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -1188,29 +1188,29 @@
             },
             api_client=api_client,
             callable=__data_source_save
         )
 
         def __document_add(
             self,
-            reference,
+            address,
             document,
             **kwargs
         ):
             """Add Document  # noqa: E501
 
-            Add a document to a package (or a data source) using a reference.  - **reference**:   - Reference to data source: PROTOCOL://DATA SOURCE   - Reference to package by id: PROTOCOL://DATA SOURCE/$ID   - Reference to package by path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE   The PROTOCOL is optional, and the default is dmss.  # noqa: E501
+            Add a document to a package (or a data source) using an address.  - **address**:   - Reference to data source: PROTOCOL://DATA SOURCE   - Reference to package by id: PROTOCOL://DATA SOURCE/$ID   - Reference to package by path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE   The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_add(reference, document, async_req=True)
+            >>> thread = api.document_add(address, document, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
                 document (str):
 
             Keyword Args:
                 update_uncontained (bool): [optional] if omitted the server will use the default value of False
                 files ([file_type]): [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
@@ -1252,41 +1252,41 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             kwargs['document'] = \
                 document
             return self.call_with_http_info(**kwargs)
 
         self.document_add = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{reference}',
+                'endpoint_path': '/api/documents/{address}',
                 'operation_id': 'document_add',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                     'document',
                     'update_uncontained',
                     'files',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                     'document',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -1294,31 +1294,31 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                     'document':
                         (str,),
                     'update_uncontained':
                         (bool,),
                     'files':
                         ([file_type],),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                     'document': 'document',
                     'update_uncontained': 'update_uncontained',
                     'files': 'files',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                     'document': 'form',
                     'update_uncontained': 'query',
                     'files': 'form',
                 },
                 'collection_format_map': {
                     'files': 'csv',
                 }
@@ -1466,28 +1466,28 @@
             },
             api_client=api_client,
             callable=__document_add_simple
         )
 
         def __document_get(
             self,
-            reference,
+            address,
             **kwargs
         ):
             """Get  # noqa: E501
 
-            Get document as JSON string.  - **reference**: A reference to a package or a data source   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)  The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
+            Get document as JSON string.  - **address**: An address to a package or a data source   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)  The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_get(reference, async_req=True)
+            >>> thread = api.document_get(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 depth (int): [optional] if omitted the server will use the default value of 0
                 resolve_links (bool): [optional] if omitted the server will use the default value of False
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -1528,66 +1528,66 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.document_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{reference}',
+                'endpoint_path': '/api/documents/{address}',
                 'operation_id': 'document_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                     'depth',
                     'resolve_links',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                     'depth':
                         (int,),
                     'resolve_links':
                         (bool,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                     'depth': 'depth',
                     'resolve_links': 'resolve_links',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                     'depth': 'query',
                     'resolve_links': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -1599,28 +1599,28 @@
             },
             api_client=api_client,
             callable=__document_get
         )
 
         def __document_remove(
             self,
-            reference,
+            address,
             **kwargs
         ):
             """Remove  # noqa: E501
 
             Remove a document from DMSS.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_remove(reference, async_req=True)
+            >>> thread = api.document_remove(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -1659,58 +1659,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.document_remove = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{reference}',
+                'endpoint_path': '/api/documents/{address}',
                 'operation_id': 'document_remove',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -1720,29 +1720,29 @@
             },
             api_client=api_client,
             callable=__document_remove
         )
 
         def __document_update(
             self,
-            id_reference,
+            id_address,
             data,
             **kwargs
         ):
             """Update  # noqa: E501
 
-            Update document - **id_reference**: <data_source>/<document_uuid> (can also include an optional .<attribute> after <document_uuid>)  # noqa: E501
+            Update document - **id_address**: <protocol>://<data_source>/$<document_uuid> (can also include an optional .<attribute> after <document_uuid>)  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_update(id_reference, data, async_req=True)
+            >>> thread = api.document_update(id_address, data, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                id_address (str):
                 data (str):
 
             Keyword Args:
                 update_uncontained (bool): [optional] if omitted the server will use the default value of False
                 files ([file_type]): [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
@@ -1784,41 +1784,41 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['id_address'] = \
+                id_address
             kwargs['data'] = \
                 data
             return self.call_with_http_info(**kwargs)
 
         self.document_update = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
+                'endpoint_path': '/api/documents/{id_address}',
                 'operation_id': 'document_update',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'id_address',
                     'data',
                     'update_uncontained',
                     'files',
                 ],
                 'required': [
-                    'id_reference',
+                    'id_address',
                     'data',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -1826,31 +1826,31 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'id_address':
                         (str,),
                     'data':
                         (str,),
                     'update_uncontained':
                         (bool,),
                     'files':
                         ([file_type],),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'id_address': 'id_address',
                     'data': 'data',
                     'update_uncontained': 'update_uncontained',
                     'files': 'files',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'id_address': 'path',
                     'data': 'form',
                     'update_uncontained': 'query',
                     'files': 'form',
                 },
                 'collection_format_map': {
                     'files': 'csv',
                 }
@@ -1866,28 +1866,28 @@
             },
             api_client=api_client,
             callable=__document_update
         )
 
         def __export(
             self,
-            reference,
+            path_address,
             **kwargs
         ):
             """Export  # noqa: E501
 
-            Download a zip-folder with one or more documents as json file(s).  - **reference**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
+            Download a zip-folder with one or more documents as json file(s).  - **address**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export(reference, async_req=True)
+            >>> thread = api.export(path_address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                path_address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -1926,58 +1926,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['path_address'] = \
+                path_address
             return self.call_with_http_info(**kwargs)
 
         self.export = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/{reference}',
+                'endpoint_path': '/api/export/{path_address}',
                 'operation_id': 'export',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'path_address',
                 ],
                 'required': [
-                    'reference',
+                    'path_address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'path_address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'path_address': 'path_address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'path_address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/zip',
@@ -1988,28 +1988,28 @@
             },
             api_client=api_client,
             callable=__export
         )
 
         def __export_meta(
             self,
-            reference,
+            path_address,
             **kwargs
         ):
             """Export Meta  # noqa: E501
 
-            Export only the metadata of an entity. An entities metadata is concatenated from the \"top down\". Inheriting parents meta, and overriding for any specified further down.  If no metadata is defined anywhere in the tree, an empty object is returned.  - **reference**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
+            Export only the metadata of an entity. An entities metadata is concatenated from the \"top down\". Inheriting parents meta, and overriding for any specified further down.  If no metadata is defined anywhere in the tree, an empty object is returned.  - **address**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export_meta(reference, async_req=True)
+            >>> thread = api.export_meta(path_address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                path_address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -2048,58 +2048,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['path_address'] = \
+                path_address
             return self.call_with_http_info(**kwargs)
 
         self.export_meta = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/meta/{reference}',
+                'endpoint_path': '/api/export/meta/{path_address}',
                 'operation_id': 'export_meta',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'path_address',
                 ],
                 'required': [
-                    'reference',
+                    'path_address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'path_address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'path_address': 'path_address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'path_address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -2107,14 +2107,157 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client,
             callable=__export_meta
         )
 
+        def __file_upload(
+            self,
+            data_source_id,
+            data,
+            file,
+            **kwargs
+        ):
+            """Upload File  # noqa: E501
+
+            Upload a new binary file and create a file entity with the binary data as content.  **file_id** The data source ID to be used for the file entity that will be created.  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.file_upload(data_source_id, data, file, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                data_source_id (str):
+                data (str):
+                file (file_type):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (int/float/tuple): timeout setting for this request. If
+                    one number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['data_source_id'] = \
+                data_source_id
+            kwargs['data'] = \
+                data
+            kwargs['file'] = \
+                file
+            return self.call_with_http_info(**kwargs)
+
+        self.file_upload = _Endpoint(
+            settings={
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'auth': [
+                    'APIKeyHeader',
+                    'OAuth2AuthorizationCodeBearer'
+                ],
+                'endpoint_path': '/api/files/{data_source_id}',
+                'operation_id': 'file_upload',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_source_id',
+                    'data',
+                    'file',
+                ],
+                'required': [
+                    'data_source_id',
+                    'data',
+                    'file',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_source_id':
+                        (str,),
+                    'data':
+                        (str,),
+                    'file':
+                        (file_type,),
+                },
+                'attribute_map': {
+                    'data_source_id': 'data_source_id',
+                    'data': 'data',
+                    'file': 'file',
+                },
+                'location_map': {
+                    'data_source_id': 'path',
+                    'data': 'form',
+                    'file': 'form',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json',
+                    'text/plain'
+                ],
+                'content_type': [
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client,
+            callable=__file_upload
+        )
+
         def __get_acl(
             self,
             data_source_id,
             document_id,
             **kwargs
         ):
             """Get Acl  # noqa: E501
@@ -2587,32 +2730,32 @@
                     'application/json'
                 ]
             },
             api_client=api_client,
             callable=__instantiate_entity
         )
 
-        def __reference_delete(
+        def __meta_by_id(
             self,
             data_source_id,
-            document_dotted_id,
+            document_id,
             **kwargs
         ):
-            """Delete Reference  # noqa: E501
+            """Get Meta By Id  # noqa: E501
 
-            Delete a reference in an entity.  Used to delete uncontained attributes in an entity.  - **document_dotted_id**: <data_source>/<path_to_entity>/<entity_name>.<attribute>  # noqa: E501
+            Get meta information from data source id.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.reference_delete(data_source_id, document_dotted_id, async_req=True)
+            >>> thread = api.meta_by_id(data_source_id, document_id, async_req=True)
             >>> result = thread.get()
 
             Args:
                 data_source_id (str):
-                document_dotted_id (str):
+                document_id (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -2653,38 +2796,38 @@
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
             kwargs['data_source_id'] = \
                 data_source_id
-            kwargs['document_dotted_id'] = \
-                document_dotted_id
+            kwargs['document_id'] = \
+                document_id
             return self.call_with_http_info(**kwargs)
 
-        self.reference_delete = _Endpoint(
+        self.meta_by_id = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/reference/{data_source_id}/{document_dotted_id}',
-                'operation_id': 'reference_delete',
-                'http_method': 'DELETE',
+                'endpoint_path': '/api/meta/{data_source_id}/{document_id}',
+                'operation_id': 'meta_by_id',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'data_source_id',
-                    'document_dotted_id',
+                    'document_id',
                 ],
                 'required': [
                     'data_source_id',
-                    'document_dotted_id',
+                    'document_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -2693,24 +2836,145 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'data_source_id':
                         (str,),
-                    'document_dotted_id':
+                    'document_id':
                         (str,),
                 },
                 'attribute_map': {
                     'data_source_id': 'data_source_id',
-                    'document_dotted_id': 'document_dotted_id',
+                    'document_id': 'document_id',
                 },
                 'location_map': {
                     'data_source_id': 'path',
-                    'document_dotted_id': 'path',
+                    'document_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json',
+                    'text/plain'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client,
+            callable=__meta_by_id
+        )
+
+        def __reference_delete(
+            self,
+            address,
+            **kwargs
+        ):
+            """Delete Reference  # noqa: E501
+
+            Delete a reference in an entity.  Used to delete uncontained attributes in an entity.  - **document_dotted_id**: <data_source>/<path_to_entity>/<entity_name>.<attribute>  # noqa: E501
+            This method makes a synchronous HTTP request by default. To make an
+            asynchronous HTTP request, please pass async_req=True
+
+            >>> thread = api.reference_delete(address, async_req=True)
+            >>> result = thread.get()
+
+            Args:
+                address (str):
+
+            Keyword Args:
+                _return_http_data_only (bool): response data without head status
+                    code and headers. Default is True.
+                _preload_content (bool): if False, the urllib3.HTTPResponse object
+                    will be returned without reading/decoding response data.
+                    Default is True.
+                _request_timeout (int/float/tuple): timeout setting for this request. If
+                    one number provided, it will be total request timeout. It can also
+                    be a pair (tuple) of (connection, read) timeouts.
+                    Default is None.
+                _check_input_type (bool): specifies if type checking
+                    should be done one the data sent to the server.
+                    Default is True.
+                _check_return_type (bool): specifies if type checking
+                    should be done one the data received from the server.
+                    Default is True.
+                _host_index (int/None): specifies the index of the server
+                    that we want to use.
+                    Default is read from the configuration.
+                async_req (bool): execute request asynchronously
+
+            Returns:
+                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+                    If the method is called asynchronously, returns the request
+                    thread.
+            """
+            kwargs['async_req'] = kwargs.get(
+                'async_req', False
+            )
+            kwargs['_return_http_data_only'] = kwargs.get(
+                '_return_http_data_only', True
+            )
+            kwargs['_preload_content'] = kwargs.get(
+                '_preload_content', True
+            )
+            kwargs['_request_timeout'] = kwargs.get(
+                '_request_timeout', None
+            )
+            kwargs['_check_input_type'] = kwargs.get(
+                '_check_input_type', True
+            )
+            kwargs['_check_return_type'] = kwargs.get(
+                '_check_return_type', True
+            )
+            kwargs['_host_index'] = kwargs.get('_host_index')
+            kwargs['address'] = \
+                address
+            return self.call_with_http_info(**kwargs)
+
+        self.reference_delete = _Endpoint(
+            settings={
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'auth': [
+                    'APIKeyHeader',
+                    'OAuth2AuthorizationCodeBearer'
+                ],
+                'endpoint_path': '/api/reference/{address}',
+                'operation_id': 'reference_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'address',
+                ],
+                'required': [
+                    'address',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'address':
+                        (str,),
+                },
+                'attribute_map': {
+                    'address': 'address',
+                },
+                'location_map': {
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -2720,32 +2984,30 @@
             },
             api_client=api_client,
             callable=__reference_delete
         )
 
         def __reference_insert(
             self,
-            data_source_id,
-            document_dotted_id,
-            reference,
+            address,
+            reference_entity,
             **kwargs
         ):
             """Insert Reference  # noqa: E501
 
             Add reference to an entity.  Used to add uncontained attributes to an entity.  - **document_dotted_id**: <data_source>/<path_to_entity>/<entity_name>.<attribute> - **reference**: a reference object in JSON format  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.reference_insert(data_source_id, document_dotted_id, reference, async_req=True)
+            >>> thread = api.reference_insert(address, reference_entity, async_req=True)
             >>> result = thread.get()
 
             Args:
-                data_source_id (str):
-                document_dotted_id (str):
-                reference (Reference):
+                address (str):
+                reference_entity (ReferenceEntity):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -2784,73 +3046,65 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['data_source_id'] = \
-                data_source_id
-            kwargs['document_dotted_id'] = \
-                document_dotted_id
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
+            kwargs['reference_entity'] = \
+                reference_entity
             return self.call_with_http_info(**kwargs)
 
         self.reference_insert = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/reference/{data_source_id}/{document_dotted_id}',
+                'endpoint_path': '/api/reference/{address}',
                 'operation_id': 'reference_insert',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'data_source_id',
-                    'document_dotted_id',
-                    'reference',
+                    'address',
+                    'reference_entity',
                 ],
                 'required': [
-                    'data_source_id',
-                    'document_dotted_id',
-                    'reference',
+                    'address',
+                    'reference_entity',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'data_source_id':
-                        (str,),
-                    'document_dotted_id':
+                    'address':
                         (str,),
-                    'reference':
-                        (Reference,),
+                    'reference_entity':
+                        (ReferenceEntity,),
                 },
                 'attribute_map': {
-                    'data_source_id': 'data_source_id',
-                    'document_dotted_id': 'document_dotted_id',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'data_source_id': 'path',
-                    'document_dotted_id': 'path',
-                    'reference': 'body',
+                    'address': 'path',
+                    'reference_entity': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
```

### Comparing `dmss-api-1.2.2/dmss_api/api/document_api.py` & `dmss-api-1.2.3/dmss_api/api/document_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,29 +34,29 @@
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         def __document_add(
             self,
-            reference,
+            address,
             document,
             **kwargs
         ):
             """Add Document  # noqa: E501
 
-            Add a document to a package (or a data source) using a reference.  - **reference**:   - Reference to data source: PROTOCOL://DATA SOURCE   - Reference to package by id: PROTOCOL://DATA SOURCE/$ID   - Reference to package by path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE   The PROTOCOL is optional, and the default is dmss.  # noqa: E501
+            Add a document to a package (or a data source) using an address.  - **address**:   - Reference to data source: PROTOCOL://DATA SOURCE   - Reference to package by id: PROTOCOL://DATA SOURCE/$ID   - Reference to package by path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE   The PROTOCOL is optional, and the default is dmss.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_add(reference, document, async_req=True)
+            >>> thread = api.document_add(address, document, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
                 document (str):
 
             Keyword Args:
                 update_uncontained (bool): [optional] if omitted the server will use the default value of False
                 files ([file_type]): [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
@@ -98,41 +98,41 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             kwargs['document'] = \
                 document
             return self.call_with_http_info(**kwargs)
 
         self.document_add = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{reference}',
+                'endpoint_path': '/api/documents/{address}',
                 'operation_id': 'document_add',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                     'document',
                     'update_uncontained',
                     'files',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                     'document',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -140,31 +140,31 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                     'document':
                         (str,),
                     'update_uncontained':
                         (bool,),
                     'files':
                         ([file_type],),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                     'document': 'document',
                     'update_uncontained': 'update_uncontained',
                     'files': 'files',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                     'document': 'form',
                     'update_uncontained': 'query',
                     'files': 'form',
                 },
                 'collection_format_map': {
                     'files': 'csv',
                 }
@@ -312,28 +312,28 @@
             },
             api_client=api_client,
             callable=__document_add_simple
         )
 
         def __document_get(
             self,
-            reference,
+            address,
             **kwargs
         ):
             """Get  # noqa: E501
 
-            Get document as JSON string.  - **reference**: A reference to a package or a data source   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)  The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
+            Get document as JSON string.  - **address**: An address to a package or a data source   - By id: PROTOCOL://DATA SOURCE/$ID.Attribute   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY.Attribute   - By query: PROTOCOL://DATA SOURCE/$ID.list(key=value)  The PROTOCOL is optional, and the default is dmss.  - **depth**: Maximum depth for resolving nested documents.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_get(reference, async_req=True)
+            >>> thread = api.document_get(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 depth (int): [optional] if omitted the server will use the default value of 0
                 resolve_links (bool): [optional] if omitted the server will use the default value of False
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -374,66 +374,66 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.document_get = _Endpoint(
             settings={
                 'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{reference}',
+                'endpoint_path': '/api/documents/{address}',
                 'operation_id': 'document_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                     'depth',
                     'resolve_links',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                     'depth':
                         (int,),
                     'resolve_links':
                         (bool,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                     'depth': 'depth',
                     'resolve_links': 'resolve_links',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                     'depth': 'query',
                     'resolve_links': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
@@ -445,28 +445,28 @@
             },
             api_client=api_client,
             callable=__document_get
         )
 
         def __document_remove(
             self,
-            reference,
+            address,
             **kwargs
         ):
             """Remove  # noqa: E501
 
             Remove a document from DMSS.  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_remove(reference, async_req=True)
+            >>> thread = api.document_remove(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -505,58 +505,58 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
         self.document_remove = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{reference}',
+                'endpoint_path': '/api/documents/{address}',
                 'operation_id': 'document_remove',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -566,29 +566,29 @@
             },
             api_client=api_client,
             callable=__document_remove
         )
 
         def __document_update(
             self,
-            id_reference,
+            id_address,
             data,
             **kwargs
         ):
             """Update  # noqa: E501
 
-            Update document - **id_reference**: <data_source>/<document_uuid> (can also include an optional .<attribute> after <document_uuid>)  # noqa: E501
+            Update document - **id_address**: <protocol>://<data_source>/$<document_uuid> (can also include an optional .<attribute> after <document_uuid>)  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.document_update(id_reference, data, async_req=True)
+            >>> thread = api.document_update(id_address, data, async_req=True)
             >>> result = thread.get()
 
             Args:
-                id_reference (str):
+                id_address (str):
                 data (str):
 
             Keyword Args:
                 update_uncontained (bool): [optional] if omitted the server will use the default value of False
                 files ([file_type]): [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
@@ -630,41 +630,41 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['id_reference'] = \
-                id_reference
+            kwargs['id_address'] = \
+                id_address
             kwargs['data'] = \
                 data
             return self.call_with_http_info(**kwargs)
 
         self.document_update = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/documents/{id_reference}',
+                'endpoint_path': '/api/documents/{id_address}',
                 'operation_id': 'document_update',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'id_reference',
+                    'id_address',
                     'data',
                     'update_uncontained',
                     'files',
                 ],
                 'required': [
-                    'id_reference',
+                    'id_address',
                     'data',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -672,31 +672,31 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'id_reference':
+                    'id_address':
                         (str,),
                     'data':
                         (str,),
                     'update_uncontained':
                         (bool,),
                     'files':
                         ([file_type],),
                 },
                 'attribute_map': {
-                    'id_reference': 'id_reference',
+                    'id_address': 'id_address',
                     'data': 'data',
                     'update_uncontained': 'update_uncontained',
                     'files': 'files',
                 },
                 'location_map': {
-                    'id_reference': 'path',
+                    'id_address': 'path',
                     'data': 'form',
                     'update_uncontained': 'query',
                     'files': 'form',
                 },
                 'collection_format_map': {
                     'files': 'csv',
                 }
```

### Comparing `dmss-api-1.2.2/dmss_api/api/entity_api.py` & `dmss-api-1.2.3/dmss_api/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/export_api.py` & `dmss-api-1.2.3/dmss_api/api/reference_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,44 +18,45 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from dmss_api.model.error_response import ErrorResponse
+from dmss_api.model.reference_entity import ReferenceEntity
 
 
-class ExportApi(object):
+class ReferenceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-        def __export(
+        def __reference_delete(
             self,
-            reference,
+            address,
             **kwargs
         ):
-            """Export  # noqa: E501
+            """Delete Reference  # noqa: E501
 
-            Download a zip-folder with one or more documents as json file(s).  - **reference**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
+            Delete a reference in an entity.  Used to delete uncontained attributes in an entity.  - **document_dotted_id**: <data_source>/<path_to_entity>/<entity_name>.<attribute>  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export(reference, async_req=True)
+            >>> thread = api.reference_delete(address, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -71,15 +72,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                None
+                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -94,90 +95,91 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
             return self.call_with_http_info(**kwargs)
 
-        self.export = _Endpoint(
+        self.reference_delete = _Endpoint(
             settings={
-                'response_type': None,
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/{reference}',
-                'operation_id': 'export',
-                'http_method': 'GET',
+                'endpoint_path': '/api/reference/{address}',
+                'operation_id': 'reference_delete',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
                 ],
                 'required': [
-                    'reference',
+                    'address',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/zip',
                     'application/json',
                     'text/plain'
                 ],
                 'content_type': [],
             },
             api_client=api_client,
-            callable=__export
+            callable=__reference_delete
         )
 
-        def __export_meta(
+        def __reference_insert(
             self,
-            reference,
+            address,
+            reference_entity,
             **kwargs
         ):
-            """Export Meta  # noqa: E501
+            """Insert Reference  # noqa: E501
 
-            Export only the metadata of an entity. An entities metadata is concatenated from the \"top down\". Inheriting parents meta, and overriding for any specified further down.  If no metadata is defined anywhere in the tree, an empty object is returned.  - **reference**:   - By path: PROTOCOL://DATA SOURCE/ROOT PACKAGE/SUB PACKAGE/ENTITY    The PROTOCOL is optional, and the default is dmss.  # noqa: E501
+            Add reference to an entity.  Used to add uncontained attributes to an entity.  - **document_dotted_id**: <data_source>/<path_to_entity>/<entity_name>.<attribute> - **reference**: a reference object in JSON format  # noqa: E501
             This method makes a synchronous HTTP request by default. To make an
             asynchronous HTTP request, please pass async_req=True
 
-            >>> thread = api.export_meta(reference, async_req=True)
+            >>> thread = api.reference_insert(address, reference_entity, async_req=True)
             >>> result = thread.get()
 
             Args:
-                reference (str):
+                address (str):
+                reference_entity (ReferenceEntity):
 
             Keyword Args:
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
@@ -193,15 +195,15 @@
                     Default is True.
                 _host_index (int/None): specifies the index of the server
                     that we want to use.
                     Default is read from the configuration.
                 async_req (bool): execute request asynchronously
 
             Returns:
-                bool, date, datetime, dict, float, int, list, str, none_type
+                {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
                     If the method is called asynchronously, returns the request
                     thread.
             """
             kwargs['async_req'] = kwargs.get(
                 'async_req', False
             )
             kwargs['_return_http_data_only'] = kwargs.get(
@@ -216,65 +218,74 @@
             kwargs['_check_input_type'] = kwargs.get(
                 '_check_input_type', True
             )
             kwargs['_check_return_type'] = kwargs.get(
                 '_check_return_type', True
             )
             kwargs['_host_index'] = kwargs.get('_host_index')
-            kwargs['reference'] = \
-                reference
+            kwargs['address'] = \
+                address
+            kwargs['reference_entity'] = \
+                reference_entity
             return self.call_with_http_info(**kwargs)
 
-        self.export_meta = _Endpoint(
+        self.reference_insert = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
                 'auth': [
                     'APIKeyHeader',
                     'OAuth2AuthorizationCodeBearer'
                 ],
-                'endpoint_path': '/api/export/meta/{reference}',
-                'operation_id': 'export_meta',
-                'http_method': 'GET',
+                'endpoint_path': '/api/reference/{address}',
+                'operation_id': 'reference_insert',
+                'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'reference',
+                    'address',
+                    'reference_entity',
                 ],
                 'required': [
-                    'reference',
+                    'address',
+                    'reference_entity',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'reference':
+                    'address':
                         (str,),
+                    'reference_entity':
+                        (ReferenceEntity,),
                 },
                 'attribute_map': {
-                    'reference': 'reference',
+                    'address': 'address',
                 },
                 'location_map': {
-                    'reference': 'path',
+                    'address': 'path',
+                    'reference_entity': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
                     'text/plain'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client,
-            callable=__export_meta
+            callable=__reference_insert
         )
```

### Comparing `dmss-api-1.2.2/dmss_api/api/health_check_api.py` & `dmss-api-1.2.3/dmss_api/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/lookup_table_api.py` & `dmss-api-1.2.3/dmss_api/api/lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/personal_access_token_api.py` & `dmss-api-1.2.3/dmss_api/api/personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/search_api.py` & `dmss-api-1.2.3/dmss_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api/whoami_api.py` & `dmss-api-1.2.3/dmss_api/api/whoami_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/api_client.py` & `dmss-api-1.2.3/dmss_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.2.2/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.3/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `dmss-api-1.2.2/dmss_api/apis/__init__.py` & `dmss-api-1.2.3/dmss_api/apis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,15 @@
 from dmss_api.api.blob_api import BlobApi
 from dmss_api.api.blueprint_api import BlueprintApi
 from dmss_api.api.datasource_api import DatasourceApi
 from dmss_api.api.default_api import DefaultApi
 from dmss_api.api.document_api import DocumentApi
 from dmss_api.api.entity_api import EntityApi
 from dmss_api.api.export_api import ExportApi
+from dmss_api.api.file_api import FileApi
 from dmss_api.api.health_check_api import HealthCheckApi
 from dmss_api.api.lookup_table_api import LookupTableApi
+from dmss_api.api.meta_api import MetaApi
 from dmss_api.api.personal_access_token_api import PersonalAccessTokenApi
 from dmss_api.api.reference_api import ReferenceApi
 from dmss_api.api.search_api import SearchApi
 from dmss_api.api.whoami_api import WhoamiApi
```

### Comparing `dmss-api-1.2.2/dmss_api/configuration.py` & `dmss-api-1.2.3/dmss_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 1.2.2".\
+               "SDK Package Version: 1.2.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `dmss-api-1.2.2/dmss_api/exceptions.py` & `dmss-api-1.2.3/dmss_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/access_level.py` & `dmss-api-1.2.3/dmss_api/model/access_level.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/acl.py` & `dmss-api-1.2.3/dmss_api/model/acl.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/data_source_information.py` & `dmss-api-1.2.3/dmss_api/model/data_source_information.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/data_source_request.py` & `dmss-api-1.2.3/dmss_api/model/data_source_request.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/entity.py` & `dmss-api-1.2.3/dmss_api/model/entity.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/error_response.py` & `dmss-api-1.2.3/dmss_api/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/get_blueprint_response.py` & `dmss-api-1.2.3/dmss_api/model/get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/lookup.py` & `dmss-api-1.2.3/dmss_api/model/lookup.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/pat_data.py` & `dmss-api-1.2.3/dmss_api/model/pat_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pat_hash (str): [optional]  # noqa: E501
-            uuid (str): [optional] if omitted the server will use the default value of "2a858b71-956f-4139-86a2-a7cf38d1b35b"  # noqa: E501
+            uuid (str): [optional] if omitted the server will use the default value of "057464f3-f376-4fcc-84e7-5c6bc6999298"  # noqa: E501
             roles ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -244,15 +244,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             pat_hash (str): [optional]  # noqa: E501
-            uuid (str): [optional] if omitted the server will use the default value of "2a858b71-956f-4139-86a2-a7cf38d1b35b"  # noqa: E501
+            uuid (str): [optional] if omitted the server will use the default value of "057464f3-f376-4fcc-84e7-5c6bc6999298"  # noqa: E501
             roles ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `dmss-api-1.2.2/dmss_api/model/recipe.py` & `dmss-api-1.2.3/dmss_api/model/recipe.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/recipe_attribute.py` & `dmss-api-1.2.3/dmss_api/model/recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/reference.py` & `dmss-api-1.2.3/dmss_api/model/reference_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from dmss_api.exceptions import ApiAttributeError
 
 
 
-class Reference(ModelNormal):
+class ReferenceEntity(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -108,15 +108,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, address, type, reference_type, *args, **kwargs):  # noqa: E501
-        """Reference - a model defined in OpenAPI
+        """ReferenceEntity - a model defined in OpenAPI
 
         Args:
             address (str):
             type (str):
             reference_type (str):
 
         Keyword Args:
@@ -197,15 +197,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, address, type, reference_type, *args, **kwargs):  # noqa: E501
-        """Reference - a model defined in OpenAPI
+        """ReferenceEntity - a model defined in OpenAPI
 
         Args:
             address (str):
             type (str):
             reference_type (str):
 
         Keyword Args:
```

### Comparing `dmss-api-1.2.2/dmss_api/model/repository.py` & `dmss-api-1.2.3/dmss_api/model/repository.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/repository_type.py` & `dmss-api-1.2.3/dmss_api/model/repository_type.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/storage_attribute.py` & `dmss-api-1.2.3/dmss_api/model/storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/storage_data_types.py` & `dmss-api-1.2.3/dmss_api/model/storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model/storage_recipe.py` & `dmss-api-1.2.3/dmss_api/model/storage_recipe.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/model_utils.py` & `dmss-api-1.2.3/dmss_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api/models/__init__.py` & `dmss-api-1.2.3/dmss_api/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 from dmss_api.model.entity import Entity
 from dmss_api.model.error_response import ErrorResponse
 from dmss_api.model.get_blueprint_response import GetBlueprintResponse
 from dmss_api.model.lookup import Lookup
 from dmss_api.model.pat_data import PATData
 from dmss_api.model.recipe import Recipe
 from dmss_api.model.recipe_attribute import RecipeAttribute
-from dmss_api.model.reference import Reference
+from dmss_api.model.reference_entity import ReferenceEntity
 from dmss_api.model.repository import Repository
 from dmss_api.model.repository_type import RepositoryType
 from dmss_api.model.storage_attribute import StorageAttribute
 from dmss_api.model.storage_data_types import StorageDataTypes
 from dmss_api.model.storage_recipe import StorageRecipe
```

### Comparing `dmss-api-1.2.2/dmss_api/rest.py` & `dmss-api-1.2.3/dmss_api/rest.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/dmss_api.egg-info/SOURCES.txt` & `dmss-api-1.2.3/dmss_api.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 dmss_api/api/blob_api.py
 dmss_api/api/blueprint_api.py
 dmss_api/api/datasource_api.py
 dmss_api/api/default_api.py
 dmss_api/api/document_api.py
 dmss_api/api/entity_api.py
 dmss_api/api/export_api.py
+dmss_api/api/file_api.py
 dmss_api/api/health_check_api.py
 dmss_api/api/lookup_table_api.py
+dmss_api/api/meta_api.py
 dmss_api/api/personal_access_token_api.py
 dmss_api/api/reference_api.py
 dmss_api/api/search_api.py
 dmss_api/api/whoami_api.py
 dmss_api/apis/__init__.py
 dmss_api/model/__init__.py
 dmss_api/model/access_level.py
@@ -37,15 +39,15 @@
 dmss_api/model/entity.py
 dmss_api/model/error_response.py
 dmss_api/model/get_blueprint_response.py
 dmss_api/model/lookup.py
 dmss_api/model/pat_data.py
 dmss_api/model/recipe.py
 dmss_api/model/recipe_attribute.py
-dmss_api/model/reference.py
+dmss_api/model/reference_entity.py
 dmss_api/model/repository.py
 dmss_api/model/repository_type.py
 dmss_api/model/storage_attribute.py
 dmss_api/model/storage_data_types.py
 dmss_api/model/storage_recipe.py
 dmss_api/models/__init__.py
 test/test_access_control_api.py
@@ -59,24 +61,26 @@
 test/test_datasource_api.py
 test/test_default_api.py
 test/test_document_api.py
 test/test_entity.py
 test/test_entity_api.py
 test/test_error_response.py
 test/test_export_api.py
+test/test_file_api.py
 test/test_get_blueprint_response.py
 test/test_health_check_api.py
 test/test_lookup.py
 test/test_lookup_table_api.py
+test/test_meta_api.py
 test/test_pat_data.py
 test/test_personal_access_token_api.py
 test/test_recipe.py
 test/test_recipe_attribute.py
-test/test_reference.py
 test/test_reference_api.py
+test/test_reference_entity.py
 test/test_repository.py
 test/test_repository_type.py
 test/test_search_api.py
 test/test_storage_attribute.py
 test/test_storage_data_types.py
 test/test_storage_recipe.py
 test/test_whoami_api.py
```

### Comparing `dmss-api-1.2.2/setup.py` & `dmss-api-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "dmss-api"
-VERSION = "1.2.2"
+VERSION = "1.2.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `dmss-api-1.2.2/test/test_access_control_api.py` & `dmss-api-1.2.3/test/test_access_control_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_access_level.py` & `dmss-api-1.2.3/test/test_access_level.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_acl.py` & `dmss-api-1.2.3/test/test_acl.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_attribute_api.py` & `dmss-api-1.2.3/test/test_attribute_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_blob_api.py` & `dmss-api-1.2.3/test/test_blob_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_blueprint_api.py` & `dmss-api-1.2.3/test/test_blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_data_source_information.py` & `dmss-api-1.2.3/test/test_data_source_information.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_data_source_request.py` & `dmss-api-1.2.3/test/test_data_source_request.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_datasource_api.py` & `dmss-api-1.2.3/test/test_datasource_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_default_api.py` & `dmss-api-1.2.3/test/test_default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,21 @@
     def test_export_meta(self):
         """Test case for export_meta
 
         Export Meta  # noqa: E501
         """
         pass
 
+    def test_file_upload(self):
+        """Test case for file_upload
+
+        Upload File  # noqa: E501
+        """
+        pass
+
     def test_get_acl(self):
         """Test case for get_acl
 
         Get Acl  # noqa: E501
         """
         pass
 
@@ -159,14 +166,21 @@
     def test_instantiate_entity(self):
         """Test case for instantiate_entity
 
         Instantiate  # noqa: E501
         """
         pass
 
+    def test_meta_by_id(self):
+        """Test case for meta_by_id
+
+        Get Meta By Id  # noqa: E501
+        """
+        pass
+
     def test_reference_delete(self):
         """Test case for reference_delete
 
         Delete Reference  # noqa: E501
         """
         pass
```

### Comparing `dmss-api-1.2.2/test/test_document_api.py` & `dmss-api-1.2.3/test/test_document_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_entity.py` & `dmss-api-1.2.3/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_entity_api.py` & `dmss-api-1.2.3/test/test_entity_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_error_response.py` & `dmss-api-1.2.3/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_export_api.py` & `dmss-api-1.2.3/test/test_export_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_get_blueprint_response.py` & `dmss-api-1.2.3/test/test_get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_health_check_api.py` & `dmss-api-1.2.3/test/test_health_check_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_lookup.py` & `dmss-api-1.2.3/test/test_lookup.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_lookup_table_api.py` & `dmss-api-1.2.3/test/test_lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_pat_data.py` & `dmss-api-1.2.3/test/test_pat_data.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_personal_access_token_api.py` & `dmss-api-1.2.3/test/test_personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_recipe.py` & `dmss-api-1.2.3/test/test_recipe.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_recipe_attribute.py` & `dmss-api-1.2.3/test/test_recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_reference.py` & `dmss-api-1.2.3/test/test_whoami_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,32 +4,32 @@
     API for basic data modelling interaction  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import dmss_api
-from dmss_api.model.reference import Reference
+from dmss_api.api.whoami_api import WhoamiApi  # noqa: E501
 
 
-class TestReference(unittest.TestCase):
-    """Reference unit test stubs"""
+class TestWhoamiApi(unittest.TestCase):
+    """WhoamiApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = WhoamiApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testReference(self):
-        """Test Reference"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = Reference()  # noqa: E501
+    def test_whoami(self):
+        """Test case for whoami
+
+        Get Information On Authenticated User  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dmss-api-1.2.2/test/test_reference_api.py` & `dmss-api-1.2.3/test/test_reference_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_repository.py` & `dmss-api-1.2.3/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_repository_type.py` & `dmss-api-1.2.3/test/test_repository_type.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_search_api.py` & `dmss-api-1.2.3/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_storage_attribute.py` & `dmss-api-1.2.3/test/test_storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_storage_data_types.py` & `dmss-api-1.2.3/test/test_storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dmss-api-1.2.2/test/test_storage_recipe.py` & `dmss-api-1.2.3/test/test_storage_recipe.py`

 * *Files identical despite different names*

