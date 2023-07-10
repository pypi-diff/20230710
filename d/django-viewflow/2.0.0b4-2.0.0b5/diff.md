# Comparing `tmp/django-viewflow-2.0.0b4.tar.gz` & `tmp/django-viewflow-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-viewflow-2.0.0b4.tar", last modified: Mon Jun  5 12:30:22 2023, max compression
+gzip compressed data, was "django-viewflow-2.0.0b5.tar", last modified: Mon Jul 10 10:45:02 2023, max compression
```

## Comparing `django-viewflow-2.0.0b4.tar` & `django-viewflow-2.0.0b5.tar`

### file list

```diff
@@ -1,327 +1,328 @@
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.392052 django-viewflow-2.0.0b4/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    34520 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/LICENSE
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1340 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/LICENSE_EXCEPTION
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      193 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/MANIFEST.in
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-06-05 12:30:22.392052 django-viewflow-2.0.0b4/PKG-INFO
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7212 2023-06-05 12:22:14.000000 django-viewflow-2.0.0b4/README.md
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.164051 django-viewflow-2.0.0b4/django_viewflow.egg-info/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-06-05 12:30:22.000000 django-viewflow-2.0.0b4/django_viewflow.egg-info/PKG-INFO
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11604 2023-06-05 12:30:22.000000 django-viewflow-2.0.0b4/django_viewflow.egg-info/SOURCES.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-06-05 12:30:22.000000 django-viewflow-2.0.0b4/django_viewflow.egg-info/dependency_links.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-01-10 07:03:38.000000 django-viewflow-2.0.0b4/django_viewflow.egg-info/not-zip-safe
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       33 2023-06-05 12:30:22.000000 django-viewflow-2.0.0b4/django_viewflow.egg-info/requires.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        9 2023-06-05 12:30:22.000000 django-viewflow-2.0.0b4/django_viewflow.egg-info/top_level.txt
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      228 2023-06-05 12:30:22.396052 django-viewflow-2.0.0b4/setup.cfg
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1405 2023-06-05 12:28:48.000000 django-viewflow-2.0.0b4/setup.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.172051 django-viewflow-2.0.0b4/viewflow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1200 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      482 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/apps.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1737 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/conf.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.172051 django-viewflow-2.0.0b4/viewflow/contrib/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/__init__.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.176051 django-viewflow-2.0.0b4/viewflow/contrib/admin/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1263 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/admin/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      444 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/admin/apps.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10383 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/auth.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.180051 django-viewflow-2.0.0b4/viewflow/contrib/plotly/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      138 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/plotly/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2170 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/plotly/material.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2494 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/plotly/views.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2257 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/contrib/plotly/viewset.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4611 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fields.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.184051 django-viewflow-2.0.0b4/viewflow/forms/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      753 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b4/viewflow/forms/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    27485 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b4/viewflow/forms/renderers.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.184051 django-viewflow-2.0.0b4/viewflow/fsm/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      751 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7886 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/admin.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15456 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3001 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/chart.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      725 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/typing.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1568 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/views.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5438 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/fsm/viewset.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6787 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/jsonstore.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.140051 django-viewflow-2.0.0b4/viewflow/locale/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.132051 django-viewflow-2.0.0b4/viewflow/locale/de/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.188051 django-viewflow-2.0.0b4/viewflow/locale/de/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6147 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19568 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.132051 django-viewflow-2.0.0b4/viewflow/locale/es/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.188051 django-viewflow-2.0.0b4/viewflow/locale/es/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9136 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20862 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/fr/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.188051 django-viewflow-2.0.0b4/viewflow/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9296 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21031 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/it/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.188051 django-viewflow-2.0.0b4/viewflow/locale/it/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9466 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21002 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/ja/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.188051 django-viewflow-2.0.0b4/viewflow/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10300 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21914 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/kk/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      378 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17712 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/ko/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/pt/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      380 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17714 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.136051 django-viewflow-2.0.0b4/viewflow/locale/ru/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11819 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    23228 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.140051 django-viewflow-2.0.0b4/viewflow/locale/zh_Hans/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/management/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2742 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/management/__init__.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.192051 django-viewflow-2.0.0b4/viewflow/management/commands/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/management/commands/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2082 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/management/commands/flowexport.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2471 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/middleware.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.140051 django-viewflow-2.0.0b4/viewflow/static/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.144051 django-viewflow-2.0.0b4/viewflow/static/viewflow/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.196051 django-viewflow-2.0.0b4/viewflow/static/viewflow/css/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2598 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/css/perfect-scrollbar.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19972 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/css/trix.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   460203 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/css/viewflow.min.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   220163 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/css/vis-network.min.css
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.140051 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.208051 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   182028 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   155276 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   206260 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   173620 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156236 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   135984 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   339600 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   215704 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3314 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   164912 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   128352 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.228051 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86508 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64960 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    94048 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    72088 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86184 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64740 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91968 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70360 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85692 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64320 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    92864 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70760 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86444 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    65484 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    93228 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    71284 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85876 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64632 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91728 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70280 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    84224 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    63048 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    90784 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    68328 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4173 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.240051 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077522 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   718180 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   603192 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   213035 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   184911 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.248051 django-viewflow-2.0.0b4/viewflow/static/viewflow/img/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1311 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/img/favicon.png
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2200 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/img/user.png
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.276051 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19549 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/perfect-scrollbar.min.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    77830 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17674 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/smartcrop.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   229927 2023-01-27 12:19:41.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/trix.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156812 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/turbo.es2017-umd.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   564585 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/viewflow.min.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1658508 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/viewflow.min.js.map
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   490205 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/vis-network.min.js
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  2010720 2023-06-05 12:29:27.000000 django-viewflow-2.0.0b4/viewflow/static/viewflow/js/vis-network.min.js.map
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.284051 django-viewflow-2.0.0b4/viewflow/templates/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      672 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/400.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1183 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/403.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      695 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/404.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      832 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/500.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.284051 django-viewflow-2.0.0b4/viewflow/templates/admin/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      151 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_change_form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      637 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_change_form_object_tools.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1206 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_change_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2998 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_transition_form.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.144051 django-viewflow-2.0.0b4/viewflow/templates/formtools/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.284051 django-viewflow-2.0.0b4/viewflow/templates/formtools/wizard/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      794 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/formtools/wizard/wizard_form.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.296051 django-viewflow-2.0.0b4/viewflow/templates/registration/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      757 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/logged_out.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1638 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/login.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1653 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/password_change_done.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2097 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/password_change_form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      586 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_complete.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      941 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      795 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_done.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      975 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3737 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/profile.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      926 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/registration/provider_list.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.296051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1776 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/base.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1211 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/base_lockscreen.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5946 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/base_page.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.296051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.296051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/import_export/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2571 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/import_export/export_action.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/import_export/import_action.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1061 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/plotly.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      831 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/swagger.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.304051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1938 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/app_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2467 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/list_bulk_actions.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      703 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/list_filter.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1401 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/list_pagination.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1860 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/object_detail_card.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1535 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/site_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      261 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/snackbar.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      851 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/view_action_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      358 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/viewflow_css.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      326 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/viewflow_js.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.304051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/material/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1864 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/material/circular_progress.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.304051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2787 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/confirm_delete.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3167 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/delete_action.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      523 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2979 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/form.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6184 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1210 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/transition.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.324051 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2768 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/assign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       40 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/base_page.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      339 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/celery_task_detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1738 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/flow_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2509 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/graph.bpmn
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4224 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/graph.svg
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4340 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_cancel.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8037 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_dashboard.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1288 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_data.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3696 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       41 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_tasks_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2716 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/start.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3339 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1104 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_assign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2899 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_base.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_cancel.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2777 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_detail.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_list.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_revive.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      740 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_unassign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      732 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_undo.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2847 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/tasks_assign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2851 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/tasks_unassign.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1371 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/workflow_menu.html
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1987 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/workflow_tasks_list.html
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.324051 django-viewflow-2.0.0b4/viewflow/templatetags/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templatetags/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      429 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templatetags/fsm.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8866 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templatetags/viewflow.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1470 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/templatetags/workflow.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1811 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/this_object.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.324051 django-viewflow-2.0.0b4/viewflow/urls/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1800 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/urls/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11582 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/urls/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11203 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/urls/model.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5347 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/urls/sites.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7314 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/utils.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.328051 django-viewflow-2.0.0b4/viewflow/views/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      707 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3991 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/actions.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1916 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3935 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/create.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3417 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/delete.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3465 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/detail.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1853 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/filters.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15971 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/list.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3844 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/search.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4714 2023-06-05 12:29:04.000000 django-viewflow-2.0.0b4/viewflow/views/update.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.348051 django-viewflow-2.0.0b4/viewflow/workflow/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      438 2022-07-13 10:36:23.000000 django-viewflow-2.0.0b4/viewflow/workflow/__init__.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6067 2023-04-27 11:52:17.000000 django-viewflow-2.0.0b4/viewflow/workflow/activation.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2417 2023-03-17 09:25:31.000000 django-viewflow-2.0.0b4/viewflow/workflow/admin.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      344 2023-04-24 08:09:15.000000 django-viewflow-2.0.0b4/viewflow/workflow/apps.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13505 2023-02-24 12:01:50.000000 django-viewflow-2.0.0b4/viewflow/workflow/base.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20092 2022-01-31 10:53:07.000000 django-viewflow-2.0.0b4/viewflow/workflow/chart.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1540 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b4/viewflow/workflow/context.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      142 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b4/viewflow/workflow/exceptions.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4242 2022-01-17 15:00:21.000000 django-viewflow-2.0.0b4/viewflow/workflow/fields.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.352051 django-viewflow-2.0.0b4/viewflow/workflow/flow/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      738 2023-04-17 08:01:45.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3994 2022-12-08 11:16:57.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/mixins.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6309 2023-04-17 08:01:26.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/nodes.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3307 2023-02-09 10:21:20.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/utils.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.352051 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1676 2022-12-08 09:41:38.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6320 2022-12-08 09:41:24.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/actions.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      903 2022-08-08 11:14:26.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/chart.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1254 2022-05-18 09:25:12.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/create.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5053 2023-05-24 08:03:19.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/dashboard.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3697 2022-12-27 05:50:40.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/detail.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2958 2021-12-14 11:27:01.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/filters.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6179 2023-05-24 07:46:01.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/list.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3642 2023-05-24 07:43:27.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/mixins.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1469 2022-07-11 07:29:24.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/views/update.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13545 2023-05-24 07:49:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/flow/viewset.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2912 2021-12-13 03:06:49.000000 django-viewflow-2.0.0b4/viewflow/workflow/lock.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9447 2022-12-21 06:55:27.000000 django-viewflow-2.0.0b4/viewflow/workflow/managers.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.388052 django-viewflow-2.0.0b4/viewflow/workflow/migrations/
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2444 2020-05-21 12:16:30.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0001_initial.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      956 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0002_fsmchange.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      426 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0003_task_owner_permission_change.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      658 2020-05-21 12:15:16.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0004_extend_fields_length.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      260 2020-05-21 12:27:44.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0004_subprocess.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      293 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0005_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      397 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0005_rename_flowcls.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4169 2020-05-21 12:17:10.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0006_i18n.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      282 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0006_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      724 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0007_owner_permission_obj.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      409 2019-10-28 09:00:22.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0007_task_assigned.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1534 2020-05-21 12:16:55.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      287 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0008_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      266 2019-10-28 12:09:38.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0009_merge.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2683 2023-04-24 08:20:10.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/0010_viewflow20.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b4/viewflow/workflow/migrations/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8354 2023-04-24 08:07:54.000000 django-viewflow-2.0.0b4/viewflow/workflow/models.py
-drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-06-05 12:30:22.392052 django-viewflow-2.0.0b4/viewflow/workflow/nodes/
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1119 2023-04-28 05:08:57.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/__init__.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2253 2023-04-27 11:59:45.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/end.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1816 2023-04-25 06:37:06.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/func.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2808 2023-04-27 10:58:01.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/handle.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1921 2022-12-08 08:45:46.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/if_gate.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2534 2023-05-09 06:58:04.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/job.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5061 2023-04-03 08:08:46.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/join.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3931 2023-04-03 09:48:31.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/mixins.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      933 2022-12-08 08:46:15.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/obsolete.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5657 2023-04-27 11:59:12.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/split.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5519 2023-04-27 10:05:03.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/start.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1474 2022-12-08 08:48:09.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/subprocess.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2548 2022-12-08 08:49:59.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/switch.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8082 2023-04-25 06:27:17.000000 django-viewflow-2.0.0b4/viewflow/workflow/nodes/view.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      372 2023-04-18 09:17:56.000000 django-viewflow-2.0.0b4/viewflow/workflow/signals.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      843 2020-06-13 08:59:51.000000 django-viewflow-2.0.0b4/viewflow/workflow/status.py
--rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1752 2020-05-18 11:34:55.000000 django-viewflow-2.0.0b4/viewflow/workflow/token.py
--rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      637 2020-06-01 11:53:45.000000 django-viewflow-2.0.0b4/viewflow/workflow/utils.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    34520 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/LICENSE
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1340 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/LICENSE_EXCEPTION
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      193 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/MANIFEST.in
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/PKG-INFO
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6963 2023-07-10 10:26:43.000000 django-viewflow-2.0.0b5/README.md
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/django_viewflow.egg-info/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1029 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/PKG-INFO
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11669 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        1 2023-01-10 07:03:38.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/not-zip-safe
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       33 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/requires.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        9 2023-07-10 10:45:02.000000 django-viewflow-2.0.0b5/django_viewflow.egg-info/top_level.txt
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      228 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/setup.cfg
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1405 2023-07-10 10:27:45.000000 django-viewflow-2.0.0b5/setup.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/viewflow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1200 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      482 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/apps.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1737 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/conf.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/viewflow/contrib/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/__init__.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.847388 django-viewflow-2.0.0b5/viewflow/contrib/admin/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1263 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/admin/__init__.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      444 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/admin/apps.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10383 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/auth.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/contrib/plotly/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      138 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2170 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/material.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2494 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/views.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2257 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/contrib/plotly/viewset.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4611 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fields.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/forms/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      753 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/forms/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    27485 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/forms/renderers.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/fsm/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      751 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7886 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/admin.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15456 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3001 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/chart.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      725 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/typing.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1568 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/views.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5438 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/fsm/viewset.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6787 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/jsonstore.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/de/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6147 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19568 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/es/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9136 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20862 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/fr/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9296 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21031 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/it/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9466 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21002 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/ja/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    10300 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    21914 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/kk/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      378 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17712 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/ko/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/pt/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      380 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17714 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/ru/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11819 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    23228 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      373 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17707 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/django.po
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.851388 django-viewflow-2.0.0b5/viewflow/management/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2742 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/management/__init__.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.855388 django-viewflow-2.0.0b5/viewflow/management/commands/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/management/commands/__init__.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2082 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/management/commands/flowexport.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2471 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/middleware.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/static/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/static/viewflow/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.855388 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2598 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/perfect-scrollbar.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19972 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/trix.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   460203 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/viewflow.min.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   220163 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/css/vis-network.min.css
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.859388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   182028 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   155276 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   206260 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   173620 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156236 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   135984 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   339600 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   215704 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3314 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   164912 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   128352 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.863388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86508 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64960 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    94048 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    72088 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86184 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64740 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91968 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70360 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85692 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64320 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    92864 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70760 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    86444 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    65484 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    93228 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    71284 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    85876 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    64632 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    91728 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    70280 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    84224 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    63048 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    90784 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    68328 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4173 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.867388 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077522 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1077336 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   718180 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   603192 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   213035 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   184911 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.867388 django-viewflow-2.0.0b5/viewflow/static/viewflow/img/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1311 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/img/favicon.png
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2200 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/img/user.png
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    19549 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    77830 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    17674 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/smartcrop.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   229927 2023-01-27 12:19:41.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/trix.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   156812 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/turbo.es2017-umd.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   564585 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  1658508 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js.map
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)   490205 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)  2010720 2023-07-10 10:41:26.000000 django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js.map
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      672 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/400.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1183 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/403.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      695 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/404.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      832 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/500.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/admin/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      151 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      637 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_form_object_tools.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1206 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2998 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_transition_form.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.843388 django-viewflow-2.0.0b5/viewflow/templates/formtools/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/formtools/wizard/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      794 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/formtools/wizard/wizard_form.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.875388 django-viewflow-2.0.0b5/viewflow/templates/registration/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      757 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/logged_out.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1638 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/login.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1653 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_done.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2097 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      586 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      941 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      795 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_done.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      975 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3737 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/profile.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      926 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/registration/provider_list.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1776 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/base.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1211 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_lockscreen.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5946 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_page.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2571 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/export_action.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/import_action.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1061 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/plotly.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      831 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/swagger.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1938 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/app_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2467 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_bulk_actions.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      703 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_filter.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1401 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_pagination.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1860 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/object_detail_card.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1535 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/site_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      261 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/snackbar.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      851 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/view_action_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      358 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/viewflow_css.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      326 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/viewflow_js.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/material/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1864 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/material/circular_progress.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.879388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2787 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/confirm_delete.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3167 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/delete_action.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      523 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3137 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/form.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6184 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1210 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/transition.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2768 2023-01-12 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/assign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       40 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/base_page.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      339 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/celery_task_detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1738 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/flow_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2509 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.bpmn
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4224 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.svg
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4340 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_cancel.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8037 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_dashboard.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1288 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_data.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3696 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)       41 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_tasks_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2716 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/start.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3339 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1104 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_assign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2899 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_base.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_cancel.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2777 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_detail.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      633 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_list.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      736 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_revive.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      740 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_unassign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      732 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_undo.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2847 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_assign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2851 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_unassign.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1371 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_menu.html
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1987 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_tasks_list.html
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/templatetags/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      429 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/fsm.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8866 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/viewflow.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1470 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/templatetags/workflow.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1811 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/this_object.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/urls/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1800 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11582 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    11203 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/model.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5347 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/urls/sites.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     7314 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/utils.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.883388 django-viewflow-2.0.0b5/viewflow/views/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      707 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3991 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/actions.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1916 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3935 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/create.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3417 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/delete.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3465 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/detail.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1853 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/filters.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    15971 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/list.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3844 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/search.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4714 2023-07-10 10:40:59.000000 django-viewflow-2.0.0b5/viewflow/views/update.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.887388 django-viewflow-2.0.0b5/viewflow/workflow/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      438 2022-07-13 10:36:23.000000 django-viewflow-2.0.0b5/viewflow/workflow/__init__.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6067 2023-04-27 11:52:17.000000 django-viewflow-2.0.0b5/viewflow/workflow/activation.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2417 2023-03-17 09:25:31.000000 django-viewflow-2.0.0b5/viewflow/workflow/admin.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      344 2023-04-24 08:09:15.000000 django-viewflow-2.0.0b5/viewflow/workflow/apps.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13505 2023-02-24 12:01:50.000000 django-viewflow-2.0.0b5/viewflow/workflow/base.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    20092 2022-01-31 10:53:07.000000 django-viewflow-2.0.0b5/viewflow/workflow/chart.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1540 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/workflow/context.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      142 2019-07-03 02:25:35.000000 django-viewflow-2.0.0b5/viewflow/workflow/exceptions.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4431 2023-07-04 09:48:28.000000 django-viewflow-2.0.0b5/viewflow/workflow/fields.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.887388 django-viewflow-2.0.0b5/viewflow/workflow/flow/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      738 2023-04-17 08:01:45.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3994 2022-12-08 11:16:57.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/mixins.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6309 2023-04-17 08:01:26.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/nodes.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3307 2023-02-09 10:21:20.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/utils.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.887388 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1676 2022-12-08 09:41:38.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6320 2022-12-08 09:41:24.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/actions.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      903 2022-08-08 11:14:26.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/chart.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1254 2022-05-18 09:25:12.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/create.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5113 2023-07-10 06:38:27.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/dashboard.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3697 2022-12-27 05:50:40.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/detail.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2958 2021-12-14 11:27:01.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/filters.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     6179 2023-05-24 07:46:01.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/list.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3642 2023-05-24 07:43:27.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/mixins.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1469 2022-07-11 07:29:24.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/views/update.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)    13545 2023-07-07 09:40:27.000000 django-viewflow-2.0.0b5/viewflow/workflow/flow/viewset.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2912 2021-12-13 03:06:49.000000 django-viewflow-2.0.0b5/viewflow/workflow/lock.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     9876 2023-07-07 10:21:50.000000 django-viewflow-2.0.0b5/viewflow/workflow/managers.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.891388 django-viewflow-2.0.0b5/viewflow/workflow/migrations/
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2444 2020-05-21 12:16:30.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0001_initial.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      956 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0002_fsmchange.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      426 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0003_task_owner_permission_change.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      658 2020-05-21 12:15:16.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0004_extend_fields_length.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      260 2020-05-21 12:27:44.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0004_subprocess.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      293 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0005_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      397 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0005_rename_flowcls.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4169 2020-05-21 12:17:10.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0006_i18n.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      282 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0006_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      724 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0007_owner_permission_obj.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      409 2019-10-28 09:00:22.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0007_task_assigned.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1534 2020-05-21 12:16:55.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      287 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0008_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      266 2019-10-28 12:09:38.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0009_merge.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2683 2023-04-24 08:20:10.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0010_viewflow20.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      747 2023-07-05 11:28:45.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/0011_alter_task_created_and_more.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2019-07-03 02:23:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/migrations/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8481 2023-07-06 09:15:24.000000 django-viewflow-2.0.0b5/viewflow/workflow/models.py
+drwxrwxr-x   0 kmmbvnr   (1000) kmmbvnr   (1000)        0 2023-07-10 10:45:02.895388 django-viewflow-2.0.0b5/viewflow/workflow/nodes/
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1119 2023-04-28 05:08:57.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/__init__.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2253 2023-04-27 11:59:45.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/end.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1816 2023-04-25 06:37:06.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/func.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2808 2023-04-27 10:58:01.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/handle.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1972 2023-07-04 09:24:08.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/if_gate.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2534 2023-05-09 06:58:04.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/job.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5061 2023-04-03 08:08:46.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/join.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     3931 2023-04-03 09:48:31.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/mixins.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      933 2022-12-08 08:46:15.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/obsolete.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5657 2023-04-27 11:59:12.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/split.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     5519 2023-04-27 10:05:03.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/start.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     4543 2023-07-04 11:54:12.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/subprocess.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     2548 2022-12-08 08:49:59.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/switch.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     8082 2023-04-25 06:27:17.000000 django-viewflow-2.0.0b5/viewflow/workflow/nodes/view.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      372 2023-04-18 09:17:56.000000 django-viewflow-2.0.0b5/viewflow/workflow/signals.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)      843 2020-06-13 08:59:51.000000 django-viewflow-2.0.0b5/viewflow/workflow/status.py
+-rw-r--r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1752 2020-05-18 11:34:55.000000 django-viewflow-2.0.0b5/viewflow/workflow/token.py
+-rw-rw-r--   0 kmmbvnr   (1000) kmmbvnr   (1000)     1226 2023-07-07 09:48:41.000000 django-viewflow-2.0.0b5/viewflow/workflow/utils.py
```

### Comparing `django-viewflow-2.0.0b4/LICENSE` & `django-viewflow-2.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/LICENSE_EXCEPTION` & `django-viewflow-2.0.0b5/LICENSE_EXCEPTION`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/PKG-INFO` & `django-viewflow-2.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-viewflow
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: Reusable library to build business applications fast
 Home-page: UNKNOWN
 Author: Mikhail Podgurskiy
 Author-email: kmmbvnr@gmail.com
 License: AGPL
 Description: UNKNOWN
 Keywords: django,admin,workflow,fsm,bpm,bpmn
```

