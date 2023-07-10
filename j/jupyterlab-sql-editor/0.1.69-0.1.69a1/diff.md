# Comparing `tmp/jupyterlab_sql_editor-0.1.69.tar.gz` & `tmp/jupyterlab_sql_editor-0.1.69a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_sql_editor-0.1.69.tar", last modified: Mon Jul 10 17:14:33 2023, max compression
+gzip compressed data, was "jupyterlab_sql_editor-0.1.69a1.tar", last modified: Fri Jul  7 16:21:05 2023, max compression
```

## Comparing `jupyterlab_sql_editor-0.1.69.tar` & `jupyterlab_sql_editor-0.1.69a1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.035591 jupyterlab_sql_editor-0.1.69/
--rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      472 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     8197 2023-07-10 17:14:33.035591 jupyterlab_sql_editor-0.1.69/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6928 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/RELEASE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      203 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/install.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.023591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/
--rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      471 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/
--rw-r--r--   0 vsts      (1001) docker     (123)     3125 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8098 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/balls_line.gif
--rw-r--r--   0 vsts      (1001) docker     (123)     4960 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/common.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8623 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/spark_streaming_query.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6895 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/sparkdf.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/common/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4621 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/common/base.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9263 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/common/export.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1768 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11138 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/
--rw-r--r--   0 vsts      (1001) docker     (123)       99 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/parser.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7418 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35548 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10544 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/trino.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3539 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/
--rw-r--r--   0 vsts      (1001) docker     (123)    21040 2023-07-10 17:14:09.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/build_log.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4029 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/package.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.023591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/schemas/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/
--rw-r--r--   0 vsts      (1001) docker     (123)     3887 2023-07-10 17:14:09.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-10 17:14:09.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.031591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/
--rw-r--r--   0 vsts      (1001) docker     (123)    23411 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
--rw-r--r--   0 vsts      (1001) docker     (123)    31873 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)    29612 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/remoteEntry.62319715761ed974bbd3.js
--rw-r--r--   0 vsts      (1001) docker     (123)    28460 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/remoteEntry.62319715761ed974bbd3.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)      164 2023-07-10 17:14:09.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/style.js
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)    12072 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
--rw-r--r--   0 vsts      (1001) docker     (123)    13811 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
--rw-r--r--   0 vsts      (1001) docker     (123)   361933 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
--rw-r--r--   0 vsts      (1001) docker     (123)   485462 2023-07-10 17:14:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.027591 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     8197 2023-07-10 17:14:32.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3163 2023-07-10 17:14:33.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-10 17:14:32.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-07-10 17:14:32.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-10 17:13:10.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-10 17:14:32.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-07-10 17:14:32.000000 jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.031591 jupyterlab_sql_editor-0.1.69/overrides/
--rw-r--r--   0 vsts      (1001) docker     (123)      676 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/overrides/sparksql-lsp.json
--rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/overrides/syntax_highlighting.json
--rw-r--r--   0 vsts      (1001) docker     (123)      671 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/overrides/trino-lsp.json
--rw-r--r--   0 vsts      (1001) docker     (123)     3887 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/package.json
--rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.031591 jupyterlab_sql_editor-0.1.69/schema/
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/schema/plugin.json
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-10 17:14:33.035591 jupyterlab_sql_editor-0.1.69/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     3960 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.035591 jupyterlab_sql_editor-0.1.69/src/
--rw-r--r--   0 vsts      (1001) docker     (123)      362 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/src/constants.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     8368 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/src/formatter.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     6249 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/src/index.ts
--rw-r--r--   0 vsts      (1001) docker     (123)     3429 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/src/utils.ts
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 17:14:33.035591 jupyterlab_sql_editor-0.1.69/style/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/style/base.css
--rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/style/index.css
--rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/style/index.js
--rw-r--r--   0 vsts      (1001) docker     (123)      554 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/tsconfig.json
--rw-r--r--   0 vsts      (1001) docker     (123)   228103 2023-07-10 17:12:25.000000 jupyterlab_sql_editor-0.1.69/yarn.lock
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.205593 jupyterlab_sql_editor-0.1.69a1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1074 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      472 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     8199 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     6928 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/RELEASE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      203 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/install.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.193592 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/
+-rw-r--r--   0 vsts      (1001) docker     (123)      261 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      471 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3125 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8098 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/balls_line.gif
+-rw-r--r--   0 vsts      (1001) docker     (123)     4960 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/common.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8623 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/spark_streaming_query.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7828 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/sparkdf.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4621 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/base.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9263 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/export.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1768 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4722 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10866 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/
+-rw-r--r--   0 vsts      (1001) docker     (123)       99 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5389 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7418 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35548 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10359 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3539 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/
+-rw-r--r--   0 vsts      (1001) docker     (123)    21048 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/build_log.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4037 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/package.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.189592 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.197593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3895 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)    23411 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    31873 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)    29620 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    28468 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)      164 2023-07-07 16:20:38.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)    12072 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    13811 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
+-rw-r--r--   0 vsts      (1001) docker     (123)   361933 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
+-rw-r--r--   0 vsts      (1001) docker     (123)   485462 2023-07-07 16:20:39.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.193592 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8199 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3163 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      357 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-07 16:19:31.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-07-07 16:21:05.000000 jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/overrides/
+-rw-r--r--   0 vsts      (1001) docker     (123)      676 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/overrides/sparksql-lsp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       91 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/overrides/syntax_highlighting.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      671 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/overrides/trino-lsp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     3895 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/package.json
+-rw-r--r--   0 vsts      (1001) docker     (123)      619 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/schema/plugin.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-07 16:21:05.205593 jupyterlab_sql_editor-0.1.69a1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3960 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/src/
+-rw-r--r--   0 vsts      (1001) docker     (123)      362 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/constants.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     8368 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/formatter.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     6249 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/index.ts
+-rw-r--r--   0 vsts      (1001) docker     (123)     3429 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/src/utils.ts
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 16:21:05.201593 jupyterlab_sql_editor-0.1.69a1/style/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/style/base.css
+-rw-r--r--   0 vsts      (1001) docker     (123)       25 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/style/index.css
+-rw-r--r--   0 vsts      (1001) docker     (123)       21 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/style/index.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      554 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/tsconfig.json
+-rw-r--r--   0 vsts      (1001) docker     (123)   228103 2023-07-07 16:18:38.000000 jupyterlab_sql_editor-0.1.69a1/yarn.lock
```

### Comparing `jupyterlab_sql_editor-0.1.69/LICENSE` & `jupyterlab_sql_editor-0.1.69a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/PKG-INFO` & `jupyterlab_sql_editor-0.1.69a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_sql_editor
-Version: 0.1.69
+Version: 0.1.69a1
 Summary: SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.
 Home-page: https://github.com/CybercentreCanada/jupyterlab-sql-editor
 Author: cccs-jc
 Author-email: contact@cyber.gc.ca
 License: MIT License (MIT)
 Keywords: sql,Jupyter,JupyterLab,JupyterLab3,jupyter,jupyterlab-extension,spark,trino,dataframe,cccs,canada
 Platform: Linux
