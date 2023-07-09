# Comparing `tmp/canarypy-0.0.13-py3-none-any.whl.zip` & `tmp/canarypy-0.0.14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,47 +1,66 @@
-Zip file size: 25325 bytes, number of entries: 45
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/__init__.py
--rw-r--r--  2.0 unx     2163 b- defN 23-Jul-02 18:37 canarypy/client.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-02 18:37 canarypy/api/__init__.py
--rw-r--r--  2.0 unx      539 b- defN 23-Jul-02 18:37 canarypy/api/config.py
--rw-r--r--  2.0 unx      558 b- defN 23-Jul-02 18:37 canarypy/api/main.py
--rw-r--r--  2.0 unx      561 b- defN 23-Jul-02 18:37 canarypy/api/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/api/db/__init__.py
--rw-r--r--  2.0 unx      370 b- defN 23-Jul-02 18:37 canarypy/api/db/base.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/api/dependencies/__init__.py
--rw-r--r--  2.0 unx      305 b- defN 23-Jul-02 18:37 canarypy/api/dependencies/db.py
--rw-r--r--  2.0 unx       85 b- defN 23-Jul-02 18:37 canarypy/api/models/__init__.py
--rw-r--r--  2.0 unx      621 b- defN 23-Jul-02 18:37 canarypy/api/models/product.py
--rw-r--r--  2.0 unx     4593 b- defN 23-Jul-02 18:37 canarypy/api/models/release.py
--rw-r--r--  2.0 unx     1055 b- defN 23-Jul-02 18:37 canarypy/api/models/signal.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/api/routes/__init__.py
--rw-r--r--  2.0 unx     2185 b- defN 23-Jul-02 18:37 canarypy/api/routes/product.py
--rw-r--r--  2.0 unx     1726 b- defN 23-Jul-02 18:37 canarypy/api/routes/release.py
--rw-r--r--  2.0 unx     1028 b- defN 23-Jul-02 18:37 canarypy/api/routes/signal.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/api/schemas/__init__.py
--rw-r--r--  2.0 unx       77 b- defN 23-Jul-02 18:37 canarypy/api/schemas/httperror.py
--rw-r--r--  2.0 unx      249 b- defN 23-Jul-02 18:37 canarypy/api/schemas/product.py
--rw-r--r--  2.0 unx      764 b- defN 23-Jul-02 18:37 canarypy/api/schemas/release.py
--rw-r--r--  2.0 unx      292 b- defN 23-Jul-02 18:37 canarypy/api/schemas/signal.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/api/services/__init__.py
--rw-r--r--  2.0 unx     1592 b- defN 23-Jul-02 18:37 canarypy/api/services/product.py
--rw-r--r--  2.0 unx    10214 b- defN 23-Jul-02 18:37 canarypy/api/services/release.py
--rw-r--r--  2.0 unx     3680 b- defN 23-Jul-02 18:37 canarypy/api/services/signal.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/cli/__init__.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Jul-02 18:37 canarypy/cli/main.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/cli/services/__init__.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Jul-02 18:37 canarypy/cli/services/product.py
--rw-r--r--  2.0 unx     1557 b- defN 23-Jul-02 18:37 canarypy/cli/services/release.py
--rw-r--r--  2.0 unx      875 b- defN 23-Jul-02 18:37 canarypy/cli/services/signal.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/web/__init__.py
--rw-r--r--  2.0 unx      485 b- defN 23-Jul-02 18:37 canarypy/web/app.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/web/services/__init__.py
--rw-r--r--  2.0 unx     2479 b- defN 23-Jul-02 18:37 canarypy/web/services/release.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 18:37 canarypy/web/views/__init__.py
--rw-r--r--  2.0 unx     6145 b- defN 23-Jul-02 18:37 canarypy/web/views/release.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jul-02 18:37 canarypy-0.0.13.dist-info/LICENSE
--rw-r--r--  2.0 unx     9507 b- defN 23-Jul-02 18:37 canarypy-0.0.13.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 18:37 canarypy-0.0.13.dist-info/WHEEL
--rw-r--r--  2.0 unx       70 b- defN 23-Jul-02 18:37 canarypy-0.0.13.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-02 18:37 canarypy-0.0.13.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3771 b- defN 23-Jul-02 18:37 canarypy-0.0.13.dist-info/RECORD
-45 files, 62497 bytes uncompressed, 19251 bytes compressed:  69.2%
+Zip file size: 38544 bytes, number of entries: 64
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/__init__.py
+-rw-r--r--  2.0 unx     2891 b- defN 23-Jul-09 22:33 canarypy/alembic.ini
+-rw-r--r--  2.0 unx     2163 b- defN 23-Jul-09 22:33 canarypy/client.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jul-09 22:33 canarypy/config.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-09 22:33 canarypy/api/__init__.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Jul-09 22:33 canarypy/api/config.py
+-rw-r--r--  2.0 unx      558 b- defN 23-Jul-09 22:33 canarypy/api/main.py
+-rw-r--r--  2.0 unx      561 b- defN 23-Jul-09 22:33 canarypy/api/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/api/db/__init__.py
+-rw-r--r--  2.0 unx      370 b- defN 23-Jul-09 22:33 canarypy/api/db/base.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/api/dependencies/__init__.py
+-rw-r--r--  2.0 unx      305 b- defN 23-Jul-09 22:33 canarypy/api/dependencies/db.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Jul-09 22:33 canarypy/api/models/__init__.py
+-rw-r--r--  2.0 unx      621 b- defN 23-Jul-09 22:33 canarypy/api/models/product.py
+-rw-r--r--  2.0 unx     4593 b- defN 23-Jul-09 22:33 canarypy/api/models/release.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jul-09 22:33 canarypy/api/models/signal.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/api/routes/__init__.py
+-rw-r--r--  2.0 unx     2185 b- defN 23-Jul-09 22:33 canarypy/api/routes/product.py
+-rw-r--r--  2.0 unx     1726 b- defN 23-Jul-09 22:33 canarypy/api/routes/release.py
+-rw-r--r--  2.0 unx     1028 b- defN 23-Jul-09 22:33 canarypy/api/routes/signal.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/api/schemas/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-09 22:33 canarypy/api/schemas/httperror.py
+-rw-r--r--  2.0 unx      249 b- defN 23-Jul-09 22:33 canarypy/api/schemas/product.py
+-rw-r--r--  2.0 unx      764 b- defN 23-Jul-09 22:33 canarypy/api/schemas/release.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-09 22:33 canarypy/api/schemas/signal.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/api/services/__init__.py
+-rw-r--r--  2.0 unx     1592 b- defN 23-Jul-09 22:33 canarypy/api/services/product.py
+-rw-r--r--  2.0 unx    10214 b- defN 23-Jul-09 22:33 canarypy/api/services/release.py
+-rw-r--r--  2.0 unx     3680 b- defN 23-Jul-09 22:33 canarypy/api/services/signal.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/cli/__init__.py
+-rw-r--r--  2.0 unx     2752 b- defN 23-Jul-09 22:33 canarypy/cli/main.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/cli/services/__init__.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Jul-09 22:33 canarypy/cli/services/product.py
+-rw-r--r--  2.0 unx     1557 b- defN 23-Jul-09 22:33 canarypy/cli/services/release.py
+-rw-r--r--  2.0 unx      875 b- defN 23-Jul-09 22:33 canarypy/cli/services/signal.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 22:33 canarypy/migrations/README
+-rw-r--r--  2.0 unx     2422 b- defN 23-Jul-09 22:33 canarypy/migrations/env.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Jul-09 22:33 canarypy/migrations/script.py.mako
+-rw-r--r--  2.0 unx      703 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/1c26034449b9_add_band_number.py
+-rw-r--r--  2.0 unx      880 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/33873c5a7bbe_change_canary_period_type.py
+-rw-r--r--  2.0 unx     1910 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/4a95c3cf7adc_initial_tables.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/5a588045e274_add_release_date.py
+-rw-r--r--  2.0 unx      668 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/652e9c47c653_add_is_canary_to_signal.py
+-rw-r--r--  2.0 unx     1553 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/67c9708da025_add_release_canary_band_table.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/738957fcc3bc_add_signal_period_column.py
+-rw-r--r--  2.0 unx      797 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/84a61d063ad6_add_release_status_columns.py
+-rw-r--r--  2.0 unx      880 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/9261790e46ac_change_canary_period_type.py
+-rw-r--r--  2.0 unx     1046 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/9505cfab1f85_refactor_bands.py
+-rw-r--r--  2.0 unx      805 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/9dbfd3ac874b_add_release_period_columns.py
+-rw-r--r--  2.0 unx      873 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/aebc398fc592_change_mandatory_field.py
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/d1b816f53004_change_product_name.py
+-rw-r--r--  2.0 unx      858 b- defN 23-Jul-09 22:33 canarypy/migrations/versions/ea0d1d149192_change_status_field.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/web/__init__.py
+-rw-r--r--  2.0 unx      485 b- defN 23-Jul-09 22:33 canarypy/web/app.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/web/services/__init__.py
+-rw-r--r--  2.0 unx     2479 b- defN 23-Jul-09 22:33 canarypy/web/services/release.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 22:33 canarypy/web/views/__init__.py
+-rw-r--r--  2.0 unx     6145 b- defN 23-Jul-09 22:33 canarypy/web/views/release.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-09 22:33 canarypy-0.0.14.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10446 b- defN 23-Jul-09 22:33 canarypy-0.0.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 22:33 canarypy-0.0.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx       70 b- defN 23-Jul-09 22:33 canarypy-0.0.14.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 22:33 canarypy-0.0.14.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5892 b- defN 23-Jul-09 22:33 canarypy-0.0.14.dist-info/RECORD
+64 files, 84970 bytes uncompressed, 28924 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
 Filename: canarypy/__init__.py
 Comment: 
 