### Comparing `django-viewflow-2.0.0b4/README.md` & `django-viewflow-2.0.0b5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -175,25 +175,21 @@
 
 Viewflow PRO has a commercial-friendly license allowing private forks and
 modifications of Viewflow. You can find the commercial license terms in
 [COMM-LICENSE](./COMM-LICENSE).
 
 ## Changelog
 
-2.0.0.b4 2023-06-05
+2.0.0.b5 2023-07-10
 -------------------
 
-- New flow.SplitFirst Node
-- New celery.Timer Node
-- Expose REST API with drf-spectacular
-- Expose list_ordering_fields in a ModelViewset
-- Retain history and return to the Inbox/Queue list views after completing a flow task
-- Enable smooth page transitions in Chrome/Safari
-- Hotwire/Turbo integration for Django Admin with viewflow.contrib.admin app
-- Resolved issue with viewflow.fsm reporting unmet condition messages
+- Alow attach layout to forms in default form rendering template
+- Fix subprocess node activation
+- Added db indexes for workflow models
+- Improve workflow REST API support
 
 
 
 [build]: https://img.shields.io/github/actions/workflow/status/viewflow/viewflow/django.yml?branch=main
 [coverage]: https://img.shields.io/coveralls/github/viewflow/viewflow/v2
 [travis-svg]: https://travis-ci.org/viewflow/viewflow.svg
 [travis]: https://travis-ci.org/viewflow/viewflow
