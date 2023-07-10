# Comparing `tmp/leanit-mweb-23.7.2.tar.gz` & `tmp/leanit-mweb-23.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanit-mweb-23.7.2.tar", last modified: Wed Jul  5 13:10:13 2023, max compression
+gzip compressed data, was "leanit-mweb-23.7.3.tar", last modified: Mon Jul 10 12:26:12 2023, max compression
```

## Comparing `leanit-mweb-23.7.2.tar` & `leanit-mweb-23.7.3.tar`

### file list

```diff
@@ -1,90 +1,94 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/
--rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.7.2/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1921 2023-06-21 11:11:08.000000 leanit-mweb-23.7.2/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/leanit_mweb.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/leanit_mweb.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     1593 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/leanit_mweb.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/leanit_mweb.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      549 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/leanit_mweb.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/leanit_mweb.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/
--rw-rw-r--   0 martin    (1000) martin    (1000)    14868 2023-07-05 12:46:44.000000 leanit-mweb-23.7.2/mweb/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/auth/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:18:02.000000 leanit-mweb-23.7.2/mweb/auth/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/auth/sso/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:23:33.000000 leanit-mweb-23.7.2/mweb/auth/sso/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      381 2023-06-30 09:43:07.000000 leanit-mweb-23.7.2/mweb/auth/sso/base.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/auth/sso/microsoft/
--rw-rw-r--   0 martin    (1000) martin    (1000)     5994 2023-07-05 13:09:44.000000 leanit-mweb-23.7.2/mweb/auth/sso/microsoft/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.7.2/mweb/form.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/jinja_template/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2001 2023-07-05 12:31:10.000000 leanit-mweb-23.7.2/mweb/jinja_template/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.7.2/mweb/jinja_template/loaders.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1995 2023-06-30 11:57:20.000000 leanit-mweb-23.7.2/mweb/manage.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/messaging/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.7.2/mweb/messaging/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.7.2/mweb/messaging/base.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.7.2/mweb/orm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.7.2/mweb/orm/exception.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.663802 leanit-mweb-23.7.2/mweb/orm/fields/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2809 2023-06-30 13:17:38.000000 leanit-mweb-23.7.2/mweb/orm/fields/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-06-30 11:55:37.000000 leanit-mweb-23.7.2/mweb/orm/fields/snowflake.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17508 2023-07-05 09:48:32.000000 leanit-mweb-23.7.2/mweb/orm/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.7.2/mweb/orm/password.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/mweb/security/
--rw-rw-r--   0 martin    (1000) martin    (1000)      564 2023-06-27 15:25:35.000000 leanit-mweb-23.7.2/mweb/security/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2135 2023-06-30 09:59:15.000000 leanit-mweb-23.7.2/mweb/security/jwt.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.7.2/mweb/staticfiles.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2745 2023-06-14 06:12:52.000000 leanit-mweb-23.7.2/mweb/testutils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-06-06 11:14:00.000000 leanit-mweb-23.7.2/mweb/thread.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/mweb/utils/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2906 2023-07-01 08:58:49.000000 leanit-mweb-23.7.2/mweb/utils/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/mweb/utils/id/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:02:22.000000 leanit-mweb-23.7.2/mweb/utils/id/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1345 2023-06-30 09:04:34.000000 leanit-mweb-23.7.2/mweb/utils/id/snowflakeid.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      931 2023-07-05 09:13:08.000000 leanit-mweb-23.7.2/mweb/utils/log_catcher.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/mweb/version.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/mweb/views/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.7.2/mweb/views/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1092 2023-06-30 11:57:20.000000 leanit-mweb-23.7.2/mweb/views/auth.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6900 2023-07-05 10:05:44.000000 leanit-mweb-23.7.2/mweb/views/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10602 2023-07-05 10:55:32.000000 leanit-mweb-23.7.2/mweb/yuga.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1912 2023-07-05 13:10:13.000000 leanit-mweb-23.7.2/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 12:07:34.000000 leanit-mweb-23.7.2/tests/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/auth/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.2/tests/auth/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/auth/sso/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.2/tests/auth/sso/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/auth/sso/microsoft/
--rw-rw-r--   0 martin    (1000) martin    (1000)      210 2023-06-30 09:30:02.000000 leanit-mweb-23.7.2/tests/auth/sso/microsoft/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1824 2023-06-30 09:36:45.000000 leanit-mweb-23.7.2/tests/auth/sso/microsoft/test_auth_callback.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1797 2023-06-30 09:36:45.000000 leanit-mweb-23.7.2/tests/auth/sso/microsoft/test_build_auth_url.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      591 2023-06-30 09:30:07.000000 leanit-mweb-23.7.2/tests/auth/sso/microsoft/test_code.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:31.000000 leanit-mweb-23.7.2/tests/orm/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/orm/fields/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 07:10:28.000000 leanit-mweb-23.7.2/tests/orm/fields/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      706 2023-06-30 11:55:37.000000 leanit-mweb-23.7.2/tests/orm/fields/test_StringField.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/orm/model/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:39.000000 leanit-mweb-23.7.2/tests/orm/model/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1158 2023-06-30 12:03:34.000000 leanit-mweb-23.7.2/tests/orm/model/test_delete_all.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.667801 leanit-mweb-23.7.2/tests/resources/
--rw-rw-r--   0 martin    (1000) martin    (1000)       76 2023-07-02 16:02:44.000000 leanit-mweb-23.7.2/tests/resources/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/tests/security/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-28 15:18:34.000000 leanit-mweb-23.7.2/tests/security/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1110 2023-06-29 11:38:56.000000 leanit-mweb-23.7.2/tests/security/test_jwt.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      685 2023-06-29 11:18:38.000000 leanit-mweb-23.7.2/tests/security/test_sign.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/tests/utils/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-29 11:22:08.000000 leanit-mweb-23.7.2/tests/utils/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1836 2023-06-30 11:57:20.000000 leanit-mweb-23.7.2/tests/utils/test_form.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      537 2023-06-30 09:05:14.000000 leanit-mweb-23.7.2/tests/utils/test_snowflake.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-07-01 08:58:49.000000 leanit-mweb-23.7.2/tests/utils/test_unflatten.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/tests/views/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:48.000000 leanit-mweb-23.7.2/tests/views/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 13:10:13.671801 leanit-mweb-23.7.2/tests/views/model/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:56.000000 leanit-mweb-23.7.2/tests/views/model/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9069 2023-07-03 08:51:42.000000 leanit-mweb-23.7.2/tests/views/model/test_paging.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.7.3/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1921 2023-06-21 11:11:08.000000 leanit-mweb-23.7.3/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.995072 leanit-mweb-23.7.3/leanit_mweb.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2430 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1676 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      549 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       11 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/leanit_mweb.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    15058 2023-07-05 16:14:36.000000 leanit-mweb-23.7.3/mweb/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/auth/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:18:02.000000 leanit-mweb-23.7.3/mweb/auth/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/auth/sso/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:23:33.000000 leanit-mweb-23.7.3/mweb/auth/sso/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      381 2023-06-30 09:43:07.000000 leanit-mweb-23.7.3/mweb/auth/sso/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/auth/sso/microsoft/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7847 2023-07-05 14:34:14.000000 leanit-mweb-23.7.3/mweb/auth/sso/microsoft/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.7.3/mweb/form.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/jinja_template/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2671 2023-07-05 15:16:21.000000 leanit-mweb-23.7.3/mweb/jinja_template/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.7.3/mweb/jinja_template/loaders.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1995 2023-06-30 11:57:20.000000 leanit-mweb-23.7.3/mweb/manage.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:11.999072 leanit-mweb-23.7.3/mweb/messaging/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:21.000000 leanit-mweb-23.7.3/mweb/messaging/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-19 13:00:37.000000 leanit-mweb-23.7.3/mweb/messaging/base.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.7.3/mweb/orm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.7.3/mweb/orm/exception.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/orm/fields/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2921 2023-07-07 08:58:44.000000 leanit-mweb-23.7.3/mweb/orm/fields/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-06-30 11:55:37.000000 leanit-mweb-23.7.3/mweb/orm/fields/snowflake.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17596 2023-07-07 08:55:19.000000 leanit-mweb-23.7.3/mweb/orm/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.7.3/mweb/orm/password.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/security/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      564 2023-06-27 15:25:35.000000 leanit-mweb-23.7.3/mweb/security/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2135 2023-06-30 09:59:15.000000 leanit-mweb-23.7.3/mweb/security/jwt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.7.3/mweb/staticfiles.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3372 2023-07-07 08:33:20.000000 leanit-mweb-23.7.3/mweb/testutils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-06-06 11:14:00.000000 leanit-mweb-23.7.3/mweb/thread.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.003072 leanit-mweb-23.7.3/mweb/utils/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2910 2023-07-07 09:14:22.000000 leanit-mweb-23.7.3/mweb/utils/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/mweb/utils/id/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:02:22.000000 leanit-mweb-23.7.3/mweb/utils/id/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1345 2023-06-30 09:04:34.000000 leanit-mweb-23.7.3/mweb/utils/id/snowflakeid.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      663 2023-07-07 09:14:55.000000 leanit-mweb-23.7.3/mweb/utils/log.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      931 2023-07-05 09:13:08.000000 leanit-mweb-23.7.3/mweb/utils/log_catcher.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/mweb/version.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/mweb/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-17 08:14:19.000000 leanit-mweb-23.7.3/mweb/views/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1092 2023-06-30 11:57:20.000000 leanit-mweb-23.7.3/mweb/views/auth.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6900 2023-07-05 10:05:44.000000 leanit-mweb-23.7.3/mweb/views/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10602 2023-07-05 10:55:32.000000 leanit-mweb-23.7.3/mweb/yuga.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1912 2023-07-10 12:26:11.000000 leanit-mweb-23.7.3/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 12:07:34.000000 leanit-mweb-23.7.3/tests/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/tests/auth/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.3/tests/auth/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.007072 leanit-mweb-23.7.3/tests/auth/sso/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-30 09:29:21.000000 leanit-mweb-23.7.3/tests/auth/sso/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/auth/sso/microsoft/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      210 2023-06-30 09:30:02.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1824 2023-06-30 09:36:45.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_auth_callback.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1797 2023-06-30 09:36:45.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_build_auth_url.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      591 2023-06-30 09:30:07.000000 leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_code.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:31.000000 leanit-mweb-23.7.3/tests/orm/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/orm/fields/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 07:10:28.000000 leanit-mweb-23.7.3/tests/orm/fields/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      873 2023-07-07 08:53:27.000000 leanit-mweb-23.7.3/tests/orm/fields/test_StringField.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/orm/model/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-14 06:24:39.000000 leanit-mweb-23.7.3/tests/orm/model/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1158 2023-06-30 12:03:34.000000 leanit-mweb-23.7.3/tests/orm/model/test_delete_all.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/resources/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       76 2023-07-02 16:02:44.000000 leanit-mweb-23.7.3/tests/resources/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.011072 leanit-mweb-23.7.3/tests/security/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-28 15:18:34.000000 leanit-mweb-23.7.3/tests/security/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1110 2023-06-29 11:38:56.000000 leanit-mweb-23.7.3/tests/security/test_jwt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      685 2023-06-29 11:18:38.000000 leanit-mweb-23.7.3/tests/security/test_sign.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/utils/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-06-29 11:22:08.000000 leanit-mweb-23.7.3/tests/utils/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/utils/log/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-07 09:15:39.000000 leanit-mweb-23.7.3/tests/utils/log/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      402 2023-07-07 09:16:21.000000 leanit-mweb-23.7.3/tests/utils/log/test_hide_secrets.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1836 2023-06-30 11:57:20.000000 leanit-mweb-23.7.3/tests/utils/test_form.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      537 2023-06-30 09:05:14.000000 leanit-mweb-23.7.3/tests/utils/test_snowflake.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      469 2023-07-01 08:58:49.000000 leanit-mweb-23.7.3/tests/utils/test_unflatten.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/views/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:48.000000 leanit-mweb-23.7.3/tests/views/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-10 12:26:12.015071 leanit-mweb-23.7.3/tests/views/model/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-07-02 15:26:56.000000 leanit-mweb-23.7.3/tests/views/model/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9069 2023-07-03 08:51:42.000000 leanit-mweb-23.7.3/tests/views/model/test_paging.py
```

### Comparing `leanit-mweb-23.7.2/LICENSE` & `leanit-mweb-23.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/PKG-INFO` & `leanit-mweb-23.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leanit-mweb
-Version: 23.7.2
+Version: 23.7.3
 Summary: Web framework
 Author: Martin Klapproth
 Author-email: martin.klapproth@staxnet.de
 Keywords: python,web
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `leanit-mweb-23.7.2/README.md` & `leanit-mweb-23.7.3/README.md`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/leanit_mweb.egg-info/PKG-INFO` & `leanit-mweb-23.7.3/leanit_mweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leanit-mweb
-Version: 23.7.2
+Version: 23.7.3
 Summary: Web framework
 Author: Martin Klapproth
 Author-email: martin.klapproth@staxnet.de
 Keywords: python,web
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `leanit-mweb-23.7.2/leanit_mweb.egg-info/SOURCES.txt` & `leanit-mweb-23.7.3/leanit_mweb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 mweb/orm/model.py
 mweb/orm/password.py
 mweb/orm/fields/__init__.py
 mweb/orm/fields/snowflake.py
 mweb/security/__init__.py
 mweb/security/jwt.py
 mweb/utils/__init__.py
+mweb/utils/log.py
 mweb/utils/log_catcher.py
 mweb/utils/id/__init__.py
 mweb/utils/id/snowflakeid.py
 mweb/views/__init__.py
 mweb/views/auth.py
 mweb/views/model.py
 tests/__init__.py
@@ -53,10 +54,12 @@
 tests/security/__init__.py
 tests/security/test_jwt.py
 tests/security/test_sign.py
 tests/utils/__init__.py
 tests/utils/test_form.py
 tests/utils/test_snowflake.py
 tests/utils/test_unflatten.py
+tests/utils/log/__init__.py
+tests/utils/log/test_hide_secrets.py
 tests/views/__init__.py
 tests/views/model/__init__.py
 tests/views/model/test_paging.py
```

