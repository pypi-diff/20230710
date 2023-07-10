# Comparing `tmp/whoisit-2.7.0.tar.gz` & `tmp/whoisit-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoisit-2.7.0.tar", last modified: Sat Jun  3 11:00:02 2023, max compression
+gzip compressed data, was "whoisit-2.7.1.tar", last modified: Mon Jul 10 18:18:16 2023, max compression
```

## Comparing `whoisit-2.7.0.tar` & `whoisit-2.7.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.0/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.0/MANIFEST.in
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-06-03 11:00:02.365261 whoisit-2.7.0/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.7.0/README.md
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.0/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2023-06-03 11:00:02.365261 whoisit-2.7.0/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2023-06-03 10:59:42.000000 whoisit-2.7.0/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.0/tests/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.0/tests/test_bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.0/tests/test_parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.0/tests/test_query.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.0/tests/test_ssl.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/whoisit/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     2359 2023-06-03 08:55:13.000000 whoisit-2.7.0/whoisit/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.0/whoisit/bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.0/whoisit/errors.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.0/whoisit/logger.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      949 2022-12-06 10:28:45.000000 whoisit-2.7.0/whoisit/overrides.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    15838 2022-12-06 10:28:45.000000 whoisit-2.7.0/whoisit/parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.0/whoisit/query.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3830 2023-06-03 08:54:56.000000 whoisit-2.7.0/whoisit/utils.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2023-06-03 10:59:35.000000 whoisit-2.7.0/whoisit/version.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-06-03 11:00:02.365261 whoisit-2.7.0/whoisit.egg-info/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2023-06-03 11:00:02.000000 whoisit-2.7.0/whoisit.egg-info/top_level.txt
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-07-10 18:18:16.365685 whoisit-2.7.1/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.1/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.1/MANIFEST.in
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-07-10 18:18:16.369685 whoisit-2.7.1/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.7.1/README.md
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.1/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2023-07-10 18:18:16.369685 whoisit-2.7.1/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2023-07-10 18:17:48.000000 whoisit-2.7.1/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-07-10 18:18:16.365685 whoisit-2.7.1/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.1/tests/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.1/tests/test_bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.1/tests/test_parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.1/tests/test_query.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.1/tests/test_ssl.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-07-10 18:18:16.365685 whoisit-2.7.1/whoisit/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2359 2023-06-03 08:55:13.000000 whoisit-2.7.1/whoisit/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.1/whoisit/bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.1/whoisit/errors.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.1/whoisit/logger.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      949 2022-12-06 10:28:45.000000 whoisit-2.7.1/whoisit/overrides.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    15838 2022-12-06 10:28:45.000000 whoisit-2.7.1/whoisit/parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.1/whoisit/query.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3940 2023-07-10 18:02:01.000000 whoisit-2.7.1/whoisit/utils.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2023-07-10 18:17:58.000000 whoisit-2.7.1/whoisit/version.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2023-07-10 18:18:16.365685 whoisit-2.7.1/whoisit.egg-info/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21653 2023-07-10 18:18:16.000000 whoisit-2.7.1/whoisit.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2023-07-10 18:18:16.000000 whoisit-2.7.1/whoisit.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2023-07-10 18:18:16.000000 whoisit-2.7.1/whoisit.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2023-07-10 18:18:16.000000 whoisit-2.7.1/whoisit.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2023-07-10 18:18:16.000000 whoisit-2.7.1/whoisit.egg-info/top_level.txt
```

### Comparing `whoisit-2.7.0/LICENSE` & `whoisit-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/PKG-INFO` & `whoisit-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Platform: UNKNOWN
```

### Comparing `whoisit-2.7.0/README.md` & `whoisit-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/setup.py` & `whoisit-2.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '2.7.0'
+version = '2.7.1'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `whoisit-2.7.0/tests/test_bootstrap.py` & `whoisit-2.7.1/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/tests/test_parser.py` & `whoisit-2.7.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/tests/test_query.py` & `whoisit-2.7.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/tests/test_ssl.py` & `whoisit-2.7.1/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/__init__.py` & `whoisit-2.7.1/whoisit/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/bootstrap.py` & `whoisit-2.7.1/whoisit/bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/errors.py` & `whoisit-2.7.1/whoisit/errors.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/logger.py` & `whoisit-2.7.1/whoisit/logger.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/overrides.py` & `whoisit-2.7.1/whoisit/overrides.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/parser.py` & `whoisit-2.7.1/whoisit/parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/query.py` & `whoisit-2.7.1/whoisit/query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.0/whoisit/utils.py` & `whoisit-2.7.1/whoisit/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import os
-from urllib3.util import retry, create_urllib3_context
+from urllib3.util import retry
+try:
+    from urllib3.util import create_urllib3_context
+except ImportError:
+    from urllib3.util.ssl_ import create_urllib3_context
 from urllib3.poolmanager import PoolManager
 import requests
 from .errors import QueryError, UnsupportedError
 from .logger import get_logger
 from .version import version
```

### Comparing `whoisit-2.7.0/whoisit.egg-info/PKG-INFO` & `whoisit-2.7.1/whoisit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Platform: UNKNOWN
```

