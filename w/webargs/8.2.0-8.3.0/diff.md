# Comparing `tmp/webargs-8.2.0.tar.gz` & `tmp/webargs-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webargs-8.2.0.tar", last modified: Tue Jul 12 13:20:40 2022, max compression
+gzip compressed data, was "webargs-8.3.0.tar", last modified: Mon Jul 10 14:47:47 2023, max compression
```

## Comparing `webargs-8.2.0.tar` & `webargs-8.3.0.tar`

### file list

```diff
@@ -1,163 +1,64 @@
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.866429 webargs-8.2.0/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2813 2022-07-12 13:19:34.000000 webargs-8.2.0/AUTHORS.rst
--rw-r--r--   0 jerome    (1000) jerome    (1000)    40791 2022-07-12 13:19:34.000000 webargs-8.2.0/CHANGELOG.rst
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4307 2022-07-12 13:19:34.000000 webargs-8.2.0/CONTRIBUTING.rst
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1074 2020-01-25 15:51:49.000000 webargs-8.2.0/LICENSE
--rw-r--r--   0 jerome    (1000) jerome    (1000)       87 2022-01-02 11:05:44.000000 webargs-8.2.0/MANIFEST.in
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5385 2022-07-12 13:20:40.866429 webargs-8.2.0/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3770 2022-07-12 13:19:34.000000 webargs-8.2.0/README.rst
--rw-r--r--   0 jerome    (1000) jerome    (1000)       81 2022-07-12 13:19:34.000000 webargs-8.2.0/pyproject.toml
--rw-r--r--   0 jerome    (1000) jerome    (1000)      220 2022-07-12 13:20:40.866429 webargs-8.2.0/setup.cfg
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3428 2022-07-12 13:19:34.000000 webargs-8.2.0/setup.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:39.862414 webargs-8.2.0/src/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:39.914414 webargs-8.2.0/src/webargs/
--rwxr-xr-x   0 jerome    (1000) jerome    (1000)      646 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5980 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/aiohttpparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1083 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/asyncparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3051 2021-03-12 22:42:08.000000 webargs-8.2.0/src/webargs/bottleparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)    29292 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/core.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2484 2021-03-12 22:42:08.000000 webargs-8.2.0/src/webargs/djangoparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6584 2021-03-12 22:42:08.000000 webargs-8.2.0/src/webargs/falconparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4387 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/fields.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3725 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/flaskparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3080 2021-11-04 22:17:20.000000 webargs-8.2.0/src/webargs/multidictproxy.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2021-03-12 22:42:08.000000 webargs-8.2.0/src/webargs/py.typed
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6837 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/pyramidparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     9861 2021-03-12 22:42:08.000000 webargs-8.2.0/src/webargs/testing.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5270 2022-07-12 13:19:34.000000 webargs-8.2.0/src/webargs/tornadoparser.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:39.922414 webargs-8.2.0/src/webargs.egg-info/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5385 2022-07-12 13:20:39.000000 webargs-8.2.0/src/webargs.egg-info/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6640 2022-07-12 13:20:39.000000 webargs-8.2.0/src/webargs.egg-info/SOURCES.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2022-07-12 13:20:39.000000 webargs-8.2.0/src/webargs.egg-info/dependency_links.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2019-12-20 20:45:43.000000 webargs-8.2.0/src/webargs.egg-info/not-zip-safe
--rw-r--r--   0 jerome    (1000) jerome    (1000)      836 2022-07-12 13:20:39.000000 webargs-8.2.0/src/webargs.egg-info/requires.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        8 2022-07-12 13:20:39.000000 webargs-8.2.0/src/webargs.egg-info/top_level.txt
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:39.942415 webargs-8.2.0/tests/
--rwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2020-01-25 15:51:49.000000 webargs-8.2.0/tests/__init__.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.370421 webargs-8.2.0/tests/__pycache__/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      136 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      136 2018-01-15 21:51:08.000000 webargs-8.2.0/tests/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      140 2020-01-25 15:53:30.000000 webargs-8.2.0/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      144 2022-01-02 11:08:24.000000 webargs-8.2.0/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    11167 2017-02-19 13:00:02.000000 webargs-8.2.0/tests/__pycache__/common.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    11077 2018-03-07 22:47:55.000000 webargs-8.2.0/tests/__pycache__/common.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      332 2019-02-01 19:40:01.000000 webargs-8.2.0/tests/__pycache__/conftest.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      321 2020-01-25 15:17:58.000000 webargs-8.2.0/tests/__pycache__/conftest.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      325 2022-01-02 11:08:24.000000 webargs-8.2.0/tests/__pycache__/conftest.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5278 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/__pycache__/test_aiohttpparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8159 2018-10-13 18:43:59.000000 webargs-8.2.0/tests/__pycache__/test_aiohttpparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     9031 2021-03-12 22:44:11.000000 webargs-8.2.0/tests/__pycache__/test_aiohttpparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8047 2022-01-02 11:08:24.000000 webargs-8.2.0/tests/__pycache__/test_aiohttpparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3992 2018-10-13 18:44:00.000000 webargs-8.2.0/tests/__pycache__/test_aiohttpparser_async_functions.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3556 2020-01-25 16:02:37.000000 webargs-8.2.0/tests/__pycache__/test_aiohttpparser_async_functions.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      985 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/__pycache__/test_bottleparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      994 2018-10-13 18:44:00.000000 webargs-8.2.0/tests/__pycache__/test_bottleparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      955 2020-01-25 15:17:58.000000 webargs-8.2.0/tests/__pycache__/test_bottleparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      973 2022-01-02 11:08:25.000000 webargs-8.2.0/tests/__pycache__/test_bottleparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    82844 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/__pycache__/test_core.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    80867 2019-02-01 19:40:02.000000 webargs-8.2.0/tests/__pycache__/test_core.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    70386 2021-03-12 22:44:12.000000 webargs-8.2.0/tests/__pycache__/test_core.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    67321 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/__pycache__/test_core.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4823 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/__pycache__/test_djangoparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4480 2018-10-13 18:44:00.000000 webargs-8.2.0/tests/__pycache__/test_djangoparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3677 2021-03-12 22:44:12.000000 webargs-8.2.0/tests/__pycache__/test_djangoparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3464 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/__pycache__/test_djangoparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2626 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/__pycache__/test_falconparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2957 2019-02-01 19:40:03.000000 webargs-8.2.0/tests/__pycache__/test_falconparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7526 2021-03-12 22:44:13.000000 webargs-8.2.0/tests/__pycache__/test_falconparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6472 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/__pycache__/test_falconparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    11779 2017-02-19 13:00:02.000000 webargs-8.2.0/tests/__pycache__/test_flaskparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    11725 2019-02-01 19:40:04.000000 webargs-8.2.0/tests/__pycache__/test_flaskparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    11298 2021-03-12 22:44:14.000000 webargs-8.2.0/tests/__pycache__/test_flaskparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    10207 2022-01-02 11:08:27.000000 webargs-8.2.0/tests/__pycache__/test_flaskparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2606 2017-02-19 13:00:02.000000 webargs-8.2.0/tests/__pycache__/test_pyramidparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2412 2018-10-13 18:44:02.000000 webargs-8.2.0/tests/__pycache__/test_pyramidparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2146 2021-03-12 22:44:14.000000 webargs-8.2.0/tests/__pycache__/test_pyramidparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1892 2022-01-02 11:08:27.000000 webargs-8.2.0/tests/__pycache__/test_pyramidparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    48403 2017-02-19 13:00:02.000000 webargs-8.2.0/tests/__pycache__/test_tornadoparser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    47742 2019-02-01 19:40:04.000000 webargs-8.2.0/tests/__pycache__/test_tornadoparser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    34353 2021-03-12 22:44:14.000000 webargs-8.2.0/tests/__pycache__/test_tornadoparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    30687 2022-01-02 11:08:28.000000 webargs-8.2.0/tests/__pycache__/test_tornadoparser.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    14332 2017-02-19 13:00:02.000000 webargs-8.2.0/tests/__pycache__/test_webapp2parser.cpython-34-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    14458 2019-02-01 19:40:04.000000 webargs-8.2.0/tests/__pycache__/test_webapp2parser.cpython-35-PYTEST.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)    13934 2020-01-31 21:17:26.000000 webargs-8.2.0/tests/__pycache__/test_webapp2parser.cpython-37-pytest-5.3.2.pyc
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.398422 webargs-8.2.0/tests/apps/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2017-02-19 12:58:09.000000 webargs-8.2.0/tests/apps/__init__.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.746427 webargs-8.2.0/tests/apps/__pycache__/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      141 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/apps/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      141 2018-01-15 21:51:08.000000 webargs-8.2.0/tests/apps/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      145 2020-01-25 15:17:58.000000 webargs-8.2.0/tests/apps/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      149 2022-01-02 11:08:25.000000 webargs-8.2.0/tests/apps/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7843 2019-02-01 19:40:04.000000 webargs-8.2.0/tests/apps/__pycache__/aiohttp_app.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8057 2021-03-12 22:44:11.000000 webargs-8.2.0/tests/apps/__pycache__/aiohttp_app.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7814 2022-01-02 11:08:25.000000 webargs-8.2.0/tests/apps/__pycache__/aiohttp_app.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5342 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/apps/__pycache__/bottle_app.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5061 2019-02-01 19:40:01.000000 webargs-8.2.0/tests/apps/__pycache__/bottle_app.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5468 2021-03-12 22:44:12.000000 webargs-8.2.0/tests/apps/__pycache__/bottle_app.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5493 2022-01-02 11:08:25.000000 webargs-8.2.0/tests/apps/__pycache__/bottle_app.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8350 2019-02-01 19:40:03.000000 webargs-8.2.0/tests/apps/__pycache__/falcon_app.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     9941 2021-03-12 22:44:14.000000 webargs-8.2.0/tests/apps/__pycache__/falcon_app.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     9483 2022-01-02 11:08:27.000000 webargs-8.2.0/tests/apps/__pycache__/falcon_app.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7503 2019-02-01 19:40:04.000000 webargs-8.2.0/tests/apps/__pycache__/flask_app.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7775 2021-03-12 22:44:14.000000 webargs-8.2.0/tests/apps/__pycache__/flask_app.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7796 2022-01-02 11:08:27.000000 webargs-8.2.0/tests/apps/__pycache__/flask_app.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5819 2018-12-30 20:42:55.000000 webargs-8.2.0/tests/apps/__pycache__/pyramid_app.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7035 2021-03-12 22:44:19.000000 webargs-8.2.0/tests/apps/__pycache__/pyramid_app.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6909 2022-01-02 11:08:34.000000 webargs-8.2.0/tests/apps/__pycache__/pyramid_app.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7366 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/apps/aiohttp_app.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3999 2021-03-12 22:42:08.000000 webargs-8.2.0/tests/apps/bottle_app.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.758427 webargs-8.2.0/tests/apps/django_app/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      136 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/apps/django_app/__init__.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.762427 webargs-8.2.0/tests/apps/django_app/__pycache__/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      152 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/apps/django_app/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      152 2018-01-15 21:51:09.000000 webargs-8.2.0/tests/apps/django_app/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      156 2020-01-25 15:18:00.000000 webargs-8.2.0/tests/apps/django_app/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      160 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/apps/django_app/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.762427 webargs-8.2.0/tests/apps/django_app/base/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2017-02-19 12:58:09.000000 webargs-8.2.0/tests/apps/django_app/base/__init__.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.798428 webargs-8.2.0/tests/apps/django_app/base/__pycache__/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      157 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/__init__.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      157 2018-01-15 21:51:09.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      161 2020-01-25 15:18:00.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      165 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      962 2018-10-13 18:44:01.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/settings.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      898 2020-01-25 15:53:31.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      902 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1244 2018-12-30 20:42:55.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/urls.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1459 2020-01-25 15:53:33.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/urls.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1470 2022-01-02 11:08:34.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      598 2017-02-19 13:00:01.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/wsgi.cpython-34.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      598 2018-10-13 18:44:00.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/wsgi.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      584 2020-01-25 15:18:00.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/wsgi.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      588 2022-01-02 11:08:26.000000 webargs-8.2.0/tests/apps/django_app/base/__pycache__/wsgi.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      827 2020-01-25 15:51:49.000000 webargs-8.2.0/tests/apps/django_app/base/settings.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1693 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/apps/django_app/base/urls.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      419 2018-10-04 19:36:56.000000 webargs-8.2.0/tests/apps/django_app/base/wsgi.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.798428 webargs-8.2.0/tests/apps/django_app/echo/
--rw-r--r--   0 jerome    (1000) jerome    (1000)        0 2017-02-19 12:58:09.000000 webargs-8.2.0/tests/apps/django_app/echo/__init__.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.834428 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      157 2018-01-21 22:24:55.000000 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      161 2020-01-25 15:18:03.000000 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      165 2022-01-02 11:08:34.000000 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5615 2018-12-30 20:53:49.000000 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/views.cpython-35.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6681 2021-03-12 22:44:18.000000 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/views.cpython-37.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6629 2022-01-02 11:08:34.000000 webargs-8.2.0/tests/apps/django_app/echo/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5762 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/apps/django_app/echo/views.py
--rwxr-xr-x   0 jerome    (1000) jerome    (1000)      250 2018-10-04 19:36:56.000000 webargs-8.2.0/tests/apps/django_app/manage.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     6331 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/apps/falcon_app.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7908 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/apps/flask_app.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     5841 2021-03-12 22:42:08.000000 webargs-8.2.0/tests/apps/pyramid_app.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)       65 2019-02-01 19:39:33.000000 webargs-8.2.0/tests/conftest.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     4049 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/test_aiohttpparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)      341 2018-10-04 19:36:56.000000 webargs-8.2.0/tests/test_bottleparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)    48360 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/test_core.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1644 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/test_djangoparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3426 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/test_falconparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     8942 2022-07-12 13:19:34.000000 webargs-8.2.0/tests/test_flaskparser.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:39.894414 webargs-8.2.0/tests/test_py3/
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2022-07-12 13:20:40.850428 webargs-8.2.0/tests/test_py3/__pycache__/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     7474 2020-01-31 21:17:27.000000 webargs-8.2.0/tests/test_py3/__pycache__/test_aiohttpparser.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3565 2020-01-31 22:40:49.000000 webargs-8.2.0/tests/test_py3/__pycache__/test_aiohttpparser_async_functions.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 jerome    (1000) jerome    (1000)      443 2020-02-29 09:47:53.000000 webargs-8.2.0/tests/test_pyramidparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)    18010 2021-03-12 22:42:08.000000 webargs-8.2.0/tests/test_tornadoparser.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1906 2022-07-12 13:19:34.000000 webargs-8.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.821781 webargs-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-10 14:47:37.000000 webargs-8.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-07-10 14:47:37.000000 webargs-8.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-10 14:47:37.000000 webargs-8.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 14:47:37.000000 webargs-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 14:47:37.000000 webargs-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-10 14:47:47.821781 webargs-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-10 14:47:37.000000 webargs-8.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 14:47:37.000000 webargs-8.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 14:47:47.825781 webargs-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-10 14:47:37.000000 webargs-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.805780 webargs-8.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.813780 webargs-8.3.0/src/webargs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/aiohttpparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/asyncparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/bottleparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32551 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/djangoparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/falconparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/flaskparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/multidictproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/pyramidparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-10 14:47:37.000000 webargs-8.3.0/src/webargs/tornadoparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.813780 webargs-8.3.0/src/webargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-07-10 14:47:47.000000 webargs-8.3.0/src/webargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-10 14:47:47.000000 webargs-8.3.0/src/webargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:47:47.000000 webargs-8.3.0/src/webargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:47:47.000000 webargs-8.3.0/src/webargs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 14:47:47.000000 webargs-8.3.0/src/webargs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 14:47:47.000000 webargs-8.3.0/src/webargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.817781 webargs-8.3.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.821781 webargs-8.3.0/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/aiohttp_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/bottle_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.821781 webargs-8.3.0/tests/apps/django_app/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.821781 webargs-8.3.0/tests/apps/django_app/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/base/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/base/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:47.821781 webargs-8.3.0/tests/apps/django_app/echo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/echo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/echo/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/django_app/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/falcon_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/apps/pyramid_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_aiohttpparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_bottleparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54404 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_djangoparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_falconparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_flaskparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_pyramidparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-07-10 14:47:37.000000 webargs-8.3.0/tests/test_tornadoparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-10 14:47:37.000000 webargs-8.3.0/tox.ini
```

### Comparing `webargs-8.2.0/AUTHORS.rst` & `webargs-8.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/CHANGELOG.rst` & `webargs-8.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 Changelog
 ---------
 
