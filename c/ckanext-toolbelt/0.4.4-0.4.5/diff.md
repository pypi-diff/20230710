# Comparing `tmp/ckanext-toolbelt-0.4.4.tar.gz` & `tmp/ckanext-toolbelt-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-toolbelt-0.4.4.tar", last modified: Mon Jul 10 18:40:21 2023, max compression
+gzip compressed data, was "ckanext-toolbelt-0.4.5.tar", last modified: Mon Jul 10 18:36:56 2023, max compression
```

## Comparing `ckanext-toolbelt-0.4.4.tar` & `ckanext-toolbelt-0.4.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.174864 ckanext-toolbelt-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34500 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-10 18:40:21.174864 ckanext-toolbelt-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.166864 ckanext-toolbelt-0.4.4/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.166864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.166864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.166864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/ckan/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/ckan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/ckan/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/ckan/search_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_gh_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.166864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/magic/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/magic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/cascade_organization_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/fdt_scroll/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/fdt_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/group_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/group_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/safe_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/types/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/scheming.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:21.170864 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 18:40:21.000000 ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-10 18:40:21.174864 ckanext-toolbelt-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-10 18:40:10.000000 ckanext-toolbelt-0.4.4/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.5/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      223 2023-06-10 18:22:10.000000 ckanext-toolbelt-0.4.5/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7449 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6769 2023-06-05 13:45:47.000000 ckanext-toolbelt-0.4.5/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      190 2023-06-15 13:56:03.000000 ckanext-toolbelt-0.4.5/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      224 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1472 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/_shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/ckan/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/ckan/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1285 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/ckan/db.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1378 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/ckan/search_index.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1397 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/dev.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      368 2023-04-03 09:57:56.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2108 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1371 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_gh_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1824 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_readme.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2346 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_template.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      115 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/decorators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/magic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3827 2023-06-15 14:06:18.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/magic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       83 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2023-05-27 13:35:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/cascade_organization_updates.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/fdt_scroll/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-06 13:24:19.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      429 2023-05-27 13:47:18.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/fdt_sqlalchemy/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1677 2023-06-05 13:39:56.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11452 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/group_changes.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4258 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/group_composite.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1824 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/safe_upload.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      183 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/pytest/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-10 17:08:54.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/pytest/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      658 2023-06-10 18:22:32.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2689 2023-04-02 13:28:30.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      163 2023-03-11 04:59:51.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/test_decorators.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      141 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/types/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      164 2023-05-27 13:47:18.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/types/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      594 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3515 2023-06-08 20:11:22.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/cache.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1053 2023-05-27 13:39:17.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/collector.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2023-05-27 13:56:56.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5015 2023-05-27 13:39:41.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/hierarchy.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1832 2023-05-12 09:32:56.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/scheming.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      694 2023-05-27 13:40:39.000000 ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/structures.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7449 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1876 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      965 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-10 18:36:56.000000 ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4681 2023-07-10 18:35:38.000000 ckanext-toolbelt-0.4.5/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.5/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2616 2023-07-10 18:36:56.327803 ckanext-toolbelt-0.4.5/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.5/setup.py
```

### Comparing `ckanext-toolbelt-0.4.4/LICENSE` & `ckanext-toolbelt-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/PKG-INFO` & `ckanext-toolbelt-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.4.4
+Version: 0.4.5
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.4.4/README.md` & `ckanext-toolbelt-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/_shared.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/_shared.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/ckan/db.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/ckan/db.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/ckan/search_index.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/ckan/search_index.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/dev.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_config.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_gh_action.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_gh_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_readme.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_readme.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/cli/make_template.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/cli/make_template.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/magic/__init__.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/cascade_organization_updates.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/group_changes.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/group_changes.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/group_composite.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/group_composite.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/plugins/safe_upload.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/plugins/safe_upload.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/__init__.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/cache.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/collector.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/collector.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/fs.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/hierarchy.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/scheming.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/scheming.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext/toolbelt/utils/structures.py` & `ckanext-toolbelt-0.4.5/ckanext/toolbelt/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/PKG-INFO` & `ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.4.4
+Version: 0.4.5
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/SOURCES.txt` & `ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/ckanext_toolbelt.egg-info/entry_points.txt` & `ckanext-toolbelt-0.4.5/ckanext_toolbelt.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/pyproject.toml` & `ckanext-toolbelt-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.4/setup.cfg` & `ckanext-toolbelt-0.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-toolbelt
-version = 0.4.4
+version = 0.4.5
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-toolbelt
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

