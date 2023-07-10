# Comparing `tmp/iceprod-2.6.9.tar.gz` & `tmp/iceprod-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceprod-2.6.9.tar", last modified: Thu Apr 13 21:55:47 2023, max compression
+gzip compressed data, was "iceprod-2.7.0.tar", last modified: Mon Jul 10 16:31:13 2023, max compression
```

## Comparing `iceprod-2.6.9.tar` & `iceprod-2.7.0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.106279 iceprod-2.6.9/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-04-13 21:55:43.000000 iceprod-2.6.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2634 2023-04-13 21:55:47.106279 iceprod-2.6.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-04-13 21:55:43.000000 iceprod-2.6.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.082279 iceprod-2.6.9/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10083 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/basic_submit.py
--rwxr-xr-x   0 root         (0) root         (0)     1331 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_add_site_to_master.py
--rwxr-xr-x   0 root         (0) root         (0)     1408 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_debugger.py
--rwxr-xr-x   0 root         (0) root         (0)     1095 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_gridftp_proxy.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_join_pool.py
--rwxr-xr-x   0 root         (0) root         (0)     3330 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_rest.py
--rwxr-xr-x   0 root         (0) root         (0)     4606 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprod_server.py
--rwxr-xr-x   0 root         (0) root         (0)     7147 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/iceprodsh
--rwxr-xr-x   0 root         (0) root         (0)     3697 2023-04-13 21:55:43.000000 iceprod-2.6.9/bin/loader.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.082279 iceprod-2.6.9/iceprod/
--rw-r--r--   0 root         (0) root         (0)      625 2023-04-13 21:55:44.000000 iceprod-2.6.9/iceprod/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/client_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.086279 iceprod-2.6.9/iceprod/core/
--rw-r--r--   0 root         (0) root         (0)     2295 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/data_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33372 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/dataclasses.py
--rw-r--r--   0 root         (0) root         (0)      591 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)    45616 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/exe.py
--rw-r--r--   0 root         (0) root         (0)     4147 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/exe_helper.py
--rw-r--r--   0 root         (0) root         (0)    18444 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/exe_json.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/file_catalog.py
--rw-r--r--   0 root         (0) root         (0)    15519 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/functions.py
--rw-r--r--   0 root         (0) root         (0)    16121 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/gridftp.py
--rw-r--r--   0 root         (0) root         (0)    21592 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/i3exec.py
--rw-r--r--   0 root         (0) root         (0)     6108 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/jsonUtil.py
--rw-r--r--   0 root         (0) root         (0)     4035 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/logger.py
--rw-r--r--   0 root         (0) root         (0)    20137 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/parser.py
--rw-r--r--   0 root         (0) root         (0)    25463 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/pilot.py
--rw-r--r--   0 root         (0) root         (0)    30084 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/resources.py
--rw-r--r--   0 root         (0) root         (0)     1949 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/serialization.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/core/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/__main__.py
--rw-r--r--   0 root         (0) root         (0)    19448 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/server.py
--rw-r--r--   0 root         (0) root         (0)     6689 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/credentials/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/materialization/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13808 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/materialize.py
--rw-r--r--   0 root         (0) root         (0)    14142 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/server.py
--rw-r--r--   0 root         (0) root         (0)     3247 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/materialization/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.090279 iceprod-2.6.9/iceprod/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/auth.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/base_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.094279 iceprod-2.6.9/iceprod/rest/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6045 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/auth.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/config.py
--rw-r--r--   0 root         (0) root         (0)    12602 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/datasets.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/grids.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/jobs.py
--rw-r--r--   0 root         (0) root         (0)    11679 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/logs.py
--rw-r--r--   0 root         (0) root         (0)     5706 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/pilots.py
--rw-r--r--   0 root         (0) root         (0)     7201 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/task_stats.py
--rw-r--r--   0 root         (0) root         (0)    39436 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/handlers/tasks.py
--rw-r--r--   0 root         (0) root         (0)     5278 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/rest/server.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/roles_groups.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.094279 iceprod-2.6.9/iceprod/server/
--rw-r--r--   0 root         (0) root         (0)     7572 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8125 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/config.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.078279 iceprod-2.6.9/iceprod/server/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.094279 iceprod-2.6.9/iceprod/server/data/etc/
--rw-r--r--   0 root         (0) root         (0)     1272 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/etc/config_defaults.json
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/etc/iceprod_schema.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.098279 iceprod-2.6.9/iceprod/server/data/www/
--rw-r--r--   0 root         (0) root         (0)     8032 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/base.css
--rw-r--r--   0 root         (0) root         (0)    13205 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chart.stackedarea.js
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    26966 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    10751 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)      643 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/documentation.css
--rw-r--r--   0 root         (0) root         (0)     1591 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/documentation.js
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/favicon.png
--rw-r--r--   0 root         (0) root         (0)    13277 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/fetch.js
--rw-r--r--   0 root         (0) root         (0)     1493 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/json-rpc.js
--rw-r--r--   0 root         (0) root         (0)     8775 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/jsonlint.js
--rw-r--r--   0 root         (0) root         (0)    46933 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/jsviews.min.js
--rw-r--r--   0 root         (0) root         (0)     3842 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/logo_155x60.png
--rw-r--r--   0 root         (0) root         (0)    10659 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/rest.js
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/robots.txt
--rw-r--r--   0 root         (0) root         (0)     5218 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/submit.css
--rw-r--r--   0 root         (0) root         (0)    29484 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/submit.js
--rw-r--r--   0 root         (0) root         (0)     7716 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www/util.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.102279 iceprod-2.6.9/iceprod/server/data/www_templates/
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/404.html
--rw-r--r--   0 root         (0) root         (0)     3092 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/base.html
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/dataset_browse.html
--rw-r--r--   0 root         (0) root         (0)     4467 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/dataset_detail.html
--rw-r--r--   0 root         (0) root         (0)     2659 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/groups.html
--rw-r--r--   0 root         (0) root         (0)     2285 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/job_browse.html
--rw-r--r--   0 root         (0) root         (0)     2255 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/job_detail.html
--rw-r--r--   0 root         (0) root         (0)      611 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/login.html
--rw-r--r--   0 root         (0) root         (0)      183 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/logout.html
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/main.html
--rw-r--r--   0 root         (0) root         (0)     6133 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/profile.html
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/site.html
--rw-r--r--   0 root         (0) root         (0)     6626 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/submit.html
--rw-r--r--   0 root         (0) root         (0)     1790 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/task_browse.html
--rw-r--r--   0 root         (0) root         (0)     4893 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/task_detail.html
--rw-r--r--   0 root         (0) root         (0)      360 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/data/www_templates/tasks.html
--rw-r--r--   0 root         (0) root         (0)     4547 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/dataset_prio.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/documentation.py
--rw-r--r--   0 root         (0) root         (0)     3501 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/globus.py
--rw-r--r--   0 root         (0) root         (0)    30282 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/grid.py
--rw-r--r--   0 root         (0) root         (0)     6785 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.102279 iceprod-2.6.9/iceprod/server/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/queue.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/schedule.py
--rw-r--r--   0 root         (0) root         (0)    29105 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/modules/website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.102279 iceprod-2.6.9/iceprod/server/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11131 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/condor.py
--rw-r--r--   0 root         (0) root         (0)    43247 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/condor_direct.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/condor_file_transfer.py
--rw-r--r--   0 root         (0) root         (0)    33448 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/sc_demo.py
--rw-r--r--   0 root         (0) root         (0)    10523 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/supercomp_cedar.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/plugins/supercomp_graham.py
--rw-r--r--   0 root         (0) root         (0)    10174 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/priority.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.106279 iceprod-2.6.9/iceprod/server/scheduled_tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3846 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_completion.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/job_completion.py
--rw-r--r--   0 root         (0) root         (0)     4904 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/job_temp_cleaning.py
--rw-r--r--   0 root         (0) root         (0)     2088 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/log_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     5274 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/non_active_tasks.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_cleanup.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_monitor.py
--rw-r--r--   0 root         (0) root         (0)     5355 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/queue_tasks.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/removed_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/reset_tasks.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/scheduled_tasks/update_task_priority.py
--rw-r--r--   0 root         (0) root         (0)     3638 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/server.py
--rw-r--r--   0 root         (0) root         (0)     8667 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/ssl_cert.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/task_queue.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-04-13 21:55:43.000000 iceprod-2.6.9/iceprod/server/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:55:47.086279 iceprod-2.6.9/iceprod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2634 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4798 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      368 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 21:55:47.000000 iceprod-2.6.9/iceprod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2090 2023-04-13 21:55:47.106279 iceprod-2.6.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-13 21:55:43.000000 iceprod-2.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.980805 iceprod-2.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-07-10 16:31:10.000000 iceprod-2.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-10 16:31:13.980805 iceprod-2.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-07-10 16:31:10.000000 iceprod-2.7.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.944805 iceprod-2.7.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10083 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/basic_submit.py
+-rwxr-xr-x   0 root         (0) root         (0)     1331 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_add_site_to_master.py
+-rwxr-xr-x   0 root         (0) root         (0)     1408 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_debugger.py
+-rwxr-xr-x   0 root         (0) root         (0)     1095 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_gridftp_proxy.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_join_pool.py
+-rwxr-xr-x   0 root         (0) root         (0)     3330 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_rest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4606 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprod_server.py
+-rwxr-xr-x   0 root         (0) root         (0)     7147 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/iceprodsh
+-rwxr-xr-x   0 root         (0) root         (0)     3697 2023-07-10 16:31:10.000000 iceprod-2.7.0/bin/loader.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.948805 iceprod-2.7.0/iceprod/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-10 16:31:11.000000 iceprod-2.7.0/iceprod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/client_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.952805 iceprod-2.7.0/iceprod/core/
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/data_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33372 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)      591 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    45616 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/exe.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/exe_helper.py
+-rw-r--r--   0 root         (0) root         (0)    18581 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/exe_json.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/file_catalog.py
+-rw-r--r--   0 root         (0) root         (0)    15648 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/functions.py
+-rw-r--r--   0 root         (0) root         (0)    16121 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/gridftp.py
+-rw-r--r--   0 root         (0) root         (0)    21592 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/i3exec.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/jsonUtil.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/logger.py
+-rw-r--r--   0 root         (0) root         (0)    20137 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/parser.py
+-rw-r--r--   0 root         (0) root         (0)    25463 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/pilot.py
+-rw-r--r--   0 root         (0) root         (0)    30084 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/serialization.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/core/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    19558 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/server.py
+-rw-r--r--   0 root         (0) root         (0)     6689 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/credentials/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/materialization/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13731 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/materialize.py
+-rw-r--r--   0 root         (0) root         (0)    14142 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/server.py
+-rw-r--r--   0 root         (0) root         (0)     3247 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/materialization/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.956805 iceprod-2.7.0/iceprod/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/base_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.960805 iceprod-2.7.0/iceprod/rest/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/config.py
+-rw-r--r--   0 root         (0) root         (0)    12602 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/datasets.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/grids.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    11679 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/logs.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/pilots.py
+-rw-r--r--   0 root         (0) root         (0)     7201 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/task_stats.py
+-rw-r--r--   0 root         (0) root         (0)    39857 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/handlers/tasks.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/rest/server.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/roles_groups.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.964805 iceprod-2.7.0/iceprod/server/
+-rw-r--r--   0 root         (0) root         (0)     7572 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8125 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/config.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.940805 iceprod-2.7.0/iceprod/server/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.964805 iceprod-2.7.0/iceprod/server/data/etc/
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/etc/config_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/etc/iceprod_schema.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.972805 iceprod-2.7.0/iceprod/server/data/www/
+-rw-r--r--   0 root         (0) root         (0)     8624 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/base.css
+-rw-r--r--   0 root         (0) root         (0)    13205 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chart.stackedarea.js
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      872 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    26966 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)      643 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/documentation.css
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/documentation.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/favicon.png
+-rw-r--r--   0 root         (0) root         (0)    13277 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/fetch.js
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/json-rpc.js
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/jsonlint.js
+-rw-r--r--   0 root         (0) root         (0)    46933 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/jsviews.min.js
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/logo_155x60.png
+-rw-r--r--   0 root         (0) root         (0)    10659 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/rest.js
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/robots.txt
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/submit.css
+-rw-r--r--   0 root         (0) root         (0)    29484 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/submit.js
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www/util.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.976805 iceprod-2.7.0/iceprod/server/data/www_templates/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/404.html
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/dataset_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/dataset_detail.html
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/groups.html
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/job_browse.html
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/job_detail.html
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/login.html
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/logout.html
+-rw-r--r--   0 root         (0) root         (0)      352 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/main.html
+-rw-r--r--   0 root         (0) root         (0)     6133 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/profile.html
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/site.html
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/submit.html
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/task_browse.html
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/task_detail.html
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/data/www_templates/tasks.html
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/dataset_prio.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/documentation.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/globus.py
+-rw-r--r--   0 root         (0) root         (0)    30407 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/grid.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.976805 iceprod-2.7.0/iceprod/server/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/queue.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    30111 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/modules/website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.980805 iceprod-2.7.0/iceprod/server/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11131 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/condor.py
+-rw-r--r--   0 root         (0) root         (0)    47154 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/condor_direct.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/condor_file_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    33448 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/sc_demo.py
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/supercomp_cedar.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/plugins/supercomp_graham.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/priority.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.980805 iceprod-2.7.0/iceprod/server/scheduled_tasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_completion.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/job_completion.py
+-rw-r--r--   0 root         (0) root         (0)     4904 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/job_temp_cleaning.py
+-rw-r--r--   0 root         (0) root         (0)     2088 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/log_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     5274 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/non_active_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_cleanup.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     5355 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/queue_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/removed_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/reset_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/scheduled_tasks/update_task_priority.py
+-rw-r--r--   0 root         (0) root         (0)     3638 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/ssl_cert.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/task_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-10 16:31:10.000000 iceprod-2.7.0/iceprod/server/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 16:31:13.948805 iceprod-2.7.0/iceprod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 16:31:13.000000 iceprod-2.7.0/iceprod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-07-10 16:31:13.980805 iceprod-2.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-10 16:31:10.000000 iceprod-2.7.0/setup.py
```

### Comparing `iceprod-2.6.9/LICENSE` & `iceprod-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/PKG-INFO` & `iceprod-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.6.9
+Version: 2.7.0
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.6.9/README.rst` & `iceprod-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/basic_submit.py` & `iceprod-2.7.0/bin/basic_submit.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprod_add_site_to_master.py` & `iceprod-2.7.0/bin/iceprod_add_site_to_master.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprod_debugger.py` & `iceprod-2.7.0/bin/iceprod_debugger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprod_gridftp_proxy.py` & `iceprod-2.7.0/bin/iceprod_gridftp_proxy.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprod_join_pool.py` & `iceprod-2.7.0/bin/iceprod_join_pool.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprod_rest.py` & `iceprod-2.7.0/bin/iceprod_rest.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprod_server.py` & `iceprod-2.7.0/bin/iceprod_server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/iceprodsh` & `iceprod-2.7.0/bin/iceprodsh`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/bin/loader.sh` & `iceprod-2.7.0/bin/loader.sh`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/__init__.py` & `iceprod-2.7.0/iceprod/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.6.9"
+__version__ = "2.7.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `iceprod-2.6.9/iceprod/client_auth.py` & `iceprod-2.7.0/iceprod/client_auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/__init__.py` & `iceprod-2.7.0/iceprod/core/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/data_transfer.py` & `iceprod-2.7.0/iceprod/core/data_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/dataclasses.py` & `iceprod-2.7.0/iceprod/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/defaults.py` & `iceprod-2.7.0/iceprod/core/defaults.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/exe.py` & `iceprod-2.7.0/iceprod/core/exe.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/exe_helper.py` & `iceprod-2.7.0/iceprod/core/exe_helper.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/exe_json.py` & `iceprod-2.7.0/iceprod/core/exe_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,26 +203,27 @@
         """
         ret = await self.rest.request('GET', '/tasks/{}'.format(task_id))
         if (not ret) or 'status' not in ret or ret['status'] != 'processing':
             raise Exception('task should be stopped')
 
     async def task_error(self, task_id, dataset_id=None, stats={},
                          start_time=None, reason=None, resources=None,
-                         site=None):
+                         site=None, failed=False):
         """
         Tell the server about the error experienced
 
         Args:
             task_id (str): task_id of task
             dataset_id (str): (optional) dataset_id of task
             stats (dict): (optional) task statistics
             start_time (float): (optional) task start time in unix seconds
             reason (str): (optional) one-line summary of error
             resources (dict): (optional) task resource usage
             site (str): (optional) site the task is running at
