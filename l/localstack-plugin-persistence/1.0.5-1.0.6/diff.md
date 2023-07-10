# Comparing `tmp/localstack-plugin-persistence-1.0.5.tar.gz` & `tmp/localstack-plugin-persistence-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-plugin-persistence-1.0.5.tar", last modified: Tue May 30 16:04:14 2023, max compression
+gzip compressed data, was "localstack-plugin-persistence-1.0.6.tar", last modified: Mon Jul 10 08:00:31 2023, max compression
```

## Comparing `localstack-plugin-persistence-1.0.5.tar` & `localstack-plugin-persistence-1.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.950637 localstack-plugin-persistence-1.0.5/
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-30 16:04:14.950722 localstack-plugin-persistence-1.0.5/PKG-INFO
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.945603 localstack-plugin-persistence-1.0.5/localstack_persistence/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      175 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/constants.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.945869 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      370 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/__plugins__.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.946446 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/
--rw-r--r--   0 giograno   (501) staff       (20)      533 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      259 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/botocore.py
--rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/cryptography.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.946704 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/services/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/services/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      391 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/services/acm.py
--rw-r--r--   0 giograno   (501) staff       (20)     1708 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/stdlib.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.947553 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1824 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     3151 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/load.py
--rw-r--r--   0 giograno   (501) staff       (20)     2045 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/manager.py
--rw-r--r--   0 giograno   (501) staff       (20)     1628 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/pods/save.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.948120 localstack-plugin-persistence-1.0.5/localstack_persistence/reset/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/reset/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      336 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/reset/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)      765 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/reset/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     2474 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/reset/reset.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.949280 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)     3405 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/api.py
--rw-r--r--   0 giograno   (501) staff       (20)      579 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     1633 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/load.py
--rw-r--r--   0 giograno   (501) staff       (20)     6970 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/manager.py
--rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/save.py
--rw-r--r--   0 giograno   (501) staff       (20)      584 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_persistence/utils.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 16:04:14.950503 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/PKG-INFO
--rw-r--r--   0 giograno   (501) staff       (20)     1679 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 giograno   (501) staff       (20)      925 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/entry_points.txt
--rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/not-zip-safe
--rw-r--r--   0 giograno   (501) staff       (20)      940 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/plux.json
--rw-r--r--   0 giograno   (501) staff       (20)      277 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/requires.txt
--rw-r--r--   0 giograno   (501) staff       (20)       23 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/top_level.txt
--rw-r--r--   0 giograno   (501) staff       (20)      571 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/pyproject.toml
--rw-r--r--   0 giograno   (501) staff       (20)      843 2023-05-30 16:04:14.951039 localstack-plugin-persistence-1.0.5/setup.cfg
--rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-05-30 16:04:14.000000 localstack-plugin-persistence-1.0.5/setup.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.357380 localstack-plugin-persistence-1.0.6/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-07-10 08:00:31.357443 localstack-plugin-persistence-1.0.6/PKG-INFO
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.353149 localstack-plugin-persistence-1.0.6/localstack_persistence/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      175 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/constants.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.353379 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      370 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/__plugins__.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.353892 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/
+-rw-r--r--   0 giograno   (501) staff       (20)      533 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      259 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/botocore.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/cryptography.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.354128 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/services/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/services/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      391 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/services/acm.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1708 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/stdlib.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.354857 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1824 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3151 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2045 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1628 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/pods/save.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.355357 localstack-plugin-persistence-1.0.6/localstack_persistence/reset/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/reset/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      336 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/reset/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      765 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/reset/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2474 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/reset/reset.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.356228 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3480 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/api.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1869 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1633 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     7045 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/save.py
+-rw-r--r--   0 giograno   (501) staff       (20)      584 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_persistence/utils.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-07-10 08:00:31.357266 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 giograno   (501) staff       (20)     1679 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      925 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-07-10 08:00:30.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/not-zip-safe
+-rw-r--r--   0 giograno   (501) staff       (20)      940 2023-07-10 08:00:30.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/plux.json
+-rw-r--r--   0 giograno   (501) staff       (20)      277 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/requires.txt
+-rw-r--r--   0 giograno   (501) staff       (20)       23 2023-07-10 08:00:31.000000 localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/top_level.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      571 2023-07-10 08:00:30.000000 localstack-plugin-persistence-1.0.6/pyproject.toml
+-rw-r--r--   0 giograno   (501) staff       (20)      843 2023-07-10 08:00:31.357750 localstack-plugin-persistence-1.0.6/setup.cfg
+-rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-07-10 08:00:30.000000 localstack-plugin-persistence-1.0.6/setup.py
```

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/__init__.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/cryptography.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/cryptography.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pickling/reducers/stdlib.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pickling/reducers/stdlib.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pods/endpoints.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pods/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pods/load.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pods/load.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pods/manager.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pods/manager.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/pods/save.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/pods/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/reset/endpoints.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/reset/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/reset/reset.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/reset/reset.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/__plugins__.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/__plugins__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging,os
 from localstack import config
 from localstack.aws.handlers import serve_custom_service_request_handlers
+from localstack.config import SNAPSHOT_FLUSH_INTERVAL
 from localstack.runtime import hooks,shutdown
 from localstack.utils.objects import singleton_factory
 from.api import LoadStrategy,SaveStrategy
 LOG=logging.getLogger(__name__)
 DEFAULT_SAVE_STRATEGY=SaveStrategy.SCHEDULED
 def is_persistence_activated():return config.PERSISTENCE and'LOCALSTACK_API_KEY'in os.environ
 @singleton_factory
@@ -37,10 +38,10 @@
 	if A==LoadStrategy.ON_STARTUP:LOG.info('restoring state of all services');get_service_state_manager().load_all()
 @hooks.on_infra_start(should_load=is_persistence_activated())
 def register_state_save_strategy():
 	from localstack.aws.handlers import run_custom_response_handlers as C,serve_custom_service_request_handlers as D;from.api import SaveStrategy as A;from.manager import SaveOnRequestHandler as H,SaveStateScheduler as I;E=get_save_strategy();F=get_service_state_manager()
 	match E:
 		case A.ON_SHUTDOWN:LOG.info('registering ON_SHUTDOWN save strategy');shutdown.SHUTDOWN_HANDLERS.register(F.save_all)
 		case A.ON_REQUEST:LOG.info('registering ON_REQUEST save strategy');G=H(get_service_state_manager());D.append(G.on_request);C.append(G.on_response)
-		case A.SCHEDULED:LOG.info('registering SCHEDULED save strategy');B=I(F,period=15);shutdown.SHUTDOWN_HANDLERS.register(B.close);D.append(B.on_request);C.append(B.on_response);B.start()
+		case A.SCHEDULED:LOG.info('registering SCHEDULED save strategy');B=I(F,period=SNAPSHOT_FLUSH_INTERVAL);shutdown.SHUTDOWN_HANDLERS.register(B.close);D.append(B.on_request);C.append(B.on_response);B.start()
 		case A.MANUAL:LOG.info('registering MANUAL save strategy (call /_localstack/state endpoints to save state)')
 		case _:LOG.warning('Unknown save strategy %s',E)
```

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/api.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/api.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/load.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/load.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/manager.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 _B=True
 _A=False
 import logging,os.path,threading,time
 from typing import Dict,Set
 from localstack.aws.api import RequestContext
