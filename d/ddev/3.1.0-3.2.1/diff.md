# Comparing `tmp/ddev-3.1.0.tar.gz` & `tmp/ddev-3.2.1.tar.gz`

## Comparing `ddev-3.1.0.tar` & `ddev-3.2.1.tar`

### file list

```diff
@@ -1,111 +1,117 @@
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 ddev-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 ddev-3.1.0/pyoxidizer.bzl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/py.typed
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/application.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/clean/__init__.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/meta/scripts/upgrade_python.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/list_versions/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/licenses.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/openmetrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/file.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/config.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/git.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/__init__.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/conftest.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/test__utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/clean/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/clean/test_clean.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/meta/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/meta/scripts/test_upgrade_python.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/release/__init__.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/release/test_list_versions.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/test_licenses.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/test_manifest.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/test_openmetrics.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/config/__init__.py
--rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/config/test_model.py
--rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/list_versions/success_disk.yaml
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/manifest/missing_app_uuid.yaml
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/manifest/success.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/helpers/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/integration/test_core.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/integration/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/repo/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/repo/test_config.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/repo/test_core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_json.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/validation/__init__.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/validation/test_tracker.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.1.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.1.0/README.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ddev-3.1.0/hatch.toml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ddev-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ddev-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 ddev-3.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 ddev-3.2.1/pyoxidizer.bzl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/py.typed
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/application.py
+-rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/clean/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/meta/scripts/upgrade_python.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/list_versions/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/licenses.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/openmetrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23643 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/hatch/__init__.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/hatch/environment_collector.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/github.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/test__utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/clean/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/clean/test_clean.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/meta/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/meta/scripts/test_upgrade_python.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/release/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/release/test_list_versions.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/test_licenses.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/test_manifest.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/test_openmetrics.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/config/__init__.py
+-rw-r--r--   0        0        0    40884 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/config/test_model.py
+-rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/github/get_pr_found.yaml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/github/get_pr_no_match.yaml
+-rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/list_versions/success_disk.yaml
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/manifest/missing_app_uuid.yaml
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/manifest/success.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/helpers/api.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/integration/test_core.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/integration/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/repo/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/repo/test_config.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/repo/test_core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_github.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_json.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_structures.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/validation/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/validation/test_tracker.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.2.1/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.2.1/README.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ddev-3.2.1/hatch.toml
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 ddev-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ddev-3.2.1/PKG-INFO
```

### Comparing `ddev-3.1.0/CHANGELOG.md` & `ddev-3.2.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,159 @@
 # CHANGELOG - ddev
 