### Comparing `leanit-mweb-23.7.2/leanit_mweb.egg-info/requires.txt` & `leanit-mweb-23.7.3/leanit_mweb.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/__init__.py` & `leanit-mweb-23.7.3/mweb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,20 +380,23 @@
         # import views
         module_name = self.__module__  # "mium_frontend"
         views_module_name = f"{module_name}.views"
         views_module = None
         try:
             views_module = importlib.import_module(views_module_name)
         except ImportError as e:
-            logger.info(f"no views package found for {module_name}: {e}")
+            logger.info(f"no views package found for {module_name}: {e} while trying to import {views_module_name}")
 
         if views_module:
             for importer, modname, ispkg in pkgutil.walk_packages(path=views_module.__path__,
                                                                   prefix=views_module.__name__ + '.'):
-                module = importlib.import_module(modname)
+                try:
+                    module = importlib.import_module(modname)
+                except ImportError as e:
+                    raise ImportError(f"could not import {modname}: {e}") from e
 
         # validate views
         from mweb.views.model import ModelView
         model_views = ModelView.__subclasses__()
 
         for model_view_class in model_views:
             self._validate_model_view(model_view_class)
```

### Comparing `leanit-mweb-23.7.2/mweb/jinja_template/loaders.py` & `leanit-mweb-23.7.3/mweb/jinja_template/loaders.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/manage.py` & `leanit-mweb-23.7.3/mweb/manage.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/orm/fields/__init__.py` & `leanit-mweb-23.7.3/mweb/orm/fields/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,21 +61,21 @@
         self.min_length = min_length
         self.max_length = max_length
         self.alphabet = alphabet
         self.choices = choices
 
     def validate(self, value):
         if self.min_length is not None and len(value) < self.min_length:
