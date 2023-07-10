# Comparing `tmp/vectice-23.2.6.1.tar.gz` & `tmp/vectice-23.2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.6.1.tar", last modified: Wed Jun 28 14:24:04 2023, max compression
+gzip compressed data, was "vectice-23.2.7.0.tar", last modified: Mon Jul 10 08:19:24 2023, max compression
```

## Comparing `vectice-23.2.6.1.tar` & `vectice-23.2.7.0.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.416848 vectice-23.2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 14:23:48.000000 vectice-23.2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-28 14:24:04.416848 vectice-23.2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-28 14:23:48.000000 vectice-23.2.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-28 14:23:48.000000 vectice-23.2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-28 14:24:04.416848 vectice-23.2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-28 14:23:48.000000 vectice-23.2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.384848 vectice-23.2.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.384848 vectice-23.2.6.1/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.392848 vectice-23.2.6.1/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19481 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.400848 vectice-23.2.6.1/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    23656 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.404848 vectice-23.2.6.1/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14757 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.408848 vectice-23.2.6.1/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.408848 vectice-23.2.6.1/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.412848 vectice-23.2.6.1/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    30604 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.416848 vectice-23.2.6.1/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-28 14:23:48.000000 vectice-23.2.6.1/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:24:04.388848 vectice-23.2.6.1/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-28 14:24:04.000000 vectice-23.2.6.1/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-28 14:24:04.000000 vectice-23.2.6.1/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:24:04.000000 vectice-23.2.6.1/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 14:24:04.000000 vectice-23.2.6.1/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-28 14:24:04.000000 vectice-23.2.6.1/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 08:19:16.000000 vectice-23.2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-10 08:19:24.550819 vectice-23.2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 08:19:16.000000 vectice-23.2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 08:19:16.000000 vectice-23.2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 08:19:24.550819 vectice-23.2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-10 08:19:16.000000 vectice-23.2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.538819 vectice-23.2.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.538819 vectice-23.2.7.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.542819 vectice-23.2.7.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.546819 vectice-23.2.7.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.546819 vectice-23.2.7.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.546819 vectice-23.2.7.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.550819 vectice-23.2.7.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-10 08:19:16.000000 vectice-23.2.7.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:19:24.538819 vectice-23.2.7.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 08:19:24.000000 vectice-23.2.7.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.6.1/LICENSE` & `vectice-23.2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/PKG-INFO` & `vectice-23.2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.6.1
+Version: 23.2.7.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.6.1/setup.py` & `vectice-23.2.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,27 @@
     url="https://www.vectice.com",
     package_data={"vectice": ["py.typed"]},
     license="Apache License 2.0",
     keywords=["Vectice", "Client", "API", "Adapter"],
     platforms=["Linux", "MacOS X", "Windows"],
     python_requires=version_requires,
     install_requires=[
+        "types-python-dateutil",
         "python-dotenv>=0.11.0",
         "requests>=2.5.0",
         "rich",
         "urllib3",
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
         "pandas",
         "typing-extensions==4.6.2",
         "pyspark",
+        "dataclasses-json==0.5.8",
     ],
     extras_require={
         "dev": [
             "black",
             "gitpython",
             "mypy",
             "ruff",
```

### Comparing `vectice-23.2.6.1/src/vectice/__init__.py` & `vectice-23.2.7.0/src/vectice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,22 @@
 
 from vectice import api, models
 from vectice.__version__ import __version__
 from vectice.connection import Connection
 from vectice.models.dataset import Dataset
 from vectice.models.git_version import CodeSource
 from vectice.models.model import Metric, Model, Property
-from vectice.models.resource import BigQueryResource, FileResource, GCSResource, Resource, S3Resource
+from vectice.models.resource import (
+    BigQueryResource,
+    DatabricksTableResource,
+    FileResource,
+    GCSResource,
+    Resource,
+    S3Resource,
+)
 from vectice.models.resource.metadata import (
     DatasetSourceOrigin,
     DatasetSourceUsage,
     DatasetType,
     DBMetadata,
     File,
     FilesMetadata,
@@ -71,14 +78,15 @@
 version = __version__
 
 __all__ = [
     "api",
     "models",
     "version",
     "connect",
+    "DatabricksTableResource",
     "BigQueryResource",
     "Resource",
     "FileResource",
     "GCSResource",
     "S3Resource",
     "DatasetSourceUsage",
     "DatasetSourceOrigin",
```

### Comparing `vectice-23.2.6.1/src/vectice/api/__init__.py` & `vectice-23.2.7.0/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/_auth.py` & `vectice-23.2.7.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/attachment.py` & `vectice-23.2.7.0/src/vectice/api/attachment.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,32 +87,32 @@
         url, model_repr = self._generate_model_url_and_id(model_version)
         url += f"?modelFramework={model_type}"
         attachment = ("file", ("model_pickle", model_content))
         self._post_attachments(url, [attachment])
         _logger.info(f"Model {model_type} successfully attached to {model_repr}.")
 
     def _identify_object(
-        self, code_version_id: int | None = None, phase_id: str | None = None
+        self, code_version_id: int | None = None, iteration_id: str | None = None
     ) -> tuple[str, str | int]:
-        if phase_id:
-            return "phase", phase_id
+        if iteration_id:
+            return "iteration", iteration_id
         elif code_version_id:
             return "codeversion", code_version_id
         else:
             raise ValueError("No ID was provided for create attachment.")
 
     def create_attachments(
         self,
         files: list[tuple[str, tuple[str, Any]]],
         project_id: str,
         code_version_id: int | None = None,
-        phase_id: str | None = None,
+        iteration_id: str | None = None,
         step_id: int | None = None,
     ) -> list[dict]:
-        parent_object, object_id = self._identify_object(code_version_id, phase_id)
+        parent_object, object_id = self._identify_object(code_version_id, iteration_id)
         entity_files = []
         query_param = f"?stepId={step_id}" if step_id is not None else ""
         url = f"/metadata/project/{project_id}/entityfiles/{parent_object}/{object_id}{query_param}"
         try:
             for file in files:
                 response = self._post_attachments(url, [file])
                 if response:
```

### Comparing `vectice-23.2.6.1/src/vectice/api/client.py` & `vectice-23.2.7.0/src/vectice/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,33 +179,35 @@
             version: The version to attach files to.
 
         Returns:
             The JSON structure.
         """
         return AttachmentApi(self.auth).post_attachment(files, version)
 
-    def create_phase_attachments(
+    def create_iteration_attachments(
         self,
         files: list[tuple[str, tuple[str, BytesIO | IOBase]]],
-        phase_id: str,
+        iteration_id: str,
         project_id: str,
         step_id: int | None = None,
     ) -> list[dict]:
         """Create an attachment.
 
         Parameters:
             files: The paths to the files to attach.
-            phase_id: The phase id to attach files to.
+            iteration_id: The iteration id to attach files to.
             project_id: The project id to attach files to.
             step_id (Optional): The step id to add this attachment as an artifact of the step.
 
         Returns:
             The JSON structure.
         """
-        return AttachmentApi(self.auth).create_attachments(files, project_id, phase_id=phase_id, step_id=step_id)
+        return AttachmentApi(self.auth).create_attachments(
+            files, project_id, iteration_id=iteration_id, step_id=step_id
+        )
 
     def create_model_predictor(self, model_type: str, model_content: BytesIO, model_version: ModelVersionOutput):
         """Create a predictor.
 
         Parameters:
             model_type: The type of model to attach.
             model_content: The binary content of the model.
@@ -317,14 +319,17 @@
         phase_id: str | None = None,
         iteration_id: str | None = None,
         code_version_id: int | None = None,
     ) -> DatasetRegisterOutput:
         if dataset._has_bigquery_resource and self.is_feature_flag_enabled("bigquery-dataset-source") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("bigquery-dataset-source"))
 
+        if dataset._has_databricks_resource and self.is_feature_flag_enabled("databricks-dataset-source") is False:
+            raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("databricks-dataset-source"))
+
         if dataset._has_dataframe is True and self.is_feature_flag_enabled("dataset-dataframe") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("dataset-dataframe"))
 
         if dataset._has_spark_df is True and self.is_feature_flag_enabled("dataset-spark-dataframe") is False:
             raise VecticeException(DISABLED_FEATURE_FLAG_MESSAGE.format("dataset-spark-dataframe"))
 
         name = self.get_dataset_name(dataset)
@@ -336,17 +341,16 @@
                 resource.metadata.set_settings(
                     MetadataSettings(
                         minimum_rows_for_statistics=self._org_config.configuration.df_statistics_row_threshold
                     )
                 )
                 metadata_asdict.append(resource.metadata.asdict())
 
