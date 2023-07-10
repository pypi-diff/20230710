# Comparing `tmp/perseus_restful_api_framework-1.26.9.tar.gz` & `tmp/perseus_restful_api_framework-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perseus_restful_api_framework-1.26.9.tar", max compression
+gzip compressed data, was "perseus_restful_api_framework-1.27.0.tar", max compression
```

## Comparing `perseus_restful_api_framework-1.26.9.tar` & `perseus_restful_api_framework-1.27.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0     9313 2023-05-23 03:25:01.596563 perseus_restful_api_framework-1.26.9/CHANGELOG.md
--rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.26.9/LICENSE
--rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.26.9/README.md
--rw-r--r--   0        0        0     1140 2023-05-23 03:29:53.383254 perseus_restful_api_framework-1.26.9/pyproject.toml
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.26.9/src/majormode/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.26.9/src/majormode/perseus/__init__.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/__init__.py
--rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_address_verification_agent.py
--rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_sender_agent.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/__init__.py
--rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/tornado_handler.py
--rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_currency_dataset.sql
--rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_exception_function.sql
--rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_geometry_function.sql
--rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_label_type.sql
--rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_locale_function.sql
--rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_constant.sql
--rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_table.sql
--rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_visibility_constant.sql
--rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.26.9/src/majormode/perseus/manage.py
--rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/__init__.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/__init__.py
--rwxr-xr-x   0        0        0   155565 2023-05-23 03:24:04.575726 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/account_service.py
--rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/contact_service.py
--rwxr-xr-x   0        0        0     3551 2023-03-03 01:25:29.385031 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_constraint.sql
--rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_function.sql
--rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_index.sql
--rwxr-xr-x   0        0        0    19425 2023-05-19 10:16:08.747757 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_table.sql
--rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_constraint.sql
--rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_function.sql
--rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_index.sql
--rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_table.sql
--rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
--rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
--rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
--rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
--rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
--rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
--rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
--rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
--rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
--rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
--rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
--rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/oauth_service.py
--rwxr-xr-x   0        0        0    15044 2023-02-09 01:22:31.540928 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/session_service.py
--rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
--rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/__init__.py
--rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/account_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/__init__.py
--rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/application_service.py
--rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_constraint.sql
--rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_index.sql
--rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_table.sql
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/__init__.py
--rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/application_service_unittest.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/__init__.py
--rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/area_service.py
--rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area2sql.py
--rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
--rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
--rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_constraint.sql
--rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_dataset.sql
--rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_function.sql
--rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_index.sql
--rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_table.sql
--rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_type.sql
--rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
--rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_index.sql
--rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_table.sql
--rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
--rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
--rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_rir_table.sql
--rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
--rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_geolite_importer.py
--rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_rir_importer.py
--rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/geoip2sql.py
--rw-r--r--   0        0        0    64863 2023-01-30 02:07:47.788329 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_http_handler.py
--rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_job_service.py
--rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_rdbms_service.py
--rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_service.py
--rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/__init__.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/__init__.py
--rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/push_notification.py
--rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
--rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_index.sql
--rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_table.sql
--rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/gcm.py
--rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/notification_service.py
--rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/__init__.py
--rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_ping.rst
--rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_status.rst
--rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/index.rst
--rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service.py
--rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service_http_handler.py
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/__init__.py
--rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/agent/team_invite.py
--rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_constraint.sql
--rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_function.sql
--rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_index.sql
--rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_table.sql
--rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/migrate_20190501.sql
--rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
--rwxr-xr-x   0        0        0   121781 2023-02-09 01:23:15.435624 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/team_service.py
--rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/template/default_invite_email.txt
--rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/__init__.py
--rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/team_service_unittest.py
--rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/__init__.py
--rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/get_version.rst
--rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/index.rst
--rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/__init__.py
--rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/version_service_unittest.py
--rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service.py
--rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service_http_handler.py
--rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.26.9/setup.py
--rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.26.9/PKG-INFO
+-rw-r--r--   0        0        0    10124 2023-07-10 03:12:09.684175 perseus_restful_api_framework-1.27.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1089 2020-11-12 14:26:46.553799 perseus_restful_api_framework-1.27.0/LICENSE
+-rw-r--r--   0        0        0     4530 2022-10-02 05:19:36.696561 perseus_restful_api_framework-1.27.0/README.md
+-rw-r--r--   0        0        0     1140 2023-07-10 03:12:20.885001 perseus_restful_api_framework-1.27.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404748 perseus_restful_api_framework-1.27.0/src/majormode/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.404886 perseus_restful_api_framework-1.27.0/src/majormode/perseus/__init__.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.405009 perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/__init__.py
+-rwxr-xr-x   0        0        0    11953 2023-02-09 01:22:31.663266 perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_address_verification_agent.py
+-rw-r--r--   0        0        0     3603 2023-02-09 01:21:55.716946 perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_sender_agent.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.405462 perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/__init__.py
+-rw-r--r--   0        0        0    17545 2023-02-09 01:22:31.663215 perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/tornado_handler.py
+-rw-r--r--   0        0        0     4900 2022-11-23 10:31:53.406176 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_currency_dataset.sql
+-rwxr-xr-x   0        0        0     1892 2023-02-09 01:21:55.716943 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_exception_function.sql
+-rw-r--r--   0        0        0     1547 2022-11-23 10:31:53.406510 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_geometry_function.sql
+-rwxr-xr-x   0        0        0     1215 2022-11-23 10:31:53.406646 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_label_type.sql
+-rwxr-xr-x   0        0        0     2684 2022-11-23 10:31:53.406769 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_locale_function.sql
+-rwxr-xr-x   0        0        0     1269 2022-11-23 10:31:53.406909 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_constant.sql
+-rw-r--r--   0        0        0     6696 2022-11-23 10:31:53.407036 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_table.sql
+-rwxr-xr-x   0        0        0     1037 2022-11-23 10:31:53.407142 perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_visibility_constant.sql
+-rwxr-xr-x   0        0        0    13514 2023-02-09 01:22:42.266123 perseus_restful_api_framework-1.27.0/src/majormode/perseus/manage.py
+-rwxr-xr-x   0        0        0     1189 2022-11-23 10:31:53.407888 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/__init__.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.408088 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/__init__.py
+-rwxr-xr-x   0        0        0   158602 2023-07-05 09:05:07.016526 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/account_service.py
+-rw-r--r--   0        0        0    53061 2023-02-08 13:43:19.667427 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/contact_service.py
+-rwxr-xr-x   0        0        0     3551 2023-03-03 01:25:29.385031 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_constraint.sql
+-rwxr-xr-x   0        0        0     7947 2023-01-30 00:41:55.092554 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_function.sql
+-rw-r--r--   0        0        0     1287 2022-11-23 10:31:53.411326 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_index.sql
+-rwxr-xr-x   0        0        0    19425 2023-05-19 10:16:08.747757 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_table.sql
+-rwxr-xr-x   0        0        0     1093 2022-11-23 10:31:53.412248 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_constraint.sql
+-rwxr-xr-x   0        0        0     1101 2022-11-23 10:31:53.412521 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_function.sql
+-rwxr-xr-x   0        0        0      989 2022-11-23 10:31:53.412719 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_index.sql
+-rwxr-xr-x   0        0        0     1637 2022-11-23 10:31:53.413015 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_table.sql
+-rwxr-xr-x   0        0        0     2093 2022-11-23 10:31:53.413203 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table.718.sql
+-rwxr-xr-x   0        0        0      870 2022-11-23 10:31:53.413470 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql
+-rwxr-xr-x   0        0        0     1033 2022-11-23 10:31:53.413751 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql
+-rw-r--r--   0        0        0     1115 2022-11-23 10:31:53.414028 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql
+-rw-r--r--   0        0        0     2599 2022-11-23 10:31:53.414316 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql
+-rw-r--r--   0        0        0     1182 2022-11-23 10:31:53.414599 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql
+-rw-r--r--   0        0        0      854 2022-11-23 10:31:53.416384 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql
+-rw-r--r--   0        0        0     1877 2022-11-23 10:31:53.416723 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql
+-rw-r--r--   0        0        0     1139 2022-11-23 10:31:53.417010 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql
+-rw-r--r--   0        0        0     1179 2023-01-30 00:54:22.647572 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql
+-rw-r--r--   0        0        0     3165 2023-03-10 00:12:11.857881 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql
+-rw-r--r--   0        0        0     6259 2022-11-23 10:31:53.422782 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/oauth_service.py
+-rwxr-xr-x   0        0        0    15044 2023-06-12 12:14:13.452381 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/session_service.py
+-rw-r--r--   0        0        0      371 2022-11-23 10:31:53.423592 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/template/default_verify_email_eng-US.txt
+-rw-r--r--   0        0        0      496 2022-11-23 10:31:53.423820 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/template/default_verify_email_fra-FR.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424102 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/__init__.py
+-rwxr-xr-x   0        0        0     7955 2022-11-23 10:31:53.424296 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/account_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.424502 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/__init__.py
+-rwxr-xr-x   0        0        0    36170 2023-02-09 01:22:42.266180 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/application_service.py
+-rwxr-xr-x   0        0        0     1581 2022-11-23 10:31:53.426329 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_constraint.sql
+-rwxr-xr-x   0        0        0     1226 2022-11-23 10:31:53.426580 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_index.sql
+-rwxr-xr-x   0        0        0     5129 2022-11-23 10:31:53.426913 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_table.sql
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.428345 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/__init__.py
+-rwxr-xr-x   0        0        0     5285 2023-01-30 01:58:24.717658 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/application_service_unittest.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.429024 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/__init__.py
+-rw-r--r--   0        0        0    38030 2023-02-09 01:22:31.541021 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/area_service.py
+-rwxr-xr-x   0        0        0     5918 2022-11-23 10:31:53.430300 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area2sql.py
+-rw-r--r--   0        0        0     5064 2022-11-23 10:31:53.430550 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area_extractor.py
+-rw-r--r--   0        0        0  5506086 2022-11-23 10:31:53.441911 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip
+-rwxr-xr-x   0        0        0     1534 2022-11-23 10:31:53.442964 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_constraint.sql
+-rw-r--r--   0        0        0     3013 2022-11-23 10:31:53.443144 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_dataset.sql
+-rw-r--r--   0        0        0    27948 2022-11-23 10:31:53.443409 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_function.sql
+-rw-r--r--   0        0        0     1324 2022-11-23 10:31:53.443571 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_index.sql
+-rwxr-xr-x   0        0        0     5732 2022-11-23 10:31:53.443741 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_table.sql
+-rwxr-xr-x   0        0        0     2447 2022-11-23 10:31:53.443964 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_type.sql
+-rwxr-xr-x   0        0        0     1097 2022-11-23 10:31:53.444132 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_constraint.sql
+-rw-r--r--   0        0        0      908 2022-11-23 10:31:53.444276 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_index.sql
+-rw-r--r--   0        0        0     7276 2022-11-23 10:31:53.444639 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_table.sql
+-rwxr-xr-x   0        0        0      923 2022-11-23 10:31:53.444789 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql
+-rwxr-xr-x   0        0        0     1631 2022-11-23 10:31:53.444977 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql
+-rw-r--r--   0        0        0     5679 2022-11-23 10:31:53.445111 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_rir_table.sql
+-rw-r--r--   0        0        0     1597 2022-11-23 10:31:53.445206 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/migrate_area_dataset.sql
+-rw-r--r--   0        0        0     1512 2022-11-23 10:31:53.445958 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_geolite_importer.py
+-rw-r--r--   0        0        0     6460 2022-11-23 10:31:53.446070 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_rir_importer.py
+-rwxr-xr-x   0        0        0    17479 2022-11-23 10:31:53.446283 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/geoip2sql.py
+-rw-r--r--   0        0        0    64867 2023-07-10 03:10:00.295237 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_http_handler.py
+-rw-r--r--   0        0        0     1331 2022-11-23 10:31:53.448135 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_job_service.py
+-rwxr-xr-x   0        0        0     3067 2023-02-09 01:22:42.266212 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_rdbms_service.py
+-rwxr-xr-x   0        0        0     4565 2023-02-09 01:21:55.697787 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_service.py
+-rwxr-xr-x   0        0        0      778 2022-11-23 10:31:53.448685 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/__init__.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.448883 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/__init__.py
+-rwxr-xr-x   0        0        0    13128 2022-11-23 10:31:53.449162 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/push_notification.py
+-rw-r--r--   0        0        0      899 2022-11-23 10:31:53.449426 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_constraint.sql
+-rw-r--r--   0        0        0     1167 2022-11-23 10:31:53.449636 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_index.sql
+-rw-r--r--   0        0        0    10511 2022-11-23 10:31:53.449859 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_table.sql
+-rw-r--r--   0        0        0     2254 2022-11-23 10:31:53.450914 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/gcm.py
+-rw-r--r--   0        0        0    65115 2023-02-09 01:22:31.540956 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/notification_service.py
+-rw-r--r--   0        0        0     1113 2022-11-23 10:31:53.451539 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/__init__.py
+-rw-r--r--   0        0        0      802 2022-11-23 10:31:53.451813 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_ping.rst
+-rw-r--r--   0        0        0      927 2023-02-08 01:28:29.061642 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_status.rst
+-rw-r--r--   0        0        0      609 2023-02-08 01:24:00.319004 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/index.rst
+-rw-r--r--   0        0        0     7536 2022-11-23 10:31:53.452507 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service.py
+-rw-r--r--   0        0        0     2427 2022-11-23 10:31:53.452658 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service_http_handler.py
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.453023 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/__init__.py
+-rw-r--r--   0        0        0     2469 2022-11-23 10:31:53.453234 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/agent/team_invite.py
+-rw-r--r--   0        0        0     2647 2022-11-23 10:31:53.453512 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_constraint.sql
+-rw-r--r--   0        0        0     3769 2022-11-23 10:31:53.453654 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_function.sql
+-rw-r--r--   0        0        0      968 2023-05-19 09:03:02.094015 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_index.sql
+-rw-r--r--   0        0        0     9034 2023-05-19 09:32:28.819485 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_table.sql
+-rw-r--r--   0        0        0      253 2022-11-23 10:31:53.454170 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/migrate_20190501.sql
+-rw-r--r--   0        0        0     2513 2022-11-23 10:31:53.454566 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql
+-rwxr-xr-x   0        0        0   124076 2023-05-25 02:34:43.732136 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/team_service.py
+-rw-r--r--   0        0        0      623 2022-11-23 10:31:53.458700 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/template/default_invite_email.txt
+-rwxr-xr-x   0        0        0     1113 2022-11-23 10:31:53.458921 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/__init__.py
+-rwxr-xr-x   0        0        0     6049 2022-11-23 10:31:53.459109 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/team_service_unittest.py
+-rw-r--r--   0        0        0      830 2022-11-23 10:31:53.459329 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/__init__.py
+-rw-r--r--   0        0        0     2734 2023-02-08 01:36:23.016572 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/get_version.rst
+-rw-r--r--   0        0        0     1913 2023-02-08 01:37:27.596508 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/index.rst
+-rwxr-xr-x   0        0        0      836 2022-11-23 10:31:53.461396 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/__init__.py
+-rwxr-xr-x   0        0        0     4574 2022-11-23 10:31:53.461950 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/version_service_unittest.py
+-rwxr-xr-x   0        0        0     2448 2023-01-17 06:08:31.898328 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service.py
+-rw-r--r--   0        0        0     1720 2023-01-17 03:47:01.966678 perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service_http_handler.py
+-rw-r--r--   0        0        0     6855 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.0/setup.py
+-rw-r--r--   0        0        0     5871 1970-01-01 00:00:00.000000 perseus_restful_api_framework-1.27.0/PKG-INFO
```

### Comparing `perseus_restful_api_framework-1.26.9/CHANGELOG.md` & `perseus_restful_api_framework-1.27.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,45 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.27.0] - 2023-07-10
+# Changed
+- HTTP request handlers return a dictionary object itself instead of embedding it in a `{ "data": dict }`
+
+## [1.26.17] - 2023-06-10
+# Fixed
+- Return the generated password when creating a new account without specifying a password
+
+## [1.26.14] - 2023-06-10
+# Fixed
+- Fix the function that generates a password to comply with password complexity requirements
+
+## [1.26.13] - 2023-06-06
+# Fixed
+- Fix the Account Service's method `get_accounts`
+
+## [1.26.12] - 2023-05-29
+# Added
+- The Account Service's method `set_object_status` to change the status of an account
+
+## [1.26.11] - 2023-05-25
+# Added
+- The Team Service's method `set_member_role` to change the role of a team member
+
+## [1.26.10] - 2023-05-23
+# Changed
+- Allow to create an account without defining a password
 
 ## [1.26.9] - 2023-05-23
 # Changed
