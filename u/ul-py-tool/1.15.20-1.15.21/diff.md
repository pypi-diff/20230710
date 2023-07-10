# Comparing `tmp/ul-py-tool-1.15.20.tar.gz` & `tmp/ul-py-tool-1.15.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-py-tool-1.15.20.tar", last modified: Thu Jun 22 11:49:33 2023, max compression
+gzip compressed data, was "ul-py-tool-1.15.21.tar", last modified: Mon Jul 10 11:36:37 2023, max compression
```

## Comparing `ul-py-tool-1.15.20.tar` & `ul-py-tool-1.15.21.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.337370 ul-py-tool-1.15.20/
--rw-r--r--   0 root         (0) root         (0)     3122 2023-06-22 11:49:33.337370 ul-py-tool-1.15.20/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2468 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 11:49:33.337370 ul-py-tool-1.15.20/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-06-22 11:49:32.000000 ul-py-tool-1.15.20/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.325370 ul-py-tool-1.15.20/ul_py_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.329370 ul-py-tool-1.15.20/ul_py_tool/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-06 11:46:30.000000 ul-py-tool-1.15.20/ul_py_tool/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-06 11:46:30.000000 ul-py-tool-1.15.20/ul_py_tool/__tests__/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.333370 ul-py-tool-1.15.20/ul_py_tool/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2022-11-05 23:11:45.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd.py
--rw-rw-rw-   0 root         (0) root         (0)     5321 2023-06-14 09:15:20.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_build_images.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_fix_own.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2022-10-10 12:04:09.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2022-08-09 14:16:36.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_install.py
--rw-rw-rw-   0 root         (0) root         (0)    33461 2023-06-22 11:36:47.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_lint.py
--rw-rw-rw-   0 root         (0) root         (0)    10007 2023-06-14 09:15:20.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_release.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2022-08-06 11:46:30.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     3597 2022-11-05 23:04:32.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_test_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     6001 2022-11-05 23:04:32.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmd_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2022-10-10 12:04:09.000000 ul-py-tool-1.15.20/ul_py_tool/commands/cmp_outdated.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/commands/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.333370 ul-py-tool-1.15.20/ul_py_tool/conf/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/conf/editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      284 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/conf/git.hook.pre-commit.sh
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/conf/git.hook.pre-push.sh
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/conf/gitattributes
--rw-rw-rw-   0 root         (0) root         (0)     1788 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/conf/gitignore
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-02 21:07:57.000000 ul-py-tool-1.15.20/ul_py_tool/conf/isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1036 2022-08-05 13:02:41.000000 ul-py-tool-1.15.20/ul_py_tool/conf/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-27 08:23:16.000000 ul-py-tool-1.15.20/ul_py_tool/conf/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-08-04 17:28:35.000000 ul-py-tool-1.15.20/ul_py_tool/conf/python-version
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-06 11:46:30.000000 ul-py-tool-1.15.20/ul_py_tool/conf/yamlint.yml
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 18:00:29.000000 ul-py-tool-1.15.20/ul_py_tool/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.337370 ul-py-tool-1.15.20/ul_py_tool/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.337370 ul-py-tool-1.15.20/ul_py_tool/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-05 23:04:32.000000 ul-py-tool-1.15.20/ul_py_tool/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/utils/__tests__/pipfile.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-07-22 16:25:14.000000 ul-py-tool-1.15.20/ul_py_tool/utils/arg_file_exists.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2022-10-10 12:04:09.000000 ul-py-tool-1.15.20/ul_py_tool/utils/arg_files_glob.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-08-02 21:07:57.000000 ul-py-tool-1.15.20/ul_py_tool/utils/arg_str2bool.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2022-10-10 12:04:09.000000 ul-py-tool-1.15.20/ul_py_tool/utils/arg_str2list.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2022-08-02 21:07:57.000000 ul-py-tool-1.15.20/ul_py_tool/utils/arg_str2yaml.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/utils/aseembly.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-08-04 17:28:35.000000 ul-py-tool-1.15.20/ul_py_tool/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2022-10-10 12:04:09.000000 ul-py-tool-1.15.20/ul_py_tool/utils/docker_file.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/utils/fs.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-08-04 11:32:36.000000 ul-py-tool-1.15.20/ul_py_tool/utils/input_lines.py
--rw-rw-rw-   0 root         (0) root         (0)     9717 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/utils/pipfile.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-02 21:07:57.000000 ul-py-tool-1.15.20/ul_py_tool/utils/run_command.py
--rw-rw-rw-   0 root         (0) root         (0)     5622 2022-08-06 11:46:30.000000 ul-py-tool-1.15.20/ul_py_tool/utils/semver.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-04-27 11:37:13.000000 ul-py-tool-1.15.20/ul_py_tool/utils/step.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-01-28 10:47:35.000000 ul-py-tool-1.15.20/ul_py_tool/utils/write_stdout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:49:33.329370 ul-py-tool-1.15.20/ul_py_tool.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3122 2023-06-22 11:49:33.000000 ul-py-tool-1.15.20/ul_py_tool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1720 2023-06-22 11:49:33.000000 ul-py-tool-1.15.20/ul_py_tool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:49:33.000000 ul-py-tool-1.15.20/ul_py_tool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 11:49:33.000000 ul-py-tool-1.15.20/ul_py_tool.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      745 2023-06-22 11:49:33.000000 ul-py-tool-1.15.20/ul_py_tool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 11:49:33.000000 ul-py-tool-1.15.20/ul_py_tool.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.572011 ul-py-tool-1.15.21/
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-07-10 11:36:37.572011 ul-py-tool-1.15.21/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2023-04-19 07:21:53.000000 ul-py-tool-1.15.21/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 11:36:37.572011 ul-py-tool-1.15.21/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-10 11:36:35.000000 ul-py-tool-1.15.21/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.468007 ul-py-tool-1.15.21/ul_py_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.468007 ul-py-tool-1.15.21/ul_py_tool/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-09 09:56:58.000000 ul-py-tool-1.15.21/ul_py_tool/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-09 09:56:58.000000 ul-py-tool-1.15.21/ul_py_tool/__tests__/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.508008 ul-py-tool-1.15.21/ul_py_tool/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd.py
+-rw-rw-rw-   0 root         (0) root         (0)     5321 2023-06-22 11:34:55.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_build_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_fix_own.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2022-08-17 07:19:19.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2022-08-09 14:42:48.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_install.py
+-rw-rw-rw-   0 root         (0) root         (0)    33461 2023-06-22 11:34:55.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)    10047 2023-07-10 11:36:35.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_release.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2022-08-06 11:24:07.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3597 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5475 2023-04-19 07:21:53.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_test_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmd_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2022-08-10 16:14:13.000000 ul-py-tool-1.15.21/ul_py_tool/commands/cmp_outdated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-19 07:21:53.000000 ul-py-tool-1.15.21/ul_py_tool/commands/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.544010 ul-py-tool-1.15.21/ul_py_tool/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/conf/editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      284 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/conf/git.hook.pre-commit.sh
+-rw-rw-rw-   0 root         (0) root         (0)      298 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/conf/git.hook.pre-push.sh
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/conf/gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/conf/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-03 08:46:47.000000 ul-py-tool-1.15.21/ul_py_tool/conf/isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2022-08-05 13:59:39.000000 ul-py-tool-1.15.21/ul_py_tool/conf/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-26 16:37:47.000000 ul-py-tool-1.15.21/ul_py_tool/conf/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-08-05 09:42:35.000000 ul-py-tool-1.15.21/ul_py_tool/conf/python-version
+-rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-05 14:08:36.000000 ul-py-tool-1.15.21/ul_py_tool/conf/yamlint.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-19 07:21:53.000000 ul-py-tool-1.15.21/ul_py_tool/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-26 16:37:47.000000 ul-py-tool-1.15.21/ul_py_tool/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.572011 ul-py-tool-1.15.21/ul_py_tool/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.572011 ul-py-tool-1.15.21/ul_py_tool/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/utils/__tests__/pipfile.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2022-07-26 16:37:47.000000 ul-py-tool-1.15.21/ul_py_tool/utils/arg_file_exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2022-08-17 07:19:19.000000 ul-py-tool-1.15.21/ul_py_tool/utils/arg_files_glob.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2022-08-02 15:17:02.000000 ul-py-tool-1.15.21/ul_py_tool/utils/arg_str2bool.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2022-08-17 07:19:19.000000 ul-py-tool-1.15.21/ul_py_tool/utils/arg_str2list.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2022-08-03 08:46:47.000000 ul-py-tool-1.15.21/ul_py_tool/utils/arg_str2yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-04-19 07:21:53.000000 ul-py-tool-1.15.21/ul_py_tool/utils/aseembly.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-08-05 09:42:35.000000 ul-py-tool-1.15.21/ul_py_tool/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2022-10-10 16:07:49.000000 ul-py-tool-1.15.21/ul_py_tool/utils/docker_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/utils/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2022-08-05 09:42:35.000000 ul-py-tool-1.15.21/ul_py_tool/utils/input_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     9717 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/utils/pipfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-03 08:46:47.000000 ul-py-tool-1.15.21/ul_py_tool/utils/run_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     5622 2022-08-09 09:56:58.000000 ul-py-tool-1.15.21/ul_py_tool/utils/semver.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2022-12-08 08:45:56.000000 ul-py-tool-1.15.21/ul_py_tool/utils/step.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2022-02-08 14:02:26.000000 ul-py-tool-1.15.21/ul_py_tool/utils/write_stdout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 11:36:37.468007 ul-py-tool-1.15.21/ul_py_tool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-07-10 11:36:37.000000 ul-py-tool-1.15.21/ul_py_tool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-07-10 11:36:37.000000 ul-py-tool-1.15.21/ul_py_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 11:36:37.000000 ul-py-tool-1.15.21/ul_py_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-10 11:36:37.000000 ul-py-tool-1.15.21/ul_py_tool.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-10 11:36:37.000000 ul-py-tool-1.15.21/ul_py_tool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 11:36:37.000000 ul-py-tool-1.15.21/ul_py_tool.egg-info/top_level.txt
```

### Comparing `ul-py-tool-1.15.20/PKG-INFO` & `ul-py-tool-1.15.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-py-tool
-Version: 1.15.20
+Version: 1.15.21
 Summary: Python ul py tool
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-py-tool-1.15.20/README.md` & `ul-py-tool-1.15.21/README.md`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/setup.py` & `ul-py-tool-1.15.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-py-tool',
-    version='1.15.20',
+    version='1.15.21',
     description='Python ul py tool',
     author='Unic-lab',
     author_email='',
     url='https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git',
     packages=find_packages(include=['ul_py_tool*']),
     platforms='any',
     package_data={
```

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_build_images.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_build_images.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_cleanup.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_fmt.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_fmt.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_install.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_install.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_lint.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_lint.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_release.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 enc_key = os.environ[self.assembly_target.encryption_key_name]
                 deploy_result = run_command(
                     [
                         f'git add . '
                         f'&& export RELEASE_TAG={component_config.tag} '
                         f'&& export WERF_SECRET_KEY={enc_key} '
                         f'&& export WERF_ENV={self.assembly_target.environment} '
-                        f'&& werf converge --config=werf-release.yaml --kube-config {kubeconfig_file_path} --namespace={release_name} --values=values.yaml  --values=charts.yaml --secret-values=secret-values.yaml --auto-rollback=true --loose-giterminism=True --dev=True'  # noqa
+                        f'&& werf converge --config=werf-release.yaml --kube-config {kubeconfig_file_path} --namespace={release_name} --values=values.yaml  --values=charts.yaml --set=component_version={component.tag} --secret-values=secret-values.yaml --auto-rollback=true --loose-giterminism=True --dev=True'  # noqa
                     ],
                     cwd=component_directory,
                     ignore_errors=True,
                 )
                 if deploy_result.code != 0:
                     for release, version in releases.items():
                         # rollback all successful releases