-        properties = (
-            [vars(PropertyInput(prop.key, prop.value)) for prop in dataset.properties] if dataset.properties else None
-        )
+        props = dataset.properties if dataset.properties is not None else []
+        properties = [vars(PropertyInput(prop.key, prop.value)) for prop in props]
 
         dataset_register_input = DatasetRegisterInput(
             name=name,
             type=dataset.type.value,
             datasetSources=metadata_asdict,
             inputs=derived_from,
             codeVersionId=code_version_id,
```

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_api.py` & `vectice-23.2.7.0/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_code.py` & `vectice-23.2.7.0/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_code_version.py` & `vectice-23.2.7.0/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_dataset.py` & `vectice-23.2.7.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_entity_file.py` & `vectice-23.2.7.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.7.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_model.py` & `vectice-23.2.7.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_organization.py` & `vectice-23.2.7.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.7.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/http_error.py` & `vectice-23.2.7.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/http_error_handlers.py` & `vectice-23.2.7.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/iteration.py` & `vectice-23.2.7.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/__init__.py` & `vectice-23.2.7.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/artifact_version.py` & `vectice-23.2.7.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/code.py` & `vectice-23.2.7.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/code_version.py` & `vectice-23.2.7.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/dataset_register.py` & `vectice-23.2.7.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/dataset_representation.py` & `vectice-23.2.7.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/dataset_version.py` & `vectice-23.2.7.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/dataset_version_representation.py` & `vectice-23.2.7.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/files_metadata.py` & `vectice-23.2.7.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/iteration.py` & `vectice-23.2.7.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/last_assets.py` & `vectice-23.2.7.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/metric.py` & `vectice-23.2.7.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/model.py` & `vectice-23.2.7.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/model_register.py` & `vectice-23.2.7.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/model_representation.py` & `vectice-23.2.7.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/model_version.py` & `vectice-23.2.7.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/model_version_representation.py` & `vectice-23.2.7.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/paged_response.py` & `vectice-23.2.7.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/phase.py` & `vectice-23.2.7.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/project.py` & `vectice-23.2.7.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/property.py` & `vectice-23.2.7.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/public_config.py` & `vectice-23.2.7.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/step.py` & `vectice-23.2.7.0/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/json/workspace.py` & `vectice-23.2.7.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/last_assets.py` & `vectice-23.2.7.0/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/phase.py` & `vectice-23.2.7.0/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/project.py` & `vectice-23.2.7.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/rest_api.py` & `vectice-23.2.7.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/step.py` & `vectice-23.2.7.0/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/version.py` & `vectice-23.2.7.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/api/workspace.py` & `vectice-23.2.7.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/connection.py` & `vectice-23.2.7.0/src/vectice/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,29 +10,28 @@
 
 import dotenv
 from rich.table import Table
 
 from vectice.api import Client
 from vectice.api.http_error_handlers import InvalidIdError
 from vectice.api.json.iteration import IterationOutput
-from vectice.api.json.last_assets import ActivityTargetType
 from vectice.api.json.phase import PhaseOutput
 from vectice.api.json.project import ProjectOutput
 from vectice.api.json.workspace import WorkspaceOutput
 from vectice.models.iteration import Iteration
 from vectice.models.phase import Phase
 from vectice.models.project import Project
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_representation import ModelRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 from vectice.models.workspace import Workspace
 from vectice.utils.common_utils import _temp_print, hide_logs
 from vectice.utils.configuration import Configuration
-from vectice.utils.last_assets import _connection_logging, _get_last_assets, _get_last_user_and_default_workspace
+from vectice.utils.last_assets import _connection_logging, _get_last_user_and_default_workspace
 from vectice.utils.logging_utils import CONNECTION_PROJECT_LOGGING, CONNECTION_WORKSPACE_LOGGING, format_description
 from vectice.utils.vectice_ids_regex import (
     DATASET_VERSION_VID_REG,
     DATASET_VID_REG,
     ITERATION_VID_REG,
     MODEL_VERSION_VID_REG,
     MODEL_VID_REG,
@@ -90,23 +89,14 @@
         str(Path.home() / ".vectice"),
         ".env",
         str(Path.home() / ".env"),
         "/etc/vectice/api.cfg",
     ]
 
     def __init__(self, api_token: str, host: str):
-        """Initialize a connection.
-
-        Parameters:
-            api_token: Your private api token.
-            host: The address of the Vectice application.
-
-        Raises:
-            RuntimeError: When the API and backend versions are incompatible.
-        """
         logging.getLogger("Client").propagate = True
         self._workspace: Workspace | None = None
         self._client = Client(token=api_token, api_endpoint=host)
         compatibility = self._client.check_compatibility()
         if compatibility.status != "OK":
             if compatibility.status == "Error":
                 _logger.error(f"compatibility error: {compatibility.message}")
@@ -125,57 +115,97 @@
     def version_api(self) -> str:
         return self._client.version_api
 
     @property
     def version_backend(self) -> str:
         return self._client.version_backend
 
-    def workspace(self, workspace: str) -> Workspace:
-        """Get a workspace.
-
-        Parameters:
-            workspace: The id or the name of the desired workspace.
+    @property
+    def my_workspace(self) -> Workspace:
+        """Retrieve your personal workspace.
 
         Returns:
-            The desired workspace.
+            Personal workspace.
         """
-        result = self._get_workspace_from_str(workspace)
-        logging_output = dedent(
-            f"""
-                        Workspace {result.name!r} successfully retrieved."
+        asset = self._client.get_user_and_default_workspace()
+        if not asset.get("defaultWorkspace"):
+            raise ValueError("Default workspace is not set.")
+        return self.workspace(asset["defaultWorkspace"]["vecticeId"])
 
-                        For quick access to the workspace in the Vectice web app, visit:
-                        {self._client.auth._API_BASE_URL}/browse/workspace/{result.id}"""
-        ).lstrip()
-        _logger.info(logging_output)
-        return result
+    @overload
+    @staticmethod
+    def connect(  # type: ignore[misc]
+        api_token: str | None = None,
+        host: str | None = None,
+        config: str | None = None,
+        workspace: str | None = None,
+        project: None = None,
+    ) -> Connection | Workspace | Project:
+        ...
 
-    def _build_workspace_from_output(self, output: WorkspaceOutput) -> Workspace:
-        workspace = Workspace(output.id, output.name, output.description)
-        workspace.__post_init__(self._client, self)
-        return workspace
+    @overload
+    @staticmethod
+    def connect(
+        api_token: str | None = None,
+        host: str | None = None,
+        config: str | None = None,
+        workspace: str | None = None,
+        project: str = "",
+    ) -> Project:
+        ...
 
-    def _build_project_from_output(self, output: ProjectOutput) -> Project:
-        workspace = self._build_workspace_from_output(output.workspace)
-        project = Project(output.id, workspace, output.name, output.description)
-        return project
+    @staticmethod
+    def connect(
+        api_token: str | None = None,
+        host: str | None = None,
+        config: str | None = None,
+        workspace: str | None = None,
+        project: str | None = None,
+    ) -> Connection | Workspace | Project:
+        """Method to connect to the Vectice backend (application).
 
-    def _build_phase_from_output(self, output: PhaseOutput) -> Phase:
-        if output.project is None:
-            raise RuntimeError("Failed to get back project from phase output")
-        project = self._build_project_from_output(output.project)
-        phase = Phase(output.id, project, output.name, output.index, output.status)
-        return phase
+        Authentication credentials are retrieved, in order, from:
 
-    def _build_iteration_from_output(self, output: IterationOutput) -> Iteration:
-        if output.phase is None:
-            raise RuntimeError("Failed to get back phase from iteration output")
-        phase = self._build_phase_from_output(output.phase)
-        iteration = Iteration(output.id, output.index, phase, output.status)
-        return iteration
+        1. keyword arguments
+        2. configuration file (`config` parameter)
+        3. environment variables
+        4. environment files in the following order
+            - `.vectice` of the working directory
+            - `.vectice` of the user home directory
+            - `.env` of the working directory
+            - `.env` of the user home directory
+            - `/etc/vectice/api.cfg` file
+
+        This method uses the `api_token`, `host`, `workspace`, `project` arguments
+        or the JSON config provided. The JSON config file is available from the Vectice
+        webapp when creating an API token.
+
+        Parameters:
+            api_token: The api token provided by the Vectice webapp.
+            host: The backend host to which the client will connect.
+                If not found, the default endpoint https://app.vectice.com is used.
+            config: A JSON config file containing keys VECTICE_API_TOKEN and
+                VECTICE_HOST as well as optionally WORKSPACE and PROJECT.
+            workspace: The name or id of an optional workspace to return.
+            project: The name or id of an optional project to return.
+
+        Returns:
+            A Connection, Workspace, or Project.
+        """
+        host = host or Connection._get_host(config)
+        api_token = api_token or Connection._get_api_token(host, config)
+        workspace = workspace or Connection._get_config_workspace(config)
+        project = project or Connection._get_config_project(config)
+        connection = Connection(api_token=api_token, host=host)
+        user_name, workspace_id = _get_last_user_and_default_workspace(connection._client)
+        url = connection._client.auth.api_base_url
+        if workspace:
+            return connection._log_workspace_or_project(workspace, project, user_name, url)
+        _connection_logging(_logger, user_name, url, workspace_id)
+        return connection
 
     def browse(
         self, asset: str
     ) -> (
         Workspace
         | Project
         | Phase
@@ -208,14 +238,58 @@
         elif re.search(DATASET_VID_REG, asset):
             return self.dataset(asset)
         elif re.search(DATASET_VERSION_VID_REG, asset):
             return self.dataset_version(asset)
 
         raise InvalidIdError("asset", asset)
 
+    def workspace(self, workspace: str) -> Workspace:
+        """Get a workspace.
+
+        Parameters:
+            workspace: The id or the name of the desired workspace.
+
+        Returns:
+            The desired workspace.
+        """
+        result = self._get_workspace_from_str(workspace)
+        logging_output = dedent(
+            f"""
+                        Workspace {result.name!r} successfully retrieved."
+
+                        For quick access to the workspace in the Vectice web app, visit:
+                        {self._client.auth._API_BASE_URL}/browse/workspace/{result.id}"""
+        ).lstrip()
+        _logger.info(logging_output)
+        return result
+
+    def _build_workspace_from_output(self, output: WorkspaceOutput) -> Workspace:
+        workspace = Workspace(output.id, output.name, output.description)
+        workspace.__post_init__(self._client, self)
+        return workspace
+
+    def _build_project_from_output(self, output: ProjectOutput) -> Project:
+        workspace = self._build_workspace_from_output(output.workspace)
+        project = Project(output.id, workspace, output.name, output.description)
+        return project
+
+    def _build_phase_from_output(self, output: PhaseOutput) -> Phase:
+        if output.project is None:
+            raise RuntimeError("Failed to get back project from phase output")
+        project = self._build_project_from_output(output.project)
+        phase = Phase(output.id, project, output.name, output.index, output.status)
+        return phase
+
+    def _build_iteration_from_output(self, output: IterationOutput) -> Iteration:
+        if output.phase is None:
+            raise RuntimeError("Failed to get back phase from iteration output")
+        phase = self._build_phase_from_output(output.phase)
+        iteration = Iteration(output.id, output.index, phase, output.status)
+        return iteration
+
     def project(self, project: str) -> Project:
         """Get a project.
 
         Parameters:
             project: The id of the desired project.
 
         Returns:
@@ -398,133 +472,14 @@
         {self._client.auth._API_BASE_URL}/workspaces"""
         ).lstrip()
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(tips)
         _temp_print(link)
 
-    @property
-    def workspaces(self) -> list[Workspace] | None:
-        """List the workspaces to which this connection has access.
-
-        Returns:
-            The workspaces to which this connection has access.
-        """
-        _, default_workspace_id = _get_last_user_and_default_workspace(self._client)
-        outputs = self._client.list_workspaces().list
-        results: list[Workspace] = []
-        for output in outputs:
-            workspace = Workspace(id=output.id, name=output.name, description=output.description)
-            workspace.__post_init__(self._client, self)
-            if output.id == default_workspace_id:
-                results.insert(0, workspace)
-                continue
-            results.append(workspace)
-        return results
-
-    @property
-    def my_workspace(self) -> Workspace:
-        """Retrieve your personal workspace.
-
-        Returns:
-            Personal workspace.
-        """
-        asset = self._client.get_user_and_default_workspace()
-        if not asset.get("defaultWorkspace"):
-            raise ValueError("Default workspace is not set.")
-        return self.workspace(asset["defaultWorkspace"]["vecticeId"])
-
-    @property
-    def last_workspace(self) -> Workspace:
-        """Retrieve last workspace with activity.
-
-        Returns:
-            Last workspace with activity.
-        """
-        target_types = [activity for activity in ActivityTargetType]
-        asset = _get_last_assets(target_types, self._client, _logger)
-        if not asset or not asset.get("workspace"):
-            raise ValueError("Workspace with activity not found.")
-        return self.workspace(asset["workspace"]["vecticeId"])
-
-    @overload
-    @staticmethod
-    def connect(  # type: ignore[misc]
-        api_token: str | None = None,
-        host: str | None = None,
-        config: str | None = None,
-        workspace: str | None = None,
-        project: None = None,
-    ) -> Connection | Workspace | Project:
-        ...
-
-    @overload
-    @staticmethod
-    def connect(
-        api_token: str | None = None,
-        host: str | None = None,
-        config: str | None = None,
-        workspace: str | None = None,
-        project: str = "",
-    ) -> Project:
-        ...
-
-    @staticmethod
-    def connect(
-        api_token: str | None = None,
-        host: str | None = None,
-        config: str | None = None,
-        workspace: str | None = None,
-        project: str | None = None,
-    ) -> Connection | Workspace | Project:
-        """Method to connect to the Vectice backend (application).
-
-        Authentication credentials are retrieved, in order, from:
-
-        1. keyword arguments
-        2. configuration file (`config` parameter)
-        3. environment variables
-        4. environment files in the following order
-            - `.vectice` of the working directory
-            - `.vectice` of the user home directory
-            - `.env` of the working directory
-            - `.env` of the user home directory
-            - `/etc/vectice/api.cfg` file
-
-        This method uses the `api_token`, `host`, `workspace`, `project` arguments
-        or the JSON config provided. The JSON config file is available from the Vectice
-        webapp when creating an API token.
-
-        Parameters:
-            api_token: The api token provided by the Vectice webapp.
-            host: The backend host to which the client will connect.
-                If not found, the default endpoint https://app.vectice.com is used.
-            config: A JSON config file containing keys VECTICE_API_TOKEN and
-                VECTICE_HOST as well as optionally WORKSPACE and PROJECT.
-            workspace: The name or id of an optional workspace to return.
-            project: The name or id of an optional project to return.
-
-        Raises:
-            ValueError: When a project is specified without a workspace.
-
-        Returns:
-            A Connection, Workspace, or Project.
-        """
-        host = host or Connection._get_host(config)
-        api_token = api_token or Connection._get_api_token(host, config)
-        workspace = workspace or Connection._get_config_workspace(config)
-        project = project or Connection._get_config_project(config)
-        connection = Connection(api_token=api_token, host=host)
-        user_name, workspace_id = _get_last_user_and_default_workspace(connection._client)
-        url = connection._client.auth.api_base_url
-        if workspace:
-            return connection._log_workspace_or_project(workspace, project, user_name, url)
-        _connection_logging(_logger, user_name, url, workspace_id)
-        return connection
-
     @staticmethod
     def _get_host(config: str | None) -> str:
         try:
             return Connection._get_config_item("VECTICE_HOST", config)
         except ValueError:
             # To remove in 23.3.1.0
             try:
```

### Comparing `vectice-23.2.6.1/src/vectice/models/__init__.py` & `vectice-23.2.7.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/attachment_container.py` & `vectice-23.2.7.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/dataset.py` & `vectice-23.2.7.0/src/vectice/models/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing_extensions import get_args
 
 from vectice.models.property import Property
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
+from vectice.models.resource.databricks_table_resource import DatabricksTableResource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
 
 _logger = logging.getLogger(__name__)
 
 
 TBaseDerivedFrom = Union[str, DatasetRepresentation, DatasetVersionRepresentation]
 
@@ -29,31 +30,14 @@
         training_resource: Resource | None = None,
         testing_resource: Resource | None = None,
         validation_resource: Resource | None = None,
         derived_from: list[TBaseDerivedFrom | Dataset] | TBaseDerivedFrom | Dataset | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
     ):
