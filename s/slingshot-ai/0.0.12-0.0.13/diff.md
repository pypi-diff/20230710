# Comparing `tmp/slingshot_ai-0.0.12.tar.gz` & `tmp/slingshot_ai-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.12.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.13.tar", max compression
```

## Comparing `slingshot_ai-0.0.12.tar` & `slingshot_ai-0.0.13.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0      828 2023-06-28 22:24:42.219777 slingshot_ai-0.0.12/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.12/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.12/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17667 2023-06-27 15:26:50.732097 slingshot_ai-0.0.12/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     2091 2023-06-27 15:26:50.733379 slingshot_ai-0.0.12/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     5723 2023-06-26 18:48:01.304541 slingshot_ai-0.0.12/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.12/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5263 2023-06-27 15:26:50.737721 slingshot_ai-0.0.12/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.12/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.12/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.12/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.12/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.12/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.12/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1123 2023-06-23 17:35:28.186738 slingshot_ai-0.0.12/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     4519 2023-06-13 20:59:00.706466 slingshot_ai-0.0.12/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.12/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     1610 2023-06-28 22:19:13.593014 slingshot_ai-0.0.12/src/slingshot/cli/machine.py
--rw-r--r--   0        0        0     2746 2023-06-28 22:19:13.594555 slingshot_ai-0.0.12/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     2433 2023-06-27 15:26:50.741510 slingshot_ai-0.0.12/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.12/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     7855 2023-06-27 15:26:50.742904 slingshot_ai-0.0.12/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.12/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3816 2023-06-15 18:10:07.073951 slingshot_ai-0.0.12/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.12/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.12/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7029 2023-06-23 22:54:16.040274 slingshot_ai-0.0.12/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.12/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.12/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     6085 2023-06-27 15:26:50.745160 slingshot_ai-0.0.12/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.12/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.12/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.12/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.12/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.12/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.12/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.12/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.12/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.12/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26704 2023-06-28 22:19:13.595704 slingshot_ai-0.0.12/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.12/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10181 2023-06-27 15:26:50.747432 slingshot_ai-0.0.12/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    14860 2023-06-28 22:19:13.596801 slingshot_ai-0.0.12/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    19427 2023-06-28 22:19:13.597533 slingshot_ai-0.0.12/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0       83 2023-06-08 13:51:24.742135 slingshot_ai-0.0.12/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    44848 2023-06-28 22:19:13.598482 slingshot_ai-0.0.12/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.12/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     2073 2023-06-27 15:26:50.749266 slingshot_ai-0.0.12/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     1856 2023-06-14 17:13:24.234357 slingshot_ai-0.0.12/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     5334 2023-06-08 13:51:24.743481 slingshot_ai-0.0.12/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    18027 2023-06-27 15:26:50.750182 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-06-08 13:51:24.744644 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5247 2023-06-27 15:26:50.751307 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2388 2023-06-08 13:51:24.745704 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.12/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    48061 2023-06-28 22:19:13.599401 slingshot_ai-0.0.12/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    52066 2023-06-28 22:19:13.600258 slingshot_ai-0.0.12/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     5420 2023-06-08 13:51:24.747044 slingshot_ai-0.0.12/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.12/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     2876 2023-06-14 14:56:40.739250 slingshot_ai-0.0.12/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4348 2023-06-27 15:26:50.754696 slingshot_ai-0.0.12/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.12/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.12/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     6308 2023-06-28 22:19:13.601576 slingshot_ai-0.0.12/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-06-27 16:58:41.652410 slingshot_ai-0.0.12/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.12/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-28 22:19:13.602762 slingshot_ai-0.0.12/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.12/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.12/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 slingshot_ai-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0      828 2023-07-10 20:52:49.613446 slingshot_ai-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-20 09:58:42.891207 slingshot_ai-0.0.13/src/slingshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738131 slingshot_ai-0.0.13/src/slingshot/cli/__init__.py
+-rw-r--r--   0        0        0    17919 2023-07-10 15:40:42.647885 slingshot_ai-0.0.13/src/slingshot/cli/add.py
+-rw-r--r--   0        0        0     2091 2023-06-27 10:21:25.506818 slingshot_ai-0.0.13/src/slingshot/cli/apply.py
+-rw-r--r--   0        0        0     6421 2023-07-05 17:23:48.992824 slingshot_ai-0.0.13/src/slingshot/cli/apps.py
+-rw-r--r--   0        0        0     5916 2023-06-23 10:00:55.765161 slingshot_ai-0.0.13/src/slingshot/cli/artifact.py
+-rw-r--r--   0        0        0     5263 2023-06-27 10:21:25.507053 slingshot_ai-0.0.13/src/slingshot/cli/auth.py
+-rw-r--r--   0        0        0      970 2023-06-08 16:54:38.738871 slingshot_ai-0.0.13/src/slingshot/cli/code.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:12:37.848609 slingshot_ai-0.0.13/src/slingshot/cli/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.738965 slingshot_ai-0.0.13/src/slingshot/cli/config/py.typed
+-rw-r--r--   0        0        0      850 2023-06-20 09:58:42.891910 slingshot_ai-0.0.13/src/slingshot/cli/config/sentry_setup.py
+-rw-r--r--   0        0        0    13774 2023-06-27 10:21:25.507213 slingshot_ai-0.0.13/src/slingshot/cli/config/slingshot_cli.py
+-rw-r--r--   0        0        0     1234 2023-06-08 16:54:38.739227 slingshot_ai-0.0.13/src/slingshot/cli/dev.py
+-rw-r--r--   0        0        0     1123 2023-06-27 10:21:25.507291 slingshot_ai-0.0.13/src/slingshot/cli/environment.py
+-rw-r--r--   0        0        0     5323 2023-07-05 17:23:48.992981 slingshot_ai-0.0.13/src/slingshot/cli/inference.py
+-rw-r--r--   0        0        0     3059 2023-06-08 16:54:38.739428 slingshot_ai-0.0.13/src/slingshot/cli/logs.py
+-rw-r--r--   0        0        0     1951 2023-06-30 17:31:08.610192 slingshot_ai-0.0.13/src/slingshot/cli/machine.py
+-rw-r--r--   0        0        0     2759 2023-07-05 17:23:48.993098 slingshot_ai-0.0.13/src/slingshot/cli/main.py
+-rw-r--r--   0        0        0     2433 2023-07-03 15:58:05.510535 slingshot_ai-0.0.13/src/slingshot/cli/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.739665 slingshot_ai-0.0.13/src/slingshot/cli/py.typed
+-rw-r--r--   0        0        0     8920 2023-07-07 09:11:42.963260 slingshot_ai-0.0.13/src/slingshot/cli/run.py
+-rw-r--r--   0        0        0     3648 2023-06-08 16:54:38.739947 slingshot_ai-0.0.13/src/slingshot/cli/secret.py
+-rw-r--r--   0        0        0     3845 2023-07-05 17:23:48.993362 slingshot_ai-0.0.13/src/slingshot/cli/session.py
+-rw-r--r--   0        0        0       67 2023-06-08 16:54:38.740233 slingshot_ai-0.0.13/src/slingshot/cli/shared/__init__.py
+-rw-r--r--   0        0        0     6260 2023-06-23 10:00:55.765417 slingshot_ai-0.0.13/src/slingshot/cli/shared/code_sync.py
+-rw-r--r--   0        0        0     7029 2023-06-20 09:58:42.892817 slingshot_ai-0.0.13/src/slingshot/cli/shared/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740473 slingshot_ai-0.0.13/src/slingshot/cli/shared/py.typed
+-rw-r--r--   0        0        0      191 2023-06-08 16:54:38.740573 slingshot_ai-0.0.13/src/slingshot/cli/shared/settings.py
+-rw-r--r--   0        0        0     5985 2023-07-07 09:11:42.964178 slingshot_ai-0.0.13/src/slingshot/cli/shared/utils.py
+-rw-r--r--   0        0        0     1388 2023-06-08 16:54:38.740763 slingshot_ai-0.0.13/src/slingshot/cli/volume.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.740862 slingshot_ai-0.0.13/src/slingshot/code/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 16:54:38.741013 slingshot_ai-0.0.13/src/slingshot/code/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741087 slingshot_ai-0.0.13/src/slingshot/code/py.typed
+-rw-r--r--   0        0        0       56 2023-06-20 09:58:42.893069 slingshot_ai-0.0.13/src/slingshot/inference_model/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-20 09:58:42.893206 slingshot_ai-0.0.13/src/slingshot/inference_model/inference_model.py
+-rw-r--r--   0        0        0      205 2023-06-08 16:54:38.741497 slingshot_ai-0.0.13/src/slingshot/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741599 slingshot_ai-0.0.13/src/slingshot/schemas/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741656 slingshot_ai-0.0.13/src/slingshot/schemas/generated/py.typed
+-rw-r--r--   0        0        0    26670 2023-07-10 20:40:20.793233 slingshot_ai-0.0.13/src/slingshot/schemas/generated/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.741863 slingshot_ai-0.0.13/src/slingshot/schemas/py.typed
+-rw-r--r--   0        0        0    10181 2023-06-27 10:21:25.507893 slingshot_ai-0.0.13/src/slingshot/schemas/schema_extensions.py
+-rw-r--r--   0        0        0    15236 2023-07-10 20:40:20.793400 slingshot_ai-0.0.13/src/slingshot/schemas/slingshot-schema.config.json
+-rw-r--r--   0        0        0    19518 2023-07-10 20:40:20.793564 slingshot_ai-0.0.13/src/slingshot/schemas/slingshot_schema.py
+-rw-r--r--   0        0        0      125 2023-07-07 09:11:36.011571 slingshot_ai-0.0.13/src/slingshot/sdk/__init__.py
+-rw-r--r--   0        0        0    45606 2023-07-10 20:40:20.793788 slingshot_ai-0.0.13/src/slingshot/sdk/apply.py
+-rw-r--r--   0        0        0     2217 2023-06-08 16:54:38.742780 slingshot_ai-0.0.13/src/slingshot/sdk/auth.py
+-rw-r--r--   0        0        0     2073 2023-06-27 10:21:25.508229 slingshot_ai-0.0.13/src/slingshot/sdk/config.py
+-rw-r--r--   0        0        0     1856 2023-06-20 09:58:42.894424 slingshot_ai-0.0.13/src/slingshot/sdk/config_utils.py
+-rw-r--r--   0        0        0     2372 2023-07-07 09:11:36.011656 slingshot_ai-0.0.13/src/slingshot/sdk/data_collector.py
+-rw-r--r--   0        0        0     5334 2023-06-08 16:54:38.743055 slingshot_ai-0.0.13/src/slingshot/sdk/errors.py
+-rw-r--r--   0        0        0      126 2023-06-08 16:54:38.743167 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-08 16:54:38.743260 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/base_graphql.py
+-rw-r--r--   0        0        0    18027 2023-06-27 10:21:25.508389 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/fragments.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.743421 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/py.typed
+-rw-r--r--   0        0        0      138 2023-06-08 16:54:38.743578 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/__init__.py
+-rw-r--r--   0        0        0     5265 2023-06-08 16:54:38.743672 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/apps.py
+-rw-r--r--   0        0        0      986 2023-06-08 16:54:38.743759 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/deployment.py
+-rw-r--r--   0        0        0     3671 2023-06-08 16:54:38.743873 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/environment.py
+-rw-r--r--   0        0        0     5247 2023-06-27 10:21:25.508545 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744004 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/py.typed
+-rw-r--r--   0        0        0     2416 2023-07-07 09:11:42.964546 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/run.py
+-rw-r--r--   0        0        0     3578 2023-06-08 16:54:38.744228 slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/storage.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.744264 slingshot_ai-0.0.13/src/slingshot/sdk/py.typed
+-rw-r--r--   0        0        0    48216 2023-07-10 20:40:20.794010 slingshot_ai-0.0.13/src/slingshot/sdk/slingshot_api.py
+-rw-r--r--   0        0        0    52406 2023-07-10 20:40:20.794271 slingshot_ai-0.0.13/src/slingshot/sdk/slingshot_sdk.py
+-rw-r--r--   0        0        0     5420 2023-06-08 16:54:38.744840 slingshot_ai-0.0.13/src/slingshot/sdk/sync.py
+-rw-r--r--   0        0        0     2862 2023-06-08 16:54:38.744928 slingshot_ai-0.0.13/src/slingshot/sdk/upload_download_utils.py
+-rw-r--r--   0        0        0     2876 2023-06-20 09:58:42.895639 slingshot_ai-0.0.13/src/slingshot/sdk/utils.py
+-rw-r--r--   0        0        0     4361 2023-07-05 17:23:48.994648 slingshot_ai-0.0.13/src/slingshot/sdk/web_path_util.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745196 slingshot_ai-0.0.13/src/slingshot/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745256 slingshot_ai-0.0.13/src/slingshot/shared/py.typed
+-rw-r--r--   0        0        0     6308 2023-06-29 15:16:46.917807 slingshot_ai-0.0.13/src/slingshot/shared/utils.py
+-rw-r--r--   0        0        0       23 2023-06-29 15:16:46.917932 slingshot_ai-0.0.13/src/slingshot/slingshot_version.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.745526 slingshot_ai-0.0.13/src/slingshot/templates/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-29 15:13:56.504338 slingshot_ai-0.0.13/src/slingshot/templates/inference_template.py
+-rw-r--r--   0        0        0     1090 2023-06-08 16:54:38.745977 slingshot_ai-0.0.13/src/slingshot/templates/label_studio_data_export_template.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:54:38.746012 slingshot_ai-0.0.13/src/slingshot/templates/py.typed
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 slingshot_ai-0.0.13/PKG-INFO
```

### Comparing `slingshot_ai-0.0.12/pyproject.toml` & `slingshot_ai-0.0.13/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "slingshot-ai"
-version = "0.0.12"
+version = "0.0.13"
 
 [tool.poetry]
 name = "slingshot-ai"
