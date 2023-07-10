# Comparing `tmp/gladier-0.8.4b1.tar.gz` & `tmp/gladier-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-0.8.4b1.tar", last modified: Tue Apr  4 15:55:07 2023, max compression
+gzip compressed data, was "gladier-0.9.0b1.tar", last modified: Mon Jul 10 16:20:44 2023, max compression
```

## Comparing `gladier-0.8.4b1.tar` & `gladier-0.9.0b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.876788 gladier-0.8.4b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 15:54:46.000000 gladier-0.8.4b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-04 15:54:46.000000 gladier-0.8.4b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-04 15:55:07.876788 gladier-0.8.4b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-04 15:54:46.000000 gladier-0.8.4b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17889 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/flows_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/funcx_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.876788 gladier-0.8.4b1/gladier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/automate.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/dynamic_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/flow_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/flow_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/flow_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/funcx_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/name_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/tool_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/tool_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 15:54:50.000000 gladier-0.8.4b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 15:55:07.876788 gladier-0.8.4b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-04 15:54:50.000000 gladier-0.8.4b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.201231 gladier-0.9.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 16:20:33.000000 gladier-0.9.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 16:20:33.000000 gladier-0.9.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-10 16:20:44.201231 gladier-0.9.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-10 16:20:33.000000 gladier-0.9.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22417 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/compute_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/compute_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/flows_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/managers/service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/storage/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.201231 gladier-0.9.0b1/gladier/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/dynamic_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/flow_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/flow_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/flow_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/name_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/tool_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/utils/tool_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 16:20:33.000000 gladier-0.9.0b1/gladier/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:20:44.197230 gladier-0.9.0b1/gladier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 16:20:44.000000 gladier-0.9.0b1/gladier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 16:20:33.000000 gladier-0.9.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 16:20:44.201231 gladier-0.9.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-10 16:20:33.000000 gladier-0.9.0b1/setup.py
```

### Comparing `gladier-0.8.4b1/LICENSE` & `gladier-0.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4b1/PKG-INFO` & `gladier-0.9.0b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.8.4b1
+Version: 0.9.0b1
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Gladier: The Globus Architecture for Data-Intensive Experimental Research.
 ==========================================================================
 |docs|
@@ -45,27 +46,15 @@
 Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage 
 systems and manage using Globus Flows.
 
 Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field, 
 Gladier can help you streamline your data management and analysis workflows, so you can focus on your scientific discoveries.
 Try Gladier today and see how it can enhance your research capabilities!
 
-
-
-Installation
-============
-
-Gladier requires Python 3.6 and higher. For a modern version of python,
-see the official `Python Installation Guide <https://docs.python-guide.org/starting/installation/>`_.
-
-The easiest way to get Gladier is through Pip on PyPi. Gladier is built with two
-main packages, the core Gladier client and Gladier Tools. Gladier Tools include
-a set of reusable, common operations. Installing it is highly recommended.
-
-With pip installed, you can do the following:
+You can install Gladier and Gladier Tools with the following:
 
 
 .. code-block:: bash
 
    pip install gladier gladier-tools
 
 See the `Read-The-Docs <https://gladier.readthedocs.io/en/stable/?badge=stable>`_ getting started.
```

### Comparing `gladier-0.8.4b1/README.rst` & `gladier-0.9.0b1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -22,27 +22,15 @@
 Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage 
 systems and manage using Globus Flows.
 
 Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field, 
 Gladier can help you streamline your data management and analysis workflows, so you can focus on your scientific discoveries.
 Try Gladier today and see how it can enhance your research capabilities!
 
-
-
-Installation
-============
-
-Gladier requires Python 3.6 and higher. For a modern version of python,
-see the official `Python Installation Guide <https://docs.python-guide.org/starting/installation/>`_.
-
-The easiest way to get Gladier is through Pip on PyPi. Gladier is built with two
-main packages, the core Gladier client and Gladier Tools. Gladier Tools include
-a set of reusable, common operations. Installing it is highly recommended.
-
-With pip installed, you can do the following:
+You can install Gladier and Gladier Tools with the following:
 
 
 .. code-block:: bash
 
    pip install gladier gladier-tools
 
 See the `Read-The-Docs <https://gladier.readthedocs.io/en/stable/?badge=stable>`_ getting started.
```

### Comparing `gladier-0.8.4b1/gladier/base.py` & `gladier-0.9.0b1/gladier/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import List, Mapping, Any
 from gladier.utils.tool_alias import ToolAlias
 from gladier.utils.flow_traversal import iter_flow
 
 
 class GladierBaseTool(object):
     """Gladier Defaults defines a common method of tying together
-    flows, funcx-functions, and default inputs for starting a flow."""
+    flows, compute-functions, and default inputs for starting a flow."""
 
     flow_definition = None
     flow_input = dict()
     flow_transition_states = []
     required_input = []
-    alias_exempt = ['funcx_endpoint_compute', 'funcx_endpoint_non_compute']
-    funcx_endpoints = dict()
-    funcx_functions = []
+    alias_exempt = ['compute_endpoint']
+    compute_endpoints = dict()
+    compute_functions = []
 
     def __init__(self, alias: str = None, alias_class: ToolAlias = None):
         self.alias = alias
         alias_cls = alias_class
         if alias and not alias_class:
             raise ValueError(
                 f'{self.__class__.__name__} given alias "{alias}" but not "alias_class". '
```

### Comparing `gladier-0.8.4b1/gladier/client.py` & `gladier-0.9.0b1/gladier/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import os
+import pathlib
 import logging
-import warnings
-from typing import Union, Mapping
 from collections.abc import Iterable
 
 from gladier.base import GladierBaseTool
 from gladier.managers.login_manager import (
-    BaseLoginManager, CallbackLoginManager, AutoLoginManager
+    BaseLoginManager, AutoLoginManager, ConfidentialClientLoginManager
 )
 from globus_sdk import AccessTokenAuthorizer, RefreshTokenAuthorizer
-from gladier.managers import FlowsManager, FuncXManager
+from gladier.managers import FlowsManager, ComputeManager
 
 from gladier.storage.tokens import GladierSecretsConfig
-from gladier.storage.config import GladierConfig
 import gladier
 import gladier.storage.config
 import gladier.utils.dynamic_imports
 import gladier.utils.automate
 import gladier.utils.name_generation
 import gladier.storage.migrations
 import gladier.utils.tool_alias
-import gladier.utils.funcx_login_manager
+import gladier.managers.compute_login_manager
 import gladier.exc
 import gladier.version
 log = logging.getLogger(__name__)
 
 
 class GladierBaseClient(object):
     """
-    The Gladier Client ties together commonly used funcx functions
+    The Gladier Client ties together commonly used compute functions
     and basic flows with auto-registration tools to make complex tasks
     easy to automate.
 
     This class is intended to be subclassed as follows:
 
     .. code-block:: python
 
@@ -56,96 +54,127 @@
     * glaider_tools (default: [])
        * A list of Gladier Tools to build a working flow_defitinion. Each tool's minimum input
          must be satisfied prior to running the flow. Can be used with the
          @generate_flow_definition decorator to automatically chain together flow definitions
          present on each tool in linear order.
     * flow_definition (default: {})
        * An explicit flow definition to use for this client. Cannot be used with