+## 3.2.1 / 2023-07-10
+
+***Fixed***:
+
+* Exclude click 8.1.4 to solve mypy issues. See [#15201](https://github.com/DataDog/integrations-core/pull/15201).
+
+## 3.2.0 / 2023-07-05
+
+***Added***:
+
+* Bump the minimum supported version of datadog-checks-dev. See [#15171](https://github.com/DataDog/integrations-core/pull/15171).
+* Move CLI plugins to ddev. See [#15166](https://github.com/DataDog/integrations-core/pull/15166).
+* Add VerbosityLevels class for ddev cli/terminal use. See [#14780](https://github.com/DataDog/integrations-core/pull/14780).
+* Add utilities for GitHub. See [#15036](https://github.com/DataDog/integrations-core/pull/15036).
+
 ## 3.1.0 / 2023-06-23
 
 ***Added***:
 
 * Update version of datadog-checks-dev. See [#14865](https://github.com/DataDog/integrations-core/pull/14865).
 * Add Git utilities. See [#14838](https://github.com/DataDog/integrations-core/pull/14838).
 * Add pluggy to ddev dependencies. See [#14821](https://github.com/DataDog/integrations-core/pull/14821).
 
 ## 3.0.0 / 2023-06-20
 
-* [Added] Bump the minimum version of datadog-checks-dev. See [#14785](https://github.com/DataDog/integrations-core/pull/14785).
-* [Added] Upgrade Pydantic model code generator. See [#14779](https://github.com/DataDog/integrations-core/pull/14779).
-* [Added] Use Git for versioning. See [#14778](https://github.com/DataDog/integrations-core/pull/14778).
-* [Added] Add validations for removed dependencies. See [#14556](https://github.com/DataDog/integrations-core/pull/14556).
-* [Added] Migrate `clean` command. See [#14726](https://github.com/DataDog/integrations-core/pull/14726).
-* [Added] Add `release list` command to list integration version releases. See [#14687](https://github.com/DataDog/integrations-core/pull/14687).
-* [Added] Migrate command to upgrade Python. See [#14700](https://github.com/DataDog/integrations-core/pull/14700).
-* [Fixed] Bump python version from py3.8 to py3.9. See [#14701](https://github.com/DataDog/integrations-core/pull/14701).
-* [Changed] Remove `pyperclip` dependency and clipboard functionality. See [#14782](https://github.com/DataDog/integrations-core/pull/14782).
+***Changed***: 
+
+* Remove `pyperclip` dependency and clipboard functionality. See [#14782](https://github.com/DataDog/integrations-core/pull/14782).
+
+***Added***: 
+
+* Bump the minimum version of datadog-checks-dev. See [#14785](https://github.com/DataDog/integrations-core/pull/14785).
+* Upgrade Pydantic model code generator. See [#14779](https://github.com/DataDog/integrations-core/pull/14779).
+* Use Git for versioning. See [#14778](https://github.com/DataDog/integrations-core/pull/14778).
+* Add validations for removed dependencies. See [#14556](https://github.com/DataDog/integrations-core/pull/14556).
+* Migrate `clean` command. See [#14726](https://github.com/DataDog/integrations-core/pull/14726).
+* Add `release list` command to list integration version releases. See [#14687](https://github.com/DataDog/integrations-core/pull/14687).
+* Migrate command to upgrade Python. See [#14700](https://github.com/DataDog/integrations-core/pull/14700).
+
+***Fixed***: 
+
+* Bump Python version from py3.8 to py3.9. See [#14701](https://github.com/DataDog/integrations-core/pull/14701).
+
 
 ## 2.1.0 / 2023-05-26
 
-* [Added] Add validation for metric limit. See [#14528](https://github.com/DataDog/integrations-core/pull/14528).
-* [Fixed] Consider changes to `metadata.csv` as testable. See [#14429](https://github.com/DataDog/integrations-core/pull/14429).
-* [Fixed] Account for dependency upgrades in CI matrix logic. See [#14366](https://github.com/DataDog/integrations-core/pull/14366).
-* [Fixed] Fix edge case in CI matrix construction. See [#14355](https://github.com/DataDog/integrations-core/pull/14355).
+***Added***: 
+
+* Add validation for metric limit. See [#14528](https://github.com/DataDog/integrations-core/pull/14528).
+
+***Fixed***: 
+
+* Consider changes to `metadata.csv` as testable. See [#14429](https://github.com/DataDog/integrations-core/pull/14429).
+* Account for dependency upgrades in CI matrix logic. See [#14366](https://github.com/DataDog/integrations-core/pull/14366).
+* Fix edge case in CI matrix construction. See [#14355](https://github.com/DataDog/integrations-core/pull/14355).
+
 
 ## 2.0.0 / 2023-04-11
 
-* [Changed] Replace flake8 and isort with Ruff. See [#14212](https://github.com/DataDog/integrations-core/pull/14212).
+***Changed***: 
+
+* Replace flake8 and isort with Ruff. See [#14212](https://github.com/DataDog/integrations-core/pull/14212).
+
 
 ## 1.6.0 / 2023-03-31
 
-* [Added] Add GitHub Actions workflows. See [#14187](https://github.com/DataDog/integrations-core/pull/14187).
+***Added***: 
+
+* Add GitHub Actions workflows. See [#14187](https://github.com/DataDog/integrations-core/pull/14187).
+
 
 ## 1.5.0 / 2023-03-23
 
-* [Added] Bump datadog-checks-dev to 18.x. See [#14225](https://github.com/DataDog/integrations-core/pull/14225).
+***Added***: 
+
+* Bump datadog-checks-dev to 18.x. See [#14225](https://github.com/DataDog/integrations-core/pull/14225).
+
 
 ## 1.4.3 / 2023-03-01
 
-* [Fixed] Bump datadog_checks_dev dependency version. See [#14064](https://github.com/DataDog/integrations-core/pull/14064).
+***Fixed***: 
+
+* Bump datadog_checks_dev dependency version. See [#14064](https://github.com/DataDog/integrations-core/pull/14064).
+
 
 ## 1.4.2 / 2023-02-27
 
-* [Fixed] Bump datadog_checks_dev dependency version. See [#14040](https://github.com/DataDog/integrations-core/pull/14040).
+***Fixed***: 
+
+* Bump datadog_checks_dev dependency version. See [#14040](https://github.com/DataDog/integrations-core/pull/14040).
+
 
 ## 1.4.1 / 2023-01-25
 
-* [Fixed] Pin and bump the datadog_checks_dev version. See [#13557](https://github.com/DataDog/integrations-core/pull/13557).
+***Fixed***: 
+
+* Pin and bump the datadog_checks_dev version. See [#13557](https://github.com/DataDog/integrations-core/pull/13557).
+
 
 ## 1.4.0 / 2023-01-20
 
-* [Added] Update manifest validation. See [#13637](https://github.com/DataDog/integrations-core/pull/13637).
-* [Added] Standardize integration selection. See [#13570](https://github.com/DataDog/integrations-core/pull/13570).
-* [Fixed] And fallbacks to some org config options. See [#13629](https://github.com/DataDog/integrations-core/pull/13629).
+***Added***: 
+
+* Update manifest validation. See [#13637](https://github.com/DataDog/integrations-core/pull/13637).
+* Standardize integration selection. See [#13570](https://github.com/DataDog/integrations-core/pull/13570).
+
+***Fixed***: 
+
+* And fallbacks to some org config options. See [#13629](https://github.com/DataDog/integrations-core/pull/13629).
+
 
 ## 1.3.0 / 2022-12-09
 
-* [Added] Add `validate license-header` subcommand. See [#13417](https://github.com/DataDog/integrations-core/pull/13417).
-* [Added] Add JSON Pointer utilities. See [#13464](https://github.com/DataDog/integrations-core/pull/13464).
-* [Added] Add utility for displaying warnings and errors. See [#13427](https://github.com/DataDog/integrations-core/pull/13427).
-* [Added] Add `config` commands. See [#13412](https://github.com/DataDog/integrations-core/pull/13412).
-* [Fixed] Bump datadog_checks_dev dependency to 17.5.0. See [#13490](https://github.com/DataDog/integrations-core/pull/13490).
-* [Fixed] Output non-critical information to stderr. See [#13459](https://github.com/DataDog/integrations-core/pull/13459).
+***Added***: 
+
+* Add `validate license-header` subcommand. See [#13417](https://github.com/DataDog/integrations-core/pull/13417).
+* Add JSON Pointer utilities. See [#13464](https://github.com/DataDog/integrations-core/pull/13464).
+* Add utility for displaying warnings and errors. See [#13427](https://github.com/DataDog/integrations-core/pull/13427).
+* Add `config` commands. See [#13412](https://github.com/DataDog/integrations-core/pull/13412).
+
+***Fixed***: 
+
+* Bump datadog_checks_dev dependency to 17.5.0. See [#13490](https://github.com/DataDog/integrations-core/pull/13490).
+* Output non-critical information to stderr. See [#13459](https://github.com/DataDog/integrations-core/pull/13459).
+
 
 ## 1.2.0 / 2022-11-23
 
-* [Added] Upgrade dependencies. See [#13375](https://github.com/DataDog/integrations-core/pull/13375).
+***Added***: 
+
+* Upgrade dependencies. See [#13375](https://github.com/DataDog/integrations-core/pull/13375).
+
 
 ## 1.1.0 / 2022-10-28
 
-* [Added] Add `status` command. See [#13197](https://github.com/DataDog/integrations-core/pull/13197).
-* [Added] Add Git utilities. See [#13185](https://github.com/DataDog/integrations-core/pull/13185).
-* [Added] Add utilities for filtering integrations. See [#13156](https://github.com/DataDog/integrations-core/pull/13156).
-* [Added] Add more utilities. See [#13136](https://github.com/DataDog/integrations-core/pull/13136).
+***Added***: 
+
+* Add `status` command. See [#13197](https://github.com/DataDog/integrations-core/pull/13197).
+* Add Git utilities. See [#13185](https://github.com/DataDog/integrations-core/pull/13185).
+* Add utilities for filtering integrations. See [#13156](https://github.com/DataDog/integrations-core/pull/13156).
+* Add more utilities. See [#13136](https://github.com/DataDog/integrations-core/pull/13136).
+
 
 ## 1.0.1 / 2022-09-16
 
-* [Fixed] Fix legacy tooling initialization when using the --here flag. See [#12823](https://github.com/DataDog/integrations-core/pull/12823).
+***Fixed***: 
+
+* Fix legacy tooling initialization when using the --here flag. See [#12823](https://github.com/DataDog/integrations-core/pull/12823).
+
 
 ## 1.0.0 / 2022-08-05
 
-* [Added] Make ddev a standalone package. See [#12565](https://github.com/DataDog/integrations-core/pull/12565).
+***Added***: 
+
+* Make ddev a standalone package. See [#12565](https://github.com/DataDog/integrations-core/pull/12565).
+
```

### Comparing `ddev-3.1.0/pyoxidizer.bzl` & `ddev-3.2.1/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/__init__.py` & `ddev-3.2.1/src/ddev/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,22 +114,23 @@
     ctx.obj = app
 
     try:
         app.config_file.load()
     except OSError as e:  # no cov
         app.abort(f'Error loading configuration: {e}')
 
-    app.set_repo(core, extras, marketplace, agent, here)
-
     app.config.terminal.styles.parse_fields()
     errors = app.initialize_styles(app.config.terminal.styles.raw_data)
     if errors and color is not False and not app.quiet:  # no cov
         for error in errors:
             app.display_warning(error)
 
+    # Do this last
+    app.set_repo(core, extras, marketplace, agent, here)
+
     # TODO: remove this when the old CLI is gone
     app.initialize_old_cli()
 
 
 ddev.add_command(ci)
 ddev.add_command(clean)
 ddev.add_command(config)
```

### Comparing `ddev-3.1.0/src/ddev/cli/application.py` & `ddev-3.2.1/src/ddev/cli/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,45 +3,51 @@
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from __future__ import annotations
 
 import os
 from typing import cast
 
 from ddev.cli.terminal import Terminal
-from ddev.config.constants import AppEnvVars
+from ddev.config.constants import AppEnvVars, VerbosityLevels
 from ddev.config.file import ConfigFile, RootConfig
 from ddev.repo.core import Repository
 from ddev.utils.fs import Path
+from ddev.utils.github import GitHubManager
 from ddev.utils.platform import Platform
 
 
 class Application(Terminal):
     def __init__(self, exit_func, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.platform = Platform(self.display_raw)
         self.__exit_func = exit_func
 
         self.config_file = ConfigFile()
-        self.quiet = self.verbosity < 0
-        self.verbose = self.verbosity > 0
+        self.quiet = self.verbosity < VerbosityLevels.INFO
+        self.verbose = self.verbosity > VerbosityLevels.INFO
 
-        # Lazily set this as we acquire more knowledge about the desired environment
+        # Lazily set these as we acquire more knowledge about the desired environment
         self.__repo = cast(Repository, None)
+        self.__github = cast(GitHubManager, None)
 
         # TODO: remove this when the old CLI is gone
         self.__config = {}
 
     @property
     def config(self) -> RootConfig:
         return self.config_file.model
 
     @property
     def repo(self) -> Repository:
         return self.__repo
 
+    @property
+    def github(self) -> GitHubManager:
+        return self.__github
+
     def set_repo(self, core: bool, extras: bool, marketplace: bool, agent: bool, here: bool):
         # Config looks like this:
         #
         # repo = "core"
         # [repos]
         # core = "~/dd/integrations-core"
         # extras = "~/dd/integrations-extras"
@@ -58,14 +64,18 @@
         elif here:
             self.__repo = Repository('local', str(Path.cwd()))
         elif repo := os.environ.get(AppEnvVars.REPO, ''):
             self.__repo = Repository(repo, self.config.repos[repo])
         else:
             self.__repo = Repository(self.config.repo.name, self.config.repo.path)
 
+        self.__github = GitHubManager(
+            self.repo, user=self.config.github.user, token=self.config.github.token, status=self.status
+        )
+
     def abort(self, text='', code=1, **kwargs):
         if text:
             self.display_error(text, **kwargs)
         self.__exit_func(code)
 
     # TODO: remove everything below when the old CLI is gone
     def initialize_old_cli(self):
```

### Comparing `ddev-3.1.0/src/ddev/cli/clean/__init__.py` & `ddev-3.2.1/src/ddev/cli/clean/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 @click.command(short_help="Remove all build artifacts")
 @click.pass_obj
 def clean(app: Application):
     """
     Remove build and test artifacts for the entire repository.
     """
-    with app.repo.path.as_cwd():
+    with app.repo.path.as_cwd(), app.status("Cleaning repository"):
         app.platform.run_command(
             ["git", "clean", "-fdX", "-e", "!.vscode", "-e", "!.idea", "-e", "!ddev/src/ddev/_version.py"]
         )
```

### Comparing `ddev-3.1.0/src/ddev/cli/config/__init__.py` & `ddev-3.2.1/src/ddev/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/env/__init__.py` & `ddev-3.2.1/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/meta/__init__.py` & `ddev-3.2.1/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/meta/scripts/__init__.py` & `ddev-3.2.1/src/ddev/cli/meta/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/meta/scripts/upgrade_python.py` & `ddev-3.2.1/src/ddev/cli/meta/scripts/upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/release/__init__.py` & `ddev-3.2.1/src/ddev/cli/release/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/release/agent/__init__.py` & `ddev-3.2.1/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/release/list_versions/__init__.py` & `ddev-3.2.1/src/ddev/cli/release/list_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/release/show/__init__.py` & `ddev-3.2.1/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/status/__init__.py` & `ddev-3.2.1/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/validate/__init__.py` & `ddev-3.2.1/src/ddev/cli/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/validate/ci.py` & `ddev-3.2.1/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/validate/licenses.py` & `ddev-3.2.1/src/ddev/cli/validate/licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/validate/manifest.py` & `ddev-3.2.1/src/ddev/cli/validate/manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/cli/validate/openmetrics.py` & `ddev-3.2.1/src/ddev/cli/validate/openmetrics.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/config/file.py` & `ddev-3.2.1/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/config/model.py` & `ddev-3.2.1/src/ddev/config/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 FIELD_TO_PARSE = object()
 
 
+def get_github_user():
+    return (
+        os.environ.get('DD_GITHUB_USER', '')
+        or os.environ.get('GITHUB_USER', '')
+        # GitHub Actions
+        or os.environ.get('GITHUB_ACTOR', '')
+    )
+
+
+def get_github_token():
+    return os.environ.get('DD_GITHUB_TOKEN', '') or os.environ.get('GH_TOKEN', '') or os.environ.get('GITHUB_TOKEN', '')
+
+
 class ConfigurationError(Exception):
     def __init__(self, *args, location):
         self.location = location
         super().__init__(*args)
 
     def __str__(self):
         return f'Error parsing config:\n{self.location}\n  {super().__str__()}'
@@ -443,15 +456,15 @@
             if 'user' in self.raw_data:
                 user = self.raw_data['user']
                 if not isinstance(user, str):
                     self.raise_error('must be a string')
 
                 self._field_user = user
             else:
-                self._field_user = self.raw_data['user'] = os.environ.get('DD_GITHUB_USER', '')
+                self._field_user = self.raw_data['user'] = get_github_user()
 
         return self._field_user
 
     @user.setter
     def user(self, value):
         self.raw_data['user'] = value
         self._field_user = FIELD_TO_PARSE
@@ -462,15 +475,15 @@
             if 'token' in self.raw_data:
                 token = self.raw_data['token']
                 if not isinstance(token, str):
                     self.raise_error('must be a string')
 
                 self._field_token = token
             else:
-                self._field_token = self.raw_data['token'] = os.environ.get('DD_GITHUB_TOKEN', '')
+                self._field_token = self.raw_data['token'] = get_github_token()
 
         return self._field_token
 
     @token.setter
     def token(self, value):
         self.raw_data['token'] = value
         self._field_token = FIELD_TO_PARSE
```

### Comparing `ddev-3.1.0/src/ddev/config/utils.py` & `ddev-3.2.1/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/integration/core.py` & `ddev-3.2.1/src/ddev/integration/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,22 @@
             elif self.name == 'datadog_checks_downloader':
                 directory = 'downloader'
             else:
                 directory = self.package_directory_name
 
             return self.path / 'datadog_checks' / directory
 
+    @property
+    def release_tag_pattern(self) -> str:
+        version_part = r'\d+\.\d+\.\d+'
+        if self.name == 'ddev':
+            version_part = f'v{version_part}'
+
+        return f'{self.name}-{version_part}'
+
     @cached_property
     def manifest(self) -> Manifest:
         from ddev.integration.manifest import Manifest
 
         return Manifest(self.path / 'manifest.json')
 
     @cached_property
```

### Comparing `ddev-3.1.0/src/ddev/repo/core.py` & `ddev-3.2.1/src/ddev/repo/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Dict, Iterable
 
 from ddev.integration.core import Integration
-from ddev.repo.constants import CONFIG_DIRECTORY
+from ddev.repo.constants import CONFIG_DIRECTORY, FULL_NAMES
 from ddev.utils.fs import Path
 from ddev.utils.git import GitManager
 
 if TYPE_CHECKING:
     from ddev.repo.config import RepositoryConfig
 
 
 class Repository:
     def __init__(self, name: str, path: str):
         self.__name = name
+        self.__full_name = FULL_NAMES.get(name, name)
         self.__path = Path(path).expand()
         self.__git = GitManager(self.__path)
         self.__integrations = IntegrationRegistry(self)
 
     @property
     def name(self) -> str:
         return self.__name
 
     @property
+    def full_name(self) -> str:
+        return self.__full_name
+
+    @property
     def path(self) -> Path:
         return self.__path
 
     @property
     def git(self) -> GitManager:
         return self.__git
```

### Comparing `ddev-3.1.0/src/ddev/utils/fs.py` & `ddev-3.2.1/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/utils/git.py` & `ddev-3.2.1/src/ddev/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/utils/json.py` & `ddev-3.2.1/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/utils/platform.py` & `ddev-3.2.1/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/utils/structures.py` & `ddev-3.2.1/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/utils/scripts/ci_matrix.py` & `ddev-3.2.1/src/ddev/utils/scripts/ci_matrix.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/src/ddev/validation/tracker.py` & `ddev-3.2.1/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/conftest.py` & `ddev-3.2.1/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from contextlib import ExitStack
 from typing import Generator
 
 import pytest
 import vcr
 from click.testing import CliRunner as __CliRunner
 from datadog_checks.dev.tooling.utils import set_root
+from ddev.cli.terminal import Terminal
 from ddev.config.constants import AppEnvVars, ConfigEnvVars
 from ddev.config.file import ConfigFile
 from ddev.repo.core import Repository
 from ddev.utils.ci import running_in_ci
 from ddev.utils.fs import Path, temp_directory
 from ddev.utils.platform import Platform
 
@@ -67,14 +68,19 @@
 
 @pytest.fixture(scope='session')
 def platform() -> Platform:
     return PLATFORM
 
 
 @pytest.fixture(scope='session')
+def terminal() -> Terminal:
+    return Terminal(verbosity=0, enable_color=False, interactive=False)
+
+
+@pytest.fixture(scope='session')
 def local_repo() -> Path:
     return Path(__file__).resolve().parent.parent.parent
 
 
 @pytest.fixture(scope='session')
 def valid_integrations(local_repo) -> list[str]:
     repo = Repository(local_repo.name, str(local_repo))
```

### Comparing `ddev-3.1.0/tests/test__utils.py` & `ddev-3.2.1/tests/test__utils.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/clean/test_clean.py` & `ddev-3.2.1/tests/cli/clean/test_clean.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/config/test_restore.py` & `ddev-3.2.1/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/config/test_set.py` & `ddev-3.2.1/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/config/test_show.py` & `ddev-3.2.1/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/meta/scripts/test_upgrade_python.py` & `ddev-3.2.1/tests/cli/meta/scripts/test_upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/release/test_list_versions.py` & `ddev-3.2.1/tests/cli/release/test_list_versions.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/status/test_status.py` & `ddev-3.2.1/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/validate/test_licenses.py` & `ddev-3.2.1/tests/cli/validate/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/validate/test_manifest.py` & `ddev-3.2.1/tests/cli/validate/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/cli/validate/test_openmetrics.py` & `ddev-3.2.1/tests/cli/validate/test_openmetrics.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/config/test_model.py` & `ddev-3.2.1/tests/config/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 import pytest
-from ddev.config.model import ConfigurationError, RootConfig
+from ddev.config.model import ConfigurationError, RootConfig, get_github_token, get_github_user
 
 
 def test_default():
     config = RootConfig({})
     config.parse_fields()
 
     assert config.raw_data == {
@@ -31,16 +31,16 @@
                 'app_key': os.getenv('DD_APP_KEY', ''),
                 'site': os.getenv('DD_SITE', 'datadoghq.com'),
                 'dd_url': os.getenv('DD_DD_URL', 'https://app.datadoghq.com'),
                 'log_url': os.getenv('DD_LOGS_CONFIG_DD_URL', ''),
             },
         },
         'github': {
-            'user': os.getenv('DD_GITHUB_USER', ''),
-            'token': os.getenv('DD_GITHUB_TOKEN', ''),
+            'user': get_github_user(),
+            'token': get_github_token(),
         },
         'pypi': {
             'user': '',
             'auth': '',
         },
         'trello': {
             'key': '',
@@ -706,20 +706,20 @@
             _ = config.orgs
 
 
 class TestGitHub:
     def test_default(self):
         config = RootConfig({})
 
-        assert config.github.user == config.github.user == os.getenv('DD_GITHUB_USER', '')
-        assert config.github.token == config.github.token == os.getenv('DD_GITHUB_TOKEN', '')
+        assert config.github.user == config.github.user == get_github_user()
+        assert config.github.token == config.github.token == get_github_token()
         assert config.raw_data == {
             'github': {
-                'user': os.getenv('DD_GITHUB_USER', ''),
-                'token': os.getenv('DD_GITHUB_TOKEN', ''),
+                'user': get_github_user(),
+                'token': get_github_token(),
             },
         }
 
     def test_not_table(self, helpers):
         config = RootConfig({'github': 9000})
 
         with pytest.raises(
```

### Comparing `ddev-3.1.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml` & `ddev-3.2.1/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/fixtures/network/list_versions/success_disk.yaml` & `ddev-3.2.1/tests/fixtures/network/list_versions/success_disk.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/fixtures/network/manifest/missing_app_uuid.yaml` & `ddev-3.2.1/tests/fixtures/network/manifest/missing_app_uuid.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/fixtures/network/manifest/success.yaml` & `ddev-3.2.1/tests/fixtures/network/manifest/success.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/helpers/api.py` & `ddev-3.2.1/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/integration/test_core.py` & `ddev-3.2.1/tests/integration/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,7 +183,21 @@
         assert integration.package_directory == local_repo / integration.name / 'datadog_checks' / 'downloader'
 
     def test_normalization(self, local_repo):
         repo = Repository(local_repo.name, str(local_repo))
         integration = repo.integrations.get('go-metro')
 
         assert integration.package_directory == local_repo / integration.name / 'datadog_checks' / 'go_metro'
+
+
+class TestReleaseTagPattern:
+    def test_shipped(self, local_repo):
+        repo = Repository(local_repo.name, str(local_repo))
+        integration = repo.integrations.get('datadog_checks_base')
+
+        assert integration.release_tag_pattern == r'datadog_checks_base-\d+\.\d+\.\d+'
+
+    def test_ddev(self, local_repo):
+        repo = Repository(local_repo.name, str(local_repo))
+        integration = repo.integrations.get('ddev')
+
+        assert integration.release_tag_pattern == r'ddev-v\d+\.\d+\.\d+'
```

### Comparing `ddev-3.1.0/tests/repo/test_core.py` & `ddev-3.2.1/tests/repo/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/utils/test_fs.py` & `ddev-3.2.1/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/utils/test_git.py` & `ddev-3.2.1/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/utils/test_json.py` & `ddev-3.2.1/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/utils/test_platform.py` & `ddev-3.2.1/tests/utils/test_platform.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/utils/test_structures.py` & `ddev-3.2.1/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/tests/validation/test_tracker.py` & `ddev-3.2.1/tests/validation/test_tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/.gitignore` & `ddev-3.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/README.md` & `ddev-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ddev-3.1.0/pyproject.toml` & `ddev-3.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,32 +22,35 @@
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "datadog-checks-dev[cli]~=21.0",
+    "datadog-checks-dev[cli]~=22.0",
     "hatch>=1.6.3",
     "httpx",
     "jsonpointer",
     "pluggy",
     "rich>=12.5.1",
     "tomli; python_version < '3.11'",
     "tomli-w",
     "tomlkit",
 ]
 dynamic = ["version"]
 
+[project.urls]
+Source = "https://github.com/DataDog/integrations-core"
+
 [project.scripts]
 ddev = "ddev.cli:main"
 ddev-starship = "ddev.plugin.external.starship.prompt:main"
 
-[project.urls]
-Source = "https://github.com/DataDog/integrations-core"
+[project.entry-points.hatch]
+datadog_checks = "ddev.plugin.external.hatch"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 root = ".."
 version_scheme = "python-simplified-semver"
```

### Comparing `ddev-3.1.0/PKG-INFO` & `ddev-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ddev
-Version: 3.1.0
+Version: 3.2.1
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
-Requires-Dist: datadog-checks-dev[cli]~=21.0
+Requires-Dist: datadog-checks-dev[cli]~=22.0
 Requires-Dist: hatch>=1.6.3
 Requires-Dist: httpx
 Requires-Dist: jsonpointer
 Requires-Dist: pluggy
 Requires-Dist: rich>=12.5.1
 Requires-Dist: tomli-w
 Requires-Dist: tomli; python_version < '3.11'
```