-- The method Account Service's `sign_up` allows passing a single contact information
+- The Account Service's method `sign_up` allows passing a single contact information
 
 ## [1.26.8] - 2023-03-08
 # Changed
 - Remove the column `picture_time` from the table `account`
 
 ## [1.26.7] - 2023-02-15
 # Fixed
```

### Comparing `perseus_restful_api_framework-1.26.9/LICENSE` & `perseus_restful_api_framework-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/README.md` & `perseus_restful_api_framework-1.27.0/README.md`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/pyproject.toml` & `perseus_restful_api_framework-1.27.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["perseus", "resful", "api", "server", "framework"]
 license = "Proprietary"
 name = "perseus-restful-api-framework"
 packages = [{ include = "majormode", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/majormode/perseus-restful-api-server-framework"
-version = "1.26.9"
+version = "1.27.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.4"
 tornado = "^6.2"
 perseus-core-library = "^1.18.24"
 pillow = "^9.4.0"
```

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_address_verification_agent.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_address_verification_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/agent/email_sender_agent.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/agent/email_sender_agent.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/bootstrap/tornado_handler.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/bootstrap/tornado_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_currency_dataset.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_currency_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_exception_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_exception_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_geometry_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_geometry_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_label_type.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_label_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_locale_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_locale_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_constant.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_object_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_object_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/db/create_visibility_constant.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/db/create_visibility_constant.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/manage.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/manage.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/account_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/account_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
     # groups user avatars all together.
     CDN_BUCKET_NAME_PICTURE = 'avatar'
 
     # Default image file format to store the picture of an account with
     # (cf. https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html).
     DEFAULT_IMAGE_FILE_FORMAT = 'JPEG'
 
