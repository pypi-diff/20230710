# Comparing `tmp/volttron_actuator-0.1.1a6.tar.gz` & `tmp/volttron_actuator-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_actuator-0.1.1a6.tar", max compression
+gzip compressed data, was "volttron_actuator-0.1.1a7.tar", max compression
```

## Comparing `volttron_actuator-0.1.1a6.tar` & `volttron_actuator-0.1.1a7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11927 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/LICENSE
--rw-r--r--   0        0        0     1830 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/README.md
--rw-r--r--   0        0        0     1910 2023-06-12 17:05:50.085291 volttron_actuator-0.1.1a6/pyproject.toml
--rw-r--r--   0        0        0     1570 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/src/actuator/__init__.py
--rw-r--r--   0        0        0    52552 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/src/actuator/agent.py
--rw-r--r--   0        0        0    16122 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/src/actuator/scheduler.py
--rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a6/setup.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a6/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-10 16:39:51.230102 volttron_actuator-0.1.1a7/LICENSE
+-rw-r--r--   0        0        0     1830 2023-07-10 16:39:51.230102 volttron_actuator-0.1.1a7/README.md
+-rw-r--r--   0        0        0     1911 2023-07-10 16:42:51.533458 volttron_actuator-0.1.1a7/pyproject.toml
+-rw-r--r--   0        0        0     1570 2023-07-10 16:39:51.230102 volttron_actuator-0.1.1a7/src/actuator/__init__.py
+-rw-r--r--   0        0        0    52552 2023-07-10 16:39:51.234102 volttron_actuator-0.1.1a7/src/actuator/agent.py
+-rw-r--r--   0        0        0    16122 2023-07-10 16:39:51.234102 volttron_actuator-0.1.1a7/src/actuator/scheduler.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a7/setup.py
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a7/PKG-INFO
```

### Comparing `volttron_actuator-0.1.1a6/LICENSE` & `volttron_actuator-0.1.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a6/README.md` & `volttron_actuator-0.1.1a7/README.md`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a6/pyproject.toml` & `volttron_actuator-0.1.1a7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-actuator"
-version = "0.1.1a6"
+version = "0.1.1a7"
 description = "The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-actuator"
 homepage = "https://github.com/VOLTTRON/volttron-actuator"
 keywords = []
@@ -35,15 +35,15 @@
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 tzlocal = "^4.2"
-volttron = ">=10.0.rc0,<11.0"
+volttron = ">=10.0.4rc1,<11.0"
 types-tzlocal = "^4.2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.4.0rc0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
```

### Comparing `volttron_actuator-0.1.1a6/src/actuator/__init__.py` & `volttron_actuator-0.1.1a7/src/actuator/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a6/src/actuator/agent.py` & `volttron_actuator-0.1.1a7/src/actuator/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a6/src/actuator/scheduler.py` & `volttron_actuator-0.1.1a7/src/actuator/scheduler.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a6/setup.py` & `volttron_actuator-0.1.1a7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['types-tzlocal>=4.2.2.2,<5.0.0.0',
  'tzlocal>=4.2,<5.0',
- 'volttron>=10.0.rc0,<11.0']
+ 'volttron>=10.0.4rc1,<11.0']
 
 entry_points = \
 {'console_scripts': ['volttron-actuator = actuator.agent:main']}
 
 setup_kwargs = {
     'name': 'volttron-actuator',
-    'version': '0.1.1a6',
+    'version': '0.1.1a7',
     'description': 'The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.',
     'long_description': '# volttron-actuator\n\n![Eclipse VOLTTRON 10.0.4rc](https://img.shields.io/badge/Eclipse%20VOLTTRON-10.0.4rc-red.svg)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Passing?](https://github.com/eclipse-volttron/volttron-actuator/actions/workflows/run-tests.yml/badge.svg)](https://github.com/VOLTTRON/volttron-actuator/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-actuator.svg)](https://pypi.org/project/volttron-actuator/)\n\n\nThe Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.\n\n## Requirements\n\n* python >= 3.10\n* volttron >= 10.0\n* tzlocal >= 4.2\n* types-tzlocal >= 4.2.2.2\n\n## Documentation\n\nMore detailed documentation can be found on [ReadTheDocs](https://volttron.readthedocs.io/en/modular/). The RST source\nof the documentation for this component is located in the "docs" directory of this repository.\n\n## Installation\n\nBefore installing, VOLTTRON should be installed and running.  Its virtual environment should be active.\nInformation on how to install of the VOLTTRON platform can be found\n[here](https://github.com/eclipse-volttron/volttron-core).\n\nInstall and start the volttron-actuator.\n\n```shell\nvctl install volttron-actuator --agent-config <path to agent config> --start\n```\n\nView the status of the installed agent\n\n```shell\nvctl status\n```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n',
     'author': 'Mark Bonicillo',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/VOLTTRON/volttron-actuator',
```

### Comparing `volttron_actuator-0.1.1a6/PKG-INFO` & `volttron_actuator-0.1.1a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-actuator
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.
 Home-page: https://github.com/VOLTTRON/volttron-actuator
 License: Apache-2.0
 Author: Mark Bonicillo
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: types-tzlocal (>=4.2.2.2,<5.0.0.0)
 Requires-Dist: tzlocal (>=4.2,<5.0)
-Requires-Dist: volttron (>=10.0.rc0,<11.0)
+Requires-Dist: volttron (>=10.0.4rc1,<11.0)
 Project-URL: Repository, https://github.com/VOLTTRON/volttron-actuator
 Description-Content-Type: text/markdown
 
 # volttron-actuator
 
 ![Eclipse VOLTTRON 10.0.4rc](https://img.shields.io/badge/Eclipse%20VOLTTRON-10.0.4rc-red.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
```