-         @generate_flow_definition
+         @generate_flow_definition. Changes are tracked on each run, and will result
+         in a flow re-deploy on any change.
+    * flow_schema (default: {})
+       * A flow schema to accompany the flow definition. Schema is checked on each
+         run and are re-deployed if it changes. Overrides any existing schema set
+         on a given flow_manager instance unless unset.
     * secret_config_filename (default: ``~/.gladier-secrets.cfg``)
        * Storage are for Globus Tokens and general storage
     * app_name (default: 'Gladier Client')
        * The app name used during a login flow
     * client_id
        * The Globus Client ID used for native logins
     * globus_group (default: None)
        * A Globus Group to be applied to all flow/run permissions. Group will automatically be
          added to flow_viewers, flow_starters, flow_administrators, run_managers, run_monitors
     * subscription_id (default: None)
        * The subscription id associated with this flow
     * alias_class (default: gladier.utils.tool_alias.StateSuffixVariablePrefix)
        * The default class used to for applying aliases to Tools
 
+    The following Environment variables can be set and are recognized by Gladier Clients:
+
+    * GLADIER_CLIENT_ID -- Used only for setting confidential client credentials instead of user
+        credentials. This is a convenience feature, as an alternative to using a
+        custom login_manager
+    * GLADIER_CLIENT_SECRET -- Secret used for confidential clients, using with GLADIER_CLIENT_ID
+
     Default options are intended for CLI usage and maximum user convenience.
 
     :param auto_registration: Automatically register functions or flows if they are not
                               previously registered or obsolete.
     :param login_manager: Class defining login behavior. Defaults to AutoLoginManager, and
                           will auto-login when additional scopes are needed.
     :param flows_manager: A flows manager class with customized behavior. Attrs like group
                           and login_manager will automatically be set if None
     :raises gladier.exc.AuthException: if authorizers given are insufficient
 
     """
-    secret_config_filename = os.path.expanduser("~/.gladier-secrets.cfg")
-    app_name = 'Gladier Client'
-    client_id = 'f1631610-d9e4-4db2-81ba-7f93ad4414e3'
-    globus_group = None
-    subscription_id = None
+    secret_config_filename: str = None
+    app_name: str = 'Gladier Client'
+    client_id: str = 'f1631610-d9e4-4db2-81ba-7f93ad4414e3'
+    globus_group: str = None
+    subscription_id: str = None
     alias_class = gladier.utils.tool_alias.StateSuffixVariablePrefix
 
     def __init__(
         self,
-        authorizers: Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]] = None,
-        auto_login: bool = True,
         auto_registration: bool = True,
         login_manager: BaseLoginManager = None,
         flows_manager: FlowsManager = None,
             ):
 
         self._tools = None
-
-        # Setup storage
-        section = gladier.utils.name_generation.get_snake_case(self.__class__.__name__)
-        self.storage = GladierConfig(self.secret_config_filename, section)
-        self.storage.update()
-
-        if auto_login is False:
-            warnings.warn('auto_login=False in Gladier clients is deprecated and will '
-                          'be removed in v0.8. See '
-                          'https://gladier.readthedocs.io/en/latest/gladier/customizing_auth.html',
-                          category=DeprecationWarning)
-        if authorizers:
-            warnings.warn('Calling Gladier clients with "authorizers" is deprecated. Instead, see '
-                          'https://gladier.readthedocs.io/en/latest/gladier/customizing_auth.html',
-                          category=DeprecationWarning)
-            self.login_manager = CallbackLoginManager(authorizers=authorizers)
-        elif not login_manager:
-            section_name = f'tokens_{self.client_id}'
-            token_storage = GladierSecretsConfig(self.secret_config_filename, section_name)
-            self.login_manager = AutoLoginManager(self.client_id, token_storage, self.app_name,
-                                                  auto_login=auto_login)
-        else:
-            self.login_manager = login_manager
+        self.storage = self._determine_storage()
+        self.login_manager = login_manager or self._determine_login_manager(self.storage)
 
         self.flows_manager = flows_manager or FlowsManager(auto_registration=auto_registration)
         if self.globus_group:
             self.flows_manager.globus_group = self.globus_group
         if self.subscription_id:
             self.flows_manager.subscription_id = self.subscription_id
         if not self.flows_manager.flow_title:
             self.flows_manager.flow_title = f'{self.__class__.__name__} flow'
 
-        self.funcx_manager = FuncXManager(auto_registration=auto_registration)
+        self.compute_manager = ComputeManager(auto_registration=auto_registration)
+        self.storage.update()
 
-        for man in (self.flows_manager, self.funcx_manager):
+        for man in (self.flows_manager, self.compute_manager):
             man.set_storage(self.storage, replace=False)
             man.set_login_manager(self.login_manager, replace=False)
             man.register_scopes()
 
+    def _get_confidential_client_credentials(self):
+        return os.getenv('GLADIER_CLIENT_ID'), os.getenv('GLADIER_CLIENT_SECRET')
+
+    def _determine_storage(self):
+        """
+        Determine the storage location for Gladier. This is typically in the ~/.gladier directory,
+        but can be changed by setting the ``secret_config_filename`` on the class.
+
+        Setting GLADIER_CLIENT_ID will change the filename to the client id, so that config
+        items will not conflict with user details.
+        """
+        # Storage will automatically change if client credentials are detected.
+        CLI_ID, _ = self._get_confidential_client_credentials()
+        client_id = CLI_ID or self.client_id
+
+        if self.secret_config_filename:
+            storage_filename = pathlib.Path(self.secret_config_filename)
+        else:
+            storage_filename = pathlib.Path(f"~/.gladier/{client_id}.cfg").expanduser()
+            storage_filename.parent.mkdir(exist_ok=True)
+
+        storage_section = gladier.utils.name_generation.get_snake_case(self.__class__.__name__)
+        storage_tokens_section = f'tokens_{client_id}'
+
+        return GladierSecretsConfig(storage_filename, storage_section,
+                                    tokens_section=storage_tokens_section)
+
+    def _determine_login_manager(self, storage):
+        """
+        Determine the login manager to use for Glaider. First searches for evnironment
+        variables for a confidential client, then defaults to an AutoLoginManager using
+        a native client id set as ``client_id`` on this class.
+        """
+        CLI_ID, CLI_SEC = self._get_confidential_client_credentials()
+        if CLI_ID and CLI_SEC:
+            log.info('Client Credentials detected, using custom internal storage for '
+                     'storing tokens.')
+            return ConfidentialClientLoginManager(CLI_ID, CLI_SEC, storage=storage)
+        else:
+            return AutoLoginManager(self.client_id, storage, self.app_name)
+
     @staticmethod
     def get_gladier_defaults_cls(tool_ref, alias_class=None):
         """
         Load a Gladier default class (gladier.GladierBaseTool) by import string. For
         Example: get_gladier_defaults_cls('gladier.tools.hello_world.HelloWorld')
 
         :param tool_ref: A tool ref can be a dotted import string or an actual GladierBaseTool