-    # Default quality to store the image with, on a scale from `1` (worst)
-    # to `95` (best).  Values above `95` should be avoided; `100` disables
+    # Default quality to store the image, on a scale from `1` (worst) to
+    # `95` (best).  Values above `95` should be avoided; `100` disables
     # portions of the JPEG compression algorithm, and results in large files
     # with hardly any gain in image quality.
     DEFAULT_IMAGE_QUALITY = 75
 
     # Duration in seconds a password reset request lives before it expires.
     DEFAULT_PASSWORD_RESET_REQUEST_LIFESPAN = 60 * 5  # 5 minutes
 
@@ -411,35 +411,61 @@
         """
         return ''.join([
             str(random.randint(0, 9))
             for _ in range(digit_count)
         ])
 
     @classmethod
-    def __generate_password(cls, length=8, are_symbols_allowed=False):
+    def __generate_password(
+            cls,
+            length: int = 8,
+            are_symbols_allowed: bool = True):
         """
         Generate a password
 
 
         :param length: Number of characters that composes the password to be
             generated.
 
         :param are_symbols_allowed: Indicate whether the password can
             contain punctuation characters.
 
 
         :return: A string representing a password randomly generated.
         """
-        alphabet = string.ascii_letters + string.digits
+        # Define the set of characters that could be used to build a password.
+        authorized_characters = string.ascii_letters + string.digits
+        if are_symbols_allowed:
+            authorized_characters += string.punctuation
+
+        # Initialize the password as an empty string.
+        password = ''
+
+        # Generate the required components.
+        password += random.choice(string.ascii_lowercase)  # Add a lowercase letter
+        password += random.choice(string.ascii_uppercase)  # Add an uppercase letter
+        password += random.choice(string.digits)  # Add a digit
         if are_symbols_allowed:
-            alphabet += cls.PASSWORD_ALLOWED_SPECIAL_CHARACTERS_LIST
+            password += random.choice(string.punctuation)  # Add a special character
+
+        # Generate the remaining characters.
+        remaining_length = length - 3 - are_symbols_allowed  # Subtract the length of the required components
+        password += ''.join(
+            random.choice(authorized_characters)
+            for _ in range(remaining_length)
+        )
+
+        # Shuffle the password to ensure randomness.
+        password_list = list(password)
+        random.shuffle(password_list)
+        password = ''.join(password_list)
 
-        password = ''.join(secrets.choice(alphabet) for _ in range(length))
         return password
 
+
     def __get_password_reset_request(
             self,
             app_id,
             check_app=False,
             connection=None,
             contact=None,
             nonce=None,
@@ -673,15 +699,15 @@
 
     def __set_picture_status(
             self,
             picture_id,
             status,
             connection=None):
         """