-        """Initialize a dataset.
-
-        Users should not instantiate a dataset directly but rather use the provided static methods
-        [`origin()`][vectice.models.dataset.Dataset.origin],
-        [`clean()`][vectice.models.dataset.Dataset.clean], and
-        [`modeling()`][vectice.models.dataset.Dataset.modeling].
-
-        Parameters:
-            type: The type of dataset.
-            name: The name of the dataset.
-            resource: A single resource (for origin and clean datasets).
-            training_resource: The resource for the training set (for modeling datasets).
-            testing_resource: The resource for the testing set (for modeling datasets).
-            validation_resource: The resource for the validation set (optional, for modeling datasets).
-            derived_from: A list of datasets (or ids) from which this dataset is derived.
-            attachments: Path of a file that will be attached to the step along with the dataset.
-        """
         self._type = type
         self._name = name or f"dataset {datetime.time}"
         self._resource = resource
         self._training_resource = training_resource
         self._testing_resource = testing_resource
         self._validation_resource = validation_resource
         self._derived_from = _get_derived_from(derived_from)
@@ -72,14 +56,20 @@
 
         self._has_bigquery_resource = (
             isinstance(self._resource, BigQueryResource)
             or isinstance(self._training_resource, BigQueryResource)
             or isinstance(self._testing_resource, BigQueryResource)
             or isinstance(self._validation_resource, BigQueryResource)
         )