@@ -181,28 +210,30 @@
         Load the current list of tools configured on this class
 
         :return: a list of subclassed instances of gladier.GladierBaseTool
         """
         if getattr(self, '_tools', None):
             return self._tools
 
-        if not getattr(self, 'gladier_tools', None) or not isinstance(self.gladier_tools, Iterable):
-            raise gladier.exc.ConfigException(
-                '"gladier_tools" must be a defined list of Gladier Tools. '
-                'Ex: ["gladier.tools.hello_world.HelloWorld"]')
+        gtools = getattr(self, 'gladier_tools', [])
+        if not gtools or not isinstance(gtools, Iterable):
+            if not self.get_flow_definition():
+                raise gladier.exc.ConfigException(
+                    '"gladier_tools" must be a defined list of Gladier Tools. '
+                    'Ex: ["gladier.tools.hello_world.HelloWorld"]')
         self._tools = [self.get_gladier_defaults_cls(gt, self.alias_class)
-                       for gt in self.gladier_tools]
+                       for gt in gtools]
         return self._tools
 
     @property
     def scopes(self):
         """
         The current list of scopes required by this class. This changes if there
         is a flow configured in the local Gladier config file, otherwise it will
-        only consist of basic scopes for running the funcx client/flows client/etc
+        only consist of basic scopes for running the compute client/flows client/etc
 
         :return: list of globus scopes required by this client
         """
         return list(self.login_manager.get_authorizers().keys())
 
     @property
     def missing_authorizers(self):
@@ -250,77 +281,139 @@
             return self.flow_definition
         elif isinstance(self.flow_definition, str):
             return self.get_gladier_defaults_cls(self.flow_definition).flow_definition
         raise gladier.exc.ConfigException('"flow_definition" must be a dict or an import string '
                                           'to a sub-class of type '
                                           '"gladier.GladierBaseTool"')
 
+    def get_flow_schema(self):
+        """
+        Get the flow schema attached to this class.
+        """
+        return getattr(self, 'flow_schema', None)
+
     def sync_flow(self):
         self.flows_manager.flow_definition = self.get_flow_definition()
+        schema = self.get_flow_schema()
+        if schema:
+            self.flows_manager.flow_schema = schema
         self.flows_manager.sync_flow()
 
     def run_flow(self, flow_input=None, use_defaults=True, **flow_kwargs):
+        r"""
+        Start a Globus Automate flow. By default, the flow definiton is checked and synced if it
+        has changed locally or deployed if it does not exist.
+
+        If a group is set, run permissions are updated and applied to the run (includes
+        'run_managers', 'run_monitors').
+
+        Any scope changes required post-deployment/update are propogated through the login_manager
+        and may require an additional login. A new flow checksum/id may be tracked in storage if
+        the flow changed or was newly deployed.
+
+        The run_flow method shadows the globus-automate-client method for running flows documented
+        here: https://globus-automate-client.readthedocs.io/en/latest/python_sdk_reference.html#globus_automate_client.flows_client.FlowsClient.run_flow  # noqa
+        Additional arguments matching the method signature may be added. Common ones include the
+        following:
+
+        * **label** (Optional[str]) An optional label which can be used to identify this run
+        * **tags** (Optional[List[str]]) Tags that will be associated with this Run.
+
+        Example:
+
+        .. code-block:: python
+
+            myinput = {
+                "input": {
+                    "args": "cat /proc/version",
+                    "capture_output": True,
+                    "compute_endpoint": "4b116d3c-1703-4f8f-9f6f-39921e5864df",
+                }
+            }
+            my_client.run_flow(myinput, label='Check Version', tags=['version', 'POSIX'])
+
+        :param flow_input: A dict of input to be passed to the automate flow. self.check_input()
+                           is called on each tool to ensure basic needs are met for each.
+                           Input MUST be wrapped inside an 'input' dict,
+                           for example {'input': {'foo': 'bar'}}.
+
+        :param use_defaults: Use the result of self.get_input() to populate base input for the
+                             flow. All conflicting input provided by flow_input overrides
+                             values set in use_defaults.
+        :param \**flow_kwargs: Set several keyed arguments that include the label to be used
+                               in the automate app. If no label is passed the standard automate
+                               label is used. Also ensure label <= 64 chars long.
+        :raise: gladier.exc.ConfigException by self.check_input()
+        :raises: gladier.exc.FlowObsolete
+        :raises: gladier.exc.NoFlowRegistered
+        :raises: gladier.exc.RegistrationException
+        :raises: gladier.exc.FunctionObsolete
+        :raises: gladier.exc.AuthException
+        :raises: Any globus_sdk.exc.BaseException
+        """
         combine_flow_input = self.get_input() if use_defaults else dict()
         if flow_input is not None:
             if not flow_input.get('input') or len(flow_input.keys()) != 1:
                 raise gladier.exc.ConfigException(
                     f'Malformed input to flow, all input must be nested under "input", got '
                     f'{flow_input.keys()}')
             combine_flow_input['input'].update(flow_input['input'])
         for tool in self.tools:
             self.check_input(tool, combine_flow_input)
 
         self.sync_flow()
         return self.flows_manager.run_flow(flow_input=combine_flow_input, **flow_kwargs)
 
-    def get_funcx_function_ids(self):
-        """Get all funcx function ids for this run, registering them if there are no ids
+    def get_compute_function_ids(self):
+        """Get all compute function ids for this run, registering them if there are no ids
         stored in the local Gladier config file OR the stored function id checksums do
         not match the actual functions provided on each of the Gladier tools. If register
         is False, no changes to the config will be made and exceptions will be raised instead.
 
         :raises: gladier.exc.RegistrationException
         :raises: gladier.exc.FunctionObsolete
-        :returns: a dict of function ids where keys are names and values are funcX function ids.
+        :returns: a dict of function ids where keys are names and values are compute function ids.
         """
-        funcx_ids = dict()
+        compute_ids = dict()
         for tool in self.tools:
             log.debug(f'Checking functions for {tool}')
-            funcx_funcs = getattr(tool, 'funcx_functions', [])
-            if not funcx_funcs:
-                log.warning(f'Tool {tool} did not define any funcX functions!')
-            if not funcx_funcs and not isinstance(funcx_funcs, Iterable):
+            compute_funcs = (
+                getattr(tool, 'compute_functions', []) + getattr(tool, 'funcx_functions', [])
+            )
+            if not compute_funcs:
+                log.warning(f'Tool {tool} did not define any compute functions!')
+            if not compute_funcs and not isinstance(compute_funcs, Iterable):
                 raise gladier.exc.DeveloperException(
-                    f'Attribute "funcx_functions" on {tool} needs to be an iterable! Found '
-                    f'{type(funcx_funcs)}')
+                    f'Attribute "compute_functions" on {tool} needs to be an iterable! Found '
+                    f'{type(compute_funcs)}')
 