+            failed (bool): (optional) instead of resetting the task, just fail
         """
         iceprod_stats = {}
         try:
             hostname = functions.gethostname()
             domain = '.'.join(hostname.split('.')[-2:])
             if start_time:
                 t = time.time() - start_time
@@ -259,15 +260,16 @@
             data['time_used'] = t
         if resources:
             data['resources'] = resources
         if site:
             data['site'] = site
         if reason:
             data['reason'] = reason
-        await self.rest.request('POST', '/tasks/{}/task_actions/reset'.format(task_id), data)
+        status = 'failed' if failed else 'reset'
+        await self.rest.request('POST', f'/tasks/{task_id}/task_actions/{status}', data)
 
     async def task_kill(self, task_id, dataset_id=None, resources=None,
                         reason=None, message=None, site=None):
         """
         Tell the server that we killed a task.
 
         Args:
```

### Comparing `iceprod-2.6.9/iceprod/core/file_catalog.py` & `iceprod-2.7.0/iceprod/core/file_catalog.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/functions.py` & `iceprod-2.7.0/iceprod/core/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,24 +266,19 @@
     except Exception:
         return socket.gethostbyname(socket.getfqdn())
 
 
 def gethostname():
     """Get hostname of this computer."""
     ret = socket.getfqdn()