+Filename: canarypy/alembic.ini
+Comment: 
+
 Filename: canarypy/client.py
 Comment: 
 
+Filename: canarypy/config.py
+Comment: 
+
 Filename: canarypy/api/__init__.py
 Comment: 
 
 Filename: canarypy/api/config.py
 Comment: 
 
 Filename: canarypy/api/main.py
@@ -93,14 +99,65 @@
 
 Filename: canarypy/cli/services/release.py
 Comment: 
 
 Filename: canarypy/cli/services/signal.py
 Comment: 
 
+Filename: canarypy/migrations/README
+Comment: 
+
+Filename: canarypy/migrations/env.py
+Comment: 
+
+Filename: canarypy/migrations/script.py.mako
+Comment: 
+
+Filename: canarypy/migrations/versions/1c26034449b9_add_band_number.py
+Comment: 
+
+Filename: canarypy/migrations/versions/33873c5a7bbe_change_canary_period_type.py
+Comment: 
+
+Filename: canarypy/migrations/versions/4a95c3cf7adc_initial_tables.py
+Comment: 
+
+Filename: canarypy/migrations/versions/5a588045e274_add_release_date.py
+Comment: 
+
+Filename: canarypy/migrations/versions/652e9c47c653_add_is_canary_to_signal.py
+Comment: 
+
+Filename: canarypy/migrations/versions/67c9708da025_add_release_canary_band_table.py
+Comment: 
+
+Filename: canarypy/migrations/versions/738957fcc3bc_add_signal_period_column.py
+Comment: 
+
+Filename: canarypy/migrations/versions/84a61d063ad6_add_release_status_columns.py
+Comment: 
+
+Filename: canarypy/migrations/versions/9261790e46ac_change_canary_period_type.py
+Comment: 
+
+Filename: canarypy/migrations/versions/9505cfab1f85_refactor_bands.py
+Comment: 
+
+Filename: canarypy/migrations/versions/9dbfd3ac874b_add_release_period_columns.py
+Comment: 
+
+Filename: canarypy/migrations/versions/aebc398fc592_change_mandatory_field.py
+Comment: 
+
+Filename: canarypy/migrations/versions/d1b816f53004_change_product_name.py
+Comment: 
+
+Filename: canarypy/migrations/versions/ea0d1d149192_change_status_field.py
+Comment: 
+
 Filename: canarypy/web/__init__.py
 Comment: 
 
 Filename: canarypy/web/app.py
 Comment: 
 
 Filename: canarypy/web/services/__init__.py
