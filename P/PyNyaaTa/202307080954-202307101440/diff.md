# Comparing `tmp/PyNyaaTa-202307080954.tar.gz` & `tmp/PyNyaaTa-202307101440.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNyaaTa-202307080954.tar", last modified: Sat Jul  8 09:54:36 2023, max compression
+gzip compressed data, was "PyNyaaTa-202307101440.tar", last modified: Mon Jul 10 14:40:35 2023, max compression
```

## Comparing `PyNyaaTa-202307080954.tar` & `PyNyaaTa-202307101440.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/
--rw-r--r--   0 root         (0) root         (0)      474 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3080 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.424649 PyNyaaTa-202307080954/PyNyaaTa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3080 2023-07-08 09:54:36.000000 PyNyaaTa-202307080954/PyNyaaTa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1635 2023-07-08 09:54:36.000000 PyNyaaTa-202307080954/PyNyaaTa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 09:54:36.000000 PyNyaaTa-202307080954/PyNyaaTa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-08 09:54:36.000000 PyNyaaTa-202307080954/PyNyaaTa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-08 09:54:36.000000 PyNyaaTa-202307080954/PyNyaaTa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-08 09:54:36.000000 PyNyaaTa-202307080954/PyNyaaTa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2659 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/README.md
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/get404.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.424649 PyNyaaTa-202307080954/pynyaata/
--rw-r--r--   0 root         (0) root         (0)     8740 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.424649 PyNyaaTa-202307080954/pynyaata/connectors/
--rw-r--r--   0 root         (0) root         (0)      699 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/connectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3895 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/connectors/animeultime.py
--rw-r--r--   0 root         (0) root         (0)     4059 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/connectors/core.py
--rw-r--r--   0 root         (0) root         (0)     3133 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/connectors/nyaa.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/connectors/yggtorrent.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/flarerequests.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/forms.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.420649 PyNyaaTa-202307080954/pynyaata/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.428649 PyNyaaTa-202307080954/pynyaata/static/css/
--rw-r--r--   0 root         (0) root         (0)    59028 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/bulma-prefers-dark.css.map
--rw-r--r--   0 root         (0) root         (0)   172028 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/bulma-prefers-dark.min.css
--rw-r--r--   0 root         (0) root         (0)    66189 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/bulma-tooltip.min.css
--rw-r--r--   0 root         (0) root         (0)    98250 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/bulma.css.map
--rw-r--r--   0 root         (0) root         (0)   206620 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/bulma.min.css
--rw-r--r--   0 root         (0) root         (0)    21778 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/font-awesome.css.map
--rw-r--r--   0 root         (0) root         (0)    31000 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     2415 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/css/styles.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.428649 PyNyaaTa-202307080954/pynyaata/static/favicons/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/favicons/animeultime.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/favicons/blank.png
--rw-r--r--   0 root         (0) root         (0)   137750 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/favicons/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     2001 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/favicons/nyaa.png
--rw-r--r--   0 root         (0) root         (0)     3107 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/favicons/pantsu.png
--rw-r--r--   0 root         (0) root         (0)     3046 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/favicons/yggtorrent.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/pynyaata/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   134808 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)   165742 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/pynyaata/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/pynyaata/templates/admin/
--rw-r--r--   0 root         (0) root         (0)     4378 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/admin/edit.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/pynyaata/templates/admin/folder/
--rw-r--r--   0 root         (0) root         (0)     1007 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/admin/folder/edit.html
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/admin/folder/list.html
--rw-r--r--   0 root         (0) root         (0)     3431 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/admin/list.html
--rw-r--r--   0 root         (0) root         (0)     2624 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/latest.html
--rw-r--r--   0 root         (0) root         (0)     4617 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/layout.html
--rw-r--r--   0 root         (0) root         (0)     1454 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/list.html
--rw-r--r--   0 root         (0) root         (0)     3032 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/pynyaata/utils.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/run.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 09:54:36.432649 PyNyaaTa-202307080954/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-08 09:54:16.000000 PyNyaaTa-202307080954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/
+-rw-r--r--   0 root         (0) root         (0)      474 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.363882 PyNyaaTa-202307101440/PyNyaaTa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-07-10 14:40:35.000000 PyNyaaTa-202307101440/PyNyaaTa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-10 14:40:35.000000 PyNyaaTa-202307101440/PyNyaaTa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:40:35.000000 PyNyaaTa-202307101440/PyNyaaTa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-10 14:40:35.000000 PyNyaaTa-202307101440/PyNyaaTa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-10 14:40:35.000000 PyNyaaTa-202307101440/PyNyaaTa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-10 14:40:35.000000 PyNyaaTa-202307101440/PyNyaaTa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/README.md
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/get404.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.363882 PyNyaaTa-202307101440/pynyaata/
+-rw-r--r--   0 root         (0) root         (0)     8740 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.363882 PyNyaaTa-202307101440/pynyaata/connectors/
+-rw-r--r--   0 root         (0) root         (0)      699 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/connectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/connectors/animeultime.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/connectors/core.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/connectors/nyaa.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/connectors/yggtorrent.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/flarerequests.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.359882 PyNyaaTa-202307101440/pynyaata/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.367882 PyNyaaTa-202307101440/pynyaata/static/css/
+-rw-r--r--   0 root         (0) root         (0)    59028 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/bulma-prefers-dark.css.map
+-rw-r--r--   0 root         (0) root         (0)   172028 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/bulma-prefers-dark.min.css
+-rw-r--r--   0 root         (0) root         (0)    66189 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/bulma-tooltip.min.css
+-rw-r--r--   0 root         (0) root         (0)    98250 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/bulma.css.map
+-rw-r--r--   0 root         (0) root         (0)   206620 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/bulma.min.css
+-rw-r--r--   0 root         (0) root         (0)    21778 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/font-awesome.css.map
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/css/styles.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.367882 PyNyaaTa-202307101440/pynyaata/static/favicons/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/favicons/animeultime.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/favicons/blank.png
+-rw-r--r--   0 root         (0) root         (0)   137750 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/favicons/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/favicons/nyaa.png
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/favicons/pantsu.png
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/favicons/yggtorrent.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/pynyaata/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)   134808 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)   165742 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/pynyaata/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/pynyaata/templates/admin/
+-rw-r--r--   0 root         (0) root         (0)     4378 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/admin/edit.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/pynyaata/templates/admin/folder/
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/admin/folder/edit.html
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/admin/folder/list.html
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/admin/list.html
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/latest.html
+-rw-r--r--   0 root         (0) root         (0)     4617 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/layout.html
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/list.html
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/pynyaata/utils.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/run.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 14:40:35.371882 PyNyaaTa-202307101440/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-10 14:40:19.000000 PyNyaaTa-202307101440/setup.py
```

### Comparing `PyNyaaTa-202307080954/PKG-INFO` & `PyNyaaTa-202307101440/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNyaaTa
-Version: 202307080954
+Version: 202307101440
 Summary: π 😼た, Xéfir's personal animes torrent search engine
 Home-page: https://git.crystalyx.net/Xefir/PyNyaaTa
 Author: Xéfir Destiny
 Author-email: xefir@crystalyx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `PyNyaaTa-202307080954/PyNyaaTa.egg-info/PKG-INFO` & `PyNyaaTa-202307101440/PyNyaaTa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNyaaTa
-Version: 202307080954
+Version: 202307101440
 Summary: π 😼た, Xéfir's personal animes torrent search engine
 Home-page: https://git.crystalyx.net/Xefir/PyNyaaTa
 Author: Xéfir Destiny
 Author-email: xefir@crystalyx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `PyNyaaTa-202307080954/PyNyaaTa.egg-info/SOURCES.txt` & `PyNyaaTa-202307101440/PyNyaaTa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/README.md` & `PyNyaaTa-202307101440/README.md`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/get404.py` & `PyNyaaTa-202307101440/get404.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/__init__.py` & `PyNyaaTa-202307101440/pynyaata/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/config.py` & `PyNyaaTa-202307101440/pynyaata/config.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/connectors/__init__.py` & `PyNyaaTa-202307101440/pynyaata/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/connectors/animeultime.py` & `PyNyaaTa-202307101440/pynyaata/connectors/animeultime.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/connectors/core.py` & `PyNyaaTa-202307101440/pynyaata/connectors/core.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/connectors/nyaa.py` & `PyNyaaTa-202307101440/pynyaata/connectors/nyaa.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/connectors/yggtorrent.py` & `PyNyaaTa-202307101440/pynyaata/connectors/yggtorrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..utils import check_blacklist_words, check_if_vf, link_exist_in_db, parse_date
 
 
 class YggTorrent(ConnectorCore):
     color = 'is-success'
     title = 'YggTorrent'
     favicon = 'yggtorrent.png'
-    base_url = 'https://www3.yggtorrent.do'
+    base_url = 'https://www3.yggtorrent.wtf'
     is_light = False
     category = 2179
 
     def get_full_search_url(self):
         sort_type = 'size'
         if self.return_type is ConnectorReturn.HISTORY:
             sort_type = 'publish_date'
```