+8.3.0 (2023-07-10)
+******************
+
+Features:
+
+* ``webargs.Parser`` now inherits from ``typing.Generic`` and is parametrizable
+  over the type of the request object. Various framework-specific parsers are
+  parametrized over their relevant request object classes.
+
+* ``webargs.Parser`` and its subclasses now support passing arguments as a
+  single keyword argument without expanding the parsed data into its
+  components. For more details, see advanced docs on
+  ``Argument Passing and arg_name``.
+
+Other changes:
+
+* Type annotations have been improved to allow ``Mapping`` for dict-like
+  schemas where previously ``dict`` was used. This makes the type covariant
+  rather than invariant (:issue:`836`).
+
+* Test against Python 3.11 (:pr:`787`).
+
 8.2.0 (2022-07-11)
 ******************
 
 Features:
 
 * A new method, ``webargs.Parser.async_parse``, can be used for async-aware
   parsing from the base parser class. This can handle async location loader
@@ -1106,15 +1128,15 @@
 
     # New API
     from webargs import fields
 
     args = {
         "name": fields.Str(required=True),
         "password": fields.Str(validate=lambda p: len(p) >= 6),
-        "display_per_page": fields.Int(missing=10),
+        "display_per_page": fields.Int(load_default=10),
         "nickname": fields.List(fields.Str()),
         "content_type": fields.Str(load_from="Content-Type"),
         "location": fields.Nested({"city": fields.Str(), "state": fields.Str()}),
         "meta": fields.Dict(),
     }
 
 Features:
```

### Comparing `webargs-8.2.0/CONTRIBUTING.rst` & `webargs-8.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/LICENSE` & `webargs-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/PKG-INFO` & `webargs-8.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: webargs
-Version: 8.2.0
+Version: 8.3.0
 Summary: Declarative parsing and validation of HTTP request objects, with built-in support for popular web frameworks, including Flask, Django, Bottle, Tornado, Pyramid, Falcon, and aiohttp.
 Home-page: https://github.com/marshmallow-code/webargs
 Author: Steven Loria
 Author-email: sloria1@gmail.com
 License: MIT
 Project-URL: Changelog, https://webargs.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://github.com/marshmallow-code/webargs/issues
 Project-URL: Funding, https://opencollective.com/marshmallow
 Project-URL: Tidelift, https://tidelift.com/subscription/pkg/pypi-webargs?utm_source=pypi-marshmallow&utm_medium=pypi
 Keywords: webargs,http,flask,django,bottle,tornado,aiohttp,request,arguments,validation,parameters,rest,api,marshmallow
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Python: >=3.7.2
 Provides-Extra: frameworks
 Provides-Extra: tests
 Provides-Extra: lint
@@ -143,9 +143,7 @@
 - Ecosystem / related packages: https://github.com/marshmallow-code/webargs/wiki/Ecosystem
 
 
 License
 =======
 
 MIT licensed. See the `LICENSE <https://github.com/marshmallow-code/webargs/blob/dev/LICENSE>`_ file for more details.
-
-
```

### Comparing `webargs-8.2.0/README.rst` & `webargs-8.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/setup.py` & `webargs-8.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,23 @@
         "pytest-asyncio",
         "webtest==3.0.0",
         "webtest-aiohttp==2.0.0",
         "pytest-aiohttp>=0.3.0",
     ]
     + FRAMEWORKS,
     "lint": [
-        "mypy==0.961",
-        "flake8==4.0.1",
-        "flake8-bugbear==22.7.1",
-        "pre-commit~=2.4",
+        "mypy==1.4.1",
+        "flake8==6.0.0",
+        "flake8-bugbear==23.6.5",
+        "pre-commit>=2.4,<4.0",
     ],
     "docs": [
-        "Sphinx==5.0.2",
+        "Sphinx==7.0.1",
         "sphinx-issues==3.0.1",
-        "furo==2022.6.21",
+        "furo==2023.5.20",
     ]
     + FRAMEWORKS,
 }
 EXTRAS_REQUIRE["dev"] = EXTRAS_REQUIRE["tests"] + EXTRAS_REQUIRE["lint"] + ["tox"]
 
 
 def find_version(fname):