```

### Comparing `jupyterlab_sql_editor-0.1.69/README.md` & `jupyterlab_sql_editor-0.1.69a1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/RELEASE.md` & `jupyterlab_sql_editor-0.1.69a1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/SparkSchemaWidget.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/balls_line.gif` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/balls_line.gif`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/common.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/common.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/spark_streaming_query.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/spark_streaming_query.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython/sparkdf.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython/sparkdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,41 +47,60 @@
 
 
 def display_spark_df(df, output, limit, truncate, show_nonprinting, args):
     """
     Execute the query of the dataframe and time the execution.
     """
     displays = []
+    start = time()
+    has_more_data = False
     if output == "grid":
-        pdf = to_pandas(df, limit, truncate, show_nonprinting)
+        has_more_data, pdf = to_pandas(df, limit, truncate, show_nonprinting)
         displays.append(render_grid(pdf, limit))
     elif output == "aggrid":
-        pdf = to_pandas(df, limit, truncate, show_nonprinting)
+        has_more_data, pdf = to_pandas(df, limit, truncate, show_nonprinting)
         displays.append(render_ag_grid(pdf))
     elif output == "json":
         json_array = []
         warnings = []
         results = df.toJSON().map(lambda j: json.loads(j)).take(limit)
+        if len(results) > limit:
+            has_more_data = True
         # cast unsafe ints to str for display
         for row in results:
             json_array.append(sanitize_results(row, warnings))
         # add warnings to displays
         for warning in warnings:
             displays.append(warning)
         if show_nonprinting:
             recursive_escape(json_array)
         displays.append(JSON(json_array, expanded=args.expand))
     elif output == "html":
