# Comparing `tmp/lightning-app-2.0.4.tar.gz` & `tmp/lightning-app-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.0.4.tar", last modified: Thu Jun 22 18:24:49 2023, max compression
+gzip compressed data, was "lightning-app-2.0.5.tar", last modified: Mon Jul 10 16:10:51 2023, max compression
```

## Comparing `lightning-app-2.0.4.tar` & `lightning-app-2.0.5.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-22 18:24:35.000000 lightning-app-2.0.4/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-22 18:24:35.000000 lightning-app-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-22 18:24:49.249991 lightning-app-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-22 18:24:35.000000 lightning-app-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-22 18:24:36.000000 lightning-app-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.217990 lightning-app-2.0.4/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:24:49.249991 lightning-app-2.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-22 18:24:36.000000 lightning-app-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (123)    34000 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.217990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_react_ui_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.217990 lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/maverick.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-22 18:24:46.000000 lightning-app-2.0.4/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/perf/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/perf/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    45732 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.245990 lightning-app-2.0.4/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.543984 lightning-app-2.0.5/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-10 16:10:36.000000 lightning-app-2.0.5/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-10 16:10:36.000000 lightning-app-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 16:10:51.591985 lightning-app-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-07-10 16:10:36.000000 lightning-app-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-10 16:10:36.000000 lightning-app-2.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.535984 lightning-app-2.0.5/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.543984 lightning-app-2.0.5/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:10:51.591985 lightning-app-2.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-07-10 16:10:36.000000 lightning-app-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.543984 lightning-app-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.547984 lightning-app-2.0.5/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.547984 lightning-app-2.0.5/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.539984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_react_ui_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.539984 lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/maverick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-07-10 16:10:48.000000 lightning-app-2.0.5/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/perf/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47270 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.579985 lightning-app-2.0.5/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.579985 lightning-app-2.0.5/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.583984 lightning-app-2.0.5/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.547984 lightning-app-2.0.5/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/version.info
```

### Comparing `lightning-app-2.0.4/.actions/assistant.py` & `lightning-app-2.0.5/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/LICENSE` & `lightning-app-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/PKG-INFO` & `lightning-app-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.4
+Version: 2.0.5
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: cloud
 Provides-Extra: ui
+Provides-Extra: cloud
 Provides-Extra: components