@@ -101,14 +101,15 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     ],
     test_suite="tests",
     project_urls={
         "Changelog": "https://webargs.readthedocs.io/en/latest/changelog.html",
```

### Comparing `webargs-8.2.0/src/webargs/__init__.py` & `webargs-8.3.0/src/webargs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Make marshmallow's validation functions importable from webargs
 from marshmallow import validate
 
 from webargs.core import ValidationError
 from webargs import fields
 
-__version__ = "8.2.0"
+__version__ = "8.3.0"
 __parsed_version__ = Version(__version__)
 __version_info__: tuple[int, int, int] | tuple[
     int, int, int, str, int
 ] = __parsed_version__.release  # type: ignore[assignment]
 if __parsed_version__.pre:
     __version_info__ += __parsed_version__.pre  # type: ignore[assignment]
 __all__ = ("ValidationError", "fields", "missing", "validate")
```

### Comparing `webargs-8.2.0/src/webargs/aiohttpparser.py` & `webargs-8.3.0/src/webargs/aiohttpparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 # Collect all exceptions from aiohttp.web_exceptions
 _find_exceptions()
 del _find_exceptions
 
 
-class AIOHTTPParser(AsyncParser):
+class AIOHTTPParser(AsyncParser[web.Request]):
     """aiohttp request argument parser."""
 
     DEFAULT_UNKNOWN_BY_LOCATION: dict[str, str | None] = {
         "match_info": RAISE,
         "path": RAISE,
         **core.Parser.DEFAULT_UNKNOWN_BY_LOCATION,
     }
```

### Comparing `webargs-8.2.0/src/webargs/asyncparser.py` & `webargs-8.3.0/src/webargs/asyncparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import typing
 
 from webargs import core
 
 
-class AsyncParser(core.Parser):
+class AsyncParser(core.Parser[core.Request]):
     """Asynchronous variant of `webargs.core.Parser`.
 
     The ``parse`` method is redefined to be ``async``.
     """
 
     async def parse(
         self,
@@ -18,15 +18,15 @@
         req: core.Request | None = None,
         *,
         location: str | None = None,
         unknown: str | None = core._UNKNOWN_DEFAULT_PARAM,
         validate: core.ValidateArg = None,
         error_status_code: int | None = None,
         error_headers: typing.Mapping[str, str] | None = None,
-    ) -> typing.Mapping | None:
+    ) -> typing.Any:
         """Coroutine variant of `webargs.core.Parser`.
 
         Receives the same arguments as `webargs.core.Parser.parse`.
         """
         data = await self.async_parse(
             argmap,
             req,
```

### Comparing `webargs-8.2.0/src/webargs/bottleparser.py` & `webargs-8.3.0/src/webargs/bottleparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 Example: ::
 
     from bottle import route, run
     from marshmallow import fields
     from webargs.bottleparser import use_args
 
     hello_args = {
-        'name': fields.Str(missing='World')
+        'name': fields.Str(load_default='World')
     }
     @route('/', method='GET', apply=use_args(hello_args))
     def index(args):
         return 'Hello ' + args['name']
 
     if __name__ == '__main__':
         run(debug=True)
 """
 import bottle
 
 from webargs import core
 
 
-class BottleParser(core.Parser):
+class BottleParser(core.Parser[bottle.Request]):
     """Bottle.py request argument parser."""
 
     def _handle_invalid_json_error(self, error, req, *args, **kwargs):
         raise bottle.HTTPError(
             status=400, body={"json": ["Invalid JSON body."]}, exception=error
         )
 
     def _raw_load_json(self, req):
         """Read a json payload from the request."""
         try:
             data = req.json
         except AttributeError:
             return core.missing
 
-        # unfortunately, bottle does not distinguish between an emtpy body, "",
+        # unfortunately, bottle does not distinguish between an empty body, "",
         # and a body containing the valid JSON value null, "null"
         # so these can't be properly disambiguated
         # as our best-effort solution, treat None as missing and ignore the
         # (admittedly unusual) "null" case
         # see: https://github.com/bottlepy/bottle/issues/1160
         if data is None:
             return core.missing
```

### Comparing `webargs-8.2.0/src/webargs/core.py` & `webargs-8.3.0/src/webargs/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import functools
-import typing
-import logging
 import json
+import logging
+import typing
 
 import marshmallow as ma
 from marshmallow import ValidationError
 from marshmallow.utils import missing
 
 from webargs.multidictproxy import MultiDictProxy
 
@@ -22,39 +22,51 @@
     "parse_json",
 ]
 
 
 Request = typing.TypeVar("Request")
 ArgMap = typing.Union[
     ma.Schema,
-    typing.Dict[str, typing.Union[ma.fields.Field, typing.Type[ma.fields.Field]]],
+    typing.Type[ma.Schema],
+    typing.Mapping[str, typing.Union[ma.fields.Field, typing.Type[ma.fields.Field]]],
     typing.Callable[[Request], ma.Schema],
 ]
+
 ValidateArg = typing.Union[None, typing.Callable, typing.Iterable[typing.Callable]]
 CallableList = typing.List[typing.Callable]
 ErrorHandler = typing.Callable[..., typing.NoReturn]
 # generic type var with no particular meaning
 T = typing.TypeVar("T")
 # type var for callables, to make type-preserving decorators
 C = typing.TypeVar("C", bound=typing.Callable)
+# type var for multidict proxy classes
+MultiDictProxyT = typing.TypeVar("MultiDictProxyT", bound=MultiDictProxy)
 # type var for a callable which is an error handler
 # used to ensure that the error_handler decorator is type preserving
 ErrorHandlerT = typing.TypeVar("ErrorHandlerT", bound=ErrorHandler)
 
 AsyncErrorHandler = typing.Callable[..., typing.Awaitable[typing.NoReturn]]
 
 
 # a value used as the default for arguments, so that when `None` is passed, it
 # can be distinguished from the default value
 _UNKNOWN_DEFAULT_PARAM = "_default"
 
 DEFAULT_VALIDATION_STATUS: int = 422
 
 
-def _iscallable(x) -> bool:
+def _record_arg_name(f: typing.Callable[..., typing.Any], argname: str | None) -> None:
+    if argname is None:
+        return
+    if not hasattr(f, "__webargs_argnames__"):
+        f.__webargs_argnames__ = ()  # type: ignore[attr-defined]
+    f.__webargs_argnames__ += (argname,)  # type: ignore[attr-defined]
+
+
+def _iscallable(x: typing.Any) -> bool:
     # workaround for
     #   https://github.com/python/mypy/issues/9778
     return callable(x)
 
 
 def _callable_or_raise(obj: T | None) -> T | None:
     """Makes sure an object is callable if it is not ``None``. If not
@@ -111,26 +123,26 @@
         else:
             raise ValueError(f"{obj!r} is not a callable or list of callables.")
     else:
         validators = []
     return validators
 
 
-class Parser:
+class Parser(typing.Generic[Request]):
     """Base parser class that provides high-level implementation for parsing
     a request.
 
     Descendant classes must provide lower-level implementations for reading
     data from  different locations, e.g. ``load_json``, ``load_querystring``,
     etc.
 
     :param str location: Default location to use for data
     :param str unknown: A default value to pass for ``unknown`` when calling the
-        schema's ``load`` method. Defaults to EXCLUDE for non-body
-        locations and RAISE for request bodies. Pass ``None`` to use the
+        schema's ``load`` method. Defaults to ``marshmallow.EXCLUDE`` for non-body
+        locations and ``marshmallow.RAISE`` for request bodies. Pass ``None`` to use the
         schema's setting instead.
     :param callable error_handler: Custom error handler function.
     """
 
     #: Default location to check for data
     DEFAULT_LOCATION: str = "json"
     #: Default value to use for 'unknown' on schema load
@@ -149,14 +161,17 @@
     DEFAULT_SCHEMA_CLASS: type[ma.Schema] = ma.Schema
     #: Default status code to return for validation errors
     DEFAULT_VALIDATION_STATUS: int = DEFAULT_VALIDATION_STATUS
     #: Default error message for validation errors
     DEFAULT_VALIDATION_MESSAGE: str = "Invalid value."
     #: field types which should always be treated as if they set `is_multiple=True`
     KNOWN_MULTI_FIELDS: list[type] = [ma.fields.List, ma.fields.Tuple]
+    #: set use_args to use a positional argument (rather than a keyword argument)
+    #  defaults to True, but will become False in a future major version
+    USE_ARGS_POSITIONAL: bool = True
 
     #: Maps location => method name
     __location_map__: dict[str, str | typing.Callable] = {
         "json": "load_json",
         "querystring": "load_querystring",
         "query": "load_querystring",
         "form": "load_form",
@@ -169,21 +184,27 @@
     def __init__(
         self,
         location: str | None = None,
         *,
         unknown: str | None = _UNKNOWN_DEFAULT_PARAM,
         error_handler: ErrorHandler | None = None,
         schema_class: type[ma.Schema] | None = None,
-    ):
+    ) -> None:
         self.location = location or self.DEFAULT_LOCATION
         self.error_callback: ErrorHandler | None = _callable_or_raise(error_handler)
         self.schema_class = schema_class or self.DEFAULT_SCHEMA_CLASS
         self.unknown = unknown
 
-    def _makeproxy(self, multidict, schema: ma.Schema, cls: type = MultiDictProxy):
+    def _makeproxy(
+        self,
+        multidict: typing.Any,
+        schema: ma.Schema,
+        *,
+        cls: type[MultiDictProxyT] | type[MultiDictProxy] = MultiDictProxy,
+    ) -> MultiDictProxyT | MultiDictProxy:
         """Create a multidict proxy object with options from the current parser"""
         return cls(multidict, schema, known_multi_fields=tuple(self.KNOWN_MULTI_FIELDS))
 
     def _get_loader(self, location: str) -> typing.Callable:
         """Get the loader function for the given location.
 
         :raises: ValueError if a given location is invalid.
@@ -206,15 +227,17 @@
 
         Needs to have the schema in hand in order to correctly handle loading
         lists from multidict objects and `many=True` schemas.
         """
         loader_func = self._get_loader(location)
         return loader_func(req, schema)
 
-    async def _async_load_location_data(self, schema, req, location):
+    async def _async_load_location_data(
+        self, schema: ma.Schema, req: Request, location: str
+    ) -> typing.Any:
         # an async variant of the _load_location_data method
         # the loader function itself may or may not be async
         loader_func = self._get_loader(location)
         if asyncio.iscoroutinefunction(loader_func):
             data = await loader_func(req, schema)
         else:
             data = loader_func(req, schema)
@@ -298,15 +321,17 @@
         """
         if isinstance(argmap, ma.Schema):
             schema = argmap
         elif isinstance(argmap, type) and issubclass(argmap, ma.Schema):
             schema = argmap()
         elif callable(argmap):
             schema = argmap(req)
-        elif isinstance(argmap, dict):
+        elif isinstance(argmap, typing.Mapping):
+            if not isinstance(argmap, dict):
+                argmap = dict(argmap)
             schema = self.schema_class.from_dict(argmap)()
         else:
             raise TypeError(f"argmap was of unexpected type {type(argmap)}")
         return schema
 
     def _prepare_for_parse(
         self,
@@ -330,15 +355,15 @@
         self,
         location_data: typing.Any,
         schema: ma.Schema,
         req: Request,
         location: str,
         unknown: str | None,
         validators: CallableList,
-    ):
+    ) -> typing.Any:
         # after the data has been fetched from a registered location,
         # this is how it is processed
         # (shared between sync and async variants)
 
         # when the desired location is empty (no data), provide an empty
         # dict as the default so that optional arguments in a location
         # (e.g. optional JSON body) work smoothly
@@ -369,29 +394,29 @@
         req: Request | None = None,
         *,
         location: str | None = None,
         unknown: str | None = _UNKNOWN_DEFAULT_PARAM,
         validate: ValidateArg = None,
         error_status_code: int | None = None,
         error_headers: typing.Mapping[str, str] | None = None,
-    ):
+    ) -> typing.Any:
         """Main request parsing method.
 
         :param argmap: Either a `marshmallow.Schema`, a `dict`
             of argname -> `marshmallow.fields.Field` pairs, or a callable
             which accepts a request and returns a `marshmallow.Schema`.
         :param req: The request object to parse.
         :param str location: Where on the request to load values.
             Can be any of the values in :py:attr:`~__location_map__`. By
             default, that means one of ``('json', 'query', 'querystring',
             'form', 'headers', 'cookies', 'files', 'json_or_form')``.
         :param str unknown: A value to pass for ``unknown`` when calling the
-            schema's ``load`` method. Defaults to EXCLUDE for non-body
-            locations and RAISE for request bodies. Pass ``None`` to use the
-            schema's setting instead.
+            schema's ``load`` method. Defaults to ``marshmallow.EXCLUDE`` for non-body
+            locations and ``marshmallow.RAISE`` for request bodies. Pass ``None`` to use
+            the schema's setting instead.
         :param callable validate: Validation function or list of validation functions
             that receives the dictionary of parsed arguments. Validator either returns a
             boolean or raises a :exc:`ValidationError`.
         :param int error_status_code: Status code passed to error handler functions when
             a `ValidationError` is raised.
         :param dict error_headers: Headers passed to error handler functions when a
             a `ValidationError` is raised.
@@ -428,15 +453,15 @@
         req: Request | None = None,
         *,
         location: str | None = None,
         unknown: str | None = _UNKNOWN_DEFAULT_PARAM,
         validate: ValidateArg = None,
         error_status_code: int | None = None,
         error_headers: typing.Mapping[str, str] | None = None,
-    ) -> typing.Mapping | None:
+    ) -> typing.Any:
         """Coroutine variant of `webargs.core.Parser.parse`.
 
         Receives the same arguments as `webargs.core.Parser.parse`.
         """
         data, req, location, validators, schema = self._prepare_for_parse(
             argmap, req, location, unknown, validate
         )
