# Comparing `tmp/edc-protocol-incident-0.1.25.tar.gz` & `tmp/edc-protocol-incident-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-protocol-incident-0.1.25.tar", last modified: Wed May 24 16:57:42 2023, max compression
+gzip compressed data, was "edc-protocol-incident-0.1.26.tar", last modified: Mon Jul 10 15:04:35 2023, max compression
```

## Comparing `edc-protocol-incident-0.1.25.tar` & `edc-protocol-incident-0.1.26.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.412697 edc-protocol-incident-0.1.25/
--rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.25/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.396960 edc-protocol-incident-0.1.25/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.401040 edc-protocol-incident-0.1.25/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.25/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.25/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.25/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.25/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-09 17:06:27.000000 edc-protocol-incident-0.1.25/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.25/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-05-24 16:57:42.412809 edc-protocol-incident-0.1.25/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1232 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.25/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.403135 edc-protocol-incident-0.1.25/edc_protocol_incident/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1331 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.404349 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2592 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/protocol_deviation_violation_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      475 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin/protocol_incident_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1637 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.404954 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1554 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_incident_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.405387 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      992 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_deviation_violation_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      794 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_incident_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1552 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.408300 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    31949 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    73009 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0002_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1181 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0003_auto_20211104_1456.py
--rw-r--r--   0 erikvw     (501) staff       (20)      719 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26979 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2621 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1455 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0007_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1086 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1217 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0009_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1091 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0010_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0011_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)      867 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0012_auto_20220913_2139.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2207 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0013_auto_20220927_0349.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1380 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0014_auto_20220927_0400.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0015_auto_20220927_0401.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1890 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      690 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.408701 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4116 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3943 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/modeladmin_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.409386 edc-protocol-incident-0.1.25/edc_protocol_incident/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/list_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_deviation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_incident.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.409585 edc-protocol-incident-0.1.25/edc_protocol_incident/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/pdf_reports/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.410536 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.411890 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.412510 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5901 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_incident.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9323 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.25/edc_protocol_incident/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:57:42.404007 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3971 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-27 01:17:18.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-05-24 16:57:42.000000 edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1788 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.25/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1128 2022-09-28 03:06:58.000000 edc-protocol-incident-0.1.25/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1241 2023-05-24 16:57:42.413132 edc-protocol-incident-0.1.25/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.393442 edc-protocol-incident-0.1.26/
+-rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.26/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.375215 edc-protocol-incident-0.1.26/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.379937 edc-protocol-incident-0.1.26/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.26/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.26/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2021-09-10 21:37:33.000000 edc-protocol-incident-0.1.26/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.26/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-09 17:06:27.000000 edc-protocol-incident-0.1.26/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 17:50:51.000000 edc-protocol-incident-0.1.26/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-07-10 15:04:35.393562 edc-protocol-incident-0.1.26/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1232 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:41:59.000000 edc-protocol-incident-0.1.26/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.382819 edc-protocol-incident-0.1.26/edc_protocol_incident/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1331 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.384088 edc-protocol-incident-0.1.26/edc_protocol_incident/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2592 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/admin/protocol_deviation_violation_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      475 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/admin/protocol_incident_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      244 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      892 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1637 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.384875 edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      182 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1554 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/protocol_incident_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.385356 edc-protocol-incident-0.1.26/edc_protocol_incident/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      135 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      992 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/forms/protocol_deviation_violation_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      794 2022-10-04 02:54:16.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/forms/protocol_incident_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1552 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.389064 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    31949 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    73009 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2355 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0002_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1181 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0003_auto_20211104_1456.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      719 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26979 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2621 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1455 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0007_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1086 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1217 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0009_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1091 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0010_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      783 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0011_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      867 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0012_auto_20220913_2139.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2207 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0013_auto_20220927_0349.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1380 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0014_auto_20220927_0400.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1179 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0015_auto_20220927_0401.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1890 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      690 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1592 2023-07-10 15:04:28.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.389547 edc-protocol-incident-0.1.26/edc_protocol_incident/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      170 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4116 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3943 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3887 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/modeladmin_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.390455 edc-protocol-incident-0.1.26/edc_protocol_incident/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      773 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/models/list_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1018 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/models/protocol_deviation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      946 2022-09-29 19:42:41.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/models/protocol_incident.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.390725 edc-protocol-incident-0.1.26/edc_protocol_incident/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/pdf_reports/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.391419 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      606 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.392850 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1895 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)       73 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.393278 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5901 2022-11-30 22:26:19.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/tests/test_protocol_incident.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9323 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/tests/test_protocol_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2022-09-27 01:17:10.000000 edc-protocol-incident-0.1.26/edc_protocol_incident/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 15:04:35.383665 edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2168 2023-07-10 15:04:35.000000 edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4062 2023-07-10 15:04:35.000000 edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-10 15:04:35.000000 edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-27 01:17:18.000000 edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2023-07-10 15:04:35.000000 edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1788 2023-05-24 16:57:33.000000 edc-protocol-incident-0.1.26/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1128 2022-09-28 03:06:58.000000 edc-protocol-incident-0.1.26/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1241 2023-07-10 15:04:35.393908 edc-protocol-incident-0.1.26/setup.cfg
```

### Comparing `edc-protocol-incident-0.1.25/.github/workflows/build.yml` & `edc-protocol-incident-0.1.26/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/.gitignore` & `edc-protocol-incident-0.1.26/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/.pre-commit-config.yaml` & `edc-protocol-incident-0.1.26/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/LICENSE` & `edc-protocol-incident-0.1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/PKG-INFO` & `edc-protocol-incident-0.1.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-protocol-incident
-Version: 0.1.25
+Version: 0.1.26
 Summary: Classes for protocol incident (violations/deviations) in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-protocol-incident
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol incident violations deviations,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-protocol-incident-0.1.25/README.rst` & `edc-protocol-incident-0.1.26/README.rst`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/action_items.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/admin/protocol_deviation_violation_admin.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/admin/protocol_deviation_violation_admin.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/auth_objects.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/auths.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/auths.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/mixins.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/mixins.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/protocol_deviation_violation_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/form_validators/protocol_incident_form_validator.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/form_validators/protocol_incident_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_deviation_violation_form.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/forms/protocol_deviation_violation_form.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/forms/protocol_incident_form.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/forms/protocol_incident_form.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/list_data.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_initial.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0001_squashed_0015_auto_20220927_0401.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0002_auto_20210911_2036.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0002_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0003_auto_20211104_1456.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0003_auto_20211104_1456.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0004_alter_protocoldeviationviolation_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0005_protocolincident_historicalprotocolincident_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0006_protocolincidents_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0007_auto_20220704_1841.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0007_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0008_alter_historicalprotocoldeviationviolation_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0009_auto_20220826_0258.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0009_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0010_auto_20220826_0322.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0010_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0011_auto_20220826_0406.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0011_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0012_auto_20220913_2139.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0012_auto_20220913_2139.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0013_auto_20220927_0349.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0013_auto_20220927_0349.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0014_auto_20220927_0400.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0014_auto_20220927_0400.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0015_auto_20220927_0401.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0015_auto_20220927_0401.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/modeladmin_mixins.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/models/list_models.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/models/list_models.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_deviation_violation.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/models/protocol_deviation_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/models/protocol_incident.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/action_items.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-local-private.pem` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/holidays.csv` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_incident.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/tests/test_protocol_incident.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/tests/test_protocol_violation.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/tests/test_protocol_violation.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident/tests/visit_schedule.py` & `edc-protocol-incident-0.1.26/edc_protocol_incident/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/PKG-INFO` & `edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-protocol-incident
-Version: 0.1.25
+Version: 0.1.26
 Summary: Classes for protocol incident (violations/deviations) in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-protocol-incident
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol incident violations deviations,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-protocol-incident-0.1.25/edc_protocol_incident.egg-info/SOURCES.txt` & `edc-protocol-incident-0.1.26/edc_protocol_incident.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 edc_protocol_incident/migrations/0011_auto_20220826_0406.py
 edc_protocol_incident/migrations/0012_auto_20220913_2139.py
 edc_protocol_incident/migrations/0013_auto_20220927_0349.py
 edc_protocol_incident/migrations/0014_auto_20220927_0400.py
 edc_protocol_incident/migrations/0015_auto_20220927_0401.py
 edc_protocol_incident/migrations/0016_historicalprotocolincident_reasons_withdrawn_and_more.py
 edc_protocol_incident/migrations/0017_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
+edc_protocol_incident/migrations/0018_alter_protocoldeviationviolation_options_and_more.py
 edc_protocol_incident/migrations/__init__.py
 edc_protocol_incident/model_mixins/__init__.py
 edc_protocol_incident/model_mixins/protocol_deviation_violation_model_mixin.py
 edc_protocol_incident/model_mixins/protocol_incident_model_mixin.py
 edc_protocol_incident/models/__init__.py
 edc_protocol_incident/models/list_models.py
 edc_protocol_incident/models/protocol_deviation_violation.py
```

### Comparing `edc-protocol-incident-0.1.25/pyproject.toml` & `edc-protocol-incident-0.1.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/runtests.py` & `edc-protocol-incident-0.1.26/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-incident-0.1.25/setup.cfg` & `edc-protocol-incident-0.1.26/setup.cfg`

 * *Files identical despite different names*

