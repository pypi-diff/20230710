# Comparing `tmp/uagents_whatsapp_utility-4.5.tar.gz` & `tmp/uagents_whatsapp_utility-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_whatsapp_utility-4.5.tar", max compression
+gzip compressed data, was "uagents_whatsapp_utility-5.0.tar", max compression
```

## Comparing `uagents_whatsapp_utility-4.5.tar` & `uagents_whatsapp_utility-5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-07-10 12:41:27.730198 uagents_whatsapp_utility-4.5/LICENSE
--rw-r--r--   0        0        0      871 2023-07-10 12:41:27.730198 uagents_whatsapp_utility-4.5/README.md
--rw-r--r--   0        0        0        0 2023-07-10 12:41:27.730198 uagents_whatsapp_utility-4.5/protocols/__init__.py
--rw-r--r--   0        0        0       78 2023-07-10 12:41:27.730198 uagents_whatsapp_utility-4.5/protocols/awesome_module.py
--rw-r--r--   0        0        0      402 2023-07-10 12:41:47.613954 uagents_whatsapp_utility-4.5/pyproject.toml
--rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 uagents_whatsapp_utility-4.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-10 12:56:47.998508 uagents_whatsapp_utility-5.0/LICENSE
+-rw-r--r--   0        0        0      663 2023-07-10 12:56:47.998508 uagents_whatsapp_utility-5.0/README.rst
+-rw-r--r--   0        0        0        0 2023-07-10 12:56:47.998508 uagents_whatsapp_utility-5.0/protocols/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-10 12:56:47.998508 uagents_whatsapp_utility-5.0/protocols/awesome_module.py
+-rw-r--r--   0        0        0      403 2023-07-10 12:57:04.594628 uagents_whatsapp_utility-5.0/pyproject.toml
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 uagents_whatsapp_utility-5.0/PKG-INFO
```

### Comparing `uagents_whatsapp_utility-4.5/LICENSE` & `uagents_whatsapp_utility-5.0/LICENSE`

 * *Files identical despite different names*