+        self._has_databricks_resource = (
+            isinstance(self._resource, DatabricksTableResource)
+            or isinstance(self._training_resource, DatabricksTableResource)
+            or isinstance(self._testing_resource, DatabricksTableResource)
+            or isinstance(self._validation_resource, DatabricksTableResource)
+        )
         self._has_dataframe = (
             (self._resource is not None and self._resource._dataframes is not None)
             or (self._training_resource is not None and self._training_resource._dataframes is not None)
             or (self._testing_resource is not None and self._testing_resource._dataframes is not None)
             or (self._validation_resource is not None and self._validation_resource._dataframes is not None)
         )
```

### Comparing `vectice-23.2.6.1/src/vectice/models/git_version.py` & `vectice-23.2.7.0/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/iteration.py` & `vectice-23.2.7.0/src/vectice/models/iteration.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,66 +81,48 @@
     def __init__(
         self,
         id: str,
         index: int,
         phase: Phase,
         status: IterationStatus = IterationStatus.NotStarted,
     ):
-        """Initialize an iteration.
-
-        Vectice users shouldn't need to instantiate Iterations manually,
-        but here are the iteration parameters.
-
-        Parameters:
-            id: The iteration identifier.
-            index: The index of the iteration.
-            phase: The project to which the iteration belongs.
-            status: The status of the iteration.
-        """
         self.__dict__ = {}
         self._id = id
         self._index = index
         self._phase = phase
         self._status = status
         self._client: Client = self._phase._client
         self._model: Model | None = None
         self._current_step: Step | None = None
         self._steps = self._populate_steps()
 
     def __repr__(self):
-        steps = len(self.steps)
+        steps = self._client.list_steps(self.id).total
         return f"Iteration (index={self._index}, status={self._status}, No. of steps={steps})"
 
     def __eq__(self, other: object):
         if not isinstance(other, Iteration):
             return NotImplemented
         return self.id == other.id
 
     def _populate_steps(self):
         with suppress(NoStepsInPhaseError):
-            check = {step.slug: step for step in self.steps}
+            step_output = self._client.list_steps(self.id, True).list
+            steps = [_get_step_type(step_output=item, iteration=self) for item in step_output]
+            check = {step.slug: step for step in steps}
             return check
         return {}
 
     def __getattr__(self, item):
         if item in self.__dict__:
             return self.__dict__[item]
         if item in super().__getattribute__("_steps"):
             step_item = self._steps[item]
             step = self._client.get_step_by_name(step_item.name, self.id)
-            step_object = _get_step_type(
-                id=step.id,
-                iteration=self,
-                name=step.name,
-                index=step.index,
-                slug=step.slug,
-                description=step.description,
-                artifacts=step.artifacts,
-            )
-            return step_object
+            return _get_step_type(step_output=step, iteration=self)
         raise AttributeError(f"The attribute '{item}' does not exist.")
 
     def __setattr__(self, attr_name, attr_value):
         if hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
             if self._status in {IterationStatus.Abandoned, IterationStatus.Completed}:
                 raise VecticeException(f"The Iteration is {self.status} and is read-only!")
             self._steps[attr_name] = self._steps[attr_name]._step_factory_and_update(value=attr_value)
@@ -200,44 +182,14 @@
         """The iteration's identifier and index.
 
         Returns:
             A dictionary containing the `id` and `index` items.
         """
         return {"id": self.id, "index": self.index}
 
-    @property
-    def step_names(self) -> list[str]:
-        """The names of the steps required in this iteration.
-
-        Returns:
-            The steps names.
-        """
-        return [step.name for step in self.steps]
-
-    @property
-    def steps(self) -> list[Step]:
-        """The steps required in this iteration.
-
-        Returns:
-            The steps required in this iteration.
-        """
-        steps_output = self._client.list_steps(self.id)
-        return [
-            _get_step_type(
-                id=item.id,
-                iteration=self,
-                name=item.name,
-                index=item.index,
-                slug=item.slug,
-                description=item.description,
-                artifacts=item.artifacts,
-            )
-            for item in steps_output.list
-        ]
-
     def list_steps(self) -> None:
         """Prints a list of steps belonging to the iteration in a tabular format, limited to the first 10 steps. A link is provided to view the remaining steps.
 
         Returns:
             None
         """
         steps_output = self._client.list_steps(self.id, populate=False)
```

### Comparing `vectice-23.2.6.1/src/vectice/models/metric.py` & `vectice-23.2.7.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/model.py` & `vectice-23.2.7.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/phase.py` & `vectice-23.2.7.0/src/vectice/models/phase.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,26 +87,14 @@
         self,
         id: str,
         project: Project,
         name: str,
         index: int,
         status: PhaseStatus = PhaseStatus.NotStarted,
     ):
-        """Initialize a phase.
-
-        Vectice users shouldn't need to instantiate Phases manually,
-        but here are the phase parameters.
-
-        Parameters:
-            id: The phase identifier.
-            project: The project to which the phase belongs.
-            name: The name of the phase.
-            index: The index of the phase.
-            status: The status of the phase.
-        """
         self._id = id
         self._project = project
         self._name = name
         self._index = index
         self._status = status
         self._client: Client = self._project._client
         self._current_iteration: Iteration | None = None
@@ -202,19 +190,20 @@
 
         iteration_statuses_log = (
             " | ".join(list(map(lambda status: get_iteration_status(status), statuses)))
             if statuses is not None and len(statuses) > 0
             else None
         )
         status_log = f"with status [{iteration_statuses_log}] " if iteration_statuses_log is not None else ""
-        description = f"""There are {iteration_outputs.total} iterations {status_log}in the phase {self.name!r} and a maximum of 10 iterations are displayed in the table below:"""
+        only_mine_log = "You have" if only_mine is True else "There are"
+        description = f"""{only_mine_log} {iteration_outputs.total} iterations {status_log}in the phase {self.name!r} and a maximum of 10 iterations are displayed in the table below:"""
         link = dedent(
             f"""
         # For quick access to the list of iterations in the Vectice web app, visit:
-        # {self._client.auth._API_BASE_URL}/phase/{self.id}/iterations?w={self.workspace.id}"""
+        # {self._client.auth._API_BASE_URL}/phase/{self.id}/iterations"""
         ).lstrip()
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(link)
 
     def create_or_get_current_iteration(self) -> Iteration | None:
         """Get or create an iteration.
```

### Comparing `vectice-23.2.6.1/src/vectice/models/project.py` & `vectice-23.2.7.0/src/vectice/models/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,25 +53,14 @@
     def __init__(
         self,
         id: str,
         workspace: Workspace,
         name: str,
         description: str | None = None,
     ):
-        """Initialize a project.
-
-        Vectice users shouldn't need to instantiate Projects manually,
-        but here are the project parameters.
-
-        Parameters:
-            id: The project identifier.
-            workspace: The workspace this project belongs to.
-            name: The name of the project.
-            description: A brief description of the project.
-        """
         self._id = id
         self._workspace = workspace
         self._name = name
         self._description = description
         self._phase: Phase | None = None
         self._client = workspace._client
 
@@ -199,17 +188,7 @@
         {self._client.auth._API_BASE_URL}/browse/project/{self.id}"""
         ).lstrip()
 
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(tips)
         _temp_print(link)