-            for func in funcx_funcs:
-                name, val = self.funcx_manager.validate_function(tool, func)
-                funcx_ids[name] = val
-        return funcx_ids
+            for func in compute_funcs:
+                name, val = self.compute_manager.validate_function(tool, func)
+                compute_ids[name] = val
+        return compute_ids
 
     def get_flow_id(self) -> str:
         """
         Get the flow id from the flows manager class.
         """
         return self.flows_manager.get_flow_id()
 
     def get_input(self) -> dict:
         """
-        Get funcx function ids, funcx endpoints, and each tool's default input. Default
+        Get compute function ids, compute endpoints, and each tool's default input. Default
         input may not be enough to run the flow. For example if a tool does processing on a
         local filesystem, the file will always need to be provided by the user when calling
         run_flow().
 
         Defaults rely on GladierBaseTool.flow_input defined separately for each tool.
 
         :return: input for a flow wrapped in an 'input' dict. For example:
                  {'input': {'foo': 'bar'}}
         """
-        flow_input = self.get_funcx_function_ids()
+        flow_input = self.get_compute_function_ids()
         for tool in self.tools:
             # conflicts = set(flow_input.keys()).intersection(set(tool.flow_input))
             # if conflicts:
             #     for prev_tools in tools:
             #         for r in prev_tools.flow_input:
             #             if set(flow_input.keys()).intersection(set(tool.flow_input)):
             #                 raise gladier.exc.ConfigException(
@@ -349,15 +442,15 @@
         for req_input in tool.get_required_input():
             if req_input not in flow_input['input']:
                 raise gladier.exc.ConfigException(
                     f'{tool} requires flow input value: "{req_input}"')
 
     def get_status(self, action_id: str):
         """
-        Get the current status of the automate flow. Attempts to do additional work on funcx
+        Get the current status of the automate flow. Attempts to do additional work on compute
         functions to deserialize any exception output.
 
         :param action_id: The globus action UUID used for this flow. The Automate flow id is
                           always the flow_id configured for this tool.
         :raises: Globus Automate exceptions from self.flows_client.flow_action_status
         :returns: a Globus Automate status object (with varying state structures)
         """
```

### Comparing `gladier-0.8.4b1/gladier/decorators.py` & `gladier-0.9.0b1/gladier/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from gladier.exc import FlowGenException
 from gladier.utils.flow_generation import generate_tool_flow, combine_tool_flows
 
 
 def generate_flow_definition(_cls=None, *, modifiers=None):
     """Class decorators for automatically generating flows on either
     GladierBaseTools or GladierClients. For GladierBaseTools, this generates
-    a simple flow containing all attached funcx_functions, applying any modifiers
+    a simple flow containing all attached compute_functions, applying any modifiers
     for custom values the GladierBaseTool needs to run. For GladierClients, this
     instead stitches together all flows defined on GladierBaseTools, in the order
     they are defined for each BaseTool. ``modifiers`` are only allowed on
     GladierBaseTools.
 
     Example:
     @generate_flow_definition(modifiers={
-        my_funcx_function: {
-            'payload': '$.MyFuncxFunction.details.result',
-            'endpoint': 'funcx_endpoint_non_compute'
+        my_compute_function: {
+            'payload': '$.MycomputeFunction.details.result',
+            'endpoint': 'compute_endpoint'
         }
     })
 
     Any modifier values without a preceding '$.' will be replaced with
     a path to general input. The above would result in the following
-    for ``funcx_endpoint_non_compute`` above:
-        '$.input.funcx_endpoint_non_compute'
+    for ``compute_endpoint`` above:
+        '$.input.compute_endpoint'
 
     :raises FlowGenException: For a variety of invalid inputs"""
     modifiers = modifiers or dict()
 
     def decorator_wrapper(cls):
         @functools.wraps(cls)
         def wrapper(*args, **kwargs):
```

### Comparing `gladier-0.8.4b1/gladier/exc.py` & `gladier-0.9.0b1/gladier/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 
 
 class NoFlowRegistered(RegistrationException):
     pass
 
 
 class ObsoleteException(RegistrationException):
-    """A funcx function or flow has local changes not reflected
+    """A compute function or flow has local changes not reflected
     in the currently registered id"""
     pass
 
 
 class FlowObsolete(ObsoleteException):
     """The local flow definition has changed and needs to be updated"""
     pass
 
 
 class FunctionObsolete(ObsoleteException):
-    """A local funcx function definition has changed and needs to be updated"""
+    """A local compute function definition has changed and needs to be updated"""
     pass
 
 
 class FlowGenException(GladierException):
     """Something went wrong when auto-generating a flow"""
     pass
```

### Comparing `gladier-0.8.4b1/gladier/managers/flows_manager.py` & `gladier-0.9.0b1/gladier/managers/flows_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from gladier.managers.service_manager import ServiceManager
 import gladier.storage.config
 import gladier.utils.dynamic_imports
 import gladier.utils.automate
 import gladier.utils.name_generation
 import gladier.storage.migrations
 import gladier.utils.tool_alias
-import gladier.utils.funcx_login_manager
+import gladier.managers.compute_login_manager
 import gladier.exc
 import gladier.version
 
 from globus_automate_client.flows_client import (
     MANAGE_FLOWS_SCOPE,
     VIEW_FLOWS_SCOPE,
     RUN_FLOWS_SCOPE,
@@ -57,16 +57,16 @@
     :param flow_schema: The schema to be used alongside the flow definition
     :param flow_title: The title for the Globus Flow
     :param globus_group: A Globus Group UUID. Used to grant all flow and run permissions
     :param subscription_id: (deprecated) Subscription ID has no effect and will be removed in a
                             future version.
     :param on_change: callback on checksum mismatch or missing flow id. Default registers/deploys
                       flow, ``None`` takes no action and attempts to run "obselete" flows.
-    :param redeploy_on_404: Deploy a new flow if attempting to run the current flow ID results in 404.
-                            Behavior is disabled if an explicit flow_id is specified.
+    :param redeploy_on_404: Deploy a new flow if attempting to run the current flow ID results
+                            in 404. Behavior is disabled if an explicit flow_id is specified.
 
     When used with a Gladier Client, following items will be auto-configured and should not be
     set explicitly in the constructor:
 
      * flow_definition
      * flow_schema
 
@@ -183,21 +183,25 @@
         return self._flows_client
 
     def refresh_flows_client(self) -> globus_automate_client.FlowsClient:
         self._flows_client = None
         return self.flows_client
 
     @staticmethod
-    def get_flow_checksum(flow_definition):
+    def get_flow_checksum(flow_definition, flow_schema):
         """
         Get the SHA256 checksum of the current flow definition.
 
         :return: sha256 hex string of flow definition
         """
-        return hashlib.sha256(json.dumps(flow_definition, sort_keys=True).encode()).hexdigest()
+
+        flow_def = json.dumps(flow_definition, sort_keys=True)
+        flow_schema = json.dumps(flow_schema, sort_keys=True)
+        data = (flow_def + flow_schema).encode()
+        return hashlib.sha256(data).hexdigest()
 
     @staticmethod
     def get_globus_urn(uuid, id_type='group'):
         """Convenience method for appending the correct Globus URN prefix on a uuid."""
         URN_PREFIXES = {
             'group': 'urn:globus:groups:id:',
             'identity': 'urn:globus:auth:identity:'
@@ -259,15 +263,15 @@
         :raises: gladier.exc.FlowObsolete if the stored flow checksums do not match
         """
         flow_id = self.get_flow_id()
         flow_checksum = self.storage.get_value('flow_checksum')
         if not flow_id:
             raise gladier.exc.NoFlowRegistered(
                 'No flow_id set on flow manager and no id tracked in storage.')
