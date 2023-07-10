# Comparing `tmp/Flask-AppBuilder-4.3.3rc2.tar.gz` & `tmp/Flask-AppBuilder-4.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-AppBuilder-4.3.3rc2.tar", last modified: Wed Jun 21 12:40:14 2023, max compression
+gzip compressed data, was "Flask-AppBuilder-4.3.4rc1.tar", last modified: Mon Jul 10 14:22:22 2023, max compression
```

## Comparing `Flask-AppBuilder-4.3.3rc2.tar` & `Flask-AppBuilder-4.3.4rc1.tar`

### file list

```diff
@@ -1,1208 +1,1182 @@
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.387719 Flask-AppBuilder-4.3.3rc2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.coveragerc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.env
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.559949 Flask-AppBuilder-4.3.3rc2/.github/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.github/prlint.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.github/stale.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.561945 Flask-AppBuilder-4.3.3rc2/.github/workflows/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8087 2023-06-19 15:21:11.000000 Flask-AppBuilder-4.3.3rc2/.github/workflows/ci.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.github/workflows/odbcinst.ini
--rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.github/workflows/ptlint.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)    64082 2023-06-21 12:38:57.000000 Flask-AppBuilder-4.3.3rc2/CHANGELOG.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/CONTRIBUTING.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.566355 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9290 2023-06-21 12:40:13.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)    38050 2023-06-21 12:40:13.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-06-21 12:40:13.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-06-21 12:40:13.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/entry_points.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/not-zip-safe
--rw-r--r--   0 dpgaspar   (501) staff       (20)      520 2023-06-21 12:40:13.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/requires.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2023-06-21 12:40:13.000000 Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/top_level.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.3rc2/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/MANIFEST.in
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9290 2023-06-21 12:40:14.390120 Flask-AppBuilder-4.3.3rc2/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/RELEASE.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.567541 Flask-AppBuilder-4.3.3rc2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/babel/messages.pot
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.557457 Flask-AppBuilder-4.3.3rc2/bin/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/babel_init.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/bootswatch_update.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/config.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/db_create.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/db_migrate.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/db_upgrade.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/hash_db_password.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/migrate_db_0.7.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/migrate_db_1.3.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/bin/sqlite_upgrade_1.3.sql
--rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-24 14:03:04.000000 Flask-AppBuilder-4.3.3rc2/docker-compose.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.588410 Flask-AppBuilder-4.3.3rc2/docs/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/Makefile
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.589057 Flask-AppBuilder-4.3.3rc2/docs/_static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_static/Flask-AppBuilder.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.589970 Flask-AppBuilder-4.3.3rc2/docs/_templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_templates/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.591801 Flask-AppBuilder-4.3.3rc2/docs/_themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/README
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.593633 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/layout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/relations.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.594862 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/static/Flask-AppBuilder.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.596075 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.596704 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_theme_support.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/actions.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/addons.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.3rc2/docs/advanced.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/cli.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/conf.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33485 2023-06-19 07:52:15.000000 Flask-AppBuilder-4.3.3rc2/docs/config.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/customizing.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/diagrams.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/generic_datasource.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/docs/i18n.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.616449 Flask-AppBuilder-4.3.3rc2/docs/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/oauth_login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/oauth_login_one_provider.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/simpleview2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/swagger001.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/images/swagger002.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/docs/index.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.3rc2/docs/installation.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/intro.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/make.bat
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/multipledbs.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/quickcharts.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/quickfiles.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/quickhowto.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/quickhowto_mongo.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/quickminimal.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/relations.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/docs/rest_api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36092 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/docs/security.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/templates.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/user_registration.rst
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/versionmigration.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/docs/views.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.617106 Flask-AppBuilder-4.3.3rc2/examples/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.618323 Flask-AppBuilder-4.3.3rc2/examples/base_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/base_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.619544 Flask-AppBuilder-4.3.3rc2/examples/base_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/base_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/base_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/base_api/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.622609 Flask-AppBuilder-4.3.3rc2/examples/basefilter/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.624523 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.494428 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.494479 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.625754 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.627665 Flask-AppBuilder-4.3.3rc2/examples/basefilter/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/basefilter/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.629553 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.631478 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/composite_keys/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.634461 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.636872 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.494950 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.494996 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.638326 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.639700 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.641530 Flask-AppBuilder-4.3.3rc2/examples/dash/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.642774 Flask-AppBuilder-4.3.3rc2/examples/dash/app/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.645269 Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/Dash_App1.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/Dash_App2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/Dash_fun.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.645847 Flask-AppBuilder-4.3.3rc2/examples/dash/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/templates/dash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.647077 Flask-AppBuilder-4.3.3rc2/examples/dash/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/dash/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.648371 Flask-AppBuilder-4.3.3rc2/examples/employees/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.650865 Flask-AppBuilder-4.3.3rc2/examples/employees/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.651606 Flask-AppBuilder-4.3.3rc2/examples/employees/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/employees/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.654317 Flask-AppBuilder-4.3.3rc2/examples/enums/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.656199 Flask-AppBuilder-4.3.3rc2/examples/enums/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.495873 Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.495917 Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.657469 Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.658656 Flask-AppBuilder-4.3.3rc2/examples/enums/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/enums/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.661835 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.665627 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.496249 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.496328 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.666924 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.668837 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.671758 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.677720 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.496774 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.496832 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.679809 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.681932 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.688176 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.691358 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.497243 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.497296 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.693450 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.696650 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/config2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/factoryapp/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.698805 Flask-AppBuilder-4.3.3rc2/examples/issue_789/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/issue_789/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/issue_789/app.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.702644 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.705871 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.497793 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.497846 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.708014 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.711121 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/masterdetail/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.715508 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.719748 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/mysecurity.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.498239 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.498383 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.721861 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.723952 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.729677 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.732735 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.498825 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.498882 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.734766 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.737920 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoengine/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.743592 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.746805 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.499241 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.499290 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.748951 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.752174 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/mongoimages/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.756405 Flask-AppBuilder-4.3.3rc2/examples/oauth/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.762084 Flask-AppBuilder-4.3.3rc2/examples/oauth/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.764227 Flask-AppBuilder-4.3.3rc2/examples/oauth/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/oauth/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.768187 Flask-AppBuilder-4.3.3rc2/examples/productsale/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.773902 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.499978 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.499908 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.777858 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.500023 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.781886 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.783897 Flask-AppBuilder-4.3.3rc2/examples/productsale/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/productsale/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.789946 Flask-AppBuilder-4.3.3rc2/examples/quickactions/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.795797 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.500464 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.500387 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.800911 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.500512 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.808446 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.812165 Flask-AppBuilder-4.3.3rc2/examples/quickactions/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickactions/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.819441 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.834156 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1685 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/data.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.500842 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.500887 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.841491 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.852445 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.859672 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.870666 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.501225 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.501277 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.878198 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5073 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.889250 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/babel/messages.pot~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.501633 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.501515 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.501563 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.900138 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.501679 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.911192 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.924398 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.945728 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.952943 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.502007 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.974671 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.502114 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.996348 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.010635 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickfiles/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.039615 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.061214 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.502424 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.502471 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.075397 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2022-08-16 10:09:18.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.096468 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-05-24 14:03:04.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.125173 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.179627 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/sec_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.503005 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.182736 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abDate.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abSelect.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.183254 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/css/clean-blog.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/css/scrolling-nav.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.183744 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/img/brand.jpg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/img/loading.gif
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.184907 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.185560 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Controllers/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.186001 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Directives/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.186230 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Services/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Services/apiService.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/angular.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/app.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/clean-blog.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/scrolling-nav.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.188011 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.188271 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/list_angulajs.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/list_contacts.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/list_json.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/mylist.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/new_base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/show_contacts.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.188742 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/widgets/list_override.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.503571 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.503620 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.189273 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.190042 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.192499 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/.coverage
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.193145 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.503950 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.503996 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.193561 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.194186 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/migrate_db_0.7.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.194641 Flask-AppBuilder-4.3.3rc2/examples/quickimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.195370 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.504459 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.504389 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.195817 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.504503 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.196303 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.196561 Flask-AppBuilder-4.3.3rc2/examples/quickimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickimages/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.197778 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.200779 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.504847 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.504898 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.201227 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.201628 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.201835 Flask-AppBuilder-4.3.3rc2/examples/quickminimal/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quickminimal/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.203271 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.204226 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/encodings.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/misc.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/modules.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/quicksqlviews.iml
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/workspace.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.204798 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.505416 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.505470 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.205297 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.205678 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.206949 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.207528 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.505797 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.207732 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/static/css/landing-page.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.207933 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/templates/mybase.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.505992 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.506036 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.208336 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.208934 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.210460 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.211306 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.216242 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/.babelrc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/README.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/package-lock.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/package.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/package.json.react-original
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.216855 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/public/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/public/favicon.ico
--rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/public/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/public/manifest.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.219578 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/App.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.219797 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/api/Api.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.220575 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/Forms.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/Table.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/index.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/webpack.config.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.221102 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/templates/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/templates/react.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.506794 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.506843 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.223823 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.224256 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.225503 Flask-AppBuilder-4.3.3rc2/examples/related_fields/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.226021 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.507192 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.507245 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.226506 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.226872 Flask-AppBuilder-4.3.3rc2/examples/related_fields/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/related_fields/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.227582 Flask-AppBuilder-4.3.3rc2/examples/simpleform/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.228212 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/forms.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.228395 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/templates/404.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.507665 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.507715 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.228767 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.229407 Flask-AppBuilder-4.3.3rc2/examples/simpleform/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleform/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.239415 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.239774 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.240141 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview1/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.245297 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.245718 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.245912 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/app/templates/method3.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.246286 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/simpleview2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.250191 Flask-AppBuilder-4.3.3rc2/examples/user_registration/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.250819 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.508855 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.508912 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.251350 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3981 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.251913 Flask-AppBuilder-4.3.3rc2/examples/user_registration/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/user_registration/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.252990 Flask-AppBuilder-4.3.3rc2/examples/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.253503 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.509292 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.509339 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.253835 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.254323 Flask-AppBuilder-4.3.3rc2/examples/widgets/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/examples/widgets/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.263060 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2023-06-21 12:38:12.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/_compat.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/actions.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.264260 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    75988 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/convert.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.264758 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/babel/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2311 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/babel/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/babel/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26094 2023-06-19 15:06:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/basemanager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48877 2023-05-08 11:18:50.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/baseviews.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.265413 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/jsontools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/widgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/console.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8459 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/const.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/exceptions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/fieldwidgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/filemanager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11138 2023-02-15 14:55:26.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/hooks.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/messages.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.266495 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10375 2022-12-22 10:35:46.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/filters.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.267062 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/interface.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10979 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/group.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mixins.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.267833 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10027 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.268512 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2022-10-27 13:02:57.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39175 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.271557 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10693 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    77462 2023-06-19 07:52:15.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/manager.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.272264 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15641 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/mongoengine/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/mongoengine/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10650 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/registerviews.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.272971 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.273289 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.273859 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.274297 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.274854 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/role/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/role/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/role/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/role/schema.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.275623 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/schema.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/validator.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.276010 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    27043 2022-11-09 14:23:15.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/manager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2022-10-27 13:02:57.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/utils.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25771 2023-03-16 10:28:12.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.510810 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.511592 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.276439 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/ab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.279352 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.280707 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.293620 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/united.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.294120 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/datepicker/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.295688 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.297296 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/aol.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/fab.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.297520 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/flags/flags16.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/flickr.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/google.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/myopenid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/yahoo.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.301466 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3321 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4834 2023-05-12 13:46:20.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117065 2023-01-10 15:35:16.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/fontawesome.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/google_charts.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.305897 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2x2.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.310772 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.511716 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.313091 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/_formhelpers.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/baselayout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/baselib.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/flash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/footer.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.313522 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/alert.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.318744 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/confirm.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13876 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/lib.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.320343 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/add.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      779 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      417 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.321936 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/activation.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1388 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      754 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/resetpassword.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.329687 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1091 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2908 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2541 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1559 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.330040 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1080 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2773 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/init.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/navbar.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1581 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/navbar_right.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.330229 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/swagger/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.344165 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.344732 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.345216 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1882 2023-02-23 14:02:46.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/__pycache__/test_0_fixture.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/addon_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1372 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/A_fixture/test_0_fixture.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.353175 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      174 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5453 2022-07-29 12:58:36.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2023-03-16 10:39:04.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/config_api.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      993 2023-05-08 12:37:37.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/config_oauth.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      629 2023-05-03 11:58:50.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/config_security.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      443 2023-02-23 14:03:19.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/const.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    84101 2023-06-21 10:49:06.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/test_api.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7970 2023-05-03 12:02:06.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/test_fab_cli.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52394 2023-06-21 11:42:44.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/test_mvc.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4712 2023-05-08 12:38:18.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/__pycache__/test_mvc_oauth.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)   229376 2023-06-21 10:43:13.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/app.db
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4453 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/config_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/config_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/config_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/config_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/const.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.353403 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/data/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/data/roles.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.353759 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/mongoengine/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.360267 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.361394 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      183 2023-02-23 14:04:47.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19332 2023-05-08 10:31:28.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/__pycache__/test_auth_ldap.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12669 2023-05-19 13:54:28.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/__pycache__/test_mvc_security.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2023-02-23 14:57:17.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/__pycache__/test_rate_limiter.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    34243 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_auth_ldap.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_auth_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_base_security_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18130 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_mvc_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_password_complexity.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2962 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_rate_limiter.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.361744 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.362209 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/sqla/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/sqla/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9786 2023-06-21 10:48:48.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/sqla/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10003 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/sqla/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.362430 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       29 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/templates/custom_index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1335 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_addon.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121914 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1245 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_custom_indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8776 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_fab_cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6503 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24066 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_mongoengine.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    68528 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_mvc.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5050 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_mvc_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    44396 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6056 2022-11-09 14:23:15.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_security_permissions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_sqlalchemy.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2540 2022-08-17 09:07:58.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.362674 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.521651 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/de/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.367649 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/de/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.522832 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/el/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.368254 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/el/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.523965 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.368590 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.524991 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/fr/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.368943 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/fr/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.525951 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/it/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.369276 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/it/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.526871 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ja_JP/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.369894 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.527762 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ko/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.370219 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ko/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.528642 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/nl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.375262 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/nl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.529572 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.375706 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.530554 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.376375 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.531522 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt_BR/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.376715 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.532460 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ru/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.377435 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ru/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.533389 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/sl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.378067 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/sl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.534308 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.378512 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:13.535239 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh_HK/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.378908 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/upload.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2022-08-17 09:07:58.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.379497 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/utils/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/utils/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/utils/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/utils/limit.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/validators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/flask_appbuilder/widgets.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.387182 Flask-AppBuilder-4.3.3rc2/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/login_oauth.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/images/simpleview2.png
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/release.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.3rc2/requirements-dev.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.3rc2/requirements-extra.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2905 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.3rc2/requirements.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.3rc2/rtd_requirements.txt
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-06-21 12:40:14.387573 Flask-AppBuilder-4.3.3rc2/scripts/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/scripts/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/scripts/babel_init.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2023-06-21 12:40:14.395144 Flask-AppBuilder-4.3.3rc2/setup.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2795 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.3rc2/setup.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.3rc2/tox.ini
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

### Comparing `Flask-AppBuilder-4.3.3rc2/.github/ISSUE_TEMPLATE.md` & `Flask-AppBuilder-4.3.4rc1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/.github/PULL_REQUEST_TEMPLATE.md` & `Flask-AppBuilder-4.3.4rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/.github/stale.yml` & `Flask-AppBuilder-4.3.4rc1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/.github/workflows/ci.yml` & `Flask-AppBuilder-4.3.4rc1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
           pip install -r requirements-dev.txt
       - name: black
         run: black --check setup.py flask_appbuilder
       - name: flake8
         run: flake8 flask_appbuilder
       - name: mypy
         run: mypy flask_appbuilder
+      - name: black
+        run: black --check tests
+      - name: flake8
+        run: flake8 tests
 
   test-postgres:
     runs-on: ubuntu-22.04
     strategy:
       matrix:
         python-version: ["3.7", "3.8", "3.9"]
     env:
@@ -75,15 +79,15 @@
           sudo apt-get install -y libldap2-dev libsasl2-dev libssl-dev
           pip install --upgrade pip
           pip install -r requirements.txt
           pip install -r requirements-dev.txt
           pip install -r requirements-extra.txt
       - name: Run tests
         run: |
