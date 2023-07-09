# Comparing `tmp/utilspkg-0.3.1.tar.gz` & `tmp/utilspkg-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilspkg-0.3.1.tar", last modified: Mon Jun 26 21:53:49 2023, max compression
+gzip compressed data, was "utilspkg-0.3.2.tar", last modified: Sun Jul  9 23:44:50 2023, max compression
```

## Comparing `utilspkg-0.3.1.tar` & `utilspkg-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-06-26 21:53:49.038733 utilspkg-0.3.1/
--rw-r--r--   0 croft      (501) staff       (20)      198 2023-06-26 21:53:49.038622 utilspkg-0.3.1/PKG-INFO
--rw-r--r--   0 croft      (501) staff       (20)       86 2023-06-26 21:37:37.000000 utilspkg-0.3.1/pyproject.toml
--rw-r--r--   0 croft      (501) staff       (20)       38 2023-06-26 21:53:49.038775 utilspkg-0.3.1/setup.cfg
--rw-r--r--   0 croft      (501) staff       (20)      422 2023-06-26 21:38:08.000000 utilspkg-0.3.1/setup.py
-drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-06-26 21:53:49.037846 utilspkg-0.3.1/utilspkg/
--rw-r--r--   0 croft      (501) staff       (20)     1053 2023-06-26 19:52:42.000000 utilspkg-0.3.1/utilspkg/__init__.py
--rw-r--r--   0 croft      (501) staff       (20)     3460 2023-06-26 19:52:59.000000 utilspkg-0.3.1/utilspkg/utils_db.py
--rw-r--r--   0 croft      (501) staff       (20)     2206 2023-06-26 19:53:12.000000 utilspkg-0.3.1/utilspkg/utils_email.py
--rw-r--r--   0 croft      (501) staff       (20)     3375 2023-06-26 19:53:16.000000 utilspkg-0.3.1/utilspkg/utils_gpt.py
--rw-r--r--   0 croft      (501) staff       (20)     1540 2023-06-26 01:09:40.000000 utilspkg-0.3.1/utilspkg/utils_init.py
--rw-r--r--   0 croft      (501) staff       (20)      764 2023-06-26 01:09:40.000000 utilspkg-0.3.1/utilspkg/utils_misc.py
--rw-r--r--   0 croft      (501) staff       (20)     6789 2023-06-26 19:09:39.000000 utilspkg-0.3.1/utilspkg/utils_slack.py
--rw-r--r--   0 croft      (501) staff       (20)     3353 2023-06-26 01:09:40.000000 utilspkg-0.3.1/utilspkg/utils_time.py
-drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-06-26 21:53:49.038395 utilspkg-0.3.1/utilspkg.egg-info/
--rw-r--r--   0 croft      (501) staff       (20)      198 2023-06-26 21:53:49.000000 utilspkg-0.3.1/utilspkg.egg-info/PKG-INFO
--rw-r--r--   0 croft      (501) staff       (20)      332 2023-06-26 21:53:49.000000 utilspkg-0.3.1/utilspkg.egg-info/SOURCES.txt
--rw-r--r--   0 croft      (501) staff       (20)        1 2023-06-26 21:53:49.000000 utilspkg-0.3.1/utilspkg.egg-info/dependency_links.txt
--rw-r--r--   0 croft      (501) staff       (20)        9 2023-06-26 21:53:49.000000 utilspkg-0.3.1/utilspkg.egg-info/top_level.txt
+drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-09 23:44:50.839333 utilspkg-0.3.2/
+-rw-r--r--   0 croft      (501) staff       (20)      198 2023-07-09 23:44:50.839228 utilspkg-0.3.2/PKG-INFO
+-rw-r--r--   0 croft      (501) staff       (20)       86 2023-06-26 21:37:37.000000 utilspkg-0.3.2/pyproject.toml
+-rw-r--r--   0 croft      (501) staff       (20)       38 2023-07-09 23:44:50.839372 utilspkg-0.3.2/setup.cfg
+-rw-r--r--   0 croft      (501) staff       (20)      422 2023-07-02 14:31:40.000000 utilspkg-0.3.2/setup.py
+drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-09 23:44:50.838618 utilspkg-0.3.2/utilspkg/
+-rw-r--r--   0 croft      (501) staff       (20)     1053 2023-06-26 19:52:42.000000 utilspkg-0.3.2/utilspkg/__init__.py
+-rw-r--r--   0 croft      (501) staff       (20)     3460 2023-06-26 19:52:59.000000 utilspkg-0.3.2/utilspkg/utils_db.py
+-rw-r--r--   0 croft      (501) staff       (20)     2206 2023-06-26 19:53:12.000000 utilspkg-0.3.2/utilspkg/utils_email.py
+-rw-r--r--   0 croft      (501) staff       (20)     3375 2023-06-26 19:53:16.000000 utilspkg-0.3.2/utilspkg/utils_gpt.py
+-rw-r--r--   0 croft      (501) staff       (20)     1661 2023-07-02 00:32:38.000000 utilspkg-0.3.2/utilspkg/utils_init.py
+-rw-r--r--   0 croft      (501) staff       (20)      764 2023-06-26 01:09:40.000000 utilspkg-0.3.2/utilspkg/utils_misc.py
+-rw-r--r--   0 croft      (501) staff       (20)     6775 2023-07-02 00:46:04.000000 utilspkg-0.3.2/utilspkg/utils_slack.py
+-rw-r--r--   0 croft      (501) staff       (20)     3353 2023-06-26 01:09:40.000000 utilspkg-0.3.2/utilspkg/utils_time.py
+-rw-r--r--   0 croft      (501) staff       (20)     2947 2023-07-09 23:40:36.000000 utilspkg-0.3.2/utilspkg/utils_times.py
+drwxr-xr-x   0 croft      (501) staff       (20)        0 2023-07-09 23:44:50.839051 utilspkg-0.3.2/utilspkg.egg-info/
+-rw-r--r--   0 croft      (501) staff       (20)      198 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/PKG-INFO
+-rw-r--r--   0 croft      (501) staff       (20)      356 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 croft      (501) staff       (20)        1 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 croft      (501) staff       (20)        9 2023-07-09 23:44:50.000000 utilspkg-0.3.2/utilspkg.egg-info/top_level.txt
```

### Comparing `utilspkg-0.3.1/utilspkg/__init__.py` & `utilspkg-0.3.2/utilspkg/__init__.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.1/utilspkg/utils_db.py` & `utilspkg-0.3.2/utilspkg/utils_db.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.1/utilspkg/utils_email.py` & `utilspkg-0.3.2/utilspkg/utils_email.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.1/utilspkg/utils_gpt.py` & `utilspkg-0.3.2/utilspkg/utils_gpt.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.1/utilspkg/utils_misc.py` & `utilspkg-0.3.2/utilspkg/utils_misc.py`

 * *Files identical despite different names*

### Comparing `utilspkg-0.3.1/utilspkg/utils_slack.py` & `utilspkg-0.3.2/utilspkg/utils_slack.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 utils_init.load_env_variables_from_yaml('/Users/croft/VScode/ptagit/env_vars.yaml')
 
 logger = utils_init.setup_logger(__name__)
 
 SLACK_API_KEY = os.environ["SLACK_ACCESS_TOKEN_TEAM"]
 TESTING_DM = os.environ["TESTING_DM"]
 TESTING_CHANNEL = os.environ["TESTING_CHANNEL"] # not currently used since all goes to the DM's "channel"
-tester = 'hi'
 
 class SlackConnect:
     """
     A utility class for sending messages and fetching conversation history from Slack.
     """
 
     def __init__(self, api_key=SLACK_API_KEY, testing_flag=False, logger=None):
```

### Comparing `utilspkg-0.3.1/utilspkg/utils_time.py` & `utilspkg-0.3.2/utilspkg/utils_time.py`

 * *Files identical despite different names*