-        Set the current status of a picture
+        Set the current status of a picture.
 
 
         :param picture_id: The identification of a picture.
 
         :param status: An item of the enumeration `ObjectStatus`
             representing the new status of the picture.
 
@@ -700,15 +726,15 @@
 
             - `update_time` (required): The time of the most recent modification of
               the picture's status.
 
 
         :raise DeletedObjectException: If the picture has been deleted.
 
-        :raise UndefinedObjectException: If the picture doesn't not exist.
+        :raise UndefinedObjectException: If the picture does not exist.
         """
         with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
             picture = self.get_picture(picture_id, check_status=False, connection=connection)
             if picture.object_status == status:
                 return
             elif picture.object_status == ObjectStatus.deleted:
                 raise self.DeletedObjectException(f"The picture {picture_id} has been deleted")
@@ -990,15 +1016,16 @@
 
 
         :raise InvalidArgumentException: If the new password doesn't meet
             the complexity requirements {@link
             AccountService.REGEX_PASSWORD_COMPLEXITY_REQUIREMENTS}.
         """
         if not cls.REGEX_PASSWORD_COMPLEXITY_REQUIREMENTS.match(password):
-            raise cls.InvalidArgumentException("The password doesn't meet complexity requirements")
+            logging.error(f"The password {password} doesn't meet the complexity requirements")
+            raise cls.InvalidArgumentException("The password doesn't meet the complexity requirements")
 
     def assert_password_reset_request_nonce_valid(
             self,
             contact,
             nonce=None,
             connection=None,
             request_id=None):
@@ -1311,15 +1338,15 @@
 
             - `account_id` (required): The identification of the user account that
               the picture is associated with.
 
             - `image_height` (required): Number of pixel rows of the user's
               original photo image.
 
-            - `image_width`  (required): Number of pixel columns of the user's
+            - `image_width` (required): Number of pixel columns of the user's
               original photo image.
 
             - `object_status`: (required): An item of the enumeration `ObjectStatus`
               that indicates the current status of this picture.
 
             - `picture_id`: (required): The identification of the picture.
 