@@ -486,75 +511,105 @@
         """
         return None
 
     @staticmethod
     def _update_args_kwargs(
         args: tuple,
         kwargs: dict[str, typing.Any],
-        parsed_args: tuple,
+        parsed_args: dict[str, typing.Any],
         as_kwargs: bool,
-    ) -> tuple[tuple, typing.Mapping]:
+        arg_name: str | None,
+    ) -> tuple[tuple, dict[str, typing.Any]]:
         """Update args or kwargs with parsed_args depending on as_kwargs"""
         if as_kwargs:
+            # expand parsed_args into kwargs
             kwargs.update(parsed_args)
         else:
-            # Add parsed_args after other positional arguments
-            args += (parsed_args,)
+            if arg_name:
+                # add parsed_args as a specific kwarg
+                kwargs[arg_name] = parsed_args
+            else:
+                # Add parsed_args after other positional arguments
+                args += (parsed_args,)
         return args, kwargs
 
     def use_args(
         self,
         argmap: ArgMap,
         req: Request | None = None,
         *,
         location: str | None = None,
         unknown: str | None = _UNKNOWN_DEFAULT_PARAM,
         as_kwargs: bool = False,
+        arg_name: str | None = None,
         validate: ValidateArg = None,
         error_status_code: int | None = None,
         error_headers: typing.Mapping[str, str] | None = None,
     ) -> typing.Callable[..., typing.Callable]:
         """Decorator that injects parsed arguments into a view function or method.
 
         Example usage with Flask: ::
 
             @app.route('/echo', methods=['get', 'post'])
             @parser.use_args({'name': fields.Str()}, location="querystring")
-            def greet(args):
-                return 'Hello ' + args['name']
+            def greet(querystring_args):
+                return 'Hello ' + querystring_args['name']
 
         :param argmap: Either a `marshmallow.Schema`, a `dict`
             of argname -> `marshmallow.fields.Field` pairs, or a callable
             which accepts a request and returns a `marshmallow.Schema`.
         :param str location: Where on the request to load values.
         :param str unknown: A value to pass for ``unknown`` when calling the
             schema's ``load`` method.
         :param bool as_kwargs: Whether to insert arguments as keyword arguments.
+        :param str arg_name: Keyword argument name to use for arguments. Mutually
+            exclusive with as_kwargs.
         :param callable validate: Validation function that receives the dictionary
             of parsed arguments. If the function returns ``False``, the parser
             will raise a :exc:`ValidationError`.
         :param int error_status_code: Status code passed to error handler functions when
             a `ValidationError` is raised.
         :param dict error_headers: Headers passed to error handler functions when a
             a `ValidationError` is raised.
         """
         location = location or self.location
         request_obj = req
+
+        if arg_name is not None and as_kwargs:
+            raise ValueError("arg_name and as_kwargs are mutually exclusive")
+        if arg_name is None and not self.USE_ARGS_POSITIONAL:
+            arg_name = f"{location}_args"
+
         # Optimization: If argmap is passed as a dictionary, we only need
         # to generate a Schema once
-        if isinstance(argmap, dict):
+        if isinstance(argmap, typing.Mapping):
+            if not isinstance(argmap, dict):
+                argmap = dict(argmap)
             argmap = self.schema_class.from_dict(argmap)()
 
         def decorator(func: typing.Callable) -> typing.Callable:
             req_ = request_obj
 
+            # check at decoration time that a unique name is being used
+            # (no arg_name conflicts)
+            if arg_name is not None and not as_kwargs:
+                existing_arg_names = getattr(func, "__webargs_argnames__", ())
+                if arg_name in existing_arg_names:
+                    raise ValueError(
+                        f"Attempted to pass `arg_name='{arg_name}'` via use_args() but "
+                        "that name was already used. If this came from stacked webargs "
+                        "decorators, try setting `arg_name` to distinguish usages."
+                    )
+
             if asyncio.iscoroutinefunction(func):
 
                 @functools.wraps(func)
-                async def wrapper(*args, **kwargs):
+                async def wrapper(
+                    *args: typing.Any, **kwargs: typing.Any
+                ) -> typing.Any:
                     req_obj = req_
 
                     if not req_obj:
                         req_obj = self.get_request_from_view_args(func, args, kwargs)
                     # NOTE: At this point, argmap may be a Schema, callable, or dict
                     parsed_args = await self.async_parse(
                         argmap,
@@ -562,22 +617,22 @@
                         location=location,
                         unknown=unknown,
                         validate=validate,
                         error_status_code=error_status_code,
                         error_headers=error_headers,
                     )
                     args, kwargs = self._update_args_kwargs(
-                        args, kwargs, parsed_args, as_kwargs
+                        args, kwargs, parsed_args, as_kwargs, arg_name
                     )
                     return await func(*args, **kwargs)
 
             else:
 
-                @functools.wraps(func)  # type: ignore
-                def wrapper(*args, **kwargs):
+                @functools.wraps(func)
+                def wrapper(*args: typing.Any, **kwargs: typing.Any) -> typing.Any:
                     req_obj = req_
 
                     if not req_obj:
                         req_obj = self.get_request_from_view_args(func, args, kwargs)
                     # NOTE: At this point, argmap may be a Schema, callable, or dict
                     parsed_args = self.parse(
                         argmap,
@@ -585,40 +640,59 @@
                         location=location,
                         unknown=unknown,
                         validate=validate,
                         error_status_code=error_status_code,
                         error_headers=error_headers,
                     )
                     args, kwargs = self._update_args_kwargs(
-                        args, kwargs, parsed_args, as_kwargs
+                        args, kwargs, parsed_args, as_kwargs, arg_name
                     )
                     return func(*args, **kwargs)
 
             wrapper.__wrapped__ = func  # type: ignore
+            _record_arg_name(wrapper, arg_name)
             return wrapper
 
         return decorator
 
-    def use_kwargs(self, *args, **kwargs) -> typing.Callable:
+    def use_kwargs(
+        self,
+        argmap: ArgMap,
+        req: Request | None = None,
+        *,
+        location: str | None = None,
+        unknown: str | None = _UNKNOWN_DEFAULT_PARAM,
+        validate: ValidateArg = None,
+        error_status_code: int | None = None,
+        error_headers: typing.Mapping[str, str] | None = None,
+    ) -> typing.Callable[..., typing.Callable]:
         """Decorator that injects parsed arguments into a view function or method
         as keyword arguments.
 
         This is a shortcut to :meth:`use_args` with ``as_kwargs=True``.
 
         Example usage with Flask: ::
 
             @app.route('/echo', methods=['get', 'post'])
             @parser.use_kwargs({'name': fields.Str()})
             def greet(name):
                 return 'Hello ' + name
 
         Receives the same ``args`` and ``kwargs`` as :meth:`use_args`.
         """
-        kwargs["as_kwargs"] = True
-        return self.use_args(*args, **kwargs)
+        return self.use_args(
+            argmap,
+            req=req,
+            as_kwargs=True,
+            location=location,
+            unknown=unknown,
+            validate=validate,
+            error_status_code=error_status_code,
+            error_headers=error_headers,
+        )
 
     def location_loader(self, name: str) -> typing.Callable[[C], C]:
         """Decorator that registers a function for loading a request location.
         The wrapped function receives a schema and a request.
 
         The schema will usually not be relevant, but it's important in some
         cases -- most notably in order to correctly load multidict values into
@@ -684,16 +758,16 @@
         """
         return location_data
 
     def _handle_invalid_json_error(
         self,
         error: json.JSONDecodeError | UnicodeDecodeError,
         req: Request,
-        *args,
-        **kwargs,
+        *args: typing.Any,
+        **kwargs: typing.Any,
     ) -> typing.NoReturn:
         """Internal hook for overriding treatment of JSONDecodeErrors.
 
         Invoked by default `load_json` implementation.
 
         External parsers can just implement their own behavior for load_json ,
         so this is not part of the public parser API.
@@ -714,29 +788,29 @@
         except json.JSONDecodeError as exc:
             if exc.doc == "":
                 return missing
             return self._handle_invalid_json_error(exc, req)
         except UnicodeDecodeError as exc:
             return self._handle_invalid_json_error(exc, req)
 
-    def load_json_or_form(self, req: Request, schema: ma.Schema):
+    def load_json_or_form(self, req: Request, schema: ma.Schema) -> typing.Any:
         """Load data from a request, accepting either JSON or form-encoded
         data.
 
         The data will first be loaded as JSON, and, if that fails, it will be
         loaded as a form post.
         """
         data = self.load_json(req, schema)
         if data is not missing:
             return data
         return self.load_form(req, schema)
 
     # Abstract Methods
 
-    def _raw_load_json(self, req: Request):
+    def _raw_load_json(self, req: Request) -> typing.Any:
         """Internal hook method for implementing load_json()
 
         Get a request body for feeding in to `load_json`, and parse it either
         using core.parse_json() or similar utilities which raise
         JSONDecodeErrors.
         Ensure consistent behavior when encountering decoding errors.
 
@@ -744,37 +818,37 @@
         implementation of `load_json` above will pass that value through.
         However, by implementing a "mostly concrete" version of load_json with
         this as a hook for getting data, we consolidate the logic for handling
         those JSONDecodeErrors.
         """
         return missing
 
-    def load_querystring(self, req: Request, schema: ma.Schema):
+    def load_querystring(self, req: Request, schema: ma.Schema) -> typing.Any:
         """Load the query string of a request object or return `missing` if no
         value can be found.
         """
         return missing
 
-    def load_form(self, req: Request, schema: ma.Schema):
+    def load_form(self, req: Request, schema: ma.Schema) -> typing.Any:
         """Load the form data of a request object or return `missing` if no
         value can be found.
         """
         return missing
 
-    def load_headers(self, req: Request, schema: ma.Schema):
+    def load_headers(self, req: Request, schema: ma.Schema) -> typing.Any:
         """Load the headers or return `missing` if no value can be found."""
         return missing
 
-    def load_cookies(self, req: Request, schema: ma.Schema):
+    def load_cookies(self, req: Request, schema: ma.Schema) -> typing.Any:
         """Load the cookies from the request or return `missing` if no value
         can be found.
         """
         return missing
 