-
-    @property
-    def phases(self) -> list[Phase]:
-        """The project's phases.
-
-        Returns:
-            The phases associated with this project.
-        """
-        outputs = self._client.list_phases(project=self._id)
-        return [Phase(item.id, self, item.name, item.index, item.status) for item in outputs.list]
```

### Comparing `vectice-23.2.6.1/src/vectice/models/property.py` & `vectice-23.2.7.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/representation/dataset_representation.py` & `vectice-23.2.7.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/__init__.py` & `vectice-23.2.7.0/src/vectice/models/resource/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
+from vectice.models.resource.databricks_table_resource import DatabricksTableResource
 from vectice.models.resource.file_resource import File, FileResource, FilesMetadata
 from vectice.models.resource.gcs_resource import GCSResource, NoSuchGCSResourceError
 from vectice.models.resource.s3_resource import NoSuchS3ResourceError, S3Resource
 
 __all__ = [
     "Resource",
+    "DatabricksTableResource",
     "FilesMetadata",
     "FileResource",
     "File",
     "GCSResource",
     "BigQueryResource",
     "NoSuchGCSResourceError",
     "S3Resource",
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/base.py` & `vectice-23.2.7.0/src/vectice/models/resource/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,27 +62,32 @@
     # origin must be a string because users can subclass resources
     # and set a custom origin
     _origin: str = DatasetSourceOrigin.OTHER.value
 
     _files_limit = 5000
 
     @abstractmethod
-    def __init__(self, paths: list[str] | str, dataframes: DataFrameType | list[DataFrameType] | None = None):
+    def __init__(
+        self,
+        paths: list[str] | str,
+        dataframes: DataFrameType | list[DataFrameType] | None = None,
+        capture_schema_only: bool = False,
+    ):
         """Initialize a resource."""
         self._metadata: Metadata | None = None
         self._data: dict | None = None
-
         self._paths = paths if isinstance(paths, list) else [paths]
+        self.capture_schema_only = capture_schema_only
 
         self._dataframes = dataframes if isinstance(dataframes, list) or dataframes is None else [dataframes]
         if self._dataframes is not None:
             for dataframe in self._dataframes:
                 if dataframe is not None and not isinstance(dataframe, get_args(DataFrameType)):
                     raise ValueError(
-                        f"Argument 'dataframe' of type '{type(dataframe)}' is invalid, only Pandas DataFrame is supported."
+                        f"Argument 'dataframe' of type '{type(dataframe)}' is invalid, only Pandas or Spark DataFrame are supported."
                     )
 
     @property
     def data(self) -> dict:
         """The resource's data.
 
         Returns:
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.7.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,23 +33,26 @@
     _origin = DatasetSourceOrigin.BIGQUERY.value
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: DataFrameType | list[DataFrameType] | None = None,
         bq_client: BQClient | None = None,
+        capture_schema_only: bool = False,
     ):
         """Initialize a BigQuery resource.
 
         Parameters:
             paths: The paths to retrieve the datasets or the tables.
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas)
             bq_client (Optional): The `google.cloud.bigquery.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning).
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+
         """
-        super().__init__(paths=paths, dataframes=dataframes)
+        super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
         self.bq_client = bq_client
 
     def _fetch_data(self) -> dict[str, tuple[Table | None, DataFrameType | None]]:
         tables: dict[str, tuple[Table | None, DataFrameType | None]] = {}
         df_index = 0
         for path in self._paths:
             path_tables, new_df_index = self._fetch_path_data(index=df_index, path=path)
@@ -135,20 +138,21 @@
             _logger.warning(f"Failed to list tables for dataset {path}")
             return {}, 0
 
     def _build_metadata(self) -> DBMetadata:
         tables_metadata: dict[str, tuple[Table | None, DataFrameType | None]] = self.data
         dbs: list[MetadataDB] = []
         for table_name, [table_metadata, dataframe] in tables_metadata.items():
-            columns: list[DBColumn] = []
+            columns: list[DBColumn] | None = None
             size = None
             rows_number = None
             updated_date = None
             created_date = None
             if table_metadata is not None:
+                columns = []
                 size = table_metadata.num_bytes
                 rows_number = table_metadata.num_rows
                 modified = table_metadata.modified
                 updated_date = modified.isoformat() if modified is not None else None
                 created = table_metadata.created
                 created_date = created.isoformat() if created is not None else None
                 for column in table_metadata.schema:
@@ -168,14 +172,16 @@
                     name=table_name,
                     rows_number=rows_number,
                     size=size,
                     columns=columns,
                     created_date=created_date,
                     updated_date=updated_date,
                     dataframe=dataframe,
+                    display_name=table_name.rpartition(".")[-1],
+                    capture_schema_only=self.capture_schema_only,
                 )
             )
 
         metadata_size = None
         for db in dbs:
             if db.size is not None:
                 if metadata_size is None:
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/description.py` & `vectice-23.2.7.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/file_resource.py` & `vectice-23.2.7.0/src/vectice/models/resource/file_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,31 +49,33 @@
 
     _origin = DatasetSourceOrigin.LOCAL.value
 
     def __init__(
         self,
         paths: str | list[str],
         dataframes: DataFrameType | list[DataFrameType] | None = None,
+        capture_schema_only: bool = False,
     ):
         """Initialize a file resource.
 
         Parameters:
             paths: The paths of the files to wrap.
-            dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas)
+            dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas, Spark)
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
 
         Examples:
             The following example shows how to wrap a CSV file
             called `iris.csv` in the current directory:
 
             ```python
             from vectice import FileResource
             iris_trainset = FileResource(paths="iris.csv")
             ```
         """
-        super().__init__(paths=paths, dataframes=dataframes)
+        super().__init__(paths=paths, dataframes=dataframes, capture_schema_only=capture_schema_only)
         paths_log = ", ".join(self._paths) if len(self._paths) > 1 else self._paths[0]
         _logger.info(f"File: {paths_log} wrapped successfully.")
 
     def _fetch_data(self) -> dict[str, bytes]:
         datas = {}
         metadata: FilesMetadata = self.metadata  # type:ignore[assignment]
         for file in metadata.files:
@@ -133,14 +135,16 @@
         return File(
             name=name,
             size=entry_stats.st_size,
             fingerprint=self._compute_digest_for_path(path),
             updated_date=self._convert_date_to_iso(entry_stats.st_mtime),
             uri=f"file://{os.path.abspath(path)}",
             dataframe=dataframe,
+            display_name=name.rpartition("/")[-1],
+            capture_schema_only=self.capture_schema_only,
         )
 
     @staticmethod
     def _compute_digest_for_path(path: str) -> str:
         sha = hashlib.sha256()
         bytes_array = bytearray(128 * 1024)
         mv = memoryview(bytes_array)
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.7.0/src/vectice/models/resource/gcs_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,23 +35,26 @@
     _origin = DatasetSourceOrigin.GCS.value
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: DataFrameType | list[DataFrameType] | None = None,
         gcs_client: Client | None = None,
+        capture_schema_only: bool = False,
     ):
         """Initialize a GCS resource.
 
         Parameters:
             uris: The uris of the referenced resources. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas)
             gcs_client (Optional): The `google.cloud.storage.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+
         """
-        super().__init__(paths=uris, dataframes=dataframes)
+        super().__init__(paths=uris, dataframes=dataframes, capture_schema_only=capture_schema_only)
         self.gcs_client = gcs_client
 
         for uri in self._paths:
             if not re.search(GS_URI_REG, uri):
                 raise ValueError(
                     f"Uri '{uri}' is not following the right pattern 'gs://<bucket_name>/<file_path_inside_bucket>'"
                 )
@@ -90,15 +93,23 @@
                     df_index += 1
             else:
                 dataframe = (
                     self._dataframes[df_index]
                     if self._dataframes is not None and len(self._dataframes) > df_index
                     else None
                 )
-                files.append(File(name=path, uri=uri, dataframe=dataframe))
+                files.append(
+                    File(
+                        name=path,
+                        uri=uri,
+                        dataframe=dataframe,
+                        display_name=path.rpartition("/")[-1],
+                        capture_schema_only=self.capture_schema_only,
+                    )
+                )
                 df_index += 1
         metadata = FilesMetadata(
             size=size,
             origin=self._origin,
             files=files,
         )
         return metadata
@@ -128,14 +139,16 @@
             size=blob.size,
             fingerprint=blob.md5_hash,
             created_date=blob.time_created.isoformat(),
             updated_date=blob.updated.isoformat(),
             uri=f"{uri}/{blob.name}",
             dataframe=dataframe,
             content_type=blob.content_type,
+            display_name=blob.name.rpartition("/")[-1],
+            capture_schema_only=self.capture_schema_only,
         )
 
     def _get_bucket_and_path_from_uri(self, uri: str) -> tuple[str, str]:
         match = re.search(GS_URI_REG, uri)
         if match is not None:
             _, bucket_name, path = match.groups()
             return bucket_name, path
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from vectice.models.resource.metadata.base import (
     DatasetSourceType,
     DatasetSourceUsage,
     Metadata,
 )
 from vectice.models.resource.metadata.column_metadata import DBColumn
 from vectice.models.resource.metadata.dataframe_config import DataFrameType
+from vectice.models.resource.metadata.extra_metadata import ExtraMetadata
 from vectice.models.resource.metadata.source import Source
 
 
 class DBMetadata(Metadata):
     """Class that describes metadata of dataset that comes from a database."""
 
     def __init__(
@@ -41,40 +42,52 @@
         }
 
 
 class MetadataDB(Source):
     def __init__(
         self,
         name: str,
-        columns: list[DBColumn],
+        columns: list[DBColumn] | None,
         rows_number: int | None = None,
         size: int | None = None,
         updated_date: str | None = None,
         created_date: str | None = None,
         dataframe: DataFrameType | None = None,
+        extra_metadata: list[ExtraMetadata] | None = None,
+        display_name: str | None = None,
+        capture_schema_only: bool = False,
     ):
         """Initialize a MetadataDB instance.
 
         Parameters:
             name: The name of the table.
             columns: The columns that compose the table.
             rows_number: The number of row of the table.
             size: The size of the table.
             updated_date: The date of last update of the table.
             created_date: The creation date of the table.
