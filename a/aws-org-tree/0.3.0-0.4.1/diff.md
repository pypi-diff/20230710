# Comparing `tmp/aws_org_tree-0.3.0.tar.gz` & `tmp/aws_org_tree-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_org_tree-0.3.0.tar", max compression
+gzip compressed data, was "aws_org_tree-0.4.1.tar", max compression
```

## Comparing `aws_org_tree-0.3.0.tar` & `aws_org_tree-0.4.1.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     1272 2023-06-09 15:25:58.611128 aws_org_tree-0.3.0/README.md
--rw-r--r--   0        0        0     7305 2023-06-09 15:09:48.414050 aws_org_tree-0.3.0/aws_org_tree.py
--rw-r--r--   0        0        0     1368 2023-06-09 15:31:21.718985 aws_org_tree-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 aws_org_tree-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-07-10 00:01:18.490382 aws_org_tree-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 00:01:18.490382 aws_org_tree-0.4.1/aws_org_tree/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-10 00:01:18.490382 aws_org_tree-0.4.1/aws_org_tree/__main__.py
+-rw-r--r--   0        0        0     7434 2023-07-10 00:01:18.490382 aws_org_tree-0.4.1/aws_org_tree/aws_org_tree.py
+-rw-r--r--   0        0        0     1461 2023-07-10 00:01:18.490382 aws_org_tree-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 aws_org_tree-0.4.1/PKG-INFO
```

### Comparing `aws_org_tree-0.3.0/README.md` & `aws_org_tree-0.4.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,32 @@
 ├── ACCOUNT iain+awsroot+zcskbx@isme.es
 ├── ORGANIZATIONAL_UNIT Email
 └── ORGANIZATIONAL_UNIT Email
     ├── ACCOUNT iain+awsroot+zcskbx+log-archive@isme.es
     └── ACCOUNT iain+awsroot+zcskbx+audit@isme.es
 ```
 
-## TODO
-
-* Use [orgtreepubsub](https://github.com/iainelder/orgtreepubsub) to crawl the org and model the resources
-* Allow templating to pull out all attributes of all resources
-
 ## Other formats
 
 I removed the JSON tree (`json-tree`) and flat JSON formats (`json-flat`) formats Use [version `0.2.0`](https://github.com/iainelder/aws-org-tree/tree/0.2.0) if you need those.
+
+## Development
+
+Install Python 3.8.
+
+Install [Poetry](https://python-poetry.org/) via [Pipx](https://pypa.github.io/pipx/).
+
+Clone the repo.
+
+Run `poetry install`.
+
+Hack away.
+
+Run quality checks with `poetry run pre-commit run --all-files`.
+
+Install quality checks as [pre-commit checks](https://pre-commit.com/) with `poetry run pre-commit install`.
+
+## Continuous integration
+
+Push to the main branch to run the development quality checks via GitHub Actions.
+
+Run continuous integration locally with [act](https://github.com/nektos/act).
```

### Comparing `aws_org_tree-0.3.0/aws_org_tree.py` & `aws_org_tree-0.4.1/aws_org_tree/aws_org_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import json
 import logging
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Mapping, Optional, Protocol, TypeVar, Union
+from importlib.metadata import version
 
 import anytree
 import anytree.exporter
 import logdecorator
 from anytree import LevelOrderIter
 from boto3.session import Session
 from mypy_boto3_organizations.client import OrganizationsClient
@@ -29,14 +30,15 @@
         self.add_argument(
             "--tree-format",
             default="text-tree",
             choices=["json-flat", "json-tree", "text-tree"],
         )
         self.add_argument("--node-name-format", default="{Name} ({Id})")
         self.add_argument("--log-level", default="WARNING")
+        self.add_argument("--version", action="version", version=version("aws-org-tree"))
 
 
 class OrgTreeArgs(Namespace):
     tree_format: str
     node_name_format: str
     log_level: str
```

### Comparing `aws_org_tree-0.3.0/pyproject.toml` & `aws_org_tree-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "aws-org-tree"
-version = "0.3.0"
+version = "0.4.1"
 description = ""
 authors = ["Iain Samuel McLean Elder <iain@isme.es>"]
 readme = "README.md"
 repository = "https://github.com/iainelder/aws-org-tree"
+packages = [{include = "aws_org_tree"}]
 
 [tool.poetry.scripts]
-aws-org-tree = "aws_org_tree:main"
+aws-org-tree = "aws_org_tree.aws_org_tree:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 boto3 = "^1.18.50"
 anytree = "^2.8.0"
 logdecorator = "^2.2"
 networkx = "^2.8"
@@ -33,24 +34,25 @@
 pytest-mock = "^3.7.0"
 mypy = "^0.942"
 black = "^22.3.0"
 isort = "^5.10.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
+cli-test-helpers = "^3.4.0"
+pytest = "^7.3.2"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
-files = "aws_org_tree.py"
 strict = true
 # Logdecorator uses untyped decorators.
 disallow_untyped_decorators = false
 
 [[tool.mypy.overrides]]
-module = ["logdecorator", "anytree", "anytree.exporter"]
+module = ["logdecorator", "anytree", "anytree.exporter", "cli_test_helpers"]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aws_org_tree-0.3.0/PKG-INFO` & `aws_org_tree-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-org-tree
-Version: 0.3.0
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/iainelder/aws-org-tree
 Author: Iain Samuel McLean Elder
 Author-email: iain@isme.es
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -50,16 +50,33 @@
 ├── ACCOUNT iain+awsroot+zcskbx@isme.es
 ├── ORGANIZATIONAL_UNIT Email
 └── ORGANIZATIONAL_UNIT Email
     ├── ACCOUNT iain+awsroot+zcskbx+log-archive@isme.es
     └── ACCOUNT iain+awsroot+zcskbx+audit@isme.es
 ```
 
-## TODO
-
-* Use [orgtreepubsub](https://github.com/iainelder/orgtreepubsub) to crawl the org and model the resources
-* Allow templating to pull out all attributes of all resources
-
 ## Other formats
 
 I removed the JSON tree (`json-tree`) and flat JSON formats (`json-flat`) formats Use [version `0.2.0`](https://github.com/iainelder/aws-org-tree/tree/0.2.0) if you need those.
 
+## Development
+
+Install Python 3.8.
+
+Install [Poetry](https://python-poetry.org/) via [Pipx](https://pypa.github.io/pipx/).
+
+Clone the repo.
+
+Run `poetry install`.
+
+Hack away.
+
+Run quality checks with `poetry run pre-commit run --all-files`.
+
+Install quality checks as [pre-commit checks](https://pre-commit.com/) with `poetry run pre-commit install`.
+
+## Continuous integration
+
+Push to the main branch to run the development quality checks via GitHub Actions.
+
+Run continuous integration locally with [act](https://github.com/nektos/act).
+
```