+Provides-Extra: test
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
@@ -48,15 +48,15 @@
   <a href="#getting-started">Getting started</a> •
   <a href="#asking-for-help">Help</a> •
   <a href="https://www.pytorchlightning.ai/community">Slack</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning_app)](https://pypi.org/project/lightning_app/)
 [![PyPI Status](https://badge.fury.io/py/lightning_app.svg)](https://badge.fury.io/py/lightning_app)
-[![PyPI Status](https://pepy.tech/badge/lightning_app)](https://pepy.tech/project/lightning_app)
+[![PyPI Status](https://pepy.tech/badge/lightning-app)](https://pepy.tech/project/lightning-app)
 [![Conda](https://img.shields.io/conda/v/conda-forge/lightning_app?label=conda&color=success)](https://anaconda.org/conda-forge/lightning_app)
 
 ![readme-gif](https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/lightning-gif-888777nslpiijdbcvctyvwhe.gif)
 
 </div>
 
 ## From production-ready, multi-cloud ML systems to simple research demos.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.4 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.5 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -10,27 +10,27 @@
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: test Provides-Extra: cloud
-Provides-Extra: ui Provides-Extra: components Provides-Extra: extra Provides-
-Extra: all Provides-Extra: dev License-File: LICENSE
+Content-Type: text/markdown Provides-Extra: ui Provides-Extra: cloud Provides-
+Extra: components Provides-Extra: test Provides-Extra: extra Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
 //badge.fury.io/py/lightning_app.svg)](https://badge.fury.io/py/lightning_app)
-  [![PyPI Status](https://pepy.tech/badge/lightning_app)](https://pepy.tech/
- project/lightning_app) [![Conda](https://img.shields.io/conda/v/conda-forge/
+  [![PyPI Status](https://pepy.tech/badge/lightning-app)](https://pepy.tech/
+ project/lightning-app) [![Conda](https://img.shields.io/conda/v/conda-forge/
   lightning_app?label=conda&color=success)](https://anaconda.org/conda-forge/
      lightning_app) ![readme-gif](https://pl-bolts-doc-images.s3.us-east-
           2.amazonaws.com/lightning-gif-888777nslpiijdbcvctyvwhe.gif)
 ## From production-ready, multi-cloud ML systems to simple research demos.
 Lightning Apps enable researchers, data scientists, and software engineers to
 build, share and iterate on highly scalable, complex AI workflows using the
 tools and technologies of their choice without any of the cloud boilerplate.
```

### Comparing `lightning-app-2.0.4/README.md` & `lightning-app-2.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 **The Deep Learning framework to train, deploy, and ship AI products Lightning fast.**
 
 **NEW- Lightning 2.0 is featuring a clean and stable API!!**
 
 ______________________________________________________________________
 
 <p align="center">
-  <a href="https://www.lightning.ai/">Lightning.ai</a> •
+  <a href="https://lightning.ai/">Lightning.ai</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/">PyTorch Lightning</a> •
   <a href="https://lightning.ai/docs/fabric/stable/">Fabric</a> •
   <a href="https://lightning.ai/docs/app/stable/">Lightning Apps</a> •
   <a href="https://pytorch-lightning.readthedocs.io/en/stable/">Docs</a> •
   <a href="#community">Community</a> •
   <a href="https://lightning.ai/docs/pytorch/stable/generated/CONTRIBUTING.html">Contribute</a> •
 </p>
```

### Comparing `lightning-app-2.0.4/pyproject.toml` & `lightning-app-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [metadata]
-name = "pytorch-lightning"
+name = "lightning"
 author = "Lightning-AI et al."
 url = "https://github.com/Lightning-AI/lightning"
 
 [build-system]
 requires = [
     "setuptools",
     "wheel",
```

### Comparing `lightning-app-2.0.4/requirements/app/base.txt` & `lightning-app-2.0.5/requirements/app/base.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-lightning-cloud >=0.5.34
+lightning-cloud >=0.5.37
 packaging
 typing-extensions >=4.0.0, <=4.4.0
 deepdiff >=5.7.0, <6.3.1
 starsessions >=1.2.1, <2.0 # strict
-fsspec >=2022.5.0, <=2022.7.1
-croniter >=1.3.0, <1.4.0  # strict; TODO: for now until we find something more robust.
+fsspec >=2022.5.0, <=2023.6.0
+croniter >=1.3.0, <1.5.0  # strict; TODO: for now until we find something more robust.
 traitlets >=5.3.0, <5.10.0
 arrow >=1.2.0, <1.2.4
-lightning-utilities >=0.7.0, <0.9.0
+lightning-utilities >=0.7.0, <0.10.0
 beautifulsoup4 >=4.8.0, <4.12.3
 inquirer >=2.10.0, <=3.1.3
 psutil <5.9.5
 click <=8.1.3
 python-multipart>=0.0.5, <=0.0.6
+backoff >=2.2.1, <2.3.0
 
-fastapi >=0.92.0, <0.98.0
+fastapi >=0.92.0, <0.100.0
 starlette  # https://fastapi.tiangolo.com/deployment/versions/#about-starlette
-pydantic >=1.7.4, <2.0.0  # https://fastapi.tiangolo.com/deployment/versions/#about-pydantic
+pydantic >=1.7.4, <2.0.0  # strict # https://fastapi.tiangolo.com/deployment/versions/#about-pydantic
 
 dateutils <=0.6.12
 Jinja2 <=3.1.2
 PyYAML <=6.0
 requests <2.31.1
 rich >=12.3.0, <=13.4.2
 urllib3 <=2.0.2
 uvicorn <=0.22.0
-websocket-client <1.5.3
-websockets <=10.4
+websocket-client <1.6.2
+websockets <=11.0.3
```

### Comparing `lightning-app-2.0.4/setup.py` & `lightning-app-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/CHANGELOG.md` & `lightning-app-2.0.5/src/lightning_app/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.5] - 2023-07-07
+
+### Added
+
+- plugin: store source app ([#17892](https://github.com/Lightning-AI/lightning/pull/17892))
+- added colocation identifier ([#16796](https://github.com/Lightning-AI/lightning/pull/16796))
+- Added exponential backoff to HTTPQueue put ([#18013](https://github.com/Lightning-AI/lightning/pull/18013))
+- Content for plugins ([#17243](https://github.com/Lightning-AI/lightning/pull/17243))
+
+### Changed
+
+- Save a reference to created tasks, to avoid tasks disappearing ([#17946](https://github.com/Lightning-AI/lightning/pull/17946))
+
+
 ## [2.0.4] - 2023-06-22
 
 ### Fixed
 
-- bumped several dependencies to address security volnebilities.
+- bumped several dependencies to address security vulnerabilities.
 
 
 ## [2.0.3] - 2023-06-07
 
 - Added the property `LightningWork.public_ip` that exposes the public IP of the `LightningWork` instance ([#17742](https://github.com/Lightning-AI/lightning/pull/17742))
 - Add missing python-multipart dependency ([#17244](https://github.com/Lightning-AI/lightning/pull/17244))
```

### Comparing `lightning-app-2.0.4/src/lightning_app/README.md` & `lightning-app-2.0.5/src/lightning_app/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   <a href="#getting-started">Getting started</a> •
   <a href="#asking-for-help">Help</a> •
   <a href="https://www.pytorchlightning.ai/community">Slack</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning_app)](https://pypi.org/project/lightning_app/)
 [![PyPI Status](https://badge.fury.io/py/lightning_app.svg)](https://badge.fury.io/py/lightning_app)
-[![PyPI Status](https://pepy.tech/badge/lightning_app)](https://pepy.tech/project/lightning_app)
+[![PyPI Status](https://pepy.tech/badge/lightning-app)](https://pepy.tech/project/lightning-app)
 [![Conda](https://img.shields.io/conda/v/conda-forge/lightning_app?label=conda&color=success)](https://anaconda.org/conda-forge/lightning_app)
 
 ![readme-gif](https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/lightning-gif-888777nslpiijdbcvctyvwhe.gif)
 
 </div>
 
 ## From production-ready, multi-cloud ML systems to simple research demos.
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
 //badge.fury.io/py/lightning_app.svg)](https://badge.fury.io/py/lightning_app)
-  [![PyPI Status](https://pepy.tech/badge/lightning_app)](https://pepy.tech/
- project/lightning_app) [![Conda](https://img.shields.io/conda/v/conda-forge/
+  [![PyPI Status](https://pepy.tech/badge/lightning-app)](https://pepy.tech/
+ project/lightning-app) [![Conda](https://img.shields.io/conda/v/conda-forge/
   lightning_app?label=conda&color=success)](https://anaconda.org/conda-forge/
      lightning_app) ![readme-gif](https://pl-bolts-doc-images.s3.us-east-
           2.amazonaws.com/lightning-gif-888777nslpiijdbcvctyvwhe.gif)
 ## From production-ready, multi-cloud ML systems to simple research demos.
 Lightning Apps enable researchers, data scientists, and software engineers to
 build, share and iterate on highly scalable, complex AI workflows using the
 tools and technologies of their choice without any of the cloud boilerplate.
```

### Comparing `lightning-app-2.0.4/src/lightning_app/__about__.py` & `lightning-app-2.0.5/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/__init__.py` & `lightning-app-2.0.5/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/__setup__.py` & `lightning-app-2.0.5/src/lightning_app/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/api/http_methods.py` & `lightning-app-2.0.5/src/lightning_app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/api/request_types.py` & `lightning-app-2.0.5/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.0.5/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.0.5/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.0.5/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_clusters.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/cmd_ssh_keys.py` & `lightning-app-2.0.5/src/lightning_app/cli/cmd_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.0.5/src/lightning_app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.0.5/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.0.5/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.0.5/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/connect/app.py` & `lightning-app-2.0.5/src/lightning_app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/connect/data.py` & `lightning-app-2.0.5/src/lightning_app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/connect/maverick.py` & `lightning-app-2.0.5/src/lightning_app/cli/connect/maverick.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/core.py` & `lightning-app-2.0.5/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_create.py` & `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_create.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/__init__.py` & `lightning-app-2.0.5/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/database/client.py` & `lightning-app-2.0.5/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/database/server.py` & `lightning-app-2.0.5/src/lightning_app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/database/utilities.py` & `lightning-app-2.0.5/src/lightning_app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.0.5/src/lightning_app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.0.5/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.0.5/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.0.5/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/python/popen.py` & `lightning-app-2.0.5/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/python/tracer.py` & `lightning-app-2.0.5/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/auto_scaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,17 @@
             # setting the server status to be busy! This will be reset by
             # the send_batch function after the server responds
             if server_url is None:
                 continue
             if batch and (is_batch_ready or is_batch_timeout):
                 self._server_status[server_url] = False
                 # find server with capacity
-                asyncio.create_task(self.send_batch(batch, server_url))
+                # Saving a reference to the result of this function, protects the task disappearing mid-execution
+                # https://docs.python.org/3/library/asyncio-task.html#asyncio.create_task
+                task = asyncio.create_task(self.send_batch(batch, server_url))  # noqa: F841
                 # resetting the batch array, TODO - not locking the array
                 self._batch = self._batch[len(batch) :]
                 self._last_batch_sent = time.time()
 
     async def process_request(self, data: BaseModel, request_id=None):
         if request_id is None:
             request_id = uuid.uuid4().hex
```

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.0.5/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/serve.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.0.5/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/components/training.py` & `lightning-app-2.0.5/src/lightning_app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/core/api.py` & `lightning-app-2.0.5/src/lightning_app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/core/app.py` & `lightning-app-2.0.5/src/lightning_app/core/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/core/constants.py` & `lightning-app-2.0.5/src/lightning_app/core/constants.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/core/flow.py` & `lightning-app-2.0.5/src/lightning_app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/core/queues.py` & `lightning-app-2.0.5/src/lightning_app/core/queues.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import warnings
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Any, Optional, Tuple
 from urllib.parse import urljoin
 
+import backoff
 import requests
 from requests.exceptions import ConnectionError, ConnectTimeout, ReadTimeout
 
 from lightning_app.core.constants import (
     HTTP_QUEUE_REFRESH_INTERVAL,
     HTTP_QUEUE_TOKEN,
     HTTP_QUEUE_URL,
@@ -427,14 +428,15 @@
                 raise queue.Empty
             return pickle.loads(resp.content)
         except ConnectionError:
             # Note: If the Http Queue service isn't available,
             # we consider the queue is empty to avoid failing the app.
             raise queue.Empty
 
+    @backoff.on_exception(backoff.expo, (RuntimeError, requests.exceptions.HTTPError))
     def put(self, item: Any) -> None:
         if not self.app_id:
             raise ValueError(f"The Lightning App ID couldn't be extracted from the queue name: {self.name}")
 
         value = pickle.dumps(item)
         queue_len = self.length()
         if queue_len >= WARNING_QUEUE_SIZE:
```

### Comparing `lightning-app-2.0.4/src/lightning_app/core/work.py` & `lightning-app-2.0.5/src/lightning_app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/frontend.py` & `lightning-app-2.0.5/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.0.5/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.0.5/src/lightning_app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/utils.py` & `lightning-app-2.0.5/src/lightning_app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/frontend/web.py` & `lightning-app-2.0.5/src/lightning_app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/perf/pdb.py` & `lightning-app-2.0.5/src/lightning_app/perf/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/plugin/actions.py` & `lightning-app-2.0.5/src/lightning_app/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/plugin/plugin.py` & `lightning-app-2.0.5/src/lightning_app/plugin/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     """A ``LightningPlugin`` is a single-file Python class that can be executed within a cloudspace to perform
     actions."""
 
     def __init__(self) -> None:
         self.project_id = ""
         self.cloudspace_id = ""
         self.cluster_id = ""
+        self.source_app = ""
 
     def run(self, *args: str, **kwargs: str) -> Optional[List[_Action]]:
         """Override with the logic to execute on the cloudspace."""
         raise NotImplementedError
 
     def run_job(self, name: str, app_entrypoint: str, env_vars: Dict[str, str] = {}) -> str:
         """Run a job in the cloudspace associated with this plugin.
@@ -56,14 +57,16 @@
             env_vars: Additional env vars to set when running the app.
 
         Returns:
             The relative URL of the created job.
         """
         from lightning_app.runners.cloud import CloudRuntime
 
+        logger.info(f"Processing job run request. name: {name}, app_entrypoint: {app_entrypoint}, env_vars: {env_vars}")
+
         # Dispatch the job
         _set_flow_context()
 
         entrypoint_file = Path(app_entrypoint)
 
         app = CloudRuntime.load_app_from_file(str(entrypoint_file.resolve().absolute()), env_vars=env_vars)
 
@@ -81,47 +84,53 @@
         os.environ["LIGHTNING_DISPATCHED"] = "1"
 
         url = runtime.cloudspace_dispatch(
             project_id=self.project_id,
             cloudspace_id=self.cloudspace_id,
             name=name,
             cluster_id=self.cluster_id,
+            source_app=self.source_app,
         )
         # Return a relative URL so it can be used with the NavigateTo action.
         return url.replace(constants.get_lightning_cloud_url(), "")
 
     def _setup(
         self,
         project_id: str,
         cloudspace_id: str,
         cluster_id: str,
+        source_app: str,
     ) -> None:
+        self.source_app = source_app
         self.project_id = project_id
         self.cloudspace_id = cloudspace_id
         self.cluster_id = cluster_id
 
 
 class _Run(BaseModel):
     plugin_entrypoint: str
     source_code_url: str
     project_id: str
     cloudspace_id: str
     cluster_id: str
     plugin_arguments: Dict[str, str]
+    source_app: str
 
 
 def _run_plugin(run: _Run) -> Dict[str, Any]:
     """Create a run with the given name and entrypoint under the cloudspace with the given ID."""
     with tempfile.TemporaryDirectory() as tmpdir:
         download_path = os.path.join(tmpdir, "source.tar.gz")
         source_path = os.path.join(tmpdir, "source")
         os.makedirs(source_path)
 
         # Download the tarball
         try:
+            logger.info(f"Downloading plugin source: {run.source_code_url}")
+
             # Sometimes the URL gets encoded, so we parse it here
             source_code_url = urlparse(run.source_code_url).geturl()
 
             response = requests.get(source_code_url)
 
             # TODO: Backoff retry a few times in case the URL is flaky
             response.raise_for_status()
@@ -132,40 +141,50 @@
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                 detail=f"Error downloading plugin source: {str(ex)}.",
             )
 
         # Extract
         try:
+            logger.info("Extracting plugin source.")
+
             with tarfile.open(download_path, "r:gz") as tf:
                 tf.extractall(source_path)
         except Exception as ex:
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                 detail=f"Error extracting plugin source: {str(ex)}.",
             )
 
         # Import the plugin
         try:
+            logger.info(f"Importing plugin: {run.plugin_entrypoint}")
+
             plugin = _load_plugin_from_file(os.path.join(source_path, run.plugin_entrypoint))
         except Exception as ex:
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=f"Error loading plugin: {str(ex)}."
             )
 
         # Ensure that apps are dispatched from the temp directory
         cwd = os.getcwd()
         os.chdir(source_path)
 
         # Setup and run the plugin
         try:
+            logger.info(
+                "Running plugin. "
+                f"project_id: {run.project_id}, cloudspace_id: {run.cloudspace_id}, cluster_id: {run.cluster_id}."
+            )
+
             plugin._setup(
                 project_id=run.project_id,
                 cloudspace_id=run.cloudspace_id,
                 cluster_id=run.cluster_id,
+                source_app=run.source_app,
             )
             actions = plugin.run(**run.plugin_arguments) or []
             return {"actions": [action.to_spec().to_dict() for action in actions]}
         except Exception as ex:
             raise HTTPException(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=f"Error running plugin: {str(ex)}."
             )
```

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.0.5/src/lightning_app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.0.5/src/lightning_app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.0.5/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.0.5/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.0.5/src/lightning_app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/cloud.py` & `lightning-app-2.0.5/src/lightning_app/runners/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
 
     def cloudspace_dispatch(
         self,
         project_id: str,
         cloudspace_id: str,
         name: str,
         cluster_id: str,
+        source_app: Optional[str] = None,
     ) -> str:
         """Slim dispatch for creating runs from a cloudspace. This dispatch avoids resolution of some properties
         such as the project and cluster IDs that are instead passed directly.
 
         Args:
             project_id: The ID of the project.
             cloudspace_id: The ID of the cloudspace.
@@ -213,57 +214,73 @@
 
         Returns:
             The URL of the created job.
         """
         # Dispatch in four phases: resolution, validation, spec creation, API transactions
         # Resolution
         root = self._resolve_root()
-        repo = self._resolve_repo(root)
+        # If the root will already be there, we don't need to upload and preserve the absolute entrypoint
+        absolute_entrypoint = str(root).startswith("/project")
+        # If system customization files found, it will set their location path
+        sys_customizations_root = self._resolve_env_root()
+        repo = self._resolve_repo(
+            root,
+            default_ignore=False,
+            package_source=not absolute_entrypoint,
+            sys_customizations_root=sys_customizations_root,
+        )
         project = self._resolve_project(project_id=project_id)
         existing_instances = self._resolve_run_instances_by_name(project_id, name)
         name = self._resolve_run_name(name, existing_instances)
         cloudspace = self._resolve_cloudspace(project_id, cloudspace_id)
         queue_server_type = self._resolve_queue_server_type()
 
-        # If system customization files found, it will set their location path
-        sys_customizations_sync_root = self._resolve_env_root()
-
         self.app._update_index_file()
 
         # Validation
         # TODO: Validate repo and surface to the user
         # self._validate_repo(root, repo)
         self._validate_work_build_specs_and_compute()
         self._validate_drives()
         self._validate_mounts()
 
         # Spec creation
         flow_servers = self._get_flow_servers()
         network_configs = self._get_network_configs(flow_servers)
         works = self._get_works(cloudspace=cloudspace)
-        run_body = self._get_run_body(cluster_id, flow_servers, network_configs, works, False, root, True)
+        run_body = self._get_run_body(
+            cluster_id,
+            flow_servers,
+            network_configs,
+            works,
+            False,
+            root,
+            True,
+            True,
+            absolute_entrypoint,
+        )
         env_vars = self._get_env_vars(self.env_vars, self.secrets, self.run_app_comment_commands)
 
-        # If the system customization root is set, prepare files for environment synchronization
-        if sys_customizations_sync_root is not None:
-            repo.prepare_sys_customizations_sync(sys_customizations_sync_root)
-
         # API transactions
+        logger.info(f"Creating cloudspace run. run_body: {run_body}")
         run = self._api_create_run(project_id, cloudspace_id, run_body)
+
         self._api_package_and_upload_repo(repo, run)
 
+        logger.info(f"Creating cloudspace run instance. name: {name}")
         run_instance = self._api_create_run_instance(
             cluster_id,
             project_id,
             name,
             cloudspace_id,
             run.id,
             V1LightningappInstanceState.RUNNING,
             queue_server_type,
             env_vars,
+            source_app=source_app,
         )
 
         return self._get_app_url(project, run_instance, "logs" if run.is_headless else "web-ui")
 
     def dispatch(
         self,
         name: str = "",
@@ -448,14 +465,17 @@
             return [lambda src, paths: [path for path in paths if path.absolute() == entrypoint]]
         return []
 
     def _resolve_repo(
         self,
         root: Path,
         ignore_functions: Optional[List[_IGNORE_FUNCTION]] = None,
+        default_ignore: bool = True,
+        package_source: bool = True,
+        sys_customizations_root: Optional[Path] = None,
     ) -> LocalSourceCodeDir:
         """Gather and merge all lightningignores from the app children and create the ``LocalSourceCodeDir``
         object."""
         if ignore_functions is None:
             ignore_functions = []
 
         if self.app is not None:
@@ -464,15 +484,21 @@
             lightningignores = flow_lightningignores + work_lightningignores
             if lightningignores:
                 merged = sum(lightningignores, ())
                 logger.debug(f"Found the following lightningignores: {merged}")
                 patterns = _parse_lightningignore(merged)
                 ignore_functions = [*ignore_functions, partial(_filter_ignored, root, patterns)]
 
-        return LocalSourceCodeDir(path=root, ignore_functions=ignore_functions)
+        return LocalSourceCodeDir(
+            path=root,
+            ignore_functions=ignore_functions,
+            default_ignore=default_ignore,
+            package_source=package_source,
+            sys_customizations_root=sys_customizations_root,
+        )
 
     def _resolve_project(self, project_id: Optional[str] = None) -> V1Membership:
         """Determine the project to run on, choosing a default if multiple projects are found."""
         return _get_project(self.backend.client, project_id=project_id)
 
     def _resolve_existing_cloudspaces(self, project_id: str, cloudspace_name: str) -> List[V1CloudSpace]:
         """Lists all the cloudspaces with a name matching the provided cloudspace name."""
@@ -761,14 +787,15 @@
             )
             user_compute_config = V1UserRequestedComputeConfig(
                 name=work.cloud_compute.name,
                 count=1,
                 disk_size=work.cloud_compute.disk_size,
                 preemptible=work.cloud_compute.interruptible,
                 shm_size=work.cloud_compute.shm_size,
+                affinity_identifier=work.cloud_compute.colocation_group_id,
             )
 
             drives = self._get_drives(work)
             mounts = self._get_mounts(work)
 
             data_connection_mounts: list[V1DataConnectionMount] = []
             if cloudspace is not None and cloudspace.code_config is not None:
@@ -778,59 +805,67 @@
             work_spec = V1LightningworkSpec(
                 build_spec=build_spec,
                 drives=drives + mounts,
                 user_requested_compute_config=user_compute_config,
                 network_config=[V1NetworkConfig(name=random_name, port=work.port)],
                 data_connection_mounts=data_connection_mounts,
             )
-            works.append(V1Work(name=work.name, spec=work_spec))
+            works.append(V1Work(name=work.name, display_name=work.display_name, spec=work_spec))
 
         return works
 
     def _get_run_body(
         self,
         cluster_id: str,
         flow_servers: List[V1Flowserver],
         network_configs: Optional[List[V1NetworkConfig]],
         works: List[V1Work],
         no_cache: bool,
         root: Path,
         start_server: bool,
+        should_mount_cloudspace_content: bool = False,
+        absolute_entrypoint: bool = False,
     ) -> CloudspaceIdRunsBody:
         """Get the specification of the run creation request."""
-        # The entry point file needs to be relative to the root of the uploaded source file directory,
-        # because the backend will invoke the lightning commands relative said source directory
-        # TODO: we shouldn't set this if the entrypoint isn't a file but the backend gives an error if we don't
-        app_entrypoint_file = Path(self.entrypoint).absolute().relative_to(root)
+        if absolute_entrypoint:
+            # If the entrypoint will already exist in the cloud then we can choose to keep it as an absolute path.
+            app_entrypoint_file = Path(self.entrypoint).absolute()
+        else:
+            # The entry point file needs to be relative to the root of the uploaded source file directory,
+            # because the backend will invoke the lightning commands relative said source directory
+            # TODO: we shouldn't set this if the entrypoint isn't a file but the backend gives an error if we don't
+            app_entrypoint_file = Path(self.entrypoint).absolute().relative_to(root)
 
         run_body = CloudspaceIdRunsBody(
             cluster_id=cluster_id,
             app_entrypoint_file=str(app_entrypoint_file),
             enable_app_server=start_server,
             flow_servers=flow_servers,
             network_config=network_configs,
             works=works,
             local_source=True,
+            should_mount_cloudspace_content=should_mount_cloudspace_content,
         )
 
         if self.app is not None:
             run_body.user_requested_flow_compute_config = V1UserRequestedFlowComputeConfig(
                 name=self.app.flow_cloud_compute.name,
                 shm_size=self.app.flow_cloud_compute.shm_size,
                 preemptible=False,
             )
 
             run_body.is_headless = _is_headless(self.app)
 
         # if requirements file at the root of the repository is present,
         # we pass just the file name to the backend, so backend can find it in the relative path
         requirements_file = root / "requirements.txt"
-        if requirements_file.is_file():
+        if requirements_file.is_file() and requirements_file.exists():
+            requirements_path = requirements_file if absolute_entrypoint else "requirements.txt"
             run_body.image_spec = Gridv1ImageSpec(
-                dependency_file_info=V1DependencyFileInfo(package_manager=V1PackageManager.PIP, path="requirements.txt")
+                dependency_file_info=V1DependencyFileInfo(package_manager=V1PackageManager.PIP, path=requirements_path)
             )
             if not DISABLE_DEPENDENCY_CACHE and not no_cache:
                 # hash used for caching the dependencies
                 run_body.dependency_cache_key = get_hash(requirements_file)
 
         return run_body
 
@@ -971,32 +1006,37 @@
         run_name: str,
         cloudspace_id: str,
         run_id: str,
         desired_state: V1LightningappInstanceState,
         queue_server_type: Optional[V1QueueServerType] = None,
         env_vars: Optional[List[V1EnvVar]] = None,
         auth: Optional[V1LightningAuth] = None,
+        source_app: Optional[str] = None,
     ) -> Externalv1LightningappInstance:
         """Create a new instance of the given run with the given specification."""
         return self.backend.client.cloud_space_service_create_lightning_run_instance(
             project_id=project_id,
             cloudspace_id=cloudspace_id,
             id=run_id,
             body=IdGetBody1(
                 cluster_id=cluster_id,
                 name=run_name,
                 desired_state=desired_state,
                 queue_server_type=queue_server_type,
                 env=env_vars,
                 auth=auth,
+                source_app=source_app,
             ),
         )
 
     @staticmethod
-    def _api_package_and_upload_repo(repo: LocalSourceCodeDir, run: V1LightningRun) -> None:
+    def _api_package_and_upload_repo(
+        repo: LocalSourceCodeDir,
+        run: V1LightningRun,
+    ) -> None:
         """Package and upload the provided local source code directory to the provided run."""
         if run.source_upload_url == "":
             raise RuntimeError("The source upload url is empty.")
         repo.package()
         repo.upload(url=run.source_upload_url)
 
     @staticmethod
```

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.0.5/src/lightning_app/runners/multiprocess.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/runtime.py` & `lightning-app-2.0.5/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.0.5/src/lightning_app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/source_code/copytree.py` & `lightning-app-2.0.5/src/lightning_app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/source_code/hashing.py` & `lightning-app-2.0.5/src/lightning_app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/source_code/local.py` & `lightning-app-2.0.5/src/lightning_app/source_code/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,85 +9,107 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import uuid
 from contextlib import contextmanager
 from pathlib import Path
 from shutil import copytree, rmtree
 from typing import List, Optional
 
 from lightning_app.core.constants import DOT_IGNORE_FILENAME, SYS_CUSTOMIZATIONS_SYNC_PATH
 from lightning_app.source_code.copytree import _copytree, _IGNORE_FUNCTION
-from lightning_app.source_code.hashing import _get_hash
 from lightning_app.source_code.tar import _tar_path
 from lightning_app.source_code.uploader import FileUploader
 
 
 class LocalSourceCodeDir:
     """Represents the source code directory and provide the utilities to manage it."""
 
     cache_location: Path = Path.home() / ".lightning" / "cache" / "repositories"
 
-    def __init__(self, path: Path, ignore_functions: Optional[List[_IGNORE_FUNCTION]] = None) -> None:
+    def __init__(
+        self,
+        path: Path,
+        ignore_functions: Optional[List[_IGNORE_FUNCTION]] = None,
+        default_ignore: bool = True,
+        package_source: bool = True,
+        sys_customizations_root: Optional[Path] = None,
+    ) -> None:
+        if "LIGHTNING_VSCODE_WORKSPACE" in os.environ:
+            # Don't use home to store the tar ball. This won't play nice with symlinks
+            self.cache_location: Path = Path("/tmp", ".lightning", "cache", "repositories")  # noqa: S108
+        else:
+            self.cache_location: Path = Path.home() / ".lightning" / "cache" / "repositories"
+
         self.path = path
         self.ignore_functions = ignore_functions
+        self.package_source = package_source
+        self.sys_customizations_root = sys_customizations_root
 
-        # cache checksum version
+        # cache version
         self._version: Optional[str] = None
         self._non_ignored_files: Optional[List[str]] = None
 
         # create global cache location if it doesn't exist
         if not self.cache_location.exists():
             self.cache_location.mkdir(parents=True, exist_ok=True)
 
-        # Create a default dotignore if it doesn't exist
-        if not (path / DOT_IGNORE_FILENAME).is_file():
+        # Create a default dotignore if requested and it doesn't exist
+        if default_ignore and not (path / DOT_IGNORE_FILENAME).is_file():
             with open(path / DOT_IGNORE_FILENAME, "w") as f:
                 f.write("venv/\n")
                 if (path / "bin" / "activate").is_file() or (path / "pyvenv.cfg").is_file():
                     # the user is developing inside venv
                     f.write("bin/\ninclude/\nlib/\npyvenv.cfg\n")
 
         # clean old cache entries
         self._prune_cache()
 
     @property
     def files(self) -> List[str]:
         """Returns a set of files that are not ignored by .lightningignore."""
         if self._non_ignored_files is None:
-            self._non_ignored_files = _copytree(self.path, "", ignore_functions=self.ignore_functions, dry_run=True)
+            if self.package_source:
+                self._non_ignored_files = _copytree(self.path, "", ignore_functions=self.ignore_functions, dry_run=True)
+            else:
+                self._non_ignored_files = []
         return self._non_ignored_files
 
     @property
     def version(self):
         """Calculates the checksum of a local path."""
         # cache value to prevent doing this over again
         if self._version is not None:
             return self._version
 
-        # stores both version and a set with the files used to generate the checksum
-        self._version = _get_hash(files=self.files, algorithm="blake2")
+        # create a random version ID and store it
+        self._version = uuid.uuid4().hex
         return self._version
 
     @property
     def package_path(self):
         """Location to tarball in local cache."""
         filename = f"{self.version}.tar.gz"
         return self.cache_location / filename
 
     @contextmanager
     def packaging_session(self) -> Path:
         """Creates a local directory with source code that is used for creating a local source-code package."""
         session_path = self.cache_location / "packaging_sessions" / self.version
         try:
             rmtree(session_path, ignore_errors=True)
-            _copytree(self.path, session_path, ignore_functions=self.ignore_functions)
+            if self.package_source:
+                _copytree(self.path, session_path, ignore_functions=self.ignore_functions)
+            if self.sys_customizations_root is not None:
+                path_to_sync = Path(session_path, SYS_CUSTOMIZATIONS_SYNC_PATH)
+                copytree(self.sys_customizations_root, path_to_sync, dirs_exist_ok=True)
             yield session_path
         finally:
             rmtree(session_path, ignore_errors=True)
 
     def _prune_cache(self) -> None:
         """Prunes cache; only keeps the 10 most recent items."""
         packages = sorted(self.cache_location.iterdir(), key=os.path.getmtime)
@@ -100,20 +122,14 @@
         if self.package_path.exists():
             return self.package_path
         # create a packaging session if not available
         with self.packaging_session() as session_path:
             _tar_path(source_path=session_path, target_file=str(self.package_path), compression=True)
         return self.package_path
 
-    def prepare_sys_customizations_sync(self, sys_customizations_root: Path) -> None:
-        """Prepares files for system environment customization setup by copying conda and system environment files
-        to an app files directory."""
-        path_to_sync = Path(self.path, SYS_CUSTOMIZATIONS_SYNC_PATH)
-        copytree(sys_customizations_root, path_to_sync, dirs_exist_ok=True)
-
     def upload(self, url: str) -> None:
         """Uploads package to URL, usually pre-signed URL.
 
         Notes
         -----
         Since we do not use multipart uploads here, we cannot upload any
         packaged repository files which have a size > 2GB.
```

### Comparing `lightning-app-2.0.4/src/lightning_app/source_code/tar.py` & `lightning-app-2.0.5/src/lightning_app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/source_code/uploader.py` & `lightning-app-2.0.5/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/copier.py` & `lightning-app-2.0.5/src/lightning_app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/drive.py` & `lightning-app-2.0.5/src/lightning_app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/filesystem.py` & `lightning-app-2.0.5/src/lightning_app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/mount.py` & `lightning-app-2.0.5/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.0.5/src/lightning_app/storage/orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,21 @@
         self.waiting_for_response: Dict[str, str] = {}
         self._validate_queues()
         self._exit_event = threading.Event()
 
         # Note: Use different sleep time locally and in the cloud
         # to reduce queue calls.
         self._sleep_time = 0.1 if "LIGHTNING_APP_STATE_URL" not in os.environ else 2
-        self.fs = _filesystem()
+        self._fs = None
+
+    @property
+    def fs(self):
+        if self._fs is None:
+            self._fs = _filesystem()
+        return self._fs
 
     def _validate_queues(self):
         assert (
             self.request_queues.keys()
             == self.response_queues.keys()
             == self.copy_request_queues.keys()
             == self.copy_response_queues.keys()
```

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/path.py` & `lightning-app-2.0.5/src/lightning_app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/payload.py` & `lightning-app-2.0.5/src/lightning_app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/storage/requests.py` & `lightning-app-2.0.5/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/structures/dict.py` & `lightning-app-2.0.5/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/structures/list.py` & `lightning-app-2.0.5/src/lightning_app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/testing/config.py` & `lightning-app-2.0.5/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/testing/helpers.py` & `lightning-app-2.0.5/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/testing/testing.py` & `lightning-app-2.0.5/src/lightning_app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.0.5/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/index.html` & `lightning-app-2.0.5/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css` & `lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css.map` & `lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.0.5/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js` & `lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt` & `lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.map` & `lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.0.5/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.0.5/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.0.5/src/lightning_app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.0.5/src/lightning_app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.0.5/src/lightning_app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/app_status.py` & `lightning-app-2.0.5/src/lightning_app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/auth.py` & `lightning-app-2.0.5/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.0.5/src/lightning_app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/cloud.py` & `lightning-app-2.0.5/src/lightning_app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/cluster_logs.py` & `lightning-app-2.0.5/src/lightning_app/utilities/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/clusters.py` & `lightning-app-2.0.5/src/lightning_app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.0.5/src/lightning_app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/component.py` & `lightning-app-2.0.5/src/lightning_app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.0.5/src/lightning_app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.0.5/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/enum.py` & `lightning-app-2.0.5/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.0.5/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/frontend.py` & `lightning-app-2.0.5/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/git.py` & `lightning-app-2.0.5/src/lightning_app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/imports.py` & `lightning-app-2.0.5/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/introspection.py` & `lightning-app-2.0.5/src/lightning_app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/layout.py` & `lightning-app-2.0.5/src/lightning_app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/load_app.py` & `lightning-app-2.0.5/src/lightning_app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/log.py` & `lightning-app-2.0.5/src/lightning_app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.0.5/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/login.py` & `lightning-app-2.0.5/src/lightning_app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.0.5/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.0.5/src/lightning_app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/network.py` & `lightning-app-2.0.5/src/lightning_app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/openapi.py` & `lightning-app-2.0.5/src/lightning_app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.0.5/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.0.5/src/lightning_app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.0.5/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,24 +77,29 @@
             If the timeout is reached, the instance pauses until the next run() call happens.
 
         shm_size: Shared memory size in MiB, backed by RAM. min 512, max 8192, it will auto update in steps of 512.
             For example 1100 will become 1024. If set to zero (the default) will get the default 64MiB inside docker.
 
         mounts: External data sources which should be mounted into a work as a filesystem at runtime.
 
+        colocation_group_id: Identifier for groups of works to be colocated in the same datacenter.
+            Set this to a string of max. 64 characters and all works with this group id will run in the same datacenter.
+            If not set, the works are not guaranteed to be colocated.
+
         interruptible: Whether to run on a interruptible machine e.g the machine can be stopped
             at any time by the providers. This is also known as spot or preemptible machines.
             Compared to on-demand machines, they tend to be cheaper.
     """
 
     name: str = "default"
     disk_size: int = 0
     idle_timeout: Optional[int] = None
     shm_size: Optional[int] = None
     mounts: Optional[Union[Mount, List[Mount]]] = None
+    colocation_group_id: Optional[str] = None
     interruptible: bool = False
     _internal_id: Optional[str] = None
 
     def __post_init__(self) -> None:
         _verify_mount_root_dirs_are_unique(self.mounts)
 
         self.name = self.name.lower()
@@ -119,14 +124,20 @@
         # TODO: Remove from the platform first.
         self.preemptible = self.interruptible
 
         # All `default` CloudCompute are identified in the same way.
         if self._internal_id is None:
             self._internal_id = self._generate_id()
 
+        if self.colocation_group_id is not None and (
+            not isinstance(self.colocation_group_id, str)
+            or (isinstance(self.colocation_group_id, str) and len(self.colocation_group_id) > 64)
+        ):
+            raise ValueError("colocation_group_id can only be a string of maximum 64 characters.")
+
     def to_dict(self) -> dict:
         _verify_mount_root_dirs_are_unique(self.mounts)
         return {"type": __CLOUD_COMPUTE_IDENTIFIER__, **asdict(self)}
 
     @classmethod
     def from_dict(cls, d: dict) -> "CloudCompute":
         assert d.pop("type") == __CLOUD_COMPUTE_IDENTIFIER__
```

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.0.5/src/lightning_app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.0.5/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.0.5/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/port.py` & `lightning-app-2.0.5/src/lightning_app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/proxies.py` & `lightning-app-2.0.5/src/lightning_app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/redis.py` & `lightning-app-2.0.5/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.0.5/src/lightning_app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.0.5/src/lightning_app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/secrets.py` & `lightning-app-2.0.5/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/state.py` & `lightning-app-2.0.5/src/lightning_app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/tracer.py` & `lightning-app-2.0.5/src/lightning_app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/tree.py` & `lightning-app-2.0.5/src/lightning_app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/types.py` & `lightning-app-2.0.5/src/lightning_app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app/utilities/warnings.py` & `lightning-app-2.0.5/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.0.5/src/lightning_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.4
+Version: 2.0.5
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: cloud
 Provides-Extra: ui
+Provides-Extra: cloud
 Provides-Extra: components
+Provides-Extra: test
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
@@ -48,15 +48,15 @@
   <a href="#getting-started">Getting started</a> •
   <a href="#asking-for-help">Help</a> •
   <a href="https://www.pytorchlightning.ai/community">Slack</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lightning_app)](https://pypi.org/project/lightning_app/)
 [![PyPI Status](https://badge.fury.io/py/lightning_app.svg)](https://badge.fury.io/py/lightning_app)
-[![PyPI Status](https://pepy.tech/badge/lightning_app)](https://pepy.tech/project/lightning_app)
+[![PyPI Status](https://pepy.tech/badge/lightning-app)](https://pepy.tech/project/lightning-app)
 [![Conda](https://img.shields.io/conda/v/conda-forge/lightning_app?label=conda&color=success)](https://anaconda.org/conda-forge/lightning_app)
 
 ![readme-gif](https://pl-bolts-doc-images.s3.us-east-2.amazonaws.com/lightning-gif-888777nslpiijdbcvctyvwhe.gif)
 
 </div>
 
 ## From production-ready, multi-cloud ML systems to simple research demos.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.4 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.5 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -10,27 +10,27 @@
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: test Provides-Extra: cloud
-Provides-Extra: ui Provides-Extra: components Provides-Extra: extra Provides-
-Extra: all Provides-Extra: dev License-File: LICENSE
+Content-Type: text/markdown Provides-Extra: ui Provides-Extra: cloud Provides-
+Extra: components Provides-Extra: test Provides-Extra: extra Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
 //badge.fury.io/py/lightning_app.svg)](https://badge.fury.io/py/lightning_app)
-  [![PyPI Status](https://pepy.tech/badge/lightning_app)](https://pepy.tech/
- project/lightning_app) [![Conda](https://img.shields.io/conda/v/conda-forge/
+  [![PyPI Status](https://pepy.tech/badge/lightning-app)](https://pepy.tech/
+ project/lightning-app) [![Conda](https://img.shields.io/conda/v/conda-forge/
   lightning_app?label=conda&color=success)](https://anaconda.org/conda-forge/
      lightning_app) ![readme-gif](https://pl-bolts-doc-images.s3.us-east-
           2.amazonaws.com/lightning-gif-888777nslpiijdbcvctyvwhe.gif)
 ## From production-ready, multi-cloud ML systems to simple research demos.
 Lightning Apps enable researchers, data scientists, and software engineers to
 build, share and iterate on highly scalable, complex AI workflows using the
 tools and technologies of their choice without any of the cloud boilerplate.
```

### Comparing `lightning-app-2.0.4/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.0.5/src/lightning_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.4/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.0.5/src/lightning_app.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-lightning-cloud>=0.5.34
+lightning-cloud>=0.5.37
 packaging
 typing-extensions<5.0,>=4.0.0
 deepdiff<7.0,>=5.7.0
 starsessions<2.0,>=1.2.1
-fsspec<2023.0,>=2022.5.0
-croniter<1.4.0,>=1.3.0
+fsspec<2024.0,>=2022.5.0
+croniter<1.5.0,>=1.3.0
 traitlets<6.0,>=5.3.0
 arrow<2.0,>=1.2.0
 lightning-utilities<1.0,>=0.7.0
 beautifulsoup4<5.0,>=4.8.0
 inquirer<4.0,>=2.10.0
 psutil<6.0
 click<9.0
 python-multipart<1.0,>=0.0.5
+backoff<3.0,>=2.2.1
 fastapi<1.0,>=0.92.0
 starlette
-pydantic<3.0,>=1.7.4
+pydantic<2.0.0,>=1.7.4
 dateutils<1.0
 Jinja2<4.0
 PyYAML<7.0
 requests<3.0
 rich<14.0,>=12.3.0
 urllib3<3.0
 uvicorn<1.0
 websocket-client<2.0
-websockets<11.0
+websockets<12.0
 
 [all]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
 s3fs<2024.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
 panel<2.0,>=1.0.0
@@ -54,15 +55,15 @@
 s3fs<2024.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
 panel<2.0,>=1.0.0
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
-coverage==7.2.5
+coverage==7.2.7
 pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.21.0
 pytest-rerunfailures<12.0
 playwright==1.35.0
@@ -81,15 +82,15 @@
 panel<2.0,>=1.0.0
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 
 [test]
-coverage==7.2.5
+coverage==7.2.7
 pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.21.0
 pytest-rerunfailures<12.0
 playwright==1.35.0
```