-          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder flask_appbuilder.tests --ignore-files="test_mongoengine\.py"
+          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder tests --ignore-files="test_mongoengine\.py"
       - name: Upload code coverage
         run: |
           bash <(curl -s https://codecov.io/bash) -cF python
 
   test-mysql:
     runs-on: ubuntu-22.04
     strategy:
@@ -126,15 +130,15 @@
           sudo apt-get install -y libldap2-dev libsasl2-dev libssl-dev
           pip install --upgrade pip
           pip install -r requirements.txt
           pip install -r requirements-dev.txt
           pip install -r requirements-extra.txt
       - name: Run tests
         run: |
-          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder flask_appbuilder.tests --ignore-files="test_mongoengine\.py"
+          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder tests --ignore-files="test_mongoengine\.py"
       - name: Upload code coverage
         run: |
           bash <(curl -s https://codecov.io/bash) -cF python
 
   test-mssql:
     runs-on: ubuntu-22.04
     strategy:
@@ -176,15 +180,15 @@
           pip install --upgrade pip
           pip install -r requirements.txt
           pip install -r requirements-dev.txt
           pip install -r requirements-extra.txt
           sudo cp .github/workflows/odbcinst.ini /etc/odbcinst.ini
       - name: Run tests
         run: |
-          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder flask_appbuilder.tests --ignore-files="test_mongoengine\.py"
+          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder tests --ignore-files="test_mongoengine\.py"
       - name: Upload code coverage
         run: |
           bash <(curl -s https://codecov.io/bash) -cF python
 
   test-mongodb:
     runs-on: ubuntu-22.04
     strategy:
@@ -220,11 +224,11 @@
           pip install --upgrade pip
           pip install -r requirements.txt
           pip install -r requirements-dev.txt
           pip install -r requirements-extra.txt
           pip install -r requirements-mongodb.txt
       - name: Run tests
         run: |
-          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder flask_appbuilder/tests/test_mongoengine.py
+          nosetests --stop -v --with-coverage --cover-package=flask_appbuilder tests/test_mongoengine.py
       - name: Upload code coverage
         run: |
           bash <(curl -s https://codecov.io/bash) -cF python
```

### Comparing `Flask-AppBuilder-4.3.3rc2/.github/workflows/ptlint.yml` & `Flask-AppBuilder-4.3.4rc1/.github/workflows/ptlint.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/CHANGELOG.rst` & `Flask-AppBuilder-4.3.4rc1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Flask-AppBuilder ChangeLog
 ==========================
 
+Improvements and Bug fixes on 4.3.4
+-----------------------------------
+
+- fix: select filters spacing, theme and operation select (#2079) [Daniel Vaz Gaspar]
+- refactor: Refactored logging functions to consistently use lazy interpolation (#2071) [Bruce]
+- feat: add optional flask-talisman and use csp nonce on scripts (#2075) [Daniel Vaz Gaspar]
+- chore: improve tests and test data load (#2072) [Daniel Vaz Gaspar]
+
 Improvements and Bug fixes on 4.3.3
 -----------------------------------
 
 - fix: marshmallow enum by value keep compatibility (#2067) [Daniel Vaz Gaspar]
 - fix: marshmallow new min version to 3.18 (#2066) [Daniel Vaz Gaspar]
 - fix: select2-ajax-widget (#2052) [Nadir Can Kavkas]
 - chore: remove marshmallow-enum dependency (#2064) [Daniel Vaz Gaspar]
```

### Comparing `Flask-AppBuilder-4.3.3rc2/CONTRIBUTING.rst` & `Flask-AppBuilder-4.3.4rc1/CONTRIBUTING.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     $ docker-compose up -d
 
 2 - Run Postgres tests
 
 .. code-block:: bash
 
-    $ nosetests flask_appbuilder.tests
+    $ nosetests -v
 
 You can also use tox
 
 .. code-block:: bash
 
     $ tox -e postgres
 
@@ -61,30 +61,24 @@
 
 2 - Export the connection string
 
 .. code-block:: bash
 
    $ export SQLALCHEMY_DATABASE_URI=postgresql+psycopg2://pguser:pguserpassword@0.0.0.0/app
 
-3 - Run the fixtures
+4 - To run a single test
 
 .. code-block:: bash
 
-    $ nosetests -v flask_appbuilder.tests.A_fixture
-
-4 - Run a single test
-
-.. code-block:: bash
-
-    $ nosetests -v flask_appbuilder.tests.test_api:APITestCase.test_get_item_dotted_mo_notation
+    $ nosetests -v tests.test_api:APITestCase.test_get_item_dotted_mo_notation
 
 .. note::
 
-    If your using SQLite3, the location of the db is: ./flask_appbuilder/tests/app.db
-    You can safely delete it, if you need to delete the fixtures for example.
+    If your using SQLite3, the location of the db is: ./tests/app.db
+    You can safely delete it, if you need to delete test data for example.
 
 
 Responsible disclosure of Security Vulnerabilities
 --------------------------------------------------
 
 We want to keep Flask-AppBuilder safe for everyone. If you've discovered a security vulnerability
 please report to danielvazgaspar@gmail.com.
```

### Comparing `Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/PKG-INFO` & `Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.3rc2
+Version: 4.3.4rc1
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
@@ -209,7 +209,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: jmespath
 Provides-Extra: oauth
 Provides-Extra: openid
+Provides-Extra: talisman
```

### Comparing `Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/SOURCES.txt` & `Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -701,15 +701,14 @@
 flask_appbuilder/static/appbuilder/img/yahoo.png
 flask_appbuilder/static/appbuilder/img/flags/flags16.png
 flask_appbuilder/static/appbuilder/js/ab.js
 flask_appbuilder/static/appbuilder/js/ab_actions.js
 flask_appbuilder/static/appbuilder/js/ab_filters.js
 flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
 flask_appbuilder/static/appbuilder/js/bootstrap.min.js
-flask_appbuilder/static/appbuilder/js/fontawesome.js
 flask_appbuilder/static/appbuilder/js/google_charts.js
 flask_appbuilder/static/appbuilder/js/jquery-latest.js
 flask_appbuilder/static/appbuilder/js/v4-shims.min.js
 flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
 flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
 flask_appbuilder/static/appbuilder/select2/select2.css
 flask_appbuilder/static/appbuilder/select2/select2.js
@@ -752,15 +751,14 @@
 flask_appbuilder/templates/appbuilder/general/security/activation.html
 flask_appbuilder/templates/appbuilder/general/security/login_db.html
 flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
 flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
 flask_appbuilder/templates/appbuilder/general/security/login_oid.html
 flask_appbuilder/templates/appbuilder/general/security/register_mail.html
 flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
-flask_appbuilder/templates/appbuilder/general/security/resetpassword.html
 flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
 flask_appbuilder/templates/appbuilder/general/widgets/chart.html
 flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
 flask_appbuilder/templates/appbuilder/general/widgets/form.html
 flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
 flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
 flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
@@ -776,69 +774,16 @@
 flask_appbuilder/templates/appbuilder/general/widgets/search.html
 flask_appbuilder/templates/appbuilder/general/widgets/show.html
 flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
 flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
 flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
 flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
 flask_appbuilder/templates/appbuilder/swagger/swagger.html
-flask_appbuilder/tests/__init__.py
-flask_appbuilder/tests/app.db
-flask_appbuilder/tests/base.py
-flask_appbuilder/tests/config_api.py
-flask_appbuilder/tests/config_oauth.py
-flask_appbuilder/tests/config_security.py
-flask_appbuilder/tests/config_security_api.py
-flask_appbuilder/tests/const.py
-flask_appbuilder/tests/test_addon.py
-flask_appbuilder/tests/test_api.py
-flask_appbuilder/tests/test_custom_indexview.py
-flask_appbuilder/tests/test_fab_cli.py
-flask_appbuilder/tests/test_menu.py
-flask_appbuilder/tests/test_mongoengine.py
-flask_appbuilder/tests/test_mvc.py
-flask_appbuilder/tests/test_mvc_oauth.py
-flask_appbuilder/tests/test_security_api.py
-flask_appbuilder/tests/test_security_permissions.py
-flask_appbuilder/tests/test_sqlalchemy.py
-flask_appbuilder/tests/test_urltools.py
-flask_appbuilder/tests/A_fixture/__init__.py
-flask_appbuilder/tests/A_fixture/addon_manager.py
-flask_appbuilder/tests/A_fixture/test_0_fixture.py
-flask_appbuilder/tests/A_fixture/__pycache__/__init__.cpython-38.pyc
-flask_appbuilder/tests/A_fixture/__pycache__/test_0_fixture.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/__init__.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/base.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/config_api.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/config_oauth.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/config_security.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/const.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/test_api.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/test_fab_cli.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/test_mvc.cpython-38.pyc
-flask_appbuilder/tests/__pycache__/test_mvc_oauth.cpython-38.pyc
-flask_appbuilder/tests/data/roles.json
-flask_appbuilder/tests/mongoengine/__init__.py
-flask_appbuilder/tests/mongoengine/models.py
-flask_appbuilder/tests/security/__init__.py
-flask_appbuilder/tests/security/test_auth_ldap.py
-flask_appbuilder/tests/security/test_auth_oauth.py
-flask_appbuilder/tests/security/test_base_security_manager.py
-flask_appbuilder/tests/security/test_mvc_security.py
-flask_appbuilder/tests/security/test_password_complexity.py
-flask_appbuilder/tests/security/test_rate_limiter.py
-flask_appbuilder/tests/security/__pycache__/__init__.cpython-38.pyc
-flask_appbuilder/tests/security/__pycache__/test_auth_ldap.cpython-38.pyc
-flask_appbuilder/tests/security/__pycache__/test_mvc_security.cpython-38.pyc
-flask_appbuilder/tests/security/__pycache__/test_rate_limiter.cpython-38.pyc
-flask_appbuilder/tests/sqla/__init__.py
-flask_appbuilder/tests/sqla/models.py
-flask_appbuilder/tests/sqla/__pycache__/__init__.cpython-38.pyc
-flask_appbuilder/tests/sqla/__pycache__/models.cpython-38.pyc
-flask_appbuilder/tests/templates/custom_index.html
 flask_appbuilder/translations/__init__.py
+flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
 flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
 flask_appbuilder/translations/de/LC_MESSAGES/messages.po
 flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
 flask_appbuilder/translations/el/LC_MESSAGES/messages.po
 flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
 flask_appbuilder/translations/es/LC_MESSAGES/messages.po
 flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
@@ -889,8 +834,42 @@
 images/login.png
 images/login_db.png
 images/login_oauth.png
 images/login_oid.png
 images/security.png
 images/simpleview2.png
 scripts/babel_extract.sh
-scripts/babel_init.sh
+scripts/babel_init.sh
+tests/__init__.py
+tests/base.py
+tests/config_api.py
+tests/config_oauth.py
+tests/config_security.py
+tests/config_security_api.py
+tests/const.py
+tests/test_addon.py
+tests/test_api.py
+tests/test_custom_indexview.py
+tests/test_fab_cli.py
+tests/test_menu.py
+tests/test_mongoengine.py
+tests/test_mvc.py
+tests/test_mvc_oauth.py
+tests/test_security_api.py
+tests/test_security_permissions.py
+tests/test_sqlalchemy.py
+tests/test_urltools.py
+tests/fixtures/__init__.py
+tests/fixtures/addon_manager.py
+tests/fixtures/data_models.py
+tests/fixtures/users.py
+tests/mongoengine/__init__.py
+tests/mongoengine/models.py
+tests/security/__init__.py
+tests/security/test_auth_ldap.py
+tests/security/test_auth_oauth.py
+tests/security/test_base_security_manager.py
+tests/security/test_mvc_security.py
+tests/security/test_password_complexity.py
+tests/security/test_rate_limiter.py
+tests/sqla/__init__.py
+tests/sqla/models.py
```

### Comparing `Flask-AppBuilder-4.3.3rc2/Flask_AppBuilder.egg-info/requires.txt` & `Flask-AppBuilder-4.3.4rc1/Flask_AppBuilder.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,7 +23,10 @@
 jmespath>=0.9.5
 
 [oauth]
 Authlib<2.0.0,>=0.14
 
 [openid]
 Flask-OpenID<2,>=1.2.5
+
+[talisman]
+flask-talisman<2.0,>=1.0.0
```

### Comparing `Flask-AppBuilder-4.3.3rc2/LICENSE` & `Flask-AppBuilder-4.3.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/PKG-INFO` & `Flask-AppBuilder-4.3.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.3rc2
+Version: 4.3.4rc1
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
@@ -209,7 +209,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: jmespath
 Provides-Extra: oauth
 Provides-Extra: openid
+Provides-Extra: talisman
```

### Comparing `Flask-AppBuilder-4.3.3rc2/README.rst` & `Flask-AppBuilder-4.3.4rc1/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/bin/config.py` & `Flask-AppBuilder-4.3.4rc1/bin/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/bin/db_migrate.py` & `Flask-AppBuilder-4.3.4rc1/bin/db_migrate.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/bin/hash_db_password.py` & `Flask-AppBuilder-4.3.4rc1/bin/hash_db_password.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/bin/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.4rc1/bin/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/bin/migrate_db_1.3.py` & `Flask-AppBuilder-4.3.4rc1/bin/migrate_db_1.3.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/bin/sqlite_upgrade_1.3.sql` & `Flask-AppBuilder-4.3.4rc1/bin/sqlite_upgrade_1.3.sql`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docker-compose.yml` & `Flask-AppBuilder-4.3.4rc1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/Makefile` & `Flask-AppBuilder-4.3.4rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.4rc1/docs/_static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_templates/layout.html` & `Flask-AppBuilder-4.3.4rc1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/LICENSE` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/README` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/layout.html` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/relations.html` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask/static/flasky.css_t` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/layout.html` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_small/static/flasky.css_t` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/_themes/flask_theme_support.py` & `Flask-AppBuilder-4.3.4rc1/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/actions.rst` & `Flask-AppBuilder-4.3.4rc1/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/addons.rst` & `Flask-AppBuilder-4.3.4rc1/docs/addons.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/advanced.rst` & `Flask-AppBuilder-4.3.4rc1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/api.rst` & `Flask-AppBuilder-4.3.4rc1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/cli.rst` & `Flask-AppBuilder-4.3.4rc1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/conf.py` & `Flask-AppBuilder-4.3.4rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/config.rst` & `Flask-AppBuilder-4.3.4rc1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/customizing.rst` & `Flask-AppBuilder-4.3.4rc1/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/diagrams.rst` & `Flask-AppBuilder-4.3.4rc1/docs/diagrams.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/generic_datasource.rst` & `Flask-AppBuilder-4.3.4rc1/docs/generic_datasource.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/i18n.rst` & `Flask-AppBuilder-4.3.4rc1/docs/i18n.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/chart.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/chart_time1.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/chart_time2.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/charts.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/contact_list.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/contacts.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/direct_chart.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/fab.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/group_list.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/grouped_chart.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/groups.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/images_list.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/list_cascade.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/list_master_detail.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/login.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/login_db.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/login_oid.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/oauth_login.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/oauth_login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/oauth_login_one_provider.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/oauth_login_one_provider.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/security.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/simpleview2.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/swagger001.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/swagger001.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/images/swagger002.png` & `Flask-AppBuilder-4.3.4rc1/docs/images/swagger002.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/index.rst` & `Flask-AppBuilder-4.3.4rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/installation.rst` & `Flask-AppBuilder-4.3.4rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/intro.rst` & `Flask-AppBuilder-4.3.4rc1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/make.bat` & `Flask-AppBuilder-4.3.4rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/multipledbs.rst` & `Flask-AppBuilder-4.3.4rc1/docs/multipledbs.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/quickcharts.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickcharts.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/quickfiles.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickfiles.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/quickhowto.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickhowto.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/quickhowto_mongo.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickhowto_mongo.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/quickminimal.rst` & `Flask-AppBuilder-4.3.4rc1/docs/quickminimal.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/relations.rst` & `Flask-AppBuilder-4.3.4rc1/docs/relations.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/rest_api.rst` & `Flask-AppBuilder-4.3.4rc1/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/security.rst` & `Flask-AppBuilder-4.3.4rc1/docs/security.rst`

 * *Files 3% similar despite different names*

```diff
@@ -934,7 +934,27 @@
 
 Now you'll have your extended User model as the authenticated user, *g.user* will have your model with the extra col.
 
 Some images:
 
 .. image:: ./images/security.png
     :width: 100%
+
+Optional dependency Flask-Talisman
+==================================
+
+All javascript code and inline scripts can have a nonce attribute provided by Flask-Talisman.
+This package will not initialize Flask-Talisman for you, but will use `csp_nonce()` on Jinja2 if it exists.
+To initialize Flask-Talisman, you can do the following:
+
+.. code-block:: python
+
+    from flask import Flask
+    from flask_appbuilder import AppBuilder
+    from flask_talisman import Talisman
+
+    app = Flask(__name__)
+    app.config.from_object('config')
+    db = SQLA(app)
+    appbuilder = AppBuilder(app, db.session)
+
+    Talisman(app)
```

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/templates.rst` & `Flask-AppBuilder-4.3.4rc1/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/user_registration.rst` & `Flask-AppBuilder-4.3.4rc1/docs/user_registration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/versionmigration.rst` & `Flask-AppBuilder-4.3.4rc1/docs/versionmigration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/docs/views.rst` & `Flask-AppBuilder-4.3.4rc1/docs/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/base_api/app/api.py` & `Flask-AppBuilder-4.3.4rc1/examples/base_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/base_api/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/base_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/basefilter/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/basefilter/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/composite_keys/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/composite_keys/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/composite_keys/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/composite_keys/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/composite_keys/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/api.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/crud_rest_api/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/crud_rest_api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/Dash_App1.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_App1.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/Dash_App2.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_App2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/dash/app/Dashboard/Dash_fun.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/Dashboard/Dash_fun.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/dash/app/templates/dash.html` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/templates/dash.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/dash/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/dash/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/dash/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/employees/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/employees/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/employees/app/security.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/employees/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/employees/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/employees/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/enums/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/enums/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/enums/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/enums/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/sec_forms.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/sec_views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/sec_forms.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/sec_views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/extendsecurity2/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/extendsecurity2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/config2.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/config2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/factoryapp/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/factoryapp/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/issue_789/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/issue_789/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/issue_789/app.py` & `Flask-AppBuilder-4.3.4rc1/examples/issue_789/app.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/masterdetail/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/masterdetail/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/mysecurity.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/mysecurity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongo_extendedsecurity/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongo_extendedsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoengine/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoengine/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/mongoimages/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/mongoimages/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/oauth/README.rst` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/oauth/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/oauth/app/security.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/oauth/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/oauth/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/oauth/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/productsale/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/productsale/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickactions/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickactions/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/data.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     politicals = ["Democratic", "Authorative"]
     for country in countries:
         c = Country(name=country)
         try:
             db.session.add(c)
             db.session.commit()
         except Exception as e:
-            log.error("Update ViewMenu error: {0}".format(str(e)))
+            log.error("Update ViewMenu error: %s", e)
             db.session.rollback()
     for political in politicals:
         c = PoliticalType(name=political)
         try:
             db.session.add(c)
             db.session.commit()
         except Exception as e:
-            log.error("Update ViewMenu error: {0}".format(str(e)))
+            log.error("Update ViewMenu error: %s", e)
             db.session.rollback()
     try:
         for x in range(1, 20):
             cs = CountryStats()
             cs.population = random.randint(1, 100)
             cs.unemployed = random.randint(1, 100)
             cs.college = random.randint(1, 100)
@@ -47,9 +47,9 @@
             day = random.choice(range(1, 28))
             cs.stat_date = datetime.datetime(year, month, day)
             cs.country_id = random.randint(1, len(countries))
             cs.political_type_id = random.randint(1, len(politicals))
             db.session.add(cs)
             db.session.commit()
     except Exception as e:
-        log.error("Update ViewMenu error: {0}".format(str(e)))
+        log.error("Update ViewMenu error: %s", e)
         db.session.rollback()
```

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/app/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     politicals = ["Democratic", "Authorative"]
     for country in countries:
         c = Country(name=country)
         try:
             db.session.add(c)
             db.session.commit()
         except Exception as e:
-            log.error("Update ViewMenu error: {0}".format(str(e)))
+            log.error("Update ViewMenu error: %s", e)
             db.session.rollback()
     for political in politicals:
         c = PoliticalType(name=political)
         try:
             db.session.add(c)
             db.session.commit()
         except Exception as e:
-            log.error("Update ViewMenu error: {0}".format(str(e)))
+            log.error("Update ViewMenu error: %s", e)
             db.session.rollback()
     try:
         for x in range(1, 20):
             cs = CountryStats()
             cs.population = random.randint(1, 100)
             cs.unemployed = random.randint(1, 100)
             cs.college = random.randint(1, 100)
@@ -57,15 +57,15 @@
             day = random.choice(range(1, 28))
             cs.stat_date = datetime.datetime(year, month, day)
             cs.country_id = random.randint(1, len(countries))
             cs.political_type_id = random.randint(1, len(politicals))
             db.session.add(cs)
             db.session.commit()
     except Exception as e:
-        log.error("Update ViewMenu error: {0}".format(str(e)))
+        log.error("Update ViewMenu error: %s", e)
         db.session.rollback()
 
 
 class CountryStatsModelView(ModelView):
     datamodel = SQLAModel(CountryStats)
     list_columns = ["country", "stat_date", "population", "unemployed", "college"]
```

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/build/lib/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/build/lib/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickcharts2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickcharts2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickfiles/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickfiles/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/forms.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/sec_views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/css/clean-blog.min.css` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/clean-blog.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/css/scrolling-nav.css` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/css/scrolling-nav.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/img/brand.jpg` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/brand.jpg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/img/loading.gif` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/Services/apiService.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/Services/apiService.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/angular.min.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/angular.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/app.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/app.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/clean-blog.min.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/clean-blog.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/static/js/scrolling-nav.js` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/static/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/list_angulajs.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_angulajs.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/list_json.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/list_json.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/templates/widgets/list.html` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/templates/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto2/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/.coverage` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/.coverage`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickhowto3/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickhowto3/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/__init__.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickimages/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quickmigrate/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quickmigrate/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/misc.xml` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/.idea/workspace.xml` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicksqlviews/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicksqlviews/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/static/css/landing-page.css` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/static/css/landing-page.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/templates/mybase.html` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/templates/mybase.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/quicktemplates/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/quicktemplates/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/api.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/package-lock.json` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/package.json` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/package.json.react-original` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/package.json.react-original`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/public/favicon.ico` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/api/Api.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/api/Api.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/Forms.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/Forms.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/static/src/components/Table.js` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/static/src/components/Table.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/templates/base.html` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/react-rest-api/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/react-rest-api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/related_fields/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/related_fields/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleform/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleform/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleform/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleform/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleview1/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview1/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleview1/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview1/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleview2/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/simpleview2/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/simpleview2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/app/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,9 +143,9 @@
 appbuilder.add_view(
     ContactTimeChartView,
     "Contacts Birth Chart",
     icon="fa-dashboard",
     category="Contacts",
 )
 
-log.info("F.A.B. Version: {0}".format(appbuilder.version))
-log.info("User extension class {0}".format(UserExtensionMixin.__subclasses__()[0]))
+log.info("F.A.B. Version: %s", appbuilder.version)
+log.info("User extension class %s", UserExtensionMixin.__subclasses__()[0])
```

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/user_registration/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/user_registration/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/NAMES.DIC` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/app/models.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/app/views.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/babel/messages.pot` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/babel/messages.pot~` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/config.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/examples/widgets/testdata.py` & `Flask-AppBuilder-4.3.4rc1/examples/widgets/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Daniel Vaz Gaspar"
-__version__ = "4.3.3rc2"
+__version__ = "4.3.4rc1"
 
 from .actions import action  # noqa: F401
 from .api import ModelRestApi  # noqa: F401
 from .base import AppBuilder  # noqa: F401
 from .baseviews import BaseView, expose  # noqa: F401
 from .charts.views import DirectByChartView, GroupByChartView  # noqa: F401
 from .models.group import aggregate_avg, aggregate_count, aggregate_sum  # noqa: F401
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/_compat.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/actions.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/actions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,15 +562,15 @@
                     # If include_route_methods is not None white list
                     if (
                         self.include_route_methods is not None
                         and attr_name not in self.include_route_methods
                     ):
                         continue
                     if attr_name in self.exclude_route_methods:
-                        log.info(f"Not registering api spec for method {attr_name}")
+                        log.info("Not registering api spec for method %s", attr_name)
                         continue
                     operations = {}
                     path = self.path_helper(path=url, operations=operations)
                     self.operation_helper(
                         path=path, operations=operations, methods=methods, func=attr
                     )
                     api_spec.path(path=path, operations=operations)
@@ -608,21 +608,24 @@
         for attr_name in dir(self):
             if (
                 self.include_route_methods is not None
                 and attr_name not in self.include_route_methods
             ):
                 continue
             if attr_name in self.exclude_route_methods:
-                log.info(f"Not registering route for method {attr_name}")
+                log.info("Not registering route for method %s", attr_name)
                 continue
             attr = getattr(self, attr_name)
             if hasattr(attr, "_urls"):
                 for url, methods in attr._urls:
                     log.info(
-                        f"Registering route {self.blueprint.url_prefix}{url} {methods}"
+                        "Registering route %s%s %s",
+                        self.blueprint.url_prefix,
+                        url,
+                        methods,
                     )
                     route_handler = wrap_route_handler_with_hooks(
                         attr_name, attr, before_request_hooks
                     )
                     self.blueprint.add_url_rule(
                         url, attr_name, route_handler, methods=methods
                     )
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/convert.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/convert.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/api/schemas.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/api/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/babel/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/babel/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/base.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     try:
         tmp = class_path.split(".")
         module_path = ".".join(tmp[0:-1])
         package = __import__(module_path)
         return reduce(getattr, tmp[1:], package)
     except Exception as e:
         log.exception(e)
-        log.error(LOGMSG_ERR_FAB_ADDON_IMPORT.format(class_path, e))
+        log.error(LOGMSG_ERR_FAB_ADDON_IMPORT, class_path, e)
         return None
 
 
 class AppBuilder:
     """
     This is the base class for all the framework.
     This is where you will register all your views and create the menu structure.
@@ -337,18 +337,18 @@
                 # Instantiate manager with appbuilder (self)
                 inst_addon_class: "BaseManager" = addon_class(self)
                 try:
                     inst_addon_class.pre_process()
                     inst_addon_class.register_views()
                     inst_addon_class.post_process()
                     self.addon_managers[addon] = inst_addon_class
-                    log.info(LOGMSG_INF_FAB_ADDON_ADDED.format(str(addon)))
+                    log.info(LOGMSG_INF_FAB_ADDON_ADDED, addon)
                 except Exception as e:
                     log.exception(e)
-                    log.error(LOGMSG_ERR_FAB_ADDON_PROCESS.format(addon, e))
+                    log.error(LOGMSG_ERR_FAB_ADDON_PROCESS, addon, e)
 
     def _check_and_init(
         self, baseview: Union[Type["AbstractViewApi"], "AbstractViewApi"]
     ) -> "AbstractViewApi":
         # If class if not instantiated, instantiate it
         # and add db session from security models.
         if hasattr(baseview, "datamodel"):
@@ -434,15 +434,15 @@
                 label=_('Your Feature'),
                 menu_cond=lambda: is_feature_enabled("your-feature"),
             )
             # Add a link
             appbuilder.add_link("google", href="www.google.com", icon = "fa-google-plus")
         """
         baseview = self._check_and_init(baseview)
-        log.info(LOGMSG_INF_FAB_ADD_VIEW.format(baseview.__class__.__name__, name))
+        log.info(LOGMSG_INF_FAB_ADD_VIEW, baseview.__class__.__name__, name)
 
         if not self._view_exists(baseview):
             baseview.appbuilder = self
             self.baseviews.append(baseview)
             self._process_inner_views()
             if self.app:
                 self.register_blueprint(baseview)
@@ -551,28 +551,28 @@
         :param baseview:
             A BaseView type class instantiated.
         :param endpoint: The endpoint path for the Flask blueprint
         :param static_folder: The static folder for the Flask blueprint
 
         """
         baseview = self._check_and_init(baseview)
-        log.info(LOGMSG_INF_FAB_ADD_VIEW.format(baseview.__class__.__name__, ""))
+        log.info(LOGMSG_INF_FAB_ADD_VIEW, baseview.__class__.__name__, "")
 
         if not self._view_exists(baseview):
             baseview.appbuilder = self
             self.baseviews.append(baseview)
             self._process_inner_views()
             if self.app:
                 self.register_blueprint(
                     baseview, endpoint=endpoint, static_folder=static_folder
                 )
                 self._add_permission(baseview)
                 self.add_limits(baseview)
         else:
-            log.warning(LOGMSG_WAR_FAB_VIEW_EXISTS.format(baseview.__class__.__name__))
+            log.warning(LOGMSG_WAR_FAB_VIEW_EXISTS, baseview.__class__.__name__)
         return baseview
 
     def add_api(self, baseview: Type["AbstractViewApi"]) -> "AbstractViewApi":
         """
         Add a BaseApi class or child to AppBuilder
 
         :param baseview: A BaseApi type class
@@ -671,23 +671,23 @@
         if self.update_perms or update_perms:
             try:
                 self.sm.add_permissions_view(
                     baseview.base_permissions, baseview.class_permission_name
                 )
             except Exception as e:
                 log.exception(e)
-                log.error(LOGMSG_ERR_FAB_ADD_PERMISSION_VIEW.format(str(e)))
+                log.error(LOGMSG_ERR_FAB_ADD_PERMISSION_VIEW, e)
 
     def _add_permissions_menu(self, name: str, update_perms: bool = False) -> None:
         if self.update_perms or update_perms:
             try:
                 self.sm.add_permissions_menu(name)
             except Exception as e:
                 log.exception(e)
-                log.error(LOGMSG_ERR_FAB_ADD_PERMISSION_MENU.format(str(e)))
+                log.error(LOGMSG_ERR_FAB_ADD_PERMISSION_MENU, e)
 
     def _add_menu_permissions(self, update_perms: bool = False) -> None:
         if self.menu is None:
             return
         if self.update_perms or update_perms:
             for category in self.menu.get_list():
                 self._add_permissions_menu(category.name, update_perms=update_perms)
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/baseviews.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/baseviews.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,23 +305,27 @@
             if (
                 self.include_route_methods is not None
                 and attr_name not in self.include_route_methods
             ):
                 continue
             if attr_name in self.exclude_route_methods:
                 log.info(
-                    f"Not registering route for method "
-                    f"{self.__class__.__name__}.{attr_name}"
+                    "Not registering route for method %s.%s",
+                    self.__class__.__name__,
+                    attr_name,
                 )
                 continue
             attr = getattr(self, attr_name)
             if hasattr(attr, "_urls"):
                 for url, methods in attr._urls:
                     log.info(
-                        f"Registering route {self.blueprint.url_prefix}{url} {methods}"
+                        "Registering route %s%s %s",
+                        self.blueprint.url_prefix,
+                        url,
+                        methods,
                     )
                     route_handler = wrap_route_handler_with_hooks(
                         attr_name, attr, before_request_hooks
                     )
                     self.blueprint.add_url_rule(
                         url, attr_name, route_handler, methods=methods
                     )
@@ -1006,15 +1010,15 @@
                 self.datamodel.get_pk_value(item),
             )
         else:
             if isclass(related_view) and issubclass(related_view, BaseView):
                 name = related_view.__name__
             else:
                 name = related_view.__class__.__name__
-            log.error("Can't find relation on related view {0}".format(name))
+            log.error("Can't find relation on related view %s", name)
             return None
         return related_view._get_view_widget(
             filters=filters,
             order_column=order_column,
             order_direction=order_direction,
             page=page,
             page_size=page_size,
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/jsontools.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/jsontools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/charts/views.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/charts/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/cli.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/console.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/console.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/const.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,119 +13,117 @@
 
         FLAMSG_<SEV>_<MODULE>_<NAME>
             <SEV> :- INF | DEB | WAR | ERR
             <MODULE> :- SEC
 
 """
 
-LOGMSG_ERR_SEC_ACCESS_DENIED = "Access is Denied for: {0} on: {1}"
+LOGMSG_ERR_SEC_ACCESS_DENIED = "Access is Denied for: %s on: %s"
 """ Access denied log message, format with user and view/resource """
-LOGMSG_WAR_SEC_LOGIN_FAILED = "Login Failed for user: {0}"
-LOGMSG_ERR_SEC_CREATE_DB = "DB Creation and initialization failed: {0}"
+LOGMSG_WAR_SEC_LOGIN_FAILED = "Login Failed for user: %s"
+LOGMSG_ERR_SEC_CREATE_DB = "DB Creation and initialization failed: %s"
 """ security models creation fails, format with error message """
-LOGMSG_ERR_SEC_ADD_ROLE = "Add Role: {0}"
+LOGMSG_ERR_SEC_ADD_ROLE = "Add Role: %s"
 """ Error adding role, format with err message """
-LOGMSG_ERR_SEC_ADD_PERMISSION = "Add Permission: {0}"
+LOGMSG_ERR_SEC_ADD_PERMISSION = "Add Permission: %s"
 """ Error adding permission, format with err message """
-LOGMSG_ERR_SEC_ADD_VIEWMENU = "Add View Menu Error: {0}"
+LOGMSG_ERR_SEC_ADD_VIEWMENU = "Add View Menu Error: %s"
 """ Error adding view menu, format with err message """
-LOGMSG_ERR_SEC_DEL_PERMISSION = "Del Permission Error: {0}"
+LOGMSG_ERR_SEC_DEL_PERMISSION = "Del Permission Error: %s"
 """ Error deleting permission, format with err message """
-LOGMSG_ERR_SEC_ADD_PERMVIEW = "Creation of Permission View Error: {0}"
+LOGMSG_ERR_SEC_ADD_PERMVIEW = "Creation of Permission View Error: %s"
 """ Error adding permission view, format with err message """
-LOGMSG_ERR_SEC_DEL_PERMVIEW = "Remove Permission from View Error: {0}"
+LOGMSG_ERR_SEC_DEL_PERMVIEW = "Remove Permission from View Error: %s"
 """ Error deleting permission view, format with err message """
 LOGMSG_WAR_SEC_DEL_PERMVIEW = (
-    "Refused to delete permission view, assoc with role exists {}.{} {}"
+    "Refused to delete permission view, assoc with role exists %s.%s %s"
 )
-LOGMSG_WAR_SEC_DEL_PERMISSION = "Refused to delete, permission {} does not exist"
-LOGMSG_WAR_SEC_DEL_VIEWMENU = "Refused to delete, view menu {} does not exist"
-LOGMSG_WAR_SEC_DEL_PERM_PVM = "Refused to delete permission {}, PVM exists {}"
-LOGMSG_WAR_SEC_DEL_VIEWMENU_PVM = "Refused to delete view menu {}, PVM exists {}"
-LOGMSG_ERR_SEC_ADD_PERMROLE = "Add Permission to Role Error: {0}"
+LOGMSG_WAR_SEC_DEL_PERMISSION = "Refused to delete, permission %s does not exist"
+LOGMSG_WAR_SEC_DEL_VIEWMENU = "Refused to delete, view menu %s does not exist"
+LOGMSG_WAR_SEC_DEL_PERM_PVM = "Refused to delete permission %s, PVM exists %s"
+LOGMSG_WAR_SEC_DEL_VIEWMENU_PVM = "Refused to delete view menu %s, PVM exists %s"
+LOGMSG_ERR_SEC_ADD_PERMROLE = "Add Permission to Role Error: %s"
 """ Error adding permission to role, format with err message """
-LOGMSG_ERR_SEC_DEL_PERMROLE = "Remove Permission to Role Error: {0}"
+LOGMSG_ERR_SEC_DEL_PERMROLE = "Remove Permission to Role Error: %s"
 """ Error deleting permission to role, format with err message """
-LOGMSG_ERR_SEC_ADD_REGISTER_USER = "Add Register User Error: {0}"
+LOGMSG_ERR_SEC_ADD_REGISTER_USER = "Add Register User Error: %s"
 """ Error adding registered user, format with err message """
-LOGMSG_ERR_SEC_DEL_REGISTER_USER = "Remove Register User Error: {0}"
+LOGMSG_ERR_SEC_DEL_REGISTER_USER = "Remove Register User Error: %s"
 """ Error deleting registered user, format with err message """
-LOGMSG_ERR_SEC_NO_REGISTER_HASH = "Attempt to activate user with false hash: {0}"
+LOGMSG_ERR_SEC_NO_REGISTER_HASH = "Attempt to activate user with false hash: %s"
 """ Attempt to activate user with not registered hash, format with hash """
-LOGMSG_ERR_SEC_AUTH_LDAP = "LDAP Error {0}"
+LOGMSG_ERR_SEC_AUTH_LDAP = "LDAP Error %s"
 """ Generic LDAP error, format with err message """
 LOGMSG_ERR_SEC_AUTH_LDAP_TLS = (
-    "LDAP Could not activate TLS on established connection with {0}"
+    "LDAP Could not activate TLS on established connection with %s"
 )
 """ LDAP Could not activate TLS on established connection with server """
-LOGMSG_ERR_SEC_ADD_USER = "Error adding new user to database. {0}"
+LOGMSG_ERR_SEC_ADD_USER = "Error adding new user to database. %s"
 """ Error adding user, format with err message """
-LOGMSG_ERR_SEC_UPD_USER = "Error updating user to database. {0} "
+LOGMSG_ERR_SEC_UPD_USER = "Error updating user to database. %s "
 """ Error updating user, format with err message """
 LOGMSG_WAR_SEC_NO_USER = "No user yet created, use flask fab command to do it."
 """ Warning when app starts if no user exists on db """
-LOGMSG_WAR_SEC_NOLDAP_OBJ = "No LDAP object found for: {0}"
+LOGMSG_WAR_SEC_NOLDAP_OBJ = "No LDAP object found for: %s"
 
-LOGMSG_INF_SEC_ADD_PERMVIEW = "Created Permission View: {0}"
+LOGMSG_INF_SEC_ADD_PERMVIEW = "Created Permission View: %s"
 """ Info when adding permission view, format with permission view class string """
-LOGMSG_INF_SEC_DEL_PERMVIEW = "Removed Permission View: {0} on {1}"
+LOGMSG_INF_SEC_DEL_PERMVIEW = "Removed Permission View: %s on %s"
 """ Info when deleting permission view, format with permission name and view name """
-LOGMSG_INF_SEC_ADD_PERMROLE = "Added Permission {0} to role {1}"
+LOGMSG_INF_SEC_ADD_PERMROLE = "Added Permission %s to role %s"
 """ Info when adding permission to role,
 format with permission view class string and role name """
-LOGMSG_INF_SEC_DEL_PERMROLE = "Removed Permission {0} to role {1}"
+LOGMSG_INF_SEC_DEL_PERMROLE = "Removed Permission %s to role %s"
 """ Info when deleting permission to role,
 format with permission view class string and role name """
-LOGMSG_INF_SEC_ADD_ROLE = "Inserted Role: {0}"
+LOGMSG_INF_SEC_ADD_ROLE = "Inserted Role: %s"
 """ Info when added role, format with role name """
 LOGMSG_INF_SEC_NO_DB = "Security DB not found Creating all Models from Base"
 LOGMSG_INF_SEC_ADD_DB = "Security DB Created"
-LOGMSG_INF_SEC_ADD_USER = "Added user {0}"
+LOGMSG_INF_SEC_ADD_USER = "Added user %s"
 """ User added, format with username """
-LOGMSG_INF_SEC_UPD_USER = "Updated user {0}"
+LOGMSG_INF_SEC_UPD_USER = "Updated user %s"
 """ User updated, format with username """
-LOGMSG_INF_SEC_UPD_ROLE = "Updated role {0}"
+LOGMSG_INF_SEC_UPD_ROLE = "Updated role %s"
 """ Role updated, format with role name """
-LOGMSG_ERR_SEC_UPD_ROLE = "An error occurred updating role {0}"
+LOGMSG_ERR_SEC_UPD_ROLE = "An error occurred updating role %s"
 """ Role updated Error, format with role name """
 
-LOGMSG_INF_FAB_ADDON_ADDED = "Registered AddOn: {0}"
+LOGMSG_INF_FAB_ADDON_ADDED = "Registered AddOn: %s"
 """ Addon imported and registered """
-LOGMSG_ERR_FAB_ADDON_IMPORT = "An error occurred when importing declared addon {0}: {1}"
+LOGMSG_ERR_FAB_ADDON_IMPORT = "An error occurred when importing declared addon %s: %s"
 """ Error on addon import, format with addon class path and error message """
-LOGMSG_ERR_FAB_ADDON_PROCESS = (
-    "An error occurred when processing declared addon {0}: {1}"
-)
+LOGMSG_ERR_FAB_ADDON_PROCESS = "An error occurred when processing declared addon %s: %s"
 """ Error on addon processing (pre, register, post),
 format with addon class path and error message """
 
 
-LOGMSG_ERR_FAB_ADD_PERMISSION_MENU = "Add Permission on Menu Error: {0}"
+LOGMSG_ERR_FAB_ADD_PERMISSION_MENU = "Add Permission on Menu Error: %s"
 """ Error when adding a permission to a menu, format with err """
-LOGMSG_ERR_FAB_ADD_PERMISSION_VIEW = "Add Permission on View Error: {0}"
+LOGMSG_ERR_FAB_ADD_PERMISSION_VIEW = "Add Permission on View Error: %s"
 """ Error when adding a permission to a menu, format with err """
 
-LOGMSG_ERR_DBI_ADD_GENERIC = "Add record error: {0}"
+LOGMSG_ERR_DBI_ADD_GENERIC = "Add record error: %s"
 """ Database add generic error, format with err message """
-LOGMSG_ERR_DBI_EDIT_GENERIC = "Edit record error: {0}"
+LOGMSG_ERR_DBI_EDIT_GENERIC = "Edit record error: %s"
 """ Database edit generic error, format with err message """
-LOGMSG_ERR_DBI_DEL_GENERIC = "Delete record error: {0}"
+LOGMSG_ERR_DBI_DEL_GENERIC = "Delete record error: %s"
 """ Database delete generic error, format with err message """
 LOGMSG_WAR_DBI_AVG_ZERODIV = "Zero division on aggregate_avg"
 
-LOGMSG_WAR_FAB_VIEW_EXISTS = "View already exists {0} ignoring"
+LOGMSG_WAR_FAB_VIEW_EXISTS = "View already exists %s ignoring"
 """ Attempt to add an already added view, format with view name """
-LOGMSG_WAR_DBI_ADD_INTEGRITY = "Add record integrity error: {0}"
+LOGMSG_WAR_DBI_ADD_INTEGRITY = "Add record integrity error: %s"
 """ Dabase integrity error, format with err message """
-LOGMSG_WAR_DBI_EDIT_INTEGRITY = "Edit record integrity error: {0}"
+LOGMSG_WAR_DBI_EDIT_INTEGRITY = "Edit record integrity error: %s"
 """ Dabase integrity error, format with err message """
-LOGMSG_WAR_DBI_DEL_INTEGRITY = "Delete record integrity error: {0}"
+LOGMSG_WAR_DBI_DEL_INTEGRITY = "Delete record integrity error: %s"
 """ Dabase integrity error, format with err message """
 
-LOGMSG_INF_FAB_ADD_VIEW = "Registering class {0} on menu {1}"
+LOGMSG_INF_FAB_ADD_VIEW = "Registering class %s on menu %s"
 """ Inform that view class was added, format with class name, name"""
 
 
 FLAMSG_ERR_SEC_ACCESS_DENIED = lazy_gettext("Access is Denied")
 """ Access denied flash message """
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/exceptions.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/fields.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/fieldwidgets.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/fieldwidgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/filemanager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/filemanager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/forms.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 else:
                     return field(
                         self.label,
                         description=self.description,
                         validators=self.validators,
                         default=self.default,
                     )
-        log.error("Column %s Type not supported" % self.colname)
+        log.error("Column %s Type not supported", self.colname)
 
 
 class GeneralModelConverter(object):
     """
         Returns a form from a model only one public exposed
         method 'create_form'
     """
@@ -253,15 +253,15 @@
                     label,
                     description,
                     lst_validators,
                     filter_rel_fields,
                     form_props,
                 )
             else:
-                log.warning("Relation {0} not supported".format(col_name))
+                log.warning("Relation %s not supported", col_name)
         else:
             return self._convert_simple(
                 col_name, label, description, lst_validators, form_props
             )
 
     def create_form(
         self,
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/hooks.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/hooks.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/menu.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/base.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/decorators.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     def __init__(self, datamodel):
         self.datamodel = datamodel
 
     def convert(self, col_name):
         for conversion in self.conversion_table:
             if getattr(self.datamodel, conversion[0])(col_name):
                 return [item(col_name, self.datamodel) for item in conversion[1]]
-        log.warning("Filter type not supported for column: %s" % col_name)
+        log.warning("Filter type not supported for column: %s", col_name)
 
 
 class Filters(object):
     filters: List[BaseFilter] = []
     """ List of instantiated BaseFilter classes """
     values: List[Any] = []
     """ list of values to apply to filters """
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/generic/interface.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/generic/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/group.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
             row = {}
             if not isinstance(item[0], tuple):
                 row[self.group_bys_cols[0]] = str(item[0])
             else:
                 for group_col_data, i in zip(item[0], enumerate(item[0])):
                     row[self.group_bys_cols[i]] = str(group_col_data)
             for col_data, i in zip(item[1:], enumerate(item[1:])):
-                log.debug("{0},{1}".format(col_data, i))
+                log.debug("%s,%s", col_data, i)
                 key = self.aggr_by_cols[i].__name__ + self.aggr_by_cols[i]
                 if isinstance(col_data, datetime.date):
                     row[key] = str(col_data)
                 else:
                     row[key] = col_data
             ret.append(row)
         return ret
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mixins.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mixins.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/fields.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/mongoengine/interface.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/mongoengine/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,17 +75,17 @@
             if order_direction == "asc":
                 objs = objs.order_by("-{0}".format(order_column))
             else:
                 objs = objs.order_by("+{0}".format(order_column))
 
         if page_size is None:  # error checking and warnings
             if page is not None:
-                log.error("Attempting to get page %s but page_size is undefined" % page)
+                log.error("Attempting to get page %s but page_size is undefined", page)
             if count > 100:
-                log.warn("Retrieving %s %s items from DB" % (count, str(self.obj)))
+                log.warn("Retrieving %s %s items from DB", count, self.obj)
         else:  # get data segment for paginated page
             offset = (page or 0) * page_size
             objs = objs[offset : offset + page_size]
 
         return count, objs
 
     def is_object_id(self, col_name):
@@ -203,41 +203,41 @@
             self.message = (as_unicode(self.add_row_message), "success")
             return True
         except Exception as e:
             self.message = (
                 as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
                 "danger",
             )
-            log.exception(LOGMSG_ERR_DBI_ADD_GENERIC.format(str(e)))
+            log.exception(LOGMSG_ERR_DBI_ADD_GENERIC, e)
             return False
 
     def edit(self, item):
         try:
             item.save()
             self.message = (as_unicode(self.edit_row_message), "success")
             return True
         except Exception as e:
             self.message = (
                 as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
                 "danger",
             )
-            log.exception(LOGMSG_ERR_DBI_EDIT_GENERIC.format(str(e)))
+            log.exception(LOGMSG_ERR_DBI_EDIT_GENERIC, e)
             return False
 
     def delete(self, item):
         try:
             item.delete()
             self.message = (as_unicode(self.delete_row_message), "success")
             return True
         except Exception as e:
             self.message = (
                 as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
                 "danger",
             )
-            log.exception(LOGMSG_ERR_DBI_DEL_GENERIC.format(str(e)))
+            log.exception(LOGMSG_ERR_DBI_DEL_GENERIC, e)
             return False
 
     def get_columns_list(self):
         """
         modified: removing the '_cls' column added by Mongoengine to support
         mongodb document inheritance
         cf. http://docs.mongoengine.org/apireference.html#documents:
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/__init__.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/filters.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/models/sqla/interface.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/models/sqla/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,15 +723,15 @@
         try:
             self.session.add(item)
             self.session.commit()
             self.message = (as_unicode(self.add_row_message), "success")
             return True
         except IntegrityError as e:
             self.message = (as_unicode(self.add_integrity_error_message), "warning")
-            log.warning(LOGMSG_WAR_DBI_ADD_INTEGRITY.format(str(e)))
+            log.warning(LOGMSG_WAR_DBI_ADD_INTEGRITY, e)
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
         except Exception as e:
             self.message = (as_unicode(self.database_error_message), "danger")
             log.exception("Database error")
@@ -744,15 +744,15 @@
         try:
             self.session.merge(item)
             self.session.commit()
             self.message = (as_unicode(self.edit_row_message), "success")
             return True
         except IntegrityError as e:
             self.message = (as_unicode(self.edit_integrity_error_message), "warning")
-            log.warning(LOGMSG_WAR_DBI_EDIT_INTEGRITY.format(str(e)))
+            log.warning(LOGMSG_WAR_DBI_EDIT_INTEGRITY, e)
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
         except Exception as e:
             self.message = (as_unicode(self.database_error_message), "danger")
             log.exception("Database error")
@@ -766,15 +766,15 @@
             self._delete_files(item)
             self.session.delete(item)
             self.session.commit()
             self.message = (as_unicode(self.delete_row_message), "success")
             return True
         except IntegrityError as e:
             self.message = (as_unicode(self.delete_integrity_error_message), "warning")
-            log.warning(LOGMSG_WAR_DBI_DEL_INTEGRITY.format(str(e)))
+            log.warning(LOGMSG_WAR_DBI_DEL_INTEGRITY, e)
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
         except Exception as e:
             self.message = (as_unicode(self.database_error_message), "danger")
             log.exception("Database error")
@@ -789,20 +789,20 @@
                 self._delete_files(item)
                 self.session.delete(item)
             self.session.commit()
             self.message = (as_unicode(self.delete_row_message), "success")
             return True
         except IntegrityError as e:
             self.message = (as_unicode(self.delete_integrity_error_message), "warning")
-            log.warning(LOGMSG_WAR_DBI_DEL_INTEGRITY.format(str(e)))
+            log.warning(LOGMSG_WAR_DBI_DEL_INTEGRITY, e)
             self.session.rollback()
             return False
         except Exception as e:
             self.message = (as_unicode(self.database_error_message), "danger")
-            log.exception(LOGMSG_ERR_DBI_DEL_GENERIC.format(str(e)))
+            log.exception(LOGMSG_ERR_DBI_DEL_GENERIC, e)
             self.session.rollback()
             return False
 
     """
     -----------------------
      FILE HANDLING METHODS
     -----------------------
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/decorators.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,17 +99,15 @@
                 if not current_user.is_authenticated:
                     verify_jwt_in_request()
                 if current_app.appbuilder.sm.has_access(
                     permission_str, class_permission_name
                 ):
                     return f(self, *args, **kwargs)
             log.warning(
-                LOGMSG_ERR_SEC_ACCESS_DENIED.format(
-                    permission_str, class_permission_name
-                )
+                LOGMSG_ERR_SEC_ACCESS_DENIED, permission_str, class_permission_name
             )
             return self.response_403()
 
         f._permission_name = permission_str
         return functools.update_wrapper(wraps, f)
 
     return _protect
@@ -135,17 +133,15 @@
                 permission_str = f"{PERMISSION_PREFIX}{_permission_name}"
         if permission_str in self.base_permissions and self.appbuilder.sm.has_access(
             permission_str, self.class_permission_name
         ):
             return f(self, *args, **kwargs)
         else:
             log.warning(
-                LOGMSG_ERR_SEC_ACCESS_DENIED.format(
-                    permission_str, self.__class__.__name__
-                )
+                LOGMSG_ERR_SEC_ACCESS_DENIED, permission_str, self.__class__.__name__
             )
             flash(as_unicode(FLAMSG_ERR_SEC_ACCESS_DENIED), "danger")
         return redirect(
             url_for(
                 self.appbuilder.sm.auth_view.__class__.__name__ + ".login",
                 next=request.url,
             )
@@ -177,17 +173,15 @@
                 permission_str = f"{PERMISSION_PREFIX}{_permission_name}"
         if permission_str in self.base_permissions and self.appbuilder.sm.has_access(
             permission_str, self.class_permission_name
         ):
             return f(self, *args, **kwargs)
         else:
             log.warning(
-                LOGMSG_ERR_SEC_ACCESS_DENIED.format(
-                    permission_str, self.__class__.__name__
-                )
+                LOGMSG_ERR_SEC_ACCESS_DENIED, permission_str, self.__class__.__name__
             )
             if not current_user.is_authenticated:
                 return response_unauthorized_mvc(401)
             return response_unauthorized_mvc(403)
 
     f._permission_name = permission_str
     return functools.update_wrapper(wraps, f)
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/forms.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 def _oauth_tokengetter(token=None):
     """
     Default function to return the current user oauth token
     from session cookie.
     """
     token = session.get("oauth")
-    log.debug("Token Get: {0}".format(token))
+    log.debug("Token Get: %s", token)
     return token
 
 
 class BaseSecurityManager(AbstractSecurityManager):
     auth_view = None
     """ The obj instance for authentication view """
     user_view = None
@@ -268,15 +268,15 @@
         if self.auth_type == AUTH_OAUTH:
             from authlib.integrations.flask_client import OAuth
 
             self.oauth = OAuth(app)
             self.oauth_remotes = dict()
             for _provider in self.oauth_providers:
                 provider_name = _provider["name"]
-                log.debug("OAuth providers init {0}".format(provider_name))
+                log.debug("OAuth providers init %s", provider_name)
                 obj_provider = self.oauth.register(
                     provider_name, **_provider["remote_app"]
                 )
                 obj_provider._tokengetter = self.oauth_tokengetter
                 if not self.oauth_user_info:
                     self.oauth_user_info = self.get_oauth_user_info
                 # Whitelist only users with matching emails
@@ -341,17 +341,16 @@
             if role_key in _role_keys:
                 for fab_role_name in fab_role_names:
                     fab_role = self.find_role(fab_role_name)
                     if fab_role:
                         _roles.add(fab_role)
                     else:
                         log.warning(
-                            "Can't find role specified in AUTH_ROLES_MAPPING: {0}".format(
-                                fab_role_name
-                            )
+                            "Can't find role specified in AUTH_ROLES_MAPPING: %s",
+                            fab_role_name,
                         )
         return _roles
 
     @property
     def auth_type_provider_name(self) -> Optional[str]:
         provider_to_auth_type = {AUTH_DB: "db", AUTH_LDAP: "ldap"}
         return provider_to_auth_type.get(self.auth_type)
@@ -539,15 +538,16 @@
 
         def wraps(provider, response=None):
             ret = f(self, provider, response=response)
             # Checks if decorator is well behaved and returns a dict as supposed.
             if not type(ret) == dict:
                 log.error(
                     "OAuth user info decorated function "
-                    "did not returned a dict, but: {0}".format(type(ret))
+                    "did not returned a dict, but: %s",
+                    type(ret),
                 )
                 return {}
             return ret
 
         self.oauth_user_info = wraps
         return wraps
 
@@ -590,57 +590,57 @@
         Since there are different OAuth API's with different ways to
         retrieve user info
         """
         # for GITHUB
         if provider == "github" or provider == "githublocal":
             me = self.appbuilder.sm.oauth_remotes[provider].get("user")
             data = me.json()
-            log.debug("User info from Github: {0}".format(data))
+            log.debug("User info from Github: %s", data)
             return {"username": "github_" + data.get("login")}
         # for twitter
         if provider == "twitter":
             me = self.appbuilder.sm.oauth_remotes[provider].get("account/settings.json")
             data = me.json()
-            log.debug("User info from Twitter: {0}".format(data))
+            log.debug("User info from Twitter: %s", data)
             return {"username": "twitter_" + data.get("screen_name", "")}
         # for linkedin
         if provider == "linkedin":
             me = self.appbuilder.sm.oauth_remotes[provider].get(
                 "people/~:(id,email-address,first-name,last-name)?format=json"
             )
             data = me.json()
-            log.debug("User info from Linkedin: {0}".format(data))
+            log.debug("User info from Linkedin: %s", data)
             return {
                 "username": "linkedin_" + data.get("id", ""),
                 "email": data.get("email-address", ""),
                 "first_name": data.get("firstName", ""),
                 "last_name": data.get("lastName", ""),
             }
         # for Google
         if provider == "google":
             me = self.appbuilder.sm.oauth_remotes[provider].get("userinfo")
             data = me.json()
-            log.debug("User info from Google: {0}".format(data))
+            log.debug("User info from Google: %s", data)
             return {
                 "username": "google_" + data.get("id", ""),
                 "first_name": data.get("given_name", ""),
                 "last_name": data.get("family_name", ""),
                 "email": data.get("email", ""),
             }
         # for Azure AD Tenant. Azure OAuth response contains
         # JWT token which has user info.
         # JWT token needs to be base64 decoded.
         # https://docs.microsoft.com/en-us/azure/active-directory/develop/
         # active-directory-protocols-oauth-code
         if provider == "azure":
-            log.debug("Azure response received : {0}".format(resp))
+            log.debug("Azure response received : %s", resp)
             id_token = resp["id_token"]
             log.debug(str(id_token))
             me = self._azure_jwt_token_parse(id_token)
-            log.debug("Parse JWT token : {0}".format(me))
+            log.debug("Parse JWT token : %s", me)
             return {
                 "name": me.get("name", ""),
                 "email": me["upn"],
                 "first_name": me.get("given_name", ""),
                 "last_name": me.get("family_name", ""),
                 "id": me["oid"],
                 "username": me["oid"],
@@ -648,15 +648,15 @@
             }
         # for OpenShift
         if provider == "openshift":
             me = self.appbuilder.sm.oauth_remotes[provider].get(
                 "apis/user.openshift.io/v1/users/~"
             )
             data = me.json()
-            log.debug("User info from OpenShift: {0}".format(data))
+            log.debug("User info from OpenShift: %s", data)
             return {"username": "openshift_" + data.get("metadata").get("name")}
         # for Okta
         if provider == "okta":
             me = self.appbuilder.sm.oauth_remotes[provider].get("userinfo")
             data = me.json()
             log.debug("User info from Okta: %s", data)
             return {
@@ -908,25 +908,25 @@
         if user is None or (not user.is_active):
             # Balance failure and success
             check_password_hash(
                 "pbkdf2:sha256:150000$Z3t6fmj2$22da622d94a1f8118"
                 "c0976a03d2f18f680bfff877c9a965db9eedc51bc0be87c",
                 "password",
             )
-            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED.format(username))
+            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED, username)
             # Balance failure and success
             if first_user:
                 self.noop_user_update(first_user)
             return None
         elif check_password_hash(user.password, password):
             self.update_user_auth_stat(user, True)
             return user
         else:
             self.update_user_auth_stat(user, False)
-            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED.format(username))
+            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED, username)
             return None
 
     def _search_ldap(self, ldap, con, username):
         """
         Searches LDAP for user.
 
         :param ldap: The ldap module reference
@@ -952,36 +952,37 @@
             self.auth_ldap_email_field,
         ]
         if len(self.auth_roles_mapping) > 0:
             request_fields.append(self.auth_ldap_group_field)
 
         # preform the LDAP search
         log.debug(
-            "LDAP search for '{0}' with fields {1} in scope '{2}'".format(
-                filter_str, request_fields, self.auth_ldap_search
-            )
+            "LDAP search for '%s' with fields %s in scope '%s'",
+            filter_str,
+            request_fields,
+            self.auth_ldap_search,
         )
         raw_search_result = con.search_s(
             self.auth_ldap_search, ldap.SCOPE_SUBTREE, filter_str, request_fields
         )
-        log.debug("LDAP search returned: {0}".format(raw_search_result))
+        log.debug("LDAP search returned: %s", raw_search_result)
 
         # Remove any search referrals from results
         search_result = [
             (dn, attrs)
             for dn, attrs in raw_search_result
             if dn is not None and isinstance(attrs, dict)
         ]
 
         # only continue if 0 or 1 results were returned
         if len(search_result) > 1:
             log.error(
-                "LDAP search for '{0}' in scope '{1}' returned multiple results".format(
-                    filter_str, self.auth_ldap_search
-                )
+                "LDAP search for '%s' in scope '%s' returned multiple results",
+                filter_str,
+                self.auth_ldap_search,
             )
             return None, None
 
         try:
             # extract the DN
             user_dn = search_result[0][0]
             # extract the other attributes
@@ -1009,17 +1010,15 @@
 
             # lookup registration role in flask db
             fab_role = self.find_role(registration_role_name)
             if fab_role:
                 user_role_objects.add(fab_role)
             else:
                 log.warning(
-                    "Can't find AUTH_USER_REGISTRATION role: {0}".format(
-                        registration_role_name
-                    )
+                    "Can't find AUTH_USER_REGISTRATION role: %s", registration_role_name
                 )
 
         return list(user_role_objects)
 
     def _ldap_bind_indirect(self, ldap, con) -> None:
         """
         Attempt to bind to LDAP using the AUTH_LDAP_BIND_USER.
@@ -1028,40 +1027,37 @@
         :param con: The ldap connection
         """
         # always check AUTH_LDAP_BIND_USER is set before calling this method
         assert self.auth_ldap_bind_user, "AUTH_LDAP_BIND_USER must be set"
 
         try:
             log.debug(
-                "LDAP bind indirect TRY with username: '{0}'".format(
-                    self.auth_ldap_bind_user
-                )
+                "LDAP bind indirect TRY with username: '%s'", self.auth_ldap_bind_user
             )
             con.simple_bind_s(self.auth_ldap_bind_user, self.auth_ldap_bind_password)
             log.debug(
-                "LDAP bind indirect SUCCESS with username: '{0}'".format(
-                    self.auth_ldap_bind_user
-                )
+                "LDAP bind indirect SUCCESS with username: '%s'",
+                self.auth_ldap_bind_user,
             )
         except ldap.INVALID_CREDENTIALS as ex:
             log.error(
                 "AUTH_LDAP_BIND_USER and AUTH_LDAP_BIND_PASSWORD are"
                 " not valid LDAP bind credentials"
             )
             raise ex
 
     @staticmethod
     def _ldap_bind(ldap, con, dn: str, password: str) -> bool:
         """
         Validates/binds the provided dn/password with the LDAP sever.
         """
         try:
-            log.debug("LDAP bind TRY with username: '{0}'".format(dn))
+            log.debug("LDAP bind TRY with username: '%s'", dn)
             con.simple_bind_s(dn, password)
-            log.debug("LDAP bind SUCCESS with username: '{0}'".format(dn))
+            log.debug("LDAP bind SUCCESS with username: '%s'", dn)
             return True
         except ldap.INVALID_CREDENTIALS:
             return False
 
     @staticmethod
     def ldap_extract(
         ldap_dict: Dict[str, bytes], field_name: str, fallback: str
@@ -1129,17 +1125,15 @@
             # Initialise LDAP connection
             con = ldap.initialize(self.auth_ldap_server)
             con.set_option(ldap.OPT_REFERRALS, 0)
             if self.auth_ldap_use_tls:
                 try:
                     con.start_tls_s()
                 except Exception:
-                    log.error(
-                        LOGMSG_ERR_SEC_AUTH_LDAP_TLS.format(self.auth_ldap_server)
-                    )
+                    log.error(LOGMSG_ERR_SEC_AUTH_LDAP_TLS, self.auth_ldap_server)
                     return None
 
             # Define variables, so we can check if they are set in later steps
             user_dn = None
             user_attributes = {}
 
             # Flow 1 - (Indirect Search Bind):
@@ -1161,24 +1155,24 @@
                     log.error(
                         "AUTH_LDAP_SEARCH must be set when using AUTH_LDAP_BIND_USER"
                     )
                     return None
 
                 # If search failed, go away
                 if user_dn is None:
-                    log.info(LOGMSG_WAR_SEC_NOLDAP_OBJ.format(username))
+                    log.info(LOGMSG_WAR_SEC_NOLDAP_OBJ, username)
                     return None
 
                 # Bind with user_dn/password (validates credentials)
                 if not self._ldap_bind(ldap, con, user_dn, password):
                     if user:
                         self.update_user_auth_stat(user, False)
 
                     # Invalid credentials, go away
-                    log.info(LOGMSG_WAR_SEC_LOGIN_FAILED.format(username))
+                    log.info(LOGMSG_WAR_SEC_LOGIN_FAILED, username)
                     return None
 
             # Flow 2 - (Direct Search Bind):
             #  - in this flow, the credentials provided by the end-user are used
             #    to preform the LDAP search
             #  - in this flow, we only search LDAP if AUTH_LDAP_SEARCH is set
             #     - features like AUTH_USER_REGISTRATION & AUTH_ROLES_SYNC_AT_LOGIN
@@ -1201,38 +1195,36 @@
                 # Bind with bind_username/password
                 # (validates credentials & authorizes for LDAP search)
                 if not self._ldap_bind(ldap, con, bind_username, password):
                     if user:
                         self.update_user_auth_stat(user, False)
 
                     # Invalid credentials, go away
-                    log.info(LOGMSG_WAR_SEC_LOGIN_FAILED.format(bind_username))
+                    log.info(LOGMSG_WAR_SEC_LOGIN_FAILED, bind_username)
                     return None
 
                 # Search for `username` (if AUTH_LDAP_SEARCH is set)
                 #  - returns the `user_attributes`
                 #    needed for AUTH_USER_REGISTRATION/AUTH_ROLES_SYNC_AT_LOGIN
                 #  - we search on `username` not `bind_username`,
                 #    because AUTH_LDAP_APPEND_DOMAIN and AUTH_LDAP_USERNAME_FORMAT
                 #    would result in an invalid search filter
                 if self.auth_ldap_search:
                     user_dn, user_attributes = self._search_ldap(ldap, con, username)
 
                     # If search failed, go away
                     if user_dn is None:
-                        log.info(LOGMSG_WAR_SEC_NOLDAP_OBJ.format(username))
+                        log.info(LOGMSG_WAR_SEC_NOLDAP_OBJ, username)
                         return None
 
             # Sync the user's roles
             if user and user_attributes and self.auth_roles_sync_at_login:
                 user.roles = self._ldap_calculate_user_roles(user_attributes)
                 log.debug(
-                    "Calculated new roles for user='{0}' as: {1}".format(
-                        user_dn, user.roles
-                    )
+                    "Calculated new roles for user='%s' as: %s", user_dn, user.roles
                 )
 
             # If the user is new, register them
             if (not user) and user_attributes and self.auth_user_registration:
                 user = self.add_user(
                     username=username,
                     first_name=self.ldap_extract(
@@ -1244,49 +1236,49 @@
                     email=self.ldap_extract(
                         user_attributes,
                         self.auth_ldap_email_field,
                         f"{username}@email.notfound",
                     ),
                     role=self._ldap_calculate_user_roles(user_attributes),
                 )
-                log.debug("New user registered: {0}".format(user))
+                log.debug("New user registered: %s", user)
 
                 # If user registration failed, go away
                 if not user:
-                    log.info(LOGMSG_ERR_SEC_ADD_REGISTER_USER.format(username))
+                    log.info(LOGMSG_ERR_SEC_ADD_REGISTER_USER, username)
                     return None
 
             # LOGIN SUCCESS (only if user is now registered)
             if user:
                 self.update_user_auth_stat(user)
                 return user
             else:
                 return None
 
         except ldap.LDAPError as e:
             msg = None
             if isinstance(e, dict):
                 msg = getattr(e, "message", None)
             if (msg is not None) and ("desc" in msg):
-                log.error(LOGMSG_ERR_SEC_AUTH_LDAP.format(e.message["desc"]))
+                log.error(LOGMSG_ERR_SEC_AUTH_LDAP, e.message["desc"])
                 return None
             else:
                 log.error(e)
                 return None
 
     def auth_user_oid(self, email):
         """
         OpenID user Authentication
 
         :param email: user's email to authenticate
         :type self: User model
         """
         user = self.find_user(email=email)
         if user is None or (not user.is_active):
-            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED.format(email))
+            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED, email)
             return None
         else:
             self.update_user_auth_stat(user)
             return user
 
     def auth_user_remote_user(self, username):
         """
@@ -1308,15 +1300,15 @@
                 email=username + "@email.notfound",
                 role=self.find_role(self.auth_user_registration_role),
             )
 
         # If user does not exist on the DB and not auto user registration,
         # or user is inactive, go away.
         elif user is None or (not user.is_active):
-            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED.format(username))
+            log.info(LOGMSG_WAR_SEC_LOGIN_FAILED, username)
             return None
 
         self.update_user_auth_stat(user)
         return user
 
     def _oauth_calculate_user_roles(self, userinfo) -> List[str]:
         user_role_objects = set()
@@ -1341,17 +1333,15 @@
 
             # lookup registration role in flask db
             fab_role = self.find_role(registration_role_name)
             if fab_role:
                 user_role_objects.add(fab_role)
             else:
                 log.warning(
-                    "Can't find AUTH_USER_REGISTRATION role: {0}".format(
-                        registration_role_name
-                    )
+                    "Can't find AUTH_USER_REGISTRATION role: %s", registration_role_name
                 )
 
         return list(user_role_objects)
 
     def auth_user_oauth(self, userinfo):
         """
         Method for authenticating user with OAuth.
@@ -1361,17 +1351,15 @@
         """
         # extract the username from `userinfo`
         if "username" in userinfo:
             username = userinfo["username"]
         elif "email" in userinfo:
             username = userinfo["email"]
         else:
-            log.error(
-                "OAUTH userinfo does not have username or email {0}".format(userinfo)
-            )
+            log.error("OAUTH userinfo does not have username or email %s", userinfo)
             return None
 
         # If username is empty, go away
         if (username is None) or username == "":
             return None
 
         # Search the DB for this user
@@ -1384,34 +1372,30 @@
         # If user is not registered, and not self-registration, go away
         if (not user) and (not self.auth_user_registration):
             return None
 
         # Sync the user's roles
         if user and self.auth_roles_sync_at_login:
             user.roles = self._oauth_calculate_user_roles(userinfo)
-            log.debug(
-                "Calculated new roles for user='{0}' as: {1}".format(
-                    username, user.roles
-                )
-            )
+            log.debug("Calculated new roles for user='%s' as: %s", username, user.roles)
 
         # If the user is new, register them
         if (not user) and self.auth_user_registration:
             user = self.add_user(
                 username=username,
                 first_name=userinfo.get("first_name", ""),
                 last_name=userinfo.get("last_name", ""),
                 email=userinfo.get("email", "") or f"{username}@email.notfound",
                 role=self._oauth_calculate_user_roles(userinfo),
             )
-            log.debug("New user registered: {0}".format(user))
+            log.debug("New user registered: %s", user)
 
             # If user registration failed, go away
             if not user:
-                log.error("Error creating a new OAuth user {0}".format(username))
+                log.error("Error creating a new OAuth user %s", username)
                 return None
 
         # LOGIN SUCCESS (only if user is now registered)
         if user:
             self.update_user_auth_stat(user)
             return user
         else:
@@ -1825,15 +1809,15 @@
         """
         state_transitions = self.create_state_transitions(baseviews, menus)
         if dry:
             return state_transitions
         if not state_transitions:
             log.info("No state transitions found")
             return dict()
-        log.debug(f"State transitions: {state_transitions}")
+        log.debug("State transitions: %s", state_transitions)
         roles = self.get_all_roles()
         for role in roles:
             permissions = list(role.permissions)
             for pvm in permissions:
                 new_pvm_states = state_transitions["add"].get(
                     (pvm.view_menu.name, pvm.permission.name)
                 )
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/mongoengine/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,22 +83,22 @@
                 register_user.password = hashed_password
             else:
                 register_user.password = generate_password_hash(password)
             register_user.registration_hash = str(uuid.uuid1())
             register_user.save()
             return register_user
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_ADD_REGISTER_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_ADD_REGISTER_USER, e)
             return False
 
     def del_register_user(self, register_user):
         try:
             register_user.delete()
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_DEL_REGISTER_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_DEL_REGISTER_USER, e)
 
     def find_user(self, username=None, email=None):
         if username:
             return self.user_model.objects(username=username).first()
         elif email:
             return self.user_model.objects(email=email).first()
 
@@ -127,28 +127,28 @@
             user.active = True
             user.roles = role if isinstance(role, list) else [role]
             if hashed_password:
                 user.password = hashed_password
             else:
                 user.password = generate_password_hash(password)
             user.save()
-            log.info(c.LOGMSG_INF_SEC_ADD_USER.format(username))
+            log.info(c.LOGMSG_INF_SEC_ADD_USER, username)
             return user
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_ADD_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_ADD_USER, e)
             return False
 
     def count_users(self):
         return len(self.user_model.objects)
 
     def update_user(self, user):
         try:
             user.save()
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_UPD_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_UPD_USER, e)
             return False
 
     def get_user_by_id(self, pk):
         return self.user_model.objects(pk=pk).first()
 
     def load_user(self, pk):
         return self.get_user_by_id(pk)
@@ -166,26 +166,26 @@
             permissions = []
 
         role = self.find_role(name)
         if role is None:
             try:
                 role = self.role_model(name=name, permissions=permissions)
                 role.save()
-                log.info(c.LOGMSG_INF_SEC_ADD_ROLE.format(name))
+                log.info(c.LOGMSG_INF_SEC_ADD_ROLE, name)
                 return role
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_ROLE.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_ROLE, e)
         return role
 
     def update_role(self, pk, name: str) -> Optional[Role]:
         try:
             role = self.role_model.objects(id=pk).update(name=name)
-            log.info(c.LOGMSG_INF_SEC_UPD_ROLE.format(role))
+            log.info(c.LOGMSG_INF_SEC_UPD_ROLE, role)
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_UPD_ROLE.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_UPD_ROLE, e)
             return
 
     def find_role(self, name):
         return self.role_model.objects(name=name).first()
 
     def get_all_roles(self):
         return self.role_model.objects
@@ -224,30 +224,30 @@
         perm = self.find_permission(name)
         if perm is None:
             try:
                 perm = self.permission_model(name=name)
                 perm.save()
                 return perm
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_PERMISSION.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_PERMISSION, e)
         return perm
 
     def del_permission(self, name):
         """
             Deletes a permission from the backend, model permission
 
             :param name:
                 name of the permission: 'can_add','can_edit' etc...
         """
         perm = self.find_permission(name)
         if perm:
             try:
                 perm.delete()
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION, e)
 
     """
     ----------------------
      PRIMITIVES VIEW MENU
     ----------------------
     """
 
@@ -269,30 +269,30 @@
         view_menu = self.find_view_menu(name)
         if view_menu is None:
             try:
                 view_menu = self.viewmenu_model(name=name)
                 view_menu.save()
                 return view_menu
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_VIEWMENU.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_VIEWMENU, e)
         return view_menu
 
     def del_view_menu(self, name):
         """
             Deletes a ViewMenu from the backend
 
             :param name:
                 name of the ViewMenu
         """
         obj = self.find_view_menu(name)
         if obj:
             try:
                 obj.delete()
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION, e)
 
     """
     ----------------------
      PERMISSION VIEW MENU
     ----------------------
     """
 
@@ -332,35 +332,33 @@
             return pv
         vm = self.add_view_menu(view_menu_name)
         perm = self.add_permission(permission_name)
         pv = self.permissionview_model()
         pv.view_menu, pv.permission = vm, perm
         try:
             pv.save()
-            log.info(c.LOGMSG_INF_SEC_ADD_PERMVIEW.format(str(pv)))
+            log.info(c.LOGMSG_INF_SEC_ADD_PERMVIEW, pv)
             return pv
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_ADD_PERMVIEW.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_ADD_PERMVIEW, e)
 
     def del_permission_view_menu(self, permission_name, view_menu_name, cascade=True):
         try:
             pv = self.find_permission_view_menu(permission_name, view_menu_name)
             # delete permission on view
             pv.delete()
             if not cascade:
                 return
             # if no more permission on permission view, delete permission
             pv = self.permissionview_model.objects(permission=pv.permission)
             if not pv:
                 self.del_permission(pv.permission.name)
-            log.info(
-                c.LOGMSG_INF_SEC_DEL_PERMVIEW.format(permission_name, view_menu_name)
-            )
+            log.info(c.LOGMSG_INF_SEC_DEL_PERMVIEW, permission_name, view_menu_name)
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_DEL_PERMVIEW.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_DEL_PERMVIEW, e)
 
     def exist_permission_on_views(self, lst, item):
         for i in lst:
             if i.permission.name == item:
                 return True
         return False
 
@@ -379,38 +377,34 @@
             :param perm_view:
                 The PermissionViewMenu object
         """
         if perm_view and perm_view not in role.permissions:
             try:
                 role.permissions.append(perm_view)
                 role.save()
-                log.info(
-                    c.LOGMSG_INF_SEC_ADD_PERMROLE.format(str(perm_view), role.name)
-                )
+                log.info(c.LOGMSG_INF_SEC_ADD_PERMROLE, perm_view, role.name)
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_PERMROLE.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_PERMROLE, e)
 
     def del_permission_role(self, role, perm_view):
         """
             Remove permission-ViewMenu object to Role
 
             :param role:
                 The role object
             :param perm_view:
                 The PermissionViewMenu object
         """
         if perm_view in role.permissions:
             try:
                 role.permissions.remove(perm_view)
                 role.save()
-                log.info(
-                    c.LOGMSG_INF_SEC_DEL_PERMROLE.format(str(perm_view), role.name)
-                )
+                log.info(c.LOGMSG_INF_SEC_DEL_PERMROLE, perm_view, role.name)
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_DEL_PERMROLE.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_DEL_PERMROLE, e)
 
     def export_roles(
         self, path: Optional[str] = None, indent: Optional[Union[int, str]] = None
     ) -> None:
         """Exports roles to JSON file."""
         timestamp = datetime.now().strftime("%Y%m%dT%H%M%S")
         filename = path or f"roles_export_{timestamp}.json"
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/mongoengine/models.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/registerviews.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/registerviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             first_name=register_user.first_name,
             last_name=register_user.last_name,
         )
         msg.recipients = [register_user.email]
         try:
             mail.send(msg)
         except Exception as e:
-            log.error("Send email exception: {0}".format(str(e)))
+            log.error("Send email exception: %s", e)
             return False
         return True
 
     def add_registration(self, username, first_name, last_name, email, password=""):
         """
             Add a registration request for the user.
 
@@ -122,15 +122,15 @@
         """
             Endpoint to expose an activation url, this url
             is sent to the user by email, when accessed the user is inserted
             and activated
         """
         reg = self.appbuilder.sm.find_register_user(activation_hash)
         if not reg:
-            log.error(c.LOGMSG_ERR_SEC_NO_REGISTER_HASH.format(activation_hash))
+            log.error(c.LOGMSG_ERR_SEC_NO_REGISTER_HASH, activation_hash)
             flash(as_unicode(self.false_error_message), "danger")
             return redirect(self.appbuilder.get_url_for_index)
         if not self.appbuilder.sm.add_user(
             username=reg.username,
             email=reg.email,
             first_name=reg.first_name,
             last_name=reg.last_name,
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/schemas.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/role/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/role/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/schema.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/schema.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/user/validator.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/user/validator.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/manager.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             inspector = Inspector.from_engine(engine)
             if "ab_user" not in inspector.get_table_names():
                 log.info(c.LOGMSG_INF_SEC_NO_DB)
                 Base.metadata.create_all(engine)
                 log.info(c.LOGMSG_INF_SEC_ADD_DB)
             super(SecurityManager, self).create_db()
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_CREATE_DB.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_CREATE_DB, e)
             exit(1)
 
     def find_register_user(self, registration_hash):
         return (
             self.get_session.query(self.registeruser_model)
             .filter(self.registeruser_model.registration_hash == registration_hash)
             .scalar()
@@ -140,30 +140,30 @@
             register_user.password = generate_password_hash(password)
         register_user.registration_hash = str(uuid.uuid1())
         try:
             self.get_session.add(register_user)
             self.get_session.commit()
             return register_user
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_ADD_REGISTER_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_ADD_REGISTER_USER, e)
             self.appbuilder.get_session.rollback()
             return None
 
     def del_register_user(self, register_user):
         """
             Deletes registration object from database
 
             :param register_user: RegisterUser object to delete
         """
         try:
             self.get_session.delete(register_user)
             self.get_session.commit()
             return True
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_DEL_REGISTER_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_DEL_REGISTER_USER, e)
             self.get_session.rollback()
             return False
 
     def find_user(self, username=None, email=None):
         """
             Finds user by username or email
         """
@@ -180,25 +180,25 @@
                 else:
                     return (
                         self.get_session.query(self.user_model)
                         .filter(self.user_model.username == username)
                         .one_or_none()
                     )
             except MultipleResultsFound:
-                log.error(f"Multiple results found for user {username}")
+                log.error("Multiple results found for user %s", username)
                 return None
         elif email:
             try:
                 return (
                     self.get_session.query(self.user_model)
                     .filter_by(email=email)
                     .one_or_none()
                 )
             except MultipleResultsFound:
-                log.error(f"Multiple results found for user with email {email}")
+                log.error("Multiple results found for user with email %s", email)
                 return None
 
     def get_all_users(self):
         return self.get_session.query(self.user_model).all()
 
     def add_user(
         self,
@@ -223,31 +223,31 @@
             user.roles = role if isinstance(role, list) else [role]
             if hashed_password:
                 user.password = hashed_password
             else:
                 user.password = generate_password_hash(password)
             self.get_session.add(user)
             self.get_session.commit()
-            log.info(c.LOGMSG_INF_SEC_ADD_USER.format(username))
+            log.info(c.LOGMSG_INF_SEC_ADD_USER, username)
             return user
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_ADD_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_ADD_USER, e)
             self.get_session.rollback()
             return False
 
     def count_users(self):
         return self.get_session.query(func.count(self.user_model.id)).scalar()
 
     def update_user(self, user):
         try:
             self.get_session.merge(user)
             self.get_session.commit()
-            log.info(c.LOGMSG_INF_SEC_UPD_USER.format(user))
+            log.info(c.LOGMSG_INF_SEC_UPD_USER, user)
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_UPD_USER.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_UPD_USER, e)
             self.get_session.rollback()
             return False
 
     def get_user_by_id(self, pk):
         return self.get_session.query(self.user_model).get(pk)
 
     def get_first_user(self) -> "User":
@@ -278,32 +278,32 @@
         if role is None:
             try:
                 role = self.role_model()
                 role.name = name
                 role.permissions = permissions
                 self.get_session.add(role)
                 self.get_session.commit()
-                log.info(c.LOGMSG_INF_SEC_ADD_ROLE.format(name))
+                log.info(c.LOGMSG_INF_SEC_ADD_ROLE, name)
                 return role
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_ROLE.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_ROLE, e)
                 self.get_session.rollback()
         return role
 
     def update_role(self, pk, name: str) -> Optional[Role]:
         role = self.get_session.query(self.role_model).get(pk)
         if not role:
             return
         try:
             role.name = name
             self.get_session.merge(role)
             self.get_session.commit()
-            log.info(c.LOGMSG_INF_SEC_UPD_ROLE.format(role))
+            log.info(c.LOGMSG_INF_SEC_UPD_ROLE, role)
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_UPD_ROLE.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_UPD_ROLE, e)
             self.get_session.rollback()
             return
 
     def find_role(self, name):
         return (
             self.get_session.query(self.role_model).filter_by(name=name).one_or_none()
         )
@@ -473,43 +473,43 @@
             try:
                 perm = self.permission_model()
                 perm.name = name
                 self.get_session.add(perm)
                 self.get_session.commit()
                 return perm
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_PERMISSION.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_PERMISSION, e)
                 self.get_session.rollback()
         return perm
 
     def del_permission(self, name: str) -> bool:
         """
             Deletes a permission from the backend, model permission
 
             :param name:
                 name of the permission: 'can_add','can_edit' etc...
         """
         perm = self.find_permission(name)
         if not perm:
-            log.warning(c.LOGMSG_WAR_SEC_DEL_PERMISSION.format(name))
+            log.warning(c.LOGMSG_WAR_SEC_DEL_PERMISSION, name)
             return False
         try:
             pvms = (
                 self.get_session.query(self.permissionview_model)
                 .filter(self.permissionview_model.permission == perm)
                 .all()
             )
             if pvms:
-                log.warning(c.LOGMSG_WAR_SEC_DEL_PERM_PVM.format(perm, pvms))
+                log.warning(c.LOGMSG_WAR_SEC_DEL_PERM_PVM, perm, pvms)
                 return False
             self.get_session.delete(perm)
             self.get_session.commit()
             return True
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION, e)
             self.get_session.rollback()
             return False
 
     """
     ----------------------
      PRIMITIVES VIEW MENU
     ----------------------
@@ -539,43 +539,43 @@
             try:
                 view_menu = self.viewmenu_model()
                 view_menu.name = name
                 self.get_session.add(view_menu)
                 self.get_session.commit()
                 return view_menu
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_VIEWMENU.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_VIEWMENU, e)
                 self.get_session.rollback()
         return view_menu
 
     def del_view_menu(self, name: str) -> bool:
         """
             Deletes a ViewMenu from the backend
 
             :param name:
                 name of the ViewMenu
         """
         view_menu = self.find_view_menu(name)
         if not view_menu:
-            log.warning(c.LOGMSG_WAR_SEC_DEL_VIEWMENU.format(name))
+            log.warning(c.LOGMSG_WAR_SEC_DEL_VIEWMENU, name)
             return False
         try:
             pvms = (
                 self.get_session.query(self.permissionview_model)
                 .filter(self.permissionview_model.view_menu == view_menu)
                 .all()
             )
             if pvms:
-                log.warning(c.LOGMSG_WAR_SEC_DEL_VIEWMENU_PVM.format(view_menu, pvms))
+                log.warning(c.LOGMSG_WAR_SEC_DEL_VIEWMENU_PVM, view_menu, pvms)
                 return False
             self.get_session.delete(view_menu)
             self.get_session.commit()
             return True
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_DEL_PERMISSION, e)
             self.get_session.rollback()
             return False
 
     """
     ----------------------
      PERMISSION VIEW MENU
     ----------------------
@@ -624,18 +624,18 @@
         vm = self.add_view_menu(view_menu_name)
         perm = self.add_permission(permission_name)
         pv = self.permissionview_model()
         pv.view_menu, pv.permission = vm, perm
         try:
             self.get_session.add(pv)
             self.get_session.commit()
-            log.info(c.LOGMSG_INF_SEC_ADD_PERMVIEW.format(str(pv)))
+            log.info(c.LOGMSG_INF_SEC_ADD_PERMVIEW, pv)
             return pv
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_ADD_PERMVIEW.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_ADD_PERMVIEW, e)
             self.get_session.rollback()
 
     def del_permission_view_menu(self, permission_name, view_menu_name, cascade=True):
         if not (permission_name and view_menu_name):
             return
         pv = self.find_permission_view_menu(permission_name, view_menu_name)
         if not pv:
@@ -643,17 +643,18 @@
         roles_pvs = (
             self.get_session.query(self.role_model)
             .filter(self.role_model.permissions.contains(pv))
             .first()
         )
         if roles_pvs:
             log.warning(
-                c.LOGMSG_WAR_SEC_DEL_PERMVIEW.format(
-                    view_menu_name, permission_name, roles_pvs
-                )
+                c.LOGMSG_WAR_SEC_DEL_PERMVIEW,
+                view_menu_name,
+                permission_name,
+                roles_pvs,
             )
             return
         try:
             # delete permission on view
             self.get_session.delete(pv)
             self.get_session.commit()
             # if no more permission on permission view, delete permission
@@ -661,19 +662,17 @@
                 return
             if (
                 not self.get_session.query(self.permissionview_model)
                 .filter_by(permission=pv.permission)
                 .all()
             ):
                 self.del_permission(pv.permission.name)
-            log.info(
-                c.LOGMSG_INF_SEC_DEL_PERMVIEW.format(permission_name, view_menu_name)
-            )
+            log.info(c.LOGMSG_INF_SEC_DEL_PERMVIEW, permission_name, view_menu_name)
         except Exception as e:
-            log.error(c.LOGMSG_ERR_SEC_DEL_PERMVIEW.format(str(e)))
+            log.error(c.LOGMSG_ERR_SEC_DEL_PERMVIEW, e)
             self.get_session.rollback()
 
     def exist_permission_on_views(self, lst, item):
         for i in lst:
             if i.permission and i.permission.name == item:
                 return True
         return False
@@ -694,19 +693,17 @@
                 The PermissionViewMenu object
         """
         if perm_view and perm_view not in role.permissions:
             try:
                 role.permissions.append(perm_view)
                 self.get_session.merge(role)
                 self.get_session.commit()
-                log.info(
-                    c.LOGMSG_INF_SEC_ADD_PERMROLE.format(str(perm_view), role.name)
-                )
+                log.info(c.LOGMSG_INF_SEC_ADD_PERMROLE, perm_view, role.name)
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_ADD_PERMROLE.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_ADD_PERMROLE, e)
                 self.get_session.rollback()
 
     def del_permission_role(self, role, perm_view):
         """
             Remove permission-ViewMenu object to Role
 
             :param role:
@@ -715,19 +712,17 @@
                 The PermissionViewMenu object
         """
         if perm_view in role.permissions:
             try:
                 role.permissions.remove(perm_view)
                 self.get_session.merge(role)
                 self.get_session.commit()
-                log.info(
-                    c.LOGMSG_INF_SEC_DEL_PERMROLE.format(str(perm_view), role.name)
-                )
+                log.info(c.LOGMSG_INF_SEC_DEL_PERMROLE, perm_view, role.name)
             except Exception as e:
-                log.error(c.LOGMSG_ERR_SEC_DEL_PERMROLE.format(str(e)))
+                log.error(c.LOGMSG_ERR_SEC_DEL_PERMROLE, e)
                 self.get_session.rollback()
 
     def export_roles(
         self, path: Optional[str] = None, indent: Optional[Union[int, str]] = None
     ) -> None:
         """ Exports roles to JSON file. """
         timestamp = datetime.now().strftime("%Y%m%dT%H%M%S")
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/sqla/models.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/security/views.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/security/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,28 +602,28 @@
 class AuthOAuthView(AuthView):
     login_template = "appbuilder/general/security/login_oauth.html"
 
     @expose("/login/")
     @expose("/login/<provider>")
     @expose("/login/<provider>/<register>")
     def login(self, provider: Optional[str] = None) -> WerkzeugResponse:
-        log.debug("Provider: {0}".format(provider))
+        log.debug("Provider: %s", provider)
         if g.user is not None and g.user.is_authenticated:
-            log.debug("Already authenticated {0}".format(g.user))
+            log.debug("Already authenticated %s", g.user)
             return redirect(self.appbuilder.get_url_for_index)
 
         if provider is None:
             return self.render_template(
                 self.login_template,
                 providers=self.appbuilder.sm.oauth_providers,
                 title=self.title,
                 appbuilder=self.appbuilder,
             )
 
-        log.debug("Going to call authorize for: {0}".format(provider))
+        log.debug("Going to call authorize for: %s", provider)
         random_state = generate_random_string()
         state = jwt.encode(
             request.args.to_dict(flat=False), random_state, algorithm="HS256"
         )
         session["oauth_state"] = random_state
         try:
             if provider == "twitter":
@@ -639,44 +639,44 @@
                 return self.appbuilder.sm.oauth_remotes[provider].authorize_redirect(
                     redirect_uri=url_for(
                         ".oauth_authorized", provider=provider, _external=True
                     ),
                     state=state.decode("ascii") if isinstance(state, bytes) else state,
                 )
         except Exception as e:
-            log.error("Error on OAuth authorize: {0}".format(e))
+            log.error("Error on OAuth authorize: %s", e)
             flash(as_unicode(self.invalid_login_message), "warning")
             return redirect(self.appbuilder.get_url_for_index)
 
     @expose("/oauth-authorized/<provider>")
     def oauth_authorized(self, provider: str) -> WerkzeugResponse:
         log.debug("Authorized init")
         if provider not in self.appbuilder.sm.oauth_remotes:
             flash("Provider not supported.", "warning")
             log.warning("OAuth authorized got an unknown provider %s", provider)
             return redirect(self.appbuilder.get_url_for_login)
         try:
             resp = self.appbuilder.sm.oauth_remotes[provider].authorize_access_token()
         except Exception as e:
-            log.error("Error authorizing OAuth access token: {0}".format(e))
+            log.error("Error authorizing OAuth access token: %s", e)
             flash("The request to sign in was denied.", "error")
             return redirect(self.appbuilder.get_url_for_login)
         if resp is None:
             flash("You denied the request to sign in.", "warning")
             return redirect(self.appbuilder.get_url_for_login)
-        log.debug("OAUTH Authorized resp: {0}".format(resp))
+        log.debug("OAUTH Authorized resp: %s", resp)
         # Retrieves specific user info from the provider
         try:
             self.appbuilder.sm.set_oauth_session(provider, resp)
             userinfo = self.appbuilder.sm.oauth_user_info(provider, resp)
         except Exception as e:
-            log.error("Error returning OAuth user info: {0}".format(e))
+            log.error("Error returning OAuth user info: %s", e)
             user = None
         else:
-            log.debug("User info retrieved from {0}: {1}".format(provider, userinfo))
+            log.debug("User info retrieved from %s: %s", provider, userinfo)
             # User email is not whitelisted
             if provider in self.appbuilder.sm.oauth_whitelists:
                 whitelist = self.appbuilder.sm.oauth_whitelists[provider]
                 allow = False
                 for email in whitelist:
                     if "email" in userinfo and re.search(email, userinfo["email"]):
                         allow = True
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/ab.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/ab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/united.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/united.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/aol.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/aol.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/fab.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/flags/flags16.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/flickr.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/flickr.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/google.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/google.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/myopenid.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/myopenid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/img/yahoo.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/img/yahoo.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 var AdminFilters = function(element, labels, form, filters, active_filters) {
     // Admin filters will deal with the adding and removing of search filters
     // :param labels:
     //      {'col','label'}
     // :param active_filters:
     //      [['col','filter name','value'],[...],...]
 
-    var $root = $(element);
-    var $container = $('.filters', $root);
-    var lastCount = 0;
+    let $root = $(element);
+    let $container = $('.filters', $root);
+    let lastCount = 0;
 
     function removeFilter() {
         $(this).closest('tr').remove();
         $('button', $root).show();
 
         return false;
     }
@@ -26,105 +26,108 @@
             } else {
                 addActiveFilter(this[0], this[1], this[2]);
             }
         });
     }
 
     function addActiveFilter(name, filter_name, value) {
-        var $el = $('<tr />').appendTo($container);
+        let $el = $('<tr />').appendTo($container);
 
         addRemoveFilter($el, name, labels[name]);
-        var i_option = addFilterOptionsValue($el, name, filter_name);
+        let i_option = addFilterOptionsValue($el, name, filter_name, false);
 
-        var $field = $(form[name]);
+        let $field = $(form[name]);
         // if form item complex like <div><input bla></div>, datetime
         if ($("input", $($field)).html() != undefined) {
             $field_inner = $("input", $field)
             $field_inner.attr('name', '_flt_' + i_option + '_' + name);
             $field_inner.val(value);
             $field_inner.attr('class', ' filter_val ' + $field_inner.attr('class'));
         } else {
-            if (($field.attr('type')) == 'checkbox') {
+            if (($field.attr('type')) === 'checkbox') {
                 $field.attr('checked', true);
             }
             $field.attr('name', '_flt_' + i_option + '_' + name);
             $field.val(value);
             $field.attr('class', ' filter_val ' + $field.attr('class'));
         }
         $el.append(
             $('<td/>').append($field)
         );
     }
 
     function addRemoveFilter($el, name, label) {
         $el.append(
-            $('<td class="col-lg-1 col-md-1" />').append(
+            $('<td />').append(
                 $('<a href="#" class="btn remove-filter" />')
                 .append($('<span class="close-icon">&times;</span>'))
                 .append('&nbsp;')
                 .append(label)
                 .on('click', removeFilter)
             )
         );
     }
 
-    function addFilterOptionsValue($el, name, value) {
-        var $select = $('<select class="filter-op my_select2" />');
-        cx = 0;
-        var i_option = -1;
+    function addFilterOptionsValue($el, name, value, activateSelect2 = true) {
+        let $select = $('<select class="filter-op my_select2" />');
+        let cx = 0;
+        let i_option = -1;
         $(filters[name]).each(function() {
             if (value == this) {
                 $select.append($('<option selected="selected"/>').attr('value', cx).text(this));
                 i_option = cx;
             } else {
                 $select.append($('<option/>').attr('value', cx).text(this));
             }
             cx += 1;
         });
-
         $el.append(
-            $('<td class="col-lg-1 col-md-1 col-sm-1" />').append($select)
+            $('<td />').append($select)
         );
         // avoids error
-        if (i_option == -1) {
-            $select.select2();
-        }
-        $select.on('change', function() {
-            changeOperation(this, $el, name)
+        // if (i_option === -1) { $select.select2(); }
+        $select.on('select2:select', function(e) {
+            changeOperation(e, $el, name);
         });
-
+        if (activateSelect2) {
+            $select.select2({
+                placeholder: "Select a State",
+                allowClear: true,
+                theme: "bootstrap"
+            });
+        }
         return i_option;
     }
 
 
     function addFilter(name, filter) {
-        var $el = $('<tr />').appendTo($container);
+        let $el = $('<tr />').appendTo($container);
 
         addRemoveFilter($el, name, labels[name]);
 
         addFilterOptionsValue($el, name);
-        var $field = $(form[name]);
+        let $field = $(form[name]);
 
         // if form item complex like <div><input bla></div>, datetime
         if ($("input", $($field)).html() != undefined) {
             $field_inner = $("input", $($field))
             $field_inner.attr('name', '_flt_0_' + name);
             $field_inner.attr('class', ' filter_val ' + $field_inner.attr('class'));
-
         } else {
             $field.attr('name', '_flt_0_' + name);
             $field.attr('class', ' filter_val ' + $field.attr('class'));
         }
         $el.append(
             $('<td/>').append($field)
         );
         if ($field.hasClass("my_select2")) {
             $field.select2({
                 placeholder: "Select a State",
-                allowClear: true
+                allowClear: true,
+                theme: "bootstrap"
             });
         }
         if ($field.hasClass("appbuilder_datetime")) {
             $field.datetimepicker();
         }
         if ($field.hasClass("appbuilder_date")) {
             $field.datetimepicker({
@@ -134,19 +137,19 @@
         lastCount += 1;
     }
 
     // ----------------------------------------------------------
     // Trigger for option change will change input element name
     // ----------------------------------------------------------
     function changeOperation(e, $el, name) {
-        $in = $el.find('.filter_val');
-        $in.attr('name', '_flt_' + $(e.target).val() + '_' + name);
+        let $in = $el.find('.filter_val');
+        const data = e.params.data;
+        $in.attr('name', '_flt_' + data.id + '_' + name);
     }
 
     $('a.filter').on('click', function() {
-        var name = $(this).attr('name');
+        const name = $(this).attr('name');
         addFilter(name);
     });
 
     addActiveFilters();
-
 };
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/google_charts.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/google_charts.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/js/v4-shims.min.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2.css` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2.js` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/select2/select2x2.png` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/baselayout.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/baselayout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/baselib.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/baselib.html`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 {% macro menu_block(menu) %}
 {% for item1 in menu.get_list() %}
     {% if item1 | is_menu_visible %}
         {% if item1.childs %}
             <li class="dropdown">
-				<a class="dropdown-toggle" data-toggle="dropdown" href="javascript:void(0)">
+				<a class="dropdown-toggle" data-toggle="dropdown" href="#">
             {% if item1.icon %}
                 <i class="fa {{item1.icon}}"></i>&nbsp;
             {% endif %}
 				{{_(item1.label)}}<b class="caret"></b></a>
 		        <ul class="dropdown-menu">
 				{% set divider = False %}
             {% for item2 in item1.childs %}
@@ -54,15 +54,15 @@
 
 {% macro locale_menu(languages) %}
 {% set locale = session['locale'] %}
 {% if not locale %}
 	{% set locale = 'en' %}
 {% endif %}
 <li class="dropdown">
-	<a class="dropdown-toggle" data-toggle="dropdown" href="javascript:void(0)">
+	<a class="dropdown-toggle" data-toggle="dropdown" href="#">
 	   <div class="f16"><i class="flag {{languages[locale].get('flag')}}"></i><b class="caret"></b>
        </div>
 	</a>
     {% if languages.keys()|length > 1 %}
 	<ul class="dropdown-menu">
 	<li class="dropdown">
 		{% for lang in languages %}
@@ -122,7 +122,13 @@
                     <i class="fa fa-fw fa-sign-in"></i>{{_("Login")}}</a></li>
                 {% endif %}
                 </ul>
         </div>
    </div>
 </div>
 {% endmacro %}
+
+{% macro get_nonce() -%}
+    {%- if csp_nonce is defined -%}
+        {{- csp_nonce() -}}
+    {%- endif %}
+{%- endmacro %}
```

#### html2text {}

```diff
@@ -29,8 +29,9 @@
     * {{ locale_menu(languages) }} {% if not current_user.is_anonymous %}
     *  {{g.user.get_full_name()}}
           o {{_("Profile")}}
           o {{_("Logout")}}
     * {% else %}
     * {{_("Login")}}
     * {% endif %}
-{% endmacro %}
+{% endmacro %} {% macro get_nonce() -%} {%- if csp_nonce is defined -%} {{-
+csp_nonce() -}} {%- endif %} {%- endmacro %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/confirm.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/confirm.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/lib.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/lib.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+{% import 'appbuilder/baselib.html' as baselib %}
+
 {% macro render_additional_links(additional_links, pk) %}
     {% if additional_links %}
         {% for item in additional_links %}
             <a href="{{item.href}}?pk={{pk}}" class="btn btn-sm btn-primary"><span class="glyphicon glyphicon"></span>
             {{_(item.label)}}</a>
         {% endfor %}
     {% endif %}
@@ -16,24 +18,35 @@
         {% if path %}
             <form id="action_form" action="{{ path }}" method="POST" style="display: none">
                 {% if csrf_token is defined and csrf_token %}
                     <input type="hidden" name="csrf_token" value="{{ csrf_token() }}"/>
                 {% endif %}
                 <input type="hidden" id="action" name="action" />
             </form>
-
-            <a href="javascript:void(0)" class="btn btn-sm btn-primary"
-               {% if action.confirmation %}
-               onclick="var a = new AdminActions(); return a.execute_single('{{path}}','{{action.confirmation}}');">
-               {% else %}
-               onclick="var a = new AdminActions(); return a.execute_single('{{path}}',false);">
-               {% endif %}
+            <a
+                id="btn-action-{{ endpoint }}"
+                href="#"
+                class="btn btn-sm btn-primary"
+            >
                 <i class="fa {{action.icon}}"></i>
-                    {{_(action.text)}}
-                </a>
+                {{_(action.text)}}
+            </a>
+
+            <script nonce="{{ baselib.get_nonce() }}">
+                document.getElementById("btn-action-{{ endpoint }}")
+                    .addEventListener("click", function () {
+                        {% if action.confirmation %}
+                            const adminAction = new AdminActions();
+                            return adminAction.execute_single('{{path}}','{{action.confirmation}}');
+                        {% else %}
+                            const adminAction = new AdminActions();
+                            return adminAction.execute_single('{{path}}',false);
+                        {% endif %}
+                    })
+            </script>
         {% endif %}
     {% endfor %}
 {% endmacro %}
 
 {% macro action_form(actions, modelview_name) %}
     {% if actions %}
         {% set endpoint = modelview_name + '.action_post' %}
@@ -62,23 +75,23 @@
     <button type="button" class="btn btn-default btn-sm dropdown-toggle" data-toggle="dropdown">
     {{_('Actions')}}<span class="caret"></span>
     </button>
     <ul class="dropdown-menu" role="menu">
         {% for action_key in actions %}
             {% set action = actions.get(action_key) %}
                 <li>
-                    <a href="javascript:void(0)"
+                    <a href="#"
                         class="{{action.name}}_menu_item">
                         <i class="fa {{action.icon}}"></i>
                         {{ _(action.text) }}
                     </a>
                 </li>
         {% endfor %}
     </ul>
-    <script type="text/javascript">
+    <script nonce="{{ baselib.get_nonce() }}">
     $(document).ready(function() {
     {% for action_key in actions %}
         {% set action = actions.get(action_key) %}
         $('.{{action.name}}_menu_item').on('click', function(){
             {% if action.confirmation %}
                 return modelActions.execute_multiple('{{action.name}}','{{action.confirmation}}');
             {% else %}
@@ -172,55 +185,55 @@
 
     {% if min > 0 %}
     <li>
         <a href="{{ init_page | link_page(modelview_name) }}">&laquo;</a>
     </li>
     {% else %}
     <li class="disabled">
-        <a href="javascript:void(0)">&laquo;</a>
+        <a href="#">&laquo;</a>
     </li>
     {% endif %}
     {% if page > 0 %}
     <li>
         <a href="{{ (page - 1) | link_page(modelview_name) }}">&lt;</a>
     </li>
     {% else %}
     <li class="disabled">
-        <a href="javascript:void(0)">&lt;</a>
+        <a href="#">&lt;</a>
     </li>
     {% endif %}
 
     {% for p in range(min, max) %}
         {% if page == p %}
         <li class="active">
-            <a href="javascript:void(0)">{{ (p + 1) }}</a>
+            <a href="#">{{ (p + 1) }}</a>
         </li>
         {% else %}
         <li>
             <a href="{{ p | link_page(modelview_name) }}">{{ (p + 1) }}</a>
         </li>
         {% endif %}
     {% endfor %}
 
     {% if page + 1 < pages %}
         <li>
             <a href="{{ (page + 1) | link_page(modelview_name) }}">&gt;</a>
         </li>
     {% else %}
         <li class="disabled">
-            <a href="javascript:void(0)">&gt;</a>
+            <a href="#">&gt;</a>
         </li>
     {% endif %}
     {% if max < pages %}
         <li>
             <a href="{{ (pages - 1) | link_page(modelview_name) }}">&raquo;</a>
         </li>
     {% else %}
         <li class="disabled">
-            <a href="javascript:void(0)">&raquo;</a>
+            <a href="#">&raquo;</a>
         </li>
     {% endif %}
 </ul>
 {% endif %}
 {% endmacro %}
 
 
@@ -385,13 +398,25 @@
        title="{{_('Show record')}}">
         <span class="sr-only">{{ _('Show') }}</span>
         <i class="fa fa-search"></i>
     </a>
 {% endmacro %}
 
 {% macro lnk_delete(my_href) %}
-    <a href="javascript:void(0)" class="btn btn-sm btn-default confirm" rel="tooltip" title="{{_('Delete record')}}"
-       onclick="var a = new AdminActions(); return a.execute_single_delete('{{my_href}}','{{ _('You sure you want to delete this item?') }}');">
+    <a
+        id="btn-delete-{{ my_href }}"
+        href="#"
+        class="btn btn-sm btn-default confirm"
+        rel="tooltip"
+        title="{{_('Delete record')}}"
+    >
         <span class="sr-only">{{ _('Delete') }}</span>
         <i class="fa fa-trash"></i>
     </a>
+    <script nonce="{{ baselib.get_nonce() }}">
+        document.getElementById("btn-delete-{{ my_href }}")
+            .addEventListener("click", function () {
+                const adminAction = new AdminActions();
+                return adminAction.execute_single_delete('{{my_href}}','{{_('Are you sure you want to delete this item?')}}');
+            })
+    </script>
 {% endmacro %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html`

 * *Files 2% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 
     {% if related_views is defined %} </div> {% endif %}
 
 {{ lib.panel_end() }}
 {% endblock %}
 
 {% block add_tail_js %}
-<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}"></script>
+<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}" nonce="{{ baselib.get_nonce() }}"></script>
 {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html`

 * *Files 7% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 
 
 {{ lib.panel_end() }}
 
 {% endblock %}
 
 {% block add_tail_js %}
-<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}"></script>
+<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}" nonce="{{ baselib.get_nonce() }}"></script>
 {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/show.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/show.html`

 * *Files 9% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 
 {% if related_views is defined %}</div>{% endif %}
 {{ lib.panel_end() }}
 
 {% endblock content %}
 
 {% block add_tail_js %}
-<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}"></script>
+<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}" nonce="{{ baselib.get_nonce() }}"></script>
 {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html`

 * *Files 10% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
 
 {{ lib.panel_end() }}
 
 {% endblock %}
 
 {% block add_tail_js %}
-<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}"></script>
+<script src="{{url_for('appbuilder.static',filename='js/ab_keep_tab.js')}}" nonce="{{ baselib.get_nonce() }}"></script>
 {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 <!-- extend base layout -->
 {% extends "appbuilder/base.html" %}
 
 {% block content %}
 
-<script type="text/javascript">
-    var baseLoginUrl = "{{appbuilder.get_url_for_login}}";
-    var baseRegisterUrl = "{{appbuilder.get_url_for_login}}";
-    var next = "?next=" + "{{request.args.get('next', '') | urlencode}}";
-
-    function signin(provider) {
-        window.location.href = baseLoginUrl + provider + next;
-    }
-</script>
-
 <div class="container">
     <div id="loginbox" style="margin-top:50px;" class="mainbox col-md-6 col-md-offset-3 col-sm-8 col-sm-offset-2">
         <div class="panel panel-primary">
             <div class="panel-heading">
                 <div class="panel-title">{{ title }}</div>
             </div>
             <div style="padding-top:30px" class="panel-body">
                 <div>
                     {% for provider in providers %}
                     <a
-                        onclick="signin('{{ provider.name }}');"
+                        id="btn-signin-{{provider.name}}"
                         class="btn btn-primary btn-block"
                         type="submit"
                     >
                         {{_('Sign In with ')}}{{ provider.name }}
                         <i id="{{provider.name}}" class="provider-select fa {{provider.icon}} fa-1x"></i>
                     </a>
                     {% endfor %}
                 </div>
             </div>
         </div>
     </div>
 </div>
 
-{% endblock %}
+<script nonce="{{ baselib.get_nonce() }}">
+    var baseLoginUrl = "{{appbuilder.get_url_for_login}}";
+    var baseRegisterUrl = "{{appbuilder.get_url_for_login}}";
+    var next = "?next=" + "{{request.args.get('next', '') | urlencode}}";
+
+    function signin(provider) {
+        window.location.href = baseLoginUrl + provider + next;
+    }
+
+    {% for provider in providers %}
+        document.getElementById("btn-signin-{{provider.name}}")
+            .addEventListener("click", function () { signin("{{provider.name}}") })
+    {% endfor %}
+
+</script>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
  {% extends "appbuilder/base.html" %} {% block content %}
 {{ title }}
 {% for provider in providers %}
 {{_('Sign In with ')}}{{ provider.name }}
  {% endfor %}
-{% endblock %}
+ {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,150 @@
 <!-- extend base layout -->
 {% extends "appbuilder/base.html" %}
 
 {% block content %}
-
-<script type="text/javascript">
-
-function showUsername() {
-    $("#username").removeClass('hidden');
-    $("#label-username").removeClass('hidden');
-}
-
-function hideUsername() {
-    $("#username").addClass('hidden');
-    $("#label-username").addClass('hidden');
-    $("#username").val('');
-}
-
-function hideOpenId() {
-    $("#openid").addClass('hidden');
-    $("#label-openid").addClass('hidden');
-    $("#openid").val('');
-}
-
-function showOpenId() {
-    $("#openid").removeClass('hidden');
-    $("#label-openid").removeClass('hidden');
-}
-
-function set_openid(openid, pr)
-{
-    $('.img-select').attr('class', 'img-rounded img-unselect');
-    $('#' + pr).attr('class', 'img-rounded img-select');
-    if (openid == '') {
-        hideUsername();
-        showOpenId();
-    }
-    else {
-        u = openid.search('<username>');
-        if (u != -1) {
-            showUsername();
-            hideOpenId();
-        }
-        else {
-            hideUsername();
-            hideOpenId();
-        }
-    }
-    form = document.forms['login'];
-    form.elements['openid'].value = openid;
-}
-
-
-function beforeSubmit() {
-    openid = $("#openid").val();
-    u = openid.search('<username>');
-    if (u != -1) {
-        openid = openid.substr(0, u) + $("#username").val();
-    }
-}
-
-//---------------------------------
-// POST FORM to Register User View
-//---------------------------------
-function registerUser() {
-    form = document.forms['login'];
-    if (form.elements['openid'].value == '') {
-        alert('Please choose a provider first');
-    }
-    else {
-        form.action = "{{appbuilder.sm.get_url_for_registeruser}}";
-        form.submit();
-    }
-}
-
-</script>
-
-
-<div class="container">
-        <div id="loginbox" style="margin-top:50px;" class="mainbox col-md-6 col-md-offset-3 col-sm-8 col-sm-offset-2">
-            <div class="panel panel-primary" >
-                    <div class="panel-heading">
-                        <div class="panel-title">{{ title }}</div>
-                    </div>
-                    <div style="padding-top:30px" class="panel-body" >
-
-    <form class="form" action="" method="post" name="login">
-        {{form.hidden_tag()}}
-        <div class="help-block">{{_("Click on your OpenID provider below")}}:</div>
-            <center>
-            <div class="center-block btn-group btn-group-lg" role="group">
-            {% for pr in providers %}
-                <a href="javascript:set_openid('{{pr.url}}', '{{pr.name}}');">
-                <img src="{{url_for('appbuilder.static',filename='img/' + pr.name.lower() + '.png')}}"
-                     id="{{pr.name}}" class="img-rounded img-unselect"/>
-                </a>
-            {% endfor %}
-        </div>
-        </center>
-        <div class="control-group{% if form.errors.openid is defined %} error{% endif %}">
-            <label class="hidden control-label" id="label-openid" for="openid">{{_("Or enter your OpenID here")}}:</label>
-            <div class="controls">
-                {{ form.openid(size = 80, class = "hidden form-control") }}
-                {% for error in form.errors.get('openid', []) %}
-                    <span class="help-inline">{{_('Please choose a provider')}}</span><br>
-                {% endfor %}
-                <label class="hidden control-label" id="label-username" for="username">{{_("Enter your OpenID Username")}}:</label>
-                {{ form.username(size = 80, class = "hidden form-control", autofocus = true) }}
-            </div>
-        </div>
-        <div class="control-group">
-            <div class="controls">
-                <label class="checkbox" for="remember_me">
-                    {{ form.remember_me }} Remember Me
-                </label>
+    <div class="container">
+        <div id="loginbox" style="margin-top:50px;"
+             class="mainbox col-md-6 col-md-offset-3 col-sm-8 col-sm-offset-2">
+            <div class="panel panel-primary">
+                <div class="panel-heading">
+                    <div class="panel-title">{{ title }}</div>
+                </div>
+                <div style="padding-top:30px" class="panel-body">
+                    <form class="form" action="" method="post" name="login">
+                        {{ form.hidden_tag() }}
+                        <div class="help-block">{{ _("Click on your OpenID provider below") }}:</div>
+                        <center>
+                            <div class="center-block btn-group btn-group-lg" role="group">
+                                {% for pr in providers %}
+                                    <a id="btn-oid-provider-{{ pr.name }}">
+                                        <img src="{{ url_for('appbuilder.static',filename='img/' + pr.name.lower() + '.png') }}"
+                                             id="{{ pr.name }}"
+                                             class="img-rounded img-unselect"/>
+                                    </a>
+                                {% endfor %}
+                            </div>
+                        </center>
+                        <div class="control-group{% if form.errors.openid is defined %} error{% endif %}">
+                            <label class="hidden control-label" id="label-openid"
+                                   for="openid">{{ _("Or enter your OpenID here") }}:</label>
+                            <div class="controls">
+                                {{ form.openid(size = 80, class = "hidden form-control") }}
+                                {% for error in form.errors.get('openid', []) %}
+                                    <span class="help-inline">{{ _('Please choose a provider') }}</span>
+                                    <br>
+                                {% endfor %}
+                                <label class="hidden control-label" id="label-username"
+                                       for="username">{{ _("Enter your OpenID Username") }}:</label>
+                                {{ form.username(size = 80, class = "hidden form-control", autofocus = true) }}
+                            </div>
+                        </div>
+                        <div class="control-group">
+                            <div class="controls">
+                                <label class="checkbox" for="remember_me">
+                                    {{ form.remember_me }} Remember Me
+                                </label>
+                            </div>
+                        </div>
+                        <input
+                                id="btn-oid-before-submit"
+                                class="btn btn-primary btn-block"
+                                type="submit"
+                                value="{{ _('Sign In') }}"
+                        >
+                        {% if appbuilder.sm.auth_user_registration %}
+                            <a
+                                    id="btn-oid-register-user"
+                                    class="btn btn-block btn-primary"
+                                    data-toggle="tooltip"
+                                    rel="tooltip"
+                                    title="{{ _('If you are not already a user, please register') }}">
+                                {{ _('Register') }}
+                            </a>
+                        {% endif %}
+                    </form>
+                </div>
             </div>
         </div>
-                <input onclick="beforeSubmit();" class="btn btn-primary btn-block" type="submit" value="{{_('Sign In')}}">
-                {% if appbuilder.sm.auth_user_registration %}
-                    <a href="javascript:registerUser();" class="btn btn-block btn-primary" data-toggle="tooltip" rel="tooltip"
-                       title="{{_('If you are not already a user, please register')}}">
-                        {{_('Register')}}
-                        </a>
-                {% endif %}
-
-    </form>
-</div>
-</div></div></div>
+    </div>
+
+    <script nonce="{{ baselib.get_nonce() }}">
+        function showUsername() {
+            $("#username").removeClass('hidden');
+            $("#label-username").removeClass('hidden');
+        }
+
+        function hideUsername() {
+            $("#username").addClass('hidden');
+            $("#label-username").addClass('hidden');
+            $("#username").val('');
+        }
+
+        function hideOpenId() {
+            $("#openid").addClass('hidden');
+            $("#label-openid").addClass('hidden');
+            $("#openid").val('');
+        }
+
+        function showOpenId() {
+            $("#openid").removeClass('hidden');
+            $("#label-openid").removeClass('hidden');
+        }
+
+        function set_openid(openid, pr) {
+            $('.img-select').attr('class', 'img-rounded img-unselect');
+            $('#' + pr).attr('class', 'img-rounded img-select');
+            if (openid == '') {
+                hideUsername();
+                showOpenId();
+            } else {
+                u = openid.search('<username>');
+                if (u != -1) {
+                    showUsername();
+                    hideOpenId();
+                } else {
+                    hideUsername();
+                    hideOpenId();
+                }
+            }
+            form = document.forms['login'];
+            form.elements['openid'].value = openid;
+        }
+
+        function beforeSubmit() {
+            openid = $("#openid").val();
+            u = openid.search('<username>');
+            if (u != -1) {
+                openid = openid.substr(0, u) + $("#username").val();
+            }
+        }
+
+        //---------------------------------
+        // POST FORM to Register User View
+        //---------------------------------
+        function registerUser() {
+            form = document.forms['login'];
+            if (form.elements['openid'].value == '') {
+                alert('Please choose a provider first');
+            } else {
+                form.action = "{{appbuilder.sm.get_url_for_registeruser}}";
+                form.submit();
+            }
+        }
+        {% for pr in providers %}
+            document.getElementById("btn-oid-provider-{{ pr.name }}")
+                .addEventListener("click", function () {
+                    set_openid("{{ pr.url | safe }}", "{{ pr.name }}");
+                });
+        {% endfor %}
+        document.getElementById("btn-oid-before-submit")
+            .addEventListener("click", function () {
+                beforeSubmit()
+            });
+        {% if appbuilder.sm.auth_user_registration %}
+            document.getElementById("btn-oid-register-user")
+                .addEventListener("click", function () {
+                    registerUser()
+                });
+        {% endif %}
+    </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
  {% extends "appbuilder/base.html" %} {% block content %}
 {{ title }}
-{{form.hidden_tag()}}
-{{_("Click on your OpenID provider below")}}:
-  {% for pr in providers %} [{{url_for('appbuilder.static',filename='img/'_+
-                   pr.name.lower()_+_'.png')}}] {% endfor %}
-{{_("Or enter your OpenID here")}}:
+{{ form.hidden_tag() }}
+{{ _("Click on your OpenID provider below") }}:
+  {% for pr in providers %} [{{ url_for('appbuilder.static',filename='img/' +
+                  pr.name.lower() + '.png') }}] {% endfor %}
+{{ _("Or enter your OpenID here") }}:
 {{ form.openid(size = 80, class = "hidden form-control") }} {% for error in
-form.errors.get('openid', []) %} {{_('Please choose a provider')}}
-{% endfor %} {{_("Enter your OpenID Username")}}: {{ form.username(size = 80,
+form.errors.get('openid', []) %} {{ _('Please choose a provider') }}
+{% endfor %} {{ _("Enter your OpenID Username") }}: {{ form.username(size = 80,
 class = "hidden form-control", autofocus = true) }}
  {{ form.remember_me }} Remember Me
-[{{_('Sign In')}}] {% if appbuilder.sm.auth_user_registration %} {{_
-('Register')}} {% endif %}
-{% endblock %}
+[{{ _('Sign In') }}] {% if appbuilder.sm.auth_user_registration %} {{ _
+('Register') }} {% endif %}
+ {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% import 'appbuilder/baselib.html' as baselib %}
 {% import 'appbuilder/general/lib.html' as lib %}
 
 {% set can_add = "can_add" | is_item_visible(modelview_name) %}
 {% set can_show = "can_show" | is_item_visible(modelview_name) %}
 {% set can_edit = "can_edit" | is_item_visible(modelview_name) %}
 {% set can_delete = "can_delete" | is_item_visible(modelview_name) %}
 {% set actions = actions | get_actions_on_list(modelview_name) %}
@@ -24,15 +25,15 @@
     {% endblock %}
 
     {% block end_content scoped %}
     {% endblock %}
 
     {{ lib.action_form(actions, modelview_name) }}
 
-    <script language="javascript">
+    <script nonce="{{ baselib.get_nonce() }}">
         $(document).ready(function() {
             window.modelActions = new AdminActions();
         });
     </script>
 
 {% else %}
     <b>{{_("No records found")}}</b>
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+{% import 'appbuilder/baselib.html' as baselib %}
+
 <div id="chart" style="height: {{height}};">
 </div>
 
-<script type="text/javascript" src="{{url_for('appbuilder.static',filename='js/google_charts.js')}}"></script>
-<script type="text/javascript">
+<script nonce="{{ baselib.get_nonce() }}" src="{{url_for('appbuilder.static',filename='js/google_charts.js')}}"></script>
+<script nonce="{{ baselib.get_nonce() }}">
             //load the Google Visualization API and the chart
             google.load('visualization', '1', {'packages': ['corechart','gauge']});
 
             //set callback
             google.setOnLoadCallback (createChart);
 
             //-----------------------------------
```

#### html2text {}

```diff
@@ -1 +1,2 @@
+{% import 'appbuilder/baselib.html' as baselib %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+{% import 'appbuilder/baselib.html' as baselib %}
+
 <div id="{{ modelview_name }}" style="height: {{height}};">
 </div>
-<script type="text/javascript" src="{{url_for('appbuilder.static',filename='js/google_charts.js')}}"></script>
-<script type="text/javascript">
+<script src="{{url_for('appbuilder.static',filename='js/google_charts.js')}}" nonce="{{ baselib.get_nonce() }}"></script>
+<script nonce="{{ baselib.get_nonce() }}">
     //load the Google Visualization API and the chart
     google.load('visualization', '1', {'packages': ['corechart']});
 
     //set callback
     google.setOnLoadCallback (createChart);
     // playground http://code.google.com/apis/ajax/playground/?type=visualization#line_chart
 
     var jsonData{{ modelview_name }} = {{ value_columns | tojson }}
 
-
     //-----------------------------------
     // Attach listener for tab open event
     //-----------------------------------
     function attachRedrawForTab(chart, dataTable, options) {
         var $tab_el = $('a[data-toggle="tab"]');
         $tab_el.on('shown.bs.tab', function () {
             // Redraws the chart when the tab is activated, so that chart size on tab
```

#### html2text {}

```diff
@@ -1 +1,2 @@
+{% import 'appbuilder/baselib.html' as baselib %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+{% import 'appbuilder/baselib.html' as baselib %}
 
-<script type="text/javascript" src="{{url_for('appbuilder.static',filename='js/google_charts.js')}}"></script>
-<script type="text/javascript">
+<script nonce="{{ baselib.get_nonce() }}" src="{{url_for('appbuilder.static',filename='js/google_charts.js')}}"></script>
+<script nonce="{{ baselib.get_nonce() }}">
             //load the Google Visualization API and the chart
             google.load('visualization', '1', {'packages': ['corechart']});
 
             //set callback
             google.setOnLoadCallback (createChart);
             // playground http://code.google.com/apis/ajax/playground/?type=visualization#line_chart
```

#### html2text {}

```diff
@@ -1 +1,2 @@
+{% import 'appbuilder/baselib.html' as baselib %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+{% import 'appbuilder/baselib.html' as baselib %}
 {% import 'appbuilder/general/lib.html' as lib %}
 
 <form id="filter_form" class="form-search" method="get">
 
     <div class="btn-group">
         <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown">
         {{_("Add Filter")}}
       <span class="caret"></span>
         </button>
         <ul class="dropdown-menu">
             {% for col in include_cols %}
-            <li><a href="javascript:void(0)" name="{{col}}" class="filter" onclick="return false;">
+            <li><a href="#" name="{{col}}" class="filter">
                 {{ label_columns[col] }}</a>
             </li>
             {% endfor %}
         </ul>
     </div>
 
     <table class="table table-responsive table-hover filters">
@@ -21,19 +22,19 @@
 
         </tbody>
     </table>
 
 {{ lib.btn_search() }}
 </form>
 
-<script>
+<script nonce="{{ baselib.get_nonce() }}">
 	(function($) {
-	var filter = new AdminFilters(
-                    '#filter_form',
-                    {{ label_columns | tojson }},
-                    {{ form_fields | tojson }},
-                    {{ search_filters | tojson }},
-                    {{ active_filters | tojson }}
-                );
-	})(jQuery);
+        const filter = new AdminFilters(
+            '#filter_form',
+            {{ label_columns | tojson }},
+            {{ form_fields | tojson }},
+            {{ search_filters | tojson }},
+            {{ active_filters | tojson }}
+        );
+    })(jQuery);
 
 </script>
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/init.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/init.html`

 * *Files 11% similar despite different names*

```diff
@@ -29,28 +29,28 @@
       <link href="{{url_for('appbuilder.static',filename='select2/select2.css')}}" rel="stylesheet">
         <link href="{{url_for('appbuilder.static',filename='select2/select2-bootstrap-theme.css')}}" rel="stylesheet">
       <link href="{{url_for('appbuilder.static',filename='css/flags/flags16.css')}}" rel="stylesheet">
       <link href="{{url_for('appbuilder.static',filename='css/ab.css')}}" rel="stylesheet">
     {% endblock %}
 
     {% block head_js %}
-      <script src="{{url_for('appbuilder.static',filename='js/jquery-latest.js')}}"></script>
-      <script src="{{url_for('appbuilder.static',filename='js/ab_filters.js')}}"></script>
-      <script src="{{url_for('appbuilder.static',filename='js/ab_actions.js')}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='js/jquery-latest.js')}}" nonce="{{baselib.get_nonce()}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='js/ab_filters.js')}}" nonce="{{baselib.get_nonce()}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='js/ab_actions.js')}}" nonce="{{baselib.get_nonce()}}"></script>
     {% endblock %}
   </head>
   <body >
     {% block body %}
     {% endblock %}
 
     {% block tail_js %}
-      <script src="{{url_for('appbuilder.static',filename='js/bootstrap.min.js')}}"></script>
-      <script src="{{url_for('appbuilder.static',filename='datepicker/bootstrap-datepicker.js')}}"></script>
-      <script src="{{url_for('appbuilder.static',filename='select2/select2.js')}}"></script>
-      <script src="{{url_for('appbuilder.static',filename='js/ab.js')}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='js/bootstrap.min.js')}}" nonce="{{baselib.get_nonce()}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='datepicker/bootstrap-datepicker.js')}}" nonce="{{baselib.get_nonce()}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='select2/select2.js')}}" nonce="{{baselib.get_nonce()}}"></script>
+      <script src="{{url_for('appbuilder.static',filename='js/ab.js')}}" nonce="{{baselib.get_nonce()}}"></script>
     {% endblock %}
 
     {% block add_tail_js %}
     {% endblock %}
 
     {% block tail %}
     {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/navbar.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 {% endmacro %}
 
 
 {% for item1 in menu.get_list() %}
     {% if item1 | is_menu_visible %}
         {% if item1.childs %}
             <li class="dropdown">
-            <a class="dropdown-toggle" data-toggle="dropdown" href="javascript:void(0)">
+            <a class="dropdown-toggle" data-toggle="dropdown" href="#">
             {% if item1.icon %}
                 <i class="fa {{item1.icon}}"></i>&nbsp;
             {% endif %}
             {{_(item1.label)}}<b class="caret"></b></a>
             <ul class="dropdown-menu">
             {% for item2 in item1.childs %}
                 {% if item2 %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/navbar_right.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/navbar_right.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% macro locale_menu(languages) %}
 {% set locale = session['locale'] %}
 {% if not locale %}
     {% set locale = 'en' %}
 {% endif %}
 {% if languages.keys()|length > 1 %}
 <li class="dropdown">
-    <a class="dropdown-toggle" data-toggle="dropdown" href="javascript:void(0)">
+    <a class="dropdown-toggle" data-toggle="dropdown" href="#">
        <div class="f16"><i class="flag {{languages[locale].get('flag')}}"></i><b class="caret"></b>
        </div>
     </a>
     <ul class="dropdown-menu">
     <li class="dropdown">
         {% for lang in languages %}
             {% if lang != locale %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 {% extends "appbuilder/base.html" %}
 
 {% block head_css %}
-{{ super() }}
-<link type="text/css" rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/swagger-ui.css">
-<link rel="shortcut icon" href="https://fastapi.tiangolo.com/img/favicon.png">
+    {{ super() }}
+    <link type="text/css" rel="stylesheet"
+          href="https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/swagger-ui.css">
+    <link rel="shortcut icon" href="https://fastapi.tiangolo.com/img/favicon.png">
 {% endblock %}
 
 {% block content %}
-<div id="swagger-ui">
-</div>
-<script src="https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/swagger-ui-bundle.js"></script>
-<!-- `SwaggerUIBundle` is now available on the page -->
-<script>
+    <div id="swagger-ui">
+    </div>
+    <script src="https://cdn.jsdelivr.net/npm/swagger-ui-dist@4/swagger-ui-bundle.js" nonce="{{ baselib.get_nonce() }}"></script>
+    <!-- `SwaggerUIBundle` is now available on the page -->
+    <script>
 
-    const ui = SwaggerUIBundle({
-        url: '{{openapi_uri}}',
-        dom_id: '#swagger-ui',
-        presets: [
-        SwaggerUIBundle.presets.apis,
-        SwaggerUIBundle.SwaggerUIStandalonePreset
-        ],
-        layout: "BaseLayout"
+        const ui = SwaggerUIBundle({
+            url: '{{openapi_uri}}',
+            dom_id: '#swagger-ui',
+            presets: [
+                SwaggerUIBundle.presets.apis,
+                SwaggerUIBundle.SwaggerUIStandalonePreset
+            ],
+            layout: "BaseLayout"
 
-    })
+        })
     </script>
 {% endblock %}
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/base.py` & `Flask-AppBuilder-4.3.4rc1/tests/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 import json
 import logging
 from typing import Any, Dict, List, Optional, Set
 import unittest
 
 from flask import Flask, Response
 from flask.testing import FlaskClient
@@ -9,15 +10,22 @@
 from flask_appbuilder.const import (
     API_SECURITY_PASSWORD_KEY,
     API_SECURITY_PROVIDER_KEY,
     API_SECURITY_REFRESH_KEY,
     API_SECURITY_USERNAME_KEY,
     API_SECURITY_VERSION,
 )
+from hiro import Timeline
 import jinja2
+from tests.const import (
+    PASSWORD_ADMIN,
+    PASSWORD_READONLY,
+    USERNAME_ADMIN,
+    USERNAME_READONLY,
+)
 
 
 class FABTestCase(unittest.TestCase):
     @staticmethod
     def auth_client_get(client, token, uri):
         return client.get(uri, headers={"Authorization": f"Bearer {token}"})
 
@@ -90,47 +98,67 @@
                         response[idx][field_name], expected_result[field_name]
                     )
 
     @staticmethod
     def browser_logout(client):
         return client.get("/logout/")
 
+    def create_default_users(self, appbuilder) -> None:
+        with Timeline(start=datetime(2020, 1, 1), scale=0).freeze():
+            self.create_admin_user(self.appbuilder, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        with Timeline(start=datetime(2020, 1, 1), scale=0).freeze():
+            self.create_user(
+                self.appbuilder,
+                USERNAME_READONLY,
+                PASSWORD_READONLY,
+                "ReadOnly",
+                first_name="readonly",
+                last_name="readonly",
+                email="readonly@fab.org",
+            )
+
     def create_admin_user(self, appbuilder, username, password):
         self.create_user(appbuilder, username, password, "Admin")
 
     @staticmethod
     def create_user(
         appbuilder,
         username,
         password,
         role_name,
         first_name="admin",
         last_name="user",
         email="admin@fab.org",
         role_names=None,
     ):
+        user = appbuilder.sm.find_user(username=username)
+        if user:
+            appbuilder.session.delete(user)
+            appbuilder.session.commit()
         roles = (
             [appbuilder.sm.find_role(role_name) for role_name in role_names]
             if role_names
             else [appbuilder.sm.find_role(role_name)]
         )
         return appbuilder.sm.add_user(
             username, first_name, last_name, email, roles, password
         )
 
 
 class BaseMVCTestCase(FABTestCase):
     def setUp(self):
         self.app = Flask(__name__)
         self.app.jinja_env.undefined = jinja2.StrictUndefined
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         logging.basicConfig(level=logging.ERROR)
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
+        self.create_default_users(self.appbuilder)
 
     @property
     def registered_endpoints(self) -> Set:
         return {item.endpoint for item in self.app.url_map.iter_rules()}
 
     def get_registered_view_endpoints(self, view_name) -> Set:
         return {
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/config_oauth.py` & `Flask-AppBuilder-4.3.4rc1/tests/config_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/config_security_api.py` & `Flask-AppBuilder-4.3.4rc1/tests/config_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/mongoengine/models.py` & `Flask-AppBuilder-4.3.4rc1/tests/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_auth_ldap.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_auth_ldap.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import unittest
 from unittest.mock import Mock
 
 from flask import Flask
 from flask_appbuilder import AppBuilder, SQLA
 from flask_appbuilder.security.manager import AUTH_LDAP
 from flask_appbuilder.security.sqla.models import User
-from flask_appbuilder.tests.const import USERNAME_ADMIN, USERNAME_READONLY
 import jinja2
 import ldap
-
+from tests.const import USERNAME_ADMIN, USERNAME_READONLY
+from tests.fixtures.users import create_default_users
 
 logging.basicConfig(format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
 logging.getLogger().setLevel(logging.DEBUG)
 log = logging.getLogger(__name__)
 
 
 class LDAPSearchTestCase(unittest.TestCase):
     def setUp(self):
         # start MockLdap
         # start Flask
         self.app = Flask(__name__)
         self.app.jinja_env.undefined = jinja2.StrictUndefined
         self.app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get(
-            "SQLALCHEMY_DATABASE_URI"
+            "SQLALCHEMY_DATABASE_URI", "sqlite:///"
         )
         self.app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
         self.app.config["AUTH_TYPE"] = AUTH_LDAP
         self.app.config["AUTH_LDAP_SERVER"] = "ldap://localhost:1389/"
         self.app.config["AUTH_LDAP_UID_FIELD"] = "uid"
         self.app.config["AUTH_LDAP_FIRSTNAME_FIELD"] = "givenName"
         self.app.config["AUTH_LDAP_LASTNAME_FIELD"] = "sn"
@@ -57,16 +57,16 @@
 
         # stop Database
         self.db.session.remove()
         self.db = None
 
     def assertOnlyDefaultUsers(self):
         users = self.appbuilder.sm.get_all_users()
-        user_names = [user.username for user in users]
-        self.assertEqual(user_names, [USERNAME_ADMIN, USERNAME_READONLY])
+        user_names = sorted([user.username for user in users])
+        self.assertEqual(user_names, [USERNAME_READONLY, USERNAME_ADMIN])
 
     def assertUserContainsRoles(self, user: User, role_names: List[str]):
         user_role_names = sorted([role.name for role in user.roles])
         self.assertListEqual(user_role_names, sorted(role_names))
 
     # ----------------
     # Unit Tests
@@ -76,14 +76,15 @@
         LDAP: test `_search_ldap` method
         """
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # prepare `con` object
         con = ldap.initialize("ldap://localhost:1389/")
         sm._ldap_bind_indirect(ldap, con)
 
         # run `_search_ldap` method
         user_dn, user_attributes = sm._search_ldap(ldap, con, "alice")
@@ -105,14 +106,15 @@
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config[
             "AUTH_LDAP_SEARCH_FILTER"
         ] = "(memberOf=cn=staff,ou=groups,dc=example,dc=org)"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # prepare `con` object
         con = ldap.initialize("ldap://localhost:1389/")
         sm._ldap_bind_indirect(ldap, con)
 
         # run `_search_ldap` method
         user_dn, user_attributes = sm._search_ldap(ldap, con, "alice")
@@ -128,14 +130,15 @@
         LDAP: test `_search_ldap` method w/returned search referrals
         """
         self.app.config["AUTH_LDAP_BIND_USER"] = "uid=admin,ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         user_alice = (
             "cn=alice,ou=users,dc=example,dc=org",
             {
                 "uid": ["alice"],
                 "userPassword": ["alice_password"],
                 "memberOf": [b"cn=staff,ou=groups,o=test"],
@@ -169,14 +172,15 @@
 
     def test__missing_credentials(self):
         """
         LDAP: test login flow for - missing credentials
         """
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # validate - login failure (missing username)
         self.assertIsNone(sm.auth_user_ldap(None, "password"))
         self.assertIsNone(sm.auth_user_ldap("", "password"))
@@ -192,22 +196,23 @@
         self.assertIsNone(sm.auth_user_ldap(None, ""))
 
         # validate - no users were created
         self.assertOnlyDefaultUsers()
 
     def test__active_user(self):
         """
-        LDAP: test login flow for - inactive user
+        LDAP: test login flow for - active user
         """
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(
             username="alice",
@@ -235,14 +240,15 @@
         """
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(
             username="alice",
@@ -276,14 +282,15 @@
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -312,14 +319,15 @@
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_ldap("alice", "alice_password")
 
@@ -344,14 +352,15 @@
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_USER_REGISTRATION"] = False
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_ldap("alice", "alice_password")
 
@@ -368,14 +377,15 @@
         self.app.config["AUTH_LDAP_SEARCH"] = None
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_ldap("alice", "alice_password")
 
@@ -388,14 +398,15 @@
         """
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(  # noqa
             username="alice",
@@ -420,14 +431,15 @@
         """
         self.app.config["AUTH_LDAP_SEARCH"] = None
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(  # noqa
             username="alice",
@@ -453,14 +465,15 @@
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_ldap("alice", "alice_password")
 
@@ -484,14 +497,15 @@
         """  # noqa
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_USER_REGISTRATION"] = False
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_ldap("alice", "alice_password")
 
@@ -508,14 +522,15 @@
         self.app.config["AUTH_LDAP_SEARCH"] = None
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_ldap("alice", "alice_password")
 
@@ -528,14 +543,15 @@
         LDAP: test login flow for - indirect bind - registered user
         """
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(  # noqa
             username="alice",
@@ -559,14 +575,15 @@
         LDAP: test login flow for - indirect bind - registered user - no ldap search
         """
         self.app.config["AUTH_LDAP_SEARCH"] = None
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(  # noqa
             username="alice",
@@ -597,14 +614,15 @@
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -636,14 +654,15 @@
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -674,14 +693,15 @@
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = False
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -716,14 +736,15 @@
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = True
         self.app.config[
             "AUTH_LDAP_USERNAME_FORMAT"
         ] = "cn=%s,ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -758,14 +779,15 @@
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -796,14 +818,15 @@
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -833,14 +856,15 @@
         }
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = False
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -874,14 +898,15 @@
         }
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = True
         self.app.config["AUTH_LDAP_SEARCH"] = "ou=users,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_USER"] = "cn=admin,dc=example,dc=org"
         self.app.config["AUTH_LDAP_BIND_PASSWORD"] = "admin_password"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_auth_oauth.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_auth_oauth.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import os
 import unittest
 
 from flask import Flask
 from flask_appbuilder import AppBuilder, SQLA
 from flask_appbuilder.const import AUTH_OAUTH
 import jinja2
-
-from ..const import USERNAME_ADMIN, USERNAME_READONLY
+from tests.const import USERNAME_ADMIN, USERNAME_READONLY
+from tests.fixtures.users import create_default_users
 
 logging.basicConfig(format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
 logging.getLogger().setLevel(logging.DEBUG)
 log = logging.getLogger(__name__)
 
 
 class OAuthRegistrationRoleTestCase(unittest.TestCase):
     def setUp(self):
         # start Flask
         self.app = Flask(__name__)
         self.app.jinja_env.undefined = jinja2.StrictUndefined
         self.app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get(
-            "SQLALCHEMY_DATABASE_URI"
+            "SQLALCHEMY_DATABASE_URI", "sqlite:///"
         )
         self.app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
         self.app.config["AUTH_TYPE"] = AUTH_OAUTH
         self.app.config[
             "OAUTH_PROVIDERS"
         ] = []  # can be empty, because we dont use the external providers in tests
 
@@ -46,16 +46,16 @@
 
         # stop Database
         self.db.session.remove()
         self.db = None
 
     def assertOnlyDefaultUsers(self):
         users = self.appbuilder.sm.get_all_users()
-        user_names = [user.username for user in users]
-        self.assertEqual(user_names, [USERNAME_ADMIN, USERNAME_READONLY])
+        user_names = sorted([user.username for user in users])
+        self.assertEqual(user_names, [USERNAME_READONLY, USERNAME_ADMIN])
 
     # ----------------
     # Userinfo Objects
     # ----------------
     userinfo_alice = {
         "username": "alice",
         "first_name": "Alice",
@@ -69,15 +69,15 @@
     # ----------------
     def test__inactive_user(self):
         """
         OAUTH: test login flow for - inactive user
         """
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
-
+        create_default_users(self.appbuilder.session)
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # register a user
         new_user = sm.add_user(
             username="alice",
             first_name="Alice",
@@ -100,14 +100,15 @@
 
     def test__missing_username(self):
         """
         OAUTH: test login flow for - missing credentials
         """
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # create userinfo with missing info
         userinfo_missing = self.userinfo_alice.copy()
         userinfo_missing["username"] = ""
@@ -125,14 +126,15 @@
         """
         OAUTH: test login flow for - unregistered user
         """
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_oauth(self.userinfo_alice)
 
@@ -153,14 +155,15 @@
     def test__unregistered__no_self_register(self):
         """
         OAUTH: test login flow for - unregistered user - no self-registration
         """
         self.app.config["AUTH_USER_REGISTRATION"] = False
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
         # attempt login
         user = sm.auth_user_oauth(self.userinfo_alice)
 
@@ -179,14 +182,15 @@
             "GROUP_1": ["Admin"],
             "GROUP_2": ["User"],
         }
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -196,18 +200,17 @@
         # validate - user was allowed to log in
         self.assertIsInstance(user, sm.user_model)
 
         # validate - user was registered
         self.assertEqual(len(sm.get_all_users()), 3)
 
         # validate - user was given the correct roles
-        self.assertListEqual(
-            user.roles,
-            [sm.find_role("Admin"), sm.find_role("Public"), sm.find_role("User")],
-        )
+        self.assertIn(sm.find_role("Admin"), user.roles)
+        self.assertIn(sm.find_role("User"), user.roles)
+        self.assertIn(sm.find_role("Public"), user.roles)
 
         # validate - user was given the correct attributes (read from LDAP)
         self.assertEqual(user.first_name, "Alice")
         self.assertEqual(user.last_name, "Doe")
         self.assertEqual(user.email, "alice@example.com")
 
     def test__unregistered__multi_role(self):
@@ -215,14 +218,15 @@
         OAUTH: test login flow for - unregistered user - multi role mapping
         """
         self.app.config["AUTH_ROLES_MAPPING"] = {"GROUP_1": ["Admin", "User"]}
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config["AUTH_USER_REGISTRATION_ROLE"] = "Public"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -232,18 +236,17 @@
         # validate - user was allowed to log in
         self.assertIsInstance(user, sm.user_model)
 
         # validate - user was registered
         self.assertEqual(len(sm.get_all_users()), 3)
 
         # validate - user was given the correct roles
-        self.assertListEqual(
-            user.roles,
-            [sm.find_role("Admin"), sm.find_role("Public"), sm.find_role("User")],
-        )
+        self.assertIn(sm.find_role("Admin"), user.roles)
+        self.assertIn(sm.find_role("Public"), user.roles)
+        self.assertIn(sm.find_role("User"), user.roles)
 
         # validate - user was given the correct attributes (read from LDAP)
         self.assertEqual(user.first_name, "Alice")
         self.assertEqual(user.last_name, "Doe")
         self.assertEqual(user.email, "alice@example.com")
 
     def test__unregistered__jmespath_role(self):
@@ -252,14 +255,15 @@
         """
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config[
             "AUTH_USER_REGISTRATION_ROLE_JMESPATH"
         ] = "contains(['alice'], username) && 'User' || 'Public'"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -284,14 +288,15 @@
         """
         OAUTH: test login flow for - registered user - multi role mapping - no login role-sync
         """  # noqa
         self.app.config["AUTH_ROLES_MAPPING"] = {"GROUP_1": ["Admin", "User"]}
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = False
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -320,14 +325,15 @@
         """
         OAUTH: test login flow for - registered user - multi role mapping - with login role-sync
         """  # noqa
         self.app.config["AUTH_ROLES_MAPPING"] = {"GROUP_1": ["Admin", "User"]}
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = True
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -359,14 +365,15 @@
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = False
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config[
             "AUTH_USER_REGISTRATION_ROLE_JMESPATH"
         ] = "contains(['alice'], username) && 'User' || 'Public'"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
 
@@ -398,14 +405,15 @@
         self.app.config["AUTH_ROLES_SYNC_AT_LOGIN"] = True
         self.app.config["AUTH_USER_REGISTRATION"] = True
         self.app.config[
             "AUTH_USER_REGISTRATION_ROLE_JMESPATH"
         ] = "contains(['alice'], username) && 'User' || 'Public'"
         self.appbuilder = AppBuilder(self.app, self.db.session)
         sm = self.appbuilder.sm
+        create_default_users(self.appbuilder.session)
 
         # add User role
         sm.add_role("User")
 
         # validate - no users are registered
         self.assertOnlyDefaultUsers()
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_base_security_manager.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_base_security_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_mvc_security.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_mvc_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from unittest.mock import patch
 
 from flask_appbuilder import ModelView
 from flask_appbuilder.exceptions import PasswordComplexityValidationError
 from flask_appbuilder.models.sqla.filters import FilterEqual
 from flask_appbuilder.models.sqla.interface import SQLAInterface
 from flask_appbuilder.security.sqla.models import User
-
-from ..base import BaseMVCTestCase
-from ..const import (
+from tests.base import BaseMVCTestCase
+from tests.const import (
     INVALID_LOGIN_STRING,
     PASSWORD_ADMIN,
     PASSWORD_READONLY,
     USERNAME_ADMIN,
     USERNAME_READONLY,
 )
-from ..sqla.models import Model1, Model2
+from tests.fixtures.data_models import model1_data
+from tests.sqla.models import Model1, Model2
 
 PASSWORD_COMPLEXITY_ERROR = (
     "Must have at least two capital letters, "
     "one special character, two digits, three lower case letters and "
     "a minimal length of 10"
 )
 
@@ -237,44 +237,49 @@
 
     def test_auth_builtin_roles(self):
         """
         Test Security builtin roles readonly
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_READONLY, PASSWORD_READONLY)
-        # Test authorized GET
-        rv = client.get("/model1view/list/")
-        self.assertEqual(rv.status_code, 200)
-        # Test authorized SHOW
-        rv = client.get("/model1view/show/1")
-        self.assertEqual(rv.status_code, 200)
-        # Test unauthorized EDIT
-        rv = client.get("/model1view/edit/1")
-        self.assertEqual(rv.status_code, 302)
-        # Test unauthorized DELETE
-        rv = client.get("/model1view/delete/1")
-        self.assertEqual(rv.status_code, 302)
+        with model1_data(self.appbuilder.session, 1):
+            # Test authorized GET
+            rv = client.get("/model1view/list/")
+            self.assertEqual(rv.status_code, 200)
+            # Test authorized SHOW
+            rv = client.get("/model1view/show/1")
+            self.assertEqual(rv.status_code, 200)
+            # Test unauthorized EDIT
+            rv = client.get("/model1view/edit/1")
+            self.assertEqual(rv.status_code, 302)
+            # Test unauthorized DELETE
+            rv = client.get("/model1view/delete/1")
+            self.assertEqual(rv.status_code, 302)
 
     def test_sec_reset_password(self):
         """
         Test Security reset password
         """
         client = self.app.test_client()
-
+        admin_user = self.appbuilder.sm.find_user(username=USERNAME_ADMIN)
         # Try Reset My password
-        rv = client.get("/users/action/resetmypassword/1", follow_redirects=True)
+        rv = client.get(
+            f"/users/action/resetmypassword/{admin_user.id}", follow_redirects=True
+        )
         # Werkzeug update to 0.15.X sends this action to wrong redirect
         # Old test was:
         # data = rv.data.decode("utf-8")
         # ok_(ACCESS_IS_DENIED in data)
         self.assertEqual(rv.status_code, 404)
 
         # Reset My password
         _ = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = client.get("/users/action/resetmypassword/1", follow_redirects=True)
+        rv = client.get(
+            f"/users/action/resetmypassword/{admin_user.id}", follow_redirects=True
+        )
         data = rv.data.decode("utf-8")
         self.assertIn("Reset Password Form", data)
         rv = client.post(
             "/resetmypassword/form",
             data=dict(password="password", conf_password="password"),
             follow_redirects=True,
         )
@@ -285,15 +290,17 @@
             "/resetmypassword/form",
             data=dict(password=PASSWORD_ADMIN, conf_password=PASSWORD_ADMIN),
             follow_redirects=True,
         )
         self.assertEqual(rv.status_code, 200)
 
         # Reset Password Admin
-        rv = client.get("/users/action/resetpasswords/1", follow_redirects=True)
+        rv = client.get(
+            f"/users/action/resetpasswords/{admin_user.id}", follow_redirects=True
+        )
         data = rv.data.decode("utf-8")
         self.assertIn("Reset Password Form", data)
         rv = client.post(
             "/resetmypassword/form",
             data=dict(password=PASSWORD_ADMIN, conf_password=PASSWORD_ADMIN),
             follow_redirects=True,
         )
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_password_complexity.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_password_complexity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/security/test_rate_limiter.py` & `Flask-AppBuilder-4.3.4rc1/tests/security/test_rate_limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 
 from flask import Flask
 from flask_appbuilder import AppBuilder, BaseView, SQLA
-from flask_appbuilder.tests.base import FABTestCase
+from flask_appbuilder.api import BaseApi, expose
+from flask_appbuilder.security.decorators import limit
 import hiro
 import jinja2
+from tests.base import FABTestCase
 
 from ..const import INVALID_LOGIN_STRING, PASSWORD_ADMIN, USERNAME_ADMIN
-from ...api import BaseApi, expose
-from ...security.decorators import limit
 
 
 class LimiterTestCase(FABTestCase):
     def setUp(self):
         self.app = Flask(__name__)
         self.app.jinja_env.undefined = jinja2.StrictUndefined
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["RATELIMIT_ENABLED"] = True
         self.app.config["AUTH_RATE_LIMITED"] = True
         self.app.config["AUTH_RATE_LIMIT"] = "2 per 5 second"
         logging.basicConfig(level=logging.ERROR)
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_addon.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_addon.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import logging
 import os
 
 from flask_appbuilder import SQLA
-from flask_appbuilder.tests.A_fixture.addon_manager import DummyAddOnManager
+from tests.fixtures.addon_manager import DummyAddOnManager
 
 from .base import FABTestCase
 
 
 log = logging.getLogger(__name__)
 
 
 class FlaskTestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["ADDON_MANAGERS"] = [
-            "flask_appbuilder.tests.A_fixture.addon_manager.DummyAddOnManager"
+            "tests.fixtures.addon_manager.DummyAddOnManager"
         ]
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def tearDown(self):
         self.appbuilder = None
         self.app = None
         self.db = None
 
     def test_addon_import(self):
         self.assertIsInstance(
             self.appbuilder.addon_managers[
-                "flask_appbuilder.tests.A_fixture.addon_manager.DummyAddOnManager"
+                "tests.fixtures.addon_manager.DummyAddOnManager"
             ],
             DummyAddOnManager,
         )
 
     def test_addon_register_views(self):
         client = self.app.test_client()
         rv = client.get("/dummy/method1/test1")
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_api.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,29 +31,36 @@
     API_URI_RIS_KEY,
 )
 from flask_appbuilder.hooks import before_request
 from flask_appbuilder.models.sqla.filters import FilterGreater, FilterSmaller
 from flask_appbuilder.models.sqla.interface import SQLAInterface
 import prison
 from sqlalchemy.sql.expression import func
-
-from .base import FABTestCase
-from .const import (
+from tests.base import FABTestCase
+from tests.const import (
     MAX_PAGE_SIZE,
     MODEL1_DATA_SIZE,
     MODEL2_DATA_SIZE,
     MODELOMCHILD_DATA_SIZE,
     PASSWORD_ADMIN,
     PASSWORD_READONLY,
     USERNAME_ADMIN,
     USERNAME_READONLY,
 )
-from .sqla.models import (
-    insert_model1,
-    insert_model2,
+from tests.fixtures.data_models import (
+    model1_data,
+    model2_data,
+    model4_data,
+    model_mm_parent_data,
+    model_om_parent_data,
+    model_oo_parent_data,
+    model_with_enums_data,
+    model_with_property_data,
+)
+from tests.sqla.models import (
     Model1,
     Model2,
     Model4,
     ModelMMChild,
     ModelMMParent,
     ModelMMParentRequired,
     ModelOMChild,
@@ -71,21 +78,23 @@
 class APICSRFTestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_wtf import CSRFProtect
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["WTF_CSRF_ENABLED"] = True
 
         self.csrf = CSRFProtect(self.app)
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
+        self.create_default_users(self.appbuilder)
+
     def test_auth_login(self):
         """
         REST Api: Test auth login CSRF
         """
         client = self.app.test_client()
         rv = self._login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         self.assertEqual(rv.status_code, 200)
@@ -108,15 +117,15 @@
     ]
 
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_ADD_SECURITY_VIEWS"] = False
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def test_disabled_security_views(self):
         """
@@ -131,15 +140,15 @@
     openapi_fab_endpoint = ["OpenApi.get", "SwaggerView.show"]
 
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_ADD_OPENAPI_VIEWS"] = False
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def test_disabled_security_views(self):
         """
@@ -162,26 +171,28 @@
             expose,
             rison,
             safe,
         )
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_API_MAX_PAGE_SIZE"] = MAX_PAGE_SIZE
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
         rison_schema = {
             "type": "object",
             "required": ["number"],
             "properties": {"number": {"type": "number"}},
         }
 
+        self.create_default_users(self.appbuilder)
+
         class Base1Api(BaseApi):
             @expose("/test1")
             @protect()
             @safe
             @rison(rison_schema)
             def test1(self, **kwargs):
                 return self.response(200, message=f"{kwargs['rison']['number'] + 1}")
@@ -611,43 +622,45 @@
 
     def test_auth_authorization_browser(self):
         """
         REST Api: Test auth with browser login
         """
         client = self.app.test_client()
         rv = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        # Test access with browser login
-        uri = "api/v1/model1browserlogin/1"
-        rv = client.get(uri)
-        self.assertEqual(rv.status_code, 200)
-        # Test unauthorized access with browser login
-        uri = "api/v1/model1api/1"
-        rv = client.get(uri)
-        self.assertEqual(rv.status_code, 401)
-        # Test access without cookie or JWT
-        rv = self.browser_logout(client)
-        # Test access with browser login
-        uri = "api/v1/model1browserlogin/1"
-        rv = client.get(uri)
-        self.assertEqual(rv.status_code, 401)
-        # Test access with JWT but without cookie
-        token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        uri = "api/v1/model1browserlogin/1"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+
+            # Test access with browser login
+            uri = f"api/v1/model1browserlogin/{model_id}"
+            rv = client.get(uri)
+            self.assertEqual(rv.status_code, 200)
+            # Test unauthorized access with browser login
+            uri = "api/v1/model1api/1"
+            rv = client.get(uri)
+            self.assertEqual(rv.status_code, 401)
+            # Test access without cookie or JWT
+            rv = self.browser_logout(client)
+            # Test access with browser login
+            uri = "api/v1/model1browserlogin/1"
+            rv = client.get(uri)
+            self.assertEqual(rv.status_code, 401)
+            # Test access with JWT but without cookie
+            token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+            uri = f"api/v1/model1browserlogin/{model_id}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
 
     def test_auth_authorization(self):
         """
         REST Api: Test auth base limited authorization
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         # Test unauthorized DELETE
-        pk = 1
-        uri = f"api/v1/model1apirestrictedpermissions/{pk}"
+        uri = "api/v1/model1apirestrictedpermissions/10"
 
         rv = self.auth_client_delete(client, token, uri)
         self.assertEqual(rv.status_code, 403)
 
         # Test unauthorized POST
         item = dict(
             field_string="test{}".format(MODEL1_DATA_SIZE + 1),
@@ -657,17 +670,20 @@
         )
         uri = "api/v1/model1apirestrictedpermissions/"
 
         rv = self.auth_client_post(client, token, uri, item)
         self.assertEqual(rv.status_code, 403)
 
         # Test authorized GET
-        uri = f"api/v1/model1apirestrictedpermissions/{pk}"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1):
+            model = self.appbuilder.get_session.query(Model1).first()
+            model_id = model.id
+            uri = f"api/v1/model1apirestrictedpermissions/{model_id}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
 
     def test_auth_builtin_roles(self):
         """
         REST Api: Test auth readonly builtin role
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_READONLY, PASSWORD_READONLY)
@@ -685,17 +701,19 @@
             field_date=None,
         )
         uri = "api/v1/model1api/"
         rv = self.auth_client_post(client, token, uri, item)
         self.assertEqual(rv.status_code, 403)
 
         # Test authorized GET
-        uri = "api/v1/model1api/1"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            uri = f"api/v1/model1api/{model_id}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
 
         # Test authorized INFO
         uri = "api/v1/model1api/_info"
         rv = self.auth_client_get(client, token, uri)
         self.assertEqual(rv.status_code, 200)
 
     def test_base_rison_argument(self):
@@ -790,17 +808,19 @@
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         uri = "api/v1/model1apiincluderoutes/_info"
         rv = self.auth_client_get(client, token, uri)
         self.assertEqual(rv.status_code, 404)
 
-        uri = "api/v1/model1apiincluderoutes/1"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            uri = f"api/v1/model1apiincluderoutes/{model_id}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
 
         # Check that permissions do not exist
         pvm = self.appbuilder.sm.find_permission_view_menu(
             "can_info", "Model1ApiIncludeRoutes"
         )
         self.assertIsNone(pvm)
         pvm = self.appbuilder.sm.find_permission_view_menu(
@@ -813,24 +833,22 @@
         self.assertIsNone(pvm)
         pvm = self.appbuilder.sm.find_permission_view_menu(
             "can_delete", "Model1ApiIncludeRoutes"
         )
         self.assertIsNone(pvm)
 
     def test_get_item(self):
-        """
-        REST Api: Test get item
-        """
-        client = self.app.test_client()
-        token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        for i in range(1, MODEL1_DATA_SIZE):
-            rv = self.auth_client_get(client, token, "api/v1/model1api/{}".format(i))
+        with model1_data(self.appbuilder.session, 1) as models:
+            client = self.app.test_client()
+            model_id = models[0].id
+            token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+            rv = self.auth_client_get(client, token, f"api/v1/model1api/{model_id}")
             data = json.loads(rv.data.decode("utf-8"))
             self.assertEqual(rv.status_code, 200)
-            self.assert_get_item(rv, data, i - 1)
+            self.assert_get_item(rv, data, 0)
 
     def assert_get_item(self, rv, data, value):
         self.assertEqual(
             data[API_RESULT_RES_KEY],
             {
                 "field_date": None,
                 "field_float": float(value),
@@ -856,22 +874,23 @@
 
     def test_get_item_select_cols(self):
         """
         REST Api: Test get item with select columns
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-
-        for i in range(1, MODEL1_DATA_SIZE):
-            uri = "api/v1/model1api/{}?q=({}:!(field_integer))".format(
-                i, API_SELECT_COLUMNS_RIS_KEY
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            uri = (
+                f"api/v1/model1api/{model_id}?"
+                f"q=({API_SELECT_COLUMNS_RIS_KEY}:!(field_integer))"
             )
             rv = self.auth_client_get(client, token, uri)
             data = json.loads(rv.data.decode("utf-8"))
-            self.assertEqual(data[API_RESULT_RES_KEY], {"field_integer": i - 1})
+            self.assertEqual(data[API_RESULT_RES_KEY], {"field_integer": 0})
             self.assertEqual(
                 data[API_DESCRIPTION_COLUMNS_RES_KEY],
                 {"field_integer": "Field Integer"},
             )
             self.assertEqual(
                 data[API_LABEL_COLUMNS_RES_KEY], {"field_integer": "Field Integer"}
             )
@@ -879,371 +898,410 @@
 
     def test_get_item_dotted_mo_notation(self):
         """
         REST Api: Test get item with dotted M-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model2 = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model2.id
-        uri = f"api/v1/model2dottednotationapi/{pk}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY],
-            {"field_string": "test0", "group": {"field_string": "test0"}},
-        )
-        self.assertEqual(rv.status_code, 200)
+        with model2_data(self.appbuilder.session, 1) as models:
+
+            model2_id = models[0].id
+            uri = f"api/v1/model2dottednotationapi/{model2_id}"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY],
+                {"field_string": "test0", "group": {"field_string": "test0"}},
+            )
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_item_select_meta_data(self):
         """
         REST Api: Test get item select meta data
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         selectable_keys = [
             API_DESCRIPTION_COLUMNS_RIS_KEY,
             API_LABEL_COLUMNS_RIS_KEY,
             API_SHOW_COLUMNS_RIS_KEY,
             API_SHOW_TITLE_RIS_KEY,
         ]
-        for selectable_key in selectable_keys:
-            argument = {API_SELECT_KEYS_RIS_KEY: [selectable_key]}
-            uri = "api/v1/model1api/1?{}={}".format(
-                API_URI_RIS_KEY, prison.dumps(argument)
-            )
-            rv = self.auth_client_get(client, token, uri)
-            data = json.loads(rv.data.decode("utf-8"))
-            self.assertEqual(len(data.keys()), 1 + 2)  # always exist id, result
-            # We assume that rison meta key equals result meta key
-            assert selectable_key in data
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            for selectable_key in selectable_keys:
+                argument = {API_SELECT_KEYS_RIS_KEY: [selectable_key]}
+                uri = (
+                    f"api/v1/model1api/{model_id}?"
+                    f"{API_URI_RIS_KEY}={prison.dumps(argument)}"
+                )
+                rv = self.auth_client_get(client, token, uri)
+                data = json.loads(rv.data.decode("utf-8"))
+                self.assertEqual(len(data.keys()), 1 + 2)  # always exist id, result
+                # We assume that rison meta key equals result meta key
+                assert selectable_key in data
 
     def test_get_item_excluded_cols(self):
         """
         REST Api: Test get item with excluded columns
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        pk = 1
-        rv = self.auth_client_get(
-            client, token, "api/v1/model1apiexcludecols/{}".format(pk)
-        )
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data[API_RESULT_RES_KEY], {"field_string": "test0"})
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            rv = self.auth_client_get(
+                client, token, f"api/v1/model1apiexcludecols/{model_id}"
+            )
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data[API_RESULT_RES_KEY], {"field_string": "test0"})
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_item_not_found(self):
         """
         REST Api: Test get item not found
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-
-        pk = MODEL1_DATA_SIZE + 1
-        rv = self.auth_client_get(client, token, "api/v1/model1api/{}".format(pk))
-        self.assertEqual(rv.status_code, 404)
+        with model1_data(self.appbuilder.session, 1):
+            model_id = MODEL1_DATA_SIZE + 1
+            rv = self.auth_client_get(client, token, f"api/v1/model1api/{model_id}")
+            self.assertEqual(rv.status_code, 404)
 
     def test_get_item_base_filters(self):
         """
         REST Api: Test get item with base filters
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        pk = 1
-        rv = self.auth_client_get(
-            client, token, "api/v1/model1apifiltered/{}".format(pk)
-        )
-        self.assertEqual(rv.status_code, 404)
-        # This one is ok pk=4 field_integer=3 2>3<4
-        pk = 4
-        rv = self.auth_client_get(client, token, f"api/v1/model1apifiltered/{pk}")
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 5):
+            # We can't get a base filtered item
+            filtered_model_id = (
+                self.appbuilder.session.query(Model1)
+                .filter(Model1.field_integer == 4)
+                .one_or_none()
+                .id
+            )
+            rv = self.auth_client_get(
+                client, token, f"api/v1/model1apifiltered/{filtered_model_id}"
+            )
+            self.assertEqual(rv.status_code, 404)
+            model_id = (
+                self.appbuilder.session.query(Model1)
+                .filter(Model1.field_integer == 3)
+                .one_or_none()
+                .id
+            )
+            rv = self.auth_client_get(
+                client, token, f"api/v1/model1apifiltered/{model_id}"
+            )
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_item_mo_field(self):
         """
         REST Api: Test get item with M-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        model2 = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model2.id
-        rv = self.auth_client_get(client, token, f"api/v1/model2api/{pk}")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        expected_rel_field = {
-            "group": {
-                "field_date": None,
-                "field_float": 0.0,
-                "field_integer": 0,
-                "field_string": "test0",
-                "id": 1,
+        with model2_data(self.appbuilder.session, 1) as models:
+            pk = models[0].id
+            rv = self.auth_client_get(client, token, f"api/v1/model2api/{pk}")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            expected_rel_field = {
+                "group": {
+                    "field_date": None,
+                    "field_float": 0.0,
+                    "field_integer": 0,
+                    "field_string": "test0",
+                    "id": models[0].group.id,
+                }
             }
-        }
-        self.assertEqual(data[API_RESULT_RES_KEY], expected_rel_field)
+            self.assertEqual(data[API_RESULT_RES_KEY], expected_rel_field)
 
     def test_get_item_mm_field(self):
         """
         REST Api: Test get item with M-M related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        pk = 1
-        rv = self.auth_client_get(client, token, f"api/v1/modelmmapi/{pk}")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        expected_rel_field = [
-            {"field_string": "1", "field_integer": 1, "id": 1},
-            {"field_string": "2", "field_integer": 2, "id": 2},
-            {"field_string": "3", "field_integer": 3, "id": 3},
-        ]
-        self.assertEqual(data[API_RESULT_RES_KEY]["children"], expected_rel_field)
+        with model_mm_parent_data(self.appbuilder.session, 1, 4) as models:
+            model_id = models[0].id
+            rv = self.auth_client_get(client, token, f"api/v1/modelmmapi/{model_id}")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            expected_rel_field = [
+                {
+                    "field_string": child.field_string,
+                    "field_integer": child.field_integer,
+                    "id": child.id,
+                }
+                for child in models[0].children
+            ]
+            self.assertEqual(data[API_RESULT_RES_KEY]["children"], expected_rel_field)
 
     def test_get_item_dotted_mm_field(self):
         """
         REST Api: Test get item with dotted M-M related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        pk = 1
-        rv = self.auth_client_get(client, token, f"api/v1/modeldottedmmapi/{pk}")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        expected_result = {
-            "field_string": "0",
-            "children": [
-                {"field_integer": 1},
-                {"field_integer": 2},
-                {"field_integer": 3},
-            ],
-        }
-        self.assertEqual(data[API_RESULT_RES_KEY], expected_result)
+        with model_mm_parent_data(self.appbuilder.session, 1, 4) as models:
+            model_id = models[0].id
+            rv = self.auth_client_get(
+                client, token, f"api/v1/modeldottedmmapi/{model_id}"
+            )
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            expected_result = {
+                "field_string": "0",
+                "children": [
+                    {"field_integer": 1},
+                    {"field_integer": 2},
+                    {"field_integer": 3},
+                ],
+            }
+            self.assertEqual(data[API_RESULT_RES_KEY], expected_result)
 
     def test_get_item_oo_field(self):
         """
         REST Api: Test get item with O-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        pk = 1
-        rv = self.auth_client_get(client, token, f"api/v1/modelooparentapi/{pk}")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(
-            data[API_RESULT_RES_KEY],
-            {
-                "field_string": "text0",
-                "child": {"field_string": "text0.child", "id": 1},
-            },
-        )
+        with model_oo_parent_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            rv = self.auth_client_get(
+                client, token, f"api/v1/modelooparentapi/{model_id}"
+            )
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(
+                data[API_RESULT_RES_KEY],
+                {
+                    "field_string": "text0",
+                    "child": {"field_string": "text0.child", "id": models[0].child.id},
+                },
+            )
 
     def test_get_item_dotted_oo_field(self):
         """
         REST Api: Test get item with dotted O-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        pk = 1
-        rv = self.auth_client_get(client, token, f"api/v1/modeldottedooparentapi/{pk}")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(
-            data[API_RESULT_RES_KEY],
-            {"field_string": "text0", "child": {"field_string": "text0.child"}},
-        )
+        with model_oo_parent_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            rv = self.auth_client_get(
+                client, token, f"api/v1/modeldottedooparentapi/{model_id}"
+            )
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(
+                data[API_RESULT_RES_KEY],
+                {"field_string": "text0", "child": {"field_string": "text0.child"}},
+            )
 
     def test_get_item_om_field(self):
         """
         REST Api: Test get item with O-M related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # We can't get a base filtered item
-        pk = 1
-        rv = self.auth_client_get(
-            client, token, "api/v1/modelomparentapi/{}".format(pk)
-        )
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        expected_rel_field = [
-            {"field_string": f"text0.{i}", "id": i}
-            for i in range(1, MODELOMCHILD_DATA_SIZE)
-        ]
-        self.assertEqual(data[API_RESULT_RES_KEY]["children"], expected_rel_field)
+        with model_om_parent_data(
+            self.appbuilder.session, 1, MODELOMCHILD_DATA_SIZE
+        ) as models:
+            model_id = models[0].id
+            rv = self.auth_client_get(
+                client, token, "api/v1/modelomparentapi/{}".format(model_id)
+            )
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            expected_rel_field = [
+                {"field_string": child.field_string, "id": child.id}
+                for child in models[0].children
+            ]
+            self.assertEqual(data[API_RESULT_RES_KEY]["children"], expected_rel_field)
 
     def test_get_list(self):
         """
         REST Api: Test get list
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = self.auth_client_get(client, token, "api/v1/model1api/")
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, "api/v1/model1api/")
 
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
 
     def test_get_list_dotted_mo_field(self):
         """
         REST Api: Test get list with dotted M-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         arguments = {"order_column": "field_string", "order_direction": "asc"}
-        uri = "api/v1/model2dottednotationapi/?{}={}".format(
-            API_URI_RIS_KEY, prison.dumps(arguments)
-        )
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        i = 0
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][i],
-            {"field_string": "test0", "group": {"field_string": "test0"}},
+        uri = (
+            f"api/v1/model2dottednotationapi/?"
+            f"{API_URI_RIS_KEY}={prison.dumps(arguments)}"
         )
+        with model2_data(self.appbuilder.session, MODEL2_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL2_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {"field_string": "test0", "group": {"field_string": "test0"}},
+            )
 
     def test_get_list_om_field(self):
         """
         REST Api: Test get list with O-M related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = self.auth_client_get(client, token, "api/v1/modelomparentapi/")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        expected_rel_field = [
-            {"field_string": f"text0.{i}", "id": i}
-            for i in range(1, MODELOMCHILD_DATA_SIZE)
-        ]
-        self.assertEqual(data[API_RESULT_RES_KEY][0]["children"], expected_rel_field)
+        with model_om_parent_data(
+            self.appbuilder.session, MODEL1_DATA_SIZE, MODELOMCHILD_DATA_SIZE
+        ) as models:
+            rv = self.auth_client_get(client, token, "api/v1/modelomparentapi/")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            expected_rel_field = [
+                {"field_string": child.field_string, "id": child.id}
+                for child in models[0].children
+            ]
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0]["children"], expected_rel_field
+            )
 
     def test_get_list_dotted_om_field(self):
         """
         REST Api: Test get list with dotted O-M related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = self.auth_client_get(client, token, "api/v1/modeldottedomparentapi/")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        expected_rel_field = [
-            {"field_string": f"text0.{i}"} for i in range(1, MODELOMCHILD_DATA_SIZE)
-        ]
-        self.assertEqual(data[API_RESULT_RES_KEY][0]["children"], expected_rel_field)
+        with model_om_parent_data(
+            self.appbuilder.session, MODEL1_DATA_SIZE, MODELOMCHILD_DATA_SIZE
+        ):
+            rv = self.auth_client_get(client, token, "api/v1/modeldottedomparentapi/")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            expected_rel_field = [
+                {"field_string": f"text0.{i}"} for i in range(1, MODELOMCHILD_DATA_SIZE)
+            ]
+            expected_rel_field.sort(key=lambda x: x["field_string"])
+            result_rel_field = data[API_RESULT_RES_KEY][0]["children"]
+            result_rel_field.sort(key=lambda x: x["field_string"])
+            self.assertEqual(result_rel_field, expected_rel_field)
 
     def test_get_list_oo_field(self):
         """
         REST Api: Test get list with O-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = self.auth_client_get(client, token, "api/v1/modelooparentapi/")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        expected_rel_field = {"field_string": "text0.child", "id": 1}
-        self.assertEqual(data[API_RESULT_RES_KEY][0]["child"], expected_rel_field)
+        with model_oo_parent_data(self.appbuilder.session, MODEL1_DATA_SIZE) as models:
+            rv = self.auth_client_get(client, token, "api/v1/modelooparentapi/")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            expected_rel_field = {
+                "field_string": models[0].child.field_string,
+                "id": models[0].child.id,
+            }
+            self.assertEqual(data[API_RESULT_RES_KEY][0]["child"], expected_rel_field)
 
     def test_get_list_dotted_oo_field(self):
         """
         REST Api: Test get list with dotted O-O related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = self.auth_client_get(client, token, "api/v1/modeldottedooparentapi/")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        expected_rel_field = {"field_string": "text0.child"}
-        self.assertEqual(data[API_RESULT_RES_KEY][0]["child"], expected_rel_field)
+        with model_oo_parent_data(self.appbuilder.session, 2):
+            rv = self.auth_client_get(client, token, "api/v1/modeldottedooparentapi/")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(data["count"], 2)
+            expected_rel_field = {"field_string": "text0.child"}
+            self.assertEqual(data[API_RESULT_RES_KEY][0]["child"], expected_rel_field)
 
     def test_get_list_dotted_mm_field(self):
         """
         REST Api: Test get list with dotted M-M related field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         arguments = {"order_column": "field_string", "order_direction": "asc"}
-        uri = (
-            f"api/v1/modeldottedmmapi/?" f"{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        )
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["count"], MODEL2_DATA_SIZE)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.modeldottedmmapi.page_size)
-        i = 0
-        self.assertEqual(data[API_RESULT_RES_KEY][i]["field_string"], "0")
-        self.assertEqual(len(data[API_RESULT_RES_KEY][i]["children"]), 3)
-        self.assertIn({"field_integer": 1}, data[API_RESULT_RES_KEY][i]["children"])
-        self.assertIn({"field_integer": 2}, data[API_RESULT_RES_KEY][i]["children"])
-        self.assertIn({"field_integer": 3}, data[API_RESULT_RES_KEY][i]["children"])
+        uri = f"api/v1/modeldottedmmapi/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+        with model_mm_parent_data(self.appbuilder.session, MODEL2_DATA_SIZE, 4):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(data["count"], MODEL2_DATA_SIZE)
+            self.assertEqual(
+                len(data[API_RESULT_RES_KEY]), self.modeldottedmmapi.page_size
+            )
+            i = 0
+            self.assertEqual(data[API_RESULT_RES_KEY][i]["field_string"], "0")
+            self.assertEqual(len(data[API_RESULT_RES_KEY][i]["children"]), 3)
+            self.assertIn({"field_integer": 1}, data[API_RESULT_RES_KEY][i]["children"])
+            self.assertIn({"field_integer": 2}, data[API_RESULT_RES_KEY][i]["children"])
+            self.assertIn({"field_integer": 3}, data[API_RESULT_RES_KEY][i]["children"])
 
     def test_get_list_dotted_mo_order(self):
         """
         REST Api: Test get list and order dotted M-O notation
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         arguments = {"order_column": "group.field_string", "order_direction": "desc"}
-        uri = "api/v1/model2dottednotationapi/?{}={}".format(
-            API_URI_RIS_KEY, prison.dumps(arguments)
-        )
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        i = 0
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][i],
-            {"field_string": "test9", "group": {"field_string": "test9"}},
+        uri = (
+            f"api/v1/model2dottednotationapi/?"
+            f"{API_URI_RIS_KEY}={prison.dumps(arguments)}"
         )
+        with model2_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            i = 0
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][i],
+                {"field_string": "test9", "group": {"field_string": "test9"}},
+            )
 
     def test_get_list_multiple_dotted_order(self):
         """
         REST Api: Test get list order multiple dotted notation
         """
 
         class Model4Api(ModelRestApi):
@@ -1257,121 +1315,129 @@
         self.appbuilder.add_api(Model4Api)
 
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         # Test order asc for model1_1
         arguments = {"order_column": "model1_1.field_string", "order_direction": "desc"}
-        uri = "api/v1/model4api/?{}={}".format(API_URI_RIS_KEY, prison.dumps(arguments))
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        i = 0
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][i],
-            {
-                "field_string": "test9",
-                "model1_1": {"field_string": "test9"},
-                "model1_2": {"field_string": "test9"},
-            },
-        )
+        uri = f"api/v1/model4api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+        with model4_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            i = 0
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][i],
+                {
+                    "field_string": "test9",
+                    "model1_1": {"field_string": "test9"},
+                    "model1_2": {"field_string": "test9"},
+                },
+            )
 
-        # Test order desc for model1_2
-        arguments = {"order_column": "model1_2.field_string", "order_direction": "asc"}
-        uri = "api/v1/model4api/?{}={}".format(API_URI_RIS_KEY, prison.dumps(arguments))
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        i = 0
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][i],
-            {
-                "field_string": "test0",
-                "model1_1": {"field_string": "test0"},
-                "model1_2": {"field_string": "test0"},
-            },
-        )
+            # Test order desc for model1_2
+            arguments = {
+                "order_column": "model1_2.field_string",
+                "order_direction": "asc",
+            }
+            uri = f"api/v1/model4api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            i = 0
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][i],
+                {
+                    "field_string": "test0",
+                    "model1_1": {"field_string": "test0"},
+                    "model1_2": {"field_string": "test0"},
+                },
+            )
 
     def test_get_list_order(self):
         """
         REST Api: Test get list order params
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         # test string order asc
         arguments = {"order_column": "field_integer", "order_direction": "asc"}
-        uri = "api/v1/model1api/?{}={}".format(API_URI_RIS_KEY, prison.dumps(arguments))
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][0],
-            {
-                "field_date": None,
-                "field_float": 0.0,
-                "field_integer": 0,
-                "field_string": "test0",
-            },
-        )
-        self.assertEqual(rv.status_code, 200)
-        # test string order desc
-        arguments = {"order_column": "field_integer", "order_direction": "desc"}
-        uri = "api/v1/model1api/?{}={}".format(API_URI_RIS_KEY, prison.dumps(arguments))
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][0],
-            {
-                "field_date": None,
-                "field_float": float(MODEL1_DATA_SIZE - 1),
-                "field_integer": MODEL1_DATA_SIZE - 1,
-                "field_string": "test{}".format(MODEL1_DATA_SIZE - 1),
-            },
-        )
-        self.assertEqual(rv.status_code, 200)
+        uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {
+                    "field_date": None,
+                    "field_float": 0.0,
+                    "field_integer": 0,
+                    "field_string": "test0",
+                },
+            )
+            self.assertEqual(rv.status_code, 200)
+            # test string order desc
+            arguments = {"order_column": "field_integer", "order_direction": "desc"}
+            uri = "api/v1/model1api/?{}={}".format(
+                API_URI_RIS_KEY, prison.dumps(arguments)
+            )
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {
+                    "field_date": None,
+                    "field_float": float(MODEL1_DATA_SIZE - 1),
+                    "field_integer": MODEL1_DATA_SIZE - 1,
+                    "field_string": "test{}".format(MODEL1_DATA_SIZE - 1),
+                },
+            )
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_list_base_order(self):
         """
         REST Api: Test get list with base order
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         # test string order asc
-        rv = self.auth_client_get(client, token, "api/v1/model1apiorder/")
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][0],
-            {
-                "field_date": None,
-                "field_float": float(MODEL1_DATA_SIZE - 1),
-                "field_integer": MODEL1_DATA_SIZE - 1,
-                "field_string": "test{}".format(MODEL1_DATA_SIZE - 1),
-            },
-        )
-        # Test override
-        arguments = {"order_column": "field_integer", "order_direction": "asc"}
-        uri = f"api/v1/model1apiorder/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][0],
-            {
-                "field_date": None,
-                "field_float": 0.0,
-                "field_integer": 0,
-                "field_string": "test0",
-            },
-        )
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, "api/v1/model1apiorder/")
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {
+                    "field_date": None,
+                    "field_float": float(MODEL1_DATA_SIZE - 1),
+                    "field_integer": MODEL1_DATA_SIZE - 1,
+                    "field_string": "test{}".format(MODEL1_DATA_SIZE - 1),
+                },
+            )
+            # Test override
+            arguments = {"order_column": "field_integer", "order_direction": "asc"}
+            uri = f"api/v1/model1apiorder/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {
+                    "field_date": None,
+                    "field_float": 0.0,
+                    "field_integer": 0,
+                    "field_string": "test0",
+                },
+            )
 
     def test_get_list_page(self):
         """
         REST Api: Test get list page params
         """
         page_size = 5
         client = self.app.test_client()
@@ -1381,55 +1447,56 @@
         arguments = {
             "page_size": page_size,
             "page": 0,
             "order_column": "field_integer",
             "order_direction": "asc",
         }
         uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][0],
-            {
-                "field_date": None,
-                "field_float": 0.0,
-                "field_integer": 0,
-                "field_string": "test0",
-            },
-        )
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), page_size)
-        # test page one
-        arguments = {
-            "page_size": page_size,
-            "page": 1,
-            "order_column": "field_integer",
-            "order_direction": "asc",
-        }
-        uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {
+                    "field_date": None,
+                    "field_float": 0.0,
+                    "field_integer": 0,
+                    "field_string": "test0",
+                },
+            )
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), page_size)
+            # test page one
+            arguments = {
+                "page_size": page_size,
+                "page": 1,
+                "order_column": "field_integer",
+                "order_direction": "asc",
+            }
+            uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+            rv = self.auth_client_get(client, token, uri)
 
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY][0],
-            {
-                "field_date": None,
-                "field_float": float(page_size),
-                "field_integer": page_size,
-                "field_string": "test{}".format(page_size),
-            },
-        )
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), page_size)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY][0],
+                {
+                    "field_date": None,
+                    "field_float": float(page_size),
+                    "field_integer": page_size,
+                    "field_string": "test{}".format(page_size),
+                },
+            )
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), page_size)
 
-        # test simple page test, mainly because of MSSQL dialect
-        arguments = {"page_size": page_size, "page": 1}
-        uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
+            # test simple page test, mainly because of MSSQL dialect
+            arguments = {"page_size": page_size, "page": 1}
+            uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_list_max_page_size(self):
         """
         REST Api: Test get list max page size config setting
         """
         page_size = 200  # Max is globally set to MAX_PAGE_SIZE
         client = self.app.test_client()
@@ -1439,17 +1506,18 @@
         arguments = {
             "page_size": page_size,
             "page": 0,
             "order_column": "field_integer",
             "order_direction": "asc",
         }
         uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), MAX_PAGE_SIZE)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), MAX_PAGE_SIZE)
 
     def test_get_list_max_page_size_override(self):
         """
         REST Api: Test get list max page size property override
         """
 
         class Model1PageSizeOverride(ModelRestApi):
@@ -1479,17 +1547,18 @@
             "page_size": page_size,
             "page": 0,
             "order_column": "field_integer",
             "order_direction": "asc",
         }
         endpoint = "api/v1/model1pagesizeoverride/"
         uri = f"{endpoint}?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), MODEL1_DATA_SIZE)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), MODEL1_DATA_SIZE)
 
     def test_get_list_filters(self):
         """
         REST Api: Test get list filter params
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1507,40 +1576,42 @@
         uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
         expected_result = {
             "field_date": None,
             "field_float": float(filter_value + 1),
             "field_integer": filter_value + 1,
             "field_string": "test{}".format(filter_value + 1),
         }
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data[API_RESULT_RES_KEY][0], expected_result)
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data[API_RESULT_RES_KEY][0], expected_result)
+            self.assertEqual(rv.status_code, 200)
 
-        # Test with JSON encode content
-        from urllib.parse import quote
+            # Test with JSON encode content
+            from urllib.parse import quote
 
-        uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={quote(json.dumps(arguments))}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data[API_RESULT_RES_KEY][0], expected_result)
-        self.assertEqual(rv.status_code, 200)
+            uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={quote(json.dumps(arguments))}"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data[API_RESULT_RES_KEY][0], expected_result)
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_list_invalid_filters(self):
         """
         REST Api: Test get list filter params
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         arguments = {API_FILTERS_RIS_KEY: [{"col": "field_integer", "opr": "gt"}]}
 
-        uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 400)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 400)
 
     def test_get_list_filters_m_m(self):
         """
         REST Api: Test get list filter params with many to many
         """
         session = self.appbuilder.get_session
 
@@ -1565,24 +1636,25 @@
         rv = self.auth_client_get(client, token, uri)
         data = json.loads(rv.data.decode("utf-8"))
         self.assertEqual(data["count"], 1)
         self.assertEqual(
             data["result"][0]["children"][0]["field_string"], "test_child_tmp"
         )
 
-        arguments = {
-            API_FILTERS_RIS_KEY: [
-                {"col": "children", "opr": "rel_m_m", "value": [1, 2]}
-            ]
-        }
-
-        uri = f"api/v1/modelmmapi/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+        with model_mm_parent_data(self.appbuilder.session, 2, 4) as models:
+            children_ids = [child.id for child in models[0].children]
+            arguments = {
+                API_FILTERS_RIS_KEY: [
+                    {"col": "children", "opr": "rel_m_m", "value": children_ids[2:4]}
+                ]
+            }
+            uri = f"api/v1/modelmmapi/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data["count"], 2)
 
         parent_ = (
             session.query(ModelMMParent)
             .filter_by(field_string="test_tmp")
             .one_or_none()
         )
         child_ = (
@@ -1679,37 +1751,39 @@
             ]
         }
         rison_args = prison.dumps(arguments)
         uri = f"api/v1/model1apisearchfilters/?{API_URI_RIS_KEY}={rison_args}"
 
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["count"], 2)
 
-        arguments = {
-            API_FILTERS_RIS_KEY: [
-                {"col": "field_integer", "opr": "gt", "value": 5},
-                {"col": "field_integer", "opr": "lt", "value": 7},
-                {"col": "field_string", "opr": "sw", "value": "a"},
-            ]
-        }
-        rison_args = prison.dumps(arguments)
-        uri = f"api/v1/model1apisearchfilters/?{API_URI_RIS_KEY}={rison_args}"
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data["count"], 2)
 
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["count"], 1)
-        self.assertEqual(data["result"][0]["field_string"], "abc")
+            arguments = {
+                API_FILTERS_RIS_KEY: [
+                    {"col": "field_integer", "opr": "gt", "value": 5},
+                    {"col": "field_integer", "opr": "lt", "value": 7},
+                    {"col": "field_string", "opr": "sw", "value": "a"},
+                ]
+            }
+            rison_args = prison.dumps(arguments)
+            uri = f"api/v1/model1apisearchfilters/?{API_URI_RIS_KEY}={rison_args}"
 
-        session.delete(model1_1)
-        session.commit()
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data["count"], 1)
+            self.assertEqual(data["result"][0]["field_string"], "abc")
+
+            session.delete(model1_1)
+            session.commit()
 
     def test_get_list_custom_search_filters(self):
         """
         REST Api: Test get list custom filters
         """
         session = self.appbuilder.get_session
         model1_1 = Model1(field_string="abc", field_integer=2)
@@ -1726,43 +1800,48 @@
             ]
         }
         rison_args = prison.dumps(arguments)
         uri = f"api/v1/model1apisearchfilters/?{API_URI_RIS_KEY}={rison_args}"
 
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["count"], 1)
-        expected_result = [
-            {
-                "field_date": None,
-                "field_float": None,
-                "field_integer": 1,
-                "field_string": "abcd",
-            }
-        ]
-        self.assertEqual(data[API_RESULT_RES_KEY], expected_result)
-
-        arguments = {
-            API_FILTERS_RIS_KEY: [
-                {"col": "field_string", "opr": "custom_filter", "value": filter_value},
-                {"col": "field_integer", "opr": "eq", "value": 3},
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data["count"], 1)
+            expected_result = [
+                {
+                    "field_date": None,
+                    "field_float": None,
+                    "field_integer": 1,
+                    "field_string": "abcd",
+                }
             ]
-        }
-        rison_args = prison.dumps(arguments)
-        uri = f"api/v1/model1apisearchfilters/?{API_URI_RIS_KEY}={rison_args}"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["count"], 0)
-        session.delete(model1_1)
-        session.delete(model1_2)
-        session.commit()
+            self.assertEqual(data[API_RESULT_RES_KEY], expected_result)
+
+            arguments = {
+                API_FILTERS_RIS_KEY: [
+                    {
+                        "col": "field_string",
+                        "opr": "custom_filter",
+                        "value": filter_value,
+                    },
+                    {"col": "field_integer", "opr": "eq", "value": 3},
+                ]
+            }
+            rison_args = prison.dumps(arguments)
+            uri = f"api/v1/model1apisearchfilters/?{API_URI_RIS_KEY}={rison_args}"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data["count"], 0)
+            session.delete(model1_1)
+            session.delete(model1_2)
+            session.commit()
 
     def test_get_info_custom_search_filters(self):
         """
         REST Api: Test get info custom filters
         """
         arguments = {"keys": ["filters"]}
         rison_args = prison.dumps(arguments)
@@ -1788,25 +1867,27 @@
         argument = {
             API_SELECT_COLUMNS_RIS_KEY: ["field_integer"],
             "order_column": "field_integer",
             "order_direction": "asc",
         }
 
         uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(argument)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data[API_RESULT_RES_KEY][0], {"field_integer": 0})
-        self.assertEqual(
-            data[API_LABEL_COLUMNS_RES_KEY], {"field_integer": "Field Integer"}
-        )
-        self.assertEqual(
-            data[API_DESCRIPTION_COLUMNS_RES_KEY], {"field_integer": "Field Integer"}
-        )
-        self.assertEqual(data[API_LIST_COLUMNS_RES_KEY], ["field_integer"])
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 5):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data[API_RESULT_RES_KEY][0], {"field_integer": 0})
+            self.assertEqual(
+                data[API_LABEL_COLUMNS_RES_KEY], {"field_integer": "Field Integer"}
+            )
+            self.assertEqual(
+                data[API_DESCRIPTION_COLUMNS_RES_KEY],
+                {"field_integer": "Field Integer"},
+            )
+            self.assertEqual(data[API_LIST_COLUMNS_RES_KEY], ["field_integer"])
+            self.assertEqual(rv.status_code, 200)
 
     def test_get_list_select_meta_data(self):
         """
         REST Api: Test get list select meta data
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1814,55 +1895,60 @@
         selectable_keys = [
             API_DESCRIPTION_COLUMNS_RIS_KEY,
             API_LABEL_COLUMNS_RIS_KEY,
             API_ORDER_COLUMNS_RIS_KEY,
             API_LIST_COLUMNS_RIS_KEY,
             API_LIST_TITLE_RIS_KEY,
         ]
-        for selectable_key in selectable_keys:
-            argument = {API_SELECT_KEYS_RIS_KEY: [selectable_key]}
-            uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(argument)}"
-            rv = self.auth_client_get(client, token, uri)
-            data = json.loads(rv.data.decode("utf-8"))
-            self.assertEqual(len(data.keys()), 1 + 3)  # always exist count, ids, result
-            # We assume that rison meta key equals result meta key
-            assert selectable_key in data
+        with model1_data(self.appbuilder.session, 1):
+            for selectable_key in selectable_keys:
+                argument = {API_SELECT_KEYS_RIS_KEY: [selectable_key]}
+                uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(argument)}"
+                rv = self.auth_client_get(client, token, uri)
+                data = json.loads(rv.data.decode("utf-8"))
+                self.assertEqual(
+                    len(data.keys()), 1 + 3
+                )  # always exist count, ids, result
+                # We assume that rison meta key equals result meta key
+                assert selectable_key in data
 
     def test_get_list_exclude_cols(self):
         """
         REST Api: Test get list with excluded columns
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         uri = "api/v1/model1apiexcludecols/"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data[API_RESULT_RES_KEY][0], {"field_string": "test0"})
+        with model1_data(self.appbuilder.session, 1):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data[API_RESULT_RES_KEY][0], {"field_string": "test0"})
 
     def test_get_list_base_filters(self):
         """
         REST Api: Test get list with base filters
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         arguments = {"order_column": "field_integer", "order_direction": "desc"}
         uri = f"api/v1/model1apifiltered/?{API_URI_RIS_KEY}={prison.dumps(arguments)}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        expected_result = [
-            {
-                "field_date": None,
-                "field_float": 3.0,
-                "field_integer": 3,
-                "field_string": "test3",
-            }
-        ]
-        self.assertEqual(data[API_RESULT_RES_KEY], expected_result)
+        with model1_data(self.appbuilder.session, 5):
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            expected_result = [
+                {
+                    "field_date": None,
+                    "field_float": 3.0,
+                    "field_integer": 3,
+                    "field_string": "test3",
+                }
+            ]
+            self.assertEqual(data[API_RESULT_RES_KEY], expected_result)
 
     def test_info_filters(self):
         """
         REST Api: Test info filters
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1958,60 +2044,68 @@
         """
         REST Api: Test info fields with related fields
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         uri = "api/v1/model2api/_info"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        expected_rel_add_field = {
-            "count": MODEL2_DATA_SIZE,
-            "description": "",
-            "label": "Group",
-            "name": "group",
-            "required": True,
-            "unique": False,
-            "type": "Related",
-            "values": [],
-        }
-        for i in range(self.model2api.page_size):
-            expected_rel_add_field["values"].append(
-                {"id": i + 1, "value": "test{}".format(i)}
-            )
-        for rel_field in data[API_ADD_COLUMNS_RES_KEY]:
-            if rel_field["name"] == "group":
-                self.assertEqual(rel_field, expected_rel_add_field)
+        with model2_data(self.appbuilder.session, MODEL2_DATA_SIZE) as models:
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            expected_rel_add_field = {
+                "count": MODEL2_DATA_SIZE,
+                "description": "",
+                "label": "Group",
+                "name": "group",
+                "required": True,
+                "unique": False,
+                "type": "Related",
+                "values": [
+                    {"id": model.group_id, "value": f"test{i}"}
+                    for i, model in enumerate(models)
+                    if i < self.model2api.page_size
+                ],
+            }
+            for rel_field in data[API_ADD_COLUMNS_RES_KEY]:
+                if rel_field["name"] == "group":
+                    self.assertEqual(rel_field, expected_rel_add_field)
 
     def test_info_fields_rel_filtered_field(self):
         """
         REST Api: Test info fields with filtered
         related fields
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         uri = "api/v1/model2apifilteredrelfields/_info"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        expected_rel_add_field = {
-            "description": "",
-            "label": "Group",
-            "name": "group",
-            "required": True,
-            "unique": False,
-            "type": "Related",
-            "count": 1,
-            "values": [{"id": 4, "value": "test3"}],
-        }
-        for rel_field in data[API_ADD_COLUMNS_RES_KEY]:
-            if rel_field["name"] == "group":
-                self.assertEqual(rel_field, expected_rel_add_field)
-        for rel_field in data[API_EDIT_COLUMNS_RES_KEY]:
-            if rel_field["name"] == "group":
-                self.assertEqual(rel_field, expected_rel_add_field)
+        with model2_data(self.appbuilder.session, 4):
+            # get the parent model
+            parent_model = (
+                self.appbuilder.session.query(Model1)
+                .filter(Model1.field_integer == 3)
+                .one_or_none()
+            )
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            expected_rel_add_field = {
+                "description": "",
+                "label": "Group",
+                "name": "group",
+                "required": True,
+                "unique": False,
+                "type": "Related",
+                "count": 1,
+                "values": [{"id": parent_model.id, "value": "test3"}],
+            }
+            for rel_field in data[API_ADD_COLUMNS_RES_KEY]:
+                if rel_field["name"] == "group":
+                    self.assertEqual(rel_field, expected_rel_add_field)
+            for rel_field in data[API_EDIT_COLUMNS_RES_KEY]:
+                if rel_field["name"] == "group":
+                    self.assertEqual(rel_field, expected_rel_add_field)
 
     def test_info_permissions(self):
         """
         REST Api: Test info permissions
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -2060,128 +2154,129 @@
     def test_delete_item(self):
         """
         REST Api: Test delete item
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test2")
-            .one_or_none()
-        )
-        pk = model.id
-        uri = f"api/v1/model2api/{pk}"
-        rv = self.auth_client_delete(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model2).get(pk)
-        self.assertEqual(model, None)
-
-        # Revert data changes
-        insert_model2(self.appbuilder.get_session, i=pk - 1)
+        with model2_data(self.appbuilder.session, 3):
+            model = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test2")
+                .one_or_none()
+            )
+            model_id = model.id
+            uri = f"api/v1/model2api/{model_id}"
+            rv = self.auth_client_delete(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model2).get(model_id)
+            self.assertEqual(model, None)
 
     def test_delete_item_integrity(self):
         """
         REST Api: Test delete item integrity
         """
+        # SQLLite does not support constraints by default
+        engine_type = self.appbuilder.get_session.bind.dialect.name
+        if engine_type == "sqlite":
+            return
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model.id
-        uri = f"api/v1/model1api/{pk}"
-        rv = self.auth_client_delete(client, token, uri)
-        self.assertEqual(rv.status_code, 422)
-        model = self.db.session.query(Model1).get(pk)
-        self.assertIsNotNone(model)
+        with model2_data(self.appbuilder.session, 1):
+            model = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model.id
+            uri = f"api/v1/model1api/{pk}"
+
+            rv = self.auth_client_delete(client, token, uri)
+            self.assertEqual(rv.status_code, 422)
+            model = self.db.session.query(Model1).get(pk)
+            self.assertIsNotNone(model)
 
     def test_delete_item_not_found(self):
         """
         REST Api: Test delete item not found
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        max_id = self.appbuilder.get_session.query(func.max(Model1.id)).scalar()
-        pk = max_id + 1
-        uri = f"api/v1/model1api/{pk}"
-        rv = self.auth_client_delete(client, token, uri)
-        self.assertEqual(rv.status_code, 404)
+        with model1_data(self.appbuilder.session, 2):
+            max_id = self.appbuilder.get_session.query(func.max(Model1.id)).scalar()
+            pk = max_id + 1
+            uri = f"api/v1/model1api/{pk}"
+            rv = self.auth_client_delete(client, token, uri)
+            self.assertEqual(rv.status_code, 404)
 
     def test_delete_item_base_filters(self):
         """
         REST Api: Test delete item with base filters
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_integer=2)
-            .one_or_none()
-        )
+        with model1_data(self.appbuilder.session, 4):
+            model = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_integer=2)
+                .one_or_none()
+            )
 
-        # Try to delete a filtered item
-        pk = model.id
-        uri = "api/v1/model1apifiltered/{}".format(pk)
-        rv = self.auth_client_delete(client, token, uri)
-        self.assertEqual(rv.status_code, 404)
+            # Try to delete a filtered item
+            pk = model.id
+            uri = "api/v1/model1apifiltered/{}".format(pk)
+            rv = self.auth_client_delete(client, token, uri)
+            self.assertEqual(rv.status_code, 404)
 
     def test_update_item(self):
         """
         REST Api: Test update item
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test2")
-            .one_or_none()
-        )
-        pk = model1.id
-        item = dict(field_string="test_Put", field_integer=0, field_float=0.0)
-        uri = f"api/v1/model1api/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model1).get(pk)
-        self.assertEqual(model.field_string, "test_Put")
-        self.assertEqual(model.field_integer, 0)
-        self.assertEqual(model.field_float, 0.0)
-
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=pk - 1)
+        with model1_data(self.appbuilder.session, 3):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test2")
+                .one_or_none()
+            )
+            model_id = model1.id
+            item = dict(field_string="test_Put", field_integer=0, field_float=0.0)
+            uri = f"api/v1/model1api/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model1).get(model_id)
+            self.assertEqual(model.field_string, "test_Put")
+            self.assertEqual(model.field_integer, 0)
+            self.assertEqual(model.field_float, 0.0)
 
     def test_update_custom_validation(self):
         """
         REST Api: Test update item custom validation
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test2")
-            .one_or_none()
-        )
-        pk = model1.id
-        item = dict(field_string="test_Put", field_integer=0, field_float=0.0)
-        uri = f"api/v1/model1customvalidationapi/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 422)
-        pk = 3
-        item = dict(field_string="Atest_Put", field_integer=0, field_float=0.0)
-        uri = f"api/v1/model1customvalidationapi/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 200)
-
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=pk - 1)
+        with model1_data(self.appbuilder.session, 3):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test2")
+                .one_or_none()
+            )
+            model_id = model1.id
+            item = dict(field_string="test_Put", field_integer=0, field_float=0.0)
+            uri = f"api/v1/model1customvalidationapi/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 422)
+            item = dict(field_string="Atest_Put", field_integer=0, field_float=0.0)
+            uri = f"api/v1/model1customvalidationapi/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 200)
 
     def test_update_item_custom_schema(self):
         """
         REST Api: Test update item custom schema
         """
         from .sqla.models import Model1CustomSchema
 
@@ -2195,267 +2290,252 @@
         # Test custom validation item must start with a capital A
         item = dict(
             field_string=f"test{MODEL1_DATA_SIZE + 1}",
             field_integer=MODEL1_DATA_SIZE + 1,
             field_float=float(MODEL1_DATA_SIZE + 1),
             field_date=None,
         )
-        uri = "api/v1/model1apicustomschema/1"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 422)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data, {"message": {"field_string": ["Name must start with an A"]}}
-        )
-
-        # Test normal update with custom schema
-        item = dict(
-            field_string=f"Atest{MODEL1_DATA_SIZE + 1}",
-            field_integer=MODEL1_DATA_SIZE + 1,
-            field_float=float(MODEL1_DATA_SIZE + 1),
-            field_date=None,
-        )
-        uri = "api/v1/model1apicustomschema/1"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 3) as models:
+            model_id = models[0].id
+            uri = f"api/v1/model1apicustomschema/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 422)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data, {"message": {"field_string": ["Name must start with an A"]}}
+            )
 
-        model = (
-            self.db.session.query(Model1)
-            .filter_by(field_string="Atest{}".format(MODEL1_DATA_SIZE + 1))
-            .first()
-        )
-        self.assertEqual(model.field_string, f"Atest{MODEL1_DATA_SIZE + 1}")
-        self.assertEqual(model.field_integer, MODEL1_DATA_SIZE + 1)
-        self.assertEqual(model.field_float, float(MODEL1_DATA_SIZE + 1))
+            # Test normal update with custom schema
+            item = dict(
+                field_string=f"Atest{MODEL1_DATA_SIZE + 1}",
+                field_integer=MODEL1_DATA_SIZE + 1,
+                field_float=float(MODEL1_DATA_SIZE + 1),
+                field_date=None,
+            )
+            uri = f"api/v1/model1apicustomschema/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 200)
 
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=0)
+            model = (
+                self.db.session.query(Model1)
+                .filter_by(field_string="Atest{}".format(MODEL1_DATA_SIZE + 1))
+                .first()
+            )
+            self.assertEqual(model.field_string, f"Atest{MODEL1_DATA_SIZE + 1}")
+            self.assertEqual(model.field_integer, MODEL1_DATA_SIZE + 1)
+            self.assertEqual(model.field_float, float(MODEL1_DATA_SIZE + 1))
 
     def test_update_item_base_filters(self):
         """
         REST Api: Test update item with base filters
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_integer=3)
-            .one_or_none()
-        )
-        pk = model1.id
-        item = dict(field_string="test_Put", field_integer=3, field_float=3.0)
-        uri = f"api/v1/model1apifiltered/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model1).get(pk)
-        self.assertEqual(model.field_string, "test_Put")
-        self.assertEqual(model.field_integer, 3)
-        self.assertEqual(model.field_float, 3.0)
-
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=pk - 1)
-
-        # We can't update an item that is base filtered
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_integer=1)
-            .one_or_none()
-        )
-        pk = model1.id
-        uri = f"api/v1/model1apifiltered/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 404)
+        with model1_data(self.appbuilder.session, 4):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_integer=3)
+                .one_or_none()
+            )
+            model_id = model1.id
+            item = dict(field_string="test_Put", field_integer=3, field_float=3.0)
+            uri = f"api/v1/model1apifiltered/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model1).get(model_id)
+            self.assertEqual(model.field_string, "test_Put")
+            self.assertEqual(model.field_integer, 3)
+            self.assertEqual(model.field_float, 3.0)
+
+            # We can't update an item that is base filtered
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_integer=1)
+                .one_or_none()
+            )
+            model_id = model1.id
+            uri = f"api/v1/model1apifiltered/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 404)
 
     def test_update_item_not_found(self):
         """
         REST Api: Test update item not found
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        max_id = self.appbuilder.get_session.query(func.max(Model1.id)).scalar()
-        pk = max_id + 1
-        item = dict(field_string="test_Put", field_integer=0, field_float=0.0)
-        uri = f"api/v1/model1api/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 404)
+        with model1_data(self.appbuilder.session, 2):
+            max_id = self.appbuilder.get_session.query(func.max(Model1.id)).scalar()
+            model_id = max_id + 1
+            item = dict(field_string="test_Put", field_integer=0, field_float=0.0)
+            uri = f"api/v1/model1api/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 404)
 
     def test_update_val_size(self):
         """
         REST Api: Test update validate size
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model1.id
-        field_string = "a" * 51
-        item = dict(field_string=field_string, field_integer=11, field_float=11.0)
-        uri = f"api/v1/model1api/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 422)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data["message"]["field_string"][0], "Longer than maximum length 50."
-        )
+
+        with model1_data(self.appbuilder.session, 2):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model1.id
+            field_string = "a" * 51
+            item = dict(field_string=field_string, field_integer=11, field_float=11.0)
+            uri = f"api/v1/model1api/{pk}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 422)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data["message"]["field_string"][0], "Longer than maximum length 50."
+            )
 
     def test_update_mm_field(self):
         """
         REST Api: Test update m-m field
         """
         session = self.appbuilder.get_session