-    def load_files(self, req: Request, schema: ma.Schema):
+    def load_files(self, req: Request, schema: ma.Schema) -> typing.Any:
         """Load files from the request or return `missing` if no values can be
         found.
         """
         return missing
 
     def handle_error(
         self,
```

### Comparing `webargs-8.2.0/src/webargs/djangoparser.py` & `webargs-8.3.0/src/webargs/djangoparser.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,70 +4,72 @@
 
     from django.views.generic import View
     from django.http import HttpResponse
     from marshmallow import fields
     from webargs.djangoparser import use_args
 
     hello_args = {
-        'name': fields.Str(missing='World')
+        'name': fields.Str(load_default='World')
     }
 
     class MyView(View):
 
         @use_args(hello_args)
         def get(self, args, request):
             return HttpResponse('Hello ' + args['name'])
 """
+import django
+
 from webargs import core
 
 
 def is_json_request(req):
     return core.is_json(req.content_type)
 
 
-class DjangoParser(core.Parser):
+class DjangoParser(core.Parser[django.http.HttpRequest]):
     """Django request argument parser.
 
     .. warning::
 
         :class:`DjangoParser` does not override
         :meth:`handle_error <webargs.core.Parser.handle_error>`, so your Django
         views are responsible for catching any :exc:`ValidationErrors` raised by
         the parser and returning the appropriate `HTTPResponse`.
     """
 
-    def _raw_load_json(self, req):
+    def _raw_load_json(self, req: django.http.HttpRequest):
         """Read a json payload from the request for the core parser's load_json
 
         Checks the input mimetype and may return 'missing' if the mimetype is
         non-json, even if the request body is parseable as json."""
         if not is_json_request(req):
             return core.missing
 
         return core.parse_json(req.body)
 
-    def load_querystring(self, req, schema):
+    def load_querystring(self, req: django.http.HttpRequest, schema):
         """Return query params from the request as a MultiDictProxy."""
         return self._makeproxy(req.GET, schema)
 
-    def load_form(self, req, schema):
+    def load_form(self, req: django.http.HttpRequest, schema):
         """Return form values from the request as a MultiDictProxy."""
         return self._makeproxy(req.POST, schema)
 
-    def load_cookies(self, req, schema):
+    def load_cookies(self, req: django.http.HttpRequest, schema):
         """Return cookies from the request."""
         return req.COOKIES
 
-    def load_headers(self, req, schema):
+    def load_headers(self, req: django.http.HttpRequest, schema):
         """Return headers from the request."""
         # Django's HttpRequest.headers is a case-insensitive dict type, but it
         # isn't a multidict, so this is not proxied
         return req.headers
 
-    def load_files(self, req, schema):
+    def load_files(self, req: django.http.HttpRequest, schema):
         """Return files from the request as a MultiDictProxy."""
         return self._makeproxy(req.FILES, schema)
 
     def get_request_from_view_args(self, view, args, kwargs):
         # The first argument is either `self` or `request`
         try:  # self.request
             return args[0].request
```

### Comparing `webargs-8.2.0/src/webargs/falconparser.py` & `webargs-8.3.0/src/webargs/falconparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Falcon request argument parsing module.
 """
 import falcon
-from falcon.util.uri import parse_query_string
-
 import marshmallow as ma
+from falcon.util.uri import parse_query_string
 
 from webargs import core
 
 HTTP_422 = "422 Unprocessable Entity"
 
 # Mapping of int status codes to string status
 status_map = {422: HTTP_422}
@@ -21,21 +20,21 @@
         status_map[status_code] = status
 
 
 _find_exceptions()
 del _find_exceptions
 
 
-def is_json_request(req):
+def is_json_request(req: falcon.Request):
     content_type = req.get_header("Content-Type")
     return content_type and core.is_json(content_type)
 
 
 # NOTE: Adapted from falcon.request.Request._parse_form_urlencoded
-def parse_form_body(req):
+def parse_form_body(req: falcon.Request):
     if (
         req.content_type is not None
         and "application/x-www-form-urlencoded" in req.content_type
     ):
         body = req.stream.read(req.content_length or 0)
         try:
             body = body.decode("ascii")
@@ -65,15 +64,15 @@
         """Override `falcon.HTTPError` to include error messages in responses."""
         ret = super().to_dict(*args, **kwargs)
         if self.errors is not None:
             ret["errors"] = self.errors
         return ret
 
 
-class FalconParser(core.Parser):
+class FalconParser(core.Parser[falcon.Request]):
     """Falcon request argument parser.
 
     Defaults to using the `media` location. See :py:meth:`~FalconParser.load_media` for
     details on the media location."""
 
     # by default, Falcon will use the 'media' location to load data
     #
@@ -90,31 +89,31 @@
     # Falcon parses query strings and form values into ordinary dicts, but with
     # the values listified where appropriate
     # it is still therefore necessary in these cases to wrap them in
     # MultiDictProxy because we need to use the schema to determine when single
     # values should be wrapped in lists due to the type of the destination
     # field
 
-    def load_querystring(self, req, schema):
+    def load_querystring(self, req: falcon.Request, schema):
         """Return query params from the request as a MultiDictProxy."""
         return self._makeproxy(req.params, schema)
 
-    def load_form(self, req, schema):
+    def load_form(self, req: falcon.Request, schema):
         """Return form values from the request as a MultiDictProxy
 
         .. note::
 
             The request stream will be read and left at EOF.
         """
         form = parse_form_body(req)
         if form is core.missing:
             return form
         return self._makeproxy(form, schema)
 
-    def load_media(self, req, schema):
+    def load_media(self, req: falcon.Request, schema):
         """Return data unpacked and parsed by one of Falcon's media handlers.
         By default, Falcon only handles JSON payloads.
 
         To configure additional media handlers, see the
         `Falcon documentation on media types`__.
 
         .. _FalconMedia: https://falcon.readthedocs.io/en/stable/api/media.html
@@ -125,32 +124,32 @@
             The request stream will be read and left at EOF.
         """
         # if there is no body, return missing instead of erroring
         if req.content_length in (None, 0):
             return core.missing
         return req.media
 
-    def _raw_load_json(self, req):
+    def _raw_load_json(self, req: falcon.Request):
         """Return a json payload from the request for the core parser's load_json
 
         Checks the input mimetype and may return 'missing' if the mimetype is
         non-json, even if the request body is parseable as json."""
         if not is_json_request(req) or req.content_length in (None, 0):
             return core.missing
         body = req.stream.read(req.content_length)
         if body:
             return core.parse_json(body)
         return core.missing
 
-    def load_headers(self, req, schema):
+    def load_headers(self, req: falcon.Request, schema):
         """Return headers from the request."""
         # Falcon only exposes headers as a dict (not multidict)
         return req.headers
 
-    def load_cookies(self, req, schema):
+    def load_cookies(self, req: falcon.Request, schema):
         """Return cookies from the request."""
         # Cookies are expressed in Falcon as a dict, but the possibility of
         # multiple values for a cookie is preserved internally -- if desired in
         # the future, webargs could add a MultiDict type for Cookies here built
         # from (req, schema), but Falcon does not provide one out of the box
         return req.cookies
 
@@ -159,27 +158,29 @@
         request is the second argument.
         """
         req = args[1]
         if not isinstance(req, falcon.Request):
             raise TypeError("Argument is not a falcon.Request")
         return req
 
-    def load_files(self, req, schema):
+    def load_files(self, req: falcon.Request, schema):
         raise NotImplementedError(
             f"Parsing files not yet supported by {self.__class__.__name__}"
         )
 
-    def handle_error(self, error, req, schema, *, error_status_code, error_headers):
+    def handle_error(
+        self, error, req: falcon.Request, schema, *, error_status_code, error_headers
+    ):
         """Handles errors during parsing."""
         status = status_map.get(error_status_code or self.DEFAULT_VALIDATION_STATUS)
         if status is None:
             raise LookupError(f"Status code {error_status_code} not supported")
         raise HTTPError(status, errors=error.messages, headers=error_headers)
 
-    def _handle_invalid_json_error(self, error, req, *args, **kwargs):
+    def _handle_invalid_json_error(self, error, req: falcon.Request, *args, **kwargs):
         status = status_map[400]
         messages = {"json": ["Invalid JSON body."]}
         raise HTTPError(status, errors=messages)
 
 
 parser = FalconParser()
 use_args = parser.use_args
```

### Comparing `webargs-8.2.0/src/webargs/fields.py` & `webargs-8.3.0/src/webargs/fields.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/src/webargs/flaskparser.py` & `webargs-8.3.0/src/webargs/flaskparser.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     @use_args(user_detail_args)
     def user_detail(args, uid):
         return ("The user page for user {uid}, showing {per_page} posts.").format(
             uid=uid, per_page=args["per_page"]
         )
 """
 from __future__ import annotations
+
 from typing import NoReturn
 
 import flask
-from werkzeug.exceptions import HTTPException
-
 import marshmallow as ma
+from werkzeug.exceptions import HTTPException
 
 from webargs import core
 
 
 def abort(http_status_code, exc=None, **kwargs) -> NoReturn:
     """Raise a HTTPException for the given http_status_code. Attach any keyword
     arguments to the exception for later processing.
@@ -41,83 +41,85 @@
         flask.abort(http_status_code)
     except HTTPException as err:
         err.data = kwargs  # type: ignore
         err.exc = exc  # type: ignore
         raise err
 
 
-def is_json_request(req):
+def is_json_request(req: flask.Request):
     return core.is_json(req.mimetype)
 
 
-class FlaskParser(core.Parser):
+class FlaskParser(core.Parser[flask.Request]):
     """Flask request argument parser."""
 
     DEFAULT_UNKNOWN_BY_LOCATION: dict[str, str | None] = {
         "view_args": ma.RAISE,
         "path": ma.RAISE,
         **core.Parser.DEFAULT_UNKNOWN_BY_LOCATION,
     }
     __location_map__ = dict(
         view_args="load_view_args",
         path="load_view_args",
         **core.Parser.__location_map__,
     )
 
-    def _raw_load_json(self, req):
+    def _raw_load_json(self, req: flask.Request):
         """Return a json payload from the request for the core parser's load_json
 
         Checks the input mimetype and may return 'missing' if the mimetype is
         non-json, even if the request body is parseable as json."""
         if not is_json_request(req):
             return core.missing
 
         return core.parse_json(req.get_data(cache=True))
 
-    def _handle_invalid_json_error(self, error, req, *args, **kwargs):
+    def _handle_invalid_json_error(self, error, req: flask.Request, *args, **kwargs):
         abort(400, exc=error, messages={"json": ["Invalid JSON body."]})
 
-    def load_view_args(self, req, schema):
+    def load_view_args(self, req: flask.Request, schema):
         """Return the request's ``view_args`` or ``missing`` if there are none."""
         return req.view_args or core.missing
 
-    def load_querystring(self, req, schema):
+    def load_querystring(self, req: flask.Request, schema):
         """Return query params from the request as a MultiDictProxy."""
         return self._makeproxy(req.args, schema)
 
-    def load_form(self, req, schema):
+    def load_form(self, req: flask.Request, schema):
         """Return form values from the request as a MultiDictProxy."""
         return self._makeproxy(req.form, schema)
 
-    def load_headers(self, req, schema):
+    def load_headers(self, req: flask.Request, schema):
         """Return headers from the request as a MultiDictProxy."""
         return self._makeproxy(req.headers, schema)
 
-    def load_cookies(self, req, schema):
+    def load_cookies(self, req: flask.Request, schema):
         """Return cookies from the request."""
         return req.cookies
 
-    def load_files(self, req, schema):
+    def load_files(self, req: flask.Request, schema):
         """Return files from the request as a MultiDictProxy."""
         return self._makeproxy(req.files, schema)
 
-    def handle_error(self, error, req, schema, *, error_status_code, error_headers):
+    def handle_error(
+        self, error, req: flask.Request, schema, *, error_status_code, error_headers
+    ):
         """Handles errors during parsing. Aborts the current HTTP request and
         responds with a 422 error.
         """
         status_code = error_status_code or self.DEFAULT_VALIDATION_STATUS
         abort(
             status_code,
             exc=error,
             messages=error.messages,
             schema=schema,
             headers=error_headers,
         )
 
-    def get_default_request(self):
+    def get_default_request(self) -> flask.Request:
         """Override to use Flask's thread-local request object by default"""
         return flask.request
 
 
 parser = FlaskParser()
 use_args = parser.use_args
 use_kwargs = parser.use_kwargs
```

### Comparing `webargs-8.2.0/src/webargs/multidictproxy.py` & `webargs-8.3.0/src/webargs/multidictproxy.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/src/webargs/pyramidparser.py` & `webargs-8.3.0/src/webargs/pyramidparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from wsgiref.simple_server import make_server
     from pyramid.config import Configurator
     from pyramid.response import Response
     from marshmallow import fields
     from webargs.pyramidparser import use_args
 
     hello_args = {
-        'name': fields.Str(missing='World')
+        'name': fields.Str(load_default='World')
     }
 
     @use_args(hello_args)
     def hello_world(request, args):
         return Response('Hello ' + args['name'])
 
     if __name__ == '__main__':
@@ -25,108 +25,111 @@
         server.serve_forever()
 """
 from __future__ import annotations
 
 import functools
 from collections.abc import Mapping
 
-from webob.multidict import MultiDict
-from pyramid.httpexceptions import exception_response
-
 import marshmallow as ma
+from pyramid.httpexceptions import exception_response
+from pyramid.request import Request
+from webob.multidict import MultiDict
 
 from webargs import core
 from webargs.core import json
 
 
-def is_json_request(req):
+def is_json_request(req: Request) -> bool:
     return core.is_json(req.headers.get("content-type"))
 
 
-class PyramidParser(core.Parser):
+class PyramidParser(core.Parser[Request]):
     """Pyramid request argument parser."""
 
     DEFAULT_UNKNOWN_BY_LOCATION: dict[str, str | None] = {
         "matchdict": ma.RAISE,
         "path": ma.RAISE,
         **core.Parser.DEFAULT_UNKNOWN_BY_LOCATION,
     }
     __location_map__ = dict(
         matchdict="load_matchdict",
         path="load_matchdict",
         **core.Parser.__location_map__,
     )
 
-    def _raw_load_json(self, req):
+    def _raw_load_json(self, req: Request):
         """Return a json payload from the request for the core parser's load_json
 
         Checks the input mimetype and may return 'missing' if the mimetype is
         non-json, even if the request body is parseable as json."""
         if not is_json_request(req):
             return core.missing
 
         return core.parse_json(req.body, encoding=req.charset)
 
-    def load_querystring(self, req, schema):
+    def load_querystring(self, req: Request, schema):
         """Return query params from the request as a MultiDictProxy."""
         return self._makeproxy(req.GET, schema)
 
-    def load_form(self, req, schema):
+    def load_form(self, req: Request, schema):
         """Return form values from the request as a MultiDictProxy."""
         return self._makeproxy(req.POST, schema)
 
-    def load_cookies(self, req, schema):
+    def load_cookies(self, req: Request, schema):
         """Return cookies from the request as a MultiDictProxy."""
         return self._makeproxy(req.cookies, schema)
 
-    def load_headers(self, req, schema):
+    def load_headers(self, req: Request, schema):
         """Return headers from the request as a MultiDictProxy."""
         return self._makeproxy(req.headers, schema)
 
-    def load_files(self, req, schema):
+    def load_files(self, req: Request, schema):
         """Return files from the request as a MultiDictProxy."""
         files = ((k, v) for k, v in req.POST.items() if hasattr(v, "file"))
         return self._makeproxy(MultiDict(files), schema)
 
-    def load_matchdict(self, req, schema):
+    def load_matchdict(self, req: Request, schema):
         """Return the request's ``matchdict`` as a MultiDictProxy."""
         return self._makeproxy(req.matchdict, schema)
 
-    def handle_error(self, error, req, schema, *, error_status_code, error_headers):
+    def handle_error(
+        self, error, req: Request, schema, *, error_status_code, error_headers
+    ):
         """Handles errors during parsing. Aborts the current HTTP request and
         responds with a 400 error.
         """
         status_code = error_status_code or self.DEFAULT_VALIDATION_STATUS
         response = exception_response(
             status_code,
             detail=str(error),
             headers=error_headers,
             content_type="application/json",
         )
         body = json.dumps(error.messages)
         response.body = body.encode("utf-8") if isinstance(body, str) else body
         raise response
 
-    def _handle_invalid_json_error(self, error, req, *args, **kwargs):
+    def _handle_invalid_json_error(self, error, req: Request, *args, **kwargs):
         messages = {"json": ["Invalid JSON body."]}
         response = exception_response(
             400, detail=str(messages), content_type="application/json"
         )
         body = json.dumps(messages)
         response.body = body.encode("utf-8") if isinstance(body, str) else body
         raise response
 
     def use_args(
         self,
         argmap,
-        req=None,
+        req: Request | None = None,
         *,
         location=core.Parser.DEFAULT_LOCATION,
         unknown=None,
         as_kwargs=False,
+        arg_name=None,
         validate=None,
         error_status_code=None,
         error_headers=None,
     ):
         """Decorator that injects parsed arguments into a view callable.
         Supports the *Class-based View* pattern where `request` is saved as an instance
         attribute on a view class.
@@ -135,26 +138,36 @@
             of argname -> `marshmallow.fields.Field` pairs, or a callable
             which accepts a request and returns a `marshmallow.Schema`.
         :param req: The request object to parse. Pulled off of the view by default.
         :param str location: Where on the request to load values.
         :param str unknown: A value to pass for ``unknown`` when calling the
             schema's ``load`` method.
         :param bool as_kwargs: Whether to insert arguments as keyword arguments.
+        :param str arg_name: Keyword argument name to use for arguments. Mutually
+            exclusive with as_kwargs.
         :param callable validate: Validation function that receives the dictionary
             of parsed arguments. If the function returns ``False``, the parser
             will raise a :exc:`ValidationError`.
         :param int error_status_code: Status code passed to error handler functions when
             a `ValidationError` is raised.
         :param dict error_headers: Headers passed to error handler functions when a
             a `ValidationError` is raised.
         """
         location = location or self.location
+
+        if arg_name is not None and as_kwargs:
+            raise ValueError("arg_name and as_kwargs are mutually exclusive")
+        if arg_name is None and not self.USE_ARGS_POSITIONAL:
+            arg_name = f"{location}_args"
+
         # Optimization: If argmap is passed as a dictionary, we only need
         # to generate a Schema once
         if isinstance(argmap, Mapping):
+            if not isinstance(argmap, dict):
+                argmap = dict(argmap)
             argmap = self.schema_class.from_dict(argmap)()
 
         def decorator(func):
             @functools.wraps(func)
             def wrapper(obj, *args, **kwargs):
                 # The first argument is either `self` or `request`
                 try:  # get self.request
@@ -168,15 +181,15 @@
                     location=location,
                     unknown=unknown,
                     validate=validate,
                     error_status_code=error_status_code,
                     error_headers=error_headers,
                 )
                 args, kwargs = self._update_args_kwargs(
-                    args, kwargs, parsed_args, as_kwargs
+                    args, kwargs, parsed_args, as_kwargs, arg_name
                 )
                 return func(obj, *args, **kwargs)
 
             wrapper.__wrapped__ = func
             return wrapper
 
         return decorator