### Comparing `PyNyaaTa-202307080954/pynyaata/flarerequests.py` & `PyNyaaTa-202307101440/pynyaata/flarerequests.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/forms.py` & `PyNyaaTa-202307101440/pynyaata/forms.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/models.py` & `PyNyaaTa-202307101440/pynyaata/models.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/bulma-prefers-dark.css.map` & `PyNyaaTa-202307101440/pynyaata/static/css/bulma-prefers-dark.css.map`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/bulma-prefers-dark.min.css` & `PyNyaaTa-202307101440/pynyaata/static/css/bulma-prefers-dark.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/bulma-tooltip.min.css` & `PyNyaaTa-202307101440/pynyaata/static/css/bulma-tooltip.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/bulma.css.map` & `PyNyaaTa-202307101440/pynyaata/static/css/bulma.css.map`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/bulma.min.css` & `PyNyaaTa-202307101440/pynyaata/static/css/bulma.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/font-awesome.css.map` & `PyNyaaTa-202307101440/pynyaata/static/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/font-awesome.min.css` & `PyNyaaTa-202307101440/pynyaata/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/css/styles.css` & `PyNyaaTa-202307101440/pynyaata/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/favicons/animeultime.png` & `PyNyaaTa-202307101440/pynyaata/static/favicons/animeultime.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/favicons/favicon.ico` & `PyNyaaTa-202307101440/pynyaata/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/favicons/nyaa.png` & `PyNyaaTa-202307101440/pynyaata/static/favicons/nyaa.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/favicons/pantsu.png` & `PyNyaaTa-202307101440/pynyaata/static/favicons/pantsu.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/favicons/yggtorrent.png` & `PyNyaaTa-202307101440/pynyaata/static/favicons/yggtorrent.png`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/fonts/FontAwesome.otf` & `PyNyaaTa-202307101440/pynyaata/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.eot` & `PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.svg` & `PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.ttf` & `PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.woff` & `PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/static/fonts/fontawesome-webfont.woff2` & `PyNyaaTa-202307101440/pynyaata/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/admin/edit.html` & `PyNyaaTa-202307101440/pynyaata/templates/admin/edit.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/admin/folder/edit.html` & `PyNyaaTa-202307101440/pynyaata/templates/admin/folder/edit.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/admin/folder/list.html` & `PyNyaaTa-202307101440/pynyaata/templates/admin/folder/list.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/admin/list.html` & `PyNyaaTa-202307101440/pynyaata/templates/admin/list.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/latest.html` & `PyNyaaTa-202307101440/pynyaata/templates/latest.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/layout.html` & `PyNyaaTa-202307101440/pynyaata/templates/layout.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/list.html` & `PyNyaaTa-202307101440/pynyaata/templates/list.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/templates/search.html` & `PyNyaaTa-202307101440/pynyaata/templates/search.html`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/pynyaata/utils.py` & `PyNyaaTa-202307101440/pynyaata/utils.py`

 * *Files identical despite different names*

### Comparing `PyNyaaTa-202307080954/setup.py` & `PyNyaaTa-202307101440/setup.py`

 * *Files identical despite different names*