-        pk = 1
-        # Fetching children so that we can revert the changes
-        original_model = session.query(ModelMMParent).filter_by(id=pk).one_or_none()
-        original_children = [child for child in original_model.children]
 
-        child = ModelMMChild()
-        child.field_string = "update_m,m"
-        session.add(child)
-        session.commit()
-
-        child_id = (
-            session.query(ModelMMChild)
-            .filter_by(field_string="update_m,m")
-            .one_or_none()
-            .id
-        )
-        item = dict(children=[child_id])
-        client = self.app.test_client()
-        token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        uri = "api/v1/modelmmapi/{}".format(pk)
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY], {"children": [child_id], "field_string": "0"}
-        )
+        with model_mm_parent_data(session, 1):
+            model_id = session.query(ModelMMParent).first().id
 
-        # Revert data changes
-        original_model = session.query(ModelMMParent).filter_by(id=pk).one_or_none()
-        original_model.children = original_children
-        session.merge(original_model)
-        session.commit()
-        child = session.query(ModelMMChild).filter_by(id=child_id).one_or_none()
-        session.delete(child)
-        session.commit()
+            child = ModelMMChild()
+            child.field_string = "update_m,m"
+            session.add(child)
+            session.commit()
+
+            child_id = (
+                session.query(ModelMMChild)
+                .filter_by(field_string="update_m,m")
+                .one_or_none()
+                .id
+            )
+            item = dict(children=[child_id])
+            client = self.app.test_client()
+            token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+            uri = "api/v1/modelmmapi/{}".format(model_id)
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY], {"children": [child_id], "field_string": "0"}
+            )
 
     def test_update_item_val_type(self):
         """
         REST Api: Test update validate type
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model1.id
-        item = dict(
-            field_string=f"test{MODEL1_DATA_SIZE + 1}",
-            field_integer=f"test{MODEL1_DATA_SIZE + 1}",
-            field_float=11.0,
-        )
-        uri = f"api/v1/model1api/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 422)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["message"]["field_integer"][0], "Not a valid integer.")
+        with model1_data(self.appbuilder.session, 2):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model1.id
+            item = dict(
+                field_string=f"test{MODEL1_DATA_SIZE + 1}",
+                field_integer=f"test{MODEL1_DATA_SIZE + 1}",
+                field_float=11.0,
+            )
+            uri = f"api/v1/model1api/{pk}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 422)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data["message"]["field_integer"][0], "Not a valid integer."
+            )
 
-        item = dict(field_string=11, field_integer=11, field_float=11.0)
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 422)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(data["message"]["field_string"][0], "Not a valid string.")
+            item = dict(field_string=11, field_integer=11, field_float=11.0)
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 422)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data["message"]["field_string"][0], "Not a valid string.")
 
     def test_update_item_excluded_cols(self):
         """
         REST Api: Test update item with excluded cols
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model1.id
-        item = dict(field_string="test_Put")
-        uri = f"api/v1/model1apiexcludecols/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model1).get(pk)
-        self.assertEqual(model.field_integer, 0)
-        self.assertEqual(model.field_float, 0.0)
-        self.assertEqual(model.field_date, None)
-        self.assertEqual(model.field_string, "test_Put")
-
-        item = dict(field_string="test_Put", field_integer=1000)
-        uri = f"api/v1/model1apiexcludecols/{pk}"
-        rv = self.auth_client_put(client, token, uri, item)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 422)
-        expected_response = {"message": {"field_integer": ["Unknown field."]}}
-        self.assertEqual(expected_response, data)
-
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=pk - 1)
+        with model1_data(self.appbuilder.session, 2):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            model_id = model1.id
+            item = dict(field_string="test_Put")
+            uri = f"api/v1/model1apiexcludecols/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model1).get(model_id)
+            self.assertEqual(model.field_integer, 0)
+            self.assertEqual(model.field_float, 0.0)
+            self.assertEqual(model.field_date, None)
+            self.assertEqual(model.field_string, "test_Put")
+
+            item = dict(field_string="test_Put", field_integer=1000)
+            uri = f"api/v1/model1apiexcludecols/{model_id}"
+            rv = self.auth_client_put(client, token, uri, item)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 422)
+            expected_response = {"message": {"field_integer": ["Unknown field."]}}
+            self.assertEqual(expected_response, data)
 
     def test_create_item(self):
         """
         REST Api: Test create item
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         item = dict(
-            field_string="test{}".format(MODEL1_DATA_SIZE + 1),
-            field_integer=MODEL1_DATA_SIZE + 1,
-            field_float=float(MODEL1_DATA_SIZE + 1),
-            field_date=None,
+            field_string="test4", field_integer=4, field_float=4.0, field_date=None
         )
         uri = "api/v1/model1api/"
-        rv = self.auth_client_post(client, token, uri, item)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 201)
-        self.assertEqual(data[API_RESULT_RES_KEY], item)
-        model = (
-            self.db.session.query(Model1)
-            .filter_by(field_string="test{}".format(MODEL1_DATA_SIZE + 1))
-            .first()
-        )
-        self.assertEqual(model.field_string, f"test{MODEL1_DATA_SIZE + 1}")
-        self.assertEqual(model.field_integer, MODEL1_DATA_SIZE + 1)
-        self.assertEqual(model.field_float, float(MODEL1_DATA_SIZE + 1))
+        with model1_data(self.appbuilder.session, 3):
+            rv = self.auth_client_post(client, token, uri, item)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 201)
+            self.assertEqual(data[API_RESULT_RES_KEY], item)
+            model = (
+                self.db.session.query(Model1).filter_by(field_string="test4").first()
+            )
+            self.assertEqual(model.field_string, "test4")
+            self.assertEqual(model.field_integer, 4)
+            self.assertEqual(model.field_float, 4.0)
 
         # Revert data changes
-        self.appbuilder.get_session.delete(model)
-        self.appbuilder.get_session.commit()
+        self.appbuilder.session.delete(model)
+        self.appbuilder.session.commit()
 
     def test_create_item_bad_request(self):
         """
         REST Api: Test create item with bad request
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         item = dict(
-            field_string="test{}".format(MODEL1_DATA_SIZE + 1),
+            field_string=f"test{MODEL1_DATA_SIZE + 1}",
             field_integer=MODEL1_DATA_SIZE + 1,
             field_float=float(MODEL1_DATA_SIZE + 1),
             field_date=None,
         )
         uri = "api/v1/model1api/"
