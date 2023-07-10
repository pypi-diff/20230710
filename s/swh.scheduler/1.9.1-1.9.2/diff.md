# Comparing `tmp/swh.scheduler-1.9.1.tar.gz` & `tmp/swh.scheduler-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.scheduler-1.9.1.tar", last modified: Tue Jun 13 11:13:44 2023, max compression
+gzip compressed data, was "swh.scheduler-1.9.2.tar", last modified: Mon Jul 10 15:11:34 2023, max compression
```

## Comparing `swh.scheduler-1.9.1.tar` & `swh.scheduler-1.9.2.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/LICENSE.Celery
--rw-r--r--   0 jenkins    (115) docker     (999)      154 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      664 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      646 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/data/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/data/elastic-template.json
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/data/update-index-settings.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      887 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7923 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3060 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/simulator.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-journal.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-simulator.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      509 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2556 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/sql/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1384 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/sql/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/
--rw-r--r--   0 jenkins    (115) docker     (999)     2105 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      649 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      928 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4203 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    38368 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/backend.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13335 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3320 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/pika_listener.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13193 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/recurrent_visits.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6758 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/runner.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)     2904 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5278 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/add_forge_now.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7130 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4791 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/celery_monitor.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2095 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/journal.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7280 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2552 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/simulator.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12528 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/task.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7044 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/task_type.py
--rw-r--r--   0 jenkins    (115) docker     (999)      584 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10293 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      473 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18240 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12011 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8849 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/model.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     3552 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/
--rw-r--r--   0 jenkins    (115) docker     (999)     5691 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6293 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2331 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/origin_scheduler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7801 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/origins.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/task_scheduler.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    10833 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    14607 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/40-func.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/50-data.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/02.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/03.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/04.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/05.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      625 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/06.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/07.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1924 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/08.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     7034 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/09.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/10.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2070 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/11.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/12.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      967 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/13.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1729 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/14.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1126 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/15.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/16.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      152 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/17.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/18.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      958 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/19.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/20.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/23.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      471 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/24.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/25.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1478 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/26.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/27.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2112 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/28.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1241 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/29.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      224 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/30-bis.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2991 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/30.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      680 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/31.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2182 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/32.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3628 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/33.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1738 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/34.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/task.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3682 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      555 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/data/logging-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2568 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10759 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_celery_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24098 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5595 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_add_forge_now.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4174 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_celery_monitor.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3765 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_journal.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5989 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4018 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_task_type.py
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1952 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3859 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2836 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)    30328 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8555 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_recurrent_visits.py
--rw-r--r--   0 jenkins    (115) docker     (999)    63287 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_scheduler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3532 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1967 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_simulator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5826 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3892 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4229 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      486 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1681 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.768254 swh.scheduler-1.9.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/LICENSE.Celery
+-rw-r--r--   0 jenkins    (115) docker     (999)      154 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-07-10 15:11:34.768254 swh.scheduler-1.9.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      664 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.752254 swh.scheduler-1.9.2/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      646 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/data/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/data/elastic-template.json
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/data/update-index-settings.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      887 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7923 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3060 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/docs/simulator.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/requirements-journal.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/requirements-simulator.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      509 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-10 15:11:34.772254 swh.scheduler-1.9.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2556 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1384 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/sql/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/swh/scheduler/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2105 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/swh/scheduler/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      649 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      928 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4203 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    38368 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/backend.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.760254 swh.scheduler-1.9.2/swh/scheduler/celery_backend/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/celery_backend/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13335 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/celery_backend/config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3320 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/celery_backend/pika_listener.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13254 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/celery_backend/recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6758 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/celery_backend/runner.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.760254 swh.scheduler-1.9.2/swh/scheduler/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2904 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5285 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/add_forge_now.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7130 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4791 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/celery_monitor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2095 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/journal.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7280 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2552 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/simulator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12649 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/task.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7044 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/task_type.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      584 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10293 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      473 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18240 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12011 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8849 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     3552 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.760254 swh.scheduler-1.9.2/swh/scheduler/simulator/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5691 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/simulator/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6293 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/simulator/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2331 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/simulator/origin_scheduler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7801 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/simulator/origins.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/simulator/task_scheduler.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.760254 swh.scheduler-1.9.2/swh/scheduler/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    10833 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    14607 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/40-func.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/50-data.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.764254 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/02.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/03.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/04.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/05.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      625 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/06.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/07.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1924 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/08.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     7034 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/09.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/10.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2070 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/11.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/12.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      967 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/13.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1729 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/14.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1126 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/15.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/16.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      152 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/17.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/18.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      958 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/19.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/20.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/23.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      471 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/24.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/25.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1478 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/26.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/27.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2112 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/28.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1241 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/29.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      224 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/30-bis.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2991 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/30.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      680 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/31.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2182 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/32.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3628 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/33.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1738 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/34.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/task.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.768254 swh.scheduler-1.9.2/swh/scheduler/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3682 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.768254 swh.scheduler-1.9.2/swh/scheduler/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      555 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/data/logging-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2568 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10759 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_celery_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    24098 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5595 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_add_forge_now.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4174 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_celery_monitor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3765 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_journal.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5989 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4018 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_task_type.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1952 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3859 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2836 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    30328 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8555 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    63287 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_scheduler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3532 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1967 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_simulator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5826 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3892 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/swh/scheduler/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-10 15:11:34.756254 swh.scheduler-1.9.2/swh.scheduler.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-07-10 15:11:34.000000 swh.scheduler-1.9.2/swh.scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4229 2023-07-10 15:11:34.000000 swh.scheduler-1.9.2/swh.scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-10 15:11:34.000000 swh.scheduler-1.9.2/swh.scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-07-10 15:11:34.000000 swh.scheduler-1.9.2/swh.scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      486 2023-07-10 15:11:34.000000 swh.scheduler-1.9.2/swh.scheduler.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-10 15:11:34.000000 swh.scheduler-1.9.2/swh.scheduler.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1681 2023-07-10 15:11:29.000000 swh.scheduler-1.9.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.scheduler-1.9.1/.pre-commit-config.yaml` & `swh.scheduler-1.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/CODE_OF_CONDUCT.md` & `swh.scheduler-1.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/LICENSE` & `swh.scheduler-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/LICENSE.Celery` & `swh.scheduler-1.9.2/LICENSE.Celery`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/PKG-INFO` & `swh.scheduler-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 1.9.1
+Version: 1.9.2
 Summary: Software Heritage Scheduler
 Home-page: https://forge.softwareheritage.org/diffusion/DSCH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scheduler
```