-        elif flow_checksum != self.get_flow_checksum(self.flow_definition):
+        elif flow_checksum != self.get_flow_checksum(self.flow_definition, self.flow_schema):
             raise gladier.exc.FlowObsolete(
                 f'"flow_definition" on {self} has changed and needs to be re-registered.')
 
     def sync_flow(self) -> str:
         """
         Get the current flow id for the current Gladier flow definition.
         If self.auto_register is True, it will automatically (re)register a flow if it
@@ -308,70 +312,44 @@
         flow_kwargs = flow_permissions
         # Input schema is a required field and must be part of all flows.
         flow_kwargs['input_schema'] = self.flow_schema
         if flow_id:
             try:
                 log.info(f'Flow checksum failed, updating flow {flow_id}...')
                 self.flows_client.update_flow(flow_id, self.flow_definition, **flow_kwargs)
-                self.storage.set_value('flow_checksum',
-                                       self.get_flow_checksum(self.flow_definition))
+                self.storage.set_value(
+                    'flow_checksum', self.get_flow_checksum(self.flow_definition, self.flow_schema)
+                )
             except globus_sdk.exc.GlobusAPIError as gapie:
                 if gapie.http_status == 404 and self.redeploy_on_404:
                     flow_id = None
                 else:
                     raise
         if flow_id is None:
             log.info('No flow detected, deploying new flow...')
             flow = self.flows_client.deploy_flow(self.flow_definition, title=self.flow_title,
                                                  **flow_kwargs).data
+            log.debug(f'Flow deployed with id {flow["id"]}')
             self.storage.set_value('flow_id', flow['id'])
-            self.storage.set_value('flow_checksum', self.get_flow_checksum(self.flow_definition))
+            self.storage.set_value(
+                'flow_checksum', self.get_flow_checksum(self.flow_definition, self.flow_schema)
+            )
             self.login_manager.add_requirements([flow['globus_auth_scope']])
             self.refresh_flows_client()
 
         return flow_id
 
     def purge_flow(self):
         """
         Remove the stored flow_id and flow_checksum.
         """
         self.storage.del_value('flow_id')
         self.storage.del_value('flow_checksum')
 
     def run_flow(self, **kwargs):
-        r"""
-        Start a Globus Automate flow. By default, the flow definiton is checked and synced if it
-        has changed locally or deployed if it does not exist.
-
-        If a group is set, run permissions are updated and applied to the run (includes
-        'run_managers', 'run_monitors').
-
-        Any scope changes required post-deployment/update are propogated through the login_manager
-        and may require an additional login. A new flow checksum/id may be tracked in storage if
-        the flow changed or was newly deployed.
-
-        :param flow_input: A dict of input to be passed to the automate flow. self.check_input()
-                           is called on each tool to ensure basic needs are met for each.
-                           Input MUST be wrapped inside an 'input' dict,
-                           for example {'input': {'foo': 'bar'}}.
-
-        :param use_defaults: Use the result of self.get_input() to populate base input for the
-                             flow. All conflicting input provided by flow_input overrides
-                             values set in use_defaults.
-        :param \**flow_kwargs: Set several keyed arguments that include the label to be used
-                               in the automate app. If no label is passed the standard automate
-                               label is used. Also ensure label <= 64 chars long.
-        :raise: gladier.exc.ConfigException by self.check_input()
-        :raises: gladier.exc.FlowObsolete
-        :raises: gladier.exc.NoFlowRegistered
-        :raises: gladier.exc.RegistrationException
-        :raises: gladier.exc.FunctionObsolete
-        :raises: gladier.exc.AuthException
-        :raises: Any globus_sdk.exc.BaseException
-        """
         flow_id = self.get_flow_id()
 
         permissions = {
             p_type: self.get_flow_permission(p_type)
             for p_type in ['run_managers', 'run_monitors']
             if self.get_flow_permission(p_type)
         }
@@ -412,15 +390,15 @@
 
         if flow['status'] == 'FAILED':
             raise gladier.exc.ConfigException(f'Flow Failed: {flow["details"]["description"]}')
         return flow
 
     def get_status(self, run_id):
         """
-        Get the current status of the automate flow. Attempts to do additional work on funcx
+        Get the current status of the automate flow. Attempts to do additional work on compute
         functions to deserialize any exception output.
 
         :param run_id: The globus action UUID used for this flow. The Automate flow id is
                           always the flow_id configured for this tool.
         :raises: Globus Automate exceptions from self.flows_client.flow_action_status
         :returns: a Globus Automate status object (with varying state structures)
         """
```

### Comparing `gladier-0.8.4b1/gladier/managers/login_manager.py` & `gladier-0.9.0b1/gladier/managers/login_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
+import time
 from typing import Callable, List, Set, Iterable, Union, Any, Mapping
 import abc
 
 import fair_research_login
-from globus_sdk import AccessTokenAuthorizer, RefreshTokenAuthorizer
+from globus_sdk import AccessTokenAuthorizer, RefreshTokenAuthorizer, ConfidentialAppAuthClient
 from gladier.exc import AuthException
+from gladier.storage.tokens import GladierSecretsConfig
 
 log = logging.getLogger(__name__)
 
 
 class BaseLoginManager(abc.ABC):
 
     def __init__(self, *args, **kwargs):
@@ -106,15 +108,15 @@
                 'Gladier client must be instantiated with a '
                 '"client_id" to use "login()!'
             )
         return fair_research_login.NativeClient(client_id=self.client_id,
                                                 app_name=self.app_name,
                                                 token_storage=self.storage)
 
-    def get_authorizers(self) -> List[Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
         try:
             return self.native_client.get_authorizers_by_scope()
         except fair_research_login.LoadError:
             return dict()
 
     def login(self, scopes):
         if self.auto_login is False:
@@ -126,15 +128,15 @@
     def logout(self):
         self.native_client.logout()
 
 
 class CallbackLoginManager(BaseLoginManager):
     """
     The Callback Login Manager allows for finer grained control of auth within Gladier. Logins
-    are lazy up until Gladier attempts to make a call to the FuncX service, Flows service, or
+    are lazy up until Gladier attempts to make a call to the Compute service, Flows service, or
     tries to run a flow. Scopes for a deployed flow may be modified at any time, requiring
     a re-login with that flow scope.
 
     :param authorizers: A dict of autorizers by scope. If these satisfy the login requirements
                         then the callback will not be triggered.
     :param callback: A Callable which will be invoked if additional scopes are needed.
 
@@ -145,17 +147,64 @@
         authorizers: Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]],
         callback: Callable = None
     ):
         super().__init__()
         self.authorizers = authorizers
         self.callback = callback
 