-        rv = client.post(
-            uri, data=item, headers={"Authorization": "Bearer {}".format(token)}
-        )
+        rv = client.post(uri, data=item, headers={"Authorization": f"Bearer {token}"})
         data = json.loads(rv.data.decode("utf-8"))
         self.assertEqual(rv.status_code, 400)
         self.assertEqual(data, {"message": "Request is not JSON"})
 
     def test_create_item_custom_validation(self):
         """
         REST Api: Test create item custom validation
@@ -2478,15 +2558,14 @@
         item = dict(
             field_string=f"A{MODEL1_DATA_SIZE + 1}",
             field_integer=MODEL1_DATA_SIZE + 1,
             field_float=float(MODEL1_DATA_SIZE + 1),
             field_date=None,
         )
         rv = self.auth_client_post(client, token, uri, item)
-        data = json.loads(rv.data.decode("utf-8"))
         self.assertEqual(rv.status_code, 201)
 
         # Revert test data
         self.appbuilder.get_session.query(Model1).filter_by(
             field_string=f"A{MODEL1_DATA_SIZE + 1}"
         ).delete()
         self.appbuilder.get_session.commit()
@@ -2631,38 +2710,43 @@
 
     def test_list_items_with_enum(self):
         """
         REST Api: Test list items with enums
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        uri = "api/v1/modelwithenumsapi/"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["result"], [{"enum1": "e1", "enum2": 2, "enum3": "e3"}])
-        self.assertEqual(data["count"], 1)
+
+        with model_with_enums_data(self.appbuilder.session, 1):
+            uri = "api/v1/modelwithenumsapi/"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(
+                data["result"], [{"enum1": "e1", "enum2": 2, "enum3": "e3"}]
+            )
+            self.assertEqual(data["count"], 1)
 
     def test_get_item_with_enums(self):
         """
         REST Api: Test get item with enums
         """