```

### Comparing `webargs-8.2.0/src/webargs/testing.py` & `webargs-8.3.0/src/webargs/testing.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/src/webargs/tornadoparser.py` & `webargs-8.3.0/src/webargs/tornadoparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 
     import tornado.web
     from marshmallow import fields
     from webargs.tornadoparser import use_args
 
     class HelloHandler(tornado.web.RequestHandler):
 
-        @use_args({'name': fields.Str(missing='World')})
+        @use_args({'name': fields.Str(load_default='World')})
         def get(self, args):
             response = {'message': 'Hello {}'.format(args['name'])}
             self.write(response)
 """
-import tornado.web
 import tornado.concurrent
+import tornado.web
 from tornado.escape import _unicode
+from tornado.httputil import HTTPServerRequest
 
 from webargs import core
 from webargs.multidictproxy import MultiDictProxy
 
 
 class HTTPError(tornado.web.HTTPError):
     """`tornado.web.HTTPError` that stores validation errors."""
 
     def __init__(self, *args, **kwargs):
         self.messages = kwargs.pop("messages", {})
         self.headers = kwargs.pop("headers", None)
         super().__init__(*args, **kwargs)
 
 
-def is_json_request(req):
+def is_json_request(req: HTTPServerRequest):
     content_type = req.headers.get("Content-Type")
     return content_type is not None and core.is_json(content_type)
 
 
 class WebArgsTornadoMultiDictProxy(MultiDictProxy):
     """
     Override class for Tornado multidicts, handles argument decoding
@@ -73,61 +74,63 @@
         if cookie is core.missing:
             return core.missing
         if key in self.multiple_keys:
             return [cookie.value]
         return cookie.value
 
 
-class TornadoParser(core.Parser):
+class TornadoParser(core.Parser[HTTPServerRequest]):
     """Tornado request argument parser."""
 
-    def _raw_load_json(self, req):
+    def _raw_load_json(self, req: HTTPServerRequest):
         """Return a json payload from the request for the core parser's load_json
 
         Checks the input mimetype and may return 'missing' if the mimetype is
         non-json, even if the request body is parseable as json."""
         if not is_json_request(req):
             return core.missing
 
         # request.body may be a concurrent.Future on streaming requests
         # this would cause a TypeError if we try to parse it
         if isinstance(req.body, tornado.concurrent.Future):
             return core.missing
 
         return core.parse_json(req.body)
 
-    def load_querystring(self, req, schema):
+    def load_querystring(self, req: HTTPServerRequest, schema):
         """Return query params from the request as a MultiDictProxy."""
         return self._makeproxy(
             req.query_arguments, schema, cls=WebArgsTornadoMultiDictProxy
         )
 
-    def load_form(self, req, schema):
+    def load_form(self, req: HTTPServerRequest, schema):
         """Return form values from the request as a MultiDictProxy."""
         return self._makeproxy(
             req.body_arguments, schema, cls=WebArgsTornadoMultiDictProxy
         )
 
-    def load_headers(self, req, schema):
+    def load_headers(self, req: HTTPServerRequest, schema):
         """Return headers from the request as a MultiDictProxy."""
         return self._makeproxy(req.headers, schema, cls=WebArgsTornadoMultiDictProxy)
 
-    def load_cookies(self, req, schema):
+    def load_cookies(self, req: HTTPServerRequest, schema):
         """Return cookies from the request as a MultiDictProxy."""
         # use the specialized subclass specifically for handling Tornado
         # cookies
         return self._makeproxy(
             req.cookies, schema, cls=WebArgsTornadoCookiesMultiDictProxy
         )
 
-    def load_files(self, req, schema):
+    def load_files(self, req: HTTPServerRequest, schema):
         """Return files from the request as a MultiDictProxy."""
         return self._makeproxy(req.files, schema, cls=WebArgsTornadoMultiDictProxy)
 
-    def handle_error(self, error, req, schema, *, error_status_code, error_headers):
+    def handle_error(
+        self, error, req: HTTPServerRequest, schema, *, error_status_code, error_headers
+    ):
         """Handles errors during parsing. Raises a `tornado.web.HTTPError`
         with a 400 error.
         """
         status_code = error_status_code or self.DEFAULT_VALIDATION_STATUS
         if status_code == 422:
             reason = "Unprocessable Entity"
         else:
@@ -136,15 +139,17 @@
             status_code,
             log_message=str(error.messages),
             reason=reason,
             messages=error.messages,
             headers=error_headers,
         )
 
-    def _handle_invalid_json_error(self, error, req, *args, **kwargs):
+    def _handle_invalid_json_error(
+        self, error, req: HTTPServerRequest, *args, **kwargs
+    ):
         raise HTTPError(
             400,
             log_message="Invalid JSON body.",
             reason="Bad Request",
             messages={"json": ["Invalid JSON body."]},
         )
```

### Comparing `webargs-8.2.0/src/webargs.egg-info/PKG-INFO` & `webargs-8.3.0/src/webargs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: webargs
-Version: 8.2.0
+Version: 8.3.0
 Summary: Declarative parsing and validation of HTTP request objects, with built-in support for popular web frameworks, including Flask, Django, Bottle, Tornado, Pyramid, Falcon, and aiohttp.
 Home-page: https://github.com/marshmallow-code/webargs
 Author: Steven Loria
 Author-email: sloria1@gmail.com
 License: MIT
 Project-URL: Changelog, https://webargs.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://github.com/marshmallow-code/webargs/issues
 Project-URL: Funding, https://opencollective.com/marshmallow
 Project-URL: Tidelift, https://tidelift.com/subscription/pkg/pypi-webargs?utm_source=pypi-marshmallow&utm_medium=pypi
 Keywords: webargs,http,flask,django,bottle,tornado,aiohttp,request,arguments,validation,parameters,rest,api,marshmallow
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Python: >=3.7.2
 Provides-Extra: frameworks
 Provides-Extra: tests
 Provides-Extra: lint
@@ -143,9 +143,7 @@
 - Ecosystem / related packages: https://github.com/marshmallow-code/webargs/wiki/Ecosystem
 
 
 License
 =======
 
 MIT licensed. See the `LICENSE <https://github.com/marshmallow-code/webargs/blob/dev/LICENSE>`_ file for more details.
