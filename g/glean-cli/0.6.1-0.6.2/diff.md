# Comparing `tmp/glean-cli-0.6.1.tar.gz` & `tmp/glean-cli-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glean-cli-0.6.1.tar", last modified: Thu Jul  6 15:36:28 2023, max compression
+gzip compressed data, was "glean-cli-0.6.2.tar", last modified: Mon Jul 10 17:31:39 2023, max compression
```

## Comparing `glean-cli-0.6.1.tar` & `glean-cli-0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.757036 glean-cli-0.6.1/
--rw-r--r--   0 melody     (501) staff       (20)    11357 2022-02-18 21:50:06.000000 glean-cli-0.6.1/LICENSE
--rw-r--r--   0 melody     (501) staff       (20)     1283 2023-07-06 15:36:28.757102 glean-cli-0.6.1/PKG-INFO
--rw-r--r--   0 melody     (501) staff       (20)      832 2023-01-03 15:16:58.000000 glean-cli-0.6.1/README.md
--rw-r--r--   0 melody     (501) staff       (20)      103 2022-02-18 21:50:06.000000 glean-cli-0.6.1/pyproject.toml
--rw-r--r--   0 melody     (501) staff       (20)      831 2023-07-06 15:36:28.757345 glean-cli-0.6.1/setup.cfg
--rw-r--r--   0 melody     (501) staff       (20)       38 2022-02-18 21:50:06.000000 glean-cli-0.6.1/setup.py
-drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.752625 glean-cli-0.6.1/src/
-drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.754459 glean-cli-0.6.1/src/glean/
--rw-r--r--   0 melody     (501) staff       (20)       18 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/__init__.py
--rw-r--r--   0 melody     (501) staff       (20)    31870 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/cli.py
--rw-r--r--   0 melody     (501) staff       (20)     1598 2023-01-03 15:16:58.000000 glean-cli-0.6.1/src/glean/credentials.py
--rw-r--r--   0 melody     (501) staff       (20)     3904 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/filesystem.py
--rw-r--r--   0 melody     (501) staff       (20)    14250 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/glean_api.py
-drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.755148 glean-cli-0.6.1/src/glean/utils/
--rw-r--r--   0 melody     (501) staff       (20)        0 2023-01-03 15:16:58.000000 glean-cli-0.6.1/src/glean/utils/__init__.py
--rw-r--r--   0 melody     (501) staff       (20)      509 2023-01-03 15:16:58.000000 glean-cli-0.6.1/src/glean/utils/cli.py
--rw-r--r--   0 melody     (501) staff       (20)     2622 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/utils/grn.py
--rw-r--r--   0 melody     (501) staff       (20)     1356 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/utils/resource.py
--rw-r--r--   0 melody     (501) staff       (20)     1089 2023-07-06 15:35:54.000000 glean-cli-0.6.1/src/glean/utils/validate_config.py
-drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.755877 glean-cli-0.6.1/src/glean_cli.egg-info/
--rw-r--r--   0 melody     (501) staff       (20)     1283 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/PKG-INFO
--rw-r--r--   0 melody     (501) staff       (20)      616 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/SOURCES.txt
--rw-r--r--   0 melody     (501) staff       (20)        1 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/dependency_links.txt
--rw-r--r--   0 melody     (501) staff       (20)       41 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/entry_points.txt
--rw-r--r--   0 melody     (501) staff       (20)      116 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/requires.txt
--rw-r--r--   0 melody     (501) staff       (20)        6 2023-07-06 15:36:28.000000 glean-cli-0.6.1/src/glean_cli.egg-info/top_level.txt
-drwxr-xr-x   0 melody     (501) staff       (20)        0 2023-07-06 15:36:28.756695 glean-cli-0.6.1/tests/
--rw-r--r--   0 melody     (501) staff       (20)      309 2023-01-03 15:16:58.000000 glean-cli-0.6.1/tests/test_cli.py
--rw-r--r--   0 melody     (501) staff       (20)     1652 2023-01-03 15:16:58.000000 glean-cli-0.6.1/tests/test_credentials.py
--rw-r--r--   0 melody     (501) staff       (20)     4632 2023-07-06 15:35:54.000000 glean-cli-0.6.1/tests/test_filesystem.py
--rw-r--r--   0 melody     (501) staff       (20)      666 2023-01-12 21:30:33.000000 glean-cli-0.6.1/tests/test_glean_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.923319 glean-cli-0.6.2/
+-rw-r--r--   0 anixon     (501) staff       (20)    11357 2022-12-17 00:47:55.000000 glean-cli-0.6.2/LICENSE
+-rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-10 17:31:39.923386 glean-cli-0.6.2/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      832 2023-01-19 16:41:15.000000 glean-cli-0.6.2/README.md
+-rw-r--r--   0 anixon     (501) staff       (20)      103 2022-12-17 00:47:55.000000 glean-cli-0.6.2/pyproject.toml
+-rw-r--r--   0 anixon     (501) staff       (20)      831 2023-07-10 17:31:39.923738 glean-cli-0.6.2/setup.cfg
+-rw-r--r--   0 anixon     (501) staff       (20)       38 2022-12-17 00:47:55.000000 glean-cli-0.6.2/setup.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.918247 glean-cli-0.6.2/src/
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.920266 glean-cli-0.6.2/src/glean/
+-rw-r--r--   0 anixon     (501) staff       (20)       18 2023-07-10 17:30:58.000000 glean-cli-0.6.2/src/glean/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)    31995 2023-07-10 17:30:58.000000 glean-cli-0.6.2/src/glean/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1598 2022-12-17 00:47:55.000000 glean-cli-0.6.2/src/glean/credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     3904 2023-06-20 13:04:07.000000 glean-cli-0.6.2/src/glean/filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)    14250 2023-07-07 16:24:44.000000 glean-cli-0.6.2/src/glean/glean_api.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.921378 glean-cli-0.6.2/src/glean/utils/
+-rw-r--r--   0 anixon     (501) staff       (20)        0 2022-12-17 00:47:55.000000 glean-cli-0.6.2/src/glean/utils/__init__.py
+-rw-r--r--   0 anixon     (501) staff       (20)      509 2023-01-03 16:54:54.000000 glean-cli-0.6.2/src/glean/utils/cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     2622 2023-06-15 18:48:08.000000 glean-cli-0.6.2/src/glean/utils/grn.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1356 2023-06-23 20:05:46.000000 glean-cli-0.6.2/src/glean/utils/resource.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1089 2023-06-15 18:48:08.000000 glean-cli-0.6.2/src/glean/utils/validate_config.py
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.922240 glean-cli-0.6.2/src/glean_cli.egg-info/
+-rw-r--r--   0 anixon     (501) staff       (20)     1283 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anixon     (501) staff       (20)      616 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        1 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anixon     (501) staff       (20)       41 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anixon     (501) staff       (20)      116 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/requires.txt
+-rw-r--r--   0 anixon     (501) staff       (20)        6 2023-07-10 17:31:39.000000 glean-cli-0.6.2/src/glean_cli.egg-info/top_level.txt
+drwxr-xr-x   0 anixon     (501) staff       (20)        0 2023-07-10 17:31:39.923189 glean-cli-0.6.2/tests/
+-rw-r--r--   0 anixon     (501) staff       (20)      309 2022-12-17 00:47:55.000000 glean-cli-0.6.2/tests/test_cli.py
+-rw-r--r--   0 anixon     (501) staff       (20)     1652 2022-12-17 00:47:55.000000 glean-cli-0.6.2/tests/test_credentials.py
+-rw-r--r--   0 anixon     (501) staff       (20)     4632 2023-06-23 20:05:46.000000 glean-cli-0.6.2/tests/test_filesystem.py
+-rw-r--r--   0 anixon     (501) staff       (20)      666 2022-12-17 00:47:55.000000 glean-cli-0.6.2/tests/test_glean_api.py
```

### Comparing `glean-cli-0.6.1/LICENSE` & `glean-cli-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/PKG-INFO` & `glean-cli-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.6.1/README.md` & `glean-cli-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/setup.cfg` & `glean-cli-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean/cli.py` & `glean-cli-0.6.2/src/glean/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,24 +75,21 @@
     Only applicable when also using the `--git-revision` flag.
     """,
 )
 dbt_manifest_option = click.option(
     "--dbt-manifest",
     "dbt_manifest_path",
     required=False,
-    # TODO(meyer): unhide when feature is stable
-    hidden=True,
     help="Path to dbt manifest JSON file (if using Glean dbt integration).",
     type=click.Path(exists=True, readable=True, file_okay=True, dir_okay=False),
 )
 run_dbt_parse_option = click.option(
     "--dbt",
     "run_dbt_parse",
     required=False,
-    hidden=True,
     help="If specified, runs `dbt parse` and uses the resulting manifest.",
     is_flag=True,
     default=False
 )
 dbt_parse_flags_argument = click.argument(
     "DBT_FLAGS",
     type=click.STRING,
@@ -122,15 +119,14 @@
     envvar="GLEAN_CREDENTIALS_FILEPATH",
 )
 @click.pass_context
 def cli(ctx, credentials_filepath):
     """A command-line interface for interacting with Glean."""
     if GLEAN_DEBUG or GLEAN_VERBOSE_DEBUG_UNSAFE:
         _enable_http_logging()
-
     ctx.ensure_object(dict)
     ctx.obj["credentials"] = get_credentials(os.path.expanduser(credentials_filepath))
 
 
 @cli.command(
     "preview",
     context_settings=dict(
@@ -184,15 +180,14 @@
     run_dbt_parse: bool,
     filepath: str,
     preview: bool,
     dbt_flags,
     allow_dangerous_empty_build: bool,
 ):
     """Validates and deploys resource configurations to your project."""
-
     dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
 
     if preview:
         click.echo("🏗️  Creating preview build...")
         build_results = _create_build_using_options(
             ctx,
             filepath,
@@ -562,15 +557,19 @@
     """Convenience wrapper for running `dbt parse` before `glean preview` or `glean deploy`.
     Must be run from your Glean project directory.
 
     Flags passed in after the Glean subcommand will be passed onwards to dbt.
     """
 
     if not run_dbt_parse:
-        return None
+        # no --dbt flag
+        if dbt_manifest_path is not None:
+            # user specified --dbt-manifest explicitly
+            click.echo(f"✅ Using manifest file at {dbt_manifest_path}\n")
+        return dbt_manifest_path
 
     if dbt_manifest_path is not None:
         click.echo()
         click.echo("🚨 `--dbt-manifest` is redundant when running with `--dbt` and will be ignored.")
         click.echo()
     click.echo("🐇 Running `dbt parse` to generate a manifest file.")
```

### Comparing `glean-cli-0.6.1/src/glean/credentials.py` & `glean-cli-0.6.2/src/glean/credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean/filesystem.py` & `glean-cli-0.6.2/src/glean/filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean/glean_api.py` & `glean-cli-0.6.2/src/glean/glean_api.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean/utils/grn.py` & `glean-cli-0.6.2/src/glean/utils/grn.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean/utils/resource.py` & `glean-cli-0.6.2/src/glean/utils/resource.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean/utils/validate_config.py` & `glean-cli-0.6.2/src/glean/utils/validate_config.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/src/glean_cli.egg-info/PKG-INFO` & `glean-cli-0.6.2/src/glean_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: Command-line tools for interacting with Glean
 Home-page: https://glean.io/
 Author: Dan Eisenberg
 Author-email: dse@glean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `glean-cli-0.6.1/src/glean_cli.egg-info/SOURCES.txt` & `glean-cli-0.6.2/src/glean_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/tests/test_credentials.py` & `glean-cli-0.6.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/tests/test_filesystem.py` & `glean-cli-0.6.2/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `glean-cli-0.6.1/tests/test_glean_api.py` & `glean-cli-0.6.2/tests/test_glean_api.py`

 * *Files identical despite different names*