-    try:
-        resp = requests.get('http://simprod.icecube.wisc.edu/downloads/getip.php', timeout=1)
-        resp.raise_for_status()
-        logging.info('getip: %r', resp.text)
-        ret2 = resp.text.split(' ')[-1]
-        if len(ret2.split('.')) > 1:
-            ret = '.'.join(ret.split('.')[:1]+ret2.split('.')[1:])
-    except Exception:
-        logging.info('error getting global ip', exc_info=True)
-    return ret
+    ret2 = socket.gethostname()
+    if len(ret2) > len(ret):
+        return ret2
+    else:
+        return ret
 
 
 @contextmanager
 def _http_helper(options={}, sync=True):
     """Set up an http session using requests"""
     if sync:
         session = Session
@@ -399,32 +394,41 @@
         # http_proxy fix
         for k in os.environ:
             if k.lower() == 'http_proxy' and not os.environ[k].startswith('http'):
                 os.environ[k] = 'http://'+os.environ[k]
 
         def _d():
             with _http_helper(options) as s:
-                with open(local, 'rb') as f:
-                    m = MultipartEncoder(
-                        fields={'field0': ('filename', f, 'text/plain')}
-                    )
-                    r = s.post(url, timeout=300, data=m,
-                               headers={'Content-Type': m.content_type})
+                try:
+                    with open(local, 'rb') as f:
+                        r = s.put(url, timeout=300, data=f)
                     r.raise_for_status()
-                    if checksum:  # get checksum
-                        r = s.get(url, stream=True, timeout=300)
-                        try:
-                            with open(local+'.tmp', 'wb') as f:
-                                for chunk in r.iter_content(65536):
-                                    f.write(chunk)
+                except requests.exceptions.HTTPError as e:
+                    if e.response.status_code != 405:
+                        raise
+                    else:
+                        logging.warning('WebDav PUT not allowed, trying multipart upload')
+                        with open(local, 'rb') as f:
+                            m = MultipartEncoder(
+                                fields={'field0': ('filename', f, 'text/plain')}
+                            )
+                            r = s.post(url, timeout=300, data=m,
+                                       headers={'Content-Type': m.content_type})
                             r.raise_for_status()
-                            if sha512sum(local+'.tmp') != chksum:
-                                raise Exception('http checksum error')
-                        finally:
-                            removedirs(local+'.tmp')
+                if checksum:  # get checksum
+                    r = s.get(url, stream=True, timeout=300)
+                    try:
+                        with open(local+'.tmp', 'wb') as f:
+                            for chunk in r.iter_content(65536):
+                                f.write(chunk)
+                        r.raise_for_status()
+                        if sha512sum(local+'.tmp') != chksum:
+                            raise Exception('http checksum error')
+                    finally:
+                        removedirs(local+'.tmp')
         await asyncio.get_event_loop().run_in_executor(None, _d)
     elif url.startswith('file:'):
         # use copy command
         url = url[5:]
 
         def _c():
             if os.path.exists(url):
```

### Comparing `iceprod-2.6.9/iceprod/core/gridftp.py` & `iceprod-2.7.0/iceprod/core/gridftp.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/i3exec.py` & `iceprod-2.7.0/iceprod/core/i3exec.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/jsonUtil.py` & `iceprod-2.7.0/iceprod/core/jsonUtil.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/logger.py` & `iceprod-2.7.0/iceprod/core/logger.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/parser.py` & `iceprod-2.7.0/iceprod/core/parser.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/pilot.py` & `iceprod-2.7.0/iceprod/core/pilot.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/resources.py` & `iceprod-2.7.0/iceprod/core/resources.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/serialization.py` & `iceprod-2.7.0/iceprod/core/serialization.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/core/util.py` & `iceprod-2.7.0/iceprod/core/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/credentials/__main__.py` & `iceprod-2.7.0/iceprod/credentials/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/credentials/server.py` & `iceprod-2.7.0/iceprod/credentials/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,21 +146,24 @@
             filters['type'] = 'oauth'
             await db.update_many(filters, {'$set': update_data})
 
         ret = {}
         async for row in db.find(base_data, projection={'_id': False}):
             ret[row['url']] = row
 
-        for key in ret:
+        for key in list(ret):
             cred = ret[key]
             if refresh and is_expired(cred) and cred['refresh_token']:
-                new_cred = await self.refresh_service.refresh_cred(cred)
-                filters = base_data.copy()
-                filters['url'] = key
-                ret[key] = await db.find_one_and_update(filters, {'$set': new_cred}, projection={'_id': False})
+                try:
+                    new_cred = await self.refresh_service.refresh_cred(cred)
+                    filters = base_data.copy()
+                    filters['url'] = key
+                    ret[key] = await db.find_one_and_update(filters, {'$set': new_cred}, projection={'_id': False})
+                except Exception:
+                    del ret[key]
 
         return ret
 
 
 class GroupCredentialsHandler(BaseCredentialsHandler):
     """
     Handle group credentials requests.
```

### Comparing `iceprod-2.6.9/iceprod/credentials/service.py` & `iceprod-2.7.0/iceprod/credentials/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         }
         if len(self.clients[openid_url]) > 1:
             args['client_secret'] = self.clients[openid_url][1]
 
         new_cred = {}
         try:
             async with httpx.AsyncClient() as client:
-                r = await client.post(auth.token_url, json=args)
+                r = await client.post(auth.token_url, data=args)
             r.raise_for_status()
             req = r.json()
         except httpx.HTTPError as exc:
             logger.debug('%r', exc.response.text)
             try:
                 req = exc.response.json()
             except Exception:
```

### Comparing `iceprod-2.6.9/iceprod/materialization/__main__.py` & `iceprod-2.7.0/iceprod/materialization/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/materialization/materialize.py` & `iceprod-2.7.0/iceprod/materialization/materialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,16 +257,14 @@
     parser.add_argument('--set_status', default=None,help='initial task status')
     parser.add_argument('-n','--num', default=100,type=int,help='number of jobs to materialize')
     parser.add_argument('--job_index', type=int, help='specific job index to buffer')
     parser.add_argument('--job_id', default=None, help='specific job id to buffer tasks into')
     parser.add_argument('--debug',action='store_true')
     parser.add_argument('--dryrun',action='store_true',help='do not modify database, just log changes')
     args = parser.parse_args()
-    if not args.rest_token:
-        raise Exception('no token for rest api')
     logging.basicConfig(level=(logging.DEBUG if args.debug else logging.INFO))
 
     rest_client = create_rest_client(args)
     materialize = Materialize(rest_client)
     if args.job_index is not None:
         logging.warning('manually buffering a job for dataset %s job %d', args.dataset_id, args.job_index)
```

### Comparing `iceprod-2.6.9/iceprod/materialization/server.py` & `iceprod-2.7.0/iceprod/materialization/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/materialization/service.py` & `iceprod-2.7.0/iceprod/materialization/service.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/__main__.py` & `iceprod-2.7.0/iceprod/rest/__main__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/auth.py` & `iceprod-2.7.0/iceprod/rest/auth.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/base_handler.py` & `iceprod-2.7.0/iceprod/rest/base_handler.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/auth.py` & `iceprod-2.7.0/iceprod/rest/handlers/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         dict: routes, database, indexes
     """
     return {
         'routes': [
             ('/roles', MultiRoleHandler, handler_cfg),
             ('/groups', MultiGroupHandler, handler_cfg),
             ('/users', MultiUserHandler, handler_cfg),
-            (r'/users/(?P<username>\w+)', UserHandler, handler_cfg),
-            (r'/users/(?P<username>\w+)/priority', UserPriorityHandler, handler_cfg),
+            (r'/users/(?P<username>[^\/\?\#]+)', UserHandler, handler_cfg),
+            (r'/users/(?P<username>[^\/\?\#]+)/priority', UserPriorityHandler, handler_cfg),
             ('/auths', AuthHandler, handler_cfg),
         ],
         'database': 'auth',
         'indexes': {
             'users': {
                 'username_index': {'keys': 'username', 'unique': True},
             },
```

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/config.py` & `iceprod-2.7.0/iceprod/rest/handlers/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/datasets.py` & `iceprod-2.7.0/iceprod/rest/handlers/datasets.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/grids.py` & `iceprod-2.7.0/iceprod/rest/handlers/grids.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/jobs.py` & `iceprod-2.7.0/iceprod/rest/handlers/jobs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/logs.py` & `iceprod-2.7.0/iceprod/rest/handlers/logs.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/pilots.py` & `iceprod-2.7.0/iceprod/rest/handlers/pilots.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/task_stats.py` & `iceprod-2.7.0/iceprod/rest/handlers/task_stats.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/rest/handlers/tasks.py` & `iceprod-2.7.0/iceprod/rest/handlers/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,24 @@
             (r'/tasks/(?P<task_id>\w+)', TasksHandler, handler_cfg),
             (r'/tasks/(?P<task_id>\w+)/status', TasksStatusHandler, handler_cfg),
             (r'/task_actions/queue', TasksActionsQueueHandler, handler_cfg),
             (r'/task_actions/bulk_status/(?P<status>\w+)', TaskBulkStatusHandler, handler_cfg),
             (r'/task_actions/process', TasksActionsProcessingHandler, handler_cfg),
             (r'/task_counts/status', TaskCountsStatusHandler, handler_cfg),
             (r'/tasks/(?P<task_id>\w+)/task_actions/reset', TasksActionsErrorHandler, handler_cfg),
+            (r'/tasks/(?P<task_id>\w+)/task_actions/failed', TasksActionsFailedHandler, handler_cfg),
             (r'/tasks/(?P<task_id>\w+)/task_actions/complete', TasksActionsCompleteHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/tasks', DatasetMultiTasksHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/tasks/(?P<task_id>\w+)', DatasetTasksHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/tasks/(?P<task_id>\w+)/status', DatasetTasksStatusHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/task_summaries/status', DatasetTaskSummaryStatusHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/task_counts/status', DatasetTaskCountsStatusHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/task_counts/name_status', DatasetTaskCountsNameStatusHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/task_actions/bulk_status/(?P<status>\w+)', DatasetTaskBulkStatusHandler, handler_cfg),
-            (r'/datasets/(?P<dataset_id>\w+)/task_actions/bulk_requirements/(?P<name>\w+)', DatasetTaskBulkRequirementsHandler, handler_cfg),
+            (r'/datasets/(?P<dataset_id>\w+)/task_actions/bulk_requirements/(?P<name>[^\/\?\#]+)', DatasetTaskBulkRequirementsHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/task_stats', DatasetTaskStatsHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/files', DatasetMultiFilesHandler, handler_cfg),
             (r'/datasets/(?P<dataset_id>\w+)/files/(?P<task_id>\w+)', DatasetTaskFilesHandler, handler_cfg),
         ],
         'database': 'tasks',
         'indexes': {
             'tasks': {
@@ -650,14 +651,16 @@
             self.finish()
 
 
 class TasksActionsErrorHandler(APIBase):
     """
     Handle task action on error (* -> reset).
     """
+    final_status = 'reset'
+
     @authorization(roles=['admin', 'system'])
     async def post(self, task_id):
         """
         Take one task, set its status to reset.
 
         Args:
             task_id (str): task id
@@ -670,15 +673,15 @@
 
         Returns:
             dict: {}  empty dict
         """
         filter_query = {'task_id': task_id, 'status': {'$ne': 'complete'}}
         update_query = defaultdict(dict,{
             '$set': {
-                'status': 'reset',
+                'status': self.final_status,
                 'status_changed': nowstr(),
             },
             '$inc': {
                 'failures': 1,
             },
         })
         if self.request.body:
@@ -697,14 +700,17 @@
                         old_val = task['requirements'][k] if k in task['requirements'] else Resources.defaults[k]
                         if k == 'cpu':  # special handling for cpu
                             if new_val <= 1.1 or new_val > 20:
                                 continue
                             if new_val < old_val*1.1:
                                 continue
                             new_val = old_val+1  # increase linearly
+                        elif new_val < 0.5:
+                            logger.info('ignoring val below 0.5 for %s: %f', k, new_val)
+                            continue
                         else:
                             new_val *= 1.5  # increase new request by 1.5
                         if isinstance(Resources.defaults[k], (int, list)):
                             new_val = math.ceil(new_val)
                     except Exception:
                         logger.info('error converting requirement %r',
                                     data['resources'][k], exc_info=True)
@@ -728,28 +734,32 @@
                     ('pilot SIGTERM', 'sigterm'),
                     ('killed', 'killed'),
                 ]
                 for text,r in reasons:
                     if text in data['reason']:
                         reason = r
                         break
-                self.statsd.incr('site.{}.task_reset.{}'.format(site, reason))
+                self.statsd.incr('site.{}.task_{}.{}'.format(site, self.final_status, reason))
         ret = await self.db.tasks.find_one_and_update(
             filter_query,
             update_query,
             projection={'_id':False}
         )
         if not ret:
             logger.info('filter_query: %r', filter_query)
             self.send_error(400, reason="Task not found")
         else:
             self.write(ret)
             self.finish()
 
 
+class TasksActionsFailedHandler(TasksActionsErrorHandler):
+    final_status = 'failed'
+
+
 class TasksActionsCompleteHandler(APIBase):
     """
     Handle task action on processing -> complete.
     """
     @authorization(roles=['admin', 'system'])
     async def post(self, task_id):
         """
@@ -930,15 +940,15 @@
             reqs['requirements.'+key] = val
 
         query = {
             'dataset_id': dataset_id,
             'name': name,
         }
         ret = await self.db.tasks.update_many(query, {'$max':reqs})
-        if (not ret) or ret.modified_count < 1:
+        if (not ret) or ret.matched_count < 1:
             self.send_error(404, reason="Tasks not found")
         else:
             self.write({})
             self.finish()
 
 
 class DatasetMultiFilesHandler(APIBase):
```

### Comparing `iceprod-2.6.9/iceprod/rest/server.py` & `iceprod-2.7.0/iceprod/rest/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/s3.py` & `iceprod-2.7.0/iceprod/s3.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/__init__.py` & `iceprod-2.7.0/iceprod/server/__init__.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/config.py` & `iceprod-2.7.0/iceprod/server/config.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/daemon.py` & `iceprod-2.7.0/iceprod/server/daemon.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/etc/config_defaults.json` & `iceprod-2.7.0/iceprod/server/data/etc/config_defaults.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/etc/iceprod_schema.json` & `iceprod-2.7.0/iceprod/server/data/etc/iceprod_schema.json`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/base.css` & `iceprod-2.7.0/iceprod/server/data/www/base.css`

 * *Files 8% similar despite different names*

```diff
@@ -295,32 +295,55 @@
 
 .dataset .settings {
     margin-left: .3em;
     margin-bottom: .5em;
     font-size: 1.05em;
 }
 .dataset .browse .entry {
-    margin: .5em;
+    margin: 1em 0;
 }
 .dataset .browse .entry .header {
     background-color: #e5e5e2;
     padding: .2em;
-    text-align:center;
+    margin-bottom: .2em;
+    text-align: center;
     font-family: sans-serif;
-}
-.dataset .browse .entry .id {
-    float:left;
+    display: flex;
+    flex-wrap: wrap;
+    justify-content: space-between;
+    gap: .2em 2em;
+}
+.dataset .browse .entry .header > div {
+    min-width: 8em;
+}
+.dataset .browse .entry .header > div:first-child {
+    text-align: left;
+}
+.dataset .browse .entry .header > div:last-child {
+    text-align: right;
+}
+.dataset .browse .entry .user-group > span {
+    min-width: 8em;
+    display: inline-block;
+}
+.dataset .browse .entry .user-group > span.username {
+    text-align: right;
+}
+.dataset .browse .entry .user-group > span.group {
+    text-align: left;
+}
+@media screen and (max-width: 900px) {
+    .dataset .browse .entry .user-group {
+        order: 10;
+        width: 100%;
+    }
 }
 .dataset .browse .entry .status {
-    float:right;
     text-transform: uppercase;
 }
-.dataset .browse .entry>span {
-    margin: .1em .5em;
-}
 .filters select {
     width: 9.5em;
 }
 
 table.key_value td {
     margin-top: .2em;
     border: 0;
```

### Comparing `iceprod-2.6.9/iceprod/server/data/www/chart.stackedarea.js` & `iceprod-2.7.0/iceprod/server/data/www/chart.stackedarea.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/chosen-sprite.png` & `iceprod-2.7.0/iceprod/server/data/www/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/chosen-sprite@2x.png` & `iceprod-2.7.0/iceprod/server/data/www/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/chosen.jquery.min.js` & `iceprod-2.7.0/iceprod/server/data/www/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/chosen.min.css` & `iceprod-2.7.0/iceprod/server/data/www/chosen.min.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/documentation.css` & `iceprod-2.7.0/iceprod/server/data/www/documentation.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/documentation.js` & `iceprod-2.7.0/iceprod/server/data/www/documentation.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/favicon.ico` & `iceprod-2.7.0/iceprod/server/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/fetch.js` & `iceprod-2.7.0/iceprod/server/data/www/fetch.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/json-rpc.js` & `iceprod-2.7.0/iceprod/server/data/www/json-rpc.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/jsonlint.js` & `iceprod-2.7.0/iceprod/server/data/www/jsonlint.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/jsviews.min.js` & `iceprod-2.7.0/iceprod/server/data/www/jsviews.min.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/logo_155x60.png` & `iceprod-2.7.0/iceprod/server/data/www/logo_155x60.png`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/rest.js` & `iceprod-2.7.0/iceprod/server/data/www/rest.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/submit.css` & `iceprod-2.7.0/iceprod/server/data/www/submit.css`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/submit.js` & `iceprod-2.7.0/iceprod/server/data/www/submit.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www/util.js` & `iceprod-2.7.0/iceprod/server/data/www/util.js`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/base.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
                 <li{% if section == 'util' %} class="current"{% end %}><a href="/help">Help</a></li>
                 {% if (not master) and master_url %}<li class="master"><a href="{{ master_url }}">Master</a></li>{% end %}
                 -->
                 {% if current_user %}
                   <li{% if section == 'profile' %} class="current"{% end %}><a href="/profile">Profile</a></li>
                 {% end %}
                 <li>
-                    {% if (not current_user) %} <a href='/login'>Login </a>
-                    {% else %} <a href='/logout'>Logout </a> 
+                    {% if (not current_user) %} <a href='/login?next={{ url_escape(request.uri) }}'>Login</a>
+                    {% else %} <a href='/logout'>Logout</a>
                     {% end %}
                 </li>
                 </ul>
             </nav>
         </header>
         <div class="body {{ section.lower().replace(' ','_') }}">
             <div class="sidebar">{% block sidebar %}{% end %}</div>
```

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/dataset_browse.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/dataset_browse.html`

 * *Files 11% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 {% end %}
 
 {% block body %}
 <div class="browse">
     {% for dataset in datasets %}
     <div class="entry">
         <div class="header">
-            <span class="id"><a href="/dataset/{{ dataset['dataset_id'] }}">{{ dataset['dataset'] }}</a></span>
-            <span class="status">{{ dataset['status'] }}</span>
-            <div style="clear:right"></div>
+            <div class="id"><a href="/dataset/{{ dataset['dataset_id'] }}">{{ dataset['dataset'] }}</a></div>
+            <div class="user-group"><span class="username">{{ dataset['username'] }}</span> <span class="group">({{ dataset['group'] }})</span></div>
+            <div class="status">{{ dataset['status'] }}</div>
         </div>
-        <span class="description">{{ dataset['description'] }}</span>
+        <div class="description">{{ dataset['description'] }}</div>
     </div>
     {% end %}
 </div>
 {% end %}
```

#### html2text {}

```diff
@@ -6,11 +6,13 @@
 {% for option in filter_options[f] %}
 % if option in filter_results[f] %} selected{% end %}>{{ option }}
 {% end %}
  {% end %} Update
 *** Submit_Dataset ***
 {% end %} {% block body %}
 {% for dataset in datasets %}
-{{_dataset['dataset']_}} {{ dataset['status'] }}
+{{_dataset['dataset']_}}
+{{ dataset['username'] }} ({{ dataset['group'] }})
+{{ dataset['status'] }}
 {{ dataset['description'] }}
 {% end %}
 {% end %}
```

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/dataset_detail.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/dataset_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/groups.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/groups.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/job_browse.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/job_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/job_detail.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/job_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/login.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/login.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/profile.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/profile.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/site.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/site.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/submit.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/submit.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/task_browse.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/task_browse.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/data/www_templates/task_detail.html` & `iceprod-2.7.0/iceprod/server/data/www_templates/task_detail.html`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/dataset_prio.py` & `iceprod-2.7.0/iceprod/server/dataset_prio.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/documentation.py` & `iceprod-2.7.0/iceprod/server/documentation.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/globus.py` & `iceprod-2.7.0/iceprod/server/globus.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/grid.py` & `iceprod-2.7.0/iceprod/server/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         return get_host.history[1]
     host = socket.getfqdn()
     get_host.history = [t, host]
     return host
 get_host.history = None  # noqa: E305
 
 
+CRED_SUBMIT_DIR = 'iceprod_credentials'
+
+
 class BaseGrid(object):
     """
     Interface for a generic job distribution system.
     Do not use this class directly.  Use one of the plugins.
     """
 
     # use only these grid states when defining grid status
@@ -510,19 +513,20 @@
             for tray in task_cfg['trays']:
                 get_creds(tray)
                 for module in tray['modules']:
                     get_creds(module)
 
             file_creds = {}
             for url in cred_keys:
-                f = os.path.join(self.credentials_dir, hashlib.sha1(oauth_creds[url]['access_token'].encode('utf-8')).hexdigest())
-                if not os.path.exists(f):
-                    with open(f, 'w') as f:
+                cred_name = hashlib.sha1(oauth_creds[url]['access_token'].encode('utf-8')).hexdigest()
+                path = os.path.join(self.credentials_dir, cred_name)
+                if not os.path.exists(path):
+                    with open(path, 'w') as f:
                         f.write(oauth_creds[url]['access_token'])
-                file_creds[url] = f
+                file_creds[url] = cred_name
             job_cfg['options']['credentials'] = file_creds
 
     async def setup_submit_directory(self,task):
         """Set up submit directory"""
         # create directory for task
         submit_dir = self.submit_dir
         task_dir = os.path.join(submit_dir,task['task_id']+'_'+str(random.randint(0,1000000)))
@@ -603,20 +607,21 @@
     def write_cfg(self, task):
         """Write the config file for a task-like object"""
         filename = os.path.join(task['submit_dir'],'task.cfg')
         filelist = [filename]
 
         config = self.create_config(task)
         if creds := config['options'].get('credentials', {}):
-            cred_dir = os.path.join(task['submit_dir'], 'iceprod_credentials')
+            cred_dir = os.path.join(task['submit_dir'], CRED_SUBMIT_DIR)
             os.mkdir(cred_dir)
-            for src in creds.values():
-                dest = os.path.join(cred_dir, os.path.basename(src))
+            for name in creds.values():
+                src = os.path.join(self.credentials_dir, name)
+                dest = os.path.join(cred_dir, name)
                 os.symlink(src, dest)
-            filelist.append('iceprod_credentials')
+            filelist.append(cred_dir)
         if 'system' in self.cfg and 'remote_cacert' in self.cfg['system']:
             config['options']['ssl'] = {}
             config['options']['ssl']['cacert'] = os.path.basename(self.cfg['system']['remote_cacert'])
             src = self.cfg['system']['remote_cacert']
             dest = os.path.join(task['submit_dir'],config['options']['ssl']['cacert'])
             try:
                 os.symlink(src,dest)
```

### Comparing `iceprod-2.6.9/iceprod/server/module.py` & `iceprod-2.7.0/iceprod/server/module.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/modules/queue.py` & `iceprod-2.7.0/iceprod/server/modules/queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/modules/schedule.py` & `iceprod-2.7.0/iceprod/server/modules/schedule.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/modules/website.py` & `iceprod-2.7.0/iceprod/server/modules/website.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import functools
 from urllib.parse import urlencode
 import re
 from datetime import datetime, timedelta
 
 from iceprod.core.jsonUtil import json_encode
 
+from cachetools.func import ttl_cache
 import tornado.web
 import tornado.httpserver
 import tornado.gen
 import jwt
 import tornado.concurrent
 from rest_tools.client import RestClient
 from rest_tools.server import catch_error, RestServer, RestHandlerSetup, RestHandler, OpenIDLoginHandler
@@ -136,14 +137,15 @@
                 login_handler_args['oauth_client_scope'] = 'offline_access posix profile'
 
             handler_args.update({
                 'cfg': self.cfg,
                 'modules': self.modules,
                 'statsd': self.statsd,
                 'rest_api': rest_address,
+                'system_rest_client': self.rest_client,
             })
             if 'debug' in self.cfg['webserver'] and self.cfg['webserver']['debug']:
                 handler_args['debug'] = True
             if 'cookie_secret' in self.cfg['webserver']:
                 cookie_secret = self.cfg['webserver']['cookie_secret']
                 logger.info('using supplied cookie secret %r', cookie_secret)
             else:
@@ -339,29 +341,30 @@
         super().initialize(**kwargs)
         self.cred_rest_client = cred_rest_client
         self.full_url = full_url
 
 
 class PublicHandler(TokenStorageMixin, RestHandler):
     """Default Handler"""
-    def initialize(self, cfg=None, modules=None, statsd=None, rest_api=None, cred_rest_client=None, full_url=None, **kwargs):
+    def initialize(self, cfg=None, modules=None, statsd=None, rest_api=None, cred_rest_client=None, system_rest_client=None, full_url=None, **kwargs):
         """
         Get some params from the website module
 
         :param cfg: the global config
         :param modules: modules handle
         :param statsd: statsd client
         :param rest_api: the rest api url
         """
         super().initialize(**kwargs)
         self.cfg = cfg
         self.modules = modules
         self.statsd = statsd
         self.rest_api = rest_api
         self.cred_rest_client = cred_rest_client
+        self.system_rest_client = system_rest_client
         self.rest_client = None
         self.full_url = full_url
 
     def get_template_namespace(self):
         namespace = super().get_template_namespace()
         namespace['version'] = iceprod.__version__
         namespace['section'] = self.request.uri.lstrip('/').split('?')[0].split('/')[0]
@@ -406,14 +409,16 @@
         self.finish()
 
 
 class Default(PublicHandler):
     """Handle / urls"""
     @catch_error
     async def get(self):
+        # try to get the user, if available
+        await self.get_current_user_async()
         self.statsd.incr('default')
         self.render('main.html')
 
 
 class Submit(PublicHandler):
     """Handle /submit urls"""
     @authenticated
@@ -437,15 +442,15 @@
             'passkey':token,
             'edit':False,
             'dataset_id':'',
             'config':default_config,
             'groups':groups,
             'description':'',
         }