+from localstack.config import SNAPSHOT_FLUSH_INTERVAL
 from localstack.services.plugins import ServiceManager
 from localstack.state import StateVisitor
 from localstack.state.snapshot import SnapshotPersistencePlugin
 from localstack.utils.functions import call_safe
 from localstack.utils.json import FileMappedDocument
 from localstack.utils.scheduler import Scheduler
 from localstack.utils.sync import SynchronizedDefaultDict
@@ -89,15 +90,15 @@
 		B=context
 		if not _should_save_request(B):return
 		C=B.service.service_name;D=A._locks[C]
 		try:A.state_manager.save(C)
 		finally:D.release()
 class SaveStateScheduler:
 	'\n    Saves the state on a regular basis, and facilitates the "SCHEDULED" save strategy (a compromise between\n    ON_REQUEST and ON_SHUTDOWN).\n\n    It also exposes a Handler that should be added to the handler chain, which schedules services similar\n    to the SaveOnRequestHandler.\n    ';state_manager:0;period:0
-	def __init__(A,state_manager,period=30):A.state_manager=state_manager;A.scheduler=Scheduler();A.period=period;A._dirty_markers=set();A._marker_lock=threading.Lock();A._save_lock=rwlock.RWLockWrite()
+	def __init__(A,state_manager,period=SNAPSHOT_FLUSH_INTERVAL):A.state_manager=state_manager;A.scheduler=Scheduler();A.period=period;A._dirty_markers=set();A._marker_lock=threading.Lock();A._save_lock=rwlock.RWLockWrite()
 	def start(A):threading.Thread(target=A.scheduler.run,daemon=_B).start();A.scheduler.schedule(A._do_save,period=A.period)
 	def schedule_for_save(A,service):
 		'\n        Schedule the given service into the next save cycle. Call this when you think the state of a\n        service may have changed and should be flushed to disk.\n\n        :param service: the service to be stored\n        '
 		with A._marker_lock:A._dirty_markers.add(service)
 	def _do_save(A):
 		'\n        Internal routine to perform save calls through the StateManager.\n        ';C=time.perf_counter()
 		with A._marker_lock:
```

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/snapshot/save.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/snapshot/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_persistence/utils.py` & `localstack-plugin-persistence-1.0.6/localstack_persistence/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/SOURCES.txt` & `localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/entry_points.txt` & `localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/localstack_plugin_persistence.egg-info/plux.json` & `localstack-plugin-persistence-1.0.6/localstack_plugin_persistence.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(0, '*

 * *                                      "'register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints'), "*

 * *                                      '(1, '*

 * *                                      "'register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource')], "*

 * *                                      'delete: [5, 3]}'}*

```diff
@@ -1,16 +1,16 @@
 {
     "localstack.hooks.on_infra_ready": [
         "do_run_state_load_all=localstack_persistence.snapshot.__plugins__:do_run_state_load_all"
     ],
     "localstack.hooks.on_infra_start": [
+        "register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints",
+        "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource",
         "register_state_load_strategy=localstack_persistence.snapshot.__plugins__:register_state_load_strategy",
         "register_state_resource=localstack_persistence.snapshot.__plugins__:register_state_resource",
         "register_state_save_strategy=localstack_persistence.snapshot.__plugins__:register_state_save_strategy",
-        "register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints",
-        "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime",
-        "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource"
+        "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime"
     ],
     "localstack.hooks.prepare_host": [
         "register_pickle_patches_host=localstack_persistence.pickling.__plugins__:register_pickle_patches_host"
     ]
 }
```

### Comparing `localstack-plugin-persistence-1.0.5/pyproject.toml` & `localstack-plugin-persistence-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.5/setup.cfg` & `localstack-plugin-persistence-1.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-plugin-persistence
-version = 1.0.5
+version = 1.0.6
 url = https://github.com/localstack/localstack-plugin-persistence
 author = LocalStack Contributors
 author_email = info@localstack.cloud
 description = plugin containing persistence code
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
```