@@ -1714,24 +1741,24 @@
                doesn't refer to a user account registered against the
                platform.
         """
         account_ids = set(account_ids)
         if not account_ids:
             return []
 
+        email_addresses = [
+            email_address
+            for email_address in account_ids
+            if isinstance(email_address, str)
+               and REGEX_PATTERN_EMAIL_ADDRESS.match(email_address.strip().lower())
+        ]
+
         with self.acquire_rdbms_connection(auto_commit=False, connection=connection) as connection:
             # For any email address provided, determine the identification of the
             # corresponding account.
-            email_addresses = [
-                email_address
-                for email_address in account_ids
-                if isinstance(email_address, str)
-                   and REGEX_PATTERN_EMAIL_ADDRESS.match(email_address.strip().lower())
-            ]
-
             if email_addresses:
                 account_ids = account_ids - set(email_addresses)
                 cursor = connection.execute(
                     """
                     SELECT DISTINCT 
                         account_id
                       FROM 
@@ -1772,15 +1799,16 @@
                   FROM 
                     account
                   WHERE 
                     account_id IN (%(account_ids)s)
                 """,
                 {
                     'account_ids': list(account_ids),
-                })
+                }
+            )
 
             accounts = [
                 row.get_object({
                     'account_id': cast.string_to_uuid,
                     'language': cast.string_to_locale,
                     'object_status': ObjectStatus,
                     'update_time': cast.string_to_timestamp
@@ -1792,15 +1820,18 @@
                 if not include_hashed_password:
                     del account.password
 
                 account.picture_url = self.build_picture_url(account.picture_id)
 
             # Include the contacts information of the user accounts.
             if include_contacts:
-                accounts_dict = dict([(account.account_id, account) for account in accounts])
+                accounts_dict = {
+                    account.account_id: account
+                    for account in accounts
+                }
 
                 cursor = connection.execute(
                     """
                     SELECT 
                         account_id,
                         property_name,
                         property_value,
@@ -1810,27 +1841,30 @@
                         account_contact
                       WHERE
                         account_id IN (%(account_ids)s)
                         AND object_status = %(OBJECT_STATUS_ENABLED)s
                     """,
                     {
                         'OBJECT_STATUS_ENABLED': ObjectStatus.enabled,
-                        'account_ids': accounts_dict.keys()
-                    })
+                        'account_ids': list(accounts_dict.keys())
+                    }
+                )
 
-                accounts_contacts = collections.defaultdict(list)
-                for account_contact in [
+                contacts = [
                     row.get_object({
                         'account_id': cast.string_to_uuid,
                         'name': ContactName
                     })
                     for row in cursor.fetch_all()
-                ]:
-                    accounts_contacts[account_contact.account_id].append(account_contact)
-                    del account_contact.account_id
+                ]
+
+                accounts_contacts = collections.defaultdict(list)
+                for contact in contacts:
+                    accounts_contacts[contact.account_id].append(contact)
+                    del contact.account_id
 
                 for account_id, account_contacts in accounts_contacts.items():
                     accounts_dict[account_id].contacts = account_contacts
 
             return accounts
 
     def get_accounts_by_contacts(
@@ -2995,14 +3029,51 @@
                 'account_id': cast.string_to_uuid,
                 'object_status': ObjectStatus,
                 'update_time': cast.string_to_timestamp,
             })
 
             return account
 
+    def set_object_status(
+            self,
+            app_id: uuid.UUID,
+            account_id: uuid.UUID,
+            object_status: ObjectStatus,
+            connection: RdbmsConnection = None):
+        """
+        Set the new status of a user's account.
+
+
+        @param app_id: The identifier of the client application used to update
+            the status of the user's account.
+
+        @param account_id: The identifier of the user's account to change its
+            status.
+
+        @param object_status: The new status of the user's account.
+
+        @param connection: A connection to the account database.
+        """
+        with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
+            connection.execute(
+                """
+                UPDATE
+                    account
+                  SET
+                    object_status = %(object_status)s,
+                    update_time = current_timestamp
+                  WHERE
+                    account_id = %(account_id)s
+                """,
+                {
+                    'account_id': account_id,
+                    'object_status': object_status,
+                }
+            )
+
     def set_username(
             self,
             app_id,
             account_id,
             username,
             connection=None):
         """
@@ -3346,17 +3417,17 @@
         """
         SessionService().drop_session(app_id, session)
 
     def sign_up(
             self,
             account_type=AccountType.standard,
             action_type=None,
+            allow_undefined_password: bool = False,
             app_id=None,
             auto_sign_in=False,
-            bypass_recaptcha=True,
             can_password_be_changed=True,
             connection=None,
             contacts=None,
             context=None,
             inherited_table_name=None,
             does_password_never_expire=True,
             enable_account=True,
@@ -3364,15 +3435,14 @@
             is_password_change_required=False,
             first_name=None,
             full_name=None,
             last_name=None,
             nationality=None,
             password=None,
             language=None,
-            recaptcha=None,
             set_pending_if_unverified_contact=False,
             strict_prosoponym=True,
             team_id=None,
             to_be_verified=False,
             username=None,
             validate_password=True):
         """
@@ -3399,16 +3469,23 @@
         :param account_type: an item of `AccountType` that
             describes the context that caused the registration of this user
             account.
 
         :param action_type: Indicate the type of the action that initiates
             the request for verifying the specified contact information.
 
+        :param allow_undefined_password: Allow to create an account without
+            defining a password.
+
+            A user can create an account by linking it to an OAuth service
+            provider.  The user doesn't need to define a password; they will sign
+            in with their OAuth account link.
+
         :param auto_sign_in: Indicate whether the platform is requested to
-            sign-in this user once the sign-up procedure completes
+            sign in this user once the sign-up procedure completes
             successfully.
 
         :param can_password_be_changed: Indicate whether the user can change
             his password.
 
         :param connection: An object `RdbmsConnection` supporting the Python
             clause `with ...`.