-        self.render('submit.html',**render_args)
+        self.render('submit.html', **render_args)
 
 
 class Config(PublicHandler):
     """Handle /config urls"""
     @authenticated
     async def get(self):
         self.statsd.incr('config')
@@ -468,38 +473,51 @@
             'description':dataset.get('description',''),
         }
         self.render('submit.html',**render_args)
 
 
 class DatasetBrowse(PublicHandler):
     """Handle /dataset urls"""
+    @ttl_cache(maxsize=256, ttl=600)
+    async def get_usernames(self):
+        ret = await self.system_rest_client.request('GET', '/users')
+        return [x['username'] for x in ret['results']]
+
     @authenticated
     async def get(self):
         self.statsd.incr('dataset_browse')
-        filter_options = {'status':['processing','suspended','errors','complete','truncated']}
-        filter_results = {n:self.get_arguments(n) for n in filter_options}
+        usernames = await self.get_usernames()
+        filter_options = {
+            'status': ['processing', 'suspended', 'errors', 'complete', 'truncated'],
+            'groups': list(GROUPS.keys()),
+            'users': usernames,
+        }
+        filter_results = {n: self.get_arguments(n) for n in filter_options}
 
-        args = {'keys': 'dataset_id|dataset|status|description'}
+        args = {'keys': 'dataset_id|dataset|status|description|group|username'}
         for name in filter_results:
             val = filter_results[name]
             if not val:
                 continue
             if any(v not in filter_options[name] for v in val):
                 raise tornado.web.HTTPError(400, reason='Bad filter '+name+' value')
             args[name] = '|'.join(val)
 
         url = '/datasets'
 
         ret = await self.rest_client.request('GET', url, args)
         datasets = sorted(ret.values(), key=lambda x:x.get('dataset',0), reverse=True)
         logger.debug('datasets: %r', datasets)
         datasets = filter(lambda x: 'dataset' in x, datasets)
