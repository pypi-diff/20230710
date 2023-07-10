# Comparing `tmp/Flask-AppBuilder-4.3.4.tar.gz` & `tmp/Flask-AppBuilder-4.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-AppBuilder-4.3.4.tar", last modified: Mon Jul 10 16:21:55 2023, max compression
+gzip compressed data, was "Flask-AppBuilder-4.3.4rc1.tar", last modified: Mon Jul 10 14:22:22 2023, max compression
```

## Comparing `Flask-AppBuilder-4.3.4.tar` & `Flask-AppBuilder-4.3.4rc1.tar`

### file list

```diff
@@ -1,1182 +1,1182 @@
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.506811 Flask-AppBuilder-4.3.4/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.coveragerc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.env
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.454022 Flask-AppBuilder-4.3.4/.github/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.github/prlint.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.github/stale.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.456005 Flask-AppBuilder-4.3.4/.github/workflows/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8119 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/.github/workflows/ci.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.github/workflows/odbcinst.ini
--rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.github/workflows/ptlint.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)    64501 2023-07-10 16:21:49.000000 Flask-AppBuilder-4.3.4/CHANGELOG.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1894 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/CONTRIBUTING.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.460619 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9312 2023-07-10 16:21:54.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36154 2023-07-10 16:21:54.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-07-10 16:21:54.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-07-10 16:21:54.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/entry_points.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/not-zip-safe
--rw-r--r--   0 dpgaspar   (501) staff       (20)      559 2023-07-10 16:21:54.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/requires.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)       23 2023-07-10 16:21:54.000000 Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/top_level.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.4/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/MANIFEST.in
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9312 2023-07-10 16:21:55.506975 Flask-AppBuilder-4.3.4/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/RELEASE.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.461956 Flask-AppBuilder-4.3.4/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/babel/messages.pot
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.451313 Flask-AppBuilder-4.3.4/bin/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/babel_init.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/bootswatch_update.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/config.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/db_create.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/db_migrate.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/db_upgrade.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/hash_db_password.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/migrate_db_0.7.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/migrate_db_1.3.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/bin/sqlite_upgrade_1.3.sql
--rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-24 14:03:04.000000 Flask-AppBuilder-4.3.4/docker-compose.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.483718 Flask-AppBuilder-4.3.4/docs/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/Makefile
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.484372 Flask-AppBuilder-4.3.4/docs/_static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_static/Flask-AppBuilder.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.485245 Flask-AppBuilder-4.3.4/docs/_templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_templates/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.487131 Flask-AppBuilder-4.3.4/docs/_themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/README
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.489085 Flask-AppBuilder-4.3.4/docs/_themes/flask/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask/layout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask/relations.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.490437 Flask-AppBuilder-4.3.4/docs/_themes/flask/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask/static/Flask-AppBuilder.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.491819 Flask-AppBuilder-4.3.4/docs/_themes/flask_small/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.492521 Flask-AppBuilder-4.3.4/docs/_themes/flask_small/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/_themes/flask_theme_support.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/actions.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/addons.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.4/docs/advanced.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/cli.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/conf.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33485 2023-06-19 07:52:15.000000 Flask-AppBuilder-4.3.4/docs/config.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/customizing.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/diagrams.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/generic_datasource.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/docs/i18n.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.515180 Flask-AppBuilder-4.3.4/docs/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/oauth_login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/oauth_login_one_provider.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/simpleview2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/swagger001.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/images/swagger002.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/docs/index.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.4/docs/installation.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/intro.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/make.bat
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/multipledbs.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/quickcharts.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/quickfiles.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/quickhowto.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/quickhowto_mongo.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/quickminimal.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/relations.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.4/docs/rest_api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/docs/security.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/templates.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/user_registration.rst
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/versionmigration.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/docs/views.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.515994 Flask-AppBuilder-4.3.4/examples/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.517540 Flask-AppBuilder-4.3.4/examples/base_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/base_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.518952 Flask-AppBuilder-4.3.4/examples/base_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/base_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/base_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/base_api/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.523841 Flask-AppBuilder-4.3.4/examples/basefilter/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.527338 Flask-AppBuilder-4.3.4/examples/basefilter/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.366419 Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.366468 Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.529767 Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.533368 Flask-AppBuilder-4.3.4/examples/basefilter/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/basefilter/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.536977 Flask-AppBuilder-4.3.4/examples/composite_keys/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/composite_keys/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.540572 Flask-AppBuilder-4.3.4/examples/composite_keys/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/composite_keys/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/composite_keys/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/composite_keys/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/composite_keys/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/composite_keys/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.545842 Flask-AppBuilder-4.3.4/examples/crud_rest_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.549798 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.367003 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.367054 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.552288 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.554841 Flask-AppBuilder-4.3.4/examples/crud_rest_api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-07-10 13:44:00.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/examples/crud_rest_api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.558448 Flask-AppBuilder-4.3.4/examples/dash/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.560612 Flask-AppBuilder-4.3.4/examples/dash/app/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.565217 Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/Dash_App1.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/Dash_App2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/Dash_fun.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.566216 Flask-AppBuilder-4.3.4/examples/dash/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/templates/dash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.568362 Flask-AppBuilder-4.3.4/examples/dash/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/dash/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.570532 Flask-AppBuilder-4.3.4/examples/employees/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/employees/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.574923 Flask-AppBuilder-4.3.4/examples/employees/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/employees/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/employees/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/employees/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.4/examples/employees/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.576290 Flask-AppBuilder-4.3.4/examples/employees/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/employees/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/employees/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.581216 Flask-AppBuilder-4.3.4/examples/enums/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.584647 Flask-AppBuilder-4.3.4/examples/enums/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.367982 Flask-AppBuilder-4.3.4/examples/enums/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.368029 Flask-AppBuilder-4.3.4/examples/enums/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.586819 Flask-AppBuilder-4.3.4/examples/enums/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.588984 Flask-AppBuilder-4.3.4/examples/enums/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/enums/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.593920 Flask-AppBuilder-4.3.4/examples/extendsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.600841 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.368445 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.368496 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.602986 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.606331 Flask-AppBuilder-4.3.4/examples/extendsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.611381 Flask-AppBuilder-4.3.4/examples/extendsecurity2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.618461 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.368868 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.368914 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.620879 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.623206 Flask-AppBuilder-4.3.4/examples/extendsecurity2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/extendsecurity2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.630017 Flask-AppBuilder-4.3.4/examples/factoryapp/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.633706 Flask-AppBuilder-4.3.4/examples/factoryapp/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.369278 Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.369328 Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.636203 Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.639897 Flask-AppBuilder-4.3.4/examples/factoryapp/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/config2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/factoryapp/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.642248 Flask-AppBuilder-4.3.4/examples/issue_789/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/issue_789/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/issue_789/app.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.646346 Flask-AppBuilder-4.3.4/examples/masterdetail/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.650068 Flask-AppBuilder-4.3.4/examples/masterdetail/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.369747 Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.369795 Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.652456 Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.656031 Flask-AppBuilder-4.3.4/examples/masterdetail/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/masterdetail/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.661042 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.665778 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/mysecurity.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.370138 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.370190 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.668126 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.670482 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.676971 Flask-AppBuilder-4.3.4/examples/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.680529 Flask-AppBuilder-4.3.4/examples/mongoengine/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.370528 Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.370575 Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.683009 Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.686596 Flask-AppBuilder-4.3.4/examples/mongoengine/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoengine/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.692874 Flask-AppBuilder-4.3.4/examples/mongoimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.696274 Flask-AppBuilder-4.3.4/examples/mongoimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.370933 Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.370983 Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.698468 Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.701895 Flask-AppBuilder-4.3.4/examples/mongoimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/mongoimages/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.706628 Flask-AppBuilder-4.3.4/examples/oauth/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.712428 Flask-AppBuilder-4.3.4/examples/oauth/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/oauth/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/oauth/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.714898 Flask-AppBuilder-4.3.4/examples/oauth/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/examples/oauth/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/oauth/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.718468 Flask-AppBuilder-4.3.4/examples/productsale/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.722007 Flask-AppBuilder-4.3.4/examples/productsale/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.371859 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.371783 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.726160 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.371907 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.730180 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.732324 Flask-AppBuilder-4.3.4/examples/productsale/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/productsale/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.738773 Flask-AppBuilder-4.3.4/examples/quickactions/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.744976 Flask-AppBuilder-4.3.4/examples/quickactions/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.372403 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.372323 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.749295 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.372455 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.753384 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.755534 Flask-AppBuilder-4.3.4/examples/quickactions/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickactions/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.759556 Flask-AppBuilder-4.3.4/examples/quickcharts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.768076 Flask-AppBuilder-4.3.4/examples/quickcharts/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1646 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/app/data.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.372797 Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.372847 Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.772259 Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.778264 Flask-AppBuilder-4.3.4/examples/quickcharts/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.782415 Flask-AppBuilder-4.3.4/examples/quickcharts2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.788680 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.373202 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.373249 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.792997 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5034 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.799205 Flask-AppBuilder-4.3.4/examples/quickcharts2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/babel/messages.pot~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.373908 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.373765 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.373823 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.805248 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.373953 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.812013 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickcharts2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.823340 Flask-AppBuilder-4.3.4/examples/quickfiles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.834761 Flask-AppBuilder-4.3.4/examples/quickfiles/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.838423 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.374317 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.849774 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.374435 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.861346 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.868878 Flask-AppBuilder-4.3.4/examples/quickfiles/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickfiles/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.884671 Flask-AppBuilder-4.3.4/examples/quickhowto/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.896248 Flask-AppBuilder-4.3.4/examples/quickhowto/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.374806 Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.374853 Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.904018 Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.915292 Flask-AppBuilder-4.3.4/examples/quickhowto/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-07-10 14:06:44.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.930743 Flask-AppBuilder-4.3.4/examples/quickhowto2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.960315 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/sec_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.375402 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.001778 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abDate.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abModelTable.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abPagination.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abSelect.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.009312 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/css/clean-blog.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/css/scrolling-nav.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.016808 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/img/brand.jpg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/img/loading.gif
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.031955 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.043274 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Controllers/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.050978 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Directives/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.054896 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Services/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Services/apiService.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/angular.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/app.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/clean-blog.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/scrolling-nav.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.089217 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.096208 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/list_angulajs.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/list_contacts.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/list_json.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/mylist.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/new_base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/show_contacts.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.110136 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/widgets/list_override.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.375962 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.376007 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.124358 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.145779 Flask-AppBuilder-4.3.4/examples/quickhowto2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.196118 Flask-AppBuilder-4.3.4/examples/quickhowto3/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/.coverage
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.217303 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.376379 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.376429 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.222658 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.223423 Flask-AppBuilder-4.3.4/examples/quickhowto3/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/migrate_db_0.7.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickhowto3/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.223886 Flask-AppBuilder-4.3.4/examples/quickimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.224591 Flask-AppBuilder-4.3.4/examples/quickimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.376885 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.376812 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.225231 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.376931 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.225843 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.226140 Flask-AppBuilder-4.3.4/examples/quickimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickimages/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.227485 Flask-AppBuilder-4.3.4/examples/quickmigrate/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.228086 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.377301 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.377360 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.228469 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.228953 Flask-AppBuilder-4.3.4/examples/quickmigrate/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickmigrate/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.229187 Flask-AppBuilder-4.3.4/examples/quickminimal/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quickminimal/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.233966 Flask-AppBuilder-4.3.4/examples/quicksqlviews/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.235104 Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/encodings.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/misc.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/modules.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/quicksqlviews.iml
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/workspace.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.235712 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.377886 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.377933 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.236183 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.236606 Flask-AppBuilder-4.3.4/examples/quicksqlviews/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicksqlviews/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.237792 Flask-AppBuilder-4.3.4/examples/quicktemplates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.238403 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.378346 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.238595 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/static/css/landing-page.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.238762 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/templates/mybase.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.378558 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.378607 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.239184 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.239767 Flask-AppBuilder-4.3.4/examples/quicktemplates/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/quicktemplates/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.240970 Flask-AppBuilder-4.3.4/examples/react-rest-api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.241728 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.243797 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/.babelrc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/README.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/package-lock.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/package.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/package.json.react-original
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.244250 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/public/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/public/favicon.ico
--rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/public/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/public/manifest.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.244573 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/App.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.244848 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/api/Api.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.245489 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/CRUDButtons.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/Forms.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/Table.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/index.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/webpack.config.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.245870 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/templates/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/templates/react.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.379515 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.379567 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.246265 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.246832 Flask-AppBuilder-4.3.4/examples/react-rest-api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/react-rest-api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.248358 Flask-AppBuilder-4.3.4/examples/related_fields/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.249083 Flask-AppBuilder-4.3.4/examples/related_fields/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.379937 Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.379985 Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.249699 Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/examples/related_fields/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.250118 Flask-AppBuilder-4.3.4/examples/related_fields/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/related_fields/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.253032 Flask-AppBuilder-4.3.4/examples/simpleform/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.253721 Flask-AppBuilder-4.3.4/examples/simpleform/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/app/forms.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.254028 Flask-AppBuilder-4.3.4/examples/simpleform/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/app/templates/404.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.380393 Flask-AppBuilder-4.3.4/examples/simpleform/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.380440 Flask-AppBuilder-4.3.4/examples/simpleform/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.254531 Flask-AppBuilder-4.3.4/examples/simpleform/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.255139 Flask-AppBuilder-4.3.4/examples/simpleform/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleform/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.255784 Flask-AppBuilder-4.3.4/examples/simpleview1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.260905 Flask-AppBuilder-4.3.4/examples/simpleview1/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.261395 Flask-AppBuilder-4.3.4/examples/simpleview1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview1/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.261868 Flask-AppBuilder-4.3.4/examples/simpleview2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.264719 Flask-AppBuilder-4.3.4/examples/simpleview2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.264917 Flask-AppBuilder-4.3.4/examples/simpleview2/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/app/templates/method3.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.265502 Flask-AppBuilder-4.3.4/examples/simpleview2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/simpleview2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.267224 Flask-AppBuilder-4.3.4/examples/user_registration/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.268026 Flask-AppBuilder-4.3.4/examples/user_registration/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.381312 Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.381365 Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.268677 Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3965 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/examples/user_registration/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.269358 Flask-AppBuilder-4.3.4/examples/user_registration/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/user_registration/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.273456 Flask-AppBuilder-4.3.4/examples/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.274164 Flask-AppBuilder-4.3.4/examples/widgets/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.381922 Flask-AppBuilder-4.3.4/examples/widgets/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.381993 Flask-AppBuilder-4.3.4/examples/widgets/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.274639 Flask-AppBuilder-4.3.4/examples/widgets/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.275458 Flask-AppBuilder-4.3.4/examples/widgets/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/examples/widgets/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.289812 Flask-AppBuilder-4.3.4/flask_appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-07-10 16:21:49.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2023-06-30 15:17:51.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/_compat.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/actions.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.291116 Flask-AppBuilder-4.3.4/flask_appbuilder/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/api/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/api/convert.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/api/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/api/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.295143 Flask-AppBuilder-4.3.4/flask_appbuilder/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/babel/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2311 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/babel/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/babel/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26023 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/basemanager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48967 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/baseviews.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.296359 Flask-AppBuilder-4.3.4/flask_appbuilder/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/charts/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/charts/jsontools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/charts/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/charts/widgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/console.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8403 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/const.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/exceptions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/fieldwidgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/filemanager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11129 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/hooks.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/messages.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.302813 Flask-AppBuilder-4.3.4/flask_appbuilder/models/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10374 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/filters.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.303718 Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/interface.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10970 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/group.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/mixins.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.309229 Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9982 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.310226 Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39115 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.316193 Flask-AppBuilder-4.3.4/flask_appbuilder/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10558 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    76822 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/manager.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.317096 Flask-AppBuilder-4.3.4/flask_appbuilder/security/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15303 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/mongoengine/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/mongoengine/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10630 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/registerviews.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.317903 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.318197 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.318953 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.319492 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission_view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2023-07-10 13:48:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.320347 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/role/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/role/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/role/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/role/schema.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.324087 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/schema.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/validator.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.324741 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/view_menu/api.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    26664 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/manager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/utils.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/security/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.384190 Flask-AppBuilder-4.3.4/flask_appbuilder/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.385050 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.325405 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/ab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.326447 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/flags/flags16.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.328302 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.345552 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/amelia.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/darkly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/flatly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/journal.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/lumen.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/paper.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/readable.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/simplex.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/slate.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/solar.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/superhero.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/united.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/yeti.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.348861 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/datepicker/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.353206 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.355263 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/aol.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/fab.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.357579 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/flags/flags16.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/flickr.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/google.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/myopenid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/yahoo.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.367643 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3321 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab_actions.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5176 2023-07-10 14:06:29.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab_filters.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/google_charts.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/jquery-latest.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.374292 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2x2.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.392805 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.385173 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.398054 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/_formhelpers.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/baselayout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4588 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/baselib.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/flash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/footer.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.398788 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/alert.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.399404 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/confirm.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14551 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/lib.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.401191 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/add.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1181 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/edit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      813 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      501 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1207 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      784 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.407824 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/activation.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_db.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6568 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.416651 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1153 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2981 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2613 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1631 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.424238 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/roles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1087 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2997 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/init.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/navbar.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1247 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1564 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/navbar_right.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.426874 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/swagger/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      884 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/swagger/swagger.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.427106 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.427253 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2023-07-05 19:34:38.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.386772 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/de/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.428080 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/de/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.387685 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/el/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.428927 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/el/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.388619 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.430002 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.389585 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/fr/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.430470 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/fr/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.390831 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/it/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.430974 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/it/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.401129 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ja_JP/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.431678 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.403885 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ko/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.436783 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ko/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.410863 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/nl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.437301 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/nl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.411935 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.437842 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.413017 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.438625 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.413937 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt_BR/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.439270 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.422740 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ru/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.440016 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ru/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.423874 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/sl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.440780 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/sl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.424894 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.441411 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:54.425953 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh_HK/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.441868 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/upload.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.447023 Flask-AppBuilder-4.3.4/flask_appbuilder/utils/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/utils/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/utils/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/utils/limit.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/validators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4/flask_appbuilder/widgets.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.472586 Flask-AppBuilder-4.3.4/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/login_oauth.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/images/simpleview2.png
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      181 2023-07-10 15:46:46.000000 Flask-AppBuilder-4.3.4/release.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4/requirements-dev.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4/requirements-extra.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2905 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4/requirements.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4/rtd_requirements.txt
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.473112 Flask-AppBuilder-4.3.4/scripts/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/scripts/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/scripts/babel_init.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2023-07-10 16:21:55.507564 Flask-AppBuilder-4.3.4/setup.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2848 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4/setup.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.482820 Flask-AppBuilder-4.3.4/tests/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5390 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/config_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/config_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/config_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/config_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/const.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.483668 Flask-AppBuilder-4.3.4/tests/fixtures/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/fixtures/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/fixtures/addon_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9430 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/fixtures/data_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1113 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/fixtures/users.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.483949 Flask-AppBuilder-4.3.4/tests/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/mongoengine/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.506183 Flask-AppBuilder-4.3.4/tests/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35649 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/test_auth_ldap.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14748 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/test_auth_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/test_base_security_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/test_mvc_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/test_password_complexity.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2956 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/security/test_rate_limiter.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 16:21:55.506589 Flask-AppBuilder-4.3.4/tests/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5815 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_addon.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129520 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1211 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_custom_indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8787 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_fab_cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6470 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24059 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_mongoengine.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    72094 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_mvc.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5016 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_mvc_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    44610 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6022 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_security_permissions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_sqlalchemy.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2506 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4/tests/test_urltools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4/tox.ini
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.761952 Flask-AppBuilder-4.3.4rc1/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.coveragerc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.env
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.477506 Flask-AppBuilder-4.3.4rc1/.github/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.github/prlint.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.github/stale.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.479676 Flask-AppBuilder-4.3.4rc1/.github/workflows/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8119 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/.github/workflows/ci.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.github/workflows/odbcinst.ini
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.github/workflows/ptlint.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    64501 2023-07-10 14:08:44.000000 Flask-AppBuilder-4.3.4rc1/CHANGELOG.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1894 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/CONTRIBUTING.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.484592 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9315 2023-07-10 14:22:21.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36154 2023-07-10 14:22:21.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-07-10 14:22:21.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-07-10 14:22:21.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/entry_points.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/not-zip-safe
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      559 2023-07-10 14:22:21.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/requires.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       23 2023-07-10 14:22:21.000000 Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/top_level.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.4rc1/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/MANIFEST.in
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9315 2023-07-10 14:22:22.762139 Flask-AppBuilder-4.3.4rc1/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/RELEASE.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.485972 Flask-AppBuilder-4.3.4rc1/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/babel/messages.pot
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.474803 Flask-AppBuilder-4.3.4rc1/bin/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/babel_init.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/bootswatch_update.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/config.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/db_create.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/db_migrate.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/db_upgrade.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/hash_db_password.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/migrate_db_0.7.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/migrate_db_1.3.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/bin/sqlite_upgrade_1.3.sql
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-24 14:03:04.000000 Flask-AppBuilder-4.3.4rc1/docker-compose.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.509453 Flask-AppBuilder-4.3.4rc1/docs/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/Makefile
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.510128 Flask-AppBuilder-4.3.4rc1/docs/_static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_static/Flask-AppBuilder.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.511041 Flask-AppBuilder-4.3.4rc1/docs/_templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_templates/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.512892 Flask-AppBuilder-4.3.4rc1/docs/_themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/README
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.514901 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/layout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/relations.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.516332 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/Flask-AppBuilder.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.517648 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.518348 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/actions.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/addons.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.4rc1/docs/advanced.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/cli.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/conf.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33485 2023-06-19 07:52:15.000000 Flask-AppBuilder-4.3.4rc1/docs/config.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/customizing.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/diagrams.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/generic_datasource.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/docs/i18n.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.539845 Flask-AppBuilder-4.3.4rc1/docs/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/oauth_login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/oauth_login_one_provider.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/simpleview2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/swagger001.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/images/swagger002.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/docs/index.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.4rc1/docs/installation.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/intro.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/make.bat
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/multipledbs.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/quickcharts.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/quickfiles.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/quickhowto.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/quickhowto_mongo.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/quickminimal.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/relations.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.4rc1/docs/rest_api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/docs/security.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/templates.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/user_registration.rst
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/versionmigration.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/docs/views.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.540671 Flask-AppBuilder-4.3.4rc1/examples/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.542228 Flask-AppBuilder-4.3.4rc1/examples/base_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/base_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.543634 Flask-AppBuilder-4.3.4rc1/examples/base_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/base_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/base_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/base_api/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.546938 Flask-AppBuilder-4.3.4rc1/examples/basefilter/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.548942 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.412790 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.412842 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.550363 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.552375 Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/basefilter/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.554480 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.556532 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/composite_keys/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.560238 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.563858 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.413370 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.413418 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.566570 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.568946 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-07-10 13:44:00.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.572337 Flask-AppBuilder-4.3.4rc1/examples/dash/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.574777 Flask-AppBuilder-4.3.4rc1/examples/dash/app/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.579803 Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_App1.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_App2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_fun.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.580990 Flask-AppBuilder-4.3.4rc1/examples/dash/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/templates/dash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.583426 Flask-AppBuilder-4.3.4rc1/examples/dash/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/dash/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.585759 Flask-AppBuilder-4.3.4rc1/examples/employees/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.590380 Flask-AppBuilder-4.3.4rc1/examples/employees/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.591672 Flask-AppBuilder-4.3.4rc1/examples/employees/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/employees/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.596393 Flask-AppBuilder-4.3.4rc1/examples/enums/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.599919 Flask-AppBuilder-4.3.4rc1/examples/enums/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.414356 Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.414403 Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.602134 Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.604348 Flask-AppBuilder-4.3.4rc1/examples/enums/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/enums/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.609420 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.616877 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.414755 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.414810 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.618976 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.622331 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.627063 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.633679 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.415155 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.415203 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.635790 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.637940 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.644275 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.647543 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.415578 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.415634 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.649690 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.652894 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/config2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/factoryapp/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.655022 Flask-AppBuilder-4.3.4rc1/examples/issue_789/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/issue_789/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/issue_789/app.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.658755 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.662134 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.416043 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.416090 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.664463 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.669335 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/masterdetail/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.677308 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.685094 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/mysecurity.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.416467 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.416518 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.689230 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.693204 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.703818 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.709651 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.416864 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.416911 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.713531 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.719616 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoengine/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.729874 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.737435 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.417283 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.417342 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.744722 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.755638 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/mongoimages/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.770392 Flask-AppBuilder-4.3.4rc1/examples/oauth/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.788944 Flask-AppBuilder-4.3.4rc1/examples/oauth/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.796507 Flask-AppBuilder-4.3.4rc1/examples/oauth/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/oauth/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.807517 Flask-AppBuilder-4.3.4rc1/examples/productsale/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.818594 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.418206 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.418118 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.826142 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.418261 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.833552 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.837306 Flask-AppBuilder-4.3.4rc1/examples/productsale/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/productsale/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.848830 Flask-AppBuilder-4.3.4rc1/examples/quickactions/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.860024 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.418837 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.418745 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.867667 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.418892 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.875299 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.879130 Flask-AppBuilder-4.3.4rc1/examples/quickactions/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickactions/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.886785 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.901826 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1646 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/data.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.419246 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.419295 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.909485 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.920806 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.928544 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.939941 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.419656 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.419707 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.947730 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5034 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.959128 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/messages.pot~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.420103 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.419968 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.420024 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.970643 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.420151 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.982103 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.993682 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.005257 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.009102 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.420528 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.030053 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.420678 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.051959 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.066717 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickfiles/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.097038 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.119205 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.421057 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.421115 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.134106 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.155893 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-07-10 14:06:44.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.185611 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.249722 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/sec_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.421740 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.343927 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abDate.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abSelect.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.361448 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/clean-blog.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/scrolling-nav.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.386210 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/brand.jpg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/loading.gif
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.417797 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.442329 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.467806 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.475190 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Services/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Services/apiService.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/angular.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/app.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/clean-blog.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/scrolling-nav.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.516947 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.517340 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_angulajs.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_contacts.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_json.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/mylist.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/new_base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/show_contacts.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.518184 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/widgets/list_override.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.422348 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.422403 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.519013 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.520372 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.527892 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/.coverage
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.528992 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.422780 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.422834 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.531966 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.533110 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/migrate_db_0.7.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.533865 Flask-AppBuilder-4.3.4rc1/examples/quickimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.535128 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.423370 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.423271 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.536076 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.423426 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.537455 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.540304 Flask-AppBuilder-4.3.4rc1/examples/quickimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickimages/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.542397 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.545798 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.423828 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.423881 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.546624 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.547407 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.547773 Flask-AppBuilder-4.3.4rc1/examples/quickminimal/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quickminimal/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.549657 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.556630 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/encodings.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/misc.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/modules.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/quicksqlviews.iml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/workspace.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.557558 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.424400 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.424454 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.558257 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.558974 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.561073 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.561845 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.424805 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.562129 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/static/css/landing-page.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.562389 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/templates/mybase.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.425014 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.425062 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.562881 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.563587 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.565476 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.566504 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.569198 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/.babelrc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/README.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package-lock.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package.json.react-original
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.569907 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/public/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/public/favicon.ico
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/public/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/public/manifest.json
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.572621 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/App.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.572827 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/api/Api.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.573597 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/Forms.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/Table.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/index.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/webpack.config.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.574092 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/templates/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/templates/react.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.425895 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.425947 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.574503 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.574974 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.578772 Flask-AppBuilder-4.3.4rc1/examples/related_fields/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.579535 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.426372 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.426430 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.580261 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.580935 Flask-AppBuilder-4.3.4rc1/examples/related_fields/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/related_fields/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.584550 Flask-AppBuilder-4.3.4rc1/examples/simpleform/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.585369 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/forms.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.585643 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/templates/404.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.426884 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.426936 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.588508 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.589075 Flask-AppBuilder-4.3.4rc1/examples/simpleform/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleform/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.589890 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.594922 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.597625 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview1/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.598064 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.598489 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.598703 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/templates/method3.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.599075 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/simpleview2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.601010 Flask-AppBuilder-4.3.4rc1/examples/user_registration/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.606208 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.427899 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.427967 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.606752 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3965 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.607301 Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/user_registration/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.608552 Flask-AppBuilder-4.3.4rc1/examples/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.609182 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.428619 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.428675 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.609624 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.610254 Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/examples/widgets/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.621448 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2023-07-10 14:07:51.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2023-06-30 15:17:51.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/_compat.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/actions.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.622512 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/convert.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.623464 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/babel/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2311 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/babel/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/babel/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26023 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/basemanager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48967 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/baseviews.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.624450 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/jsontools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/widgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/console.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8403 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/const.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/exceptions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/fieldwidgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/filemanager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11129 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/hooks.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/messages.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.628750 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10374 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/filters.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.629727 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/interface.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10970 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/group.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mixins.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.630463 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9982 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.631176 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39115 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.633601 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10558 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    76822 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/manager.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.634125 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15303 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10630 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/registerviews.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.634621 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.634774 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.635268 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.635574 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2023-07-10 13:48:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.636111 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/role/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/role/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/role/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/role/schema.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.636953 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/schema.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/validator.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.637389 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    26664 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/manager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/utils.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.430268 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.431295 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.637826 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/ab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.638682 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.640025 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.647690 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/united.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.648125 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.649520 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.650884 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/aol.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/fab.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.651086 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flickr.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/google.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/myopenid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/yahoo.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.653216 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3321 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5176 2023-07-10 14:06:29.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/google_charts.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.655089 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.659484 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.431431 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.666948 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/_formhelpers.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/baselayout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4588 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/baselib.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/flash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/footer.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.667544 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/alert.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.670610 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/confirm.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14551 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/lib.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.679674 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/add.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1181 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      813 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      501 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1207 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      784 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.683749 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/activation.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6568 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.701918 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1153 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2981 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2613 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1631 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.702302 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1087 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2997 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/init.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1247 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1564 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar_right.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.702479 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/swagger/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      884 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.702666 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.702779 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2023-07-05 19:34:38.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.433433 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.703579 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.434576 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.709028 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.435643 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.710101 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.436735 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.710544 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.437775 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.710941 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.438792 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.711621 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.439801 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.712031 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.440907 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.712466 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.442033 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.717488 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.443178 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.718140 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.444239 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.718799 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.445342 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.721691 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.446357 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.722366 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.447363 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.722919 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:21.448433 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.723471 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/upload.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/urltools.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.724038 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/limit.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/validators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.4rc1/flask_appbuilder/widgets.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.742163 Flask-AppBuilder-4.3.4rc1/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/login_oauth.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/images/simpleview2.png
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      180 2023-07-10 14:16:28.000000 Flask-AppBuilder-4.3.4rc1/release.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4rc1/requirements-dev.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4rc1/requirements-extra.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2905 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.4rc1/requirements.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.4rc1/rtd_requirements.txt
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.742687 Flask-AppBuilder-4.3.4rc1/scripts/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/scripts/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/scripts/babel_init.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2023-07-10 14:22:22.762640 Flask-AppBuilder-4.3.4rc1/setup.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2848 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.4rc1/setup.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.754572 Flask-AppBuilder-4.3.4rc1/tests/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5390 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/config_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/config_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/config_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/config_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/const.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.755269 Flask-AppBuilder-4.3.4rc1/tests/fixtures/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/fixtures/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/fixtures/addon_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9430 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/fixtures/data_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1113 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/fixtures/users.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.755550 Flask-AppBuilder-4.3.4rc1/tests/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/mongoengine/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.756872 Flask-AppBuilder-4.3.4rc1/tests/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35649 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/test_auth_ldap.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14748 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/test_auth_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/test_base_security_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/test_mvc_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/test_password_complexity.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2956 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/security/test_rate_limiter.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-10 14:22:22.761776 Flask-AppBuilder-4.3.4rc1/tests/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5815 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_addon.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   129520 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1211 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_custom_indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8787 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_fab_cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6470 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24059 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_mongoengine.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    72094 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_mvc.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5016 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_mvc_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    44610 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6022 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_security_permissions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_sqlalchemy.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2506 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.4rc1/tests/test_urltools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.4rc1/tox.ini
```

### Comparing `Flask-AppBuilder-4.3.4/.github/ISSUE_TEMPLATE.md` & `Flask-AppBuilder-4.3.4rc1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/.github/PULL_REQUEST_TEMPLATE.md` & `Flask-AppBuilder-4.3.4rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/.github/stale.yml` & `Flask-AppBuilder-4.3.4rc1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/.github/workflows/ci.yml` & `Flask-AppBuilder-4.3.4rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/.github/workflows/ptlint.yml` & `Flask-AppBuilder-4.3.4rc1/.github/workflows/ptlint.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/CHANGELOG.rst` & `Flask-AppBuilder-4.3.4rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/CONTRIBUTING.rst` & `Flask-AppBuilder-4.3.4rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/PKG-INFO` & `Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.4
+Version: 4.3.4rc1
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
```

### Comparing `Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/SOURCES.txt` & `Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/Flask_AppBuilder.egg-info/requires.txt` & `Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/LICENSE` & `Flask-AppBuilder-4.3.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/PKG-INFO` & `Flask-AppBuilder-4.3.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.4
+Version: 4.3.4rc1
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
```

### Comparing `Flask-AppBuilder-4.3.4/README.rst` & `Flask-AppBuilder-4.3.4rc1/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/bin/config.py` & `Flask-AppBuilder-4.3.4rc1/bin/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/bin/db_migrate.py` & `Flask-AppBuilder-4.3.4rc1/bin/db_migrate.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/bin/hash_db_password.py` & `Flask-AppBuilder-4.3.4rc1/bin/hash_db_password.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/bin/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.4rc1/bin/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/bin/migrate_db_1.3.py` & `Flask-AppBuilder-4.3.4rc1/bin/migrate_db_1.3.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/bin/sqlite_upgrade_1.3.sql` & `Flask-AppBuilder-4.3.4rc1/bin/sqlite_upgrade_1.3.sql`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docker-compose.yml` & `Flask-AppBuilder-4.3.4rc1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/Makefile` & `Flask-AppBuilder-4.3.4rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.4rc1/docs/_static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_templates/layout.html` & `Flask-AppBuilder-4.3.4rc1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/LICENSE` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/README` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask/layout.html` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask/relations.html` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask/static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask/static/flasky.css_t` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask_small/layout.html` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask_small/static/flasky.css_t` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/_themes/flask_theme_support.py` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/actions.rst` & `Flask-AppBuilder-4.3.4rc1/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/addons.rst` & `Flask-AppBuilder-4.3.4rc1/docs/addons.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/advanced.rst` & `Flask-AppBuilder-4.3.4rc1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/api.rst` & `Flask-AppBuilder-4.3.4rc1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/cli.rst` & `Flask-AppBuilder-4.3.4rc1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/conf.py` & `Flask-AppBuilder-4.3.4rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/config.rst` & `Flask-AppBuilder-4.3.4rc1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/customizing.rst` & `Flask-AppBuilder-4.3.4rc1/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/diagrams.rst` & `Flask-AppBuilder-4.3.4rc1/docs/diagrams.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/generic_datasource.rst` & `Flask-AppBuilder-4.3.4rc1/docs/generic_datasource.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/i18n.rst` & `Flask-AppBuilder-4.3.4rc1/docs/i18n.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/chart.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/chart_time1.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/chart_time2.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/charts.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/contact_list.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/contacts.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/direct_chart.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/fab.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/group_list.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/grouped_chart.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/groups.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/images_list.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/list_cascade.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/list_master_detail.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/login.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/login_db.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/login_oid.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/oauth_login.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/oauth_login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/oauth_login_one_provider.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/oauth_login_one_provider.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/security.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/simpleview2.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/swagger001.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/swagger001.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/images/swagger002.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/swagger002.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/index.rst` & `Flask-AppBuilder-4.3.4rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/installation.rst` & `Flask-AppBuilder-4.3.4rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/intro.rst` & `Flask-AppBuilder-4.3.4rc1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/make.bat` & `Flask-AppBuilder-4.3.4rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/multipledbs.rst` & `Flask-AppBuilder-4.3.4rc1/docs/multipledbs.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/quickcharts.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickcharts.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/quickfiles.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickfiles.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/quickhowto.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickhowto.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/quickhowto_mongo.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickhowto_mongo.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/quickminimal.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickminimal.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/relations.rst` & `Flask-AppBuilder-4.3.4rc1/docs/relations.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/rest_api.rst` & `Flask-AppBuilder-4.3.4rc1/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/security.rst` & `Flask-AppBuilder-4.3.4rc1/docs/security.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/templates.rst` & `Flask-AppBuilder-4.3.4rc1/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/user_registration.rst` & `Flask-AppBuilder-4.3.4rc1/docs/user_registration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/versionmigration.rst` & `Flask-AppBuilder-4.3.4rc1/docs/versionmigration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/docs/views.rst` & `Flask-AppBuilder-4.3.4rc1/docs/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/base_api/app/api.py` & `Flask-AppBuilder-4.3.4rc1/examples/base_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/base_api/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/base_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/basefilter/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/composite_keys/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/composite_keys/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/composite_keys/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/composite_keys/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/api.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/crud_rest_api/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/Dash_App1.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_App1.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/Dash_App2.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_App2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/dash/app/Dashboard/Dash_fun.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_fun.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/dash/app/templates/dash.html` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/templates/dash.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/dash/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/dash/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/employees/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/employees/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/employees/app/security.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/employees/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/employees/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/enums/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/enums/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/enums/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/sec_forms.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/sec_views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/sec_forms.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/sec_views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/extendsecurity2/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/config2.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/config2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/factoryapp/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/issue_789/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/issue_789/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/issue_789/app.py` & `Flask-AppBuilder-4.3.4rc1/examples/issue_789/app.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/masterdetail/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/mysecurity.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/mysecurity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongo_extendedsecurity/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoengine/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/mongoimages/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/oauth/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/oauth/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/oauth/app/security.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/oauth/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/oauth/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/productsale/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickactions/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/app/data.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/data.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/build/lib/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickcharts2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickfiles/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/forms.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/sec_views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abModelSearch.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abModelTable.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/angularAssets/abPagination.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/css/clean-blog.min.css` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/clean-blog.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/css/scrolling-nav.css` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/scrolling-nav.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/img/brand.jpg` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/brand.jpg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/img/loading.gif` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Directives/bigDirectives.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Directives/btnDirectives.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/Services/apiService.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Services/apiService.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/angular.min.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/angular.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/app.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/app.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/clean-blog.min.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/clean-blog.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/static/js/scrolling-nav.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/list_angulajs.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_angulajs.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/list_json.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_json.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/templates/widgets/list.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto2/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/.coverage` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/.coverage`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickhowto3/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickimages/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quickmigrate/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/misc.xml` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/.idea/workspace.xml` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicksqlviews/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/app/static/css/landing-page.css` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/static/css/landing-page.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/app/templates/mybase.html` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/templates/mybase.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/quicktemplates/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/api.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/package-lock.json` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/package.json` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/package.json.react-original` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package.json.react-original`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/public/favicon.ico` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/api/Api.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/api/Api.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/CRUDButtons.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/Forms.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/Forms.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/static/src/components/Table.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/Table.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/templates/base.html` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/react-rest-api/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/related_fields/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleform/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleform/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleform/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleview1/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview1/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleview1/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview1/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleview2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/simpleview2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/user_registration/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/examples/widgets/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Daniel Vaz Gaspar"
-__version__ = "4.3.4"
+__version__ = "4.3.4rc1"
 
 from .actions import action  # noqa: F401
 from .api import ModelRestApi  # noqa: F401
 from .base import AppBuilder  # noqa: F401
 from .baseviews import BaseView, expose  # noqa: F401
 from .charts.views import DirectByChartView, GroupByChartView  # noqa: F401
 from .models.group import aggregate_avg, aggregate_count, aggregate_sum  # noqa: F401