@@ -111,26 +168,26 @@
 
 Filename: canarypy/web/views/__init__.py
 Comment: 
 
 Filename: canarypy/web/views/release.py
 Comment: 
 
-Filename: canarypy-0.0.13.dist-info/LICENSE
+Filename: canarypy-0.0.14.dist-info/LICENSE
 Comment: 
 
-Filename: canarypy-0.0.13.dist-info/METADATA
+Filename: canarypy-0.0.14.dist-info/METADATA
 Comment: 
 
-Filename: canarypy-0.0.13.dist-info/WHEEL
+Filename: canarypy-0.0.14.dist-info/WHEEL
 Comment: 
 
-Filename: canarypy-0.0.13.dist-info/entry_points.txt
+Filename: canarypy-0.0.14.dist-info/entry_points.txt
 Comment: 
 
-Filename: canarypy-0.0.13.dist-info/top_level.txt
+Filename: canarypy-0.0.14.dist-info/top_level.txt
 Comment: 
 
-Filename: canarypy-0.0.13.dist-info/RECORD
+Filename: canarypy-0.0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## canarypy/cli/main.py

```diff
@@ -2,14 +2,15 @@
 
 import click
 from InquirerPy import prompt
 
 from canarypy.cli.services.product import ProductService
 from canarypy.cli.services.release import ReleaseService
 from canarypy.cli.services.signal import SignalService
+from canarypy.config import MIGRATION_PATH
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -118,9 +119,9 @@
 
 
 @db.command(help="Upgrade the database")
 def init():
     from alembic import command
     from alembic.config import Config
 
-    alembic_cfg = Config("alembic.ini")
+    alembic_cfg = Config(MIGRATION_PATH)
     command.upgrade(alembic_cfg, "head")
```