-        self.render('dataset_browse.html',datasets=datasets,
-                    filter_options=filter_options,
-                    filter_results=filter_results)
+        self.render(
+            'dataset_browse.html',
+            datasets=datasets,
+            filter_options=filter_options,
+            filter_results=filter_results,
+        )
 
 
 class Dataset(PublicHandler):
     """Handle /dataset urls"""
     @authenticated
     async def get(self, dataset_id):
         self.statsd.incr('dataset')
@@ -638,14 +656,16 @@
         job['tasks'].sort(key=lambda x:x['task_index'])
         self.render('job_detail.html', dataset=dataset, job=job, passkey=passkey)
 
 
 class Documentation(PublicHandler):
     @catch_error
     async def get(self, url):
+        # try to get the user, if available
+        await self.get_current_user_async()
         self.statsd.incr('documentation')
         doc_path = get_pkgdata_filename('iceprod.server','data/docs')
         full_path = os.path.join(doc_path, url)
         if not full_path.startswith(doc_path):
             self.set_status(404)
             self.render('404.html', path='bad docs path')
             return
@@ -666,22 +686,26 @@
         self.flush()
 
 
 class Help(PublicHandler):
     """Help Page"""
     @catch_error
     async def get(self):
+        # try to get the user, if available
+        await self.get_current_user_async()
         self.statsd.incr('help')
         self.render('help.html')
 
 
 class Other(PublicHandler):
     """Handle any other urls - this is basically all 404"""
     @catch_error
     async def get(self):
+        # try to get the user, if available
+        await self.get_current_user_async()
         self.statsd.incr('other')
         path = self.request.path
         self.set_status(404)
         self.render('404.html', path=path)
 
 
 class Profile(PublicHandler):
@@ -690,17 +714,17 @@
     async def get(self):
         self.statsd.incr('profile')
         username = self.current_user
         groups = self.auth_groups
         group_creds = {}
         for g in groups:
             if g != 'users':
-                ret = await self.rest_client.request('GET', f'/groups/{g}/credentials')
+                ret = await self.cred_rest_client.request('GET', f'/groups/{g}/credentials')
                 group_creds[g] = ret
-        user_creds = await self.rest_client.request('GET', f'/users/{username}/credentials')
+        user_creds = await self.cred_rest_client.request('GET', f'/users/{username}/credentials')
         self.render('profile.html', username=username, groups=groups,
                     group_creds=group_creds, user_creds=user_creds)
 
     @authenticated
     async def post(self):
         username = self.current_user
 
@@ -709,15 +733,15 @@
                 'url': 'https://data.icecube.aq',
                 'type': 'oauth',
                 'access_token': self.auth_access_token,
             }
             if self.auth_refresh_token:
                 args['refresh_token'] = self.auth_refresh_token
                 args['expiration'] = (datetime.utcnow() + timedelta(days=30)).isoformat()
-            await self.rest_client.request('POST', f'/users/{username}/credentials', args)
+            await self.cred_rest_client.request('POST', f'/users/{username}/credentials', args)
 
         else:
             type_ = self.get_argument('type')
             args = {
                 'url': self.get_argument('url'),
                 'type': type_,
             }
@@ -732,25 +756,26 @@
                     args['refresh_token'] = ref
                 if not (acc or ref):
                     raise tornado.web.HTTPError(400, reason='need access or refresh token')
             else:
                 raise tornado.web.HTTPError(400, reason='bad cred type')
 
             if self.get_argument('add_user_cred', ''):
-                await self.rest_client.request('POST', f'/users/{username}/credentials', args)
+                await self.cred_rest_client.request('POST', f'/users/{username}/credentials', args)
             elif self.get_argument('add_group_cred', ''):
                 groupname = self.get_argument('group')
                 if groupname not in self.auth_groups or groupname == 'users':
                     raise tornado.web.HTTPError(400, reason='bad group name')
-                await self.rest_client.request('POST', f'/groups/{groupname}/credentials', args)
+                await self.cred_rest_client.request('POST', f'/groups/{groupname}/credentials', args)
 
         # now show the profile page
         await self.get()
 
 
 class Logout(PublicHandler):
     @catch_error
     async def get(self):
         self.statsd.incr('logout')
         self.clear_tokens()
         self.current_user = None
+        self.request.uri = '/'  # for login redirect, fake the main page
         self.render('logout.html', status=None)
```

### Comparing `iceprod-2.6.9/iceprod/server/plugins/condor.py` & `iceprod-2.7.0/iceprod/server/plugins/condor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/plugins/condor_direct.py` & `iceprod-2.7.0/iceprod/server/plugins/condor_direct.py`

 * *Files 7% similar despite different names*

```diff
@@ -158,36 +158,68 @@
             self.queue_params['requirements.site'] = self.site
         logger.info('resources: %r', self.resources)
         logger.info('queue params: %r', self.queue_params)
 
         self.grid_remove_once = set()
 
     async def upload_logfiles(self, task_id, dataset_id, submit_dir=None, reason=''):
-        """upload logfiles"""
+        """
+        Upload logfiles
+
+        Args:
+            task_id (str): task id
+            dataset_id (str): dataset id
+            submit_dir (str): (optional) submit dir for task
+            reason (str): (optional) reason to inject into stdlog if it does not exist
+
+        Returns:
+            payload_failure (bool): indicate if the task had a payload failure
+        """
         if submit_dir is None:
             submit_dir = ''
 
+        payload_failure = False
+
         data = {'name': 'stdlog', 'task_id': task_id, 'dataset_id': dataset_id}
 
         # upload stdlog
         data['data'] = read_filename(os.path.join(submit_dir, constants['stdlog']))