-
-
```

### Comparing `webargs-8.2.0/src/webargs.egg-info/requires.txt` & `webargs-8.3.0/src/webargs.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 Flask>=0.12.5
 Django>=2.2.0
 bottle>=0.12.13
 tornado>=4.5.2
 pyramid>=1.9.1
 falcon>=2.0.0
 aiohttp>=3.0.8
-mypy==0.961
-flake8==4.0.1
-flake8-bugbear==22.7.1
-pre-commit~=2.4
+mypy==1.4.1
+flake8==6.0.0
+flake8-bugbear==23.6.5
+pre-commit<4.0,>=2.4
 tox
 
 [docs]
-Sphinx==5.0.2
+Sphinx==7.0.1
 sphinx-issues==3.0.1
-furo==2022.6.21
+furo==2023.5.20
 Flask>=0.12.5
 Django>=2.2.0
 bottle>=0.12.13
 tornado>=4.5.2
 pyramid>=1.9.1
 falcon>=2.0.0
 aiohttp>=3.0.8
@@ -38,18 +38,18 @@
 bottle>=0.12.13
 tornado>=4.5.2
 pyramid>=1.9.1
 falcon>=2.0.0
 aiohttp>=3.0.8
 
 [lint]
-mypy==0.961
-flake8==4.0.1
-flake8-bugbear==22.7.1
-pre-commit~=2.4
+mypy==1.4.1
+flake8==6.0.0
+flake8-bugbear==23.6.5
+pre-commit<4.0,>=2.4
 
 [tests]
 pytest
 pytest-asyncio
 webtest==3.0.0
 webtest-aiohttp==2.0.0
 pytest-aiohttp>=0.3.0
```

### Comparing `webargs-8.2.0/tests/apps/aiohttp_app.py` & `webargs-8.3.0/tests/apps/aiohttp_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from aiohttp.web import json_response
 import marshmallow as ma
 
 from webargs import fields
 from webargs.aiohttpparser import parser, use_args, use_kwargs
 from webargs.core import json
 
-hello_args = {"name": fields.Str(missing="World", validate=lambda n: len(n) >= 3)}
+hello_args = {"name": fields.Str(load_default="World", validate=lambda n: len(n) >= 3)}
 hello_multiple = {"name": fields.List(fields.Str())}
 
 
 class HelloSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
 
 
 hello_many_schema = HelloSchema(many=True)
 
 # variant which ignores unknown fields
 hello_exclude_schema = HelloSchema(unknown=ma.EXCLUDE)
```

### Comparing `webargs-8.2.0/tests/apps/bottle_app.py` & `webargs-8.3.0/tests/apps/bottle_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import marshmallow as ma
 from webargs import fields
 from webargs.bottleparser import parser, use_args, use_kwargs
 from webargs.core import json
 
 
-hello_args = {"name": fields.Str(missing="World", validate=lambda n: len(n) >= 3)}
+hello_args = {"name": fields.Str(load_default="World", validate=lambda n: len(n) >= 3)}
 hello_multiple = {"name": fields.List(fields.Str())}
 
 
 class HelloSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
 
 
 hello_many_schema = HelloSchema(many=True)
 
 # variant which ignores unknown fields
 hello_exclude_schema = HelloSchema(unknown=ma.EXCLUDE)
```

### Comparing `webargs-8.2.0/tests/apps/django_app/base/settings.py` & `webargs-8.3.0/tests/apps/django_app/base/settings.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/tests/apps/django_app/base/urls.py` & `webargs-8.3.0/tests/apps/django_app/base/urls.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/tests/apps/django_app/echo/views.py` & `webargs-8.3.0/tests/apps/django_app/echo/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import marshmallow as ma
 
 from webargs import fields
 from webargs.djangoparser import parser, use_args, use_kwargs
 from webargs.core import json
 
 
-hello_args = {"name": fields.Str(missing="World", validate=lambda n: len(n) >= 3)}
+hello_args = {"name": fields.Str(load_default="World", validate=lambda n: len(n) >= 3)}
 hello_multiple = {"name": fields.List(fields.Str())}
 
 
 class HelloSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
 
 
 hello_many_schema = HelloSchema(many=True)
 
 # variant which ignores unknown fields
 hello_exclude_schema = HelloSchema(unknown=ma.EXCLUDE)
```

### Comparing `webargs-8.2.0/tests/apps/falcon_app.py` & `webargs-8.3.0/tests/apps/falcon_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import falcon
 import marshmallow as ma
 
 from webargs import fields
 from webargs.core import json
 from webargs.falconparser import parser, use_args, use_kwargs
 
-hello_args = {"name": fields.Str(missing="World", validate=lambda n: len(n) >= 3)}
+hello_args = {"name": fields.Str(load_default="World", validate=lambda n: len(n) >= 3)}
 hello_multiple = {"name": fields.List(fields.Str())}
 
 FALCON_MAJOR_VERSION = int(falcon.__version__.split(".")[0])
 FALCON_SUPPORTS_ASYNC = FALCON_MAJOR_VERSION >= 3
 
 
 class HelloSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
 
 
 hello_many_schema = HelloSchema(many=True)
 
 # variant which ignores unknown fields
 hello_exclude_schema = HelloSchema(unknown=ma.EXCLUDE)
 
@@ -133,15 +133,15 @@
 
     on_post = on_get
 
 
 class EchoHeaders:
     def on_get(self, req, resp):
         class HeaderSchema(ma.Schema):
-            NAME = fields.Str(missing="World")
+            NAME = fields.Str(load_default="World")
 
         resp.body = json.dumps(parser.parse(HeaderSchema(), req, location="headers"))
 
 
 class EchoCookie:
     def on_get(self, req, resp):
         resp.body = json.dumps(parser.parse(hello_args, req, location="cookies"))
```

### Comparing `webargs-8.2.0/tests/apps/flask_app.py` & `webargs-8.3.0/tests/apps/flask_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 FLASK_SUPPORTS_ASYNC = FLASK_MAJOR_VERSION >= 2
 
 
 class TestAppConfig:
     TESTING = True
 
 
-hello_args = {"name": fields.Str(missing="World", validate=lambda n: len(n) >= 3)}
+hello_args = {"name": fields.Str(load_default="World", validate=lambda n: len(n) >= 3)}
 hello_multiple = {"name": fields.List(fields.Str())}
 
 
 class HelloSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
 
 
 hello_many_schema = HelloSchema(many=True)
 
 app = Flask(__name__)
 app.config.from_object(TestAppConfig)
```

### Comparing `webargs-8.2.0/tests/apps/pyramid_app.py` & `webargs-8.3.0/tests/apps/pyramid_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from pyramid.httpexceptions import HTTPBadRequest
 import marshmallow as ma
 
 from webargs import fields
 from webargs.pyramidparser import parser, use_args, use_kwargs
 from webargs.core import json
 
-hello_args = {"name": fields.Str(missing="World", validate=lambda n: len(n) >= 3)}
+hello_args = {"name": fields.Str(load_default="World", validate=lambda n: len(n) >= 3)}
 hello_multiple = {"name": fields.List(fields.Str())}
 
 
 class HelloSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
 
 
 hello_many_schema = HelloSchema(many=True)
 
 # variant which ignores unknown fields
 hello_exclude_schema = HelloSchema(unknown=ma.EXCLUDE)
```

### Comparing `webargs-8.2.0/tests/test_aiohttpparser.py` & `webargs-8.3.0/tests/test_aiohttpparser.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/tests/test_core.py` & `webargs-8.3.0/tests/test_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import collections
 import datetime
 import typing
 from unittest import mock
 
 import pytest
+from bottle import MultiDict as BotMultiDict
+from django.utils.datastructures import MultiValueDict as DjMultiDict
 from marshmallow import (
+    EXCLUDE,
+    INCLUDE,
+    RAISE,
     Schema,
     post_load,
     pre_load,
     validates_schema,
-    EXCLUDE,
-    INCLUDE,
-    RAISE,
-)
-from werkzeug.datastructures import MultiDict as WerkMultiDict
-from django.utils.datastructures import MultiValueDict as DjMultiDict
-from bottle import MultiDict as BotMultiDict
-
-from webargs import fields, ValidationError
-from webargs.core import (
-    Parser,
-    is_json,
-    get_mimetype,
 )
+from webargs import ValidationError, fields
+from webargs.core import Parser, get_mimetype, is_json
 from webargs.multidictproxy import MultiDictProxy
+from werkzeug.datastructures import MultiDict as WerkMultiDict
 
 
 class MockHTTPError(Exception):
     def __init__(self, status_code, headers):
         self.status_code = status_code
         self.headers = headers
         super().__init__(self, "HTTP Error occurred")
@@ -45,15 +40,15 @@
     def load_json(self, req, schema):
         return req.json
 
     def load_cookies(self, req, schema):
         return req.cookies
 
 
-@pytest.yield_fixture(scope="function")
+@pytest.fixture(scope="function")
 def web_request():
     req = mock.Mock()
     req.query = {}
     yield req
     req.query = {}
 
 
@@ -295,32 +290,32 @@
 
 def test_default_location():
     assert Parser.DEFAULT_LOCATION == "json"
 
 
 def test_missing_with_default(parser, web_request):
     web_request.json = {}
-    args = {"val": fields.Field(missing="pizza")}
+    args = {"val": fields.Field(load_default="pizza")}
     result = parser.parse(args, web_request)
     assert result["val"] == "pizza"
 
 
 def test_default_can_be_none(parser, web_request):
     web_request.json = {}
-    args = {"val": fields.Field(missing=None, allow_none=True)}
+    args = {"val": fields.Field(load_default=None, allow_none=True)}
     result = parser.parse(args, web_request)
     assert result["val"] is None
 
 
 # Regression test for issue #11
 def test_arg_with_default_and_location(parser, web_request):
     web_request.json = {}
     args = {
         "p": fields.Int(
-            missing=1,
+            load_default=1,
             validate=lambda p: p > 0,
             error="La page demandée n'existe pas",
             location="querystring",
         )
     }
     assert parser.parse(args, web_request) == {"p": 1}
 
@@ -506,15 +501,14 @@
     result = parser.parse(
         {"x_foo": fields.Int(data_key="X-Foo")}, web_request, location="data"
     )
     assert result["x_foo"] == 42
 
 
 def test_full_input_validation(parser, web_request):
-
     web_request.json = {"foo": 41, "bar": 42}
 
     args = {"foo": fields.Int(), "bar": fields.Int()}
     with pytest.raises(ValidationError):
         # Test that `validate` receives dictionary of args
         parser.parse(args, web_request, validate=lambda args: args["foo"] > args["bar"])
 
@@ -653,27 +647,27 @@
 
 def test_parse_nested_with_missing_key_and_data_key(web_request):
     parser = MockRequestParser()
 
     web_request.json = {"nested_arg": {}}
     args = {
         "nested_arg": fields.Nested(
-            {"found": fields.Field(missing=None, allow_none=True, data_key="miss")}
+            {"found": fields.Field(load_default=None, allow_none=True, data_key="miss")}
         )
     }
 
     parsed = parser.parse(args, web_request)
     assert parsed == {"nested_arg": {"found": None}}
 
 
 def test_parse_nested_with_default(web_request):
     parser = MockRequestParser()
 
     web_request.json = {"nested_arg": {}}
-    args = {"nested_arg": fields.Nested({"miss": fields.Field(missing="<foo>")})}
+    args = {"nested_arg": fields.Nested({"miss": fields.Field(load_default="<foo>")})}
 
     parsed = parser.parse(args, web_request)
     assert parsed == {"nested_arg": {"miss": "<foo>"}}
 
 
 def test_nested_many(web_request, parser):
     web_request.json = {"pets": [{"name": "Pips"}, {"name": "Zula"}]}
@@ -718,14 +712,21 @@
     @parser.use_args(json_args, web_request)
     def viewfunc(query_parsed, json_parsed):
         return {"json": json_parsed, "query": query_parsed}
 
     assert viewfunc() == {"json": {"username": "foo"}, "query": {"page": 42}}
 
 