-        html_text = to_html(df, limit, truncate, show_nonprinting)
+        has_more_data, html_text = to_html(df, limit, truncate, show_nonprinting)
         displays.append(HTML(html_text))
     elif output == "text":
         text = df._jdf.showString(limit, truncate, False)
         displays.append(PlainText(data=text))
-    elif output == "skip" or output == "none":
-        displays.append(PlainText(data="Display of results skipped"))
+    elif limit <= 0 or output == "skip" or output == "none":
+        displays.append("Query execution skipped")
+        return []
+    elif output == "schema":
+        df.printSchema()
+        return []
+    else:
+        displays.append(PlainText(data=f"Invalid output option {output}, valid options are grid, json, html, text"))
+    end = time()
+    elapsed = end - start
+    if has_more_data:
+        message = "only showing top %d %s\n" % (
+            limit,
+            "row" if limit == 1 else "rows",
+        )
+        displays.append(PlainText(data=message))
+    displays.append(PlainText(data=f"Execution time: {elapsed:.2f} seconds"))
     return displays
 
 
 def display_link():
     """
     Display a link in notebook so a user can open the spark UI's details.
     """
@@ -171,28 +190,32 @@
     Execute the query unerlying the dataframe and creates an html representation of the results.
     Code inspired from spark's dataframe.py
     """
     sock_info = df._jdf.getRowsToPython(max_num_rows, truncate)
     rows = list(_load_from_socket(sock_info, BatchedSerializer(PickleSerializer())))
     columns = rows[0]
     row_data = rows[1:]
+    has_more_data = len(row_data) > max_num_rows
     row_data = row_data[:max_num_rows]
     html = rows_to_html(columns, row_data, show_nonprinting)
-    return html
+    if has_more_data:
+        html += "only showing top %d %s\n" % (max_num_rows, "row" if max_num_rows == 1 else "rows")
+    return has_more_data, html
 
 
 def to_pandas(df, max_num_rows, truncate, show_nonprinting):
     """
     Execute the query unerlying the dataframe and creates a pandas dataframe with the results.
     Code inspired from spark's dataframe.py
     """
     sock_info = df._jdf.getRowsToPython(max_num_rows, truncate)
     rows = list(_load_from_socket(sock_info, BatchedSerializer(PickleSerializer())))
     head = rows[0]
     row_data = rows[1:]
+    has_more_data = len(row_data) > max_num_rows
     row_data = row_data[:max_num_rows]
     pdf = pd.DataFrame(columns=head)
     for i, row in enumerate(row_data):
         if show_nonprinting:
             row = [escape_control_chars(str(v)) for v in row]
         pdf.loc[i] = row
-    return pdf
+    return has_more_data, pdf
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/common/base.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/base.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/common/export.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/common/export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/main.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/main.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/spark_export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/sparksql/sparksql.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         streaming_mode = args.streaming_mode.lower()
 
         truncate = 256
         if args.truncate and args.truncate > 0:
             truncate = args.truncate
 
         limit = args.limit
-        if limit is None or limit <= 0:
+        if limit is None:
             limit = self.limit
 
         if output not in VALID_OUTPUTS:
             print(f"Invalid output option {args.output}. The valid options are {VALID_OUTPUTS}.")
             return
 
         self.spark = self.get_instantiated_spark_session()
@@ -150,30 +150,26 @@
         # statements like INSERT INTO, USE SCHEMA, CREATE TABLE, DROP TABLE
         # execute immediatly, they do not require us to perform a .show(), .collect()
         # we detect these use case by checking for an empty list of columns (no return schema)
         # we treat these use cases differently than a SELECT that returns rows of data
         start = time()
         try:
             df = self.spark.sql(sql)
-            if output == "schema":
-                df.printSchema()
-                return
             results = self.spark.createDataFrame(df.take(limit + 1), schema=df.schema)
         except PYSPARK_ERROR_TYPES as exc:
             if args.lean_exceptions:
                 self.print_pyspark_error(exc)
                 return
             else:
                 raise exc
         end = time()
-        print(f"Execution time: {end - start:.2f} seconds")
-
-        # The text output already has it's own message coming from Spark
-        if results.count() > limit and not (output == "skip" or output == "none" or output == "text"):
-            print(f"Only showing top {limit} {'row' if limit == 1 else 'rows'}")
+        if len(results.columns) == 0:
+            elapsed = end - start
+            print(f"Execution time: {elapsed:.2f} seconds")
+            return
 
         if args.cache or args.eager:
             load_type = "eager" if args.eager else "lazy"
             print(f"Cached dataframe with {load_type} load")
             results = results.cache()
             if args.eager:
                 results.count()
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/main.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/main.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/parser.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parser_test.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/parsetab.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/trino.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import os
-from time import time
 
 import pandas as pd
 import trino
 from IPython.core.magic import line_cell_magic, magics_class, needs_local_scope
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from IPython.display import HTML, JSON, display
 from traitlets import Bool, Instance, Int, Unicode, Union
@@ -115,26 +114,30 @@
             catalog = self.catalog
 
         schema = args.schema
         if not schema:
             schema = self.schema
 
         limit = args.limit
-        if limit is None or limit <= 0:
+        if limit is None:
             limit = self.limit
 
         catalog_array = self.get_catalog_array()
         if self.check_refresh(args.refresh.lower(), output_file, catalog_array):
             return
 
         output = args.output.lower()
         if output not in VALID_OUTPUTS:
             print(f"Invalid output option {args.output}. The valid options are {VALID_OUTPUTS}.")
             return
 
+        if limit <= 0 or output == "skip" or output == "none":
+            print("Query execution skipped")
+            return
+
         sql = self.get_sql_statement(cell, args.sql, args.jinja)
         if not sql:
             return
 
         if output == "sql":
             return self.display_sql(sql)
         elif not args.raw:
@@ -147,23 +150,20 @@
             user=self.user,
             catalog=catalog,
             schema=schema,
             http_scheme=self.httpScheme,
             verify=self.verify,
         )
         self.cur = self.conn.cursor()
-        start = time()
         self.cur.execute(sql)
         results = self.cur.fetchmany(limit + 1)
         columns = list(map(lambda d: d[0], self.cur.description))
-        end = time()
-        print(f"Execution time: {end - start:.2f} seconds")
 
-        if len(results) > limit and not (output == "skip" or output == "none"):
-            print(f"Only showing top {limit} {'row' if limit == 1 else 'rows'}")
+        if len(results) > limit:
+            print("Only showing top %d row(s)" % limit)
             results = results[:limit]
 
         results = list(map(lambda row: [self.format_cell(v, output, truncate) for v in row], results[:limit]))
 
         if args.dataframe:
             print(f"Saved results to pandas dataframe named `{args.dataframe}`")
             pdf = pd.DataFrame.from_records(results, columns=columns)
@@ -208,16 +208,14 @@
                 ),
             )
         elif output == "html":
             html = rows_to_html(columns, results, show_nonprinting)
             display(HTML(make_tag("table", False, html)))
         elif output == "text":
             print(self.render_text(results, columns))
-        elif output == "skip" or output == "none":
-            display("Display of results skipped")
 
     def check_refresh(self, refresh_arg, output_file, catalog_array):
         if refresh_arg == "all":
             update_database_schema(self.cur, output_file, catalog_array)
             return True
         if refresh_arg != "none":
             print(f"Invalid refresh option given {refresh_arg}. Valid refresh options are [all|local|none]")
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/ipython_magic/trino/trino_export.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/build_log.json` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993348233291%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'jupyterlab-sql-editor': {'version': "*

 * *      "'0.1.69-alpha.1'}}}}}}"}*

```diff
@@ -602,15 +602,15 @@
                             "singleton": true
                         },
                         "@types/codemirror": {},
                         "codemirror": {},
                         "jupyterlab-sql-editor": {
                             "import": "/home/vsts/work/1/s/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.69"
+                            "version": "0.1.69-alpha.1"
                         },
                         "npm-run-all": {},
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/package.json` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757936507936508%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7a5c41927a28f0d15d2b.js'}}",*

 * * "'version'": "'0.1.69-alpha.1'"}*

```diff
@@ -41,15 +41,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/CybercentreCanada/jupyterlab-sql-editor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.62319715761ed974bbd3.js",
+            "load": "static/remoteEntry.7a5c41927a28f0d15d2b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_sql_editor/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
             "@krassowski/jupyterlab-lsp": {
@@ -109,9 +109,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.69"
+    "version": "0.1.69-alpha.1"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.1.69-alpha.1'"}*

```diff
@@ -104,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.69"
+    "version": "0.1.69-alpha.1"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/remoteEntry.62319715761ed974bbd3.js` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -428,15 +428,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-sql-editor", "0.1.69", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-sql-editor", "0.1.69-alpha.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                     register("sql-formatter", "6.1.2", () => (__webpack_require__.e("vendors-node_modules_sql-formatter_lib_index_js").then(() => (() => (__webpack_require__( /*! ./node_modules/sql-formatter/lib/index.js */ "./node_modules/sql-formatter/lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
@@ -1099,8 +1099,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-sql-editor");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-sql-editor"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.62319715761ed974bbd3.js.map
+//# sourceMappingURL=remoteEntry.7a5c41927a28f0d15d2b.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/remoteEntry.62319715761ed974bbd3.js.map` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.7a5c41927a28f0d15d2b.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.62319715761ed974bbd3.js",
+    "file": "remoteEntry.7a5c41927a28f0d15d2b.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qRAAqR;WACnT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-sql-editor/webpack/container-entry",
         "webpack://jupyterlab-sql-editor/webpack/bootstrap",
         "webpack://jupyterlab-sql-editor/webpack/runtime/compat get default export",
@@ -30,15 +30,15 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"67b6c3715f795c58c5d6\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"8ab7ecce559b1f364311\",\"style_index_js\":\"7a9353dfa84524daa532\",\"vendors-node_modules_sql-formatter_lib_index_js\":\"1955e937c0ff0f3413ea\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-sql-editor:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-sql-editor\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-sql-editor\", \"0.1.69\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"6.1.2\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-sql-editor\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-sql-editor\", \"0.1.69-alpha.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"sql-formatter\", \"6.1.2\", () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/sql-formatter/lib/index.js */ \"./node_modules/sql-formatter/lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\": () => (loadSingletonVersionCheck(\"default\", \"@krassowski/jupyterlab-lsp\", [1,3,10,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/codemirror\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/fileeditor\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,1])),\n\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\": () => (loadStrictVersionCheckFallback(\"default\", \"sql-formatter\", [4,6,1,2], () => (__webpack_require__.e(\"vendors-node_modules_sql-formatter_lib_index_js\").then(() => (() => (__webpack_require__(/*! sql-formatter */ \"./node_modules/sql-formatter/lib/index.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@krassowski/jupyterlab-lsp\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/codemirror\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/fileeditor\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/sql-formatter/sql-formatter\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-sql-editor\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_sql_editor\"] = self[\"webpackChunkjupyterlab_sql_editor\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-sql-editor\");\n",
         ""
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/PKG-INFO` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-sql-editor
-Version: 0.1.69
+Version: 0.1.69a1
 Summary: SQL editor support for formatting, syntax highlighting and code completion of SQL in cell magic, line magic, python string and file editor.
 Home-page: https://github.com/CybercentreCanada/jupyterlab-sql-editor
 Author: cccs-jc
 Author-email: contact@cyber.gc.ca
 License: MIT License (MIT)
 Keywords: sql,Jupyter,JupyterLab,JupyterLab3,jupyter,jupyterlab-extension,spark,trino,dataframe,cccs,canada
 Platform: Linux
```

### Comparing `jupyterlab_sql_editor-0.1.69/jupyterlab_sql_editor.egg-info/SOURCES.txt` & `jupyterlab_sql_editor-0.1.69a1/jupyterlab_sql_editor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 jupyterlab_sql_editor/ipython_magic/trino/trino_export.py
 jupyterlab_sql_editor/labextension/build_log.json
 jupyterlab_sql_editor/labextension/package.json
 jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/package.json.orig
 jupyterlab_sql_editor/labextension/schemas/jupyterlab-sql-editor/plugin.json
 jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js
 jupyterlab_sql_editor/labextension/static/lib_index_js.67b6c3715f795c58c5d6.js.map
-jupyterlab_sql_editor/labextension/static/remoteEntry.62319715761ed974bbd3.js
-jupyterlab_sql_editor/labextension/static/remoteEntry.62319715761ed974bbd3.js.map
+jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js
+jupyterlab_sql_editor/labextension/static/remoteEntry.7a5c41927a28f0d15d2b.js.map
 jupyterlab_sql_editor/labextension/static/style.js
 jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js
 jupyterlab_sql_editor/labextension/static/style_index_js.7a9353dfa84524daa532.js.map
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.8ab7ecce559b1f364311.js.map
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js
 jupyterlab_sql_editor/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.1955e937c0ff0f3413ea.js.map
```

### Comparing `jupyterlab_sql_editor-0.1.69/overrides/sparksql-lsp.json` & `jupyterlab_sql_editor-0.1.69a1/overrides/sparksql-lsp.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/overrides/trino-lsp.json` & `jupyterlab_sql_editor-0.1.69a1/overrides/trino-lsp.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/package.json` & `jupyterlab_sql_editor-0.1.69a1/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.1.69-alpha.1'"}*

```diff
@@ -104,9 +104,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.69"
+    "version": "0.1.69-alpha.1"
 }
```

### Comparing `jupyterlab_sql_editor-0.1.69/pyproject.toml` & `jupyterlab_sql_editor-0.1.69a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/schema/plugin.json` & `jupyterlab_sql_editor-0.1.69a1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/setup.py` & `jupyterlab_sql_editor-0.1.69a1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/src/formatter.ts` & `jupyterlab_sql_editor-0.1.69a1/src/formatter.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/src/index.ts` & `jupyterlab_sql_editor-0.1.69a1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/src/utils.ts` & `jupyterlab_sql_editor-0.1.69a1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/tsconfig.json` & `jupyterlab_sql_editor-0.1.69a1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_sql_editor-0.1.69/yarn.lock` & `jupyterlab_sql_editor-0.1.69a1/yarn.lock`

 * *Files identical despite different names*

