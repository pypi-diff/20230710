# Comparing `tmp/messagingclient-0.1.2.tar.gz` & `tmp/messagingclient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/workspaces/messaging-client/dist/tmpltqmq5oy/messagingclient-0.1.2.tar", last modified: Mon Nov  8 22:05:11 2021, max compression
+gzip compressed data, was "/workspaces/messaging-client/dist/.tmp-h79r9l15/messagingclient-0.1.3.tar", last modified: Mon Jul 10 17:11:38 2023, max compression
```

## Comparing `messagingclient-0.1.2.tar` & `messagingclient-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-08 22:05:11.000000 messagingclient-0.1.2/
--rw-rw-r--   0 root         (0) root         (0)    35149 2021-08-20 22:20:26.000000 messagingclient-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2021-11-08 22:05:11.000000 messagingclient-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       18 2021-08-20 22:20:26.000000 messagingclient-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient/
--rw-r--r--   0 root         (0) root         (0)       59 2021-11-08 22:03:52.000000 messagingclient-0.1.2/messagingclient/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1601 2021-11-08 21:57:59.000000 messagingclient-0.1.2/messagingclient/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)      533 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-11-08 22:05:11.000000 messagingclient-0.1.2/messagingclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      666 2021-11-08 22:05:11.000000 messagingclient-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2021-10-14 13:54:53.000000 messagingclient-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:11:38.000000 messagingclient-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)    35149 2021-08-20 22:20:26.000000 messagingclient-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-10 17:11:38.000000 messagingclient-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2021-08-20 22:20:26.000000 messagingclient-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-10 17:10:59.000000 messagingclient-0.1.3/messagingclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-07-10 17:11:17.000000 messagingclient-0.1.3/messagingclient/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      497 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-10 17:11:38.000000 messagingclient-0.1.3/messagingclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-10 17:11:38.000000 messagingclient-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2021-10-14 13:54:52.000000 messagingclient-0.1.3/setup.py
```

### Comparing `messagingclient-0.1.2/LICENSE` & `messagingclient-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `messagingclient-0.1.2/messagingclient/client.py` & `messagingclient-0.1.3/messagingclient/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,11 +40,11 @@
         subscription_name = f"projects/{PROJECT_NAME}/subscriptions/{queue}"
         with pubsub_v1.SubscriberClient() as subscriber:
             future = subscriber.subscribe(
                 subscription_name, callback_wrapper, flow_control=flow_control
             )
             try:
                 future.result()
-            except Exception:
+            except Exception as exc:
                 # terminate on any exception so that the worker isn't hung.
                 future.cancel()
-                print("stopped listening")
+                print(f"stopped listening: {exc}")
```

### Comparing `messagingclient-0.1.2/setup.cfg` & `messagingclient-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2
+current_version = 0.1.3
 
 [metadata]
 name = messagingclient
 version = 0.1.0
 author = Akhilesh Halageri
 description = Messaging client
 long_description = file: README.md
```

### Comparing `messagingclient-0.1.2/setup.py` & `messagingclient-0.1.3/setup.py`

 * *Files identical despite different names*

