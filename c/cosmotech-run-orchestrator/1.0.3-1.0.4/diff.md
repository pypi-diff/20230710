# Comparing `tmp/cosmotech-run-orchestrator-1.0.3.tar.gz` & `tmp/cosmotech-run-orchestrator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-run-orchestrator-1.0.3.tar", last modified: Fri Jul  7 09:44:02 2023, max compression
+gzip compressed data, was "cosmotech-run-orchestrator-1.0.4.tar", last modified: Mon Jul 10 12:20:59 2023, max compression
```

## Comparing `cosmotech-run-orchestrator-1.0.3.tar` & `cosmotech-run-orchestrator-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.065537 cosmotech-run-orchestrator-1.0.3/cosmotech/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.065537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/parameters_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/command_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/schema/run_template_json_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:44:01.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.470696 cosmotech-run-orchestrator-1.0.4/cosmotech/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.470696 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20143 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/parameters_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/command_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/schema/run_template_json_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 12:20:59.000000 cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:20:59.474696 cosmotech-run-orchestrator-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/tests/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-10 12:20:50.000000 cosmotech-run-orchestrator-1.0.4/tests/test_template.py
```

### Comparing `cosmotech-run-orchestrator-1.0.3/LICENSE` & `cosmotech-run-orchestrator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from azure.kusto.ingest import FileDescriptor
 from azure.kusto.ingest import IngestionMappingKind
 from azure.kusto.ingest import IngestionProperties
 from azure.kusto.ingest import IngestionResult
 from azure.kusto.ingest import ReportLevel
 
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.command()
 @click.option("--dataset-absolute-path",
               envvar="CSM_DATASET_ABSOLUTE_PATH",
               show_envvar=True,
@@ -76,14 +77,15 @@
               help="whether or not to send datasets (parameters path is mandatory then)")
 @click.option("--wait/--no-wait",
               envvar="WAIT_FOR_INGESTION",
               show_envvar=True,
               default=False,
               show_default=True,
               help="Toggle waiting for the ingestion results")
+@web_help("commands/simulation_to_adx")
 def main(
     send_parameters: bool,
     send_datasets: bool,
     dataset_absolute_path: str,
     parameters_absolute_path: str,
     simulation_id: str,
     adx_uri: str,
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/download_cloud_steps.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/download_cloud_steps.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from azure.identity import DefaultAzureCredential
 from cosmotech_api.api.solution_api import SolutionApi
 from cosmotech_api.api.workspace_api import Workspace
 from cosmotech_api.api.workspace_api import WorkspaceApi
 from cosmotech_api.exceptions import ServiceException
 
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.command()
 @click.option("--organization-id",
               envvar="CSM_ORGANIZATION_ID",
               show_envvar=True,
@@ -53,14 +54,15 @@
               required=True)
 @click.option("--api-scope",
               envvar="CSM_API_SCOPE",
               show_envvar=True,
               help="The identification scope of a Cosmotech API",
               metavar="URI",
               required=True)
+@web_help("commands/download_cloud_steps")
 def main(workspace_id, organization_id, run_template_id, handler_list, api_scope, api_url):
     """
 Uses environment variables to download cloud based Template steps
 Requires a valid Azure connection either with:
 - The AZ cli command: **az login**
 - A triplet of env var `AZURE_TENANT_ID`, `AZURE_CLIENT_ID`, `AZURE_CLIENT_SECRET`
     """
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/legacy_json_generator.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/legacy_json_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 from cosmotech_api.api.solution_api import Solution
 
 from cosmotech.orchestrator.core.orchestrator import Orchestrator
 from cosmotech.orchestrator.core.step import Step
 from cosmotech.orchestrator.utils.api import get_solution
 from cosmotech.orchestrator.utils.api import read_solution_file
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.json import CustomJSONEncoder
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.group()
+@web_help("commands/legacy_json_generator")
 def main():
     """Base command for the json generator using legacy files  
 Check the help of the sub commands for more information:  
 - `cloud` requires access to a fully deployed solution  
 - `solution` requires a `Solution.yaml` file"""
     pass
 
@@ -38,14 +40,15 @@
                 required=True,
                 nargs=1)
 @click.argument("run-template-id",
                 required=True)
 @click.option("--describe/--no-describe",
               show_default=True, default=False,
               help="Show a description of the generated template after generation")
+@web_help("commands/legacy_json_generator")
 def solution(solution_file, run_template_id, output, describe):
     """Read SOLUTION_FILE to get a RUN_TEMPLATE_ID and generate an orchestrator file at OUTPUT"""
     if _solution := read_solution_file(solution_file):
         return generate_from_solution(sol=_solution, run_template_id=run_template_id, output=output, describe=describe)
     return 1
 
 