## Comparing `canarypy-0.0.13.dist-info/LICENSE` & `canarypy-0.0.14.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `canarypy-0.0.13.dist-info/METADATA` & `canarypy-0.0.14.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canarypy
-Version: 0.0.13
+Version: 0.0.14
 Summary: CanaryPy - A light and powerful canary release for Data Pipelines
 Home-page: https://github.com/thcidale0808/canarypy
 Author: Thiago Assumpcao
 Author-email: thcidale@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/thcidale0808/canarypy/issues
 Project-URL: Source, https://github.com/thcidale0808/canarypy/
@@ -58,14 +58,19 @@
 
 It integrates a FastAPI application for managing APIs, a Streamlit application for interactive web dashboards, a command-line interface (CLI) for enabling user interaction through terminal commands, and a Python client for incorporating CanaryPy functionalities in your Python applications.
 
 With CanaryPy, you gain the ability to test the waters with new features or updates, ensuring they function as expected in a live environment but affecting only a small subset of data pipelines. CanaryPy's canary release strategy promotes safer deployments, contributing to overall enhanced performance and robustness of your data platform.
 
 ## How it works
 
+CanaryPy has three main entities: 
+* `Product`: It is an application that will have releases. 
+* `Release`: It is any version of your Product. It can be of two types: `active` and `canary`. A release is created as canary which will be tested against the `active` using a linear growth rollout strategy. If the canary performs well during all the phases, it'll be promoted to `active`. The release performance is measure based on its signals.
+* `Signal`: It the execution result of a release. It can have a `success` or `failed` state. Typically, is the result of your job.
+
 CanaryPy also includes a CLI to manage the products, releases, and signals. The CLI is built using the Click library.
 
 The CLI uses the FastAPI application as the backend and therefore the following environment variables need to be set to run the CLI:
 
 * `CANARYPY_URL`: The base URL of the FastAPI application. Defaults to `http://localhost:8080`.
 
 ### Features available
@@ -101,14 +106,22 @@
 
 ```python
 from canarypy.client import CanaryPyClient
 client = CanaryPyClient(base_url="http://localhost:8000")
 client.send_signal_to_canary(artifact_url, version, instance_id, description, status)
 ```
 
+# Airflow Integration
+
+`CanaryPy` provides a plugin to integrate your Airflow tasks with CanaryPy backend with a minimal effort. The plugin can be installed by executing:
+
+`pip install canarypy-airflow-plugin`
+
+Check this [tutorial](examples/airflow-tutorial.md) to understand how this integration works. The plugin code can be found [here](integrations/airflow).
+
 # CanaryPy Deployment
 
 CanaryPy is built around a modular architecture composed by an FastAPI application that host the rest APIs and a Streamlist application that show metrics about release performance. Both applications use a shared PostgreSQL database to store the data.
 
 Setting up CanaryPy for a production environment involves tuning up these two components and making sure the shared PostgreSQL database they both depend on is ready to go. Let's get into the nuts and bolts of how to do that.
 
 ## FastAPI Application
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: canarypy Version: 0.0.13 Summary: CanaryPy - A
+Metadata-Version: 2.1 Name: canarypy Version: 0.0.14 Summary: CanaryPy - A
 light and powerful canary release for Data Pipelines Home-page: https://
 github.com/thcidale0808/canarypy Author: Thiago Assumpcao Author-email:
 thcidale@gmail.com License: UNKNOWN Project-URL: Bug Reports, https://
 github.com/thcidale0808/canarypy/issues Project-URL: Source, https://
 github.com/thcidale0808/canarypy/ Platform: UNKNOWN Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Build Tools Classifier: License :: OSI