+        for line in data['data'].split('\n'):
+            if 'task exe' in line and 'return code' in line:
+                return_code = int(line.rsplit(':', 1)[1].strip())
+                if return_code != 0 and return_code != 132:  # ignore SIGILL
+                    payload_failure = True
+                    break
+
         if not data['data']:
             data['data'] = reason
         await self.rest_client.request('POST', '/logs', data)
 
         # upload stderr
         data['name'] = 'stderr'
         data['data'] = read_filename(os.path.join(submit_dir, constants['stderr']))
         await self.rest_client.request('POST', '/logs', data)
+        if payload_failure:
+            for line in data['data'].split('\n'):
+                # find cases where it's probably a node failure
+                if ('No such file or directory' in line
+                        or 'No space left on device' in line
+                        or 'Illegal instruction' in line
+                        or ('Killed' in line and 'env-shell.sh' in line)
+                        or 'py3-v4.1.1/RHEL_8_x86_64/lib/libCore.so.6.18: undefined symbol: usedToIdentifyRootClingByDlSym' in line):
+                    payload_failure = False
+                    break
 
         # upload stdout
         data['name'] = 'stdout'
         data['data'] = read_filename(os.path.join(submit_dir, constants['stdout']))
         await self.rest_client.request('POST', '/logs', data)
 
+        return payload_failure
+
     async def get_hold_reason(self, submit_dir, resources=None):
         """Search for a hold reason in the condor.log"""
         if submit_dir is None:
             submit_dir = ''
         reason = None
         filename = os.path.join(submit_dir, 'condor.log')
         if os.path.exists(filename):
@@ -202,23 +234,27 @@
                             try:
                                 val = float(line.split('used')[-1].split('mb')[0].strip())/1024.
                             except Exception:
                                 try:
                                     val = float(line.split(':')[-1].split('mb')[0].strip())/1024.
                                 except Exception:
                                     pass
+                        elif 'memory usage exceeded' in line:
+                            resource_type = 'memory'
                         elif 'cpu limit' in line or 'cpu consumption limit':
                             resource_type = 'cpu'
                             try:
                                 val = float(line.split('used')[-1].split('cores')[0].strip())
                             except Exception:
                                 try:
                                     val = float(line.split('used')[-1].split('usr')[0].strip())
                                 except Exception:
                                     pass
+                        elif 'cpu usage exceeded' in line:
+                            resource_type = 'cpu'
                         elif 'execution time limit' in line:
                             resource_type = 'time'
                             try:
                                 val = float(line.split('used')[-1].split('.')[0].strip())/3600.
                             except Exception:
                                 pass
                         elif 'local storage limit' in line:
@@ -226,34 +262,53 @@
                             try:
                                 val = float(line.split('used')[-1].split('mb')[0].strip())/1024.
                             except Exception:
                                 try:
                                     val = float(line.split('used')[-1].split('gb')[0].strip())
                                 except Exception:
                                     pass
+                        elif 'disk usage exceeded' in line:
+                            resource_type = 'disk'
                         if resource_type:
-                            reason = f'Resource overusage for {resource_type}: {val}'
                             if val:
                                 resources[resource_type] = val
+                            reason = f'Resource overusage for {resource_type}: {resources[resource_type]}'
                             break
+                    elif 'Transfer output files failure' in line:
+                        reason = 'Failed to transfer output files'
+                        break
+                    elif 'Transfer input files failure' in line:
+                        reason = 'Failed to transfer input files'
+                        break
+                    elif 'failed due to remote transfer hook error' in line:
+                        if 'failed to send file' in line:
+                            reason = 'Failed to transfer output files'
+                        elif 'failed to receive file' in line:
+                            reason = 'Failed to transfer input files'
+                        else:
+                            reason = 'Failed to transfer files'
+                        break
         return reason
 
     async def task_error(self, task_id, dataset_id, submit_dir, reason='',
-                         site=None, pilot_id=None, kill=False):
+                         site=None, pilot_id=None, kill=False, failed=False):
         """reset a task"""
         if submit_dir is None:
             submit_dir = ''
         # search for resources in stdout
         resources = {}
+        batch_job_id = None
         filename = os.path.join(submit_dir, self.batch_outfile)
         if os.path.exists(filename):
             with open(filename) as f:
                 resource_lines = False
                 for line in f:
                     line = line.strip()
+                    if (not batch_job_id) and 'Job submitted from host' in line:
+                        batch_job_id = '.'.join(line.split('(', 1)[1].split('.')[0:2])
                     if line == 'Resources:':
                         resource_lines = True
                         continue
                     if resource_lines:
                         if ':' in line:
                             name,value = line.split(':',1)
                             if value.isdigit():
@@ -262,14 +317,20 @@
                                 try:
                                     resources[name] = float(value)
                                 except Exception:
                                     resources[name] = value
                             continue
                         else:
                             break
+
+        if batch_job_id:
+            resources.update(await self.get_grid_resources(batch_job_id))
+
+        if (not reason) and failed:
+            reason = 'payload failure'
         if not reason:
             # search for reason in logfile
             filename = os.path.join(submit_dir, constants['stdlog'])
             for line in read_filename(filename):
                 line = line.strip()
                 if 'failed to download' in line:
                     reason = 'failed to download input file(s)'
@@ -302,15 +363,15 @@
                             host = line.split()[2].strip(':')
             submitter = grid.get_host()
             message = reason + f'\n\npilot_id: {pilot_id}\nhostname: {host}\nsubmitter: {submitter}\nsite: {site}'
             await comms.task_kill(task_id, dataset_id=dataset_id, reason=reason,
                                   resources=resources, message=message, site=site)
         else:
             await comms.task_error(task_id, dataset_id=dataset_id, reason=reason,
-                                   resources=resources, site=site)
+                                   resources=resources, site=site, failed=failed)
 
     async def finish_task(self, task_id, dataset_id, submit_dir, site=None):
         """complete a task"""
         if submit_dir is None:
             submit_dir = ''
         # search for reasources in slurm stdout
         resources = {}
@@ -401,30 +462,33 @@
         async def post_process(task):
             task_id = task['task_id']
             ret = await self.rest_client.request('GET', f'/tasks/{task_id}')
             if ret['status'] == 'processing':
                 task['dataset_id'] = ret['dataset_id']
 
                 logger.info('uploading logs for task %s', task_id)
-                await self.upload_logfiles(task_id, task['dataset_id'],
-                                           submit_dir=task['submit_dir'])
+                payload_failure = await self.upload_logfiles(task_id, task['dataset_id'],
+                                                             submit_dir=task['submit_dir'])
                 if task['grid']['status'] == 'ok':
                     # upload files (may be a no-op)
                     await self.upload_output(task)
 
                     logger.info('finished task %s', task_id)
                     await self.finish_task(task_id,
                                            dataset_id=task['dataset_id'],
                                            submit_dir=task['submit_dir'],
                                            site=task['grid']['site'])
                 else:
                     logger.info('error in task %s', task_id)
+                    if payload_failure:
+                        logger.info('payload failed')
                     await self.task_error(task_id, task['dataset_id'],
                                           submit_dir=task['submit_dir'],
-                                          site=task['grid']['site'])
+                                          site=task['grid']['site'],
+                                          failed=payload_failure)
 
         async def post_process_complete(fut):
             ret = await fut
             task = ret['args'][0]
             if 'exception' in ret:
                 reason = f'failed post-processing task\n{ret["exception"]}'
                 logger.warning(reason)
@@ -913,14 +977,33 @@
             minor_2 = int(parts[1].split('.')[1])
             for i in range(minor_1, minor_2+1):
                 grid_queue_id.append('{}.{}'.format(major,i))
         task['grid_queue_id'] = ','.join(grid_queue_id)
 
         return task
 
+    async def get_grid_resources(self, job_id):
+        """Get resource information from a running/held task on the queue system"""
+        ret = {}
+        cmd = ['condor_q', job_id, '-af:,', 'CpusUsage', 'GPUsUsage', 'ResidentSetSize_RAW', 'DiskUsage_RAW', 'LastRemoteWallClockTime']
+        out = await check_output_clean_env(*cmd)
+        print('get_grid_status():',out)
+        cpu, gpu, memory, disk, time = out.strip().split(',')
+        if cpu != 'undefined':
+            ret['cpu'] = float(cpu)
+        if gpu != 'undefined':
+            ret['gpu'] = float(gpu)
+        if memory != 'undefined':
+            ret['memory'] = float(memory)/1024/1024.
+        if disk != 'undefined':
+            ret['disk'] = float(disk)/1024/1024.
+        if time != 'undefined':
+            ret['time'] = float(time)/3600.
+        return ret
+
     async def get_grid_status(self):
         """Get all tasks running on the queue system.
            Returns {grid_queue_id:{status,submit_dir}}
         """
         ret = {}
         cmd = ['condor_q', '-constraint', f'Owner == "{getpass.getuser()}" && IceProdSiteId == "{self.cfg["site_id"]}"',
                '-af:j,', 'jobstatus', 'MATCH_EXP_JOBGLIDEIN_ResourceName', 'cmd']
