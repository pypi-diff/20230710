# Comparing `tmp/ckanext-toolbelt-0.4.2.tar.gz` & `tmp/ckanext-toolbelt-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-toolbelt-0.4.2.tar", last modified: Thu Jun 15 14:08:48 2023, max compression
+gzip compressed data, was "ckanext-toolbelt-0.4.3.tar", last modified: Mon Jul 10 17:32:12 2023, max compression
```

## Comparing `ckanext-toolbelt-0.4.2.tar` & `ckanext-toolbelt-0.4.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      223 2023-06-10 18:22:10.000000 ckanext-toolbelt-0.4.2/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7449 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6769 2023-06-05 13:45:47.000000 ckanext-toolbelt-0.4.2/README.md
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4633 2023-06-15 14:08:31.000000 ckanext-toolbelt-0.4.2/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2599 2023-06-15 14:08:48.891449 ckanext-toolbelt-0.4.2/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/setup.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      190 2023-06-15 13:56:03.000000 ckanext-toolbelt-0.4.2/src/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      224 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1472 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/_shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/ckan/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/ckan/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1285 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/ckan/db.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1378 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/ckan/search_index.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1397 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/dev.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      368 2023-04-03 09:57:56.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2108 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1371 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_gh_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1824 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_readme.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2346 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_template.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      652 2023-04-01 15:00:10.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      463 2023-04-02 12:00:10.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/action_release-please.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1968 2023-04-01 12:17:07.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/action_test.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      859 2023-04-07 20:52:14.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/config_gulp-sass.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      727 2023-05-30 13:02:03.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       72 2023-05-07 13:09:03.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/config_pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-04-02 12:33:30.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_black.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      207 2023-04-03 08:52:49.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_commitizen.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2023-04-03 15:36:15.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_isort.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2325 2023-04-11 15:57:47.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_pyright.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-04-02 12:33:54.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_pytest.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1360 2023-04-15 11:39:33.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_ruff.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      115 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/decorators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/magic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3827 2023-06-15 14:06:18.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/magic/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       83 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2023-05-27 13:35:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/cascade_organization_updates.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_scroll/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-06 13:24:19.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      429 2023-05-27 13:47:18.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_scroll/templates/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      150 2023-03-06 13:25:14.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1677 2023-06-05 13:39:56.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11452 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/group_changes.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4258 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/group_composite.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1824 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/safe_upload.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.861450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.861450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/group/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3034 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      562 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.871450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1046 2023-04-21 15:01:05.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1112 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1231 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      103 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      234 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      183 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/pytest/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-10 17:08:54.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/pytest/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      658 2023-06-10 18:22:32.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2689 2023-04-02 13:28:30.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      163 2023-03-11 04:59:51.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/test_decorators.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      141 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/test_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1216 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/test_cache.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      755 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/test_collector.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2856 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/test_hierarchy.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/types/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      164 2023-05-27 13:47:18.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/types/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      594 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3515 2023-06-08 20:11:22.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/cache.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1053 2023-05-27 13:39:17.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/collector.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2023-05-27 13:56:56.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5015 2023-05-27 13:39:41.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/hierarchy.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1832 2023-05-12 09:32:56.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/scheming.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      694 2023-05-27 13:40:39.000000 ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/structures.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-15 14:08:48.881450 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7449 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3560 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      965 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-15 14:08:48.000000 ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/top_level.txt
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      223 2023-06-10 18:22:10.000000 ckanext-toolbelt-0.4.3/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7449 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6769 2023-06-05 13:45:47.000000 ckanext-toolbelt-0.4.3/README.md
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4697 2023-07-05 16:15:57.000000 ckanext-toolbelt-0.4.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2599 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      190 2023-06-15 13:56:03.000000 ckanext-toolbelt-0.4.3/src/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      224 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1472 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/_shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/ckan/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/ckan/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1285 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/ckan/db.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1378 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/ckan/search_index.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1397 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/dev.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      368 2023-04-03 09:57:56.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2108 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1371 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_gh_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1824 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_readme.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2346 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_template.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      652 2023-04-01 15:00:10.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      463 2023-04-02 12:00:10.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/action_release-please.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1968 2023-04-01 12:17:07.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/action_test.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      859 2023-04-07 20:52:14.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/config_gulp-sass.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      727 2023-05-30 13:02:03.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/config_pre-commit.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       72 2023-05-07 13:09:03.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/config_pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-04-02 12:33:30.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_black.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      207 2023-04-03 08:52:49.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_commitizen.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2023-04-03 15:36:15.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_isort.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2325 2023-04-11 15:57:47.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_pyright.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2023-04-02 12:33:54.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_pytest.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1424 2023-07-05 16:16:22.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_ruff.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      115 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/decorators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/magic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3827 2023-06-15 14:06:18.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/magic/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       83 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2023-05-27 13:35:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/cascade_organization_updates.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_scroll/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-03-06 13:24:19.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_scroll/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      429 2023-05-27 13:47:18.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_scroll/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_scroll/templates/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      150 2023-03-06 13:25:14.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_scroll/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1677 2023-06-05 13:39:56.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11452 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/group_changes.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4258 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/group_composite.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1824 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/safe_upload.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.726610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.726610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/group/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3034 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      562 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.726610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1046 2023-04-21 15:01:05.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1112 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1231 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      103 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/no_change.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      234 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/title.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.736611 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      183 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/pytest/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-10 17:08:54.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/pytest/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      658 2023-06-10 18:22:32.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2689 2023-04-02 13:28:30.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      163 2023-03-11 04:59:51.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/test_decorators.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      141 2023-03-11 04:59:56.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1216 2022-08-04 10:07:37.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/test_cache.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      755 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/test_collector.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2856 2023-05-07 13:31:23.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/test_hierarchy.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/types/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      164 2023-05-27 13:47:18.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/types/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      594 2023-05-07 13:14:42.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3515 2023-06-08 20:11:22.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/cache.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1053 2023-05-27 13:39:17.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/collector.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2023-05-27 13:56:56.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5015 2023-05-27 13:39:41.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/hierarchy.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1832 2023-05-12 09:32:56.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/scheming.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      694 2023-05-27 13:40:39.000000 ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/structures.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-10 17:32:12.746610 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7449 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3560 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      965 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       75 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-10 17:32:12.000000 ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/top_level.txt
```

### Comparing `ckanext-toolbelt-0.4.2/LICENSE` & `ckanext-toolbelt-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/PKG-INFO` & `ckanext-toolbelt-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.4.2
+Version: 0.4.3
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.4.2/README.md` & `ckanext-toolbelt-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/pyproject.toml` & `ckanext-toolbelt-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,17 @@
        "T20",  # print statements
        "TID",  # tidier imports
        "TCH",
        "TRY",  # better exceptions
        "UP",  # upgrade syntax for newer versions of the language
 ]
 ignore = [
-       # "PT004", # fixture does not return anything, add leading underscore: violated by clean_db
-       # "PLC1901", # simplify comparison to empty string: violated by SQLAlchemy filters
+       "E712", # comparison to bool: violated by SQLAlchemy filters
+       "PT004", # fixture does not return anything, add leading underscore: violated by clean_db
+       "PLC1901", # simplify comparison to empty string: violated by SQLAlchemy filters
 ]
 
 [tool.ruff.per-file-ignores]
 "src/ckanext/toolbelt/tests*" = [
                          "S",  # security testing
                          "PLR2004", # magic value used in comparison
                          "PT004",
```

### Comparing `ckanext-toolbelt-0.4.2/setup.cfg` & `ckanext-toolbelt-0.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-toolbelt
-version = 0.4.2
+version = 0.4.3
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-toolbelt
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/_shared.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/_shared.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/ckan/db.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/ckan/db.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/ckan/search_index.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/ckan/search_index.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/dev.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/dev.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_config.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_gh_action.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_gh_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_readme.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_readme.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/make_template.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/make_template.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/action_pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/action_test.yaml` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/action_test.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/config_gulp-sass.js` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/config_gulp-sass.js`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/config_pre-commit.yaml` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/config_pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_pyright.toml` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_pyright.toml`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/cli/templates/template_ruff.toml` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/cli/templates/template_ruff.toml`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,17 @@
        # "T10",  # debugging statements
        # "T20",  # print statements
        # "TID",  # tidier imports
        # "TRY",  # better exceptions
        # "UP",  # upgrade syntax for newer versions of the language
 ]
 ignore = [
-       # "PT004", # fixture does not return anything, add leading underscore: violated by clean_db
-       # "PLC1901", # simplify comparison to empty string: violated by SQLAlchemy filters
+       "E712", # comparison to bool: violated by SQLAlchemy filters
+       "PT004", # fixture does not return anything, add leading underscore: violated by clean_db
+       "PLC1901", # simplify comparison to empty string: violated by SQLAlchemy filters
 ]
 
 [tool.ruff.per-file-ignores]
 "ckanext/$PLUGIN/tests*" = [
                          "S",  # security testing
                          "PLR2004" # magic value used in comparison
 ]
```

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/magic/__init__.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/cascade_organization_updates.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/fdt_sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/group_changes.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/group_changes.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/group_composite.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/group_composite.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/safe_upload.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/safe_upload.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/group/changes.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/group/snippets/item_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/activities/changed_group.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/description.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/plugins/templates/group_changes/snippets/group_changes/image_url.html`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/pytest/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/plugins/test_cascade_organization_updates.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/test_cache.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/test_collector.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/test_collector.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/tests/utils/test_hierarchy.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/tests/utils/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/__init__.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/cache.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/collector.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/collector.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/fs.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/hierarchy.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/scheming.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/scheming.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext/toolbelt/utils/structures.py` & `ckanext-toolbelt-0.4.3/src/ckanext/toolbelt/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/PKG-INFO` & `ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-toolbelt
-Version: 0.4.2
+Version: 0.4.3
 Home-page: https://github.com/DataShades/ckanext-toolbelt
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/SOURCES.txt` & `ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-toolbelt-0.4.2/src/ckanext_toolbelt.egg-info/entry_points.txt` & `ckanext-toolbelt-0.4.3/src/ckanext_toolbelt.egg-info/entry_points.txt`

 * *Files identical despite different names*