-version = "0.0.12"
+version = "0.0.13"
 description = ""
 authors = ["Slingshot AI <service-account@slingshot.xyz>"]
 packages = [ { include = "slingshot", from = "src" } ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = ">=3.8.1"
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/add.py` & `slingshot_ai-0.0.13/src/slingshot/cli/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 from slingshot.sdk import SlingshotSDK
 from slingshot.sdk.config import client_settings
 from slingshot.sdk.utils import console, edit_slingshot_yaml
 
 from .. import schemas
 from ..sdk.errors import SlingshotException
 from ..shared.utils import load_slingshot_project_config
+from .project import list_and_set_project_id
 
 app = SlingshotCLIApp()
 yaml = r_yaml.YAML()
 
 OPTIONS = ["run", "deployment", "app", "environment", "label-studio", "session"]
 OPTION_TO_SPEC_CLASS: dict[str, Type[SlingshotAbstractAppSpec] | Type[slingshot_yaml_schemas.EnvironmentSpec]] = {
     "run": slingshot_yaml_schemas.RunSpec,
     "deployment": slingshot_yaml_schemas.DeploymentSpec,
     "app": slingshot_yaml_schemas.SlingshotCustomAppSpec,
     "environment": slingshot_yaml_schemas.EnvironmentSpec,
 }
 
 
-def pydantic_to_dict(pydantic: BaseModel) -> dict[str, Any]:
+def pydantic_to_dict(pydantic: BaseModel, *, exclude_unset: bool = True) -> dict[str, Any]:
     # Convert enums to strings
-    return json.loads(pydantic.json(exclude_none=True))
+    return json.loads(pydantic.json(exclude_none=True, exclude_defaults=True, exclude_unset=exclude_unset))
 
 
 def _display_name_to_id(input_str: str) -> str:
     """Converts a name to a valid project ID by removing special characters and replacing spaces with hyphens."""
     lower = input_str.strip().lower()
     single_space = re.sub(r"\s+", "-", lower)
     single_hyphen = re.sub(r"-+", "-", single_space)
@@ -51,15 +52,17 @@
 
 async def _create_project(sdk: SlingshotSDK) -> str:
     new_id = None
     display_name = typer.prompt("Enter a name for your project")
     project_id_default = _display_name_to_id(display_name) + "-" + uuid.uuid4().hex[:5]
     while True:
         # Replace multiple spaces with a single space and spaces with hyphens
-        new_id = new_id or typer.prompt("Enter an ID for your project (used for URLs)", default=project_id_default)
+        new_id = new_id or typer.prompt(
+            "Enter a slug for your project (unique ID used for URLs)", default=project_id_default
+        )
         try:
             project_response = await sdk.create_project(new_id, display_name=display_name)
             if project_response.error:
                 console.print(f"[red]Error creating project[/red]: {project_response.error.message}")
                 display_name = None
                 new_id = None
                 continue
@@ -68,44 +71,45 @@
             console.print(f"Created project: {new_id}")
             await sdk.use_project(project_response.data.project_id)
             return project_response.data.project_id
         except ValidationError as e:
             for error in e.errors():
                 loc = error['loc']
                 if loc[0] == 'project_id':
-                    console.print(f"[red]Project ID is invalid[/red]: {error['msg']}")
+                    console.print(f"[red]Project slug is invalid[/red]: {error['msg']}")
                     new_id = None
                 if loc[0] == 'project_display_name':
                     console.print(f"[red]Project name is invalid[/red]: {error['msg']}")
                     display_name = None
 
 
 @app.command(requires_auth=False, requires_project=False, top_level=True, name="init")
 async def init(*, sdk: SlingshotSDK) -> None:
     """Initialize a new project in the current directory"""
     if not sdk.project_id:
         if prompt_confirm("No project selected. Do you want to create a new one?", default=False):
             await _create_project(sdk)
         else:
-            "Okay, skipping. To use an existing project, run 'slingshot use'"
+            if prompt_confirm("Would you like to select an existing project?", default=False):
+                await list_and_set_project_id(sdk)
 
     # Check if the slingshot.yaml exists
     if client_settings.slingshot_config_path.exists() and client_settings.slingshot_config_path.stat().st_size > 0:
         console.print(
             "This project already has a `slingshot yaml`. You can add components to it with [bold]slingshot add[/bold]"
         )
         if not typer.confirm("Do you want to reinitialize this project from scratch?"):
             await sdk.apply_project(and_wait=True)
             return
 
     # Touch the file
     client_settings.slingshot_config_path.touch()
 
     # Insert an empty schemas.SlingshotAppSpec
-    doc = pydantic_to_dict(slingshot_yaml_schemas.ProjectManifest())
+    doc = pydantic_to_dict(slingshot_yaml_schemas.ProjectManifest(), exclude_unset=False)
     yaml.indent(mapping=2, sequence=4, offset=2)
     with client_settings.slingshot_config_path.open("w") as f:
         yaml.dump(doc, f)
 
     first = True
     while True:
         prompt = "Do you want to add another component?" if not first else "Do you want to add a component?"
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/apply.py` & `slingshot_ai-0.0.13/src/slingshot/cli/apply.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.13/src/slingshot/cli/apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 async def start_app(
     *,
     sdk: SlingshotSDK,
     name: Optional[str] = typer.Argument(None, help="App name"),
     sessions: bool = typer.Option(False, "--sessions", "-s", help="Only show sessions"),
 ) -> str:
     """Start a Slingshot app"""
-    applied = await sdk.apply_project()
+    applied, await_env_specs = await sdk.apply_project()
     source_code_id = await prompt_push_code(sdk)
 
     if not name:
         filter_fn = filter_for_sessions if sessions else filter_for_apps
         id_and_name_or_none = await prompt_for_app_spec(
             sdk, filter_fn, app_display_name='session' if sessions else 'app', raise_if_missing=False
         )
@@ -51,14 +51,27 @@
             all_app_specs = await sdk.list_apps()
             session_specs = [app_spec for app_spec in all_app_specs if app_spec.app_type == schemas.AppType.SESSION]
             if not session_specs:
                 raise SlingshotException("Session not created, exiting")
         else:
             raise typer.Exit(1)
 
+    assert sdk.project
+    app_spec = await sdk.api.get_app_spec_by_name(name, sdk.project.project_id)
+    if not app_spec:
+        raise SlingshotException(f"No run found with the name '{name}'")
+
+    await_env_spec_names = [spec.execution_environment_spec_name for spec in await_env_specs]
+    if app_spec.execution_environment_spec.execution_environment_spec_name in await_env_spec_names:
+        console.print(
+            "Waiting for environment "
+            f"'{app_spec.execution_environment_spec.execution_environment_spec_name}' to compile"
+        )
+        await sdk._wait_for_env_compile(app_spec.execution_environment_spec.execution_environment, should_print=True)
+
     app_instance = await sdk.start_app(app_name=name, source_code_id=source_code_id)
     url = await sdk.web_path_util.app(app_spec=app_instance.app_spec_id)
     console.print(f"Starting app '{name}'. See details here: {url}")
 
     console.print(f"Following logs. Ctrl-C to stop, and run 'slingshot logs {name} --follow' to follow again")
     status = await follow_app_logs_until_ready(sdk, app_instance.app_spec_id)
     if status == schemas.AppInstanceStatus.ERROR:
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/artifact.py` & `slingshot_ai-0.0.13/src/slingshot/cli/artifact.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.13/src/slingshot/cli/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/code.py` & `slingshot_ai-0.0.13/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.13/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.13/src/slingshot/cli/config/slingshot_cli.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.13/src/slingshot/cli/dev.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.13/src/slingshot/cli/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.13/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/machine.py` & `slingshot_ai-0.0.13/src/slingshot/cli/machine.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,24 +15,31 @@
     all_machine_types = await sdk.list_machine_types()
     table = Table(title=f"Machine Types")
     table.add_column("Machine Type", style="cyan")
     table.add_column("Number of GPUs", style="cyan")
     table.add_column("GPU VRAM", style="cyan")
     table.add_column("CPU", style="cyan")
     table.add_column("RAM", style="cyan")
+    table.add_column("Cost", style="cyan")
 
-    # TODO: show price per hour
     for machine_type in all_machine_types:
         name = machine_type.name
         details = machine_type.details
         for gpu_count_machine_size in details.gpu_count_machine_sizes:
+            machine_costs = gpu_count_machine_size.machine_costs
             gpu_vram = str(details.vram_gb) + "GB" if details.vram_gb else "-"
             gpu_count = str(gpu_count_machine_size.specs.gpu_limit)
             cpu = gpu_count_machine_size.specs.cpu_limit + " cores"
             ram = gpu_count_machine_size.specs.memory_limit.replace("Gi", "GB")
-            table.add_row(name, gpu_count, gpu_vram, cpu, ram)
+            cost = (
+                machine_costs.cpu_credits_per_sec
+                + machine_costs.mem_credits_per_sec
+                + machine_costs.gpu_credits_per_sec
+            ) * 60
+            cost_str = f"~{round(cost)}"
+            table.add_row(name, gpu_count, gpu_vram, cpu, ram, f"{cost_str:>6} credits/min")
     console.print(table)
     console.print(
         "💡 To specify a machine type in your [yellow]slingshot.yaml[/yellow], "
         "set the [cyan]machine_type[/cyan] field to the value of the 'Machine Type' column, "
         "and the [cyan]num_gpu[/cyan] field to the number of GPUs you want to use (defaults to 0).\n"
     )
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/main.py` & `slingshot_ai-0.0.13/src/slingshot/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 cli.add_subcommands(auth.app, name="auth", help="Authenticate with Slingshot 👋", no_args_is_help=True)
 cli.add_subcommands(artifact.app, name="artifact", help="Manage artifacts 💾", no_args_is_help=True)
 cli.add_subcommands(code.app, name="code", help="Manage and push code 👩‍💻", no_args_is_help=True)
 cli.add_subcommands(environment.app, name="environment", help="Manage environments 🌱", no_args_is_help=True)
 cli.add_subcommands(project.app, name="project", help="Manage your Slingshot project 📊", no_args_is_help=True)
 cli.add_subcommands(secret.app, name="secret", help="Create and manage secrets 🔐", no_args_is_help=True)
-cli.add_subcommands(volume.app, name="volume", help="Create and manage volumes 📁", no_args_is_help=True)
+cli.add_subcommands(volume.app, name="volume", help="Create and manage volumes 📁", no_args_is_help=True, hidden=True)
 cli.add_subcommands(run.app, name="run", help="Train ML models 🧠", no_args_is_help=True)
 cli.add_subcommands(inference.app, name="inference", help="Deploy ML models for inference 🏃‍♀️", no_args_is_help=True)
 cli.add_subcommands(session.app, name="session", help="Start an interactive session 🕹️", no_args_is_help=True)
 cli.add_subcommands(apps.app, name="app", help="Start an app 🖥️", no_args_is_help=True)
 cli.add_subcommands(dev.app, name="dev", help="Developer commands", no_args_is_help=True, hidden=True)
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/project.py` & `slingshot_ai-0.0.13/src/slingshot/cli/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/run.py` & `slingshot_ai-0.0.13/src/slingshot/cli/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,26 +42,38 @@
     config_file: Optional[str] = typer.Option(None, "--config", "-C", help="Path to config file for run."),
     debug: bool = typer.Option(False, "--debug", "-d", help="Run in debug mode.", hidden=True),
 ) -> None:
     """Start a run"""
     if debug:
         console.log("Debug mode enabled.")
 