@@ -3513,76 +3590,87 @@
             raise self.InvalidArgumentException(f'Unsupported type "{str(account_type)}" of user account')
 
         # A username must be provided when the given contact information has
         # not been verified.  The reason is if another user provides the same
         # contact information and it passes the verification challenge, this
         # identification will be reallocated to this second user account,
         # meaning that the first user won't have any more identification to
-        # sign-in to the platform.
+        # sign in to the platform.
         if not username and not contacts and account_type not in [
                 AccountType.sns,
                 AccountType.ghost
             ]:
             raise self.InvalidArgumentException(
-                "A username and/or a contact information MUST be provided")
+                "A username and/or a contact information MUST be provided"
+            )
 
         if username:
             username = username.strip().lower()
             if not self.is_username_available(app_id, username):
                 raise self.UsernameAlreadyUsedException(
-                    "This username is already associated with an existing user account"
+                    f"The username {username} is already associated with an existing user account"
                 )
 
         generate_password = password is None and enable_account and account_type not in [
                 AccountType.sns,
                 AccountType.ghost,
                 AccountType.botnet
         ]
         if generate_password:
-            password = self.__generate_password(self.MINIMUM_PASSWORD_LENGTH)
+            password = self.__generate_password(
+                length=self.MINIMUM_PASSWORD_LENGTH,
+                are_symbols_allowed=True
+            )
             generated_password = password
 
         if password:
             password = password.strip()
             if validate_password:
                 self.__validate_password_complexity_requirements(password)
             password = self.__encrypt_password(password)
 
+        elif not allow_undefined_password and account_type == AccountType.standard:
+            raise self.InvalidArgumentException("A password MUST be defined")
+
         if is_password_change_required and not can_password_be_changed:
             raise self.InvalidArgumentException(
                 f"Conflicting values of arguments `is_password_change_required` f{is_password_change_required} "
-                f"and `can_password_be_changed` f{can_password_be_changed}")
+                f"and `can_password_be_changed` f{can_password_be_changed}"
+            )
 
         # Format first name, last name, and full name.
         first_name = prosoponym.format_first_name(first_name, locale=language)
         last_name = prosoponym.format_last_name(last_name, locale=language)
         if first_name and last_name:
             full_name = prosoponym.format_full_name(
                 first_name,
                 last_name,
                 language,
                 full_name=full_name,
-                strict=strict_prosoponym)
+                strict=strict_prosoponym
+            )
 
-        # The creation of a user account requires to pass a reCAPTCHA
-        # challenge, except under the following conditions:
+        # @todo: Remove this security; way too much coupling.
         #
-        # * The function is explicitly requested to bypass the reCAPTCHA
-        #   challenge, which option is useful for internal service usage only,
-        #   when creating a new user account who authenticates with
-        #   credentials on trusted 3rd party platforms, such as an OAuth
-        #   access token.
-        # * The environment stage of the platform is development or
-        #   integration.
-        # * The user account to be created is either a botnet or a test
-        #   account.
-        if recaptcha:
-            (recaptcha_private_key, client_ip_address, recaptcha_challenge, recaptcha_response) = recaptcha
-            if not recaptcha.verify(recaptcha_private_key, client_ip_address, recaptcha_challenge, recaptcha_response):
-                raise self.IllegalAccessException('Incorrect reCAPTCHA response')
+        # # The creation of a user account requires to pass a reCAPTCHA
+        # # challenge, except under the following conditions:
+        # #
+        # # * The function is explicitly requested to bypass the reCAPTCHA
+        # #   challenge, which option is useful for internal service usage only,
+        # #   when creating a new user account who authenticates with
+        # #   credentials on trusted 3rd party platforms, such as an OAuth
+        # #   access token.
+        # # * The environment stage of the platform is development or
+        # #   integration.
+        # # * The user account to be created is either a botnet or a test
+        # #   account.
+        # if recaptcha:
+        #     (recaptcha_private_key, client_ip_address, recaptcha_challenge, recaptcha_response) = recaptcha
+        #     if not recaptcha.verify(recaptcha_private_key, client_ip_address, recaptcha_challenge, recaptcha_response):
+        #         raise self.IllegalAccessException('Incorrect reCAPTCHA response')
 
         if contacts:
             if not isinstance(contacts, (list, set, tuple)):
                 contacts = [contacts]
 
             for contact in contacts:
                 print(f"Verifying the contact {contact.property_value} ({contact.property_name})")
@@ -3645,17 +3733,18 @@
                     'is_password_change_required': is_password_change_required,
                     'first_name': first_name or None,
                     'full_name': full_name,
                     'last_name': last_name or None,
                     'language': language or DEFAULT_LOCALE,
                     'nationality': nationality,
                     'object_status': ObjectStatus.enabled if enable_account else ObjectStatus.pending,
-                    'password': password,
+                    'password': password or None,
                     'username': username or None,
-                })
+                }
+            )
 
             account = cursor.fetch_one().get_object({
                 'account_id': cast.string_to_uuid,
                 'creation_time': cast.string_to_timestamp,
                 'language': cast.string_to_locale,
             })
 
@@ -3697,19 +3786,20 @@
 
                 account_session.creation_time = account.creation_time
                 account_session.language = account.language
                 account_session.object_status = account.object_status
 
                 self.__update_last_login_time(account.account_id, connection)
 
-        # :todo: Remove this ugly hack with a message queue system.
+        response = account_session if auto_sign_in else account
+
         if generate_password:
-            account.password = generated_password
+            response.password = generated_password
 