```

### Comparing `django-viewflow-2.0.0b4/django_viewflow.egg-info/PKG-INFO` & `django-viewflow-2.0.0b5/django_viewflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: django-viewflow
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: Reusable library to build business applications fast
 Home-page: UNKNOWN
 Author: Mikhail Podgurskiy
 Author-email: kmmbvnr@gmail.com
 License: AGPL
 Description: UNKNOWN
 Keywords: django,admin,workflow,fsm,bpm,bpmn
```

### Comparing `django-viewflow-2.0.0b4/django_viewflow.egg-info/SOURCES.txt` & `django-viewflow-2.0.0b5/django_viewflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,15 @@
 viewflow/workflow/migrations/0006_merge.py
 viewflow/workflow/migrations/0007_owner_permission_obj.py
 viewflow/workflow/migrations/0007_task_assigned.py
 viewflow/workflow/migrations/0008_jsonfield_and_artifact.py
 viewflow/workflow/migrations/0008_merge.py
 viewflow/workflow/migrations/0009_merge.py
 viewflow/workflow/migrations/0010_viewflow20.py
+viewflow/workflow/migrations/0011_alter_task_created_and_more.py
 viewflow/workflow/migrations/__init__.py
 viewflow/workflow/nodes/__init__.py
 viewflow/workflow/nodes/end.py
 viewflow/workflow/nodes/func.py
 viewflow/workflow/nodes/handle.py
 viewflow/workflow/nodes/if_gate.py
 viewflow/workflow/nodes/job.py