+def test_use_args_forbids_invalid_usages(parser):
+    with pytest.raises(
+        ValueError, match="arg_name and as_kwargs are mutually exclusive"
+    ):
+        parser.use_args({}, web_request, arg_name="foo", as_kwargs=True)
+
+
 def test_use_kwargs_stacked(web_request, parser):
     query_args = {
         "page": fields.Int(error_messages={"invalid": "{input} not a valid integer"})
     }
     json_args = {"username": fields.Str()}
     web_request.json = {"username": "foo"}
     web_request.query = {"page": 42}
@@ -771,15 +772,14 @@
         parser.parse(args, web_request)
     assert excinfo.value.messages == {
         "json": {"ids": ["Missing data for required field."]}
     }
 
 
 def test_parse_with_callable(web_request, parser):
-
     web_request.json = {"foo": 42}
 
     class MySchema(Schema):
         foo = fields.Field()
 
     def make_schema(req):
         assert req is web_request
@@ -823,15 +823,14 @@
         web_request.json = {"email": "foo@bar.com", "password": "bar"}
 
         result = parser.parse(self.UserSchema(), web_request)
 
         assert result == {"email": "foo@bar.com", "password": "bar"}
 
     def test_use_args_can_be_passed_a_schema(self, web_request, parser):
-
         web_request.json = {"email": "foo@bar.com", "password": "bar"}
 
         @parser.use_args(self.UserSchema(), web_request)
         def viewfunc(args):
             return args
 
         assert viewfunc() == {"email": "foo@bar.com", "password": "bar"}
@@ -857,15 +856,14 @@
         @parser.use_args(factory, web_request)
         def viewfunc(args):
             return args
 
         assert viewfunc() == {"email": "foo@bar.com", "password": "bar"}
 
     def test_use_kwargs_can_be_passed_a_schema(self, web_request, parser):
-
         web_request.json = {"email": "foo@bar.com", "password": "bar"}
 
         @parser.use_kwargs(self.UserSchema(), web_request)
         def viewfunc(email, password):
             return {"email": email, "password": password}
 
         assert viewfunc() == {"email": "foo@bar.com", "password": "bar"}
@@ -1396,17 +1394,188 @@
     # doesn't strip whitespace from JSON data
     #   - values=[" foo  ", ...]  will have whitespace preserved
     #   - ids=[" 1", ...]  will still parse okay because "  1" is valid for fields.Int
     ret = parser.parse(schema, web_request, location="json")
     assert ret == {"ids": [1, 3, 4], "values": [" foo  ", " bar"]}
 
 
-def test_parse_rejects_non_dict_argmap_mapping(parser, web_request):
-    web_request.json = {"username": 42, "password": 42}
+def test_parse_allows_non_dict_argmap_mapping(parser, web_request):
+    web_request.json = {"username": "dadams", "password": 42}
+    # UserDict is dict-like in all meaningful ways, but not a subclass of `dict`
+    # it will therefore need to be converted when used
     argmap = collections.UserDict(
-        {"username": fields.Field(), "password": fields.Field()}
+        {"username": fields.String(), "password": fields.Field()}
     )
 
+    ret = parser.parse(argmap, web_request)
+    assert ret == {"username": "dadams", "password": 42}
+
+
+def test_use_args_allows_non_dict_argmap_mapping(parser, web_request):
+    web_request.json = {"username": "dadams", "password": 42}
     # UserDict is dict-like in all meaningful ways, but not a subclass of `dict`
-    # it will therefore be rejected with a TypeError when used
+    # it will therefore need to be converted when used
+    argmap = collections.UserDict(
+        {"username": fields.String(), "password": fields.Field()}
+    )
+
+    @parser.use_args(argmap, web_request)
+    def viewfunc(args):
+        return args
+
+    assert viewfunc() == {"username": "dadams", "password": 42}
+
+
+def test_parse_rejects_unknown_argmap_type(parser, web_request):
+    web_request.json = {"username": "dadams", "password": 42}
+
+    class MyType:
+        pass
+
+    with pytest.raises(TypeError, match="argmap was of unexpected type"):
+        parser.parse(MyType(), web_request)
+
+
+def test_parser_opt_out_positional_args(web_request):
+    class OptOutParser(MockRequestParser):
+        USE_ARGS_POSITIONAL = False
+
+    parser = MockRequestParser()
+    opt_out_parser = OptOutParser()
+    web_request.json = {"foo": "bar"}
+
+    # first, test the behavior of a base parser for comparison
+    #
+    # no specific arg name, default parser, everything works
+    # works for 'args', 'json_args', or any other name
+    @parser.use_args({"foo": fields.Field()}, web_request)
+    def viewfunc1(args):
+        return args
+
+    @parser.use_args({"foo": fields.Field()}, web_request)
+    def viewfunc2(json_args):
+        return json_args
+
+    assert viewfunc1() == {"foo": "bar"}
+    assert viewfunc2() == {"foo": "bar"}
+
+    # second, test the behavior of a parser which sets USE_ARGS_POSITIONAL=False
+    #
+    # `json_args` as the arg name works as a positional or keyword-only
+    # but `args` as the arg name does not
+    @opt_out_parser.use_args({"foo": fields.Field()}, web_request)
+    def viewfunc3(json_args):
+        return json_args
+
+    @opt_out_parser.use_args({"foo": fields.Field()}, web_request)
+    def viewfunc4(*, json_args):
+        return json_args
+
+    @opt_out_parser.use_args({"foo": fields.Field()}, web_request)
+    def viewfunc5(args):
+        return args
+
+    assert viewfunc3() == {"foo": "bar"}
+    assert viewfunc4() == {"foo": "bar"}
+
     with pytest.raises(TypeError):
-        parser.parse(argmap, web_request)
+        assert viewfunc5()
+
+
+def test_use_args_implicit_arg_names(web_request):
+    class OptOutParser(MockRequestParser):
+        USE_ARGS_POSITIONAL = False
+
+    parser = OptOutParser()
+    web_request.json = {"foo": "bar"}
+    web_request.query = {"bar": "baz"}
+
+    @parser.use_args({"foo": fields.Field()}, web_request)
+    @parser.use_args({"bar": fields.Field()}, web_request, location="query")
+    def viewfunc(*, json_args, query_args):
+        return (json_args, query_args)
+
+    assert viewfunc() == ({"foo": "bar"}, {"bar": "baz"})
+
+
+@pytest.mark.parametrize("use_positional_setting", (True, False))
+def test_use_args_explicit_arg_names(web_request, use_positional_setting):
+    class MyParser(MockRequestParser):
+        USE_ARGS_POSITIONAL = use_positional_setting
+
+    parser = MyParser()
+    web_request.json = {"foo": "bar"}
+    web_request.query = {"bar": "baz"}
+
+    @parser.use_args({"foo": fields.Field()}, web_request, arg_name="j")
+    @parser.use_args(
+        {"bar": fields.Field()}, web_request, location="query", arg_name="q"
+    )
+    def viewfunc(*, j, q):
+        return (j, q)
+
+    assert viewfunc() == ({"foo": "bar"}, {"bar": "baz"})
+
+
+def test_use_args_errors_on_explicit_arg_name_conflict(web_request):
+    parser = MockRequestParser()
+    web_request.json = {"foo": "bar"}
+    web_request.query = {"bar": "baz"}
+
+    with pytest.raises(ValueError, match="Attempted to pass `arg_name='q'`"):
+
+        @parser.use_args({"foo": fields.Field()}, web_request, arg_name="q")
+        @parser.use_args(
+            {"bar": fields.Field()}, web_request, location="query", arg_name="q"
+        )
+        def viewfunc(*, j, q):
+            return (j, q)
+
+
+def test_use_args_errors_on_implicit_arg_name_conflict(web_request):
+    class MyParser(MockRequestParser):
+        USE_ARGS_POSITIONAL = False
+
+    parser = MyParser()
+    web_request.json = {"foo": "bar"}
+
+    with pytest.raises(ValueError, match="Attempted to pass `arg_name='json_args'`"):
+
+        @parser.use_args({"foo": fields.Field()}, web_request)
+        @parser.use_args({"foo": fields.Field()}, web_request)
+        def viewfunc(*, j, q):
+            return (j, q)
+
+
+def test_use_args_with_arg_name_supports_multi_stacked_decorators(web_request):
+    # this test case specifically explores the use-case in which a view function is
+    # decorated with one `use_args` call, and then "permuted" by decorating it with
+    # other `use_args` calls
+    class MyParser(MockRequestParser):
+        USE_ARGS_POSITIONAL = False
+
+    parser = MyParser()
+
+    # create two body variants of the same route, from a single function
+    # they share the same query params
+    with_body_foo = parser.use_args({"foo": fields.Field()}, web_request)
+    with_body_bar = parser.use_args({"bar": fields.Field()}, web_request)
+
+    @parser.use_args({"snork": fields.Field()}, web_request, location="query")
+    def mypartial(*, json_args, query_args):
+        return (json_args, query_args)
+
+    route_foo = with_body_foo(mypartial)
+    route_bar = with_body_bar(mypartial)
+
+    # first, test that these behave as expected
+    web_request.json = {"foo": "bar"}
+    web_request.query = {"snork": 2}
+    assert route_foo() == ({"foo": "bar"}, {"snork": 2})
+
+    web_request.json = {"bar": "baz"}
+    assert route_bar() == ({"bar": "baz"}, {"snork": 2})
+
+    # now, inspect their internal state
+    assert mypartial.__webargs_argnames__ == ("query_args",)
+    assert route_foo.__webargs_argnames__ == ("query_args", "json_args")
+    assert route_bar.__webargs_argnames__ == ("query_args", "json_args")
```

### Comparing `webargs-8.2.0/tests/test_djangoparser.py` & `webargs-8.3.0/tests/test_djangoparser.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/tests/test_falconparser.py` & `webargs-8.3.0/tests/test_falconparser.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/tests/test_flaskparser.py` & `webargs-8.3.0/tests/test_flaskparser.py`

 * *Files identical despite different names*

### Comparing `webargs-8.2.0/tests/test_tornadoparser.py` & `webargs-8.3.0/tests/test_tornadoparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 name = "name"
 value = "value"
 
 
 class AuthorSchema(ma.Schema):
-    name = fields.Str(missing="World", validate=lambda n: len(n) >= 3)
+    name = fields.Str(load_default="World", validate=lambda n: len(n) >= 3)
     works = fields.List(fields.Str())
 
 
 author_schema = AuthorSchema()
 
 
 def test_tornado_multidictproxy():
```

### Comparing `webargs-8.2.0/tox.ini` & `webargs-8.3.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tox]
 envlist=
     lint
-    py{37,38,39,310}
+    py{37,38,39,310,311}
     py37-mindeps
-    py310-marshmallowdev
+    py311-marshmallowdev
     docs
 
 [testenv]
 extras = tests
 deps =
     !marshmallowdev: marshmallow>=3.0.0,<4.0.0
     marshmallowdev: https://github.com/marshmallow-code/marshmallow/archive/dev.tar.gz
@@ -38,17 +38,17 @@
 skip_install = true
 commands = pre-commit run --all-files
 
 # a separate `mypy` target which runs `mypy` in an environment with
 # `webargs` and `marshmallow` both installed is a valuable safeguard against
 # issues in which `mypy` running on every file standalone won't catch things
 [testenv:mypy]
-deps = mypy==0.930
+deps = mypy==1.3.0
 extras = frameworks
-commands = mypy src/
+commands = mypy src/ {posargs}
 
 [testenv:docs]
 extras = docs
 commands = sphinx-build docs/ docs/_build {posargs}
 
 ; Below tasks are for development only (not run in CI)
```

