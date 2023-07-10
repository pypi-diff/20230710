# Comparing `tmp/mail_satvadev-1.0.3.tar.gz` & `tmp/mail_satvadev-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail_satvadev-1.0.3.tar", max compression
+gzip compressed data, was "mail_satvadev-1.0.4.tar", max compression
```

## Comparing `mail_satvadev-1.0.3.tar` & `mail_satvadev-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1052 2023-07-03 07:33:14.103926 mail_satvadev-1.0.3/LICENSE
--rw-r--r--   0        0        0     5498 2023-07-03 07:53:58.087565 mail_satvadev-1.0.3/README.md
--rw-r--r--   0        0        0      710 2023-07-10 09:43:48.295395 mail_satvadev-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 07:33:14.103926 mail_satvadev-1.0.3/src/mail_satvadev/__init__.py
--rw-r--r--   0        0        0      148 2023-07-07 08:54:38.066354 mail_satvadev-1.0.3/src/mail_satvadev/apps.py
--rw-r--r--   0        0        0      935 2023-07-03 07:33:14.103926 mail_satvadev-1.0.3/src/mail_satvadev/filters.py
--rw-r--r--   0        0        0     2011 2023-07-07 12:39:54.100787 mail_satvadev-1.0.3/src/mail_satvadev/messages.py
--rw-r--r--   0        0        0      859 2023-07-03 10:21:44.739667 mail_satvadev-1.0.3/src/mail_satvadev/tasks.py
--rw-r--r--   0        0        0     6331 1970-01-01 00:00:00.000000 mail_satvadev-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-03 07:33:14.103926 mail_satvadev-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5498 2023-07-10 09:48:13.141367 mail_satvadev-1.0.4/README.md
+-rw-r--r--   0        0        0      710 2023-07-10 10:22:58.198360 mail_satvadev-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 07:33:14.103926 mail_satvadev-1.0.4/src/mail_satvadev/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-10 09:48:13.141367 mail_satvadev-1.0.4/src/mail_satvadev/apps.py
+-rw-r--r--   0        0        0      935 2023-07-03 07:33:14.103926 mail_satvadev-1.0.4/src/mail_satvadev/filters.py
+-rw-r--r--   0        0        0     2011 2023-07-10 09:48:13.145367 mail_satvadev-1.0.4/src/mail_satvadev/messages.py
+-rw-r--r--   0        0        0      859 2023-07-10 09:48:13.145367 mail_satvadev-1.0.4/src/mail_satvadev/tasks.py
+-rw-r--r--   0        0        0     6331 1970-01-01 00:00:00.000000 mail_satvadev-1.0.4/PKG-INFO
```

### Comparing `mail_satvadev-1.0.3/LICENSE` & `mail_satvadev-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.3/README.md` & `mail_satvadev-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.3/src/mail_satvadev/filters.py` & `mail_satvadev-1.0.4/src/mail_satvadev/filters.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.3/src/mail_satvadev/messages.py` & `mail_satvadev-1.0.4/src/mail_satvadev/messages.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.3/src/mail_satvadev/tasks.py` & `mail_satvadev-1.0.4/src/mail_satvadev/tasks.py`

 * *Files identical despite different names*

### Comparing `mail_satvadev-1.0.3/PKG-INFO` & `mail_satvadev-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mail-satvadev
-Version: 1.0.3
+Version: 1.0.4
 Summary: Template for email
 Author: satva.dev
 Author-email: info@satva.dev
 Requires-Python: >=3.9.10,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