```

### Comparing `django-viewflow-2.0.0b4/setup.py` & `django-viewflow-2.0.0b5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 README = open("README.md", "r", encoding="utf-8").read()
 
 setuptools.setup(
     name="django-viewflow",
-    version="2.0.0b4",
+    version="2.0.0b5",
     author_email="kmmbvnr@gmail.com",
     author="Mikhail Podgurskiy",
     description="Reusable library to build business applications fast",
     include_package_data=True,
     keywords=["django", "admin", "workflow", "fsm", "bpm", "bpmn"],
     license="AGPL",
     # long_description_content_type="text/markdown",
```

### Comparing `django-viewflow-2.0.0b4/viewflow/__init__.py` & `django-viewflow-2.0.0b5/viewflow/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/conf.py` & `django-viewflow-2.0.0b5/viewflow/conf.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/contrib/admin/__init__.py` & `django-viewflow-2.0.0b5/viewflow/contrib/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/contrib/auth.py` & `django-viewflow-2.0.0b5/viewflow/contrib/auth.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/contrib/plotly/material.py` & `django-viewflow-2.0.0b5/viewflow/contrib/plotly/material.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/contrib/plotly/views.py` & `django-viewflow-2.0.0b5/viewflow/contrib/plotly/views.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/contrib/plotly/viewset.py` & `django-viewflow-2.0.0b5/viewflow/contrib/plotly/viewset.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fields.py` & `django-viewflow-2.0.0b5/viewflow/fields.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/forms/__init__.py` & `django-viewflow-2.0.0b5/viewflow/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/forms/renderers.py` & `django-viewflow-2.0.0b5/viewflow/forms/renderers.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/__init__.py` & `django-viewflow-2.0.0b5/viewflow/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/admin.py` & `django-viewflow-2.0.0b5/viewflow/fsm/admin.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/base.py` & `django-viewflow-2.0.0b5/viewflow/fsm/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/chart.py` & `django-viewflow-2.0.0b5/viewflow/fsm/chart.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/typing.py` & `django-viewflow-2.0.0b5/viewflow/fsm/typing.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/views.py` & `django-viewflow-2.0.0b5/viewflow/fsm/views.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/fsm/viewset.py` & `django-viewflow-2.0.0b5/viewflow/fsm/viewset.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/jsonstore.py` & `django-viewflow-2.0.0b5/viewflow/jsonstore.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/de/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/de/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/es/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/es/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/fr/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/fr/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/it/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/it/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/ja/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/ja/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/kk/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/ko/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/pt/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/ru/LC_MESSAGES/django.mo` & `django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/ru/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/locale/zh_Hans/LC_MESSAGES/django.po` & `django-viewflow-2.0.0b5/viewflow/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/management/__init__.py` & `django-viewflow-2.0.0b5/viewflow/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/management/commands/flowexport.py` & `django-viewflow-2.0.0b5/viewflow/management/commands/flowexport.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/middleware.py` & `django-viewflow-2.0.0b5/viewflow/middleware.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/css/perfect-scrollbar.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/perfect-scrollbar.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/css/trix.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/trix.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/css/viewflow.min.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/viewflow.min.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/css/vis-network.min.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-outlined.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-round.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-sharp.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons-two-tone.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/material-icons/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Black.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Light.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Medium.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-RegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-Thin.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/Roboto-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/roboto/roboto-fontface.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.eot`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.otf`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.ttf`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/SimpleIcons.woff2`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/fonts/simple-icons/simple-icons.min.css`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/img/favicon.png` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/img/favicon.png`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/img/user.png` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/img/user.png`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/perfect-scrollbar.min.js` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/perfect-scrollbar.min.js.map`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/smartcrop.js` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/smartcrop.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/trix.js` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/trix.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/turbo.es2017-umd.js` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/turbo.es2017-umd.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/viewflow.min.js` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/viewflow.min.js.map` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/viewflow.min.js.map`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/vis-network.min.js` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/static/viewflow/js/vis-network.min.js.map` & `django-viewflow-2.0.0b5/viewflow/static/viewflow/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/400.html` & `django-viewflow-2.0.0b5/viewflow/templates/400.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/403.html` & `django-viewflow-2.0.0b5/viewflow/templates/403.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/404.html` & `django-viewflow-2.0.0b5/viewflow/templates/404.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/500.html` & `django-viewflow-2.0.0b5/viewflow/templates/500.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_change_form_object_tools.html` & `django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_change_list.html` & `django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_change_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/admin/fsm_transition_form.html` & `django-viewflow-2.0.0b5/viewflow/templates/admin/fsm_transition_form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/formtools/wizard/wizard_form.html` & `django-viewflow-2.0.0b5/viewflow/templates/formtools/wizard/wizard_form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/logged_out.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/login.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/password_change_done.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/password_change_form.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_complete.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_confirm.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_done.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/password_reset_form.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/profile.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/profile.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/registration/provider_list.html` & `django-viewflow-2.0.0b5/viewflow/templates/registration/provider_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/base.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/base.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/base_lockscreen.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_lockscreen.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/base_page.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/base_page.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/import_export/export_action.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/import_export/export_action.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/plotly.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/plotly.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/contrib/swagger.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/contrib/swagger.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/app_menu.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/app_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/list_bulk_actions.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_bulk_actions.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/list_filter.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_filter.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/list_pagination.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/list_pagination.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/object_detail_card.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/object_detail_card.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/site_menu.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/site_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/includes/view_action_menu.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/includes/view_action_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/material/circular_progress.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/material/circular_progress.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/confirm_delete.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/delete_action.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/delete_action.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/detail.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/detail.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/form.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/form.html`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,19 @@
             </section>
 
             {% block form %}
               <vf-form>
                 <form class="vf-form" method="POST" {% if form.is_multipart %} enctype="multipart/form-data"{% endif %}>
                   {% csrf_token %}
                   <section class="vf-card__form">
-                    {% render form view.layout %}
+                    {% if form.layout %}
+                      {% render form form.layout %}
+                    {% else %}
+                      {% render form view.layout %}
+                    {% endif %}
                   </section>
                   {% block form-actions %}
                     <section class="mdc-card__actions vf-card__actions">
                       {% block form-actions-list %}
                         <button class="mdc-button mdc-card__action mdc-card__action--button mdc-button--raised" type="submit">{% trans "Save" %}</button>
                       {% endblock %}
                     </section>
```

#### html2text {}

```diff
@@ -12,12 +12,13 @@
 %} {% endif %} {% if view.object.pk %}{% if detail_url %}{% trans 'Change' %}{%
 else %}{{ view.object }}{% endif %}{% else %}{% trans 'Add' %}{% endif %} {%
 endblock %} *****
 {% endblock %} {% block form-header-menu %}
 {% include 'viewflow/includes/view_action_menu.html' with view=view only %}
 {% endblock %}  {% block form %}
 % if form.is_multipart %} enctype="multipart/form-data"{% endif %}> {%
-csrf_token %}  {% render form view.layout %}  {% block form-actions %}  {%
-block form-actions-list %} {% trans "Save" %} {% endblock %}  {% endblock %}
+csrf_token %}  {% if form.layout %} {% render form form.layout %} {% else %} {%
+render form view.layout %} {% endif %}  {% block form-actions %}  {% block
+form-actions-list %} {% trans "Save" %} {% endblock %}  {% endblock %}
  {% endblock form %}
 {% endblock form-cell %}
 {% endblock content %}
```

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/list.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/views/transition.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/views/transition.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/assign.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/assign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/flow_menu.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/flow_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/graph.bpmn` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.bpmn`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/graph.svg` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/graph.svg`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_cancel.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_cancel.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_dashboard.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_dashboard.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_data.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_data.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_detail.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_detail.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/process_list.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/process_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/start.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/start.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_assign.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_assign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_base.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_base.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_cancel.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_cancel.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_detail.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_detail.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_list.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_revive.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_revive.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_unassign.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_unassign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/task_undo.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/task_undo.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/tasks_assign.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_assign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/tasks_unassign.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/tasks_unassign.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/workflow_menu.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_menu.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templates/viewflow/workflow/workflow_tasks_list.html` & `django-viewflow-2.0.0b5/viewflow/templates/viewflow/workflow/workflow_tasks_list.html`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templatetags/viewflow.py` & `django-viewflow-2.0.0b5/viewflow/templatetags/viewflow.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/templatetags/workflow.py` & `django-viewflow-2.0.0b5/viewflow/templatetags/workflow.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/this_object.py` & `django-viewflow-2.0.0b5/viewflow/this_object.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/urls/__init__.py` & `django-viewflow-2.0.0b5/viewflow/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/urls/base.py` & `django-viewflow-2.0.0b5/viewflow/urls/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/urls/model.py` & `django-viewflow-2.0.0b5/viewflow/urls/model.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/urls/sites.py` & `django-viewflow-2.0.0b5/viewflow/urls/sites.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/utils.py` & `django-viewflow-2.0.0b5/viewflow/utils.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/__init__.py` & `django-viewflow-2.0.0b5/viewflow/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/actions.py` & `django-viewflow-2.0.0b5/viewflow/views/actions.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/base.py` & `django-viewflow-2.0.0b5/viewflow/views/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/create.py` & `django-viewflow-2.0.0b5/viewflow/views/create.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/delete.py` & `django-viewflow-2.0.0b5/viewflow/views/delete.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/detail.py` & `django-viewflow-2.0.0b5/viewflow/views/detail.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/filters.py` & `django-viewflow-2.0.0b5/viewflow/views/filters.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/list.py` & `django-viewflow-2.0.0b5/viewflow/views/list.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/search.py` & `django-viewflow-2.0.0b5/viewflow/views/search.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/views/update.py` & `django-viewflow-2.0.0b5/viewflow/views/update.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/activation.py` & `django-viewflow-2.0.0b5/viewflow/workflow/activation.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/admin.py` & `django-viewflow-2.0.0b5/viewflow/workflow/admin.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/base.py` & `django-viewflow-2.0.0b5/viewflow/workflow/base.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/chart.py` & `django-viewflow-2.0.0b5/viewflow/workflow/chart.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/context.py` & `django-viewflow-2.0.0b5/viewflow/workflow/context.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/fields.py` & `django-viewflow-2.0.0b5/viewflow/workflow/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,86 +7,99 @@
 from viewflow.workflow.exceptions import FlowRuntimeError
 from viewflow.workflow.token import Token
 
 
 @lru_cache(maxsize=None)
 def import_flow_by_ref(flow_strref):
     """Return flow class by flow string reference."""
-    app_label, flow_path = flow_strref.split('/')
+    app_label, flow_path = flow_strref.split("/")
     # TODO Raise if imported class is not Flow
-    return import_string('{}.{}'.format(get_app_package(app_label), flow_path))
+    return import_string("{}.{}".format(get_app_package(app_label), flow_path))
 
 
 @lru_cache(maxsize=None)
 def get_flow_ref(flow_class):
     """Convert flow class to string reference."""
     module = "{}.{}".format(flow_class.__module__, flow_class.__name__)
     app_label, app_package = get_containing_app_data(module)
     if app_label is None:
-        raise FlowRuntimeError('No application found for {}. Check your INSTALLED_APPS setting'.format(module))
+        raise FlowRuntimeError(
+            "No application found for {}. Check your INSTALLED_APPS setting".format(
+                module
+            )
+        )
 
-    subpath = module[len(app_package) + 1:]
+    subpath = module[len(app_package) + 1 :]
     return "{}/{}".format(app_label, subpath)
 
 
 @lru_cache(maxsize=None)
 def import_task_by_ref(task_strref):
     """Return flow task by reference like `app_label/path.to.Flowclass.task_name`."""
-    app_label, flow_path = task_strref.split('/')
-    flow_path, task_name = flow_path.rsplit('.', 1)
-    flow_class = import_string('{}.{}'.format(get_app_package(app_label), flow_path))
+    app_label, flow_path = task_strref.split("/")
+    flow_path, task_name = flow_path.rsplit(".", 1)
+    flow_class = import_string("{}.{}".format(get_app_package(app_label), flow_path))
     # TODO Raise if imported class is not Node
     return flow_class.instance.node(task_name)
 
 
 @lru_cache(maxsize=None)
 def get_task_ref(flow_task):
     """Convert task to the string reference suitable to store in the db."""
     module = flow_task.flow_class.__module__
     app_label, app_package = get_containing_app_data(module)
     if app_label is None:
-        raise FlowRuntimeError('No application found for {}. Check your INSTALLED_APPS setting'.format(module))
-
-    subpath = module[len(app_package) + 1:]
-
-    return "{}/{}.{}.{}".format(app_label, subpath, flow_task.flow_class.__name__, flow_task.name)
+        raise FlowRuntimeError(
+            "No application found for {}. Check your INSTALLED_APPS setting".format(
+                module
+            )
+        )
+
+    subpath = module[len(app_package) + 1 :]
+
+    return "{}/{}.{}.{}".format(
+        app_label, subpath, flow_task.flow_class.__name__, flow_task.name
+    )
 
 
 class FlowReferenceField(models.CharField):
     description = """Flow class reference field,
     stores flow as app_label/flows.FlowName> to
     avoid possible collisions with app name changes"""
 
     def __init__(self, *args, **kwargs):  # noqa D1o2
-        kwargs.setdefault('max_length', 250)
+        kwargs.setdefault("max_length", 250)
         super(FlowReferenceField, self).__init__(*args, **kwargs)
 
     def to_python(self, value):  # noqa D102
         if value:
             return import_flow_by_ref(value)
         return value
 
     def from_db_value(self, value, expression, connection):
         if value is None:
             return value
-        return import_flow_by_ref(value)
+        try:
+            return import_flow_by_ref(value)
+        except LookupError:
+            return None
 
     def get_prep_value(self, value):  # noqa D1o2
         if value and not isinstance(value, str):
             return get_flow_ref(value)
         return value
 
     def value_to_string(self, obj):  # noqa D1o2
         value = super(FlowReferenceField, self).value_from_object(obj)
         return self.get_prep_value(value)
 
 
 class TaskReferenceField(models.CharField):
     def __init__(self, *args, **kwargs):
-        kwargs.setdefault('max_length', 255)
+        kwargs.setdefault("max_length", 255)
         super(TaskReferenceField, self).__init__(*args, **kwargs)
 
     def to_python(self, value):
         if value:
             return import_task_by_ref(value)  # TODO Raise  ValidationError
         return value
 
@@ -103,15 +116,15 @@
     def value_to_string(self, obj):  # noqa D102
         value = super(TaskReferenceField, self).value_from_object(obj)
         return self.get_prep_value(value)
 
 
 class TokenField(models.CharField):
     def __init__(self, *args, **kwargs):
-        kwargs.setdefault('max_length', 150)
+        kwargs.setdefault("max_length", 150)
         super(TokenField, self).__init__(*args, **kwargs)
 
     def from_db_value(self, value, expression, connection):
         if value is None:
             return value
         return Token(value)
```

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/__init__.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/mixins.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/mixins.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/nodes.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/nodes.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/utils.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/utils.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/__init__.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/actions.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/actions.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/chart.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/chart.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/create.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/create.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/dashboard.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     # def queryset(self):
     #    if self.viewset is not None and hasattr(self.viewset, 'get_task_queryset'):
     #        return self.viewset.get_queryset(self.request)
     #    return self.flow_class.task_class._default_manager
 
     def get_context_data(self, **kwargs):
         sorted_nodes, _ = chart.topsort(self.flow_class)
-        nodes = [node for node in sorted_nodes if node.task_type in ["HUMAN", "JOB"]]
+        nodes = [
+            node
+            for node in sorted_nodes
+            if node.task_type in ["HUMAN", "JOB", "SUBPROCESS"]
+        ]
 
         start_nodes = [
             {"node": node, "can_execute": node.can_execute(self.request.user)}
             for node in self.flow_class.instance.get_start_nodes()
         ]
 
         end_nodes = [node for node in sorted_nodes if node.task_type in ["END"]]
```

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/detail.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/detail.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/filters.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/filters.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/list.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/list.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/mixins.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/views/update.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/views/update.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/flow/viewset.py` & `django-viewflow-2.0.0b5/viewflow/workflow/flow/viewset.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/lock.py` & `django-viewflow-2.0.0b5/viewflow/workflow/lock.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/managers.py` & `django-viewflow-2.0.0b5/viewflow/workflow/managers.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models.query import QuerySet
 from django.db.models.constants import LOOKUP_SEP
 from django.db.models.query import ModelIterable
 
 from .status import STATUS
+from .utils import get_next_process_task
 
 
 def _available_flows(flow_classes, user):
     result = []
     for flow_class in flow_classes:
         if flow_class.instance.has_view_permission(user):
             result.append(flow_class)
@@ -253,30 +254,36 @@
     def next_user_task(self, process, user):
         """
         Lookup for the next task for a user execution.
 
         Prefer assigned tasks first, if not, return first task from user queue
         """
 
-        # first try to find an assigned task
-        task = self.filter(process=process, owner=user, status=STATUS.ASSIGNED).first()
+        # task inside a same process
+        task = get_next_process_task(self, process, user)
 
-        # lookup for a task in a queue
+        # task inside subprocess
         if task is None:
-            task = (
-                self.user_queue(user).filter(process=process, status=STATUS.NEW).first()
-            )
-
-        # lookup for a job
-        if task is None:
-            task = (
-                self.filter(process=process, flow_task_type='JOB', status__in=[
-                    STATUS.NEW, STATUS.SCHEDULED, STATUS.STARTED
-                ]).first()
-            )
+            subprocess_task = self.filter(process__parent_task__process=process).first()
+            if subprocess_task:
+                task = get_next_process_task(self, subprocess_task.process, user)
+
+        # task inside parent process
+        if task is None and process.parent_task_id:
+            task = get_next_process_task(self, process.parent_task.process, user)
+
+        # task inside other subprocesses of parent task
+        if task is None and process.parent_task_id:
+            processes = process.__class__._default_manager.filter(
+                parent_task__process=process.parent_task.process
+            ).exclude(pk=process.pk)
+            for sub_process in processes:
+                task = get_next_process_task(self, sub_process, user)
+                if task:
+                    break
 
         return task
 
     def _chain(self, **kwargs):
         chained = super()._chain(**kwargs)
         if hasattr(self, "_coerced"):
             chained._coerced = self._coerced
```

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0001_initial.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0002_fsmchange.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0002_fsmchange.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0004_extend_fields_length.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0004_extend_fields_length.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0006_i18n.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0006_i18n.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0007_owner_permission_obj.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0007_owner_permission_obj.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0008_jsonfield_and_artifact.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/migrations/0010_viewflow20.py` & `django-viewflow-2.0.0b5/viewflow/workflow/migrations/0010_viewflow20.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/models.py` & `django-viewflow-2.0.0b5/viewflow/workflow/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         _("Status"),
         choices=status.STATUS.choices,
         db_index=True,
         default=status.STATUS.NEW,
         max_length=50,
     )
 