-        model1 = (
-            self.appbuilder.get_session.query(ModelWithEnums)
-            .filter(ModelWithEnums.enum1 == "e1")
-            .first()
-        )
-        pk = model1.id
-        client = self.app.test_client()
-        token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        uri = f"api/v1/modelwithenumsapi/{pk}"
-        rv = self.auth_client_get(client, token, uri)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(rv.status_code, 200)
-        self.assertEqual(data["result"], {"enum1": "e1", "enum2": 2, "enum3": "e3"})
+        with model_with_enums_data(self.appbuilder.session, 1):
+            model1 = (
+                self.appbuilder.get_session.query(ModelWithEnums)
+                .filter(ModelWithEnums.enum1 == "e1")
+                .first()
+            )
+            pk = model1.id
+            client = self.app.test_client()
+            token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+            uri = f"api/v1/modelwithenumsapi/{pk}"
+            rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(rv.status_code, 200)
+            self.assertEqual(data["result"], {"enum1": "e1", "enum2": 2, "enum3": "e3"})
 
     def test_model_with_enum_oas(self):
         """
         REST Api: Test model with enum OAS
         """
         self.maxDiff = None
         client = self.app.test_client()
@@ -2741,55 +2825,59 @@
 
     def test_create_item_mm_field(self):
         """
         REST Api: Test create with M-M field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        item = dict(field_string="new1", children=[1, 2])
-        uri = "api/v1/modelmmapi/"
-        rv = self.auth_client_post(client, token, uri, item)
-        self.assertEqual(rv.status_code, 201)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY], {"children": [1, 2], "field_string": "new1"}
-        )
-        # Test without M-M field data, default is not required
-        item = dict(field_string="new2")
-        uri = "api/v1/modelmmapi/"
-        rv = self.auth_client_post(client, token, uri, item)
-        self.assertEqual(rv.status_code, 201)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data[API_RESULT_RES_KEY], {"children": [], "field_string": "new2"}
-        )
-        # Test without M-M field data, default is required
-        item = dict(field_string="new1")
-        uri = "api/v1/modelmmrequiredapi/"
-        rv = self.auth_client_post(client, token, uri, item)
-        self.assertEqual(rv.status_code, 422)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertEqual(
-            data, {"message": {"children": ["Missing data for required field."]}}
-        )
 
-        # Rollback data changes
-        model1 = (
-            self.appbuilder.get_session.query(ModelMMParent)
-            .filter_by(field_string="new1")
-            .one_or_none()
-        )
-        model2 = (
-            self.appbuilder.get_session.query(ModelMMParent)
-            .filter_by(field_string="new2")
-            .one_or_none()
-        )
-        self.appbuilder.get_session.delete(model1)
-        self.appbuilder.get_session.delete(model2)
-        self.appbuilder.get_session.commit()
+        with model_mm_parent_data(self.appbuilder.session, 1, 4) as models:
+            children_ids = [child.id for child in models[0].children]
+            item = dict(field_string="new1", children=children_ids[0:2])
+            uri = "api/v1/modelmmapi/"
+            rv = self.auth_client_post(client, token, uri, item)
+            self.assertEqual(rv.status_code, 201)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY],
+                {"children": children_ids[0:2], "field_string": "new1"},
+            )
+            # Test without M-M field data, default is not required
+            item = dict(field_string="new2")
+            uri = "api/v1/modelmmapi/"
+            rv = self.auth_client_post(client, token, uri, item)
+            self.assertEqual(rv.status_code, 201)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data[API_RESULT_RES_KEY], {"children": [], "field_string": "new2"}
+            )
+            # Test without M-M field data, default is required
+            item = dict(field_string="new1")
+            uri = "api/v1/modelmmrequiredapi/"
+            rv = self.auth_client_post(client, token, uri, item)
+            self.assertEqual(rv.status_code, 422)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(
+                data, {"message": {"children": ["Missing data for required field."]}}
+            )
+
+            # Rollback data changes
+            model1 = (
+                self.appbuilder.get_session.query(ModelMMParent)
+                .filter_by(field_string="new1")
+                .one_or_none()
+            )
+            model2 = (
+                self.appbuilder.get_session.query(ModelMMParent)
+                .filter_by(field_string="new2")
+                .one_or_none()
+            )
+            self.appbuilder.get_session.delete(model1)
+            self.appbuilder.get_session.delete(model2)
+            self.appbuilder.get_session.commit()
 
     def test_create_item_om_field(self):
         """
         REST Api: Test create with O-M field
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -2820,65 +2908,75 @@
 
     def test_get_list_col_function(self):
         """
         REST Api: Test get list of objects with columns as functions
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        uri = "api/v1/model1funcapi/"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        for i in range(1, self.model1api.page_size):
-            item = data[API_RESULT_RES_KEY][i - 1]
-            self.assertEqual(
-                item["full_concat"], f"test{str(i - 1)}.{i - 1}.{float(i - 1)}.{None}"
-            )
+
+        with model1_data(self.appbuilder.session):
+            uri = "api/v1/model1funcapi/"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            for i in range(1, self.model1api.page_size):
+                item = data[API_RESULT_RES_KEY][i - 1]
+                self.assertEqual(
+                    item["full_concat"],
+                    f"test{str(i - 1)}.{i - 1}.{float(i - 1)}.{None}",
+                )
 
     def test_get_list_col_property(self):
         """
         REST Api: Test get list of objects with columns as property
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         uri = "api/v1/modelwithpropertyapi/"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        for i in range(1, self.model1api.page_size):
-            item = data[API_RESULT_RES_KEY][i - 1]
-            self.assertEqual(item["custom_property"], f"{item['field_string']}_custom")
+
+        with model_with_property_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL1_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            for i in range(1, self.model1api.page_size):
+                item = data[API_RESULT_RES_KEY][i - 1]
+                self.assertEqual(
+                    item["custom_property"], f"{item['field_string']}_custom"
+                )
 
     def test_get_list_col_callable(self):
         """
         REST Api: Test get list of objects with columns as callable
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         uri = "api/v1/model2callablecolapi/"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        # Tests count property
-        self.assertEqual(data["count"], MODEL1_DATA_SIZE)
-        # Tests data result default page size
-        self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
-        results = data[API_RESULT_RES_KEY]
-        for i, item in enumerate(results):
-            self.assertEqual(
-                item["field_method"], f"{item['field_string']}_field_method"
-            )
+
+        with model2_data(self.appbuilder.session, MODEL2_DATA_SIZE):
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            # Tests count property
+            self.assertEqual(data["count"], MODEL2_DATA_SIZE)
+            # Tests data result default page size
+            self.assertEqual(len(data[API_RESULT_RES_KEY]), self.model1api.page_size)
+            results = data[API_RESULT_RES_KEY]
+            for i, item in enumerate(results):
+                self.assertEqual(
+                    item["field_method"], f"{item['field_string']}_field_method"
+                )
 
     def test_openapi(self):
         """
         REST Api: Test OpenAPI spec
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -2915,38 +3013,32 @@
 
         self.model2permoverride1 = Model2PermOverride1
         self.appbuilder.add_api(Model2PermOverride1)
 
         role = self.appbuilder.sm.add_role("Test")
         pvm = self.appbuilder.sm.find_permission_view_menu("can_access", "api")
         self.appbuilder.sm.add_permission_role(role, pvm)