-    def get_authorizers(self) -> List[Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
         return self.authorizers
 
     def login(self, scopes):
         if not self.callback:
             raise AuthException('New login required for scopes and no callback set on '
                                 f'login manager: {scopes}')
         new_authorizers = self.callback(scopes)
         self.authorizers.update(new_authorizers)
         log.info('New authorizers have been cached for re-use.')
+
+
+class ConfidentialClientLoginManager(BaseLoginManager):
+    refresh_tokens = True
+
+    def __init__(self, client_id: str, client_secret: str, storage: GladierSecretsConfig):
+        super().__init__()
+        self.storage: GladierSecretsConfig = storage
+        self.client_id = client_id
+        self.app = ConfidentialAppAuthClient(client_id, client_secret)
+
+    def login(self, scopes: List[str]) -> None:
+        log.info('Initiating client credentials grant using client_id and secret')
+        response = self.app.oauth2_client_credentials_tokens(requested_scopes=scopes)
+        self.storage.write_tokens(response.by_resource_server)
+
+    def by_scopes(self, tokens):
+        # Get a flat list of scopes
+        scopes = [tset['scope'].split() for tset in tokens.values()]
+        scopes = [item for sublist in scopes for item in sublist]
+
+        token_group = {}
+        for scope in scopes:
+            for tgroup in tokens.values():
+                if scope in tgroup['scope'].split():
+                    token_group[scope] = tgroup
+        return token_group
+
+    def get_authorizers(self) -> Mapping[str, Union[AccessTokenAuthorizer, RefreshTokenAuthorizer]]:
+        tokens = self.storage.read_tokens()
+        if not tokens:
+            log.info('Tokens failed to load, no tokens in storage.')
+            return dict()
+
+        expired = any(t['expires_at_seconds'] < time.time() for t in tokens.values())
+        if expired:
+            log.info('Tokens Expired, clearing cache')
+            self.storage.clear_tokens()
+            return dict()
+
+        return {
+            scope: RefreshTokenAuthorizer(refresh_token=tdata['refresh_token'],
+                                          auth_client=self.app,
+                                          access_token=tdata['access_token'],
+                                          expires_at=tdata['expires_at_seconds'])
+            for scope, tdata in self.by_scopes(tokens).items()
+        }
```

### Comparing `gladier-0.8.4b1/gladier/managers/service_manager.py` & `gladier-0.9.0b1/gladier/managers/service_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4b1/gladier/storage/config.py` & `gladier-0.9.0b1/gladier/storage/config.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4b1/gladier/storage/tokens.py` & `gladier-0.9.0b1/gladier/storage/tokens.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import os
 import stat
+import logging
 from fair_research_login.token_storage import flat_pack, flat_unpack
 from gladier.storage.config import GladierConfig
 
 
+log = logging.getLogger(__name__)
+
+
 class GladierSecretsConfig(GladierConfig):
 
     DEFAULT_PERMISSION = stat.S_IRUSR | stat.S_IWUSR
 
+    def __init__(self, *args, tokens_section='tokens', **kwargs):
+        self.tokens_section = tokens_section
+        super().__init__(*args, **kwargs)
+
     def save(self):
         super().save()
         os.chmod(self.filename, self.DEFAULT_PERMISSION)
 
+    def load(self):
+        super().load()
+        if self.tokens_section not in self.sections():
+            self[self.tokens_section] = {}
+            self.save()
+
     def write_tokens(self, tokens):
         self.load()
         for name, value in flat_pack(tokens).items():
-            self.set(self.section, name, value)
+            self.set(self.tokens_section, name, value)
+        log.debug(f'Wrote tokens to {self.filename}')
         self.save()
 
     def read_tokens(self):
         self.load()
-        return flat_unpack(dict(self.items(self.section)))
+        return flat_unpack(dict(self.items(self.tokens_section)))
 
     def clear_tokens(self):
         self.load()
-        self.remove_section(self.section)
-        self.add_section(self.section)
+        self.remove_section(self.tokens_section)
+        self.add_section(self.tokens_section)
+        log.debug(f'Tokens cleared from {self.filename}')
         self.save()
```

### Comparing `gladier-0.8.4b1/gladier/utils/automate.py` & `gladier-0.9.0b1/gladier/utils/automate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import traceback
 import logging
-from funcx.serialize import FuncXSerializer
+from globus_compute_sdk import serialize
 
 log = logging.getLogger(__name__)
 
 automate_response_keys = {'action_id', 'status', 'state_name'}
-funcx_response_keys = {'result', 'status', 'exception', 'task_id'}
+compute_response_keys = {'result', 'status', 'exception', 'task_id'}
 
 
 def is_automate_response(state_output):
     return (
         isinstance(state_output, dict) and
         set(state_output.keys()).intersection(automate_response_keys)
     )
 
 
-def is_funcx_response(state_output):
+def is_compute_response(state_output):
     return (
         is_automate_response(state_output) and
-        set(state_output['details'].keys()).intersection(funcx_response_keys)
+        set(state_output['details'].keys()).intersection(compute_response_keys)
     )
 
 
 def get_details(response, state_name=None):
     if state_name and is_automate_response(response['details']['output'].get(state_name)):
         return response['details']['output'][state_name]
 
-    if is_funcx_response(response['details']['output'].get(state_name)):
+    if is_compute_response(response['details']['output'].get(state_name)):
         resp = response['details']['output'][state_name]
         if resp.get('exception'):
             resp['exception'] = deserialize_exception(resp['exception'])
         return resp
 
     for flow_state, data in response['details']['output'].items():
         # Reject any output that isn't structured as a response
-        if not is_funcx_response(data):
+        if not is_compute_response(data):
             continue
         if isinstance(data['details'], dict) and data['details'].get('exception'):
             exc = deserialize_exception(data['details']['exception'])
             data['details']['exception'] = exc
     return response
 
 
 def deserialize_exception(encoded_exc):
     try:
-        FuncXSerializer().deserialize(encoded_exc).reraise()
+        serialize.ComputeSerializer().deserialize(encoded_exc).reraise()
     except Exception:
         return traceback.format_exc()
```

### Comparing `gladier-0.8.4b1/gladier/utils/dynamic_imports.py` & `gladier-0.9.0b1/gladier/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4b1/gladier/utils/flow_generation.py` & `gladier-0.9.0b1/gladier/utils/flow_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import typing
 from gladier.base import GladierBaseTool
 from gladier.client import GladierBaseClient
 from gladier.exc import FlowGenException
 from gladier.utils.flow_modifiers import FlowModifiers
 from gladier.utils.name_generation import (
-    get_funcx_flow_state_name,
-    get_funcx_function_name
+    get_compute_flow_state_name,
+    get_compute_function_name
 )
 from gladier.utils.tool_chain import ToolChain
 
 
 log = logging.getLogger(__name__)
 
 
@@ -22,53 +22,66 @@
     Modifiers can be applied to any of the states within the flow.
     """
     flow_moder = FlowModifiers(client.tools, modifiers, cls=client)
     chain = ToolChain(flow_comment=client.__doc__).chain(client.tools)
     return flow_moder.apply_modifiers(chain.flow_definition)
 
 
-def _get_duplicate_functions(funcx_functions: typing.List[callable]):
+def _get_duplicate_functions(compute_functions: typing.List[callable]):
     tracked_set = set()
-    func_names = [get_funcx_flow_state_name(f) for f in funcx_functions]
+    func_names = [get_compute_flow_state_name(f) for f in compute_functions]
     return [f for f in func_names if f in tracked_set or tracked_set.add(f)]
 
 
+def _fix_old_tools(tool):
+    funcx_functions = getattr(tool, 'funcx_functions', None)
+    compute_functions = getattr(tool, 'compute_functions', None)
+
+    if funcx_functions and not compute_functions:
+        log.warning(f'Tool {tool} defines attributue "funcx_functions" which has now been '
+                    'changed to "compute_functions". Automatically configuring compute_functions '
+                    f'for new tool. Please update the old tool {tool}')
+        setattr(tool, 'compute_functions', funcx_functions)
+
+
 def generate_tool_flow(tool: GladierBaseTool, modifiers):
-    """Generate a flow definition for a Gladier Tool based on the defined ``funcx_functions``.
-    Accepts modifiers for funcx functions"""
-    duplicate_functions = _get_duplicate_functions(tool.funcx_functions)
+    """Generate a flow definition for a Gladier Tool based on the defined ``compute_functions``.
+    Accepts modifiers for compute functions"""
+    _fix_old_tools(tool)
+
+    duplicate_functions = _get_duplicate_functions(tool.compute_functions)
     if duplicate_functions:
         raise FlowGenException(f'Tool {tool} contains duplicate function names: '
                                f'{duplicate_functions}')
 
     flow_moder = FlowModifiers([tool], modifiers, cls=tool)
 
     tools = ToolChain()
-    for fx_func in tool.funcx_functions:
-        tools.chain_state(*generate_funcx_flow_state(fx_func))
+    for fx_func in tool.compute_functions:
+        tools.chain_state(*generate_compute_flow_state(fx_func))
 
     flow = tools.flow_definition
     if not flow['States']:
         raise FlowGenException(f'Tool {tool} has no flow states. Add a list of python functions '
-                               f'as "{tool}.funcx_functions = [myfunction]" or set a custom flow '
+                               f'as "{tool}.compute_functions = [myfunction]" or set a custom flow '
                                f'definition instead using `{tool}.flow_definition = mydef`')
     return flow_moder.apply_modifiers(flow)
 
 
-def generate_funcx_flow_state(funcx_function):
-    state_name = get_funcx_flow_state_name(funcx_function)
+def generate_compute_flow_state(compute_function):
+    state_name = get_compute_flow_state_name(compute_function)
 
     return state_name, {
-        'Comment': funcx_function.__doc__,
+        'Comment': compute_function.__doc__,
         'Type': 'Action',
-        'ActionUrl': 'https://compute2.dev.funcx.org/fxap',
+        'ActionUrl': 'https://compute.actions.globus.org',
         'ExceptionOnActionFailure': False,
         'Parameters': {
             'tasks': [{
-                'endpoint.$': '$.input.funcx_endpoint_compute',
-                'function.$': f'$.input.{get_funcx_function_name(funcx_function)}',
+                'endpoint.$': '$.input.compute_endpoint',
+                'function.$': f'$.input.{get_compute_function_name(compute_function)}',
                 'payload.$': '$.input',
             }]
         },
         'ResultPath': f'$.{state_name}',
         'WaitTime': 300,
     }
```

### Comparing `gladier-0.8.4b1/gladier/utils/flow_modifiers.py` & `gladier-0.9.0b1/gladier/utils/flow_modifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from gladier.exc import FlowModifierException
-from gladier.utils.name_generation import get_funcx_flow_state_name
+from gladier.utils.name_generation import get_compute_flow_state_name
 
 log = logging.getLogger(__name__)
-funcx_modifiers = {'endpoint', 'payload', 'tasks'}
+compute_modifiers = {'endpoint', 'payload', 'tasks'}
 # All top level states can be modified.
 # https://globus-automate-client.readthedocs.io/en/latest/authoring_flows.html#action-state-type
 state_modifiers = {
     'Type',
     'ActionUrl',
     'WaitTime',
     'ExceptionOnActionFailure',
@@ -19,47 +19,57 @@
     'ActionScope',
     'Next',
     'End',
 }
 
 
 class FlowModifiers:
-    supported_modifiers = state_modifiers.union(funcx_modifiers)
-    funcx_modifiers = funcx_modifiers
+    supported_modifiers = state_modifiers.union(compute_modifiers)
+    compute_modifiers = compute_modifiers
     state_modifiers = state_modifiers
 
     def __init__(self, tools, modifiers, cls=None):
         self.cls = cls
         self.tools = tools
-        self.functions = [func for tool in tools for func in tool.funcx_functions]
+        self.functions = [func for tool in tools for func in tool.compute_functions]
         self.function_names = [f.__name__ for f in self.functions]
-        self.state_names = [get_funcx_flow_state_name(f) for f in self.functions]
+        self.state_names = [get_compute_flow_state_name(f) for f in self.functions]
         self.modifiers = modifiers
         self.check_modifiers()
 
     def get_function(self, function_identifier):
         if function_identifier in self.function_names:
             return self.functions[self.function_names.index(function_identifier)]
         if function_identifier in self.functions:
             return function_identifier
 
     def get_flow_state_name(self, function_identifier):
         func = self.get_function(function_identifier)
-        return get_funcx_flow_state_name(func)
+        return get_compute_flow_state_name(func)
 
     def get_state_result_path(self, state_name):
         return f'$.{state_name}.details.results'
 
     def check_modifiers(self):
         log.debug(f'Checking modifiers: {self.modifiers}')
         if not isinstance(self.modifiers, dict):
             raise FlowModifierException(f'{self.cls}: Flow Modifiers must be a dict')
 
+        legacy_funcs = [func for tool in self.tools
+                        for func in getattr(tool, 'funcx_functions', [])]
+        legacy_func_names = [f.__name__ for f in legacy_funcs]
+
         # Check if modifiers were set correctly
         for name, mods in self.modifiers.items():
+            if name in legacy_func_names:
+                raise FlowModifierException(
+                    f'Class {self.cls} is a Legacy Gladier tool pre-v0.9.0. Please use a modern '
+                    'version or follow the migration guide here to make it compatible: \n\n'
+                    '\thttps://gladier.readthedocs.io/en/latest/migration.html\n')
+
             if not self.get_function(name):
                 raise FlowModifierException(f'Class {self.cls} included modifier which does not '
                                             f'exist: {name}. Allowed modifiers include '
                                             f'{", ".join(self.function_names)}')
 
             for mod_name, mod_value in mods.items():
                 if mod_name not in self.supported_modifiers:
@@ -73,16 +83,16 @@
             flow['States'][state_name] = self.apply_modifier(flow['States'][state_name], mods)
         return flow
 
     def apply_modifier(self, flow_state, state_modifiers):
 
         for modifier_name, value in state_modifiers.items():
             log.debug(f'Applying modifier "{modifier_name}", value "{value}"')
-            # If this is for a funcx task
-            if modifier_name in self.funcx_modifiers:
+            # If this is for a compute task
+            if modifier_name in self.compute_modifiers:
                 if modifier_name == 'tasks':
                     flow_state['Parameters'] = self.generic_set_modifier(
                         flow_state['Parameters'], 'tasks', value)
                 else:
                     flow_state['Parameters']['tasks'] = [
                         self.generic_set_modifier(fx_task, modifier_name, value)
                         for fx_task in flow_state['Parameters']['tasks']
@@ -90,15 +100,15 @@
             elif modifier_name in self.state_modifiers:
                 self.generic_set_modifier(flow_state, modifier_name, value)
         return flow_state
 
     def generic_set_modifier(self, item, mod_name, mod_value):
         if not isinstance(mod_value, str):
             if mod_value in self.functions:
-                sn = get_funcx_flow_state_name(mod_value)
+                sn = get_compute_flow_state_name(mod_value)
                 mod_value = self.get_state_result_path(sn)
         elif isinstance(mod_value, str) and not mod_value.startswith('$.'):
             if mod_value in self.function_names:
                 sn = self.state_names[self.function_names.index(mod_value)]
                 mod_value = self.get_state_result_path(sn)
             elif mod_value in self.state_names:
                 mod_value = self.get_state_result_path(mod_value)
```

### Comparing `gladier-0.8.4b1/gladier/utils/flow_traversal.py` & `gladier-0.9.0b1/gladier/utils/flow_traversal.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4b1/gladier/utils/name_generation.py` & `gladier-0.9.0b1/gladier/utils/name_generation.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 def get_snake_case(upper_camel_case):
     # https://stackoverflow.com/questions/1175208/elegant-python-function-to-convert-camelcase-to-snake-case
     snake_name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', upper_camel_case)
     snake_name = re.sub('([a-z0-9])([A-Z])', r'\1_\2', snake_name).lower()
     return snake_name
 
 
-def get_funcx_flow_state_name(funcx_function):
+def get_compute_flow_state_name(compute_function):
     """State names in Automate are typically upper camel case. This function generates
-    an upper case funcx function name for flow states."""
-    return get_upper_camel_case(funcx_function.__name__)
+    an upper case compute function name for flow states."""
+    return get_upper_camel_case(compute_function.__name__)
 
 
-def get_funcx_function_name(funcx_function):
+def get_compute_function_name(compute_function):
     """
-    Generate a function name given a funcx function. These function names are used to refer
-    to funcx functions within the config. There is no guarantee of uniqueness for function
+    Generate a function name given a compute function. These function names are used to refer
+    to compute functions within the config. There is no guarantee of uniqueness for function
     names.
 
     :return: human readable string identifier for a function (intended for a gladier.cfg file)
     """
-    return f'{funcx_function.__name__}_funcx_id'
+    return f'{compute_function.__name__}_function_id'
 
 
-def get_funcx_function_checksum_name(funcx_function):
+def get_compute_function_checksum_name(compute_function):
     """
-    Generate a name to refer to the checksum for a given funcx function. Based off of the
-    name generated for the function self.get_funcx_function_name. Human readable, intended
+    Generate a name to refer to the checksum for a given compute function. Based off of the
+    name generated for the function self.get_compute_function_name. Human readable, intended
     for config.
 
     :return:  human readable string identifier for a function checksum (for a gladier.cfg file)
     """
-    return f'{get_funcx_function_name(funcx_function)}_checksum'
+    return f'{get_compute_function_name(compute_function)}_checksum'
```

### Comparing `gladier-0.8.4b1/gladier/utils/tool_alias.py` & `gladier-0.9.0b1/gladier/utils/tool_alias.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4b1/gladier/utils/tool_chain.py` & `gladier-0.9.0b1/gladier/utils/tool_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,17 @@
     def check_tools(self, tools: List[GladierBaseTool]):
 
         states = set()
         for tool in tools:
             flow_def = tool.get_flow_definition()
             if flow_def is None:
                 raise FlowGenException(f'Tool {tool} did not set .flow_definition attribute or set '
-                                       f'@generate_flow_definition (funcx functions only). Please '
-                                       f'set a flow definition for {tool.__class__.__name__}.')
+                                       '@generate_flow_definition (comptue functions only).'
+                                       'Please set a flow definition for'
+                                       f'{tool.__class__.__name__}.')
 
             new_states = set(flow_def.get('States'))
             conflicts = states & new_states
             if conflicts:
                 raise StateNameConflict(f'States in tool {tool} '
                                         f'has been defined more than once: {conflicts}')
             states = states | new_states
