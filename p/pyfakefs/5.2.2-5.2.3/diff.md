# Comparing `tmp/pyfakefs-5.2.2.tar.gz` & `tmp/pyfakefs-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfakefs-5.2.2.tar", last modified: Thu Apr 13 17:55:43 2023, max compression
+gzip compressed data, was "pyfakefs-5.2.3.tar", last modified: Mon Jul 10 17:28:27 2023, max compression
```

## Comparing `pyfakefs-5.2.2.tar` & `pyfakefs-5.2.3.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    43745 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/COPYING
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.844593 pyfakefs-5.2.2/pyfakefs/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    45851 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_file.py
--rw-r--r--   0 runner    (1001) docker     (123)   115325 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2180 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_filesystem_shutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    42878 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_filesystem_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_open.py
--rw-r--r--   0 runner    (1001) docker     (123)    50722 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_os.py
--rw-r--r--   0 runner    (1001) docker     (123)    17959 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    34457 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_scandir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/mox3_stubout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/patched_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.852594 pyfakefs-5.2.2/pyfakefs/pytest_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_doctest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_param_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_module_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_plugin_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/pyfakefs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/all_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/all_tests_without_extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/dynamic_patch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/example_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_glob_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22148 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_shutil_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   105643 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_unittest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_vs_real_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    83871 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_open_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   230962 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_os_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_pathlib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_stat_time_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_tempfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/pyfakefs/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/config_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/deprecated_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/module_with_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/import_as_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/logsio.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/patched_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.848593 pyfakefs-5.2.2/pyfakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:27.839208 pyfakefs-5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    44696 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/COPYING
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-10 17:28:27.839208 pyfakefs-5.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:27.835208 pyfakefs-5.2.3/pyfakefs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45924 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116686 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3755 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_filesystem_shutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_filesystem_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50798 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/fake_scandir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/mox3_stubout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/patched_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:27.835208 pyfakefs-5.2.3/pyfakefs/pytest_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_doctest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_fixture_param_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_module_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_plugin_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:27.839208 pyfakefs-5.2.3/pyfakefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/all_tests_without_extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/dynamic_patch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_glob_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_shutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105643 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34071 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_unittest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_vs_real_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84325 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_open_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   230962 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_os_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_pathlib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_stat_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fake_tempfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:27.839208 pyfakefs-5.2.3/pyfakefs/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fixtures/config_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fixtures/deprecated_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/fixtures/module_with_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/import_as_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/logsio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/mox3_stubout_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/mox3_stubout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/patched_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyfakefs/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:28:27.835208 pyfakefs-5.2.3/pyfakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-10 17:28:27.000000 pyfakefs-5.2.3/pyfakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-10 17:28:27.000000 pyfakefs-5.2.3/pyfakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:28:27.000000 pyfakefs-5.2.3/pyfakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 17:28:27.000000 pyfakefs-5.2.3/pyfakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 17:28:27.000000 pyfakefs-5.2.3/pyfakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-10 17:28:27.839208 pyfakefs-5.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 17:28:16.000000 pyfakefs-5.2.3/setup.py
```

### Comparing `pyfakefs-5.2.2/CHANGES.md` & `pyfakefs-5.2.3/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 # pyfakefs Release Notes
 The released versions correspond to PyPI releases.
 