-        user = self.appbuilder.sm.add_user(
+        self.appbuilder.sm.add_user(
             "test", "test", "user", "test@fab.org", role, "test"
         )
 
         client = self.app.test_client()
         token = self.login(client, "test", "test")
-        uri = "api/v1/model2permoverride1/"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        uri = "api/v1/model2permoverride1/_info"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        uri = "api/v1/model2permoverride1/1"
-        rv = self.auth_client_delete(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
 
-        # Revert test data
-        insert_model2(self.appbuilder.get_session, i=0)
-        self.appbuilder.get_session.delete(
-            self.appbuilder.sm.find_user(username="test")
-        )
-        self.appbuilder.get_session.delete(self.appbuilder.sm.find_role("Test"))
-        self.appbuilder.get_session.delete(user)
-        self.appbuilder.get_session.commit()
+        with model2_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            uri = "api/v1/model2permoverride1/"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            uri = "api/v1/model2permoverride1/_info"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            uri = f"api/v1/model2permoverride1/{model_id}"
+            rv = self.auth_client_delete(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
 
     def test_method_permission_override(self):
         """
         REST Api: Test method permission name override
         """
 
         class Model2PermOverride2(ModelRestApi):
@@ -2967,26 +3059,30 @@
         pvm = self.appbuilder.sm.find_permission_view_menu(
             "can_read", "Model2PermOverride2"
         )
         self.appbuilder.sm.add_permission_role(role, pvm)
         user = self.appbuilder.sm.add_user(
             "test", "test", "user", "test@fab.org", role, "test"
         )
+        if not user:
+            user = self.appbuilder.sm.find_user("test")
 
         client = self.app.test_client()
         token = self.login(client, "test", "test")
-        uri = "api/v1/model2permoverride2/"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        uri = "api/v1/model2permoverride2/_info"
-        rv = self.auth_client_get(client, token, uri)
-        self.assertEqual(rv.status_code, 200)
-        uri = "api/v1/model2permoverride2/1"
-        rv = self.auth_client_delete(client, token, uri)
-        self.assertEqual(rv.status_code, 403)
+
+        with model2_data(self.appbuilder.session, 1):
+            uri = "api/v1/model2permoverride2/"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            uri = "api/v1/model2permoverride2/_info"
+            rv = self.auth_client_get(client, token, uri)
+            self.assertEqual(rv.status_code, 200)
+            uri = "api/v1/model2permoverride2/1"
+            rv = self.auth_client_delete(client, token, uri)
+            self.assertEqual(rv.status_code, 403)
 
         # Revert test data
         self.db.session.delete(user)
         self.db.session.commit()
         self.appbuilder.get_session.delete(self.appbuilder.sm.find_role("Test"))
         self.appbuilder.get_session.commit()
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_custom_indexview.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_custom_indexview.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 class FlaskTestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__, template_folder=".")
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config[
             "FAB_INDEX_VIEW"
-        ] = "flask_appbuilder.tests.test_custom_indexview.CustomIndexView"
+        ] = "tests.test_custom_indexview.CustomIndexView"
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def tearDown(self):
         self.appbuilder = None
         self.app = None
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_fab_cli.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_fab_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,21 +118,23 @@
 
         for input, expected_output in scenarii.items():
             self.assertEqual(cast_int_like_to_int(input), expected_output)
 
 
 class SQLAlchemyImportExportTestCase(FABTestCase):
     def setUp(self):
-        with open("flask_appbuilder/tests/data/roles.json", "r") as fd:
+        basedir = os.path.abspath(os.path.dirname(__file__))
+
+        with open(os.path.join(basedir, "data/roles.json"), "r") as fd:
             self.expected_roles = json.loads(fd.read())
 
     def test_export_roles(self):
         with tempfile.TemporaryDirectory() as tmp_dir:
             app = Flask("src_app")
-            app.config.from_object("flask_appbuilder.tests.config_security")
+            app.config.from_object("tests.config_security")
             app.config[
                 "SQLALCHEMY_DATABASE_URI"
             ] = f"sqlite:///{os.path.join(tmp_dir, 'src.db')}"
             db = SQLA(app)
             app_builder = AppBuilder(app, db.session)  # noqa: F841
             cli_runner = app.test_cli_runner()
 
@@ -164,15 +166,15 @@
                     resulting_role_permission_view_menus,
                     expected_role_permission_view_menus,
                 )
 
     def test_export_roles_filename(self):
         with tempfile.TemporaryDirectory() as tmp_dir:
             app = Flask("src_app")