-    created = models.DateTimeField(_("Created"), default=timezone.now)
+    created = models.DateTimeField(_("Created"), default=timezone.now, db_index=True)
     assigned = models.DateTimeField(_("Assigned"), blank=True, null=True)
     started = models.DateTimeField(_("Started"), blank=True, null=True)
     finished = models.DateTimeField(_("Finished"), blank=True, null=True)
 
     previous = models.ManyToManyField(
         "self", symmetrical=False, related_name="leading", verbose_name=_("Previous")
     )
@@ -245,14 +245,17 @@
     )
     artifact_object_id = models.PositiveIntegerField(null=True, blank=True)
 
     class Meta:  # noqa D101
         ordering = ["-created"]
         verbose_name = _("Process")
         verbose_name_plural = _("Process list")
+        indexes = [
+            models.Index(fields=["artifact_content_type", "artifact_object_id"]),
+        ]
 
 
 class Task(AbstractTask):
     """Default viewflow Task model."""
 
     process = models.ForeignKey(
         on_delete=models.CASCADE,
```

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/__init__.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/end.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/end.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/func.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/func.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/handle.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/handle.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/if_gate.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/if_gate.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,53 +3,59 @@
 from ..base import Node, Edge
 from ..activation import Activation
 from . import mixins
 
 
 class IfActivation(Activation):
     """Conditionally activate one of outgoing nodes."""
+
     _condition_result = None
 
     @Activation.status.super()
     def activate(self):
         self._condition_result = self.flow_task.condition(self)
 
     @Activation.status.super()
     def create_next(self):
-        next_node = self.flow_task._on_true if self._condition_result else self.flow_task._on_false
+        next_node = (
+            self.flow_task._on_true
+            if self._condition_result
+            else self.flow_task._on_false
+        )
         if next_node:
             yield next_node._create(self, self.task.token)
 
 
 class If(Node):
     """If gateway, activate one of outgoing node."""
+
     activation_class = IfActivation
 
-    task_type = 'EXCLUSIVE_GATEWAY'
+    task_type = "EXCLUSIVE_GATEWAY"
 
     shape = {
-        'width': 50,
-        'height': 50,
-        'svg': """
+        "width": 50,
+        "height": 50,
+        "svg": """
             <path class="gateway" d="M25,0L50,25L25,50L0,25L25,0"/>
             <text class="gateway-marker" font-size="16px" x="25" y="31">X</text>
-        """
+        """,
     }
 
-    bpmn_element = 'exclusiveGateway'
+    bpmn_element = "exclusiveGateway"
 
     def __init__(self, cond, **kwargs):
         super().__init__(**kwargs)
         self._condition = cond
         self._on_true = None
         self._on_false = None
 
     def _outgoing(self):
-        yield Edge(src=self, dst=self._on_true, edge_class='cond_true')
-        yield Edge(src=self, dst=self._on_false, edge_class='cond_false')
+        yield Edge(src=self, dst=self._on_true, edge_class="cond_true")
+        yield Edge(src=self, dst=self._on_false, edge_class="cond_false")
 
     def _resolve(self, instance):
         super()._resolve(instance)
         self._on_true = this.resolve(instance, self._on_true)
         self._on_false = this.resolve(instance, self._on_false)
 
     @property
```

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/job.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/job.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/join.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/join.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/mixins.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/mixins.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/obsolete.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/obsolete.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/split.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/split.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/start.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/start.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/switch.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/switch.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/nodes/view.py` & `django-viewflow-2.0.0b5/viewflow/workflow/nodes/view.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/status.py` & `django-viewflow-2.0.0b5/viewflow/workflow/status.py`

 * *Files identical despite different names*

### Comparing `django-viewflow-2.0.0b4/viewflow/workflow/token.py` & `django-viewflow-2.0.0b5/viewflow/workflow/token.py`

 * *Files identical despite different names*