-        return account_session if auto_sign_in else account
+        return response
 
     def update_password_reset_request(
             self,
             request_id,
             connection=None,
             object_status=ObjectStatus.deleted):
         """
@@ -3829,15 +3919,15 @@
                     ObjectStatus.enabled,
                     connection=connection
                 )
         else:
             # Check that the capture time of the photo is not in the future.
             capture_time = self.__adjust_photo_capture_time(capture_time)
 
-            # Register the photo
+            # Register the photo.
             picture = self.__add_picture(
                 app_id,
                 account_id,
                 submitter_account_id,
                 capture_time,
                 image,
                 image_file_checksum,
```

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/contact_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/contact_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_account_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_account_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/create_session_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/create_session_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table.718.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table.718.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.11.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.12.9.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.14.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.17.31.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.21.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.22.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.24.0.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.12.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/db/migrate_account_table@1.25.19.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/oauth_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/oauth_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/session_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/session_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/account/test/account_service_unittest.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/account/test/account_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/application_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/application_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/db/create_application_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/db/create_application_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/application/test/application_service_unittest.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/application/test/application_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/area_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/area_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area2sql.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/area_extractor.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/area_extractor.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/data/vietnam/vietnamese_administrative_area_boundaries.json.zip`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_dataset.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_area_type.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_area_type.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_geoip_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_geoip_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_mobile-phone-operator_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/create_rir_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/create_rir_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/db/migrate_area_dataset.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/db/migrate_area_dataset.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_geolite_importer.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_geolite_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/_rir_importer.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/_rir_importer.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/area/script/geoip2sql.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/area/script/geoip2sql.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_http_handler.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_http_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             @param object_class: Python class to be used to instantiate a new
                 object from the JSON value of the given argument when the
                 specified data type of this argument is `object`.  This Python
                 class MUST implement a static method `from json` that returns an
                 instance of this class providing a JSON expression.
 
 
-            @return: The casted value of the argument.
+            @return: The cast value of the argument.
 
 
             @raise MissingArgumentException: If the JSON expression doesn't
                 contain the specified argument while this argument is required.
             """
             if not isinstance(payload, dict):
                 raise ValueError("The argument 'payload' MUST be a dictionary")
@@ -1160,15 +1160,15 @@
         @param result: result returned by the RESTful API service method that
             has processed a HTTP request.
         """
         # Convert the result to an empty dictionary if the result is null, or
         # a dictionary with a unique entry `data` if the result is not a
         # Python built-in collections, nor an object having `__dict__` attribute.
         self._result = dict() if result is None \
-            else result if (isinstance(result, (list, set, tuple)) or hasattr(result, '__dict__')) \
+            else result if (isinstance(result, (dict, list, set, tuple)) or hasattr(result, '__dict__')) \
             else dict(data=result)
 
     def __str__(self):
         """
         Return a string representation of the JSON expression of the result
         returned by the RESTful API service method that has processed a HTTP
         request.