@@ -28,65 +28,76 @@
 Streamlit application for interactive web dashboards, a command-line interface
 (CLI) for enabling user interaction through terminal commands, and a Python
 client for incorporating CanaryPy functionalities in your Python applications.
 With CanaryPy, you gain the ability to test the waters with new features or
 updates, ensuring they function as expected in a live environment but affecting
 only a small subset of data pipelines. CanaryPy's canary release strategy
 promotes safer deployments, contributing to overall enhanced performance and
-robustness of your data platform. ## How it works CanaryPy also includes a CLI
-to manage the products, releases, and signals. The CLI is built using the Click
-library. The CLI uses the FastAPI application as the backend and therefore the
-following environment variables need to be set to run the CLI: *
-`CANARYPY_URL`: The base URL of the FastAPI application. Defaults to `http://
-localhost:8080`. ### Features available #### Products Products are the fist
-step in the CanaryPy system. A product is a software application that is being
-released using the CanaryPy system. The CLI provides the following commands to
-manage products: `canapyry product create` This will prompt the user to enter
-the details of the product, and will create the product in the system. ####
-Releases Releases are the second step in the CanaryPy system. A release is a
-version of a product that is being released using the CanaryPy system. The CLI
-provides the following commands to manage releases: `canarypy release create --
-semver_version  --artifact_url ` This will create a new release for a product.
-The semver version and the artifact URL are required parameters. it's possible
-to fetch the latest stable release of a product using the python client as
-shown below: ```python from canarypy.client import CanaryPyClient client =
-CanaryPyClient(base_url="http://localhost:8000")
+robustness of your data platform. ## How it works CanaryPy has three main
+entities: * `Product`: It is an application that will have releases. *
+`Release`: It is any version of your Product. It can be of two types: `active`
+and `canary`. A release is created as canary which will be tested against the
+`active` using a linear growth rollout strategy. If the canary performs well
+during all the phases, it'll be promoted to `active`. The release performance
+is measure based on its signals. * `Signal`: It the execution result of a
+release. It can have a `success` or `failed` state. Typically, is the result of
+your job. CanaryPy also includes a CLI to manage the products, releases, and
+signals. The CLI is built using the Click library. The CLI uses the FastAPI
+application as the backend and therefore the following environment variables
+need to be set to run the CLI: * `CANARYPY_URL`: The base URL of the FastAPI
+application. Defaults to `http://localhost:8080`. ### Features available ####
+Products Products are the fist step in the CanaryPy system. A product is a
+software application that is being released using the CanaryPy system. The CLI
+provides the following commands to manage products: `canapyry product create`
+This will prompt the user to enter the details of the product, and will create
+the product in the system. #### Releases Releases are the second step in the
+CanaryPy system. A release is a version of a product that is being released
+using the CanaryPy system. The CLI provides the following commands to manage
+releases: `canarypy release create --semver_version  --artifact_url ` This will
+create a new release for a product. The semver version and the artifact URL are
+required parameters. it's possible to fetch the latest stable release of a
+product using the python client as shown below: ```python from canarypy.client
+import CanaryPyClient client = CanaryPyClient(base_url="http://localhost:8000")
 client.get_latest_stable_version(product_name) ``` #### Signals Signals are the
 third step in the CanaryPy system. A signal is the result of an execution of a
 product with a release. The CLI provides the following commands to manage
 signals: `canarypy signal create --status  --description  --instance-id  -
 - semver-version  --artifact-url ` It's also possible to send signals to the
 CanaryPy system using the Python client as shown below: ```python from
 canarypy.client import CanaryPyClient client = CanaryPyClient(base_url="http://
 localhost:8000") client.send_signal_to_canary(artifact_url, version,
-instance_id, description, status) ``` # CanaryPy Deployment CanaryPy is built
-around a modular architecture composed by an FastAPI application that host the
-rest APIs and a Streamlist application that show metrics about release
-performance. Both applications use a shared PostgreSQL database to store the
-data. Setting up CanaryPy for a production environment involves tuning up these
-two components and making sure the shared PostgreSQL database they both depend
-on is ready to go. Let's get into the nuts and bolts of how to do that. ##
-FastAPI Application The FastAPI application serves as the backend for CanaryPy,
-providing RESTful APIs for managing products, releases, and signals. ###
-Summary The application provides endpoints for creating and retrieving products
-and their respective releases. It also includes endpoints for creating and
-retrieving signals related to each release. The FastAPI application uses a
-PostgreSQL database to store the data. ### Endpoints The CanaryPy provides
-endpoints to manage products, releases, and signals. More details about the
-endpoints can be found in the `/docs` endpoint. ### How to run 1. The following
-environment variable can be set to start the FastAPI server: *
-`CANARYPY_API_PORT`: The base URL of the FastAPI application. Defaults to
-`8080`. * `CANARYPY_API_HOST`: The base URL of the FastAPI application.
-Defaults to `0.0.0.0`. * `CANARYPY_API_RELOAD`: Whether to reload the server
-when code changes are detected. Defaults to `True`. * `CANARYPY_API_DEBUG`:
-Whether to run the server in debug mode. Defaults to `True`. *
-`CANARYPY_API_LOG_LEVEL`: The log level for the server. Defaults to `info`. *
-`CANARYPY_DB_CONN_STRING`: The connection string for the database.
-Alternatively, you can set the connection details in separated environment
-variables: * `CANARYPY_DB_USER`: The username for the database. *
+instance_id, description, status) ``` # Airflow Integration `CanaryPy` provides
+a plugin to integrate your Airflow tasks with CanaryPy backend with a minimal
+effort. The plugin can be installed by executing: `pip install canarypy-
+airflow-plugin` Check this [tutorial](examples/airflow-tutorial.md) to
+understand how this integration works. The plugin code can be found [here]
+(integrations/airflow). # CanaryPy Deployment CanaryPy is built around a
+modular architecture composed by an FastAPI application that host the rest APIs
+and a Streamlist application that show metrics about release performance. Both
+applications use a shared PostgreSQL database to store the data. Setting up
+CanaryPy for a production environment involves tuning up these two components
+and making sure the shared PostgreSQL database they both depend on is ready to
+go. Let's get into the nuts and bolts of how to do that. ## FastAPI Application
+The FastAPI application serves as the backend for CanaryPy, providing RESTful
+APIs for managing products, releases, and signals. ### Summary The application
+provides endpoints for creating and retrieving products and their respective
+releases. It also includes endpoints for creating and retrieving signals
+related to each release. The FastAPI application uses a PostgreSQL database to
+store the data. ### Endpoints The CanaryPy provides endpoints to manage
+products, releases, and signals. More details about the endpoints can be found
+in the `/docs` endpoint. ### How to run 1. The following environment variable
+can be set to start the FastAPI server: * `CANARYPY_API_PORT`: The base URL of
+the FastAPI application. Defaults to `8080`. * `CANARYPY_API_HOST`: The base
+URL of the FastAPI application. Defaults to `0.0.0.0`. * `CANARYPY_API_RELOAD`:
+Whether to reload the server when code changes are detected. Defaults to
+`True`. * `CANARYPY_API_DEBUG`: Whether to run the server in debug mode.
+Defaults to `True`. * `CANARYPY_API_LOG_LEVEL`: The log level for the server.
+Defaults to `info`. * `CANARYPY_DB_CONN_STRING`: The connection string for the
+database. Alternatively, you can set the connection details in separated
+environment variables: * `CANARYPY_DB_USER`: The username for the database. *
 `CANARYPY_DB_PASSWORD`: The password for the database. * `CANARYPY_DB_HOST`:
 The host for the database. * `CANARYPY_DB_PORT`: The port for the database. *
 `CANARYPY_DB_NAME`: The name of the database. 2. Run the FastAPI application
 using the following command `canarypy api start` ## Streamlit Application The
 Streamlit application serves as a web-based user interface for visualizing the
 release metrics. ### Summary The application fetches the metrics data from the
 FastAPI backend and displays it in a user-friendly format, helping you
```