-            dataframe (Optional): A dataframe allowing vectice to optionally compute more metadata about this resource such as columns stats, size, rows number and column numbers. (Support Pandas)
+            dataframe (Optional): A dataframe allowing vectice to optionally compute more metadata about this resource such as columns stats, size, rows number and column numbers. (Support Pandas and Spark)
+            extra_metadata (Optional): Extra metadata to be captured.
+            display_name (Optional): Name that will be shown in the UI.
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+
         """
         super().__init__(
             name=name,
             size=size,
-            columns=list(columns),
+            columns=list(columns) if columns is not None else None,
             updated_date=updated_date,
             created_date=created_date,
             dataframe=dataframe,
+            extra_metadata=extra_metadata,
+            display_name=display_name,
+            capture_schema_only=capture_schema_only,
         )
         self.rows_number = rows_number
 
     def asdict(self) -> dict:
         return {
             "rowsNumber": self.rows_number,
+            "columnsNumber": len(self.columns) if self.columns is not None else None,
             **super().asdict(),
+            "tablename": self.display_name,
         }
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,131 @@
 from __future__ import annotations
 
+import logging
 from abc import abstractmethod
 from typing import Generic, TypeVar
 
 from pandas import Series, api
 
 from vectice.models.resource.metadata.column_metadata import (
     BooleanStat,
+    Column,
     ColumnCategoryType,
     DateStat,
     MostCommon,
     NumericalStat,
     Quantiles,
     Size,
     TextStat,
 )
-from vectice.models.resource.metadata.dataframe_config import DataFramePandasType
-from vectice.models.resource.metadata.df_wrapper_default import DataFrameDefaultWrapper
+from vectice.models.resource.metadata.dataframe_config import (
+    MAX_COLUMNS_CAPTURE_STATS,
+    DataFramePandasType,
+)
+from vectice.models.resource.metadata.df_wrapper_resource import DataFrameWrapper
+
+_logger = logging.getLogger(__name__)
 
 PT = TypeVar("PT", bound=DataFramePandasType)
 
 
-class DataFrameDefaultPandasWrapper(DataFrameDefaultWrapper[PT], Generic[PT]):
+class DataFrameDefaultPandasWrapper(DataFrameWrapper[PT], Generic[PT]):
     rows: int
     columns_numbers: int
 
     def __init__(self, dataframe: PT):
         super().__init__(dataframe)
         self.rows, self.columns_numbers = self.dataframe.shape
 
     @abstractmethod
     def __compute_date_column_statistics__(self, series: Series) -> DateStat:
         pass
 
     def get_size(self) -> Size:
         return Size(rows=int(self.rows), columns=int(self.columns_numbers))
 
-    def is_date_series(self, column: Series) -> bool:
-        if api.types.is_datetime64_any_dtype(column):
+    def is_date_series(self, column_type: str) -> bool:
+        if api.types.is_datetime64_any_dtype(column_type):
             return True
 
         try:
             # Temporary fixing issue -> TypeError: data type 'dbdate' not understood [EN-2534]
-            if column.dtypes == "dbdate":
+            if column_type == "dbdate":
                 return True
         except TypeError:
             pass
 
         return False
 
-    def __capture_column_stats__(
-        self, series: Series, minimum_rows_for_statistics: int
-    ) -> tuple[ColumnCategoryType | None, TextStat | BooleanStat | NumericalStat | DateStat | None]:
-        if api.types.is_bool_dtype(series):
-            return (
-                ColumnCategoryType.BOOLEAN,
-                self.__compute_boolean_column_statistics__(series)
-                if self.rows >= minimum_rows_for_statistics
-                else None,
-            )
-        elif api.types.is_numeric_dtype(series):
-            return (
-                ColumnCategoryType.NUMERICAL,
-                self.__compute_numeric_column_statistics__(series)
-                if self.rows >= minimum_rows_for_statistics
-                else None,
-            )
-        elif self.is_date_series(series):
-            return (
-                ColumnCategoryType.DATE,
-                self.__compute_date_column_statistics__(series) if self.rows >= minimum_rows_for_statistics else None,
+    def capture_column_schema(self) -> list[Column]:
+        column_cat: ColumnCategoryType | None = None
+        list_schema: list[Column] = []
+
+        for idx, (column, column_type) in enumerate(self.dataframe.dtypes.items()):
+            if idx >= MAX_COLUMNS_CAPTURE_STATS:
+                _logger.warning(
+                    f"Statistics are only captured for the first {MAX_COLUMNS_CAPTURE_STATS} columns of your dataframe."
+                )
+                break
+            column = str(column)
+            if api.types.is_bool_dtype(column_type):
+                column_cat = ColumnCategoryType.BOOLEAN
+                dtype = str(column_type)
+            elif api.types.is_numeric_dtype(column_type):
+                column_cat = ColumnCategoryType.NUMERICAL
+                dtype = str(column_type)
+            elif self.is_date_series(column_type):
+                column_cat = ColumnCategoryType.DATE
+                dtype = str(column_type)
+            elif api.types.is_string_dtype(column_type):
+                column_cat = ColumnCategoryType.TEXT
+                dtype = str(column_type)
+            else:
+                column_cat = None
+                dtype = str(column_type)
+
+            list_schema.append(
+                Column(
+                    name=column,
+                    data_type=dtype if dtype != "object" else "string",
+                    stats=None,
+                    category_type=column_cat,
+                )
             )
-        elif api.types.is_string_dtype(series) | api.types.is_categorical_dtype(series):
-            return (
-                ColumnCategoryType.TEXT,
-                self.__compute_string_column_statistics__(series) if self.rows >= minimum_rows_for_statistics else None,
-            )
-        return None, None
+
+        return list_schema
+
+    def capture_column_statistics(self, list_col_schema: list[Column]) -> list[Column]:
+        columns: list[Column] = []
+        stat: TextStat | BooleanStat | NumericalStat | DateStat | None = None
+        for col in list_col_schema:
+            column = self.dataframe[col.name]
+            col_type = col.category_type
+            if col_type is not None:
+                stat = self.__capture_pandas_stats__(column, col_type)
+            else:
+                stat = None
+            col.stats = stat
+
+            columns.append(col)
+
+        return columns
+
+    def __capture_pandas_stats__(
+        self, series: Series, col_type: ColumnCategoryType
+    ) -> TextStat | BooleanStat | NumericalStat | DateStat | None:
+        if col_type.value == "BOOLEAN":
+            return self.__compute_boolean_column_statistics__(series)
+        elif col_type.value == "NUMERICAL":
+            return self.__compute_numeric_column_statistics__(series)
+        elif col_type.value == "DATE":
+            return self.__compute_date_column_statistics__(series)
+        elif col_type.value == "TEXT":
+            return self.__compute_string_column_statistics__(series)
+        return None
 
     def __compute_boolean_column_statistics__(self, series: Series) -> BooleanStat:
         """Parse a dataframe series and return statistics about it.
 
         The computed statistics are:
         - The percentage of True
         - The percentage of False
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.7.0/src/vectice/models/resource/metadata/source.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,46 +10,56 @@
 from vectice.models.resource.metadata.base import MetadataSettings
 from vectice.models.resource.metadata.column_metadata import Column
 from vectice.models.resource.metadata.dataframe_config import DataFrameType
 from vectice.models.resource.metadata.df_wrapper_pandas import PandasDFWrapper
 from vectice.models.resource.metadata.df_wrapper_pyspark_pandas import PysparkPandasDFWrapper
 from vectice.models.resource.metadata.df_wrapper_resource import DataFrameWrapper
 from vectice.models.resource.metadata.df_wrapper_spark_df import SparkDFWrapper
+from vectice.models.resource.metadata.extra_metadata import ExtraMetadata
 
 _logger = logging.getLogger(__name__)
 
 
 class Source:
     def __init__(
         self,
         name: str,
         size: int | None = None,
         columns: list[Column] | None = None,
         updated_date: str | None = None,
         created_date: str | None = None,
         dataframe: DataFrameType | None = None,
+        extra_metadata: list[ExtraMetadata] | None = None,
+        display_name: str | None = None,
+        capture_schema_only: bool = False,
     ):
         """Initialize a MetadataDB instance.
 
         Parameters:
             name: The name of the source.
             size: The size of the source.
             columns: The columns that compose the source.
             updated_date: The date of last update of the source.
-            created_date: The date of last update of the source.
-            dataframe (Optional): A dataframe allowing vectice to optionally compute more metadata about this resource such as columns stats, size, rows number and column numbers. (Support Pandas)
+            created_date: The date of creation of the source.
+            dataframe (Optional): A dataframe allowing vectice to optionally compute more metadata about this resource such as columns stats, size, rows number and column numbers. (Support Pandas and Spark)
+            extra_metadata (Optional): Extra metadata to be captured.
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+
         """
         self.name = name
+        self.display_name = display_name
         self.size = size
         self.columns = columns
         self.created_date = created_date
         self.updated_date = updated_date
+        self.extra_metadata = extra_metadata
         self._dataframe = dataframe
         self._wrapper: PandasDFWrapper | PysparkPandasDFWrapper | SparkDFWrapper | None = None
         self._settings = MetadataSettings()
+        self.capture_schema_only = capture_schema_only
 
         if isinstance(self._dataframe, PandasDF):
             self._wrapper = PandasDFWrapper(self._dataframe)
         elif isinstance(self._dataframe, SparkDF):
             self._wrapper = SparkDFWrapper(self._dataframe)
         elif isinstance(self._dataframe, PysparkPandasDF):
             _logger.warning(
@@ -60,34 +70,37 @@
                 "WARNING: Custom wrappers are not supported yet, pass a Pandas or a Spark DataFrame to get statistics."
             )
 
     def set_settings(self, settings: MetadataSettings):
         self._settings = settings
 
     def asdict(self) -> dict:
-        size_info: Dict[str, int | float | None] = {"rowsNumber": None, "columnsNumber": None}
+        size_info: Dict[str, int | float | None] = {}
         skipped_statistics = False
         if self._wrapper is not None:
             df_info = self._wrapper.get_size()
             minimum_rows_for_statistics = self._settings.minimum_rows_for_statistics
             if df_info.rows < minimum_rows_for_statistics:
                 skipped_statistics = True
                 _logger.warning(
                     f"Statistics are not captured if numbers of rows are below {minimum_rows_for_statistics}, to keep the data anonymous."
                 )
             size_info = df_info.asdict()
 
         columns_list: list[Column] = self.columns if self.columns is not None else []
         columns_list = (
-            self._wrapper.capture_columns(minimum_rows_for_statistics) if self._wrapper is not None else columns_list
+            self._wrapper.capture_columns(minimum_rows_for_statistics, capture_schema_only=self.capture_schema_only)
+            if self._wrapper is not None
+            else columns_list
         )
         columns_list_dict = [col.asdict() for col in columns_list]
-
+        exm = self.extra_metadata
         return {
             **size_info,
             "size": self.size,
             "name": self.name,
             "updatedDate": self.updated_date,
             "createdDate": self.created_date,
             "columns": columns_list_dict,
             "skippedStatistics": skipped_statistics,
+            "extraMetadata": [metadata.to_dict() for metadata in exm] if exm is not None else None,  # type: ignore[attr-defined]
         }
```

### Comparing `vectice-23.2.6.1/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.7.0/src/vectice/models/resource/s3_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,27 @@
     _origin = DatasetSourceOrigin.S3.value
 
     def __init__(
         self,
         uris: str | list[str],
         dataframes: DataFrameType | list[DataFrameType] | None = None,
         s3_client: Client | None = None,
+        capture_schema_only: bool = False,
     ):
         """Initialize an S3 resource.
 
         Parameters:
             uris: The uris of the resources to get. Should follow the pattern 's3://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats. (Support Pandas)
             s3_client (Optional): The Amazon s3 client to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
+            capture_schema_only (Optional): A boolean parameter indicating whether to capture only the schema or both the schema and column statistics of the dataframes.
+
         """
-        super().__init__(paths=uris, dataframes=dataframes)
+        super().__init__(paths=uris, dataframes=dataframes, capture_schema_only=capture_schema_only)
         self.s3_client = s3_client
-
         for uri in self._paths:
             if not re.search(S3_URI_REG, uri):
                 raise ValueError(
                     f"Uri '{uri}' is not following the right pattern 's3://<bucket_name>/<file_path_inside_bucket>'"
                 )
 
     def _fetch_data(self) -> dict[str, ObjectTypeDef | None]:
@@ -93,15 +95,21 @@
                     df_index += new_df_index
         else:
             for index, uri in enumerate(self._paths):
                 dataframe = (
                     self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
                 )
                 _, path = self._get_bucket_and_path_from_uri(uri)
-                file = File(name=path, uri=uri, dataframe=dataframe)
+                file = File(
+                    name=path,
+                    uri=uri,
+                    dataframe=dataframe,
+                    display_name=path.rpartition("/")[-1],
+                    capture_schema_only=self.capture_schema_only,
+                )
                 files.append(file)
 
         metadata = FilesMetadata(files=files, origin=self._origin, size=size)
         return metadata
 
     def _build_files_list_with_size(
         self, index: int, bucket_name: str, s3_object: list[ObjectTypeDef]
@@ -126,14 +134,16 @@
                 name=name,
                 size=size,
                 fingerprint=self._get_formatted_etag_from_object(object),
                 updated_date=object["LastModified"].isoformat(),
                 created_date=None,
                 uri=uri,
                 dataframe=dataframe,
+                display_name=name.rpartition("/")[-1],
+                capture_schema_only=self.capture_schema_only,
             )
             total_size += size
             files.append(file)
             df_index += 1
         return files, total_size, df_index
 
     def _get_s3_objects_list(self, s3_client: Client) -> list[tuple[str, list[ListObjectsV2OutputTypeDef]]]:
```

### Comparing `vectice-23.2.6.1/src/vectice/models/step.py` & `vectice-23.2.7.0/src/vectice/models/step.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 class Step:
     """Model a Vectice step.
 
     Steps define the logical sequence of steps required to complete
     the phase along with their expected outcomes.
 
     Steps belong to an Iteration. The steps created under a Phase are
-    Step Definitions that are then re-used in Iterations to iteratively
-    complete the steps until a satisfactory result is obtained.
+    Step Definitions that are then re-used in Iterations.
 
     ```tree
     phase 1
         step definition 1
         step definition 2
         step definition 3
     ```
@@ -66,57 +65,41 @@
 
     If steps are added to a phase after iterations have been created
     and completed, these steps won't appear in these iterations.
 
     NOTE: **Phases and Steps Definitions are created in the Vectice App,
     Iterations are created from the Vectice Python API.**
 
-    To complete an iteration's step, you just need to assign a value to it.
-    To access the step and assign a value, you can use the "slug" of the step:
+    To access the step and assign a value, you must use the "slug" of the step:
     the slug is the name of the step, transformed to fit Python's naming rules,
     and prefixed with `step_`. For example, a step called "Clean Dataset" can
     be accessed with `my_iteration.step_clean_dataset`.
 
-    Therefore, to complete a step:
+    Therefore, to assign a value to a step:
 
     ```python
     my_clean_dataset = ...
     my_iteration.step_clean_dataset = my_clean_dataset
     ```
 
-    Depending on the step, you can assign it a [`Model`][vectice.models.model.Model],
-    a [`Dataset`][vectice.models.dataset.Dataset], code source, or attachments.
+    You can assign a [`Model`][vectice.models.model.Model],
+    [`Dataset`][vectice.models.dataset.Dataset], comments or files to any step.
     """
 
     def __init__(
         self,
         id: int,
         iteration: Iteration,
         name: str,
         index: int,
         slug: str,
         description: str | None = None,
         artifacts: list[IterationStepArtifact] | None = None,
         step_type: StepType = StepType.Step,
     ):
-        """Initialize a step.
-
-        Vectice users shouldn't need to instantiate Steps manually,
-        but here are the step parameters.
-
-        Parameters:
-            id: The step identifier.
-            iteration: The iteration to which the step belongs.
-            name: The name of the step.
-            index: The index of the step.
-            slug: The slug of the step.
-            description: The description of the step.
-            artifacts: The artifacts linked to the steps.
-            step_type: The step type.
-        """
         self._id = id
         self._iteration: Iteration = iteration
         self._name = name
         self._index = index
         self._description = description
         self._client = self._iteration._client
         self._artifacts = artifacts or []
@@ -516,16 +499,16 @@
         self, value: str | IOBase | Image, flush_step_artifacts=False
     ) -> tuple[IterationStepArtifactInput, str]:
         if flush_step_artifacts is True:
             self._flush_artifacts(step_type=StepType.StepImage)
 
         image, filename = _get_image_variables(value)
         try:
-            artifact, *_ = self._client.create_phase_attachments(
-                [("file", (filename, image))], self.phase.id, self.project.id, self.id
+            artifact, *_ = self._client.create_iteration_attachments(
+                [("file", (filename, image))], self.iteration.id, self.project.id, self.id
             )
             if isinstance(image, BufferedReader):
                 image.close()
             return (
                 IterationStepArtifactInput(id=artifact["fileId"], type=IterationStepArtifactType.EntityFile.name),
                 filename,
             )
@@ -575,37 +558,27 @@
         elif self._type is not StepType.StepNumber and isinstance(value, (int, float)):
             _logger.debug(f"Step type changed from {self._type.name} to StepNumber")
         elif self._type is not StepType.StepString and isinstance(value, str):
             _logger.debug(f"Step type changed from {self._type.name} to StepString")
 
     @property
     def name(self) -> str:
-        """The step's name.
-
-        Returns:
-            The step's name.
-        """
         return self._name
 
     @property
     def id(self) -> int:
         """The step's id.
 
         Returns:
             The step's id.
         """
         return self._id
 
     @id.setter
     def id(self, step_id: int):
-        """Set the step's id.
-
-        Parameters:
-            step_id: The id to set.
-        """
         self._id = step_id
 
     @property
     def index(self) -> int:
         """The step's index.
 
         Returns:
@@ -692,19 +665,14 @@
             return _check_code_source(self._client, self.project.id, _logger)
         else:
             _inform_if_git_repo()
             return None
 
     @property
     def model(self) -> Model | None:
-        """The step's model.
-
-        Returns:
-            The step's model.
-        """
         return self._model
 
     def _set_model_attachments(self, model: Model, model_version: ModelVersionOutput):
         logging.getLogger("vectice.models.attachment_container").propagate = True
         attachments = None
         if model.attachments:
             container = AttachmentContainer(model_version, self._client)
```

### Comparing `vectice-23.2.6.1/src/vectice/models/step_dataset.py` & `vectice-23.2.7.0/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/step_image.py` & `vectice-23.2.7.0/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/step_model.py` & `vectice-23.2.7.0/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/step_number.py` & `vectice-23.2.7.0/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/step_string.py` & `vectice-23.2.7.0/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/models/workspace.py` & `vectice-23.2.7.0/src/vectice/models/workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,24 +51,14 @@
     ```
 
     See [`Connection.connect`][vectice.Connection.connect] to learn
     how to connect to Vectice.
     """
 
     def __init__(self, id: str, name: str, description: str | None = None):
-        """Initialize a workspace.
-
-        Vectice users shouldn't need to instantiate Workspaces manually,
-        but here are the workspace parameters.
-
-        Parameters:
-            id: The workspace identifier.
-            name: The name of the workspace.
-            description: The description of the workspace.
-        """
         self._id = id
         self._name = name
         self._description = description
         self._client: Client
         self._connection: Connection
 
     def __post_init__(self, client: Client, connection: Connection):
@@ -174,24 +164,14 @@
 
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(tips)
         _temp_print(link)
 
     @property
-    def projects(self) -> list[Project]:
-        """List projects.
-
-        Returns:
-            A list of projects in this workspace.
-        """
-        response = self._client.list_projects(self.id)
-        return [Project(item.id, self, item.name, item.description) for item in response.list]
-
-    @property
     def connection(self) -> Connection:
         """The Connection to which this workspace belongs.
 
         Returns:
             The Connection to which this workspace belongs.
         """
         return self._connection
```

### Comparing `vectice-23.2.6.1/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.7.0/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/utils/common_utils.py` & `vectice-23.2.7.0/src/vectice/utils/common_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
 from contextlib import contextmanager
-from io import BufferedReader, IOBase
+from io import BufferedReader, BytesIO, IOBase
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Union
 
 from gql.transport.exceptions import TransportQueryError
-from PIL import Image
+from PIL import Image, ImageFile
 from rich.console import Console
 from rich.table import Table
 
-from vectice.api.json.iteration import IterationStatus, IterationStepArtifact
-from vectice.api.json.step import StepType
+from vectice.api.json.iteration import IterationStatus
+from vectice.api.json.step import StepOutput, StepType
 
 if TYPE_CHECKING:
     from vectice.models.iteration import Iteration
     from vectice.models.step import Step
 
 
 @contextmanager
@@ -45,37 +45,33 @@
     """
     refresh_iteration = iteration._phase.iteration(iteration.index)
     if refresh_iteration._status in {IterationStatus.Completed, IterationStatus.Abandoned}:
         raise RuntimeError(f"The Iteration is {refresh_iteration.status} and is read-only.")
 
 
 def _get_step_type(
-    id: int,
+    step_output: StepOutput,
     iteration: Iteration,
-    name: str,
-    index: int,
-    slug: str,
-    description: str | None = None,
-    artifacts: list[IterationStepArtifact] | None = None,
 ) -> Step | Any:
     # TODO: cyclic imports
     from vectice.models.step import Step
     from vectice.models.step_dataset import StepDataset
     from vectice.models.step_image import StepImage
     from vectice.models.step_model import StepModel
     from vectice.models.step_number import StepNumber
     from vectice.models.step_string import StepString
 
+    artifacts = step_output.artifacts
     step = Step(
-        id=id,
+        id=step_output.id,
         iteration=iteration,
-        name=name,
-        index=index,
-        slug=slug,
-        description=description,
+        name=step_output.name,
+        index=step_output.index,
+        slug=step_output.slug,
+        description=step_output.description,
         artifacts=artifacts,
         step_type=StepType.Step,
     )
 
     def _get_number(text: int | float | str):
         try:
             return float(text)
@@ -122,27 +118,35 @@
 def _validate_image(path: str) -> BufferedReader:
     try:
         return open(path, "rb")
     except FileNotFoundError:
         raise ValueError(f"The provided image {path!r} cannot be opened. Check its format and permissions.") from None
 
 
-def _get_image_variables(value: str | IOBase | Image.Image) -> tuple[BufferedReader | IOBase, str]:
+def _get_image_variables(value: str | IOBase | Image.Image) -> tuple[BufferedReader | IOBase | BytesIO, str]:
     if isinstance(value, IOBase):
         image = value
         filename = os.path.basename(value.name)  # type: ignore[attr-defined]
         return image, filename
     if isinstance(value, str):
         image = _validate_image(value)
         filename = os.path.basename(image.name)
         return image, filename
     if isinstance(value, Image.Image):
-        image = value.tobytes()
+        previous_load_truncated_images = ImageFile.LOAD_TRUNCATED_IMAGES
+        previous_max_image_pixels = Image.MAX_IMAGE_PIXELS
+        ImageFile.LOAD_TRUNCATED_IMAGES = True
+        Image.MAX_IMAGE_PIXELS = None
+        in_mem_file = BytesIO()
+        value.save(in_mem_file, format=value.format)
+        in_mem_file.seek(0)
         filename = os.path.basename(value.filename)
-        return image, filename
+        ImageFile.LOAD_TRUNCATED_IMAGES = previous_load_truncated_images
+        Image.MAX_IMAGE_PIXELS = previous_max_image_pixels
+        return in_mem_file, filename
 
     raise ValueError("Unsupported image provided.")
 
 
 def _temp_print(string: str | None = None, table: Table | None = None) -> None:
     console = Console(width=120)
     if string:
```

### Comparing `vectice-23.2.6.1/src/vectice/utils/configuration.py` & `vectice-23.2.7.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/utils/deprecation.py` & `vectice-23.2.7.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice/utils/last_assets.py` & `vectice-23.2.7.0/src/vectice/utils/last_assets.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,17 @@
 
 from vectice.utils.automatic_link_utils import existing_dataset_logger, existing_model_logger
 
 if TYPE_CHECKING:
     from logging import Logger
 
     from vectice.api import Client
-    from vectice.api.json.last_assets import ActivityTargetType
     from vectice.models.step import Step
 
 
-def _get_last_assets(target_types: list[ActivityTargetType], client: Client, _logger: Logger):
-    target_types_array = [target.value for target in target_types]
-    try:
-        last_asset = client.get_last_assets(target_types_array, {"index": 1, "size": 1}).list[0]
-        return last_asset
-    except IndexError as e:
-        _logger.debug(f"There were no assets with activity found. Sanity check {e}")
-        return
-
-
 def _get_last_user_and_default_workspace(client: Client) -> tuple[str, str | None]:
     asset = client.get_user_and_default_workspace()
     workspace_id = str(asset["defaultWorkspace"]["vecticeId"]) if asset["defaultWorkspace"] else None
     return asset["user"]["name"], workspace_id
 
 
 def _connection_logging(_logger: Logger, user_name: str, host: str, workspace_id: str | None):
```

### Comparing `vectice-23.2.6.1/src/vectice/utils/logging_utils.py` & `vectice-23.2.7.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.6.1/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.7.0/src/vectice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.6.1
+Version: 23.2.7.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.6.1/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.7.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -90,29 +90,30 @@
 src/vectice/models/representation/dataset_representation.py
 src/vectice/models/representation/dataset_version_representation.py
 src/vectice/models/representation/model_representation.py
 src/vectice/models/representation/model_version_representation.py
 src/vectice/models/resource/__init__.py
 src/vectice/models/resource/base.py
 src/vectice/models/resource/bigquery_resource.py
+src/vectice/models/resource/databricks_table_resource.py
 src/vectice/models/resource/description.py
 src/vectice/models/resource/file_resource.py
 src/vectice/models/resource/gcs_resource.py
 src/vectice/models/resource/s3_resource.py
 src/vectice/models/resource/metadata/__init__.py
 src/vectice/models/resource/metadata/base.py
 src/vectice/models/resource/metadata/column_metadata.py
 src/vectice/models/resource/metadata/dataframe_config.py
 src/vectice/models/resource/metadata/db_metadata.py
-src/vectice/models/resource/metadata/df_wrapper_default.py
 src/vectice/models/resource/metadata/df_wrapper_pandas.py
 src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
 src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
 src/vectice/models/resource/metadata/df_wrapper_resource.py
 src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+src/vectice/models/resource/metadata/extra_metadata.py
 src/vectice/models/resource/metadata/files_metadata.py
 src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
 src/vectice/models/resource/metadata/source.py
 src/vectice/utils/__init__.py
 src/vectice/utils/api_utils.py
 src/vectice/utils/automatic_link_utils.py
 src/vectice/utils/common_utils.py
```

### Comparing `vectice-23.2.6.1/src/vectice.egg-info/requires.txt` & `vectice-23.2.7.0/src/vectice.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+types-python-dateutil
 python-dotenv>=0.11.0
 requests>=2.5.0
 rich
 urllib3
 gql[requests]
 GitPython
 packaging
 Pillow
 pandas
 typing-extensions==4.6.2
 pyspark
+dataclasses-json==0.5.8
 
 [dev]
 black
 gitpython
 mypy
 ruff
 types-requests
```