-    await sdk.apply_project()
+    _, await_env_specs = await sdk.apply_project()
     source_code_id = await prompt_push_code(sdk)
 
     cli_args = parse_extra_args(ctx.args)
     config = await get_hyperparameter_config_from_file(Path(config_file)) if config_file else {}
     config = {**config, **cli_args}
 
     if not name:
         _, name = await prompt_for_app_spec(sdk, filter_for_runs, app_display_name="run")
 
-    new_run = await sdk.start_run(run_template_name=name, source_code_id=source_code_id, hyperparameters=config)
     assert sdk.project
+    run_spec = await sdk.api.get_app_spec_by_name(name, sdk.project.project_id)
+    if not run_spec:
+        raise SlingshotException(f"No run found with the name '{name}'")
+
+    await_env_spec_names = [spec.execution_environment_spec_name for spec in await_env_specs]
+    if run_spec.execution_environment_spec.execution_environment_spec_name in await_env_spec_names:
+        console.print(
+            "Waiting for environment "
+            f"'{run_spec.execution_environment_spec.execution_environment_spec_name}' to compile"
+        )
+        await sdk._wait_for_env_compile(run_spec.execution_environment_spec.execution_environment, should_print=True)
+
+    new_run = await sdk.start_run(run_template_name=name, source_code_id=source_code_id, hyperparameters=config)
     link = await sdk.web_path_util.run(new_run)
     console.print(f"Run created with name '{new_run.run_name}', view in browser at {link}")
     console.print(
         f"Following logs. Ctrl-C to stop, and run 'slingshot run logs {new_run.run_name} --follow' to follow again"
     )
     await follow_run_logs_until_done(sdk, run_id=new_run.run_id)
 
@@ -162,18 +174,24 @@
 
 
 @app.command("list", requires_project=True)
 async def list_runs(sdk: SlingshotSDK) -> None:
     """List all runs in the project."""
     runs = await sdk.list_runs()
     if not runs:
-        console.print(
-            "No runs found! "
-            "Edit [yellow]slingshot.yaml[/yellow] or use [yellow]slingshot add[/yellow] to add a run template."
-        )
+        run_templates = await sdk.list_run_templates()
+        if not run_templates:
+            console.print(
+                "No runs found! "
+                "Edit [yellow]slingshot.yaml[/yellow] or use [yellow]slingshot add[/yellow] to add a run template."
+            )
+            return
+        console.print("No runs found! Use [yellow]slingshot run start[/yellow] to start a run.")
+        console.print("Available run templates:")
+        console.print("\n".join(f"    - [cyan]{run_template.app_spec_name}[/cyan]" for run_template in run_templates))
         return
 
     table = Table(title="Runs")
     table.add_column("Run Name", style="cyan")
     table.add_column("Status", style="cyan")
     table.add_column("Environment", style="cyan")
     table.add_column("Source Code", style="cyan")
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.13/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/session.py` & `slingshot_ai-0.0.13/src/slingshot/cli/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 async def start(
     name: Optional[str] = typer.Argument(None, help="Session name."),
     do_sync: bool = typer.Option(False, "--sync", "-s"),
     sync_path: Optional[Path] = typer.Option(None, "--sync-path", "-p"),
     *,
     sdk: SlingshotSDK,
 ) -> None:
-    """Start a new session"""
+    """Start a session app"""
     if sync_path and not do_sync:
         do_sync = True
     if do_sync:
         await check_ssh_key_exists(sdk)
 
     start_app_name: str = await start_app.function(sdk=sdk, name=name, sessions=True)
     app_spec = await sdk.get_app(start_app_name)
@@ -66,14 +66,15 @@
     await start_code_sync_ssh(sync_path, app_spec, sdk=sdk)
 
 
 @app.command(requires_project=True)
 async def stop(
     name: Optional[str] = typer.Option(None, "--name", help="Session name to stop."), *, sdk: SlingshotSDK
 ) -> None:
+    """Stop a session app"""
     if not name:
         _, name = await prompt_for_app_spec(
             sdk, filter_for_sessions, filter_for_running_apps, app_display_name="session"
         )
     await sdk.stop_app(app_name=name)
     console.print(f"[green]Session '{name}' stopped successfully[/green].")
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.13/src/slingshot/cli/shared/code_sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.13/src/slingshot/cli/shared/prompt.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.13/src/slingshot/cli/shared/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
     for task in pending:
         task.cancel()
 
     # If task_status was cancelled or raised an exception, handle it
     if task_status.cancelled():
         raise SlingshotException("Something went wrong following logs")
-    elif exception := task_status.exception() is not None:
-        assert isinstance(exception, BaseException)
+    elif (exception := task_status.exception()) is not None:
         raise exception
 
     return task_status.result()
 
 
 async def follow_app_logs_until_ready(sdk: SlingshotSDK, app_spec_id: str) -> schemas.AppInstanceStatus:
     task_logs = asyncio.create_task(sdk.print_logs(app_spec_id=app_spec_id, follow=True))
@@ -49,16 +48,15 @@
     done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
     for task in pending:
         task.cancel()
 
     # If task_status was cancelled or raised an exception, handle it
     if task_status.cancelled():
         raise SlingshotException("Something went wrong following logs")
-    elif exception := task_status.exception() is not None:
-        assert isinstance(exception, BaseException)
+    elif (exception := task_status.exception()) is not None:
         raise exception
 
     return task_status.result()
 
 
 def datetime_to_human_readable(dt: datetime) -> str:
     """Assumes UTC datetime and converts to local time in the format of: Mar 2, 2021 1:30AM EST"""
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.13/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.13/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.13/src/slingshot/schemas/generated/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,19 +116,14 @@
     description: Optional[str] = Field(None, title='Source Code Description')
 
 
 class BodyUpdateSshPublicKey(BaseModel):
     ssh_public_key: str = Field(..., title='Ssh Public Key')
 
 
-class CancelResponseEnum(str, Enum):
-    OK = 'OK'
-    NOT_TRAINING = 'NOT_TRAINING'
-
-
 class CreateServiceAccountResponse(BaseModel):
     service_account_id: str = Field(..., title='Service Account Id')
     key: str = Field(..., title='Key')
 
 
 class DeleteResult(str, Enum):
     NOT_FOUND = 'NOT_FOUND'
@@ -178,14 +173,15 @@
     exec_env_not_found = 'exec_env_not_found'
     volume_does_not_exist = 'volume_does_not_exist'
     volume_is_locked = 'volume_is_locked'
     volume_already_exists = 'volume_already_exists'
     volume_name_invalid = 'volume_name_invalid'
     artifact_is_unzipping = 'artifact_is_unzipping'
     entity_does_not_exist = 'entity_does_not_exist'
+    multiple_gpus_not_allowed = 'multiple_gpus_not_allowed'
 
 
 class EvaluateDeploymentBody(BaseModel):
     deployment_id: str = Field(..., title='Deployment Id')
     evaluation_deployment_id: Optional[str] = Field(
         None, title='Evaluation Deployment Id'
     )
@@ -230,18 +226,14 @@
 
 class LatencyQuantiles(BaseModel):
     count: int = Field(..., title='Count')
     p50: Optional[float] = Field(None, title='P50')
     p90: Optional[float] = Field(None, title='P90')
     p95: Optional[float] = Field(None, title='P95')
     p99: Optional[float] = Field(None, title='P99')
-    p50_ewma: Optional[float] = Field(None, title='P50 Ewma')
-    p90_ewma: Optional[float] = Field(None, title='P90 Ewma')
-    p95_ewma: Optional[float] = Field(None, title='P95 Ewma')
-    p99_ewma: Optional[float] = Field(None, title='P99 Ewma')
 
 
 class LogLine(BaseModel):
     timestamp: datetime = Field(..., title='Timestamp')
     log: str = Field(..., title='Log')
 
 
@@ -338,14 +330,20 @@
 
 class OpenAIUsage(BaseModel):
     prompt_tokens: int = Field(..., title='Prompt Tokens')
     completion_tokens: Optional[int] = Field(None, title='Completion Tokens')
     total_tokens: int = Field(..., title='Total Tokens')
 
 