### Comparing `swh.scheduler-1.9.1/conftest.py` & `swh.scheduler-1.9.2/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/data/README.md` & `swh.scheduler-1.9.2/data/README.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/data/elastic-template.json` & `swh.scheduler-1.9.2/data/elastic-template.json`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/docs/cli.rst` & `swh.scheduler-1.9.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/docs/index.rst` & `swh.scheduler-1.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/docs/simulator.rst` & `swh.scheduler-1.9.2/docs/simulator.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/mypy.ini` & `swh.scheduler-1.9.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/setup.py` & `swh.scheduler-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/sql/Makefile` & `swh.scheduler-1.9.2/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/__init__.py` & `swh.scheduler-1.9.2/swh/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/api/client.py` & `swh.scheduler-1.9.2/swh/scheduler/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/api/serializers.py` & `swh.scheduler-1.9.2/swh/scheduler/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/api/server.py` & `swh.scheduler-1.9.2/swh/scheduler/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/backend.py` & `swh.scheduler-1.9.2/swh/scheduler/backend.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/celery_backend/config.py` & `swh.scheduler-1.9.2/swh/scheduler/celery_backend/config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/celery_backend/pika_listener.py` & `swh.scheduler-1.9.2/swh/scheduler/celery_backend/pika_listener.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/celery_backend/recurrent_visits.py` & `swh.scheduler-1.9.2/swh/scheduler/celery_backend/recurrent_visits.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     from ..interface import SchedulerInterface
     from ..model import ListedOrigin
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_POLICY = [
-    {"policy": "already_visited_order_by_lag", "weight": 50},
-    {"policy": "never_visited_oldest_update_first", "weight": 50},
+    {"policy": "already_visited_order_by_lag", "weight": 40},
+    {"policy": "never_visited_oldest_update_first", "weight": 40},
+    {"policy": "origins_without_last_update", "weight": 20},
 ]
 DEFAULT_DVCS_POLICY = [
     {"policy": "already_visited_order_by_lag", "weight": 49},
     {"policy": "never_visited_oldest_update_first", "weight": 49},
     {"policy": "origins_without_last_update", "weight": 2},
 ]
 DEFAULT_GIT_POLICY = [
```

### Comparing `swh.scheduler-1.9.1/swh/scheduler/celery_backend/runner.py` & `swh.scheduler-1.9.2/swh/scheduler/celery_backend/runner.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/__init__.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/add_forge_now.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/add_forge_now.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,21 +45,22 @@
     lister_name,
     options,
 ):
     """Register the lister tasks in the scheduler.
 
     The specifics of what tasks are registered depends on the add-forge-now --preset
     option:
+
+    \b
     - staging preset: a single oneshot full listing task is scheduled. This "full"
       listing is limited to 3 pages and 10 origins per page. The origins are recorded as
       disabled (to avoid their recurrent loading).
     - production preset: a recurrent full and incremental (if the loader has such a
       task) listing task are scheduled. The first run of the full lister is scheduled
       immediately, and the first run of the incremental lister is delayed by a day.
-
     """
     from .utils import lister_task_type, parse_options, task_add
 
     scheduler = ctx.obj["scheduler"]
     preset = ctx.obj["preset"]
 
     # Map the associated task types for the lister