```

### Comparing `gladier-0.8.4b1/gladier.egg-info/PKG-INFO` & `gladier-0.9.0b1/gladier.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.8.4b1
+Version: 0.9.0b1
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Gladier: The Globus Architecture for Data-Intensive Experimental Research.
 ==========================================================================
 |docs|
@@ -45,27 +46,15 @@
 Gladier provides a simple software interface to enable researchers to rapidly create, manage, and deploy complex automation flows. It has been used as a programmable data capture, storage, and analysis architecture at experimental facilities including the Argonne Leadership Computing Facility and the Advanced Photon Source. Gladier makes it easy to connect heterogeneous data and computing substrates deployed across distributed compute and storage 
 systems and manage using Globus Flows.
 
 Whether you're working in materials science, X-ray science, automated laboratores, genomics, or any other research field, 
 Gladier can help you streamline your data management and analysis workflows, so you can focus on your scientific discoveries.
 Try Gladier today and see how it can enhance your research capabilities!
 
-
-
-Installation
-============
-
-Gladier requires Python 3.6 and higher. For a modern version of python,
-see the official `Python Installation Guide <https://docs.python-guide.org/starting/installation/>`_.
-
-The easiest way to get Gladier is through Pip on PyPi. Gladier is built with two
-main packages, the core Gladier client and Gladier Tools. Gladier Tools include
-a set of reusable, common operations. Installing it is highly recommended.
-
-With pip installed, you can do the following:
+You can install Gladier and Gladier Tools with the following:
 
 
 .. code-block:: bash
 
    pip install gladier gladier-tools
 
 See the `Read-The-Docs <https://gladier.readthedocs.io/en/stable/?badge=stable>`_ getting started.