-            raise ValidationFailedException(f"String is too short: '{value}'")
+            raise ValidationFailedException(f"String is too short: '{value}' (min: {self.min_length})")
         if self.max_length is not None and len(value) > self.max_length:
-            raise ValidationFailedException(f"String is too long: '{value}'")
+            raise ValidationFailedException(f"String is too long: '{value}' (max: {self.max_length})")
         if self.alphabet is not None and not set(value).issubset(set(self.alphabet)):
-            raise ValidationFailedException(f"String contains invalid characters: '{value}'")
+            raise ValidationFailedException(f"String contains invalid characters: '{value}' (alphabet: {self.alphabet})")
         if self.choices is not None and value not in self.choices:
-            raise ValidationFailedException(f"String is not in choices: '{value}'")
+            raise ValidationFailedException(f"String '{value}' of field is not in choices: {','.join(self.choices)}")
         return super().validate(value)
 
 
 class EmailField(StringField):
     pattern = re.compile(r'^[\w\.-]+@[\w\.-]+\.\w+$')
 
     def validate(self, value):
```

### Comparing `leanit-mweb-23.7.2/mweb/orm/model.py` & `leanit-mweb-23.7.3/mweb/orm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,21 +89,22 @@
         return new
 
     @classmethod
     def create(cls, **kwargs) -> "cls":
         insert_doc = {}
 
         for field_name, field_instance in cls.fields.items():