```

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/admin.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/admin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/celery_monitor.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/journal.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/journal.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/origin.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/origin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/simulator.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/task.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,37 +48,35 @@
 @click.argument("file", type=click.File(encoding="utf-8"))
 @click.pass_context
 def schedule_tasks(ctx, columns, delimiter, file):
     """Schedule tasks from a CSV input file.
 
     The following columns are expected, and can be set through the -c option:
 
-     - type: the type of the task to be scheduled (mandatory)
-
-     - args: the arguments passed to the task (JSON list, defaults to an empty
-       list)
-
-     - kwargs: the keyword arguments passed to the task (JSON object, defaults
-       to an empty dict)
-
-     - next_run: the date at which the task should run (datetime, defaults to
-       now)
+    \b
+    - type: the type of the task to be scheduled (mandatory)
+    - args: the arguments passed to the task (JSON list, defaults to an empty
+      list)
+    - kwargs: the keyword arguments passed to the task (JSON object, defaults
+      to an empty dict)
+    - next_run: the date at which the task should run (datetime, defaults to
+      now)
 
     The CSV can be read either from a named file, or from stdin (use - as
     filename).
 
-    Use sample:
-
-    cat scheduling-task.txt | \
-        python3 -m swh.scheduler.cli \
-            --database 'service=swh-scheduler-dev' \
-            task schedule \
-                --columns type --columns kwargs --columns policy \
-                --delimiter ';' -
+    Use sample::
 
+        \b
+        cat scheduling-task.txt | \\
+            python3 -m swh.scheduler.cli \\
+                --database 'service=swh-scheduler-dev' \\
+                task schedule \\
+                    --columns type --columns kwargs --columns policy \\
+                    --delimiter ';' -
     """
     import csv
     import json
 
     from swh.scheduler.utils import utcnow
 
     from .utils import pretty_print_task
@@ -124,21 +122,23 @@
 def schedule_task(ctx, task_type_name, options, policy, priority, next_run):
     """Schedule one task from arguments.
 
     The first argument is the name of the task type. Flag options (policy, priority) are
     task configuration. Further options are positional and keyword argument(s) of the
     task, in YAML format. Keyword args are of the form key=value.
 
-    Usage sample:
-
-    swh-scheduler --database 'service=swh-scheduler' \
-        task add list-pypi
+    Usage sample::
 
-    swh-scheduler --database 'service=swh-scheduler' \
-        task add list-debian-distribution --policy=oneshot distribution=stretch
+        \b
+        swh-scheduler --database 'service=swh-scheduler' \\
+            task add list-pypi
+
+        \b
+        swh-scheduler --database 'service=swh-scheduler' \\
+            task add list-debian-distribution --policy=oneshot distribution=stretch
 
     Note: if the priority is not given, the task won't have the priority set,
     which is considered as the lowest priority level.
 
     """
     from .utils import parse_options, task_add
 
@@ -220,18 +220,19 @@
 ):
     """Schedules tasks for origins that are already known.
 
     The first argument is the name of the task type, further ones are
     keyword argument(s) of the task in the form key=value, where value is
     in YAML format.
 
-    Usage sample:
+    Usage sample::
 
-    swh-scheduler --database 'service=swh-scheduler' \
-        task schedule_origins index-origin-metadata
+        \b
+        swh-scheduler --database 'service=swh-scheduler' \\
+            task schedule_origins index-origin-metadata
     """
     from itertools import islice
 
     from swh.storage import get_storage
 
     from .utils import parse_options, schedule_origin_batches
 
@@ -436,17 +437,18 @@
 @click.pass_context
 def respawn_tasks(ctx, task_ids: List[str], next_run: datetime.datetime):
     """Respawn tasks.
 
     Respawn tasks given by their ids (see the 'task list' command to
     find task ids) at the given date (immediately by default).
 
-    Eg.
+    For example::
 
-       swh-scheduler task respawn 1 3 12
+        \b
+        swh-scheduler task respawn 1 3 12
     """
     from swh.scheduler.utils import utcnow
 
     scheduler = ctx.obj["scheduler"]
     if next_run is None:
         next_run = utcnow()
     output = []
```

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/task_type.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/task_type.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/test_cli_utils.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/cli/utils.py` & `swh.scheduler-1.9.2/swh/scheduler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/interface.py` & `swh.scheduler-1.9.2/swh/scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/journal_client.py` & `swh.scheduler-1.9.2/swh/scheduler/journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/model.py` & `swh.scheduler-1.9.2/swh/scheduler/model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/pytest_plugin.py` & `swh.scheduler-1.9.2/swh/scheduler/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/simulator/__init__.py` & `swh.scheduler-1.9.2/swh/scheduler/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/simulator/common.py` & `swh.scheduler-1.9.2/swh/scheduler/simulator/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/simulator/origin_scheduler.py` & `swh.scheduler-1.9.2/swh/scheduler/simulator/origin_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/simulator/origins.py` & `swh.scheduler-1.9.2/swh/scheduler/simulator/origins.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/simulator/task_scheduler.py` & `swh.scheduler-1.9.2/swh/scheduler/simulator/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/30-schema.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/40-func.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/40-func.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/50-data.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/50-data.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/60-indexes.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/02.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/02.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/03.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/03.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/04.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/04.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/05.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/05.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/06.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/06.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/07.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/07.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/08.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/08.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/09.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/09.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/10.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/10.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/11.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/11.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/12.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/12.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/13.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/13.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/14.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/14.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/15.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/15.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/16.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/16.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/19.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/19.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/23.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/23.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/25.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/25.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/26.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/26.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/27.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/27.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/28.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/28.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/29.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/29.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/30.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/30.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/31.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/31.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/32.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/32.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/33.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/33.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/34.sql` & `swh.scheduler-1.9.2/swh/scheduler/sql/upgrades/34.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/task.py` & `swh.scheduler-1.9.2/swh/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/common.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/conftest.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/data/logging-config.yaml` & `swh.scheduler-1.9.2/swh/scheduler/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/tasks.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_api_client.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_celery_tasks.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_celery_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_add_forge_now.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_add_forge_now.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_celery_monitor.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_journal.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_journal.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_origin.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_origin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_task_type.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_task_type.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_utils.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_common.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_config.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_init.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_journal_client.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_model.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_recurrent_visits.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_recurrent_visits.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_scheduler.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_server.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_simulator.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/tests/test_utils.py` & `swh.scheduler-1.9.2/swh/scheduler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh/scheduler/utils.py` & `swh.scheduler-1.9.2/swh/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/swh.scheduler.egg-info/PKG-INFO` & `swh.scheduler-1.9.2/swh.scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 1.9.1
+Version: 1.9.2
 Summary: Software Heritage Scheduler
 Home-page: https://forge.softwareheritage.org/diffusion/DSCH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scheduler
```

### Comparing `swh.scheduler-1.9.1/swh.scheduler.egg-info/SOURCES.txt` & `swh.scheduler-1.9.2/swh.scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.1/tox.ini` & `swh.scheduler-1.9.2/tox.ini`

 * *Files identical despite different names*

