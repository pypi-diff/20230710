# Comparing `tmp/antigranular-0.0.tar.gz` & `tmp/antigranular-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular-0.0.tar", max compression
+gzip compressed data, was "antigranular-0.1.0.tar", max compression
```

## Comparing `antigranular-0.0.tar` & `antigranular-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0      529 2023-05-09 16:15:43.817098 antigranular-0.0/README.md
--rw-r--r--   0        0        0      270 2023-05-09 15:30:43.876489 antigranular-0.0/antigranular/__init__.py
--rw-r--r--   0        0        0      408 2023-05-09 16:58:56.886937 antigranular-0.0/pyproject.toml
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 antigranular-0.0/setup.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 antigranular-0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 07:47:40.286437 antigranular-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4188 2023-07-10 07:47:40.286437 antigranular-0.1.0/README.md
+-rw-r--r--   0        0        0      522 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/__init__.py
+-rw-r--r--   0        0        0    10806 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/client.py
+-rw-r--r--   0        0        0      882 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/config/config.py
+-rw-r--r--   0        0        0     2933 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/enclave_client/mock_client.py
+-rw-r--r--   0        0        0      753 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/enclave_client/oblv_client.py
+-rw-r--r--   0        0        0     1019 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/magics/errors.py
+-rw-r--r--   0        0        0     6474 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/magics/magics.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/models/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/models/models.py
+-rw-r--r--   0        0        0      140 2023-07-10 07:47:40.286437 antigranular-0.1.0/antigranular/utils/error_print.py
+-rw-r--r--   0        0        0      736 2023-07-10 07:47:40.286437 antigranular-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 antigranular-0.1.0/setup.py
+-rw-r--r--   0        0        0     5103 1970-01-01 00:00:00.000000 antigranular-0.1.0/PKG-INFO
```