-            if value := kwargs.get(field_name):
-                insert_doc[field_name] = field_instance.to_db(value)
+            if py_value := kwargs.get(field_name):
+                insert_doc[field_name] = field_instance.to_db(py_value)
             else:
-                value = field_instance.get_default()
-                if value is not None:
-                    insert_doc[field_name] = value
-                    # logger.debug(f"field_name: {field_name}, value: {value}")
+                py_value = field_instance.get_default()
+                if py_value is not None:
+                    insert_doc[field_name] = field_instance.to_db(py_value)
+
+            field_instance.validate(py_value)
 
         instance = cls(**insert_doc)
 
         sql = f"INSERT INTO \"{cls._table}\" ({','.join(insert_doc.keys())}) VALUES ({','.join(['%s'] * len(insert_doc))})"
         # logger.debug(f"SQL: {sql}")
 
         instance.on_pre_create()
@@ -416,15 +417,17 @@
         await asyncio.get_event_loop().run_in_executor(self._db, self.save, tracing_context)
 
     def _get_update_query_and_values(self, update_doc: Dict):
         set_values = []
         set_args = []
         for key, value in update_doc.items():
             set_values.append(f"{key}=%s")
-            set_args.append(value)
+            field = self.fields[key]
+            field.validate(value)
+            set_args.append(field.to_db(value))
         set_values = ",".join(set_values)
 
         where_values = []
         where_args = []
         for key in self._pk:
             where_values.append(f"{key}=%s")
             where_args.append(getattr(self, key))