```

### Comparing `gladier-0.8.4b1/gladier.egg-info/SOURCES.txt` & `gladier-0.9.0b1/gladier.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 gladier/version.py
 gladier.egg-info/PKG-INFO
 gladier.egg-info/SOURCES.txt
 gladier.egg-info/dependency_links.txt
 gladier.egg-info/requires.txt
 gladier.egg-info/top_level.txt
 gladier/managers/__init__.py
+gladier/managers/compute_login_manager.py
+gladier/managers/compute_manager.py
 gladier/managers/flows_manager.py
-gladier/managers/funcx_manager.py
 gladier/managers/login_manager.py
 gladier/managers/service_manager.py
 gladier/storage/__init__.py
 gladier/storage/config.py
 gladier/storage/migrations.py
 gladier/storage/tokens.py
 gladier/utils/__init__.py
 gladier/utils/automate.py
 gladier/utils/dynamic_imports.py
 gladier/utils/flow_generation.py
 gladier/utils/flow_modifiers.py
 gladier/utils/flow_traversal.py
-gladier/utils/funcx_login_manager.py
 gladier/utils/name_generation.py
 gladier/utils/tool_alias.py
 gladier/utils/tool_chain.py
```

### Comparing `gladier-0.8.4b1/setup.py` & `gladier-0.9.0b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,9 +39,10 @@
         'Operating System :: MacOS :: MacOS X',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ]
 )
```