@@ -83,14 +86,15 @@
               show_envvar=True,
               help="The name of the run template in the cosmotech api",
               metavar="NAME",
               required=True)
 @click.option("--describe/--no-describe",
               show_default=True, default=False,
               help="Show a description of the generated template after generation")
+@web_help("commands/legacy_json_generator")
 def cloud(workspace_id, organization_id, run_template_id, api_scope, api_url, output, describe):
     """Connect to the cosmotech API to download a run template and generate an orchestrator file at OUTPUT"""
 
     if sol := get_solution(api_scope=api_scope,
                            api_url=api_url,
                            organization_id=organization_id,
                            workspace_id=workspace_id):
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/main.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 from cosmotech.orchestrator.console_scripts.download_cloud_steps import main as dl_cloud_cmd
 from cosmotech.orchestrator.console_scripts.legacy_json_generator import main as legacy_gen_cmd
 from cosmotech.orchestrator.console_scripts.orchestrator import main as orchestrator_cmd
 from cosmotech.orchestrator.console_scripts.parameters_generation import main as parameters_cmd
 from cosmotech.orchestrator.console_scripts.run_step import main as run_cmd
 from cosmotech.orchestrator.console_scripts.scenario_data_downloader import main as scenario_dl_cmd
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.group("csm-run-orchestrator")
 @click_log.simple_verbosity_option(LOGGER,
                                    "--log-level",
                                    envvar="LOG_LEVEL",
                                    show_envvar=True)
+@web_help(None)
 def main():
     """Cosmotech Run Orchestrator
     
 Command toolkit allowing to run Cosmotech Run Templates"""
     pass
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/orchestrator.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # specifically authorized by written means by Cosmo Tech.
 
 import pathlib
 from typing import Optional
 
 from cosmotech.orchestrator.core.orchestrator import Orchestrator
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.command()
 @click.argument("template", type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True), nargs=1)
 @click.option("--dry-run/--no-dry-run", "-n",
               envvar="DRY_RUN",
@@ -38,14 +39,15 @@
               envvar="CSM_SKIP_STEPS",
               show_envvar=True,
               default=[],
               type=str,
               multiple=True,
               metavar="STEP_ID",
               help="Define a list of steps to be skipped during this run")