```

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_stats.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_test.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_test.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_test_secrets.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_test_secrets.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmd_version.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmd_version.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/cmp_outdated.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/cmp_outdated.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/commands/conf.py` & `ul-py-tool-1.15.21/ul_py_tool/commands/conf.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/conf/gitignore` & `ul-py-tool-1.15.21/ul_py_tool/conf/gitignore`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/conf/mypy.ini` & `ul-py-tool-1.15.21/ul_py_tool/conf/mypy.ini`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/conf/yamlint.yml` & `ul-py-tool-1.15.21/ul_py_tool/conf/yamlint.yml`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/main.py` & `ul-py-tool-1.15.21/ul_py_tool/main.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/__tests__/pipfile.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/__tests__/pipfile.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/arg_files_glob.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/arg_files_glob.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/arg_str2list.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/arg_str2list.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/arg_str2yaml.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/arg_str2yaml.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/docker_file.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/docker_file.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/pipfile.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/pipfile.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/run_command.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/run_command.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/semver.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/semver.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool/utils/step.py` & `ul-py-tool-1.15.21/ul_py_tool/utils/step.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool.egg-info/PKG-INFO` & `ul-py-tool-1.15.21/ul_py_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-py-tool
-Version: 1.15.20
+Version: 1.15.21
 Summary: Python ul py tool
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-py-tool-1.15.20/ul_py_tool.egg-info/SOURCES.txt` & `ul-py-tool-1.15.21/ul_py_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.20/ul_py_tool.egg-info/requires.txt` & `ul-py-tool-1.15.21/ul_py_tool.egg-info/requires.txt`

 * *Files identical despite different names*