```

### Comparing `leanit-mweb-23.7.2/mweb/orm/password.py` & `leanit-mweb-23.7.3/mweb/orm/password.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/security/__init__.py` & `leanit-mweb-23.7.3/mweb/security/__init__.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/security/jwt.py` & `leanit-mweb-23.7.3/mweb/security/jwt.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/staticfiles.py` & `leanit-mweb-23.7.3/mweb/staticfiles.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/testutils.py` & `leanit-mweb-23.7.3/mweb/testutils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import logging
 import re
 
 from httpx import Response
-from starlette.testclient import TestClient
+from starlette.testclient import TestClient as StarlettTestClient
+
 
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     pass
@@ -75,7 +76,28 @@
 
         if self.method == 'post':
             return client.post(self.action, data=self.data, **kwargs)
         elif self.method == 'get':
             return client.get(self.action, params=self.data, **kwargs)
         else:
             raise ValueError(f"Unknown method: {self.method}")
+
+
+class TestClient(StarlettTestClient):
+
+    def _fix_redirect_kwargs(self, kwargs):
+        if "allow_redirects" in kwargs:
+            kwargs["follow_redirects"] = kwargs["allow_redirects"]
+            del kwargs["allow_redirects"]
+        elif "follow_redirects" in kwargs:
+            pass
+        else:
+            kwargs["follow_redirects"] = False
+
+    def get(self, *args, **kwargs):
+        self._fix_redirect_kwargs(kwargs)
+        return super().get(*args, **kwargs)
+
+    def post(self, *args, **kwargs):
+        self._fix_redirect_kwargs(kwargs)
+        return super().post(*args, **kwargs)
+
```

### Comparing `leanit-mweb-23.7.2/mweb/thread.py` & `leanit-mweb-23.7.3/mweb/thread.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/utils/__init__.py` & `leanit-mweb-23.7.3/mweb/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
+
 import logging