-            app.config.from_object("flask_appbuilder.tests.config_security")
+            app.config.from_object("tests.config_security")
 
             app.config[
                 "SQLALCHEMY_DATABASE_URI"
             ] = f"sqlite:///{os.path.join(tmp_dir, 'src.db')}"
             db = SQLA(app)
             app_builder = AppBuilder(app, db.session)  # noqa: F841
 
@@ -188,15 +190,15 @@
             )
 
     @patch("json.dumps")
     def test_export_roles_indent(self, mock_json_dumps):
         """Test that json.dumps is called with the correct argument passed from CLI."""
         with tempfile.TemporaryDirectory() as tmp_dir:
             app = Flask("src_app")
-            app.config.from_object("flask_appbuilder.tests.config_security")
+            app.config.from_object("tests.config_security")
             app.config[
                 "SQLALCHEMY_DATABASE_URI"
             ] = f"sqlite:///{os.path.join(tmp_dir, 'src.db')}"
             db = SQLA(app)
             app_builder = AppBuilder(app, db.session)  # noqa: F841
             cli_runner = app.test_cli_runner()
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_menu.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
         from flask_appbuilder.views import ModelView
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_API_MAX_PAGE_SIZE"] = MAX_PAGE_SIZE
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
         class Model1View(ModelView):
             datamodel = SQLAInterface(Model1)
@@ -57,15 +57,15 @@
 
         # as logged out user
         rv = client.get(uri)
         self.assertEqual(rv.status_code, 401)
 
     def test_menu_api(self):
         """
-            REST Api: Test menu data
+        REST Api: Test menu data
         """
         uri = "/api/v1/menu/"
         client = self.app.test_client()
 
         # Enable Model1Dynamic
         self._conditional_value = True
 
@@ -75,15 +75,15 @@
         data = rv.data.decode("utf-8")
         self.assertIn("Security", data)
         self.assertIn("Model1", data)
         self.assertIn("Model1Dynamic", data)
 
     def test_menu_api_limited(self):
         """
-            REST Api: Test limited menu data
+        REST Api: Test limited menu data
         """
         limited_user = "user1"
         limited_password = "user1"
         limited_role = "Limited"
 
         role = self.appbuilder.sm.add_role(limited_role)
         pvm = self.appbuilder.sm.find_permission_view_menu("menu_access", "Model1")
@@ -130,15 +130,15 @@
             self.appbuilder.sm.find_user(username=limited_user)
         )
         self.appbuilder.get_session.delete(self.appbuilder.sm.find_role(limited_role))
         self.appbuilder.get_session.commit()
 
     def test_menu_api_public(self):
         """
-            REST Api: Test public menu data
+        REST Api: Test public menu data
         """
         role = self.appbuilder.sm.find_role("Public")
         pvm = self.appbuilder.sm.find_permission_view_menu("menu_access", "Model1")
         self.appbuilder.sm.add_permission_role(role, pvm)
         pvm = self.appbuilder.sm.find_permission_view_menu(
             "menu_access", "Model1Dynamic"
         )
@@ -171,15 +171,15 @@
         # Revert test data
         role = self.appbuilder.sm.find_role("Public")
         role.permissions = []
         self.appbuilder.get_session.commit()
 
     def test_redirect_after_logout(self):
         """
-            REST Api: Test redirect after logout
+        REST Api: Test redirect after logout
         """
         limited_user = "user1"
         limited_password = "user1"
 
         client = self.app.test_client()
 
         self.login(client, limited_user, limited_password)
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_mongoengine.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_mongoengine.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,32 +218,32 @@
 
     def clean_data(self):
         Model1.drop_collection()
         Model2.drop_collection()
 
     def test_fab_views(self):
         """
-            Test views creation and registration
+        Test views creation and registration
         """
         eq_(len(self.appbuilder.baseviews), 26)  # current minimal views are 26
 
     def test_index(self):
         """
-            Test initial access and index message
+        Test initial access and index message
         """
         client = self.app.test_client()
 
         # Check for Welcome Message
         rv = client.get("/")
         data = rv.data.decode("utf-8")
         ok_(DEFAULT_INDEX_STRING in data)
 
     def test_sec_login(self):
         """
-            Test Security Login, Logout, invalid login, invalid access
+        Test Security Login, Logout, invalid login, invalid access
         """
         client = self.app.test_client()
 
         # Try to List and Redirect to Login
         rv = client.get("/model1view/list/")
         eq_(rv.status_code, 302)
         rv = client.get("/model2view/list/")
@@ -266,15 +266,15 @@
         # Invalid Login
         rv = self.browser_login(client, DEFAULT_ADMIN_USER, "password")
         data = rv.data.decode("utf-8")
         ok_(INVALID_LOGIN_STRING in data)
 
     def test_sec_reset_password(self):
         """
-            Test Security reset password
+        Test Security reset password
         """
         from flask_appbuilder.security.mongoengine.models import User
 
         client = self.app.test_client()
 
         # Try Reset My password
         user = User.objects.filter(**{"username": "admin"})[0]