+## [Version 5.2.3](https://pypi.python.org/pypi/pyfakefs/5.2.3) (2023-07-10)
+Adds compatibility with PyPy 3.10 and Python 3.12.
+
+### Fixes
+* Re-create temp directory if it had been created before on resetting file system
+  (see [#814](../../issues/814)).
+* Exclude pytest `pathlib` modules from patching to avoid mixup of patched/unpatched
+  code (see [#814](../../issues/814)).
+* Adapt to changes in Python 3.12 beta1 (only working partially,
+  see [#830](../../issues/830) and [#831](../../issues/831)).
+* Adapt to changes in `shutil` in Python 3.12 beta2 (see [#814](../../issues/814)).
+* Fix support for newer PyPi versions (see [#859](../../issues/859)).
+
+### Documentation
+* Added a note regarding the incompatibility of the built-in `sqlite3` module with
+  `pyfakefs` (see [#850](../../issues/850))
+
+### Infrastructure
+* Added pytype check for non-test modules in CI (see [#599](../../issues/599)).
+* Added tests for different pypy3 versions.
+
 ## [Version 5.2.2](https://pypi.python.org/pypi/pyfakefs/5.2.2) (2023-04-13)
 Fixes a regression in 5.2.0
 
 ### Changes
 * Made the user and group IDs accessible via dedicated ``get_uid`` and ``get_gid``
   functions (for symmetry to ``set_uid`` / ``set_gid``)
```

### Comparing `pyfakefs-5.2.2/COPYING` & `pyfakefs-5.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/PKG-INFO` & `pyfakefs-5.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.2.2
+Version: 5.2.3
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
@@ -37,18 +37,24 @@
 
 
 pyfakefs implements a fake file system that mocks the Python file system modules.
 Using pyfakefs, your tests operate on a fake file system in memory without
 touching the real disk. The software under test requires no modification to
 work with pyfakefs.
 
-pyfakefs acts as a `pytest` plugin by providing the `fs` fixture, which will
-automatically invoke the fake filesystem. It also provides
-the `fake_filesystem_unittest.TestCase` class for use with `unittest` and
-the means to use the fake filesystem with other test frameworks.
+Pyfakefs creates a new empty in-memory file system at each test start, which replaces
+the real filesystem during the test. Think of pyfakefs as making a per-test temporary
+directory, except for an entire file system.
+
+There are several means to achieve this: by using
+the `fs` fixture if running pytest, by using `fake_filesystem_unittest.TestCase` as a
+base class if using unittest, by using a `fake_filesystem_unittest.Patcher` instance
+as a context manager, or by using the `patchfs` decorator.
+
+
 
 pyfakefs works with current versions of Linux, Windows and macOS.
 
 ## Documentation
 
 This document provides a general overview for pyfakefs.  There is more:
```

### Comparing `pyfakefs-5.2.2/README.md` & `pyfakefs-5.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 
 
 pyfakefs implements a fake file system that mocks the Python file system modules.
 Using pyfakefs, your tests operate on a fake file system in memory without
 touching the real disk. The software under test requires no modification to
 work with pyfakefs.
 
-pyfakefs acts as a `pytest` plugin by providing the `fs` fixture, which will
-automatically invoke the fake filesystem. It also provides
-the `fake_filesystem_unittest.TestCase` class for use with `unittest` and
-the means to use the fake filesystem with other test frameworks.
+Pyfakefs creates a new empty in-memory file system at each test start, which replaces
+the real filesystem during the test. Think of pyfakefs as making a per-test temporary
+directory, except for an entire file system.
+
+There are several means to achieve this: by using
+the `fs` fixture if running pytest, by using `fake_filesystem_unittest.TestCase` as a
+base class if using unittest, by using a `fake_filesystem_unittest.Patcher` instance
+as a context manager, or by using the `patchfs` decorator.
+
+
 
 pyfakefs works with current versions of Linux, Windows and macOS.
 
 ## Documentation
 
 This document provides a general overview for pyfakefs.  There is more:
```

### Comparing `pyfakefs-5.2.2/pyfakefs/extra_packages.py` & `pyfakefs-5.2.3/pyfakefs/extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_file.py` & `pyfakefs-5.2.3/pyfakefs/fake_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
                 self._byte_contents += b"\0" * (st_size - current_size)
         self.st_size = st_size
         self.epoch += 1
 
     @property
     def path(self) -> AnyStr:
         """Return the full path of the current object."""
-        names: List[AnyStr] = []
+        names: List[AnyStr] = []  # pytype: disable=invalid-annotation
         obj: Optional[FakeFile] = self
         while obj:
             names.insert(0, matching_string(self.name, obj.name))  # type: ignore
             obj = obj.parent_dir
         sep = self.filesystem.get_path_separator(names[0])
         if names[0] == sep:
             names.pop(0)
@@ -1276,15 +1276,15 @@
         if self.filedes is not None:
             return self.filedes
         raise OSError(errno.EBADF, "Invalid file descriptor")
 
     def read(self, numBytes: int = -1) -> bytes:
         """Read from the real pipe."""
         if self.real_file:
-            return self.real_file.read(numBytes)
+            return self.real_file.read(numBytes)  # pytype: disable=bad-return-type
         return os.read(self.fd, numBytes)
 
     def flush(self) -> None:
         """Flush the real pipe?"""
 
     def write(self, contents: bytes) -> int:
         """Write to the real pipe."""
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_filesystem.py` & `pyfakefs-5.2.3/pyfakefs/fake_filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 True
 """
 import errno
 import heapq
 import os
 import random
 import sys
+import tempfile
 from collections import namedtuple, OrderedDict
 from doctest import TestResults
 from enum import Enum
 from stat import (
     S_IFREG,
     S_IFDIR,
     S_ISLNK,
@@ -193,29 +194,35 @@
     """
 
     def __init__(
         self,
         path_separator: str = os.path.sep,
         total_size: Optional[int] = None,
         patcher: Any = None,
+        create_temp_dir: bool = False,
     ) -> None:
         """
         Args:
             path_separator:  optional substitute for os.path.sep
             total_size: if not None, the total size in bytes of the
                 root filesystem.
+            patcher: the Patcher instance if created from the Patcher
+            create_temp_dir: If True, a temp directory is created on initialization.
+                Under Posix, if the temp directory is not `/tmp`, a link to the temp
+                path is additionally created at `/tmp`.
 
         Example usage to use the same path separator under all systems:
 
         >>> filesystem = FakeFilesystem(path_separator='/')
 
         """
         self.path_separator: str = path_separator
         self.alternative_path_separator: Optional[str] = os.path.altsep
         self.patcher = patcher
+        self.create_temp_dir = create_temp_dir
         if path_separator != os.sep:
             self.alternative_path_separator = None
 
         # is_windows_fs can be used to test the behavior of pyfakefs under
         # Windows fs on non-Windows systems and vice verse;
         # is it used to support drive letters, UNC paths and some other
         # Windows-specific features
@@ -224,15 +231,15 @@
         # can be used to test some MacOS-specific behavior under other systems
         self._is_macos = sys.platform == "darwin"
 
         # is_case_sensitive can be used to test pyfakefs for case-sensitive
         # file systems on non-case-sensitive systems and vice verse
         self.is_case_sensitive: bool = not (self.is_windows_fs or self._is_macos)
 
-        self.root = FakeDirectory(self.path_separator, filesystem=self)
+        self.root: FakeDirectory
         self._cwd = ""
 
         # We can't query the current value without changing it:
         self.umask: int = os.umask(0o22)
         os.umask(self.umask)
 
         # A list of open file objects. Their position in the list is their
@@ -240,17 +247,17 @@
         self.open_files: List[Optional[List[AnyFileWrapper]]] = []
         # A heap containing all free positions in self.open_files list
         self._free_fd_heap: List[int] = []
         # last used numbers for inodes (st_ino) and devices (st_dev)
         self.last_ino: int = 0
         self.last_dev: int = 0
         self.mount_points: Dict[AnyString, Dict] = OrderedDict()
-        self._add_root_mount_point(total_size)
-        self._add_standard_streams()
-        self.dev_null: Any = FakeNullFile(self)
+        self.dev_null: Any = None
+        self.reset(total_size=total_size, init_pathlib=False)
+
         # set from outside if needed
         self.patch_open_code = PatchMode.OFF
         self.shuffle_listdir_results = False
 
     @property
     def is_linux(self) -> bool:
         return not self.is_windows_fs and not self.is_macos
@@ -326,29 +333,32 @@
         self._is_macos = value == OSType.MACOS
         self.is_case_sensitive = value == OSType.LINUX
         self.path_separator = "\\" if value == OSType.WINDOWS else "/"
         self.alternative_path_separator = "/" if value == OSType.WINDOWS else None
         self.reset()
         FakePathModule.reset(self)
 
-    def reset(self, total_size: Optional[int] = None):
+    def reset(self, total_size: Optional[int] = None, init_pathlib: bool = True):
         """Remove all file system contents and reset the root."""
         self.root = FakeDirectory(self.path_separator, filesystem=self)
 
         self.dev_null = FakeNullFile(self)
-        self.open_files = []
-        self._free_fd_heap = []
+        self.open_files.clear()
+        self._free_fd_heap.clear()
         self.last_ino = 0
         self.last_dev = 0
-        self.mount_points = OrderedDict()
+        self.mount_points.clear()
         self._add_root_mount_point(total_size)
         self._add_standard_streams()
-        from pyfakefs import fake_pathlib
+        if self.create_temp_dir:
+            self._create_temp_dir()
+        if init_pathlib:
+            from pyfakefs import fake_pathlib
 
-        fake_pathlib.init_module(self)
+            fake_pathlib.init_module(self)
 
     def _add_root_mount_point(self, total_size):
         mount_point = "C:" if self.is_windows_fs else self.path_separator
         self._cwd = mount_point
         if not self.cwd.endswith(self.path_separator):
             self._cwd += self.path_separator
         self.add_mount_point(mount_point, total_size)
@@ -536,19 +546,19 @@
         assert mount_point
         return mount_point
 
     def _mount_point_dir_for_cwd(self) -> FakeDirectory:
         """Return the fake directory object of the mount point where the
         current working directory points to."""
 
-        def object_from_path(file_path):
+        def object_from_path(file_path) -> FakeDirectory:
             path_components = self._path_components(file_path)
             target = self.root
             for component in path_components:
-                target = target.get_entry(component)
+                target = cast(FakeDirectory, target.get_entry(component))
             return target
 
         path = to_string(self.cwd)
         for mount_path in self.mount_points:
             if path == to_string(mount_path):
                 return object_from_path(mount_path)
         mount_path = ""
@@ -912,16 +922,20 @@
             (str) A copy of path with empty components and dot components
             removed.
         """
         path_str = self.normcase(path)
         drive, path_str = self.splitdrive(path_str)
         sep = self.get_path_separator(path_str)
         is_absolute_path = path_str.startswith(sep)
-        path_components: List[AnyStr] = path_str.split(sep)
-        collapsed_path_components: List[AnyStr] = []
+        path_components: List[AnyStr] = path_str.split(
+            sep
+        )  # pytype: disable=invalid-annotation
+        collapsed_path_components: List[
+            AnyStr
+        ] = []  # pytype: disable=invalid-annotation
         dot = matching_string(path_str, ".")
         dotdot = matching_string(path_str, "..")
         for component in path_components:
             if (not component) or (component == dot):
                 continue
             if component == dotdot:
                 if collapsed_path_components and (
@@ -1376,15 +1390,15 @@
             (bool) True if the corresponding object exists.
 
         Raises:
             TypeError: if file_path is None.
         """
         if check_link and self.islink(file_path):
             return True
-        path = to_string(make_string_path(file_path))
+        path = to_string(self.make_string_path(file_path))
         if path is None:
             raise TypeError
         if not path:
             return False
         if path == self.dev_null.name:
             return not self.is_windows_fs or sys.version_info >= (3, 8)
         try:
@@ -1459,15 +1473,15 @@
             return path
         if path == matching_string(path, self.dev_null.name):
             return path
         path_components = self._path_components(path)
         resolved_components = self._resolve_components(path_components)
         path = self._components_to_path(resolved_components)
         # after resolving links, we have to check again for Windows root
-        return self.replace_windows_root(path)
+        return self.replace_windows_root(path)  # pytype: disable=bad-return-type
 
     def _components_to_path(self, component_folders):
         sep = (
             self.get_path_separator(component_folders[0])
             if component_folders
             else self.path_separator
         )
@@ -1566,15 +1580,15 @@
                 # (which will normalize to /c)
                 # /a/b => d should yield a/d
                 components = link_path_components[:-1]
                 components.append(link_path)
                 link_path = sep.join(components)
             # Don't call self.NormalizePath(), as we don't want to prepend
             # self.cwd.
-            return self.normpath(link_path)
+            return self.normpath(link_path)  # pytype: disable=bad-return-type
         raise ValueError("Invalid link")
 
     def get_object_from_normpath(
         self,
         file_path: AnyPath,
         check_read_perm: bool = True,
         check_owner: bool = False,
@@ -2911,14 +2925,27 @@
         return str(self.root_dir)
 
     def _add_standard_streams(self) -> None:
         self._add_open_file(StandardStreamWrapper(sys.stdin))
         self._add_open_file(StandardStreamWrapper(sys.stdout))
         self._add_open_file(StandardStreamWrapper(sys.stderr))
 
+    def _create_temp_dir(self):
+        # the temp directory is assumed to exist at least in `tempfile`,
+        # so we create it here for convenience
+        temp_dir = tempfile.gettempdir()
+        if not self.exists(temp_dir):
+            self.create_dir(temp_dir)
+        if sys.platform != "win32" and not self.exists("/tmp"):
+            # under Posix, we also create a link in /tmp if the path does not exist
+            self.create_symlink("/tmp", temp_dir)
+            # reset the used size to 0 to avoid having the link size counted
+            # which would make disk size tests more complicated
+            next(iter(self.mount_points.values()))["used_size"] = 0
+
 
 def _run_doctest() -> TestResults:
     import doctest
     import pyfakefs
 
     return doctest.testmod(pyfakefs.fake_filesystem)
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_filesystem_unittest.py` & `pyfakefs-5.2.3/pyfakefs/fake_filesystem_unittest.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 that even in your test fixture, familiar functions like `open()` and
 `os.makedirs()` manipulate the fake file system.
 
 Existing unit tests that use the real file system can be retrofitted to use
 pyfakefs by simply changing their base class from `:py:class`unittest.TestCase`
 to `:py:class`pyfakefs.fake_filesystem_unittest.TestCase`.
 """
-import _io  # type:ignore [import]
+import _io  # type:ignore[import]
+import builtins
 import doctest
 import functools
 import genericpath
 import inspect
 import io
 import linecache
 import os
@@ -74,19 +75,15 @@
     reset_ids,
     PatchMode,
     FakeFilesystem,
 )
 from pyfakefs.helpers import IS_PYPY
 from pyfakefs.mox3_stubout import StubOutForTesting
 
-try:
-    from importlib.machinery import ModuleSpec
-except ImportError:
-    ModuleSpec = object  # type: ignore[assignment, misc]
-
+from importlib.machinery import ModuleSpec
 from importlib import reload
 
 from pyfakefs import fake_filesystem, fake_io, fake_os, fake_open, fake_path, fake_file
 from pyfakefs import fake_filesystem_shutil
 from pyfakefs import fake_pathlib
 from pyfakefs import mox3_stubout
 from pyfakefs.extra_packages import pathlib2, use_scandir
@@ -455,15 +452,15 @@
         os,
         io,
         _io,
         genericpath,
         os.path,
     }
     if sys.platform == "win32":
-        import nt  # type:ignore [import]
+        import nt  # type:ignore[import]
         import ntpath
 
         SKIPMODULES.add(nt)
         SKIPMODULES.add(ntpath)
     else:
         import posix
         import posixpath
@@ -559,14 +556,15 @@
             set_uid(1)
             set_gid(1)
 
         self._skip_names = self.SKIPNAMES.copy()
         # save the original open function for use in pytest plugin
         self.original_open = open
         self.patch_open_code = patch_open_code
+        self.fake_open: fake_open.FakeFileOpen
 
         if additional_skip_names is not None:
             skip_names = [
                 cast(ModuleType, m).__name__ if inspect.ismodule(m) else cast(str, m)
                 for m in additional_skip_names
             ]
             self._skip_names.update(skip_names)
@@ -673,24 +671,26 @@
             self._fake_module_classes["scandir"] = fake_scandir.FakeScanDirModule
 
     def _init_fake_module_functions(self) -> None:
         # handle patching function imported separately like
         # `from os import stat`
         # each patched function name has to be looked up separately
         for mod_name, fake_module in self._fake_module_classes.items():
-            if hasattr(fake_module, "dir") and inspect.isfunction(fake_module.dir):
-                for fct_name in fake_module.dir():
-                    module_attr = (getattr(fake_module, fct_name), mod_name)
-                    self._fake_module_functions.setdefault(fct_name, {})[
-                        mod_name
-                    ] = module_attr
-                    if mod_name == "os":
+            if hasattr(fake_module, "dir"):
+                module_dir = fake_module.dir
+                if inspect.isfunction(module_dir):
+                    for fct_name in fake_module.dir():
+                        module_attr = (getattr(fake_module, fct_name), mod_name)
                         self._fake_module_functions.setdefault(fct_name, {})[
-                            OS_MODULE
+                            mod_name
                         ] = module_attr
+                        if mod_name == "os":
+                            self._fake_module_functions.setdefault(fct_name, {})[
+                                OS_MODULE
+                            ] = module_attr
 
         # special handling for functions in os.path
         fake_module = fake_filesystem.FakePathModule
         for fct_name in fake_module.dir():
             module_attr = (getattr(fake_module, fct_name), PATH_MODULE)
             self._fake_module_functions.setdefault(fct_name, {})[
                 "genericpath"
@@ -840,16 +840,17 @@
 
     def _refresh(self) -> None:
         """Renew the fake file system and set the _isStale flag to `False`."""
         if self._stubs is not None:
             self._stubs.smart_unset_all()
         self._stubs = mox3_stubout.StubOutForTesting()
 
-        self.fs = fake_filesystem.FakeFilesystem(patcher=self)
+        self.fs = fake_filesystem.FakeFilesystem(patcher=self, create_temp_dir=True)
         self.fs.patch_open_code = self.patch_open_code
+        self.fake_open = fake_open.FakeFileOpen(self.fs)
         for name in self._fake_module_classes:
             self.fake_modules[name] = self._fake_module_classes[name](self.fs)
             if hasattr(self.fake_modules[name], "skip_names"):
                 self.fake_modules[name].skip_names = self._skip_names
         self.fake_modules[PATH_MODULE] = self.fake_modules["os"].path
         for name in self._unfaked_module_classes:
             self.unfaked_modules[name] = self._unfaked_module_classes[name]()
@@ -872,40 +873,28 @@
             sys.platform == "darwin"
             and hasattr(shutil, "_HAS_FCOPYFILE")
             and shutil._HAS_FCOPYFILE
         )
         if self.has_fcopy_file:
             shutil._HAS_FCOPYFILE = False  # type: ignore[attr-defined]
 
-        temp_dir = tempfile.gettempdir()
         with warnings.catch_warnings():
             # ignore warnings, see #542 and #614
             warnings.filterwarnings("ignore")
             self._find_modules()
 
         self._refresh()
 
         if doctester is not None:
             doctester.globs = self.replace_globs(doctester.globs)
 
         self.start_patching()
         linecache.open = self.original_open  # type: ignore[attr-defined]
         tokenize._builtin_open = self.original_open  # type: ignore
 
-        # the temp directory is assumed to exist at least in `tempfile`,
-        # so we create it here for convenience
-        assert self.fs is not None
-        self.fs.create_dir(temp_dir)
-        if sys.platform != "win32" and not self.fs.exists("/tmp"):
-            # under Posix, we also create a link in /tmp if the path does not exist
-            self.fs.create_symlink("/tmp", temp_dir)
-            # reset the used size to 0 to avoid having the link size counted
-            # which would make disk size tests more complicated
-            next(iter(self.fs.mount_points.values()))["used_size"] = 0
-
     def start_patching(self) -> None:
         if not self._patching:
             self._patching = True
 
             self.patch_modules()
             self.patch_functions()
             self.patch_defaults()
@@ -917,33 +906,40 @@
                     reload(module)
 
     def patch_functions(self) -> None:
         assert self._stubs is not None
         for (name, ft_name, ft_mod), modules in self.FS_FUNCTIONS.items():
             method, mod_name = self._fake_module_functions[ft_name][ft_mod]
             fake_module = self.fake_modules[mod_name]
-            attr = method.__get__(fake_module, fake_module.__class__)
+            attr = method.__get__(
+                fake_module, fake_module.__class__
+            )  # pytype: disable=attribute-error
             for module in modules:
                 self._stubs.smart_set(module, name, attr)
 
     def patch_modules(self) -> None:
         assert self._stubs is not None
         for name, modules in self.FS_MODULES.items():
             for module, attr in modules:
                 self._stubs.smart_set(module, name, self.fake_modules[attr])
         for name, modules in self.SKIPPED_FS_MODULES.items():
             for module, attr in modules:
                 if attr in self.unfaked_modules:
                     self._stubs.smart_set(module, name, self.unfaked_modules[attr])
+        if sys.version_info >= (3, 12):
+            # workaround for patching open - does not work with skip modules
+            self._stubs.smart_set(builtins, "open", self.fake_open)
 
     def patch_defaults(self) -> None:
         for fct, idx, ft in self.FS_DEFARGS:
             method, mod_name = self._fake_module_functions[ft.__name__][ft.__module__]
             fake_module = self.fake_modules[mod_name]
-            attr = method.__get__(fake_module, fake_module.__class__)
+            attr = method.__get__(
+                fake_module, fake_module.__class__
+            )  # pytype: disable=attribute-error
             new_defaults = []
             assert fct.__defaults__ is not None
             for i, d in enumerate(fct.__defaults__):
                 if i == idx:
                     new_defaults.append(attr)
                 else:
                     new_defaults.append(d)
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_io.py` & `pyfakefs-5.2.3/pyfakefs/fake_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     AnyStr,
     IO,
     TYPE_CHECKING,
 )
 
 from pyfakefs.fake_file import AnyFileWrapper
 from pyfakefs.fake_open import FakeFileOpen
+from pyfakefs.helpers import IS_PYPY
 
 if TYPE_CHECKING:
     from pyfakefs.fake_filesystem import FakeFilesystem
 
 
 class PatchMode(Enum):
     """Defines if patching shall be on, off, or in automatic mode.
@@ -98,15 +99,15 @@
         module_name = module_name.replace(os.sep, ".")
         if any(
             [
                 module_name == sn or module_name.endswith("." + sn)
                 for sn in self.skip_names
             ]
         ):
-            return io.open(
+            return io.open(  # pytype: disable=wrong-arg-count
                 file,
                 mode,
                 buffering,
                 encoding,
                 errors,
                 newline,
                 closefd,
@@ -120,15 +121,15 @@
     if sys.version_info >= (3, 8):
 
         def open_code(self, path):
             """Redirect the call to open. Note that the behavior of the real
             function may be overridden by an earlier call to the
             PyFile_SetOpenCodeHook(). This behavior is not reproduced here.
             """
-            if not isinstance(path, str):
+            if not isinstance(path, str) and not IS_PYPY:
                 raise TypeError("open_code() argument 'path' must be str, not int")
             patch_mode = self.filesystem.patch_open_code
             if (
                 patch_mode == PatchMode.AUTO
                 and self.filesystem.exists(path)
                 or patch_mode == PatchMode.ON
             ):
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_open.py` & `pyfakefs-5.2.3/pyfakefs/fake_open.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,15 +279,17 @@
                     file_object.set_contents("")
         else:
             if open_modes.must_exist:
                 self.filesystem.raise_os_error(errno.ENOENT, file_path)
             if self.filesystem.islink(file_path):
                 link_object = self.filesystem.resolve(file_path, follow_symlinks=False)
                 assert link_object.contents is not None
-                target_path = cast(AnyStr, link_object.contents)
+                target_path = cast(
+                    AnyStr, link_object.contents
+                )  # pytype: disable=invalid-annotation
             else:
                 target_path = file_path
             if self.filesystem.ends_with_path_separator(target_path):
                 error = (
                     errno.EINVAL
                     if self.filesystem.is_windows_fs
                     else errno.ENOENT
@@ -313,18 +315,23 @@
             if isinstance(wrapper, FakeFileWrapper):
                 self._delete_on_close = wrapper.delete_on_close
             file_object = cast(
                 FakeFile, self.filesystem.get_open_file(filedes).get_object()
             )
             assert file_object is not None
             path = file_object.name
-            return file_object, cast(AnyStr, path), filedes, cast(AnyStr, path)
+            return (
+                file_object,
+                cast(AnyStr, path),  # pytype: disable=invalid-annotation
+                filedes,
+                cast(AnyStr, path),  # pytype: disable=invalid-annotation
+            )
 
         # open a file file by path
-        file_path = cast(AnyStr, file_)
+        file_path = cast(AnyStr, file_)  # pytype: disable=invalid-annotation
         if file_path == self.filesystem.dev_null.name:
             file_object = self.filesystem.dev_null
             real_path = file_path
         else:
             real_path = self.filesystem.resolve_path(file_path)
             if self.filesystem.exists(file_path):
                 file_object = self.filesystem.get_object_from_normpath(
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_os.py` & `pyfakefs-5.2.3/pyfakefs/fake_os.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,15 +499,17 @@
             OSError: if the path does not exist.
         """
         if not self.filesystem.is_linux:
             raise AttributeError("module 'os' has no attribute 'listxattr'")
 
         path_str = self.filesystem.cwd if path is None else path
         file_obj = self.filesystem.resolve(
-            cast(AnyStr, path_str), follow_symlinks, allow_fd=True
+            cast(AnyStr, path_str),  # pytype: disable=invalid-annotation
+            follow_symlinks,
+            allow_fd=True,
         )
         return list(file_obj.xattr.keys())
 
     def removexattr(
         self, path: AnyStr, attribute: AnyString, *, follow_symlinks: bool = True
     ) -> None:
         """Removes the extended filesystem attribute attribute from `path`.
@@ -1342,25 +1344,26 @@
     def handle_original_call(f: Callable) -> Callable:
         """Decorator used for real pathlib Path methods to ensure that
         real os functions instead of faked ones are used.
         Applied to all non-private methods of `FakeOsModule`."""
 
         @functools.wraps(f)
         def wrapped(*args, **kwargs):
-            if not f.__name__.startswith("_") and FakeOsModule.use_original:
+            if FakeOsModule.use_original:
                 # remove the `self` argument for FakeOsModule methods
                 if args and isinstance(args[0], FakeOsModule):
                     args = args[1:]
                 return getattr(os, f.__name__)(*args, **kwargs)
             return f(*args, **kwargs)
 
         return wrapped
 
     for name, fn in inspect.getmembers(FakeOsModule, inspect.isfunction):
-        setattr(FakeOsModule, name, handle_original_call(fn))
+        if not fn.__name__.startswith("_"):
+            setattr(FakeOsModule, name, handle_original_call(fn))
 
 
 @contextmanager
 def use_original_os():
     """Temporarily use original os functions instead of faked ones.
     Used to ensure that skipped modules do not use faked calls.
     """
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_path.py` & `pyfakefs-5.2.3/pyfakefs/fake_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     Tuple,
     AnyStr,
     overload,
     ClassVar,
     TYPE_CHECKING,
 )
 
-from pyfakefs import __version__  # noqa: F401 for upwards compatibility
 from pyfakefs.helpers import (
     make_string_path,
     to_string,
     matching_string,
 )
 
 if TYPE_CHECKING:
@@ -497,15 +496,15 @@
 
         def __init__(self, filesystem: "FakeFilesystem"):
             """Init.
 
             Args:
                 filesystem: FakeFilesystem used to provide file system information
             """
-            import nt
+            import nt  # type:ignore[import]
 
             self.filesystem = filesystem
             self.nt_module: Any = nt
 
         if sys.version_info >= (3, 12):
 
             def _path_isdir(self, path: AnyStr) -> bool:
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_pathlib.py` & `pyfakefs-5.2.3/pyfakefs/fake_pathlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from urllib.parse import quote_from_bytes as urlquote_from_bytes
 
 from pyfakefs import fake_scandir
 from pyfakefs.extra_packages import use_scandir
 from pyfakefs.fake_filesystem import FakeFilesystem
 from pyfakefs.fake_open import FakeFileOpen
 from pyfakefs.fake_os import FakeOsModule, use_original_os
+from pyfakefs.helpers import IS_PYPY
 
 
 def init_module(filesystem):
     """Initializes the fake module with the fake file system."""
     # pylint: disable=protected-access
     FakePath.filesystem = filesystem
     if sys.version_info < (3, 12):
@@ -86,20 +87,20 @@
     def _wrapped(pathobj1, pathobj2, *args):
         return strfunc(pathobj2.filesystem, str(pathobj2), str(pathobj1), *args)
 
     return staticmethod(_wrapped)
 
 
 try:
-    accessor = pathlib._Accessor  # type: ignore [attr-defined]
+    accessor = pathlib._Accessor  # type: ignore[attr-defined]
 except AttributeError:
     accessor = object
 
 
-class _FakeAccessor(accessor):  # type: ignore [valid-type, misc]
+class _FakeAccessor(accessor):  # type: ignore[valid-type, misc]
     """Accessor which forwards some of the functions to FakeFilesystem
     methods.
     """
 
     stat = _wrap_strfunc(FakeFilesystem.stat)
 
     lstat = _wrap_strfunc(
@@ -126,17 +127,16 @@
     def chmod(self, pathobj, *args, **kwargs):
         if "follow_symlinks" in kwargs:
             if sys.version_info < (3, 10):
                 raise TypeError(
                     "chmod() got an unexpected keyword " "argument 'follow_symlinks'"
                 )
 
-            if (
-                not kwargs["follow_symlinks"]
-                and os.os_module.chmod not in os.os_module.supports_follow_symlinks
+            if not kwargs["follow_symlinks"] and (
+                os.chmod not in os.supports_follow_symlinks or IS_PYPY
             ):
                 raise NotImplementedError(
                     "`follow_symlinks` for chmod() is not available " "on this system"
                 )
         return pathobj.filesystem.chmod(str(pathobj), *args, **kwargs)
 
     mkdir = _wrap_strfunc(FakeFilesystem.makedir)
@@ -181,17 +181,17 @@
 
     utime = _wrap_strfunc(FakeFilesystem.utime)
 
 
 _fake_accessor = _FakeAccessor()
 
 if sys.version_info < (3, 12):
-    flavour = pathlib._Flavour  # type: ignore [attr-defined]
+    flavour = pathlib._Flavour  # type: ignore[attr-defined]
 
-    class _FakeFlavour(flavour):  # type: ignore [valid-type, misc]
+    class _FakeFlavour(flavour):  # type: ignore[valid-type, misc]
         """Fake Flavour implementation used by PurePath and _Flavour"""
 
         filesystem = None
         sep = "/"
         altsep = None
         has_drv = False
 
@@ -517,26 +517,26 @@
         if cls is FakePathlibModule.Path:
             cls = (
                 FakePathlibModule.WindowsPath
                 if cls.filesystem.is_windows_fs
                 else FakePathlibModule.PosixPath
             )
         if sys.version_info < (3, 12):
-            return cls._from_parts(args)
+            return cls._from_parts(args)  # pytype: disable=attribute-error
         else:
             return object.__new__(cls)
 
     if sys.version_info[:2] == (3, 10):
         # Overwritten class methods to call _init to set the fake accessor,
         # which is not done in Python 3.10, and not needed from Python 3.11 on
         @classmethod
-        def _from_parts(cls, args, init=False):  # pylint: disable=unused-argument
+        def _from_parts(cls, args):
             self = object.__new__(cls)
             self._init()
-            drv, root, parts = self._parse_args(args)
+            drv, root, parts = self._parse_args(args)  # pytype: disable=attribute-error
             self._drv = drv
             self._root = root
             self._parts = parts
             return self
 
         @classmethod
         def _from_parsed_parts(cls, drv, root, parts):
@@ -590,15 +590,17 @@
             else:
                 if strict is not None:
                     raise TypeError(
                         "resolve() got an unexpected keyword argument 'strict'"
                     )
                 strict = True
             self._raise_on_closed()
-            path = self._flavour.resolve(self, strict=strict)
+            path = self._flavour.resolve(
+                self, strict=strict
+            )  # pytype: disable=attribute-error
             if path is None:
                 self.stat()
                 path = str(self.absolute())
             path = self.filesystem.absnormpath(path)
             return FakePath(path)
 
     def open(self, mode="r", buffering=-1, encoding=None, errors=None, newline=None):
@@ -616,37 +618,41 @@
     def read_bytes(self):
         """Open the fake file in bytes mode, read it, and close the file.
 
         Raises:
             OSError: if the target object is a directory, the path is
                 invalid or permission is denied.
         """
-        with FakeFileOpen(self.filesystem)(self._path(), mode="rb") as f:
+        with FakeFileOpen(self.filesystem)(
+            self._path(), mode="rb"
+        ) as f:  # pytype: disable=attribute-error
             return f.read()
 
     def read_text(self, encoding=None, errors=None):
         """
         Open the fake file in text mode, read it, and close the file.
         """
-        with FakeFileOpen(self.filesystem)(
+        with FakeFileOpen(self.filesystem)(  # pytype: disable=attribute-error
             self._path(), mode="r", encoding=encoding, errors=errors
         ) as f:
             return f.read()
 
     def write_bytes(self, data):
         """Open the fake file in bytes mode, write to it, and close the file.
         Args:
             data: the bytes to be written
         Raises:
             OSError: if the target object is a directory, the path is
                 invalid or permission is denied.
         """
         # type-check for the buffer interface before truncating the file
         view = memoryview(data)
-        with FakeFileOpen(self.filesystem)(self._path(), mode="wb") as f:
+        with FakeFileOpen(self.filesystem)(
+            self._path(), mode="wb"
+        ) as f:  # pytype: disable=attribute-error
             return f.write(view)
 
     def write_text(self, data, encoding=None, errors=None, newline=None):
         """Open the fake file in text mode, write to it, and close
         the file.
 
         Args:
@@ -663,15 +669,15 @@
         """
         if not isinstance(data, str):
             raise TypeError("data must be str, not %s" % data.__class__.__name__)
         if newline is not None and sys.version_info < (3, 10):
             raise TypeError(
                 "write_text() got an unexpected " "keyword argument 'newline'"
             )
-        with FakeFileOpen(self.filesystem)(
+        with FakeFileOpen(self.filesystem)(  # pytype: disable=attribute-error
             self._path(),
             mode="w",
             encoding=encoding,
             errors=errors,
             newline=newline,
         ) as f:
             return f.write(data)
@@ -754,20 +760,20 @@
 
         def is_absolute(self):
             if self.filesystem.is_windows_fs:
                 return self.drive and self.root
             return os.path.isabs(self._path())
 
         def is_reserved(self):
-            if not self.filesystem.is_windows_fs or not self._parts:
+            if not self.filesystem.is_windows_fs or not self._tail:
                 return False
-            if self._parts[0].startswith("\\\\"):
+            if self._tail[0].startswith("\\\\"):
                 # UNC paths are never reserved.
                 return False
-            name = self._parts[-1].partition(".")[0].partition(":")[0].rstrip(" ")
+            name = self._tail[-1].partition(".")[0].partition(":")[0].rstrip(" ")
             return name.upper() in pathlib._WIN_RESERVED_NAMES
 
 
 class FakePathlibModule:
     """Uses FakeFilesystem to provide a fake pathlib module replacement.
     Can be used to replace both the standard `pathlib` module and the
     `pathlib2` package available on PyPi.
@@ -882,20 +888,20 @@
     else:
         _flavour = ntpath if os.name == "nt" else posixpath
 
     def __new__(cls, *args, **kwargs):
         """Creates the correct subclass based on OS."""
         if cls is RealPathlibModule.Path:
             cls = (
-                RealPathlibModule.WindowsPath
+                RealPathlibModule.WindowsPath  # pytype: disable=attribute-error
                 if os.name == "nt"
-                else RealPathlibModule.PosixPath
+                else RealPathlibModule.PosixPath  # pytype: disable=attribute-error
             )
         if sys.version_info < (3, 12):
-            return cls._from_parts(args)
+            return cls._from_parts(args)  # pytype: disable=attribute-error
         else:
             return object.__new__(cls)
 
 
 if sys.version_info > (3, 10):
 
     def with_original_os(f: Callable) -> Callable:
@@ -906,15 +912,16 @@
         def wrapped(*args, **kwargs):
             with use_original_os():
                 return f(*args, **kwargs)
 
         return wrapped
 
     for name, fn in inspect.getmembers(RealPath, inspect.isfunction):
-        setattr(RealPath, name, with_original_os(fn))
+        if not name.startswith("__"):
+            setattr(RealPath, name, with_original_os(fn))
 
 
 class RealPathlibPathModule:
     """Patches `pathlib.Path` by passing all calls to RealPathlibModule."""
 
     real_pathlib = None
```

### Comparing `pyfakefs-5.2.2/pyfakefs/fake_scandir.py` & `pyfakefs-5.2.3/pyfakefs/fake_scandir.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/helpers.py` & `pyfakefs-5.2.3/pyfakefs/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 @overload
 def make_string_path(dir_name: os.PathLike) -> str:
     ...
 
 
 def make_string_path(dir_name: AnyPath) -> AnyStr:
-    return cast(AnyStr, os.fspath(dir_name))
+    return cast(AnyStr, os.fspath(dir_name))  # pytype: disable=invalid-annotation
 
 
 def to_string(path: Union[AnyStr, Union[str, bytes]]) -> str:
     """Return the string representation of a byte string using the preferred
     encoding, or the string itself if path is a str."""
     if isinstance(path, bytes):
         return path.decode(locale.getpreferredencoding(False))
@@ -178,15 +178,15 @@
     """Return the string as byte or unicode depending
     on the type of matched, assuming string is an ASCII string.
     """
     if string is None:
         return string
     if isinstance(matched, bytes) and isinstance(string, str):
         return string.encode(locale.getpreferredencoding(False))
-    return string
+    return string  # pytype: disable=bad-return-type
 
 
 class FakeStatResult:
     """Mimics os.stat_result for use as return type of `stat()` and similar.
     This is needed as `os.stat_result` has no possibility to set
     nanosecond times directly.
     """
```

### Comparing `pyfakefs-5.2.2/pyfakefs/mox3_stubout.py` & `pyfakefs-5.2.3/pyfakefs/mox3_stubout.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         if orig_attr is None:
             raise AttributeError("Attribute not found.")
 
         # Calling getattr() on a staticmethod transforms it to a 'normal'
         # function. We need to ensure that we put it back as a staticmethod.
         old_attribute = obj.__dict__.get(attr_name)
         if old_attribute is not None and isinstance(old_attribute, staticmethod):
-            orig_attr = staticmethod(orig_attr)
+            orig_attr = staticmethod(orig_attr)  # pytype: disable=not-callable
 
         self.stubs.append((orig_obj, attr_name, orig_attr))
         setattr(orig_obj, attr_name, new_attr)
 
     def smart_unset_all(self):
         """Reverses all the SmartSet() calls.
```

### Comparing `pyfakefs-5.2.2/pyfakefs/patched_packages.py` & `pyfakefs-5.2.3/pyfakefs/patched_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         modules_to_patch["django.core.files.locks"] = FakeLocks
     return modules_to_patch
 
 
 def get_classes_to_patch():
     classes_to_patch = {}
     if patch_pandas:
-        classes_to_patch["TextFileReader"] = "pandas.io.parsers"
+        classes_to_patch["TextFileReader"] = ["pandas.io.parsers"]
     return classes_to_patch
 
 
 def get_fake_module_classes():
     fake_module_classes = {}
     if patch_pandas:
         fake_module_classes["TextFileReader"] = FakeTextFileReader
```

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_plugin.py` & `pyfakefs-5.2.3/pyfakefs/pytest_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,28 @@
 
 def my_fakefs_test(fs):
     fs.create_file('/var/data/xx1.txt')
     assert os.path.exists('/var/data/xx1.txt')
 """
 import py
 import pytest
+from _pytest import capture
 
 from pyfakefs.fake_filesystem_unittest import Patcher
 
+try:
+    from _pytest import pathlib
+except ImportError:
+    pathlib = None
+
 Patcher.SKIPMODULES.add(py)
 Patcher.SKIPMODULES.add(pytest)
+Patcher.SKIPMODULES.add(capture)
+if pathlib is not None:
+    Patcher.SKIPMODULES.add(pathlib)
 
 
 @pytest.fixture
 def fs(request):
     """Fake filesystem."""
     if hasattr(request, "param"):
         # pass optional parameters via @pytest.mark.parametrize
```

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/conftest.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/example.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_doctest_test.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_doctest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_param_test.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_fixture_param_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_test.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_module_fixture_test.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_module_fixture_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 
 @pytest.fixture(scope="module", autouse=True)
 def use_fs(fs_module):
     fs_module.create_file(os.path.join("foo", "bar"))
     yield fs_module
 
 
-def test_fs_uses_fs_module(fs):
+@pytest.mark.usefixtures("fs")
+def test_fs_uses_fs_module():
     # check that `fs` uses the same filesystem as `fs_module`
     assert os.path.exists(os.path.join("foo", "bar"))
```

### Comparing `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_plugin_test.py` & `pyfakefs-5.2.3/pyfakefs/pytest_tests/pytest_plugin_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests that the pytest plugin properly provides the "fs" fixture"""
 import os
 import tempfile
 
+from pyfakefs.fake_filesystem import OSType
 from pyfakefs.fake_filesystem_unittest import Pause
 import pyfakefs.pytest_tests.io
 
 
 def test_fs_fixture(fs):
     fs.create_file("/var/data/xx1.txt")
     assert os.path.exists("/var/data/xx1.txt")
@@ -56,7 +57,22 @@
 def test_use_own_io_module(fs):
     filepath = "foo.txt"
     with open(filepath, "w") as f:
         f.write("bar")
 
     stream = pyfakefs.pytest_tests.io.InputStream(filepath)
     assert stream.read() == "bar"
+
+
+def test_switch_to_windows(fs):
+    fs.os = OSType.WINDOWS
+    assert os.path.exists(tempfile.gettempdir())
+
+
+def test_switch_to_linux(fs):
+    fs.os = OSType.LINUX
+    assert os.path.exists(tempfile.gettempdir())
+
+
+def test_switch_to_macos(fs):
+    fs.os = OSType.MACOS
+    assert os.path.exists(tempfile.gettempdir())
```

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/all_tests.py` & `pyfakefs-5.2.3/pyfakefs/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/all_tests_without_extra_packages.py` & `pyfakefs-5.2.3/pyfakefs/tests/all_tests_without_extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/dynamic_patch_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/dynamic_patch_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/example.py` & `pyfakefs-5.2.3/pyfakefs/tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/example_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_glob_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_glob_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_shutil_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_shutil_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import shutil
 import sys
 import tempfile
 import unittest
 from pathlib import Path
 
 from pyfakefs import fake_filesystem_unittest
-from pyfakefs.helpers import get_uid, set_uid, is_root
+from pyfakefs.helpers import get_uid, set_uid, is_root, IS_PYPY
 from pyfakefs.tests.test_utils import RealFsTestMixin
 
 is_windows = sys.platform == "win32"
 
 
 class RealFsTestCase(fake_filesystem_unittest.TestCase, RealFsTestMixin):
     def __init__(self, methodName="runTest"):
@@ -227,14 +227,15 @@
         shutil.copystat(src_file, dst_file)
         src_stat = os.stat(src_file)
         dst_stat = os.stat(dst_file)
         self.assertEqual(src_stat.st_mode, dst_stat.st_mode)
         self.assertAlmostEqual(src_stat.st_atime, dst_stat.st_atime, places=2)
         self.assertAlmostEqual(src_stat.st_mtime, dst_stat.st_mtime, places=2)
 
+    @unittest.skipIf(IS_PYPY, "Functionality not supported in PyPy")
     def test_copystat_symlinks(self):
         """Regression test for #799"""
         self.skip_if_symlink_not_supported()
         f = self.make_path("xyzzy")
         self.create_file(f)
         sym1 = self.make_path("sym1")
         sym2 = self.make_path("sym2")
```

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_unittest_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_unittest_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import pathlib
 import runpy
 import shutil
 import sys
 import tempfile
 import unittest
 import warnings
-from distutils.dir_util import copy_tree, remove_tree
 from pathlib import Path
 from unittest import TestCase, mock
 
 import pyfakefs.tests.import_as_example
 import pyfakefs.tests.logsio
 from pyfakefs import fake_filesystem_unittest, fake_filesystem
 from pyfakefs.fake_filesystem import OSType
@@ -40,14 +39,18 @@
     Patcher,
     Pause,
     patchfs,
     PatchMode,
 )
 from pyfakefs.tests.fixtures import module_with_attributes
 
+if sys.version_info < (3, 12):
+    # distutils removed in Python 3.12
+    from distutils.dir_util import copy_tree, remove_tree
+
 
 class TestPatcher(TestCase):
     def test_context_manager(self):
         with Patcher() as patcher:
             patcher.fs.create_file("/foo/bar", contents="test")
             with open("/foo/bar") as f:
                 contents = f.read()
@@ -148,17 +151,17 @@
         self.assertTrue(self.fs.exists("/test/dir1/dir2b"))
         self.assertTrue(self.fs.exists("/test/dir1/dir2a"))
 
         shutil.rmtree("/test/dir1")
         self.assertFalse(self.fs.exists("/test/dir1"))
 
     def test_fakepathlib(self):
-        with pathlib.Path("/fake_file.txt") as p:
-            with p.open("w") as f:
-                f.write("text")
+        p = pathlib.Path("/fake_file.txt")
+        with p.open("w") as f:
+            f.write("text")
         is_windows = sys.platform.startswith("win")
         if is_windows:
             self.assertTrue(self.fs.exists(r"\fake_file.txt"))
         else:
             self.assertTrue(self.fs.exists("/fake_file.txt"))
 
 
@@ -221,20 +224,22 @@
 
     def test_import_function_from_os_as_other_name(self):
         file_path = "/foo/bar"
         self.fs.create_file(file_path, contents=b"abc")
         stat_result = pyfakefs.tests.import_as_example.file_stat2(file_path)
         self.assertEqual(3, stat_result.st_size)
 
+    @unittest.skipIf(sys.version_info >= (3, 12), "Currently not working in 3.12")
     def test_import_open_as_other_name(self):
         file_path = "/foo/bar"
         self.fs.create_file(file_path, contents=b"abc")
         contents = pyfakefs.tests.import_as_example.file_contents1(file_path)
         self.assertEqual("abc", contents)
 
+    @unittest.skipIf(sys.version_info >= (3, 12), "Currently not working in 3.12")
     def test_import_io_open_as_other_name(self):
         file_path = "/foo/bar"
         self.fs.create_file(file_path, contents=b"abc")
         contents = pyfakefs.tests.import_as_example.file_contents2(file_path)
         self.assertEqual("abc", contents)
 
 
@@ -389,14 +394,18 @@
         self.fs.create_file("foo")
         self.assertFalse(pyfakefs.tests.import_as_example.check_if_exists6("foo"))
 
     def test_fake_path_does_not_exist7(self):
         self.fs.create_file("foo")
         self.assertFalse(pyfakefs.tests.import_as_example.check_if_exists7("foo"))
 
+    @unittest.skipIf(
+        sys.version_info >= (3, 12),
+        "Skip modules currently not working for open in 3.12",
+    )
     def test_open_succeeds(self):
         pyfakefs.tests.import_as_example.open_this_file()
 
     def test_path_succeeds(self):
         pyfakefs.tests.import_as_example.return_this_file_path()
 
 
@@ -434,14 +443,18 @@
         self.fs.create_file("foo")
         self.assertFalse(pyfakefs.tests.import_as_example.check_if_exists6("foo"))
 
     def test_fake_path_does_not_exist7(self):
         self.fs.create_file("foo")
         self.assertFalse(pyfakefs.tests.import_as_example.check_if_exists7("foo"))
 
+    @unittest.skipIf(
+        sys.version_info >= (3, 12),
+        "Skip modules currently not working for open in 3.12",
+    )
     def test_open_succeeds(self):
         pyfakefs.tests.import_as_example.open_this_file()
 
     def test_path_succeeds(self):
         pyfakefs.tests.import_as_example.return_this_file_path()
 
 
@@ -653,19 +666,19 @@
 
 class TestTempDirCreation(fake_filesystem_unittest.TestCase):
     """Test that the temp directory exists at test start."""
 
     def setUp(self):
         self.setUpPyfakefs()
 
-    def testTempDirExists(self):
+    def test_tempdir_exists(self):
         self.assertTrue(os.path.exists(tempfile.gettempdir()))
 
     @unittest.skipIf(sys.platform == "win32", "POSIX only test")
-    def testTmpExists(self):
+    def test_tmp_exists(self):
         # directory or link under Linux, link under macOS
         self.assertTrue(os.path.exists("/tmp"))
 
 
 class TestTempFileReload(unittest.TestCase):
     """Regression test for #356 to make sure that reloading the tempfile
     does not affect other tests."""
@@ -700,39 +713,41 @@
         shutil.make_archive("archive", "zip", root_dir="foo")
 
     def test_b(self):
         # used to fail because 'bar' could not be found
         shutil.make_archive("archive", "zip", root_dir="foo")
 
 
-class TestDistutilsCopyTree(fake_filesystem_unittest.TestCase):
-    """Regression test for #501."""
+if sys.version_info < (3, 12):
 
-    def setUp(self):
-        self.setUpPyfakefs()
-        self.fs.create_dir("./test/subdir/")
-        self.fs.create_dir("./test/subdir2/")
-        self.fs.create_file("./test2/subdir/1.txt")
-
-    def test_file_copied(self):
-        copy_tree("./test2/", "./test/")
-        remove_tree("./test2/")
-
-        self.assertTrue(os.path.isfile("./test/subdir/1.txt"))
-        self.assertFalse(os.path.isdir("./test2/"))
-
-    def test_file_copied_again(self):
-        # used to fail because 'test2' could not be found
-        self.assertTrue(os.path.isfile("./test2/subdir/1.txt"))
+    class TestDistutilsCopyTree(fake_filesystem_unittest.TestCase):
+        """Regression test for #501."""
+
+        def setUp(self):
+            self.setUpPyfakefs()
+            self.fs.create_dir("./test/subdir/")
+            self.fs.create_dir("./test/subdir2/")
+            self.fs.create_file("./test2/subdir/1.txt")
+
+        def test_file_copied(self):
+            copy_tree("./test2/", "./test/")
+            remove_tree("./test2/")
+
+            self.assertTrue(os.path.isfile("./test/subdir/1.txt"))
+            self.assertFalse(os.path.isdir("./test2/"))
+
+        def test_file_copied_again(self):
+            # used to fail because 'test2' could not be found
+            self.assertTrue(os.path.isfile("./test2/subdir/1.txt"))
 
-        copy_tree("./test2/", "./test/")
-        remove_tree("./test2/")
+            copy_tree("./test2/", "./test/")
+            remove_tree("./test2/")
 
-        self.assertTrue(os.path.isfile("./test/subdir/1.txt"))
-        self.assertFalse(os.path.isdir("./test2/"))
+            self.assertTrue(os.path.isfile("./test/subdir/1.txt"))
+            self.assertFalse(os.path.isdir("./test2/"))
 
 
 class PathlibTest(TestCase):
     """Regression test for #527"""
 
     @patchfs
     def test_cwd(self, fs):
```

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_vs_real_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_filesystem_vs_real_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_open_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_open_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import stat
 import sys
 import time
 import unittest
 
 from pyfakefs import fake_filesystem, helpers
-from pyfakefs.helpers import is_root
+from pyfakefs.helpers import is_root, IS_PYPY
 from pyfakefs.fake_io import FakeIoModule
 from pyfakefs.fake_filesystem_unittest import PatchMode
 from pyfakefs.tests.test_utils import RealFsTestCase
 
 
 class FakeFileOpenTestBase(RealFsTestCase):
     def setUp(self):
@@ -1053,18 +1053,27 @@
             self.open_code = self.fake_io_module.open_code
 
     def tearDown(self):
         if not self.use_real_fs():
             self.filesystem.patch_open_code = False
         super(FakeFilePatchedOpenCodeTest, self).tearDown()
 
+    @unittest.skipIf(IS_PYPY, "Different behavior in PyPy")
     def test_invalid_path(self):
         with self.assertRaises(TypeError):
             self.open_code(4)
 
+    @unittest.skipIf(not IS_PYPY, "Different behavior in PyPy")
+    def test_open_code_fd_pypy(self):
+        file_path = self.make_path("foo")
+        self.create_file(file_path, contents="test")
+        fd = self.os.open(file_path, os.O_RDONLY)
+        with self.open_code(fd) as f:
+            assert f.read() == b"test"
+
     def test_byte_contents_open_code(self):
         byte_fractions = b"\xe2\x85\x93 \xe2\x85\x94 \xe2\x85\x95 \xe2\x85\x96"
         file_path = self.make_path("foo")
         self.create_file(file_path, contents=byte_fractions)
         with self.open_code(file_path) as f:
             contents = f.read()
         self.assertEqual(contents, byte_fractions)
@@ -1086,14 +1095,15 @@
     def setUp(self):
         super(FakeFileUnpatchedOpenCodeTest, self).setUp()
         if self.use_real_fs():
             self.open_code = io.open_code
         else:
             self.open_code = self.fake_io_module.open_code
 
+    @unittest.skipIf(IS_PYPY, "Different behavior in PyPy")
     def test_invalid_path(self):
         with self.assertRaises(TypeError):
             self.open_code(4)
 
     def test_open_code_in_real_fs(self):
         file_path = __file__
```

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_os_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_os_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_pathlib_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_pathlib_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_stat_time_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_stat_time_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fake_tempfile_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/fake_tempfile_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fixtures/deprecated_property.py` & `pyfakefs-5.2.3/pyfakefs/tests/fixtures/deprecated_property.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/fixtures/module_with_attributes.py` & `pyfakefs-5.2.3/pyfakefs/tests/fixtures/module_with_attributes.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/import_as_example.py` & `pyfakefs-5.2.3/pyfakefs/tests/import_as_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/logsio.py` & `pyfakefs-5.2.3/pyfakefs/tests/logsio.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_example.py` & `pyfakefs-5.2.3/pyfakefs/tests/mox3_stubout_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/mox3_stubout_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/patched_packages_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/patched_packages_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # limitations under the License.
 
 """
 Provides patches for some commonly used modules that enable them to work
 with pyfakefs.
 """
 import os
+import sys
 import unittest
 
 from pyfakefs import fake_filesystem_unittest
 from pyfakefs.helpers import IS_PYPY
 
 try:
     import pandas as pd
@@ -32,15 +33,17 @@
 
 try:
     import openpyxl
 except ImportError:
     openpyxl = None
 
 
-@unittest.skipIf(IS_PYPY, "Has a problem with current PyPy")
+@unittest.skipIf(
+    IS_PYPY and sys.version_info < (3, 8), "Has a problem with older PyPy versions"
+)
 class TestPatchedPackages(fake_filesystem_unittest.TestCase):
     def setUp(self):
         self.setUpPyfakefs()
 
     if pd is not None:
 
         def test_read_csv(self):
```

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/performance_test.py` & `pyfakefs-5.2.3/pyfakefs/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.2/pyfakefs/tests/test_utils.py` & `pyfakefs-5.2.3/pyfakefs/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+# Disable attribute errors - attributes not be found in mixin (shall be cleaned up...)
+# pytype: disable=attribute-error
 """Common helper classes used in tests, or as test class base."""
 import os
 import platform
 import shutil
 import stat
 import sys
 import tempfile
```

### Comparing `pyfakefs-5.2.2/pyfakefs.egg-info/PKG-INFO` & `pyfakefs-5.2.3/pyfakefs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.2.2
+Version: 5.2.3
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
@@ -37,18 +37,24 @@
 
 
 pyfakefs implements a fake file system that mocks the Python file system modules.
 Using pyfakefs, your tests operate on a fake file system in memory without
 touching the real disk. The software under test requires no modification to
 work with pyfakefs.
 
-pyfakefs acts as a `pytest` plugin by providing the `fs` fixture, which will
-automatically invoke the fake filesystem. It also provides
-the `fake_filesystem_unittest.TestCase` class for use with `unittest` and
-the means to use the fake filesystem with other test frameworks.
+Pyfakefs creates a new empty in-memory file system at each test start, which replaces
+the real filesystem during the test. Think of pyfakefs as making a per-test temporary
+directory, except for an entire file system.
+
+There are several means to achieve this: by using
+the `fs` fixture if running pytest, by using `fake_filesystem_unittest.TestCase` as a
+base class if using unittest, by using a `fake_filesystem_unittest.Patcher` instance
+as a context manager, or by using the `patchfs` decorator.
+
+
 
 pyfakefs works with current versions of Linux, Windows and macOS.
 
 ## Documentation
 
 This document provides a general overview for pyfakefs.  There is more:
```

### Comparing `pyfakefs-5.2.2/pyfakefs.egg-info/SOURCES.txt` & `pyfakefs-5.2.3/pyfakefs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pyfakefs/fake_os.py
 pyfakefs/fake_path.py
 pyfakefs/fake_pathlib.py
 pyfakefs/fake_scandir.py
 pyfakefs/helpers.py
 pyfakefs/mox3_stubout.py
 pyfakefs/patched_packages.py
+pyfakefs/py.typed
 pyfakefs/pytest_plugin.py
 pyfakefs.egg-info/PKG-INFO
 pyfakefs.egg-info/SOURCES.txt
 pyfakefs.egg-info/dependency_links.txt
 pyfakefs.egg-info/entry_points.txt
 pyfakefs.egg-info/top_level.txt
 pyfakefs/pytest_tests/__init__.py
```

### Comparing `pyfakefs-5.2.2/setup.cfg` & `pyfakefs-5.2.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 python_requires = >=3.7
 test_suite = pyfakefs.tests
 include_package_data = True
 
 [options.packages.find]
 exclude = docs
 
+[options.package_data]
+pyfakefs = py.typed
+
 [options.entry_points]
 pytest11 = 
 	pytest_fakefs = pyfakefs.pytest_plugin
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