+@web_help("commands/orchestrator")
 def main(template: str, dry_run: bool, display_env: bool, gen_env_target: Optional[str], skipped_steps: list[str]):
     """Runs the given `TEMPLATE` file  
 Commands are run as subprocess using `bash -c "<command> <arguments>"`.  
 In case you are in a python venv, the venv is activated before any command is run."""
     f = Orchestrator()
     try:
         c, s, g = f.load_json_file(template, dry_run, display_env, skipped_steps)
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/parameters_generation.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/parameters_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 from cosmotech_api.api.solution_api import RunTemplate
 from cosmotech_api.api.solution_api import Solution
 
 from cosmotech.orchestrator.console_scripts.scenario_data_downloader import write_parameters
 from cosmotech.orchestrator.utils.api import get_solution
 from cosmotech.orchestrator.utils.api import read_solution_file
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.group()
+@web_help("commands/parameters_generator")
 def main():
     """Base command to initialize parameter folders  
 Will create:    
 - A `parameters.json`/`parameters.csv` in the folder with all parameters  
 - A folder per `%DATASETID%` datasets with the name of the parameter  
 Check the help of the sub commands for more information:  
 - `cloud` requires access to a fully deployed solution  
@@ -49,14 +51,15 @@
               help="Toggle writing of parameters in json format")
 @click.option("--write-csv/--no-write-csv",
               envvar="WRITE_CSV",
               show_envvar=True,
               default=True,
               show_default=True,
               help="Toggle writing of parameters in csv format")
+@web_help("commands/parameters_generator")
 def solution(
     solution_file: str,
     run_template_id: str,
     output_folder: str,
     write_json: bool,
     write_csv: bool
 ):
@@ -110,14 +113,15 @@
               help="Toggle writing of parameters in json format")
 @click.option("--write-csv/--no-write-csv",
               envvar="WRITE_CSV",
               show_envvar=True,
               default=True,
               show_default=True,
               help="Toggle writing of parameters in csv format")
+@web_help("commands/parameters_generator")
 def cloud(
     workspace_id: str,
     organization_id: str,
     run_template_id: str,
     api_scope: str,
     api_url: str,
     output_folder: str,
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/run_step.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/run_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import os
 import pathlib
 import subprocess
 import sys
 import venv
 
 from cosmotech.orchestrator.utils.click import click
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 @click.command()
 @click.option("--template",
               envvar="CSM_RUN_TEMPLATE_ID",
               required=True,
@@ -25,14 +26,15 @@
               envvar="CSM_CONTAINER_MODE",
               default="CSMDOCKER",
               show_envvar=True,
               show_default=True,
               help="\bA list of Steps definer in the `TEMPLATE` folder that will be executed (comma-separated).  \n"
                    "Defaults to `CSMDOCKER` equivalent to "
                    "`parameters_handler,validator,prerun,engine,postrun` (the legacy order)")
+@web_help("commands/run_step")
 def main(template: str, steps: str):
     """Runs a list of steps of a run template in a CosmoTech project
 Known limitations:
 - The step MUST contain an executable main.py file
 - The engine step requires to set the env var CSM_SIMULATION if you have a run without a python engine
 """
     project = pathlib.Path(".")
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from csv import DictWriter
 from distutils.dir_util import copy_tree
 
 from CosmoTech_Acceleration_Library.Accelerators.scenario_download.scenario_downloader import ScenarioDownloader
 
 from cosmotech.orchestrator.utils.click import click
 from cosmotech.orchestrator.utils.decorators import require_env
+from cosmotech.orchestrator.utils.decorators import web_help
 from cosmotech.orchestrator.utils.logger import LOGGER
 
 
 def download_scenario_data(
     organization_id: str,
     workspace_id: str,
     scenario_id: str,
@@ -158,14 +159,15 @@
               envvar="FETCH_DATASET",
               show_envvar=True,
               default=True,
               show_default=True,
               help="Toggle fetching datasets")
 @require_env('CSM_API_SCOPE', "The identification scope of a Cosmotech API")
 @require_env('CSM_API_URL', "The URL to a Cosmotech API")
+@web_help("commands/scenario_data_downloader")
 def main(
     scenario_id: str,
     workspace_id: str,
     organization_id: str,
     dataset_absolute_path: str,
     parameters_absolute_path: str,
     write_json: bool,
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/command_template.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/command_template.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/environment.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/environment.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/orchestrator.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,26 @@
     def load_json_file(
         self, json_file_path,
         dry: bool = False,
         display_env: bool = False,
         skipped_steps: list[str] = ()
     ):
         _path = pathlib.Path(json_file_path)
+        _run_content = json.load(open(_path))
+        return self._load_from_json_content(json_file_path, _run_content, dry, display_env, skipped_steps)
+
+    def _load_from_json_content(
+        self, json_file_path, _run_content,
+        dry: bool = False,
+        display_env: bool = False,
+        skipped_steps: list[str] = ()
+    ):
         g = flowpipe.Graph(name=json_file_path)
         steps: dict[str, (Step, flowpipe.Node)] = dict()
         commands: dict[str, CommandTemplate] = dict()
-        _run_content = json.load(open(_path))
         schema_path = pathlib.Path(__file__).parent.parent / "schema/run_template_json_schema.json"
         schema = json.load(open(schema_path))
         jsonschema.validate(_run_content, schema)
         for tmpl in _run_content.get("commandTemplates", list()):
             self.load_command(commands, **tmpl)
         for step in _run_content.get("steps", list()):
             id = step.get('id')
```

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/runner.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/runner.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/step.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/core/step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/schema/run_template_json_schema.json` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/schema/run_template_json_schema.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/api.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/api.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/click.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/click.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/json.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/logger.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/singleton.py` & `cosmotech-run-orchestrator-1.0.4/cosmotech/orchestrator/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/SOURCES.txt` & `cosmotech-run-orchestrator-1.0.4/cosmotech_run_orchestrator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,8 +28,12 @@
 cosmotech/orchestrator/utils/singleton.py
 cosmotech_run_orchestrator.egg-info/PKG-INFO
 cosmotech_run_orchestrator.egg-info/SOURCES.txt
 cosmotech_run_orchestrator.egg-info/dependency_links.txt
 cosmotech_run_orchestrator.egg-info/entry_points.txt
 cosmotech_run_orchestrator.egg-info/not-zip-safe
 cosmotech_run_orchestrator.egg-info/requires.txt
-cosmotech_run_orchestrator.egg-info/top_level.txt
+cosmotech_run_orchestrator.egg-info/top_level.txt
+tests/test_environment.py
+tests/test_orchestrator.py
+tests/test_step.py
+tests/test_template.py
```

### Comparing `cosmotech-run-orchestrator-1.0.3/setup.py` & `cosmotech-run-orchestrator-1.0.4/setup.py`

 * *Files identical despite different names*