```

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_job_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_job_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_rdbms_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_rdbms_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/base_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/base_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/agent/push_notification.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/agent/push_notification.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/db/create_notification_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/db/create_notification_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/gcm.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/gcm.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/notification/notification_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_ping.rst` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_ping.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/get_status.rst` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/get_status.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/doc/api/index.rst` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/status/status_service_http_handler.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/status/status_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/agent/team_invite.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/agent/team_invite.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_constraint.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_constraint.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_function.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_function.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_index.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_index.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/create_team_table.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/create_team_table.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/db/migrate_team_table@1.13.3.sql`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/team_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/team_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 import traceback
 import uuid
 
 from PIL import Image
 from majormode.perseus.constant.team import MemberRole
 from majormode.perseus.constant.contact import ContactName
 from majormode.perseus.constant.obj import ObjectStatus
+from majormode.perseus.utils.rdbms import RdbmsConnection
+
 from majormode.perseus.service.account.account_service import AccountService
 from majormode.perseus.service.base_rdbms_service import BaseRdbmsService
 from majormode.perseus.service.base_service import BaseService
 from majormode.perseus.utils import cast
 from majormode.perseus.utils import file_util
 from majormode.perseus.utils import image_util
 from majormode.perseus.utils import key_util
@@ -2728,14 +2730,85 @@
                   ON CONFLICT DO NOTHING
                 """,
                 {
                     'account_id': account_id,
                     'team_id': team_id
                 })
 
+    def set_member_role(
+            self,
+            team_id: uuid.UUID,
+            account_id: uuid.UUID,
+            role: any,
+            connection: RdbmsConnection = None) -> any:
+        """
+        Change the role of a team member.
+
+
+        :param team_id: The identifier of a team.
+
+        :param account_id: The identifier of the team member to change their
+            role.
+
+        :param role: The new role of the team member.
+
+        :param connection: A connection to the team database.
+
+
+        :return: An object containing the following attributes:
+
+            - ``account_id: UUID`` (required): The identifier of the team member's
+              account.
+
+            - ``team_id: UUID`` (required): The identifier of the team.
+
+            - ``update_time: ISO8601DateTime`` (required): The time of the most
+              recent modification of the team member's information.
+
+
+        :raise UndefinedObjectException: If the team or the team member
+            doesn't exist.
+        """
+        with self.acquire_rdbms_connection(auto_commit=True, connection=connection) as connection:
+            cursor = connection.execute(
+                """
+                UPDATE
+                    team_member
+                  SET
+                    role = %(role)s,
+                    update_time = current_timestamp
+                  WHERE
+                    team_id = %(team_id)s
+                    AND account_id = %(account_id)s
+                  RETURNING
+                    account_id,
+                    team_id,
+                    update_time
+                """,
+                {
+                    'account_id': account_id,
+                    'role': role,
+                    'team_id': team_id,
+                }
+            )
+
+            row = cursor.fetch_one()
+            if not row:
+                raise self.UndefinedObjectException(
+                    f"The member {account_id} of the team {team_id} doesn't exist"
+                )
+
+            member_info = row.get_object({
+                'account_id': cast.string_to_uuid,
+                'team_id': cast.string_to_uuid,
+                'update_time': cast.string_to_timestamp
+            })
+
+            return member_info
+
     def upload_logo(
             self,
             team_id,
             account_id,
             logo_file,
             connection=None,
             image_file_format=DEFAULT_LOGO_IMAGE_FILE_FORMAT,
```

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/template/default_invite_email.txt` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/template/default_invite_email.txt`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/team/test/team_service_unittest.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/team/test/team_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/get_version.rst` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/get_version.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/doc/api/index.rst` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/__init__.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/__init__.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/test/version_service_unittest.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/test/version_service_unittest.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/src/majormode/perseus/service/version/version_service_http_handler.py` & `perseus_restful_api_framework-1.27.0/src/majormode/perseus/service/version/version_service_http_handler.py`

 * *Files identical despite different names*

### Comparing `perseus_restful_api_framework-1.26.9/setup.py` & `perseus_restful_api_framework-1.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  'prosoponym>=1.0.7,<2.0.0',
  'psutil>=5.9.4,<6.0.0',
  'pymemcache>=4.0.0,<5.0.0',
  'tornado>=6.2,<7.0']
 
 setup_kwargs = {
     'name': 'perseus-restful-api-framework',
-    'version': '1.26.9',
+    'version': '1.27.0',
     'description': 'Python server framework for quickly building RESTful APIs with minimal effort',
     'long_description': '# Perseus: RESTful API Server Framework\n\nPerseus is a Python framework for quickly building RESTful API servers with minimal effort.\n\nPerseus provides an initial set of core services that supports the following features:\n\n- Client application registration with API keys generation\n- Client application access control with RESTful request signature\n- Client application and RESTful API server version compatibility check\n- User authentication and session management\n- Team/group management\n- RESTful request logging with data sensitiveness support\n- RESTful service automatic discovery\n- HTTP request query parameters & body JSON message automatically parsing (depending on the HTTP method used) with data type check and conversion\n\nPerseus is based on [Tornado](https://www.tornadoweb.org/) for handling client network connection.\n\n## RESTful API Request Handler\n\n```python\nfrom majormode.perseus.service.base_http_handler import HttpRequest\nfrom majormode.perseus.service.base_http_handler import HttpRequestHandler\nfrom majormode.perseus.service.base_http_handler import http_request\n\nimport AttendantService\n\n\nclass AttendantServiceHttpRequestHandler(HttpRequestHandler):\n    @http_request(r\'^/attendant/session$\',\n                  http_method=HttpRequest.HttpMethod.POST,\n                  authentication_required=False,\n                  sensitive_data=True,\n                  signature_required=False)\n    def sign_in(self, request):\n        email_address = request.get_argument(\n            \'email_address\',\n            data_type=HttpRequest.ArgumentDataType.email_address,\n            is_required=True)\n\n        password = request.get_argument(\n            \'password\',\n            data_type=HttpRequest.ArgumentDataType.string,\n            is_required=True)\n\n        return AttendantService().sign_in(request.app_id, email_address, password)\n```\n\n## Configure the environment variables\n\n```env\n# Copyright (C) 2021 Majormode.  All rights reserved.\n#\n# Permission is hereby granted, free of charge, to any person obtaining\n# a copy of this software and associated documentation files (the\n# "Software"), to deal in the Software without restriction, including\n# without limitation the rights to use, copy, modify, merge, publish,\n# distribute, sublicense, and/or sell copies of the Software, and to\n# permit persons to whom the Software is furnished to do so, subject to\n# the following conditions:\n#\n# The above copyright notice and this permission notice shall be\n# included in all copies or substantial portions of the Software.\n#\n# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,\n# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\n# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\n# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\n# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n# Connection properties of the RESTful API server instances.  Defaults\n# to 127.0.0.1:8081.\nAPI_SERVER_HOSTNAME=127.0.0.1\nAPI_SERVER_PORTS=\n\n# Root path of the Network File System (NFS) -- referring to the\n# distributed file system (not the protocol) -- where the Content\n# Delivery Network (CDN) files are stored into, such as avatars, etc.\nCDN_NFS_ROOT_PATH=\n\n# Hostname of the Content Delivery Network (CDN) server that hosts media\n# files such as avatars, etc.\nCDN_URL_HOSTNAME=\n\n# Environment stage of the API server instances.  Possible values are:\n#\n# - dev\n# - int\n# - staging\n# - prod\n#\n# Defaults to `dev`.\nENVIRONMENT_STAGE=\n\n# Connection properties to a Memcached server (a distributed memory\n# object caching system).  Defaults to 127.0.0.1:11211.\nMEMCACHED_HOSTNAME = \'127.0.0.1\'\nMEMCACHED_PORT = 11211\n\n# Threshold for the logger to level.  Logging messages which are less\n# severe than the specified level will be ignored; logging messages\n# which have this severity level or higher will be emitted.  Possible\n# values are:\n#\n# - debug\n# - info\n# - warning\n# - error\n# - critical\n#\n# Default to \'debug\'.\nLOGGING_LEVEL=\n\n# Environment variables to select default parameter values to connect\n# to PostgreSQL Relational Database Management System.\nPG_HOSTNAME=localhost\nPG_PORT=5432\nPG_DATABASE_NAME=\nPG_USERNAME=\nPG_PASSWORD=\n```\n\n## Run the RESTful API Server Processes\n\n```bash\n$ fab start --port=65180,65181,...\n```\n\nHashtags/Topics: `#perseus` `#restful` `#api` `#server` `#framework` `#python`\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel.caune@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/majormode/perseus-restful-api-server-framework',
```

### Comparing `perseus_restful_api_framework-1.26.9/PKG-INFO` & `perseus_restful_api_framework-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perseus-restful-api-framework
-Version: 1.26.9
+Version: 1.27.0
 Summary: Python server framework for quickly building RESTful APIs with minimal effort
 Home-page: https://github.com/majormode/perseus-restful-api-server-framework
 License: Proprietary
 Keywords: perseus,resful,api,server,framework
 Author: Daniel CAUNE
 Author-email: daniel.caune@gmail.com
 Requires-Python: >=3.9,<4.0
```