@@ -324,15 +324,15 @@
             ),
             follow_redirects=True,
         )
         self.assertEqual(rv.status_code, 200)
 
     def test_model_crud(self):
         """
-            Test Model add, delete, edit
+        Test Model add, delete, edit
         """
         client = self.app.test_client()
         rv = self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
 
         rv = client.post(
             "/model1view/add",
             data=dict(
@@ -367,15 +367,15 @@
         eq_(rv.status_code, 200)
         model = Model1.objects
         eq_(len(model), 0)
         self.clean_data()
 
     def test_excluded_cols(self):
         """
-            Test add_exclude_columns, edit_exclude_columns, show_exclude_columns
+        Test add_exclude_columns, edit_exclude_columns, show_exclude_columns
         """
         client = self.app.test_client()
         rv = self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
         rv = client.get("/model22view/add")
         eq_(rv.status_code, 200)
         data = rv.data.decode("utf-8")
         ok_("field_string" in data)
@@ -401,15 +401,15 @@
         ok_("Field Float" in data)
         ok_("Field Date" in data)
         ok_("Excluded String" not in data)
         self.clean_data()
 
     def test_query_rel_fields(self):
         """
-            Test add and edit form related fields filter
+        Test add and edit form related fields filter
         """
         client = self.app.test_client()
         rv = self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
         self.insert_data2()
 
         # Base filter string starts with
         rv = client.get("/model2view/add")
@@ -423,15 +423,15 @@
         data = rv.data.decode("utf-8")
         ok_("G2" in data)
         ok_("G1" not in data)
         self.clean_data()
 
     def test_model_list_order(self):
         """
-            Test Model order on lists
+        Test Model order on lists
         """
         self.insert_data()
 
         client = self.app.test_client()
         self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
 
         rv = client.post(
@@ -452,15 +452,15 @@
         rv.data.decode("utf-8")
         # TODO
         # VALIDATE LIST IS ORDERED
         self.clean_data()
 
     def test_model_add_validation(self):
         """
-            Test Model add validations
+        Test Model add validations
         """
         client = self.app.test_client()
         self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
 
         rv = client.post(
             "/model1view/add",
             data=dict(field_string="test1", field_integer="1"),
@@ -491,15 +491,15 @@
 
         model = Model1.objects()
         eq_(len(model), 1)
         self.clean_data()
 
     def test_model_edit_validation(self):
         """
-            Test Model edit validations
+        Test Model edit validations
         """
         client = self.app.test_client()
         self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
 
         client.post(
             "/model1view/add",
             data=dict(field_string="test1", field_integer="1"),
@@ -528,15 +528,15 @@
         eq_(rv.status_code, 200)
         data = rv.data.decode("utf-8")
         ok_(NOTNULL_VALIDATION_STRING in data)
         self.clean_data()
 
     def test_model_base_filter(self):
         """
-            Test Model base filtered views
+        Test Model base filtered views
         """
         client = self.app.test_client()
         self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
         self.insert_data()
         models = Model1.objects()
         eq_(len(models), 23)
 
@@ -551,46 +551,48 @@
         data = rv.data.decode("utf-8")
         ok_("atest" in data)
         ok_("btest" not in data)
         self.clean_data()
 
     def test_model_list_method_field(self):
         """
-            Tests a model's field has a method
+        Tests a model's field has a method
         """
         client = self.app.test_client()
         self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
         self.insert_data2()
         rv = client.get("/model2view/list/")
         eq_(rv.status_code, 200)
         data = rv.data.decode("utf-8")
         ok_("field_method_value" in data)
         self.clean_data()
 
     def test_compactCRUDMixin(self):
         """
-            Test CompactCRUD Mixin view
+        Test CompactCRUD Mixin view
         """
         client = self.app.test_client()
         self.browser_login(client, DEFAULT_ADMIN_USER, DEFAULT_ADMIN_PASSWORD)
         self.insert_data2()
         rv = client.get("/model1compactview/list/")
         eq_(rv.status_code, 200)
         self.clean_data()
 
 
 class MongoImportExportTestCase(unittest.TestCase):
     def setUp(self):
-        with open("flask_appbuilder/tests/data/roles.json", "r") as fd:
+        basedir = os.path.abspath(os.path.dirname(__file__))
+
+        with open(os.path.join(basedir, "data/roles.json"), "r") as fd:
             self.expected_roles = json.loads(fd.read())
 
     def test_export_roles(self):
         with tempfile.TemporaryDirectory() as tmp_dir:
             app = Flask(__name__)
-            app.config.from_object("flask_appbuilder.tests.config_security")
+            app.config.from_object("tests.config_security")
             app.config["MONGODB_SETTINGS"] = {
                 "db": "app",
                 "host": "localhost",
                 "port": 27017,
             }
             db_mongo = MongoEngine(app)  # noqa: F841
             app_builder = AppBuilder(  # noqa: F841
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_mvc.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_mvc.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,33 +23,29 @@
     FilterEqual,
     FilterEqualFunction,
     FilterStartsWith,
 )
 from flask_appbuilder.models.sqla.interface import SQLAInterface
 from flask_appbuilder.views import CompactCRUDMixin, MasterDetailView, ModelView
 from flask_wtf import CSRFProtect
-
-from .base import BaseMVCTestCase, FABTestCase
-from .const import (
+from tests.base import BaseMVCTestCase, FABTestCase
+from tests.const import (
     MODEL1_DATA_SIZE,
     PASSWORD_ADMIN,
     PASSWORD_READONLY,
     USERNAME_ADMIN,
     USERNAME_READONLY,
 )
-from .sqla.models import (
-    insert_model1,
-    insert_model2,
-    insert_model3,
-    Model1,
-    Model2,
-    Model3,
-    ModelWithEnums,
-    TmpEnum,
+from tests.fixtures.data_models import (
+    model1_data,
+    model2_data,
+    model3_data,
+    model_with_enums_data,
 )
+from tests.sqla.models import Model1, Model2, Model3, ModelWithEnums, TmpEnum
 
 logging.basicConfig(format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
 logging.getLogger().setLevel(logging.DEBUG)
 
 
 """
     Constant english display string from framework
@@ -64,15 +60,15 @@
 
 class MVCBabelTestCase(FABTestCase):
     def test_babel_empty_languages(self):
         """
         MVC: Test babel empty languages
         """
         app = Flask(__name__)
-        app.config.from_object("flask_appbuilder.tests.config_api")
+        app.config.from_object("tests.config_api")
         app.config["LANGUAGES"] = {}
         db = SQLA(app)
         AppBuilder(app, db.session)
 
         client = app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         rv = client.get("/users/list/")
@@ -82,15 +78,15 @@
         self.assertNotIn('class="f16', data)
 
     def test_babel_languages(self):
         """
         MVC: Test babel languages
         """
         app = Flask(__name__)
-        app.config.from_object("flask_appbuilder.tests.config_api")
+        app.config.from_object("tests.config_api")
         app.config["LANGUAGES"] = {
             "en": {"flag": "gb", "name": "English"},
             "pt": {"flag": "pt", "name": "Portuguese"},
         }
         db = SQLA(app)
         AppBuilder(app, db.session)
 
@@ -136,25 +132,26 @@
     def test_list_filter_end_with(self):
         """
         MVC: Test ends with filter
         """
         with self.app.test_client() as client:
             self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
             # test filter ends with
-            rv = client.get(
-                "/model1view/list?_flt_1_field_string=0", follow_redirects=True
-            )
-            data = rv.data.decode("utf-8")
-            self.assertIn("test0", data)
+            with model1_data(self.appbuilder.session, 2):
+                rv = client.get(
+                    "/model1view/list?_flt_1_field_string=0", follow_redirects=True
+                )
+                data = rv.data.decode("utf-8")
+                self.assertIn("test0", data)
 
-            rv = client.get(
-                "/model1view/list?_flt_1_field_string=1", follow_redirects=True
-            )
-            data = rv.data.decode("utf-8")
-            self.assertNotIn("test0", data)
+                rv = client.get(
+                    "/model1view/list?_flt_1_field_string=1", follow_redirects=True
+                )
+                data = rv.data.decode("utf-8")
+                self.assertNotIn("test0", data)
 
     def test_list_filter_invalid_object(self):
         """
         MVC: Test Filter with related object not found
         """
         with self.app.test_client() as c:
             self.browser_login(c, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -264,15 +261,15 @@
             self.assertNotIn("admin@fab.org", data)
 
 
 class MVCCSRFTestCase(BaseMVCTestCase):
     def setUp(self):
 
         self.app = Flask(__name__)
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["WTF_CSRF_ENABLED"] = True
 
         self.csrf = CSRFProtect(self.app)
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
         class Model2View(ModelView):
@@ -283,46 +280,47 @@
     def test_a_csrf_delete_not_allowed(self):
         """
         MVC: Test GET delete with CSRF is not allowed
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model.id
-        rv = client.get(f"/model2view/delete/{pk}")
+        with model2_data(self.appbuilder.session, 1):
+            model = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model.id
+            rv = client.get(f"/model2view/delete/{pk}")
 
-        self.assertEqual(rv.status_code, 302)
-        model = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        self.assertIsNotNone(model)
+            self.assertEqual(rv.status_code, 302)
+            model = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            self.assertIsNotNone(model)
 
     def test_a_csrf_delete_protected(self):
         """
         MVC: Test POST delete with CSRF
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-
-        model = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model.id
-        rv = client.post(f"/model2view/delete/{pk}")
-        # Missing CSRF token
-        self.assertEqual(rv.status_code, 400)
+        with model2_data(self.appbuilder.session, 1):
+            model = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model.id
+            rv = client.post(f"/model2view/delete/{pk}")
+            # Missing CSRF token
+            self.assertEqual(rv.status_code, 400)
 
 
 class MVCSwitchRouteMethodsTestCase(BaseMVCTestCase):
     """
     Specific to test ModelView's:
         - include_route_methods
         - exclude_route_methods
@@ -775,24 +773,25 @@
 
     def test_related_view_edit_with_excluded_search(self):
         """
         Test related edit view with excluded search field
         """
         with self.app.test_client() as client:
             self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+            with model2_data(self.appbuilder.session, 3) as models:
+                model_id = models[0].id
+                # Test excluded search field will not impact related view
+                rv = client.get(f"/model2view/edit/{model_id}?_flt_0_group=1")
+                data = rv.data.decode("utf-8")
+                self.assertNotIn('<label for="group"', data)
 
-            # Test excluded search field will not impact related view
-            rv = client.get("/model2view/edit/1?_flt_0_group=1")
-            data = rv.data.decode("utf-8")
-            self.assertNotIn('<label for="group"', data)
-
-            # Test direct edit view includes related field
-            rv = client.get("/model2view/edit/2")
-            data = rv.data.decode("utf-8")
-            self.assertIn('<label for="group"', data)
+                # Test direct edit view includes related field
+                rv = client.get(f"/model2view/edit/{model_id}")
+                data = rv.data.decode("utf-8")
+                self.assertIn('<label for="group"', data)
 
     def test_related_view_add_with_excluded_search(self):
         """
         Test related add view with excluded search field
         """
         with self.app.test_client() as client:
             self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -828,15 +827,15 @@
         self.assertEqual(rv.status_code, 200)
 
     def test_model_crud_add(self):
         """
         Test ModelView CRUD Add
         """
         client = self.app.test_client()
-        rv = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+        self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         field_string = f"test{MODEL1_DATA_SIZE+1}"
         rv = client.post(
             "/model1view/add",
             data=dict(
                 field_string=field_string,
                 field_integer=f"{MODEL1_DATA_SIZE}",
@@ -860,84 +859,82 @@
         self.appbuilder.get_session.commit()
 
     def test_model_crud_edit(self):
         """
         Test ModelView CRUD Edit
         """
         client = self.app.test_client()
-        rv = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-
-        model = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model.id
-        rv = client.post(
-            f"/model1view/edit/{pk}",
-            data=dict(field_string="test_edit", field_integer="200"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
+        self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model = self.db.session.query(Model1).filter_by(id=pk).one_or_none()
-        self.assertEqual(model.field_string, "test_edit")
-        self.assertEqual(model.field_integer, 200)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            rv = client.post(
+                f"/model1view/edit/{model_id}",
+                data=dict(field_string="test_edit", field_integer="200"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
 
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=pk - 1)
+            model = self.db.session.query(Model1).filter_by(id=model_id).one_or_none()
+            self.assertEqual(model.field_string, "test_edit")
+            self.assertEqual(model.field_integer, 200)
 
     def test_model_crud_delete(self):
         """
         Test Model CRUD delete
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        model = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model.id
-        rv = client.get(f"/model2view/delete/{pk}", follow_redirects=True)
-
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model2).get(pk)
-        self.assertEqual(model, None)
+        with model2_data(self.appbuilder.session, 2):
+            model = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model.id
+            rv = client.get(f"/model2view/delete/{pk}", follow_redirects=True)
 
-        # Revert data changes
-        insert_model2(self.appbuilder.get_session, i=0)
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model2).get(pk)
+            self.assertEqual(model, None)
 
     def test_model_delete_integrity(self):
         """
         Test Model CRUD delete integrity validation
         """
+        # SQLLite does not support constraints by default
+        engine_type = self.appbuilder.get_session.bind.dialect.name
+        if engine_type == "sqlite":
+            return
+
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test1")
-            .one_or_none()
-        )
-        pk = model1.id
-        rv = client.get(f"/model1view/delete/{pk}", follow_redirects=True)
 
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model1).filter_by(id=pk).one_or_none()
-        self.assertNotEqual(model, None)
+        with model2_data(self.appbuilder.session, 2):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test1")
+                .one_or_none()
+            )
+            pk = model1.id
+            rv = client.get(f"/model1view/delete/{pk}", follow_redirects=True)
+
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model1).filter_by(id=pk).one_or_none()
+            self.assertNotEqual(model, None)
 
     def test_model_crud_composite_pk(self):
         """
         MVC CRUD generic-alter datasource where model has composite
         primary keys
         """
         try:
             from urllib import quote
-        except Exception:
+        except ImportError:
             from urllib.parse import quote
 
         client = self.app.test_client()
         rv = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         rv = client.post(
             "/model3view/add",
@@ -1009,74 +1006,81 @@
     def test_model_crud_add_with_enum(self):
         """
         Test Model add for Model with Enum Columns
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        data = {"enum1": "e3", "enum2": "e3", "enum3": "e3"}
-        rv = client.post("/modelwithenumsview/add", data=data, follow_redirects=True)
-        self.assertEqual(rv.status_code, 200)
+        with model_with_enums_data(self.appbuilder.session, 1):
+            data = {"enum1": "e3", "enum2": "e3", "enum3": "e3"}
+            rv = client.post(
+                "/modelwithenumsview/add", data=data, follow_redirects=True
+            )
+            self.assertEqual(rv.status_code, 200)
 
-        model = (
-            self.appbuilder.get_session.query(ModelWithEnums)
-            .filter_by(enum1="e3")
-            .one_or_none()
-        )
-        self.assertIsNotNone(model)
-        self.assertEqual(model.enum2, TmpEnum.e3)
+            model = (
+                self.appbuilder.get_session.query(ModelWithEnums)
+                .filter_by(enum1="e3")
+                .one_or_none()
+            )
+            self.assertIsNotNone(model)
+            self.assertEqual(model.enum2, TmpEnum.e3)
 
-        # Revert data changes
-        model = (
-            self.appbuilder.get_session.query(ModelWithEnums)
-            .filter_by(enum1="e3")
-            .one_or_none()
-        )
-        self.appbuilder.get_session.delete(model)
-        self.appbuilder.get_session.commit()
+            # Revert data changes
+            model = (
+                self.appbuilder.get_session.query(ModelWithEnums)
+                .filter_by(enum1="e3")
+                .one_or_none()
+            )
+            self.appbuilder.get_session.delete(model)
+            self.appbuilder.get_session.commit()
 
     def test_model_crud_edit_with_enum(self):
         """
         Test Model edit for Model with Enum Columns
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        data = {"enum1": "e3", "enum2": "e3", "enum3": "e3"}
-        pk = 1
-        rv = client.post(
-            f"/modelwithenumsview/edit/{pk}", data=data, follow_redirects=True
-        )
-        self.assertEqual(rv.status_code, 200)
+        with model_with_enums_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            data = {"enum1": "e3", "enum2": "e3", "enum3": "e3"}
+            rv = client.post(
+                f"/modelwithenumsview/edit/{model_id}", data=data, follow_redirects=True
+            )
+            self.assertEqual(rv.status_code, 200)
 
-        model = (
-            self.appbuilder.get_session.query(ModelWithEnums)
-            .filter_by(enum1="e3")
-            .one_or_none()
-        )
-        self.assertIsNotNone(model)
-        self.assertEqual(model.enum2, TmpEnum.e3)
-        model.enum2 = TmpEnum.e2
-        model.enum1 = "e1"
-        self.appbuilder.get_session.commit()
+            model = (
+                self.appbuilder.get_session.query(ModelWithEnums)
+                .filter_by(enum1="e3")
+                .one_or_none()
+            )
+            self.assertIsNotNone(model)
+            self.assertEqual(model.enum2, TmpEnum.e3)
+            model.enum2 = TmpEnum.e2
+            model.enum1 = "e1"
+            self.appbuilder.get_session.commit()
 
     def test_formatted_cols(self):
         """
         Test ModelView's formatters_columns
         """
         client = self.app.test_client()
-        rv = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = client.get("/model1formattedview/list/")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("FORMATTED_STRING", data)
-        rv = client.get("/model1formattedview/show/1")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("FORMATTED_STRING", data)
+        self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            rv = client.get("/model1formattedview/list/")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("FORMATTED_STRING", data)
+            rv = client.get(f"/model1formattedview/show/{model_id}")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("FORMATTED_STRING", data)
 
     def test_modelview_add_redirects(self):
         """
         Test ModelView redirects after add
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1099,44 +1103,42 @@
 
     def test_modelview_edit_redirects(self):
         """
         Test ModelView redirects after edit
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model_id = (
-            self.db.session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-            .id
-        )
-        rv = client.post(
-            f"/model1viewwithredirects/edit/{model_id}",
-            data=dict(field_string="test_redirect", field_integer="200"),
-        )
-        self.assertEqual(rv.status_code, 302)
-        self.assertEqual("/", rv.headers["Location"])
-
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=model_id - 1)
+        with model1_data(self.appbuilder.session, 3):
+            model_id = (
+                self.db.session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+                .id
+            )
+            rv = client.post(
+                f"/model1viewwithredirects/edit/{model_id}",
+                data=dict(field_string="test_redirect", field_integer="200"),
+            )
+            self.assertEqual(rv.status_code, 302)
+            self.assertEqual("/", rv.headers["Location"])
 
     def test_modelview_delete_redirects(self):
         """
         Test ModelView redirects after delete
         """
         client = self.app.test_client()
-        rv = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model_id = (
-            self.db.session.query(Model1).filter_by(field_string="test0").first().id
-        )
-        rv = client.get(f"/model1viewwithredirects/delete/{model_id}")
-        self.assertEqual(rv.status_code, 302)
-        self.assertEqual("/", rv.headers["Location"])
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=model_id - 1)
+        self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        with model1_data(self.appbuilder.session, 1):
+            model_id = (
+                self.db.session.query(Model1).filter_by(field_string="test0").first().id
+            )
+            rv = client.get(f"/model1viewwithredirects/delete/{model_id}")
+            self.assertEqual(rv.status_code, 302)
+            self.assertEqual("/", rv.headers["Location"])
 
     def test_add_excluded_cols(self):
         """
         Test add_exclude_columns
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1151,93 +1153,96 @@
 
     def test_edit_excluded_cols(self):
         """
         Test edit_exclude_columns
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-
-        model = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        rv = client.get(f"/model22view/edit/{model.id}")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("field_string", data)
-        self.assertIn("field_integer", data)
-        self.assertIn("field_float", data)
-        self.assertIn("field_date", data)
-        self.assertNotIn("excluded_string", data)
+        with model2_data(self.appbuilder.session, 2):
+            model = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            rv = client.get(f"/model22view/edit/{model.id}")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("field_string", data)
+            self.assertIn("field_integer", data)
+            self.assertIn("field_float", data)
+            self.assertIn("field_date", data)
+            self.assertNotIn("excluded_string", data)
 
     def test_show_excluded_cols(self):
         """
         Test show_exclude_columns
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        model = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        rv = client.get(f"/model22view/show/{model.id}")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("Field String", data)
-        self.assertIn("Field Integer", data)
-        self.assertIn("Field Float", data)
-        self.assertIn("Field Date", data)
-        self.assertNotIn("Excluded String", data)
+        with model2_data(self.appbuilder.session, 3):
+            model = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            rv = client.get(f"/model22view/show/{model.id}")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("Field String", data)
+            self.assertIn("Field Integer", data)
+            self.assertIn("Field Float", data)
+            self.assertIn("Field Date", data)
+            self.assertNotIn("Excluded String", data)
 
     def test_query_rel_fields(self):
         """
         Test add and edit form related fields filter
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # Base filter string starts with
-        rv = client.get("/model2view/add")
-        data = rv.data.decode("utf-8")
-        self.assertIn("test0", data)
-        self.assertNotIn("test1", data)
+        with model2_data(self.appbuilder.session, 2):
+            # Base filter string starts with
+            rv = client.get("/model2view/add")
+            data = rv.data.decode("utf-8")
+            self.assertIn("test0", data)
+            self.assertNotIn("test1", data)
 
-        model2 = (
-            self.appbuilder.get_session.query(Model2)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        # Base filter string starts with
-        rv = client.get(f"/model2view/edit/{model2.id}")
-        data = rv.data.decode("utf-8")
-        self.assertIn("test1", data)
+            model2 = (
+                self.appbuilder.get_session.query(Model2)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            # Base filter string starts with
+            rv = client.get(f"/model2view/edit/{model2.id}")
+            data = rv.data.decode("utf-8")
+            self.assertIn("test1", data)
 
     def test_model_list_order(self):
         """
         Test Model order on lists
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = client.get(
-            "/model1view/list?_oc_Model1View=field_string&_od_Model1View=asc",
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("test0", data)
-        rv = client.get(
-            "/model1view/list?_oc_Model1View=field_string&_od_Model1View=desc",
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn(f"test{MODEL1_DATA_SIZE-1}", data)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            rv = client.get(
+                "/model1view/list?_oc_Model1View=field_string&_od_Model1View=asc",
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("test0", data)
+            rv = client.get(
+                "/model1view/list?_oc_Model1View=field_string&_od_Model1View=desc",
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn(f"test{MODEL1_DATA_SIZE-1}", data)
 
     def test_model_list_order_related(self):
         """
         Test Model order related field on lists
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1251,125 +1256,134 @@
     def test_model_add_unique_validation(self):
         """
         Test Model add unique field validation
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # Test unique constraint
-        rv = client.post(
-            "/model1view/add",
-            data=dict(field_string="test1", field_integer="2"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn(UNIQUE_VALIDATION_STRING, data)
+        with model1_data(self.appbuilder.session, 2):
+            # Test unique constraint
+            rv = client.post(
+                "/model1view/add",
+                data=dict(field_string="test1", field_integer="2"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn(UNIQUE_VALIDATION_STRING, data)
 
-        model = self.db.session.query(Model1).all()
-        self.assertEqual(len(model), MODEL1_DATA_SIZE)
+            model = self.db.session.query(Model1).all()
+            self.assertEqual(len(model), 2)
 
     def test_model_add_required_validation(self):
         """
         Test Model add required fields validation
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        # Test field required
-        rv = client.post(
-            "/model1view/add",
-            data=dict(field_string="", field_integer="1"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn(NOTNULL_VALIDATION_STRING, data)
+        with model1_data(self.appbuilder.session, 2):
+            # Test field required
+            rv = client.post(
+                "/model1view/add",
+                data=dict(field_string="", field_integer="1"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn(NOTNULL_VALIDATION_STRING, data)
 
-        model = self.db.session.query(Model1).all()
-        self.assertEqual(len(model), MODEL1_DATA_SIZE)
+            model = self.db.session.query(Model1).all()
+            self.assertEqual(len(model), 2)
 
     def test_model_edit_unique_validation(self):
         """
         Test Model edit unique validation
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = client.post(
-            "/model1view/edit/1",
-            data=dict(field_string="test2", field_integer="2"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn(UNIQUE_VALIDATION_STRING, data)
+        with model1_data(self.appbuilder.session, 3) as models:
+            model_id = models[0].id
+            rv = client.post(
+                f"/model1view/edit/{model_id}",
+                data=dict(field_string="test2", field_integer="2"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn(UNIQUE_VALIDATION_STRING, data)
 
     def test_model_edit_required_validation(self):
         """
         Test Model edit required validation
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = client.post(
-            "/model1view/edit/1",
-            data=dict(field_string="", field_integer="2"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn(NOTNULL_VALIDATION_STRING, data)
+        with model1_data(self.appbuilder.session, 3) as models:
+            model_id = models[0].id
+            rv = client.post(
+                f"/model1view/edit/{model_id}",
+                data=dict(field_string="", field_integer="2"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn(NOTNULL_VALIDATION_STRING, data)
 
     def test_model_base_filter(self):
         """
         Test Model base filtered views
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        models = self.db.session.query(Model1).all()
-        self.assertEqual(len(models), MODEL1_DATA_SIZE)
+        with model1_data(self.appbuilder.session, MODEL1_DATA_SIZE):
+            models = self.db.session.query(Model1).all()
+            self.assertEqual(len(models), MODEL1_DATA_SIZE)
 
-        # Base filter string starts with
-        rv = client.get("/model1filtered1view/list/")
-        data = rv.data.decode("utf-8")
-        self.assertIn("test2", data)
-        self.assertNotIn("test0", data)
+            # Base filter string starts with
+            rv = client.get("/model1filtered1view/list/")
+            data = rv.data.decode("utf-8")
+            self.assertIn("test2", data)
+            self.assertNotIn("test0", data)
 
-        # Base filter integer equals
-        rv = client.get("/model1filtered2view/list/")
-        data = rv.data.decode("utf-8")
-        self.assertIn("test0", data)
-        self.assertNotIn("test1", data)
+            # Base filter integer equals
+            rv = client.get("/model1filtered2view/list/")
+            data = rv.data.decode("utf-8")
+            self.assertIn("test0", data)
+            self.assertNotIn("test1", data)
 
     def test_filterequalfunction_with_relation(self):
         """
         Test FilterEqualFunction
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         # Base filter string starts with
-        rv = client.get("/model2filterequalfunctionview/list/")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("test1", data)
-        self.assertNotIn("test0", data)
-        self.assertNotIn("test2", data)
+        with model2_data(self.appbuilder.session, 3):
+            rv = client.get("/model2filterequalfunctionview/list/")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("test1", data)
+            self.assertNotIn("test0", data)
+            self.assertNotIn("test2", data)
 
     def test_model_list_method_field(self):
         """
         Tests a model's field has a method
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = client.get("/model2view/list/")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("_field_method", data)
+        with model2_data(self.appbuilder.session, 1):
+            rv = client.get("/model2view/list/")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn("_field_method", data)
 
     def test_compactCRUDMixin(self):
         """
         Test CompactCRUD Mixin view with composite keys
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
@@ -1379,61 +1393,62 @@
         # test with composite pk
         try:
             from urllib import quote
         except Exception:
             from urllib.parse import quote
 
         pk = '[3, {"_type": "datetime", "value": "2017-03-03T00:00:00"}]'
-        rv = client.post(
-            "/model3compactview/edit/" + quote(pk),
-            data=dict(field_string="bar"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model3).first()
-        self.assertEqual(model.field_string, "bar")
-
-        rv = client.get("/model3compactview/delete/" + quote(pk), follow_redirects=True)
-        self.assertEqual(rv.status_code, 200)
-        model = self.db.session.query(Model3).first()
-        self.assertEqual(model, None)
+        with model3_data(self.appbuilder.session):
+            rv = client.post(
+                "/model3compactview/edit/" + quote(pk),
+                data=dict(field_string="bar"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model3).first()
+            self.assertEqual(model.field_string, "bar")
 
-        # Revert data changes
-        insert_model3(self.appbuilder.get_session)
+            rv = client.get(
+                "/model3compactview/delete/" + quote(pk), follow_redirects=True
+            )
+            self.assertEqual(rv.status_code, 200)
+            model = self.db.session.query(Model3).first()
+            self.assertEqual(model, None)
 
     def test_edit_add_form_action_prefix_for_compactCRUDMixin(self):
         """
         Test form_action in add, form_action in edit (CompactCRUDMixin)
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         # Make sure we have something to edit.
         prefix = "/some-prefix"
         base_url = "http://localhost" + prefix
         session_form_action_key = "Model1CompactView__session_form_action"
 
-        with client as c:
-            expected_form_action = prefix + "/model1compactview/add/?"
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            with client as c:
+                expected_form_action = prefix + "/model1compactview/add/?"
 
-            c.get("/model1compactview/add/", base_url=base_url)
-            self.assertEqual(session[session_form_action_key], expected_form_action)
+                c.get("/model1compactview/add/", base_url=base_url)
+                self.assertEqual(session[session_form_action_key], expected_form_action)
 
-            expected_form_action = prefix + "/model1compactview/edit/1?"
-            c.get("/model1compactview/edit/1", base_url=base_url)
+                expected_form_action = f"{prefix}/model1compactview/edit/{model_id}?"
+                c.get(f"/model1compactview/edit/{model_id}", base_url=base_url)
 
-            self.assertEqual(session[session_form_action_key], expected_form_action)
+                self.assertEqual(session[session_form_action_key], expected_form_action)
 
     def test_charts_view(self):
         """
         Test Various Chart views
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        # self.insert_data2()
         rv = client.get("/model2chartview/chart/")
         self.assertEqual(rv.status_code, 200)
         rv = client.get("/model2groupbychartview/chart/")
         self.assertEqual(rv.status_code, 200)
         rv = client.get("/model2directbychartview/chart/")
         self.assertEqual(rv.status_code, 200)
         # TODO: fix this
@@ -1442,37 +1457,39 @@
 
     def test_master_detail_view(self):
         """
         Test Master detail view
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        # self.insert_data2()
-        rv = client.get("/model1masterview/list/")
-        self.assertEqual(rv.status_code, 200)
-        rv = client.get("/model1masterview/list/1")
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            rv = client.get("/model1masterview/list/")
+            self.assertEqual(rv.status_code, 200)
+            rv = client.get(f"/model1masterview/list/{model_id}")
+            self.assertEqual(rv.status_code, 200)
 
-        rv = client.get("/model1masterchartview/list/")
-        self.assertEqual(rv.status_code, 200)
-        rv = client.get("/model1masterchartview/list/1")
-        self.assertEqual(rv.status_code, 200)
+            rv = client.get("/model1masterchartview/list/")
+            self.assertEqual(rv.status_code, 200)
+            rv = client.get(f"/model1masterchartview/list/{model_id}")
+            self.assertEqual(rv.status_code, 200)
 
     def test_api_read(self):
         """
         Testing the api/read endpoint
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = client.get("/model1formattedview/api/read")
-        self.assertEqual(rv.status_code, 200)
-        data = json.loads(rv.data.decode("utf-8"))
-        self.assertIn("result", data)
-        self.assertIn("pks", data)
-        assert len(data.get("result")) > 10
+        with model1_data(self.appbuilder.get_session):
+            rv = client.get("/model1formattedview/api/read")
+            self.assertEqual(rv.status_code, 200)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertIn("result", data)
+            self.assertIn("pks", data)
+            assert len(data.get("result")) > 10
 
     def test_api_unauthenticated(self):
         """
         Testing unauthenticated access to MVC API
         """
         client = self.app.test_client()
         self.browser_logout(client)
@@ -1495,50 +1512,52 @@
 
     def test_api_create(self):
         """
         Testing the api/create endpoint
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        rv = client.post(
-            "/model1view/api/create",
-            data=dict(field_string="zzz"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        model1 = (
-            self.db.session.query(Model1).filter_by(field_string="zzz").one_or_none()
-        )
-        self.assertIsNotNone(model1)
+        with model1_data(self.appbuilder.session, 1):
+            rv = client.post(
+                "/model1view/api/create",
+                data=dict(field_string="zzz"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            model1 = (
+                self.db.session.query(Model1)
+                .filter_by(field_string="zzz")
+                .one_or_none()
+            )
+            self.assertIsNotNone(model1)
 
         # Revert data changes
         self.appbuilder.get_session.delete(model1)
         self.appbuilder.get_session.commit()
 
     def test_api_update(self):
         """
         Validate that the api update endpoint updates [only] the fields in
         POST data
         """
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
-        item = self.db.session.query(Model1).filter_by(id=1).one()
-        field_integer_before = item.field_integer
-        rv = client.put(
-            "/model1view/api/update/1",
-            data=dict(field_string="zzz"),
-            follow_redirects=True,
-        )
-        self.assertEqual(rv.status_code, 200)
-        item = self.db.session.query(Model1).filter_by(id=1).one()
-        self.assertEqual(item.field_string, "zzz")
-        self.assertEqual(item.field_integer, field_integer_before)
-
-        # Revert data changes
-        insert_model1(self.appbuilder.get_session, i=0)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
+            item = self.db.session.query(Model1).get(model_id)
+            field_integer_before = item.field_integer
+            rv = client.put(
+                f"/model1view/api/update/{model_id}",
+                data=dict(field_string="zzz"),
+                follow_redirects=True,
+            )
+            self.assertEqual(rv.status_code, 200)
+            item = self.db.session.query(Model1).get(model_id)
+            self.assertEqual(item.field_string, "zzz")
+            self.assertEqual(item.field_integer, field_integer_before)
 
     def test_class_method_permission_override(self):
         """
         MVC: Test class method permission name override
         """
         from flask_appbuilder import ModelView
         from flask_appbuilder.models.sqla.interface import SQLAInterface
@@ -1594,14 +1613,15 @@
         model = (
             self.db.session.query(Model1).filter_by(field_string="test1").one_or_none()
         )
         self.assertEqual(model.field_string, "test1")
         self.assertEqual(model.field_integer, 1)
 
         # Cleanup
+        self.db.session.delete(model)
         self.db.session.delete(user)
         self.db.session.commit()
 
     def test_method_permission_override(self):
         """
         MVC: Test method permission name override
         """
@@ -1647,74 +1667,76 @@
 
         client = self.app.test_client()
         self.browser_login(client, "test", "test")
 
         rv = client.post(
             "/model1permoverride/add",
             data=dict(
-                field_string=f"test{MODEL1_DATA_SIZE+1}",
+                field_string="tmp_test",
                 field_integer="1",
                 field_float="0.12",
                 field_date="2014-01-01",
             ),
             follow_redirects=True,
         )
         self.assertEqual(rv.status_code, 200)
         model1 = (
             self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string=f"test{MODEL1_DATA_SIZE+1}")
+            .filter_by(field_string="tmp_test")
             .one_or_none()
         )
         self.assertIsNotNone(model1)
 
         # Revert data changes
         self.appbuilder.get_session.delete(model1)
         self.appbuilder.get_session.commit()
 
-        # Verify write links are on the UI
-        rv = client.get("/model1permoverride/list/")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertIn("/model1permoverride/delete/1", data)
-        self.assertIn("/model1permoverride/add", data)
-        self.assertIn("/model1permoverride/edit/1", data)
-        self.assertIn("/model1permoverride/show/1", data)
-
-        # Delete write permission from Test Role
-        role = self.appbuilder.sm.find_role("Test")
-        pvm_write = self.appbuilder.sm.find_permission_view_menu(
-            "can_write", "Model1PermOverride"
-        )
-        self.appbuilder.sm.del_permission_role(role, pvm_write)
-
-        # Unauthorized delete
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test1")
-            .one_or_none()
-        )
-        pk = model1.id
-        rv = client.get(f"/model1permoverride/delete/{pk}")
-        self.assertEqual(rv.status_code, 302)
-        model = self.db.session.query(Model1).filter_by(id=pk).one_or_none()
-        self.assertEqual(model.field_string, "test1")
+        with model1_data(self.appbuilder.session, 2) as models:
+            model_id = models[0].id
+            # Verify write links are on the UI
+            rv = client.get("/model1permoverride/list/")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertIn(f"/model1permoverride/delete/{model_id}", data)
+            self.assertIn("/model1permoverride/add", data)
+            self.assertIn(f"/model1permoverride/edit/{model_id}", data)
+            self.assertIn(f"/model1permoverride/show/{model_id}", data)
+
+            # Delete write permission from Test Role
+            role = self.appbuilder.sm.find_role("Test")
+            pvm_write = self.appbuilder.sm.find_permission_view_menu(
+                "can_write", "Model1PermOverride"
+            )
+            self.appbuilder.sm.del_permission_role(role, pvm_write)
 
-        # Verify write links are gone from UI
-        rv = client.get("/model1permoverride/list/")
-        self.assertEqual(rv.status_code, 200)
-        data = rv.data.decode("utf-8")
-        self.assertNotIn("/model1permoverride/delete/1", data)
-        self.assertNotIn("/model1permoverride/add/", data)
-        self.assertNotIn("/model1permoverride/edit/1", data)
-        self.assertIn("/model1permoverride/show/1", data)
+            # Unauthorized delete
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test1")
+                .one_or_none()
+            )
+            pk = model1.id
+            rv = client.get(f"/model1permoverride/delete/{pk}")
+            self.assertEqual(rv.status_code, 302)
+            model = self.db.session.query(Model1).filter_by(id=pk).one_or_none()
+            self.assertEqual(model.field_string, "test1")
 
-        # Revert data changes
-        self.db.session.delete(self.appbuilder.sm.find_role("Test"))
-        self.db.session.delete(user)
-        self.db.session.commit()
+            # Verify write links are gone from UI
+            rv = client.get("/model1permoverride/list/")
+            self.assertEqual(rv.status_code, 200)
+            data = rv.data.decode("utf-8")
+            self.assertNotIn(f"/model1permoverride/delete/{model_id}", data)
+            self.assertNotIn("/model1permoverride/add/", data)
+            self.assertNotIn(f"/model1permoverride/edit/{model_id}", data)
+            self.assertIn(f"/model1permoverride/show/{model_id}", data)
+
+            # Revert data changes
+            self.db.session.delete(self.appbuilder.sm.find_role("Test"))
+            self.db.session.delete(user)
+            self.db.session.commit()
 
     def test_action_permission_override(self):
         """
         MVC: Test action permission name override
         """
         from flask_appbuilder import action, ModelView
         from flask_appbuilder.models.sqla.interface import SQLAInterface
@@ -1760,32 +1782,33 @@
         )
         self.appbuilder.sm.add_permission_role(role, pvm_read)
         self.appbuilder.sm.add_permission_role(role, pvm_write)
 
         client = self.app.test_client()
         self.browser_login(client, "test", "test")
 
-        model1 = (
-            self.appbuilder.get_session.query(Model1)
-            .filter_by(field_string="test0")
-            .one_or_none()
-        )
-        pk = model1.id
-        rv = client.get(f"/model1permoverride/action/action1/{pk}")
-        self.assertEqual(rv.status_code, 200)
+        with model1_data(self.appbuilder.session, 1):
+            model1 = (
+                self.appbuilder.get_session.query(Model1)
+                .filter_by(field_string="test0")
+                .one_or_none()
+            )
+            pk = model1.id
+            rv = client.get(f"/model1permoverride/action/action1/{pk}")
+            self.assertEqual(rv.status_code, 200)
 
-        # Delete write permission from Test Role
-        role = self.appbuilder.sm.find_role("Test")
-        pvm_write = self.appbuilder.sm.find_permission_view_menu(
-            "can_write", "Model1PermOverride"
-        )
-        self.appbuilder.sm.del_permission_role(role, pvm_write)
+            # Delete write permission from Test Role
+            role = self.appbuilder.sm.find_role("Test")
+            pvm_write = self.appbuilder.sm.find_permission_view_menu(
+                "can_write", "Model1PermOverride"
+            )
+            self.appbuilder.sm.del_permission_role(role, pvm_write)
 
-        rv = client.get("/model1permoverride/action/action1/1")
-        self.assertEqual(rv.status_code, 302)
+            rv = client.get("/model1permoverride/action/action1/1")
+            self.assertEqual(rv.status_code, 302)
 
         # cleanup
         self.db.session.delete(user)
         self.db.session.commit()
 
     def test_permission_converge_compress(self):
         """
@@ -1825,16 +1848,16 @@
         role = self.appbuilder.sm.find_role("Test")
         user = self.appbuilder.sm.add_user(
             "test", "test", "user", "test@fab.org", role, "test"
         )
         # Remove previous class, Hack to test code change
         for i, baseview in enumerate(self.appbuilder.baseviews):
             if baseview.__class__.__name__ == "Model1View":
+                self.appbuilder.baseviews.pop(i)
                 break
-        self.appbuilder.baseviews.pop(i)
 
         target_state_transitions = {
             "add": {
                 ("Model1View", "can_edit"): {("view2", "can_access")},
                 ("Model1View", "can_add"): {("view2", "can_access")},
                 ("Model1View", "can_list"): {("view2", "can_access")},
                 ("Model1View", "can_download"): {("view2", "can_access")},
@@ -1868,54 +1891,63 @@
         self._before_request_enabled = False
         self._before_request_can_list = False
         self._before_request_can_show = False
 
         client = self.app.test_client()
         self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        rv = client.get("/modelbeforerequest/enabled")
-        self.assertEqual(rv.status_code, 404)
+        with model1_data(self.appbuilder.session, 1) as models:
+            model_id = models[0].id
 
-        rv = client.get("/modelbeforerequest/list/")
-        self.assertEqual(rv.status_code, 404)
+            rv = client.get("/modelbeforerequest/enabled")
+            self.assertEqual(rv.status_code, 404)
 
-        rv = client.get("/modelbeforerequest/show/1")
-        self.assertEqual(rv.status_code, 404)
+            rv = client.get("/modelbeforerequest/list/")
+            self.assertEqual(rv.status_code, 404)
 
-        # /enable is available, but not others
-        self._before_request_enabled = True
+            rv = client.get(f"/modelbeforerequest/show/{model_id}")
+            self.assertEqual(rv.status_code, 404)
 
-        rv = client.get("/modelbeforerequest/enabled")
-        self.assertEqual(rv.status_code, 200)
+            # /enable is available, but not others
+            self._before_request_enabled = True
 
-        rv = client.get("/modelbeforerequest/list/")
-        self.assertEqual(rv.status_code, 404)
+            rv = client.get("/modelbeforerequest/enabled")
+            self.assertEqual(rv.status_code, 200)
 
-        rv = client.get("/modelbeforerequest/show/1", follow_redirects=True)
-        self.assertEqual(rv.status_code, 404)
+            rv = client.get("/modelbeforerequest/list/")
+            self.assertEqual(rv.status_code, 404)
 
-        # Now list is available, but not show
-        self._before_request_enabled = True
-        self._before_request_can_list = True
+            rv = client.get(
+                f"/modelbeforerequest/show/{model_id}", follow_redirects=True
+            )
+            self.assertEqual(rv.status_code, 404)
 
-        rv = client.get("/modelbeforerequest/enabled")
-        self.assertEqual(rv.status_code, 200)
+            # Now list is available, but not show
+            self._before_request_enabled = True
+            self._before_request_can_list = True
 
-        rv = client.get("/modelbeforerequest/list/", follow_redirects=True)
-        self.assertEqual(rv.status_code, 200)
+            rv = client.get("/modelbeforerequest/enabled")
+            self.assertEqual(rv.status_code, 200)
+
+            rv = client.get("/modelbeforerequest/list/", follow_redirects=True)
+            self.assertEqual(rv.status_code, 200)
 
-        rv = client.get("/modelbeforerequest/show/1", follow_redirects=True)
-        self.assertEqual(rv.status_code, 404)
+            rv = client.get(
+                f"/modelbeforerequest/show/{model_id}", follow_redirects=True
+            )
+            self.assertEqual(rv.status_code, 404)
 
-        # Everything is available
-        self._before_request_enabled = True
-        self._before_request_can_list = True
-        self._before_request_can_show = True
+            # Everything is available
+            self._before_request_enabled = True
+            self._before_request_can_list = True
+            self._before_request_can_show = True
 
-        rv = client.get("/modelbeforerequest/enabled")
-        self.assertEqual(rv.status_code, 200)
+            rv = client.get("/modelbeforerequest/enabled")
+            self.assertEqual(rv.status_code, 200)
 
-        rv = client.get("/modelbeforerequest/list/", follow_redirects=True)
-        self.assertEqual(rv.status_code, 200)
+            rv = client.get("/modelbeforerequest/list/", follow_redirects=True)
+            self.assertEqual(rv.status_code, 200)
 
-        rv = client.get("/modelbeforerequest/show/1", follow_redirects=True)
-        self.assertEqual(rv.status_code, 200)
+            rv = client.get(
+                f"/modelbeforerequest/show/{model_id}", follow_redirects=True
+            )
+            self.assertEqual(rv.status_code, 200)
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_mvc_oauth.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_mvc_oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from urllib.parse import quote
 
 from flask_appbuilder import SQLA
 from flask_appbuilder.security.sqla.models import User
-from flask_appbuilder.tests.base import FABTestCase
 from flask_login import current_user
 import jwt
+from tests.base import FABTestCase
 
 
 class UserInfoReponseMock:
     def json(self):
         return {
             "id": "1",
             "given_name": "first-name",
@@ -29,15 +29,15 @@
 class APICSRFTestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_wtf import CSRFProtect
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
-        self.app.config.from_object("flask_appbuilder.tests.config_oauth")
+        self.app.config.from_object("tests.config_oauth")
         self.app.config["WTF_CSRF_ENABLED"] = True
 
         self.csrf = CSRFProtect(self.app)
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def tearDown(self):
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_security_api.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_security_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 from typing import List
 
 from flask import Flask
 from flask_appbuilder import AppBuilder
 from flask_appbuilder import SQLA
 from flask_appbuilder.security.sqla.models import Permission, Role, User, ViewMenu
-from flask_appbuilder.tests.base import FABTestCase
-from flask_appbuilder.tests.const import PASSWORD_ADMIN, USERNAME_ADMIN
 import prison
+from tests.base import FABTestCase
+from tests.const import PASSWORD_ADMIN, USERNAME_ADMIN
 from werkzeug.security import generate_password_hash
 
 
 log = logging.getLogger(__name__)
 
 
 class UserAPITestCase(FABTestCase):
     def setUp(self) -> None:
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_security_api")
+        self.app.config.from_object("tests.config_security_api")
         self.db = SQLA(self.app)
 
         self.session = self.db.session
         self.appbuilder = AppBuilder(self.app, self.session)
         self.user_model = User
         self.role_model = Role
 
@@ -63,14 +63,16 @@
         rv = self.auth_client_get(client, token, uri)
         self.assertEqual(rv.status_code, 200)
 
     def test_user_list(self):
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
+        admin_role_id = self.appbuilder.sm.find_role("Admin").id
+        readonly_role_id = self.appbuilder.sm.find_role("ReadOnly").id
         query = {"order_column": "username", "order_direction": "desc"}
         uri = f"api/v1/security/users/?q={prison.dumps(query)}"
         rv = self.auth_client_get(client, token, uri)
         response = json.loads(rv.data)
 
         self.assertEqual(rv.status_code, 200)
         assert "count" in response
@@ -81,26 +83,26 @@
                 "active": True,
                 "changed_by": None,
                 "created_by": None,
                 "created_on": "2020-01-01T00:00:00",
                 "email": "admin@fab.org",
                 "first_name": "admin",
                 "last_name": "user",
-                "roles": [{"id": 2, "name": "Admin"}],
+                "roles": [{"id": admin_role_id, "name": "Admin"}],
                 "username": "testadmin",
             },
             {
                 "active": True,
                 "changed_by": None,
                 "created_by": None,
                 "created_on": "2020-01-01T00:00:00",
                 "email": "readonly@fab.org",
                 "first_name": "readonly",
                 "last_name": "readonly",
-                "roles": [{"id": 1, "name": "ReadOnly"}],
+                "roles": [{"id": readonly_role_id, "name": "ReadOnly"}],
                 "username": "readonly",
             },
         ]
         self.assert_response(response["result"], expected_results)
         self.assertEqual(
             [
                 "active",
@@ -121,14 +123,15 @@
             list(response["result"][0].keys()),
         )
 
     def test_user_list_search_username(self):
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
+        readonly_role_id = self.appbuilder.sm.find_role("ReadOnly").id
         query = {"filters": [{"col": "username", "opr": "eq", "value": "readonly"}]}
         uri = f"api/v1/security/users/?q={prison.dumps(query)}"
         rv = self.auth_client_get(client, token, uri)
         response = json.loads(rv.data)
 
         expected_results = [
             {
@@ -136,43 +139,46 @@
                 "changed_by": None,
                 "changed_on": "2020-01-01T00:00:00",
                 "created_by": None,
                 "created_on": "2020-01-01T00:00:00",
                 "email": "readonly@fab.org",
                 "first_name": "readonly",
                 "last_name": "readonly",
-                "roles": [{"id": 1, "name": "ReadOnly"}],
+                "roles": [{"id": readonly_role_id, "name": "ReadOnly"}],
                 "username": "readonly",
             }
         ]
         self.assert_response(response["result"], expected_results)
         self.assertEqual(rv.status_code, 200)
         assert "count" in response
         self.assertEqual(response["count"], 1)
 
     def test_user_list_search_roles(self):
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
-        query = {"filters": [{"col": "roles", "opr": "rel_m_m", "value": 2}]}
+        admin_role_id = self.appbuilder.sm.find_role("Admin").id
+        query = {
+            "filters": [{"col": "roles", "opr": "rel_m_m", "value": admin_role_id}]
+        }
         uri = f"api/v1/security/users/?q={prison.dumps(query)}"
         rv = self.auth_client_get(client, token, uri)
         response = json.loads(rv.data)
 
         expected_results = [
             {
                 "active": True,
                 "changed_by": None,
                 "changed_on": "2020-01-01T00:00:00",
                 "created_by": None,
                 "created_on": "2020-01-01T00:00:00",
                 "email": "admin@fab.org",
                 "first_name": "admin",
                 "last_name": "user",
-                "roles": [{"id": 2, "name": "Admin"}],
+                "roles": [{"id": admin_role_id, "name": "Admin"}],
                 "username": "testadmin",
             }
         ]
         self.assert_response(response["result"], expected_results)
         self.assertEqual(rv.status_code, 200)
         assert "count" in response
         self.assertEqual(response["count"], 1)
@@ -421,15 +427,15 @@
 class RolePermissionAPITestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_ADD_SECURITY_API"] = True
         self.db = SQLA(self.app)
         self.session = self.db.session
         self.appbuilder = AppBuilder(self.app, self.db.session)
         self.permission_model = Permission
         self.viewmenu_model = ViewMenu
         self.role_model = Role
@@ -536,16 +542,15 @@
         self.assertEqual(rv.status_code, 405)
 
         new_permission = self.appbuilder.sm.find_permission(permission_name)
         assert new_permission is not None
         self.appbuilder.sm.del_permission(permission_name)
 
     def test_list_view_api(self):
-        """REST Api: Test view apis
-        """
+        """REST Api: Test view apis"""
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         count = self.session.query(self.viewmenu_model).count()
 
         uri = "api/v1/security/resources/"
         rv = self.auth_client_get(client, token, uri)
@@ -650,16 +655,15 @@
         rv = self.auth_client_delete(client, token, uri)
         self.assertEqual(rv.status_code, 200)
 
         new_view_menu = self.appbuilder.sm.find_view_menu(view_menu_name)
         assert new_view_menu is None
 
     def test_list_permission_view_api(self):
-        """REST Api: Test permission view apis
-        """
+        """REST Api: Test permission view apis"""
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         uri = "api/v1/security/permissions-resources/"
         rv = self.auth_client_get(client, token, uri)
         self.assertEqual(rv.status_code, 200)
 
@@ -757,16 +761,15 @@
         rv = self.auth_client_delete(client, token, uri)
         self.assertEqual(rv.status_code, 200)
 
         pvm = self.appbuilder.sm.find_permission_view_menu(permission_name, view_name)
         assert pvm is None
 
     def test_list_role_api(self):
-        """REST Api: Test role apis
-        """
+        """REST Api: Test role apis"""
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         uri = "api/v1/security/roles/"
         rv = self.auth_client_get(client, token, uri)
         self.assertEqual(rv.status_code, 200)
 
@@ -1043,15 +1046,15 @@
 class UserRolePermissionDisabledTestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def tearDown(self):
         self.appbuilder.session.close()
         engine = self.appbuilder.session.get_bind(mapper=None, clause=None)
         for baseview in self.appbuilder.baseviews:
@@ -1093,15 +1096,15 @@
 
         def passwordValidator(password):
             if len(password) < 5:
                 raise PasswordComplexityValidationError
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_ADD_SECURITY_API"] = True
         self.app.config["FAB_PASSWORD_COMPLEXITY_ENABLED"] = True
         self.app.config["FAB_PASSWORD_COMPLEXITY_VALIDATOR"] = passwordValidator
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
         self.user_model = User
 
@@ -1153,15 +1156,15 @@
 
         def passwordValidator(password):
             if len(password) < 5:
                 raise PasswordComplexityValidationError
 
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
         self.app.config["FAB_ADD_SECURITY_API"] = True
         self.app.config["FAB_PASSWORD_COMPLEXITY_ENABLED"] = True
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
         self.user_model = User
 
     def tearDown(self):
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_security_permissions.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_security_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from flask_appbuilder import SQLA
-from flask_appbuilder.tests.base import FABTestCase
 from flask_login import AnonymousUserMixin
+from tests.base import FABTestCase
 
 
 class SecurityPermissionsTestCase(FABTestCase):
     def setUp(self):
         from flask import Flask
         from flask_appbuilder import AppBuilder
 
         self.app = Flask(__name__)
-        self.app.config.from_object("flask_appbuilder.tests.config_security")
+        self.app.config.from_object("tests.config_security")
         self.app.config["FAB_ADD_SECURITY_VIEWS"] = False
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
         self._db_role_1 = self.appbuilder.sm.add_role("DB_ROLE1")
         self._pvm1 = self.appbuilder.sm.add_permission_view_menu(
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_sqlalchemy.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/tests/test_urltools.py` & `Flask-AppBuilder-4.3.4rc1/tests/test_urltools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 
 from flask import Flask
 from flask_appbuilder import AppBuilder, SQLA
 from flask_appbuilder.models.sqla.interface import SQLAInterface
-from flask_appbuilder.tests.sqla.models import Model1
 from flask_appbuilder.urltools import get_filter_args
+from tests.sqla.models import Model1
 
 from .base import FABTestCase
 
 
 class FlaskTestCase(FABTestCase):
     def setUp(self):
         self.app = Flask(__name__)
         self.basedir = os.path.abspath(os.path.dirname(__file__))
-        self.app.config.from_object("flask_appbuilder.tests.config_api")
+        self.app.config.from_object("tests.config_api")
 
         self.db = SQLA(self.app)
         self.appbuilder = AppBuilder(self.app, self.db.session)
 
     def test_get_filter_args_allow_one(self):
         datamodel = SQLAInterface(Model1)
         with self.appbuilder.get_app.test_request_context(
```

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/upload.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/upload.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/urltools.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/utils/base.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/utils/limit.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/utils/limit.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/validators.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/validators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/views.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/flask_appbuilder/widgets.py` & `Flask-AppBuilder-4.3.4rc1/flask_appbuilder/widgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.4rc1/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/chart.png` & `Flask-AppBuilder-4.3.4rc1/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/chart_time1.png` & `Flask-AppBuilder-4.3.4rc1/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/chart_time2.png` & `Flask-AppBuilder-4.3.4rc1/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/charts.png` & `Flask-AppBuilder-4.3.4rc1/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/contact_list.png` & `Flask-AppBuilder-4.3.4rc1/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/contacts.png` & `Flask-AppBuilder-4.3.4rc1/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/direct_chart.png` & `Flask-AppBuilder-4.3.4rc1/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/fab.png` & `Flask-AppBuilder-4.3.4rc1/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/group_list.png` & `Flask-AppBuilder-4.3.4rc1/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/grouped_chart.png` & `Flask-AppBuilder-4.3.4rc1/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/groups.png` & `Flask-AppBuilder-4.3.4rc1/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/images_list.png` & `Flask-AppBuilder-4.3.4rc1/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/list_cascade.png` & `Flask-AppBuilder-4.3.4rc1/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.4rc1/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.4rc1/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/list_master_detail.png` & `Flask-AppBuilder-4.3.4rc1/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/login.png` & `Flask-AppBuilder-4.3.4rc1/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/login_db.png` & `Flask-AppBuilder-4.3.4rc1/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/login_oauth.png` & `Flask-AppBuilder-4.3.4rc1/images/login_oauth.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/login_oid.png` & `Flask-AppBuilder-4.3.4rc1/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/security.png` & `Flask-AppBuilder-4.3.4rc1/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/images/simpleview2.png` & `Flask-AppBuilder-4.3.4rc1/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/requirements.txt` & `Flask-AppBuilder-4.3.4rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/rtd_requirements.txt` & `Flask-AppBuilder-4.3.4rc1/rtd_requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/setup.cfg` & `Flask-AppBuilder-4.3.4rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.3rc2/setup.py` & `Flask-AppBuilder-4.3.4rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         "sqlalchemy-utils>=0.32.21, <1",
         "WTForms<4",
     ],
     extras_require={
         "jmespath": ["jmespath>=0.9.5"],
         "oauth": ["Authlib>=0.14, <2.0.0"],
         "openid": ["Flask-OpenID>=1.2.5, <2"],
+        "talisman": ["flask-talisman>=1.0.0, <2.0"],
     },
     tests_require=["nose>=1.0", "mockldap>=0.3.0", "hiro>=0.5.1"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
```

### Comparing `Flask-AppBuilder-4.3.3rc2/tox.ini` & `Flask-AppBuilder-4.3.4rc1/tox.ini`

 * *Files identical despite different names*