```

### Comparing `iceprod-2.6.9/iceprod/server/plugins/condor_file_transfer.py` & `iceprod-2.7.0/iceprod/server/plugins/condor_file_transfer.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/plugins/sc_demo.py` & `iceprod-2.7.0/iceprod/server/plugins/sc_demo.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/plugins/supercomp_cedar.py` & `iceprod-2.7.0/iceprod/server/plugins/supercomp_cedar.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/plugins/supercomp_graham.py` & `iceprod-2.7.0/iceprod/server/plugins/supercomp_graham.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/priority.py` & `iceprod-2.7.0/iceprod/server/priority.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,27 +166,27 @@
             priority *= dataset_prio / max_dataset_prio
             logger.info(f'{dataset_id} after dataset adjustment: {priority}')
         if group == 'users':
             logger.info('group is "users", so skipping dataset group adjustment')
         elif max_dataset_prio_group > 0:
             priority -= (1. - dataset_prio / max_dataset_prio_group) / 4.
             logger.info(f'{dataset_id} after dataset group adjustment: {priority}')
-        priority *= user_prio
+        priority *= user_prio**.5
         logger.info(f'{dataset_id} after user adjustment: {priority}')
         priority *= group_prio
         logger.info(f'{dataset_id} after group adjustment: {priority}')
 
         # bias against large datasets
-        factor = (10000. / num_dataset_tasks)**.15 if num_dataset_tasks > 0 else 1.
+        factor = (10000. / num_dataset_tasks)**.1 if num_dataset_tasks > 0 else 1.
         if factor > 1:
             factor = 1.
         priority *= factor
         logger.info(f'{dataset_id} after large dataset adjustment: {priority}')
 
-        priority -= (1. * num_dataset_tasks_avail / num_all_tasks) / 5.
+        priority -= (1. * num_dataset_tasks_avail / num_all_tasks) / 4.
         logger.info(f'{dataset_id} after avail tasks adjustment: {priority}')
 
         if priority < 0.:
             priority = 0.
         elif priority > 1.:
             priority = 1.
         logger.info(f'{dataset_id} final priority: {priority}')
```

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/buffer_jobs_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_cleanup.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_completion.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_completion.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/dataset_monitor.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/dataset_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/job_completion.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/job_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 import logging
 
 from iceprod.client_auth import add_auth_to_argparse, create_rest_client
 
 logger = logging.getLogger('job_completion')
 
 
-async def run(rest_client, debug=False):
+async def run(rest_client, dataset_id=None, debug=False):
     """
     Actual runtime / loop.
 
     Args:
         rest_client (:py:class:`iceprod.core.rest_client.Client`): rest client
+        dataset_id (str): specific dataset to run on
         debug (bool): debug flag to propagate exceptions
     """
-    datasets = await rest_client.request('GET', '/dataset_summaries/status')
-    dataset_ids = []
-    if 'processing' in datasets:
-        dataset_ids.extend(list(datasets['processing']))
-    if 'truncated' in datasets:
-        dataset_ids.extend(list(datasets['truncated']))
+    if dataset_id:
+        dataset_ids = [dataset_id]
+    else:
+        datasets = await rest_client.request('GET', '/dataset_summaries/status')
+        dataset_ids = []
+        if 'processing' in datasets:
+            dataset_ids.extend(list(datasets['processing']))
+        if 'truncated' in datasets:
+            dataset_ids.extend(list(datasets['truncated']))
     for dataset_id in dataset_ids:
         try:
             jobs = await rest_client.request('GET', '/datasets/{}/job_summaries/status'.format(dataset_id))
             if 'processing' not in jobs:
                 continue
             for job_id in jobs['processing']:
                 tasks = await rest_client.request('GET', '/datasets/{}/tasks?keys=task_id|task_index|status&job_id={}'.format(dataset_id,job_id))
@@ -58,20 +62,21 @@
 
 
 def main():
     parser = argparse.ArgumentParser(description='run a scheduled task once')
     add_auth_to_argparse(parser)
     parser.add_argument('--log-level', default='info', help='log level')
     parser.add_argument('--debug', default=False, action='store_true', help='debug enabled')
+    parser.add_argument('--dataset-id', help='specific dataset to run on')
 
     args = parser.parse_args()
 
     logformat = '%(asctime)s %(levelname)s %(name)s %(module)s:%(lineno)s - %(message)s'
     logging.basicConfig(format=logformat, level=getattr(logging, args.log_level.upper()))
 
     rest_client = create_rest_client(args)
 
-    asyncio.run(run(rest_client, debug=args.debug))
+    asyncio.run(run(rest_client, dataset_id=args.dataset_id, debug=args.debug))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/job_temp_cleaning.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/job_temp_cleaning.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/log_cleanup.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/log_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/non_active_tasks.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/non_active_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_cleanup.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_cleanup.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/pilot_monitor.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/pilot_monitor.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/queue_tasks.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/queue_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/removed_tasks.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/removed_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/reset_tasks.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/reset_tasks.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/scheduled_tasks/update_task_priority.py` & `iceprod-2.7.0/iceprod/server/scheduled_tasks/update_task_priority.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/server.py` & `iceprod-2.7.0/iceprod/server/server.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/ssl_cert.py` & `iceprod-2.7.0/iceprod/server/ssl_cert.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         cert.add_extensions([
             crypto.X509Extension(b"basicConstraints", True,
                                  b"CA:TRUE, pathlen:1"),
             crypto.X509Extension(b"keyUsage", True,
                                  b"keyCertSign, cRLSign"),
             crypto.X509Extension(b"subjectKeyIdentifier", False, hash,
                                  subject=cert),
-            crypto.X509Extension(b"subjectAltName", False, b'DNS:'+hostname)
+            crypto.X509Extension(b"subjectAltName", False, b'DNS:'+hostname.encode('utf-8'))
         ])
         cert.sign(k, 'sha512')
 
         open(cert_filename, "wb").write(
             crypto.dump_certificate(crypto.FILETYPE_PEM, cert))
         open(key_filename, "wb").write(
             crypto.dump_privatekey(crypto.FILETYPE_PEM, k))
@@ -125,15 +125,15 @@
             cert.gmtime_adj_notBefore(0)
             cert.gmtime_adj_notAfter(days*24*60*60)
             cert.set_serial_number(uuid.uuid4().int)
             cert.set_issuer(cert.get_subject())
             cert.set_pubkey(k)
 
             # add extensions
-            exts = [crypto.X509Extension(b'subjectAltName', False, b'DNS:'+hostname)]
+            exts = [crypto.X509Extension(b'subjectAltName', False, b'DNS:'+hostname.encode('utf-8'))]
             if allow_resign:
                 exts.extend([
                     crypto.X509Extension("basicConstraints", True,
                                          "CA:TRUE, pathlen:0"),
                     # crypto.X509Extension("keyUsage", True,
                     #                      "keyCertSign, cRLSign"),
                     # crypto.X509Extension("subjectKeyIdentifier", False, hash,
@@ -166,15 +166,15 @@
             cert2.set_serial_number(1)
             cert2.gmtime_adj_notBefore(0)
             cert2.gmtime_adj_notAfter(days*24*60*60)
             cert2.set_issuer(ca_cert.get_subject())
             cert2.set_pubkey(cert.get_pubkey())
 
             # add extensions
-            exts = [crypto.X509Extension(b"subjectAltName", False, b'DNS:'+hostname)]
+            exts = [crypto.X509Extension(b"subjectAltName", False, b'DNS:'+hostname.encode('utf-8'))]
             if allow_resign:
                 exts.extend([
                     crypto.X509Extension(b"basicConstraints", True,
                                          b"CA:TRUE, pathlen:0"),
                     # crypto.X509Extension("keyUsage", True,
                     #                      "keyCertSign, cRLSign"),
                     # crypto.X509Extension("subjectKeyIdentifier", False, hash,
```

### Comparing `iceprod-2.6.9/iceprod/server/task_queue.py` & `iceprod-2.7.0/iceprod/server/task_queue.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod/server/util.py` & `iceprod-2.7.0/iceprod/server/util.py`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/iceprod.egg-info/PKG-INFO` & `iceprod-2.7.0/iceprod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceprod
-Version: 2.6.9
+Version: 2.7.0
 Summary: IceCube dataset management system
 Home-page: https://github.com/WIPACrepo/iceprod
 Download-URL: https://pypi.org/project/iceprod/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/iceprod/issues
```

### Comparing `iceprod-2.6.9/iceprod.egg-info/SOURCES.txt` & `iceprod-2.7.0/iceprod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iceprod-2.6.9/setup.cfg` & `iceprod-2.7.0/setup.cfg`

 * *Files identical despite different names*