+class PriceData(BaseModel):
+    cpu_credits_per_sec: float = Field(..., title='Cpu Credits Per Sec')
+    mem_credits_per_sec: float = Field(..., title='Mem Credits Per Sec')
+    gpu_credits_per_sec: float = Field(..., title='Gpu Credits Per Sec')
+
+
 class ProjectId(BaseModel):
     project_id: str = Field(..., title='Project Id')
 
 
 class PromptOpenAIBody(BaseModel):
     openai_request: Union[
         OpenAIChatRequest, OpenAICompletionRequest, OpenAIEmbeddingRequest
@@ -457,25 +455,14 @@
 
 
 class UploadedSourceCodeResponse(BaseModel):
     data: Optional[UploadedSourceCode] = None
     error: Optional[SlingshotLogicalError] = None
 
 
-class UsageBinsLatencyQuantiles(BaseModel):
-    bins_start: List[datetime] = Field(..., title='Start time of each bin')
-    bins_end: List[datetime] = Field(..., title='End time of each bin')
-    data: List[LatencyQuantiles] = Field(..., title='Data values of each bin')
-
-
-class UsageBinsLatencyQuantilesResponse(BaseModel):
-    data: Optional[UsageBinsLatencyQuantiles] = None
-    error: Optional[SlingshotLogicalError] = None
-
-
 class UsageRange(str, Enum):
     HOURLY = 'HOURLY'
     DAILY = 'DAILY'
     MONTHLY = 'MONTHLY'
 
 
 class ValidationError(BaseModel):
@@ -530,25 +517,20 @@
 
 
 class BoolResponse(BaseModel):
     data: Optional[bool] = Field(None, title='Data')
     error: Optional[SlingshotLogicalError] = None
 
 
-class CancelResponseEnumResponse(BaseModel):
-    data: Optional[CancelResponseEnum] = None
-    error: Optional[SlingshotLogicalError] = None
-
-
 class CreateAppBody(BaseModel):
     name: str = Field(..., title='Name')
     command: Optional[str] = Field(None, title='Command')
     exec_env_spec_id: str = Field(..., title='Exec Env Spec Id')
     machine_size: MachineSize
-    service_account: bool = Field(..., title='Service Account')
+    attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     mounts: List[
         Union[
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
@@ -617,14 +599,15 @@
     )
 
 
 class GpuCountMachineSize(BaseModel):
     gpu_count: int = Field(..., title='Gpu Count')
     machine_size: MachineSize
     specs: MachineSpecs
+    machine_costs: PriceData
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(None, title='Detail')
 
 
 class HasAppInstanceIdResponse(BaseModel):
@@ -732,15 +715,15 @@
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     exec_env_id: str = Field(..., title='Exec Env Id')
     cmd: str = Field(..., description='Command to run', title='Cmd')
-    service_account: bool = Field(..., title='Service Account')
+    attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: Optional[str] = Field(None, title='Source Code Id')
     app_port: Optional[int] = Field(None, title='App Port')
 
 
 class StartDeploymentBody(BaseModel):
     machine_size: MachineSize
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
@@ -750,15 +733,15 @@
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     exec_env_id: str = Field(..., title='Exec Env Id')
     cmd: str = Field(..., description='Command to run', title='Cmd')
-    service_account: bool = Field(..., title='Service Account')
+    attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: str = Field(..., title='Source Code Id')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
 
 
 class StartRunBody(BaseModel):
     machine_size: MachineSize
@@ -769,30 +752,41 @@
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     exec_env_id: str = Field(..., title='Exec Env Id')
     cmd: str = Field(..., description='Command to run', title='Cmd')
-    service_account: bool = Field(..., title='Service Account')
+    attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: str = Field(..., title='Source Code Id')
 
 
 class UpdateAppBody(BaseModel):
     name: Optional[str] = Field(None, title='Name')
     command: Optional[str] = Field(None, title='Command')
     exec_env_spec_id: str = Field(..., title='Exec Env Spec Id')
     machine_size: MachineSize
-    service_account: bool = Field(..., title='Service Account')
+    attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     mounts: List[
         Union[
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
     app_port: Optional[int] = Field(None, title='App Port')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
     soft_concurrency: Optional[PositiveInt] = Field(None, title='Soft Concurrency')
+
+
+class UsageBinsLatencyQuantiles(BaseModel):
+    bins_start: List[datetime] = Field(..., title='Start time of each bin')
+    usage_range: UsageRange = Field(..., title='Range of each bin')
+    data: List[LatencyQuantiles] = Field(..., title='Data values of each bin')
+
+
+class UsageBinsLatencyQuantilesResponse(BaseModel):
+    data: Optional[UsageBinsLatencyQuantiles] = None
+    error: Optional[SlingshotLogicalError] = None
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.13/src/slingshot/schemas/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.13/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996388888888889%*

 * *Differences: {"'definitions'": "{'SlingshotCustomAppSpec': {'properties': {'attach_project_credentials': "*

 * *                  "OrderedDict([('title', 'Attach project credentials'), ('description', 'If true, "*

 * *                  'will make an API key available to instances under the `SLINGSHOT_API_KEY` '*

 * *                  'environmentvariable so that they can make requests using the Slingshot SDK for '*

 * *                  "this project'), ('default', True), ('type', 'boolean')]), delete: "*

 * *                  "['service_accoun […]*

```diff
@@ -3,14 +3,20 @@
     "$schema": "http://json-schema.org/draft/2020-12/schema",
     "definitions": {
         "DeploymentSpec": {
             "example": {
                 "environment": "deployment"
             },
             "properties": {
+                "attach_project_credentials": {
+                    "default": true,
+                    "description": "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environmentvariable so that they can make requests using the Slingshot SDK for this project",
+                    "title": "Attach project credentials",
+                    "type": "boolean"
+                },
                 "cmd": {
                     "description": "The command to run.",
                     "title": "Command",
                     "type": "string"
                 },
                 "config_variables": {
                     "description": "Optional user defined arguments to pass to the app.",
@@ -60,20 +66,14 @@
                     "type": "string"
                 },
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
                     "type": "integer"
-                },
-                "service_account": {
-                    "default": false,
-                    "description": "If true, will attach a service account to instances so that they can make requests to the Slingshot API for this project",
-                    "title": "Service account",
-                    "type": "boolean"
                 }
             },
             "required": [
                 "environment",
                 "cmd"
             ],
             "title": "Deployment",
@@ -202,14 +202,20 @@
         },
         "RunSpec": {
             "example": {
                 "cmd": "python train.py",
                 "environment": "training"
             },
             "properties": {
+                "attach_project_credentials": {
+                    "default": true,
+                    "description": "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environmentvariable so that they can make requests using the Slingshot SDK for this project",
+                    "title": "Attach project credentials",
+                    "type": "boolean"
+                },
                 "cmd": {
                     "description": "The command to run.",
                     "title": "Command",
                     "type": "string"
                 },
                 "config_variables": {
                     "description": "Optional user defined arguments to pass to the app.",
@@ -259,20 +265,14 @@
                     "type": "string"
                 },
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
                     "type": "integer"
-                },
-                "service_account": {
-                    "default": false,
-                    "description": "If true, will attach a service account to instances so that they can make requests to the Slingshot API for this project",
-                    "title": "Service account",
-                    "type": "boolean"
                 }
             },
             "required": [
                 "environment",
                 "cmd"
             ],
             "title": "Run",
@@ -280,14 +280,20 @@
         },
         "SessionAppSpec": {
             "example": {
                 "cmd": "python app.py",
                 "environment": "slackbot"
             },
             "properties": {
+                "attach_project_credentials": {
+                    "default": true,
+                    "description": "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environmentvariable so that they can make requests using the Slingshot SDK for this project",
+                    "title": "Attach project credentials",
+                    "type": "boolean"
+                },
                 "config_variables": {
                     "description": "Optional user defined arguments to pass to the app.",
                     "title": "Arguments",
                     "type": "object"
                 },
                 "environment": {
                     "description": "The name of the execution environment.",
@@ -332,20 +338,14 @@
                 },
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
                     "type": "integer"
                 },
-                "service_account": {
-                    "default": true,
-                    "description": "If true, attach a service account to the app.",
-                    "title": "Service account",
-                    "type": "boolean"
-                },
                 "using": {
                     "description": "Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
                     "enum": [
                         "session"
                     ],
                     "title": "Using",
                     "type": "string"
@@ -361,14 +361,20 @@
         },
         "SlingshotCustomAppSpec": {
             "example": {
                 "cmd": "python app.py",
                 "environment": "slackbot"
             },
             "properties": {
+                "attach_project_credentials": {
+                    "default": true,
+                    "description": "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environmentvariable so that they can make requests using the Slingshot SDK for this project",
+                    "title": "Attach project credentials",
+                    "type": "boolean"
+                },
                 "cmd": {
                     "description": "The command to run.",
                     "title": "Command",
                     "type": "string"
                 },
                 "config_variables": {
                     "description": "Optional user defined arguments to pass to the app.",
@@ -422,20 +428,14 @@
                     "title": "Number of GPUs",
                     "type": "integer"
                 },
                 "port": {
                     "description": "The port to expose.",
                     "title": "Port",
                     "type": "integer"
-                },
-                "service_account": {
-                    "default": false,
-                    "description": "If true, will attach a service account to instances so that they can make requests to the Slingshot API for this project",
-                    "title": "Service account",
-                    "type": "boolean"
                 }
             },
             "required": [
                 "name",
                 "environment",
                 "cmd"
             ],
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.13/src/slingshot/schemas/slingshot_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,19 +204,21 @@
     config_variables: dict[str, Any] = Field(
         default_factory=dict, title="Arguments", description="Optional user defined arguments to pass to the app."
     )
 
     mounts: list[MountSpecUnion] = Field(
         default_factory=list, title="Mounts", description="The mounts for the environment."
     )
-    service_account: bool = Field(
-        False,
-        title="Service account",
-        description="If true, will attach a service account to instances so that they "
-        "can make requests to the Slingshot API for this project",
+    attach_project_credentials: bool = Field(
+        True,
+        title="Attach project credentials",
+        description=(
+            "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environment"
+            "variable so that they can make requests using the Slingshot SDK for this project"
+        ),
     )
 
     class Config:
         title = "App"
         description = "An app script."
         schema_extra = {"example": {"cmd": "python app.py", "environment": "slackbot"}}
 
@@ -299,46 +301,43 @@
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
         if existing.app_type != "CUSTOM":
             diff.append(f"Changed to 'app'")
         if self.port != existing.app_port:
             diff.append(f"Port changed from '{existing.app_port}' → '{self.port}'")
 
-        if self.service_account and not existing.service_account:
-            diff.append(f"Service account added")
-        elif not self.service_account and existing.service_account:
-            diff.append(f"Service account removed")
+        if self.attach_project_credentials and not existing.service_account:
+            diff.append(f"Project credentials added")
+        elif not self.attach_project_credentials and existing.service_account:
+            diff.append(f"Project credentials account removed")
         return diff
 
 
 class SessionAppSpec(SlingshotAbstractAppSpec):
     using: Literal["session"] = Field(
         ...,
         title="Using",
         description="Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
     )
-    service_account: bool = Field(
-        True, title="Service account", description="If true, attach a service account to the app."
-    )
 
     @property
     def port(self) -> int:
         return 8080
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
         diff = super().diff(existing)
         if self.using and self.using != existing.app_type.lower():
             diff.append(f"Using changed from '{existing.app_type.lower()}' → '{self.using}'")
         if self.port != existing.app_port:
             diff.append(f"Port changed from '{existing.app_port}' → '{self.port}'")
-        if self.service_account and not existing.service_account:
-            diff.append(f"Service account added")
-        elif not self.service_account and existing.service_account:
-            diff.append(f"Service account removed")
+        if self.attach_project_credentials and not existing.service_account:
+            diff.append(f"Project credentials added")
+        elif not self.attach_project_credentials and existing.service_account:
+            diff.append(f"Project credentials removed")
         return diff
 
 
 class RunSpec(SlingshotAbstractAppSpec):
     name: str = Field("run", title="Name", description="The name of the run.")
     mounts: list[MountSpecUnion] = Field(
         default_factory=list, title="Mounts", description="The mounts for the environment."
@@ -351,18 +350,18 @@
         schema_extra = {"example": {"cmd": "python train.py", "environment": "training"}}
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
-        if self.service_account and not existing.service_account:
-            diff.append(f"Service account added")
-        elif not self.service_account and existing.service_account:
-            diff.append(f"Service account removed")
+        if self.attach_project_credentials and not existing.service_account:
+            diff.append(f"Project credentials added")
+        elif not self.attach_project_credentials and existing.service_account:
+            diff.append(f"Project credentials removed")
         return diff
 
 
 class DeploymentSpec(SlingshotAbstractAppSpec):
     name: str = Field("deployment", title="Name", description="The name of the deployment.")
     cmd: str = Field(..., title="Command", description="The command to run.")
 
@@ -375,18 +374,18 @@
         """Returns a list of differences between this and another app spec."""
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
         if existing.app_type != schemas.AppType.DEPLOYMENT:
             diff.append(f"Changed to 'deployment'")
 
-        if self.service_account and not existing.service_account:
-            diff.append(f"Service account added")
-        elif not self.service_account and existing.service_account:
-            diff.append(f"Service account removed")
+        if self.attach_project_credentials and not existing.service_account:
+            diff.append(f"Project credentials added")
+        elif not self.attach_project_credentials and existing.service_account:
+            diff.append(f"Project credentials removed")
         return diff
 
 
 class ProjectManifest(BaseModel):
     environments: dict[str, EnvironmentSpec] = Field(
         default_factory=dict, title="Environments", description="The environments to use for the job."
     )
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/apply.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/apply.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 class ApplyService:
     WAIT_FOR_ENV_POLL_INTERVAL = 2
 
     def __init__(self, sdk: "SlingshotSDK") -> None:
         if not (project := sdk.project):
-            raise SlingshotException("No project set. Please run 'slingshot init'`' or 'slingshot use'.")
+            raise SlingshotException("No project set. Please run 'slingshot init' or 'slingshot use'.")
         self._project = project
         self._sdk = sdk
 
     async def plan(self, config: schemas.ProjectManifest | None = None) -> tuple[EnvSpecPlan, AppSpecPlan]:
         if not config:
             config = load_slingshot_project_config()
         env_plan, updated_env_names = await self.plan_environments(config)
@@ -129,23 +129,23 @@
             change_msgs,
         ) = _diff_existing_env_yaml_specs(existing_env_specs, config.environments, envs_that_require_gpu)
         if change_msgs:
             console.print("\n".join(change_msgs))
         return (env_specs_to_create, env_specs_to_update, env_specs_to_delete), updated_spec_names
 
     async def apply_env_specs(
-        self, config: schemas.ProjectManifest, env_spec_plan: EnvSpecPlan
+        self, config_: schemas.ProjectManifest, env_spec_plan: EnvSpecPlan
     ) -> tuple[list[fragments.ExecutionEnvironmentSpec], dict[str, str]]:
         env_specs_to_create, env_specs_to_update, env_specs_to_delete = env_spec_plan
         existing_specs = await self._sdk.list_environments()
         env_spec_name_to_id = {
             spec.execution_environment_spec_name: spec.execution_environment_spec_id for spec in existing_specs
         }
 
-        envs_that_require_gpu = _get_envs_requiring_gpu(config)
+        envs_that_require_gpu = _get_envs_requiring_gpu(config_)
         has_env_updates = (len(env_specs_to_create) + len(env_specs_to_update) + len(env_specs_to_delete)) > 0
         if not has_env_updates:
             console.print("No changes detected to environments ✅ ")
             return [], env_spec_name_to_id
 
         environments_to_wait_for = []
         for spec, spec_name in env_specs_to_create:
@@ -232,30 +232,28 @@
 
     async def delete_env_spec(self, env_spec: fragments.ExecutionEnvironmentSpec) -> None:
         console.print(f"Deleting environment '{env_spec.execution_environment_spec_name}'...", end="")
         await self._sdk.delete_environment(environment_id=env_spec.execution_environment_spec_id)
         console.print("✅ ")
 
     async def _wait_for_environment(self, env_spec: fragments.ExecutionEnvironmentSpec, wait_for_s: int = 30) -> None:
-        env = await self._sdk.api.get_exec_env(
-            env_spec.execution_environment.execution_environment_id, project_id=self._project.project_id
-        )
+        env = await self._sdk.api.get_exec_env(env_spec.execution_environment.execution_environment_id)
         assert env, "Environment not found"
         if env.build and env.build.build_status == "SUCCESS":
             # Don't show anything if it's already ready
             return
         status = env.status
         if status == schemas.ExecEnvStatus.COMPILING.value:
             console.print(f"Waiting for environment '{env_spec.execution_environment_spec_name}'.", end="")
             try:
                 status = await self._sdk._wait_for_env_compile(env, max_wait=wait_for_s, should_print=True)
             except SlingshotException:
                 pass
 
-        url = await self._sdk.web_path_util.environment(env)
+        url = await self._sdk.web_path_util.environment(env_spec)
         if status == schemas.ExecEnvStatus.COMPILING:
             console.print(f"Environment is still compiling. You might want to check back in a few minutes: {url}")
             return
         elif status == schemas.ExecEnvStatus.FAILED:
             console.print(f"Something went wrong while preparing your environment.")
             console.print(f"\n[red]Error preparing environment:[/red]{env.error_message}: {url}")
             raise typer.Exit(1)
@@ -302,15 +300,17 @@
         app_spec_id_response = await self._sdk.create_app(
             name=app_spec.name,
             command=app_spec.cmd if hasattr(app_spec, "cmd") else None,
             app_type=app_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=app_spec.mounts,
-            service_account=app_spec.service_account if hasattr(app_spec, "service_account") else False,
+            attach_project_credentials=(
+                app_spec.attach_project_credentials if hasattr(app_spec, "attach_project_credentials") else False
+            ),
             config_variables=app_spec.config_variables,
             app_port=app_spec.port if hasattr(app_spec, "port") else None,
         )
         app_spec_id = get_data_or_raise(app_spec_id_response)
         console.print("✅")
         return app_spec_id
 
@@ -323,15 +323,15 @@
             app_spec_id=existing_app_spec_id,
             name=app_spec.name,
             command=app_spec.cmd if hasattr(app_spec, "cmd") else None,
             env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             config_variables=app_spec.config_variables,
             mounts=app_spec.mounts,
-            service_account=app_spec.service_account if hasattr(app_spec, "service_account") else False,
+            attach_project_credentials=app_spec.service_account if hasattr(app_spec, "service_account") else False,
             app_port=app_spec.port if hasattr(app_spec, "port") else None,
             batch_size=app_spec.batch_size if hasattr(app_spec, "batch_size") else None,
             batch_interval=app_spec.batch_interval if hasattr(app_spec, "batch_interval") else None,
         )
         console.print("✅ ")
 
     async def delete_app_spec(self, app_spec: fragments.AppSpec) -> None:
@@ -341,26 +341,30 @@
 
     async def run(
         self,
         project_manifest: schemas.ProjectManifest,
         env_spec_plan: EnvSpecPlan,
         app_spec_plan: AppSpecPlan,
         and_wait: bool,
-    ) -> None:
+    ) -> list[fragments.ExecutionEnvironmentSpec]:
+        """
+        Returns the list of execution environment specs that were created or updated.
+        """
         console.print(f"Applying 'slingshot.yaml' for project '{self._project.project_id}'.")
         env_specs_to_wait_for, env_spec_name_to_id = await self.apply_env_specs(
             project_manifest, env_spec_plan=env_spec_plan
         )
         await self.apply_app_specs(app_spec_plan=app_spec_plan, env_spec_name_to_id=env_spec_name_to_id)
         config.project_config.last_pushed_manifest = load_slingshot_project_config()
         if and_wait:
             if env_specs_to_wait_for:
                 console.print("[green]Waiting for environments, you can safely exit with Ctrl+C...[/green]")
             for env in env_specs_to_wait_for:
                 await self._wait_for_environment(env)
+        return env_specs_to_wait_for
 
     async def apply_to_local(self, remote_manifest: schemas.ProjectManifest | None = None, force: bool = False) -> bool:
         """
         Applies the remote manifest to the local slingshot.yaml.
 
         The last pushed manifest is used as the base of the initial diff. If there is no last-pushed manifest,
         the base is an empty manifest so that all remote changes are computed in the plan and can be applied.
@@ -407,21 +411,25 @@
             else:
                 config.project_config.last_pushed_manifest = load_slingshot_project_config()
             return True
         except Exception as e:
             # If the validation succeeded but apply fails nonetheless, we should still prompt the user
             return await prompt_override_local_remote(diff=diff, remote_manifest=remote_manifest, force=force)
 
-    async def plan_prompt_apply(self, and_wait: bool, force: bool) -> bool:
+    async def plan_prompt_apply(
+        self, *, force: bool, and_wait: bool = False
+    ) -> tuple[bool, list[fragments.ExecutionEnvironmentSpec]]:
         """
         Plan, prompt and apply changes to the remote environment.
 
-        If force is true, the changes will be applied without prompting.
+        If force is true, the changes will be applied without prompting. If it's a string, then only the matching
+        environment spec (by ID) will be awaited.
 
-        Returns True if any changes were applied, False otherwise.
+        Returns (True, x) if any changes were applied, False otherwise. X is the list of any environment specs created
+        or updated.
         """
         # We use a "last-pushed-manifest" as a merge base to determine what changes to apply.
         #  There are three cases to keep in mind:
         #  - No last-pushed-manifest and no remote manifest: it's a new project -- can safely apply the diff and push
         #  - No last-pushed-manifest and remote manifest: it's a new copy of a project -- user should pull first
         #  - last-pushed-manifest and remote manifest: it's a normal case -- perform a three-way merge
         last_pushed_manifest = config.project_config.last_pushed_manifest
@@ -431,36 +439,41 @@
             last_pushed_manifest = ProjectManifest()
         if isinstance(last_pushed_manifest, ProjectManifest):
             last_pushed_manifest = last_pushed_manifest.dict()
 
         remote_manifest = await remote_project_manifest(self._sdk)
         remote_diff = DeepDiff(last_pushed_manifest, remote_manifest.dict(), ignore_order=True)
         if is_last_pushed_manifest_empty and len(remote_diff.keys()) > 0 and not force:
-            raise SlingshotException("You have unmerged remote changes. Run 'slingshot pull' and then try apply again.")
+            raise SlingshotException(
+                "You have unmerged remote changes. Run 'slingshot pull' and then try apply again. To ignore this "
+                "error and force-apply, run 'slingshot apply -y'."
+            )
 
         current_manifest = load_slingshot_project_config()
-        if not validate_if_changes_can_be_applied(remote_diff, current_manifest=current_manifest):
+        if not (force or validate_if_changes_can_be_applied(remote_diff, current_manifest=current_manifest)):
             raise SlingshotException(
                 "Cannot apply changes because local and remote changes conflict. Run 'slingshot pull' then try again."
             )
 
         any_changes_applied = False
         if not force:
             any_changes_applied = await self.apply_to_local(remote_manifest)
 
         manifest = load_slingshot_project_config()  # Reload local, in case it was changed
         env_spec_plan, app_spec_plan = await self.plan(config=manifest)
         if any(env_spec_plan) or any(app_spec_plan):
             if force or prompt_confirm("Do you want to apply these changes?", default=True):
-                await self.run(manifest, env_spec_plan=env_spec_plan, app_spec_plan=app_spec_plan, and_wait=and_wait)
-                return True
-            return any_changes_applied
+                env_specs_to_wait_for = await self.run(
+                    manifest, env_spec_plan=env_spec_plan, app_spec_plan=app_spec_plan, and_wait=and_wait
+                )
+                return True, env_specs_to_wait_for
+            return any_changes_applied, []
         else:
             logger.debug("No changes detected ✅ ")
-            return any_changes_applied
+            return any_changes_applied, []
 
 
 async def prompt_override_local_remote(
     diff: DeepDiff, remote_manifest: schemas.ProjectManifest, *, force: bool
 ) -> bool:
     unable_to_synchronise_message = (
         f"[yellow]Conflict resolution[/yellow]: Unable to synchronise remote changes to your local slingshot.yaml."
@@ -880,15 +893,15 @@
     existing_app_specs = await sdk.list_apps()
 
     for spec in existing_app_specs:
         name = spec.app_spec_name
         environment = spec.execution_environment_spec.execution_environment_spec_name
         config_variables = json.loads(spec.config_variables) if spec.config_variables else {}
         port = spec.app_port
-        service_account = spec.service_account
+        attach_project_credentials = spec.service_account
         cmd = spec.app_spec_command
         machine_type, num_gpu = machine_size_to_machine_type_gpu_count(spec.machine_size)
 
         mounts = [
             parse_obj_as(schemas.MountSpecUnion, {"mode": i.mode, "name": i.name, "path": i.path, "tag": i.tag})
             for i in spec.mount_specs
         ]
@@ -897,54 +910,54 @@
                 schemas.SlingshotCustomAppSpec(
                     name=name,
                     environment=environment,
                     machine_type=machine_type,
                     num_gpu=num_gpu,
                     config_variables=config_variables,
                     port=port,
-                    service_account=service_account,
+                    attach_project_credentials=attach_project_credentials,
                     cmd=cmd,
                     mounts=mounts,
                 )
             )
         elif spec.app_type == schemas.AppType.SESSION:
             app_specs.append(
                 schemas.SessionAppSpec(
                     name=name,
                     environment=environment,
                     machine_type=machine_type,
                     num_gpu=num_gpu,
                     config_variables=config_variables,
-                    service_account=service_account,
+                    attach_project_credentials=attach_project_credentials,
                     using="session",
                     mounts=mounts,
                 )
             )
         elif spec.app_type == schemas.AppType.RUN:
             app_specs.append(
                 schemas.RunSpec(
                     name=name,
                     environment=environment,
                     machine_type=machine_type,
                     num_gpu=num_gpu,
                     config_variables=config_variables,
-                    service_account=service_account,
+                    attach_project_credentials=attach_project_credentials,
                     cmd=cmd,
                     mounts=mounts,
                 )
             )
         elif spec.app_type == schemas.AppType.DEPLOYMENT:
             app_specs.append(
                 schemas.DeploymentSpec(
                     name=name,
                     environment=environment,
                     machine_type=machine_type,
                     num_gpu=num_gpu,
                     config_variables=config_variables,
-                    service_account=service_account,
+                    attach_project_credentials=attach_project_credentials,
                     cmd=cmd,
                     mounts=mounts,
                 )
             )
         else:
             raise ValueError(f"Unknown app type {spec.app_type}")
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/config.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/config.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/config_utils.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/config_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/fragments.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class RunsForProjectResponse(BaseModel):
     runs: list[Run] = Field(..., alias="trainingRuns")
 
 
 class RunsForProjectQuery(BaseGraphQLQuery[RunsForProjectResponse]):
     _query = """
         query RunsForProject($projectId: String!) {
-            trainingRuns(where: {project: {projectId: {_eq: $projectId}}}) {
+            trainingRuns(where: {project: {projectId: {_eq: $projectId}}}, orderBy: {createdAt: DESC}) {
                 ...Run
             }
         } """
 
     _depends_on = [Run]
 
     def __init__(self, project_id: str):
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/slingshot_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
     """
     Misc API methods
     """
 
     async def get_backend_version(self) -> str:
         """Get the current version of the backend."""
-        return await self._client.make_request("version", method="get", response_model=str)
+        return await self._client.make_request("version", method="get", response_model=str, _setup=False)
 
     async def list_machine_types(self) -> list[schemas.MachineTypeListItem]:
         """Get a list of available machine types."""
         return await self._client.make_request(
             "machine_types", method="get", response_model=list[schemas.MachineTypeListItem]
         )
 
@@ -275,15 +275,15 @@
             json_data={"token": auth0_token, "cli": True},
         )
         auth_token = get_data_or_raise(auth_token_resp)
         logger.info("Signed in successfully")
         return auth_token
 
     async def sa_login(self, api_key: str) -> schemas.ServiceAccountToken:
-        """Sign in with a service account API key. If no API key is provided, the API key will be read from the
+        """Sign in with a Slingshot project API key. If no API key is provided, the API key will be read from the
         environment variable `SLINGSHOT_API_KEY`"""
         try:
             sa_token_resp: schemas.Response[schemas.ServiceAccountToken] = await self._client.make_request(
                 "/auth/service_account/token",
                 method="post",
                 _setup=False,
                 response_model=schemas.Response[schemas.ServiceAccountToken],
@@ -410,16 +410,17 @@
         return (data and data.app_specs[0]) or None
 
     async def get_app_spec_by_name(self, app_spec_name: str, project_id: str) -> fragments.AppSpec | None:
         """Get an app spec by name."""
         query = queries.AppSpecByNameQuery(app_spec_name=app_spec_name, project_id=project_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
-        assert len(data.app_specs) == 1
-        return (data and data.app_specs[0]) or None
+
+        # If there's no matching app spec for this name, then data.app_specs is an empty list.
+        return (data and data.app_specs and data.app_specs[0]) or None
 
     @overload
     async def get_run(self, *, run_id: str, project_id: str) -> fragments.Run | None:
         ...
 
     @overload
     async def get_run(self, *, run_name: str, project_id: str) -> fragments.Run | None:
@@ -495,17 +496,15 @@
     ) -> fragments.BlobArtifact | None:
         """Get a blob artifact by id."""
         query = queries.BlobArtifactByNameQuery(blob_artifact_name=blob_artifact_name, project_id=project_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
         return data.blob_artifacts[0] if data.blob_artifacts else None
 
-    async def get_exec_env(
-        self, exec_env_id: str, *, project_id: str | None = None
-    ) -> fragments.ExecutionEnvironment | None:
+    async def get_exec_env(self, exec_env_id: str) -> fragments.ExecutionEnvironment | None:
         """Get an execution environment by id."""
         query = queries.ExecutionEnvironmentByIdQuery(exec_env_id=exec_env_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
         if not data.execution_environments_by_pk:
             return None
 
@@ -634,32 +633,30 @@
         self,
         name: str,
         command: str | None,
         app_type: schemas.AppType,
         exec_env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
-        service_account: bool,
+        attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
-        batch_size: int | None = None,
-        batch_interval: int | None = None,
         *,
         project_id: str,
     ) -> schemas.AppSpecIdResponse:
         """Create an app spec."""
         mount_requests = [parse_obj_as(schemas.MountRequestUnion, i) for i in mounts]
         body = schemas.CreateAppBody(
             name=name,
             command=command,
             app_type=app_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mount_requests,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
         ).dict()
         body["machine_size"] = machine_size.value
 
         return await self._client.make_request(
             url=f"project/{project_id}/apps", method="post", response_model=schemas.AppSpecIdResponse, json_data=body
@@ -706,15 +703,15 @@
     async def update_app(
         self,
         app_spec_id: str,
         command: str | None,
         exec_env_spec_id: str,
         machine_size: MachineSize,
         mounts: list[schemas.MountSpecUnion],
-        service_account: bool,
+        attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
         batch_size: int | None = None,
         batch_interval: int | None = None,
         *,
         name: str | None = None,
         project_id: str,
@@ -724,15 +721,15 @@
         body = schemas.UpdateAppBody(
             command=command,
             name=name,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mount_requests,
             config_variables=config_variables,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             app_port=app_port,
             batch_size=batch_size,
             batch_interval=batch_interval,
         ).dict()
         # TODO: Find a way for pydantic not to convert machine_size to an enum
         body["machine_size"] = machine_size.value
         return await self._client.make_request(
@@ -796,15 +793,15 @@
         app_spec: fragments.AppSpec,
         machine_size: schemas.MachineSize | None = None,
         source_code_id: str | None = None,
         cmd: str | None = None,
         mount_specs: list[schemas.MountSpecUnion] | None = None,
         config_variables: JSONType | None = None,
         exec_env_id: str | None = None,
-        service_account: bool | None = None,
+        attach_project_credentials: bool | None = None,
         app_port: int | None = None,
         project_id: str,
     ) -> schemas.HasAppInstanceIdResponse:
         """Start an app."""
         # TODO: Separate the SDK logic (using existing spec) from the API logic
 
         if app_spec.app_type == schemas.AppType.SESSION:
@@ -813,25 +810,27 @@
         machine_size = machine_size or app_spec.machine_size
         command = cmd or app_spec.app_spec_command
         if mount_specs is None:
             mount_specs = [schemas.mount_spec_from_remote(mount_spec) for mount_spec in app_spec.mount_specs]
         if config_variables is None and app_spec.config_variables is not None:
             config_variables = json.loads(app_spec.config_variables)
         exec_env_id = exec_env_id or app_spec.execution_environment_spec.execution_environment.execution_environment_id
-        service_account = service_account if service_account is not None else app_spec.service_account
+        attach_project_credentials = (
+            attach_project_credentials if attach_project_credentials is not None else app_spec.service_account
+        )
         app_port = app_port or app_spec.app_port
         mount_requests = [parse_obj_as(schemas.MountRequestUnion, i) for i in mount_specs]
         body = schemas.StartAppBody(
             machine_size=machine_size,
             source_code_id=source_code_id,
             cmd=command,
             mounts=mount_requests,
             config_variables=config_variables,
             exec_env_id=exec_env_id,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             app_port=app_port,
         )
 
         return await self._client.make_request(
             url=f"project/{project_id}/apps/{app_spec.app_spec_id}/start",
             method="post",
             response_model=schemas.HasAppInstanceIdResponse,
@@ -843,38 +842,40 @@
         run_spec: fragments.AppSpec,
         source_code_id: str | None = None,
         machine_size: Optional[schemas.MachineSize] = None,
         hyperparameters: Hyperparameter | None = None,
         cmd: str | None = None,
         mount_specs: list[schemas.MountSpecUnion] | None = None,
         exec_env_id: str | None = None,
-        service_account: bool | None = None,
+        attach_project_credentials: bool | None = None,
         debug_mode: bool = False,  # TODO: maybe don't expose this to the user
         *,
         project_id: str,
     ) -> schemas.RunCreateResponse:
         """Start a run."""
         machine_size = machine_size or run_spec.machine_size
         if not hyperparameters and run_spec.config_variables:
             hyperparameters = json.loads(run_spec.config_variables)
         command = cmd or run_spec.app_spec_command
         mount_specs = mount_specs or [
             gql_mount_spec_to_read_mount_spec(mount_spec) for mount_spec in run_spec.mount_specs
         ]
         exec_env_id = exec_env_id or run_spec.execution_environment_spec.execution_environment.execution_environment_id
-        should_attach_service_account = service_account if service_account is not None else run_spec.service_account
+        should_attach_project_credentials = (
+            attach_project_credentials if attach_project_credentials is not None else run_spec.service_account
+        )
 
         body = schemas.StartAppBody(
             source_code_id=source_code_id,
             machine_size=machine_size,
             config_variables=hyperparameters,
             cmd=command,
             mounts=mount_specs,  # TODO: Fix this
             exec_env_id=exec_env_id,
-            service_account=should_attach_service_account,
+            attach_project_credentials=should_attach_project_credentials,
         )
 
         return await self._client.make_request(
             url=f"project/{project_id}/run/{run_spec.app_spec_id}/start",
             method="post",
             response_model=schemas.RunCreateResponse,
             params={"debug_mode": json.dumps(debug_mode)},
@@ -903,24 +904,24 @@
         mount_specs = mount_specs or [
             gql_mount_spec_to_read_mount_spec(mount_spec) for mount_spec in deployment_spec.mount_specs
         ]
         exec_env_id = (
             exec_env_id or deployment_spec.execution_environment_spec.execution_environment.execution_environment_id
         )
         cmd = cmd or deployment_spec.app_spec_command
-        should_attach_service_account = deployment_spec.service_account
+        should_attach_project_credentials = deployment_spec.service_account
 
         body = schemas.StartAppBody(
             source_code_id=source_code_id,
             machine_size=machine_size,
             config_variables=config_variables,
             mounts=mount_specs,  # TODO: Fix this
             exec_env_id=exec_env_id,
             cmd=cmd,
-            service_account=should_attach_service_account,
+            attach_project_credentials=should_attach_project_credentials,
         )
         return await self._client.make_request(
             url=f"project/{project_id}/deploy/{deployment_spec_id}/start",
             method="post",
             response_model=schemas.DeploymentInstanceIdResponse,
             json_data=body.dict(),
         )
@@ -939,20 +940,18 @@
 
     async def stop_app(self, app_spec_id: str, project_id: str) -> schemas.ResponseOK:
         """Stop an app."""
         return await self._client.make_request(
             url=f"project/{project_id}/apps/{app_spec_id}/stop", method="post", response_model=schemas.ResponseOK
         )
 
-    async def cancel_run(self, run_id: str, *, project_id: str) -> schemas.CancelResponseEnumResponse:
+    async def cancel_run(self, run_id: str, *, project_id: str) -> schemas.ResponseOK:
         """Cancel a run."""
         return await self._client.make_request(
-            url=f"project/{project_id}/run/{run_id}/cancel",
-            method="post",
-            response_model=schemas.CancelResponseEnumResponse,
+            url=f"project/{project_id}/run/{run_id}/cancel", method="post", response_model=schemas.ResponseOK
         )
 
     async def stop_deployment(self, deployment_spec_id: str, *, project_id: str) -> schemas.ResponseOK:
         """Stop a deployment."""
         return await self._client.make_request(
             url=f"project/{project_id}/deploy/{deployment_spec_id}/stop",
             method="post",
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/slingshot_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from ..cli.shared import format_logline
 from ..schemas import Hyperparameter, LogLine, Response, SshPort
 from ..shared.utils import get_data_or_raise
 from .apply import ApplyService
 from .auth import login_auth0
 from .config import global_config, project_config
 from .graphql import fragments
+from .graphql.fragments import ExecutionEnvironmentSpec
 from .slingshot_api import JSONType, SlingshotAPI, SlingshotClient, _zip_dir
 from .sync import sync_code, zip_code_artifact
 from .utils import console, md5_hash
 from .web_path_util import WebPathUtil
 
 logger = getLogger(__name__)
 
@@ -115,15 +116,18 @@
             time.time() - global_config.last_checked_for_updates < global_config.check_for_updates_interval
         ):
             return False
         global_config.last_checked_for_updates = time.time()
         version = await self._api.get_backend_version()
         logger.debug(f"Current version: {__version__}, backend version: {version}")
         if version != __version__:
-            console.print(f"A new version of Slingshot is available: {version}")  # TODO: Tell the user how to upgrade
+            console.print(
+                f"🎉 A new version of Slingshot is available, "
+                f"run [cyan]pip install slingshot-ai=={version}[/cyan] to install the latest version"
+            )
             return True
         return False
 
     """
     Auth SDK methods
     """
 
@@ -215,21 +219,23 @@
         """Set the current project"""
         project_fields = await self._api.get_project_by_id(project_id)
         if not project_fields:
             raise SlingshotException(f"Project '{project_id}' not found.")
         self.project = project_fields
         project_config.project_id = project_id
 
-    async def apply_project(self, and_wait: bool = False, force: bool = False) -> bool:
+    async def apply_project(
+        self, and_wait: bool = False, force: bool = False
+    ) -> tuple[bool, list[ExecutionEnvironmentSpec]]:
         """
         Apply the YAML configuration in the current directory to the current project.
 
         Returns True if any changes were applied, False otherwise.
         """
-        return await ApplyService(self).plan_prompt_apply(and_wait, force=force)
+        return await ApplyService(self).plan_prompt_apply(and_wait=and_wait, force=force)
 
     async def apply_to_local(self, force: bool = False) -> bool:
         """Apply the YAML configuration from the remote project to the current project"""
         return await ApplyService(self).apply_to_local(None, force=force)
 
     """
     Source code SDK methods
@@ -880,75 +886,75 @@
         self,
         name: str,
         command: str | None,
         app_type: schemas.AppType,
         exec_env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
-        service_account: bool,
+        attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
     ) -> schemas.AppSpecIdResponse:
         """Create a new app with the given name and configuration."""
         # TODO: this also supports creating runs/templates, but not sure if we should keep this behavior
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.create_app(
             name=name,
             command=command,
             app_type=app_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mounts,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
             project_id=project_id,
         )
 
     async def create_run_template(
         self,
         name: str,
         command: str | None,
         exec_env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
-        service_account: bool,
+        attach_project_credentials: bool,
         config_variables: JSONType | None = None,
     ) -> schemas.AppSpecIdResponse:
         """Create a new run template with the given name and configuration."""
         return await self.create_app(
             name=name,
             command=command,
             app_type=schemas.AppType.RUN,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mounts,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
         )
 
     async def create_deployment(
         self,
         name: str,
         command: str | None,
         exec_env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
-        service_account: bool,
+        attach_project_credentials: bool,
         config_variables: JSONType | None = None,
     ) -> schemas.AppSpecIdResponse:
         """Create a new deployment with the given name and configuration."""
         return await self.create_app(
             name=name,
             command=command,
             app_type=schemas.AppType.DEPLOYMENT,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
             mounts=mounts,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
         )
 
     async def create_environment(
         self,
         name: str,
         requested_python_requirements: list[schemas.RequestedRequirement] | None = None,
@@ -989,15 +995,15 @@
     async def update_app(
         self,
         app_spec_id: str,
         command: str | None,
         env_spec_id: str,
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
-        service_account: bool,
+        attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
         batch_size: int | None = None,
         batch_interval: int | None = None,
         *,
         name: str | None = None,
     ) -> schemas.Response[bool]:
@@ -1006,15 +1012,15 @@
         return await self._api.update_app(
             app_spec_id=app_spec_id,
             name=name,
             command=command,
             exec_env_spec_id=env_spec_id,
             machine_size=machine_size,
             mounts=mounts,
-            service_account=service_account,
+            attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
             batch_size=batch_size,
             batch_interval=batch_interval,
             project_id=project_id,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/upload_download_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/utils.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.13/src/slingshot/sdk/web_path_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,21 +113,21 @@
         if isinstance(deployment_spec, str):
             app_spec_id = deployment_spec
         else:
             app_spec_id = deployment_spec.app_spec_id
         return f"{self.homepage}/project/{project.project_id}/deployments/{app_spec_id}"
 
     @typing.overload
-    async def environment(self, env: schemas.HasExecutionEnvironmentId) -> str:
+    async def environment(self, env: schemas.HasExecutionEnvironmentSpecId) -> str:
         ...
 
     @typing.overload
     async def environment(self, env: str) -> str:
         ...
 
-    async def environment(self, env: schemas.HasExecutionEnvironmentId | str) -> str:
+    async def environment(self, env: schemas.HasExecutionEnvironmentSpecId | str) -> str:
         project = await self._sdk._get_current_project_or_raise()
         if isinstance(env, str):
             env_id = env
         else:
-            env_id = env.execution_environment_id
+            env_id = env.execution_environment_spec_id
         return f"{self.homepage}/project/{project.project_id}/environments/{env_id}"
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.13/src/slingshot/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.13/src/slingshot/templates/inference_template.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-from fastapi import Request
-
 from slingshot import InferenceModel, Prediction
 
 
 class MyDeployment(InferenceModel):
     async def load(self) -> None:
         """
         Slingshot will call this method to load the model.
 
         Implementation example:
             self.model = torch.load("/mnt/model/model.pt")
         """
         ...
 
-    async def predict(self, request: Request) -> Prediction | list[Prediction]:
+    async def predict(self, examples: list[bytes]) -> Prediction | list[Prediction]:
         """
         Slingshot will call this method to make predictions, passing in the raw request bytes and returns a dictionary.
         For text inputs, the bytes will be the UTF-8 encoded string.
 
         If the model is not batched, the input will be a list with a single element and the output should be a single
         dictionary as the prediction response. Otherwise, the input will be a list of examples and the output should be
         a list of dictionaries with the same length and order as the input.
```

### Comparing `slingshot_ai-0.0.12/src/slingshot/templates/label_studio_data_export_template.py` & `slingshot_ai-0.0.13/src/slingshot/templates/label_studio_data_export_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.12/PKG-INFO` & `slingshot_ai-0.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slingshot-ai
-Version: 0.0.12
+Version: 0.0.13
 Summary: 
 Author: Slingshot AI
 Author-email: service-account@slingshot.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