```

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/_compat.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/actions.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/actions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/api/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/api/convert.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/convert.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/api/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/api/schemas.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/babel/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/babel/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/base.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/baseviews.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/baseviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/charts/jsontools.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/jsontools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/charts/views.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/cli.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/console.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/console.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/const.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/const.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/exceptions.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/fields.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/fieldwidgets.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/fieldwidgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/filemanager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/filemanager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/forms.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/hooks.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/hooks.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/menu.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/base.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/decorators.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/generic/interface.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/group.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/group.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/mixins.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mixins.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/fields.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/mongoengine/interface.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/models/sqla/interface.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/decorators.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/forms.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/mongoengine/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/mongoengine/models.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/registerviews.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/registerviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/schemas.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/role/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/role/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/schema.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/schema.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/user/validator.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/validator.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/apis/view_menu/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/sqla/models.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/security/views.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/ab.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/ab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/bootstrap.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/flags/flags16.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/amelia.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/cerulean.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/cosmo.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/cyborg.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/darkly.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/flatly.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/journal.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/lumen.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/paper.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/readable.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/sandstone.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/simplex.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/slate.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/solar.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/spacelab.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/superhero.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/united.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/united.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/css/themes/yeti.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/aol.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/aol.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/fab.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/flags/flags16.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/flickr.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flickr.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/google.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/google.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/myopenid.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/myopenid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/img/yahoo.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/yahoo.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab_actions.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab_filters.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/bootstrap.min.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/google_charts.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/google_charts.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/jquery-latest.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/js/v4-shims.min.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/select2/select2x2.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/baselayout.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/baselayout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/baselib.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/baselib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/confirm.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/confirm.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/lib.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/lib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/edit.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/show.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_db.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/login_oid.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/search.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/show.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/init.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/init.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/navbar.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/navbar_menu.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/navbar_right.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/templates/appbuilder/swagger/swagger.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/de/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/el/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/it/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/upload.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/upload.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/urltools.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/utils/base.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/utils/limit.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/limit.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/validators.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/validators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/views.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/flask_appbuilder/widgets.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/widgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.4rc1/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/chart.png` & `Flask-AppBuilder-4.3.4rc1/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/chart_time1.png` & `Flask-AppBuilder-4.3.4rc1/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/chart_time2.png` & `Flask-AppBuilder-4.3.4rc1/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/charts.png` & `Flask-AppBuilder-4.3.4rc1/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/contact_list.png` & `Flask-AppBuilder-4.3.4rc1/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/contacts.png` & `Flask-AppBuilder-4.3.4rc1/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/direct_chart.png` & `Flask-AppBuilder-4.3.4rc1/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/fab.png` & `Flask-AppBuilder-4.3.4rc1/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/group_list.png` & `Flask-AppBuilder-4.3.4rc1/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/grouped_chart.png` & `Flask-AppBuilder-4.3.4rc1/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/groups.png` & `Flask-AppBuilder-4.3.4rc1/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/images_list.png` & `Flask-AppBuilder-4.3.4rc1/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/list_cascade.png` & `Flask-AppBuilder-4.3.4rc1/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.4rc1/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.4rc1/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/list_master_detail.png` & `Flask-AppBuilder-4.3.4rc1/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/login.png` & `Flask-AppBuilder-4.3.4rc1/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/login_db.png` & `Flask-AppBuilder-4.3.4rc1/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/login_oauth.png` & `Flask-AppBuilder-4.3.4rc1/images/login_oauth.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/login_oid.png` & `Flask-AppBuilder-4.3.4rc1/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/security.png` & `Flask-AppBuilder-4.3.4rc1/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/images/simpleview2.png` & `Flask-AppBuilder-4.3.4rc1/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/requirements.txt` & `Flask-AppBuilder-4.3.4rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/rtd_requirements.txt` & `Flask-AppBuilder-4.3.4rc1/rtd_requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/setup.cfg` & `Flask-AppBuilder-4.3.4rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/setup.py` & `Flask-AppBuilder-4.3.4rc1/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/base.py` & `Flask-AppBuilder-4.3.4rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/config_oauth.py` & `Flask-AppBuilder-4.3.4rc1/tests/config_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/config_security_api.py` & `Flask-AppBuilder-4.3.4rc1/tests/config_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/fixtures/data_models.py` & `Flask-AppBuilder-4.3.4rc1/tests/fixtures/data_models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/fixtures/users.py` & `Flask-AppBuilder-4.3.4rc1/tests/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/mongoengine/models.py` & `Flask-AppBuilder-4.3.4rc1/tests/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/security/test_auth_ldap.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_auth_ldap.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/security/test_auth_oauth.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_auth_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/security/test_base_security_manager.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_base_security_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/security/test_mvc_security.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_mvc_security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/security/test_password_complexity.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_password_complexity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/security/test_rate_limiter.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/sqla/models.py` & `Flask-AppBuilder-4.3.4rc1/tests/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_addon.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_addon.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_api.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_custom_indexview.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_custom_indexview.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_fab_cli.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_fab_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_menu.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_mongoengine.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_mongoengine.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_mvc.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_mvc.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_mvc_oauth.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_mvc_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_security_api.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_security_permissions.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_security_permissions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_sqlalchemy.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tests/test_urltools.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.4/tox.ini` & `Flask-AppBuilder-4.3.4rc1/tox.ini`

 * *Files identical despite different names*