+
 from starlette.requests import Request
+
 logger = logging.getLogger(__name__)
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     pass
 
@@ -78,7 +81,8 @@
     :type delimiter: str
     :return: A tuple of pairs, where each pair contains two elements from the input list.
     :rtype: tuple
     """
     split_data = data.split(delimiter)
     result = tuple((split_data[i], split_data[i+1]) for i in range(0, len(split_data), 2))
     return result
+
```

### Comparing `leanit-mweb-23.7.2/mweb/utils/id/snowflakeid.py` & `leanit-mweb-23.7.3/mweb/utils/id/snowflakeid.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/utils/log_catcher.py` & `leanit-mweb-23.7.3/mweb/utils/log_catcher.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/views/auth.py` & `leanit-mweb-23.7.3/mweb/views/auth.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/views/model.py` & `leanit-mweb-23.7.3/mweb/views/model.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/mweb/yuga.py` & `leanit-mweb-23.7.3/mweb/yuga.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/setup.py` & `leanit-mweb-23.7.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '23.7.2'
+VERSION = '23.7.3'
 DESCRIPTION = 'Web framework'
 LONG_DESCRIPTION = 'Web framework'
 
 # Setting up
 setup(
     name="leanit-mweb",
     version=VERSION,
```

### Comparing `leanit-mweb-23.7.2/tests/auth/sso/microsoft/test_auth_callback.py` & `leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_auth_callback.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/auth/sso/microsoft/test_build_auth_url.py` & `leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_build_auth_url.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/auth/sso/microsoft/test_code.py` & `leanit-mweb-23.7.3/tests/auth/sso/microsoft/test_code.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/orm/fields/test_StringField.py` & `leanit-mweb-23.7.3/tests/orm/fields/test_StringField.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,10 +16,14 @@
             field.validate("abcd")
 
     def test_alphabet(self):
         field = StringField(alphabet="abc")
         with self.assertRaises(ValidationFailedException):
             field.validate("def")
 
+    def test_choices(self):
+        field = StringField(choices=["a", "b"])
+        with self.assertRaises(ValidationFailedException):
+            field.validate("c")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `leanit-mweb-23.7.2/tests/orm/model/test_delete_all.py` & `leanit-mweb-23.7.3/tests/orm/model/test_delete_all.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/security/test_jwt.py` & `leanit-mweb-23.7.3/tests/security/test_jwt.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/security/test_sign.py` & `leanit-mweb-23.7.3/tests/security/test_sign.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/utils/test_form.py` & `leanit-mweb-23.7.3/tests/utils/test_form.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/utils/test_snowflake.py` & `leanit-mweb-23.7.3/tests/utils/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.7.2/tests/views/model/test_paging.py` & `leanit-mweb-23.7.3/tests/views/model/test_paging.py`

 * *Files identical despite different names*

