# Comparing `tmp/scippnexus-23.5.1.tar.gz` & `tmp/scippnexus-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippnexus-23.5.1.tar", last modified: Wed May 24 07:01:07 2023, max compression
+gzip compressed data, was "scippnexus-23.7.0.tar", last modified: Mon Jul 10 08:10:46 2023, max compression
```

## Comparing `scippnexus-23.5.1.tar` & `scippnexus-23.7.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-05-24 07:00:53.000000 scippnexus-23.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-24 07:00:53.000000 scippnexus-23.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 07:00:53.000000 scippnexus-23.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-24 07:01:07.320955 scippnexus-23.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-05-24 07:00:53.000000 scippnexus-23.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-24 07:00:53.000000 scippnexus-23.5.1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_static/logo-2022.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/about/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/getting-started/quick-start-guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/application-definitions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/functions.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/user-guide/nexus-classes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-05-24 07:00:53.000000 scippnexus-23.5.1/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-24 07:00:53.000000 scippnexus-23.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-24 07:00:53.000000 scippnexus-23.5.1/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.312955 scippnexus-23.5.1/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-05-24 07:00:53.000000 scippnexus-23.5.1/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-24 07:01:07.320955 scippnexus-23.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/_hdf5_nexus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/data/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/definitions/
--rw-r--r--   0 runner    (1001) docker     (122)     5027 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/definitions/nxcansas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/file.py
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/leaf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    11665 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     9934 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxdetector.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxdisk_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxfermi_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxlog.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxmonitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    25066 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxsource.py
--rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/nxtransformations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/src/scippnexus/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.308956 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/attrs.py
--rw-r--r--   0 runner    (1001) docker     (122)    18007 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/file.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    26655 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     5942 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)     8477 2023-05-24 07:00:53.000000 scippnexus-23.5.1/src/scippnexus/v2/nxtransformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.316955 scippnexus-23.5.1/src/scippnexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-24 07:01:07.000000 scippnexus-23.5.1/src/scippnexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 07:01:07.320955 scippnexus-23.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/application_definition_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/externalfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/load_files_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    19069 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxcylindrical_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    27977 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxdata_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    28814 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxdetector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5341 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxevent_data_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxlog_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxmonitor_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxoff_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxsample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18094 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tests/nxtransformations_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-05-24 07:00:53.000000 scippnexus-23.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.688113 scippnexus-23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3695 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-10 08:10:30.000000 scippnexus-23.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-07-10 08:10:30.000000 scippnexus-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-10 08:10:30.000000 scippnexus-23.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-10 08:10:46.688113 scippnexus-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-07-10 08:10:30.000000 scippnexus-23.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-10 08:10:30.000000 scippnexus-23.7.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/_static/logo-2022.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.672113 scippnexus-23.7.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7443 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/about/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.676113 scippnexus-23.7.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/getting-started/quick-start-guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.676113 scippnexus-23.7.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/user-guide/application-definitions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/user-guide/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/user-guide/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/user-guide/nexus-classes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-07-10 08:10:30.000000 scippnexus-23.7.0/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-10 08:10:30.000000 scippnexus-23.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.676113 scippnexus-23.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-10 08:10:30.000000 scippnexus-23.7.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.676113 scippnexus-23.7.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-07-10 08:10:30.000000 scippnexus-23.7.0/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-10 08:10:46.688113 scippnexus-23.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.668113 scippnexus-23.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.680113 scippnexus-23.7.0/src/scippnexus/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4520 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/_hdf5_nexus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.680113 scippnexus-23.7.0/src/scippnexus/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.680113 scippnexus-23.7.0/src/scippnexus/definitions/
+-rw-r--r--   0 runner    (1001) docker     (122)     5027 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/definitions/nxcansas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.680113 scippnexus-23.7.0/src/scippnexus/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11487 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9934 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxdetector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxdisk_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxfermi_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxlog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25066 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxsource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/nxtransformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.684113 scippnexus-23.7.0/src/scippnexus/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.668113 scippnexus-23.7.0/src/scippnexus/v2/application_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.684113 scippnexus-23.7.0/src/scippnexus/v2/application_definitions/nxcansas/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18007 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26716 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5942 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3549 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8477 2023-07-10 08:10:30.000000 scippnexus-23.7.0/src/scippnexus/v2/nxtransformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.680113 scippnexus-23.7.0/src/scippnexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-10 08:10:46.000000 scippnexus-23.7.0/src/scippnexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-07-10 08:10:46.000000 scippnexus-23.7.0/src/scippnexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 08:10:46.000000 scippnexus-23.7.0/src/scippnexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-10 08:10:46.000000 scippnexus-23.7.0/src/scippnexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-10 08:10:46.000000 scippnexus-23.7.0/src/scippnexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 08:10:46.688113 scippnexus-23.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/application_definition_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/externalfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/load_files_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19069 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxcylindrical_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27977 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28814 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxdetector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5341 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxevent_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxlog_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxmonitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxoff_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxsample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18094 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tests/nxtransformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-07-10 08:10:30.000000 scippnexus-23.7.0/tox.ini
```

### Comparing `scippnexus-23.5.1/.github/workflows/ci.yml` & `scippnexus-23.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/.github/workflows/docs.yml` & `scippnexus-23.7.0/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -41,29 +41,29 @@
       - run: sudo apt install --yes graphviz pandoc
       - uses: actions/checkout@v3
         with:
           ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
           fetch-depth: 0  # history required so cmake can determine version
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: '3.8'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
           tox --skip-pkg-install -e docs -- scippnexus==${VERSION}
           echo "target=$(python docs/version.py --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
         if: ${{ inputs.publish }}
       - run: tox -e docs
         if: ${{ !inputs.publish }}
       - uses: actions/upload-artifact@v3
         with:
           name: html
           path: html/
 
-      - uses: JamesIves/github-pages-deploy-action@v4.4.1
+      - uses: JamesIves/github-pages-deploy-action@v4.4.2
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           target-folder: ${{ env.target }}
           single-commit: true
           clean-exclude: release
```

### Comparing `scippnexus-23.5.1/.github/workflows/release.yml` & `scippnexus-23.7.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,57 +30,59 @@
           path: conda/package/*/scippnexus*.tar.bz2
 
   build_wheels:
     name: Wheels
     runs-on: ubuntu-20.04
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0  # history required so setuptools_scm can determine version
 
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: '3.8'
 
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/wheels.txt
 
       - name: Build wheels
         run: python -m build
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
           path: dist
 
   upload_pypi:
     name: Deploy PyPI
     needs: [build_wheels, build_conda]
     runs-on: ubuntu-20.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
       - uses: actions/setup-python@v3
-      - uses: pypa/gh-action-pypi-publish@v1.8.6
+      - uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   upload_conda:
     name: Deploy Conda Forge
     needs: [build_wheels, build_conda]
     runs-on: ubuntu-20.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
       - uses: conda-incubator/setup-miniconda@v2
+        with:
+          python-version: '3.10'
       - run: conda install -c conda-forge --yes anaconda-client
       - run: anaconda --token ${{ secrets.ANACONDATOKEN }} upload --user scipp --label main $(ls conda-package-*/*/*.tar.bz2)
 
   manage-versions:
     name: Manage Versions
     runs-on: ubuntu-20.04
     outputs:
@@ -88,15 +90,15 @@
       version-replaced: ${{ steps.version.outputs.replaced }}
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0  # history required so cmake can determine version
       - uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: '3.8'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
         run: |
           echo "new=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=is-new)" >> $GITHUB_OUTPUT
           echo "replaced=$(python docs/version.py --version=${GITHUB_REF_NAME} --action=get-replaced)" >> $GITHUB_OUTPUT
```

### Comparing `scippnexus-23.5.1/.pre-commit-config.yaml` & `scippnexus-23.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/LICENSE` & `scippnexus-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/PKG-INFO` & `scippnexus-23.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.5.1
+Version: 23.7.0
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.5.1/README.md` & `scippnexus-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/conda/meta.yaml` & `scippnexus-23.7.0/conda/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requirements:
   build:
     - setuptools
     - setuptools_scm
   run:
     - python>=3.8
     - python-dateutil
-    - scipp>=23.03.1
+    - scipp>=23.07.0
     - scipy
     - h5py
 
 test:
   imports:
     - scippnexus
   requires:
```

### Comparing `scippnexus-23.5.1/docs/_static/favicon.ico` & `scippnexus-23.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/_static/logo-2022.svg` & `scippnexus-23.7.0/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/_templates/scipp-class-template.rst` & `scippnexus-23.7.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/_templates/scipp-module-template.rst` & `scippnexus-23.7.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/_templates/sections/header-article.html` & `scippnexus-23.7.0/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/about/about.rst` & `scippnexus-23.7.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/about/release-notes.rst` & `scippnexus-23.7.0/docs/about/release-notes.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 
 Release Notes
 =============
 
 
 .. Template, copy this to create a new section after a release:
 
-   v0.xy.0 (Unreleased)
-   --------------------
+   vrelease
+   --------
 
    Features
    ~~~~~~~~
 
    Breaking changes
    ~~~~~~~~~~~~~~~~
 
    Bugfixes
    ~~~~~~~~
 
    Deprecations
    ~~~~~~~~~~~~
 
-   Contributors
-   ~~~~~~~~~~~~
+v23.07.0
+--------
+
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-   Simon Heybrock :sup:`a`\ ,
-   Neil Vaytet :sup:`a`\ ,
-   and Jan-Lukas Wynen :sup:`a`
+* When loading slices, coordinates are no longer converted to attributes but are flagged as unaligned.
+  This is equivalent to slicing in Scipp since v23.07.0 `#154 <https://github.com/scipp/scippnexus/pull/154>`_.
 
 v23.05.1
 --------
 
 Bugfixes
 ~~~~~~~~
```

### Comparing `scippnexus-23.5.1/docs/conf.py` & `scippnexus-23.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/getting-started/installation.rst` & `scippnexus-23.7.0/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/getting-started/quick-start-guide.ipynb` & `scippnexus-23.7.0/docs/getting-started/quick-start-guide.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/index.rst` & `scippnexus-23.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/user-guide/application-definitions.ipynb` & `scippnexus-23.7.0/docs/user-guide/application-definitions.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/user-guide/classes.rst` & `scippnexus-23.7.0/docs/user-guide/classes.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/user-guide/nexus-classes.ipynb` & `scippnexus-23.7.0/docs/user-guide/nexus-classes.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/docs/version.py` & `scippnexus-23.7.0/docs/version.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/pyproject.toml` & `scippnexus-23.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/requirements/ci.txt` & `scippnexus-23.7.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/requirements/docs.txt` & `scippnexus-23.7.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/requirements/static.txt` & `scippnexus-23.7.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/resources/logo-2022.svg` & `scippnexus-23.7.0/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/setup.cfg` & `scippnexus-23.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	python-dateutil
-	scipp>=23.03.1
+	scipp>=23.07.0
 	scipy  # we use scipp.interpolate which depends on this
 	h5py
 python_requires = >=3.8
 include_package_data = True
 
 [options.packages.find]
 where = src
```

### Comparing `scippnexus-23.5.1/src/scippnexus/__init__.py` & `scippnexus-23.7.0/src/scippnexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/_common.py` & `scippnexus-23.7.0/src/scippnexus/_common.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/_hdf5_nexus.py` & `scippnexus-23.7.0/src/scippnexus/_hdf5_nexus.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/data/__init__.py` & `scippnexus-23.7.0/src/scippnexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/definition.py` & `scippnexus-23.7.0/src/scippnexus/definition.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/definitions/nxcansas.py` & `scippnexus-23.7.0/src/scippnexus/definitions/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md` & `scippnexus-23.7.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/file.py` & `scippnexus-23.7.0/src/scippnexus/file.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/leaf.py` & `scippnexus-23.7.0/src/scippnexus/leaf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nexus_classes.py` & `scippnexus-23.7.0/src/scippnexus/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxcylindrical_geometry.py` & `scippnexus-23.7.0/src/scippnexus/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxdata.py` & `scippnexus-23.7.0/src/scippnexus/nxdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,21 +223,21 @@
     def _dim_of_coord(self, name: str, coord: Field) -> Union[None, str]:
         if len(coord.dims) == 1:
             return coord.dims[0]
         if name in coord.dims and name in self.dims:
             return name
         return self._bin_edge_dim(coord)
 
-    def _coord_to_attr(self, da: sc.DataArray, name: str, coord: Field) -> bool:
+    def _should_be_aligned(self, da: sc.DataArray, name: str, coord: Field) -> bool:
         dim_of_coord = self._dim_of_coord(name, coord)
         if dim_of_coord is None:
-            return False
-        if dim_of_coord not in da.dims:
             return True
-        return False
+        if dim_of_coord not in da.dims:
+            return False
+        return True
 
     def _getitem(self, select: ScippIndex) -> sc.DataArray:
         from .nexus_classes import NXgeometry
 
         signal = self._signal
         if signal is None:
             raise NexusStructureError("No signal field found, cannot load group.")
@@ -288,19 +288,15 @@
                 self.dims, field.dims, select, bin_edge_dim=self._bin_edge_dim(field)
             )
             coord: sc.Variable = asarray(self[name][sel])
             if (error_name := self._strategy.coord_errors(self, name)) is not None:
                 stddevs = asarray(self[error_name][sel])
                 coord.variances = sc.pow(stddevs, sc.scalar(2)).values
             try:
-                if self._coord_to_attr(da, name, field):
-                    # Like scipp, slicing turns coord into attr if slicing removes the
-                    # dim corresponding to the coord.
-                    da.attrs[name] = coord
-                else:
-                    da.coords[name] = coord
+                da.coords[name] = coord
+                da.coords.set_aligned(name, self._should_be_aligned(da, name, field))
             except sc.DimensionError as e:
                 raise NexusStructureError(
                     f"Field in NXdata incompatible with dims or shape of signal: {e}"
                 ) from e
 
         return da
```

### Comparing `scippnexus-23.5.1/src/scippnexus/nxdetector.py` & `scippnexus-23.7.0/src/scippnexus/nxdetector.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxevent_data.py` & `scippnexus-23.7.0/src/scippnexus/nxevent_data.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxlog.py` & `scippnexus-23.7.0/src/scippnexus/nxlog.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxmonitor.py` & `scippnexus-23.7.0/src/scippnexus/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxobject.py` & `scippnexus-23.7.0/src/scippnexus/nxobject.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxoff_geometry.py` & `scippnexus-23.7.0/src/scippnexus/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxsample.py` & `scippnexus-23.7.0/src/scippnexus/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/nxtransformations.py` & `scippnexus-23.7.0/src/scippnexus/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/typing.py` & `scippnexus-23.7.0/src/scippnexus/typing.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/__init__.py` & `scippnexus-23.7.0/src/scippnexus/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py` & `scippnexus-23.7.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/attrs.py` & `scippnexus-23.7.0/src/scippnexus/v2/attrs.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/base.py` & `scippnexus-23.7.0/src/scippnexus/v2/base.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/field.py` & `scippnexus-23.7.0/src/scippnexus/v2/field.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/file.py` & `scippnexus-23.7.0/src/scippnexus/v2/file.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nexus_classes.py` & `scippnexus-23.7.0/src/scippnexus/v2/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nxcylindrical_geometry.py` & `scippnexus-23.7.0/src/scippnexus/v2/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nxdata.py` & `scippnexus-23.7.0/src/scippnexus/v2/nxdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,36 +350,41 @@
     def _dim_of_coord(self, name: str, coord: sc.Variable) -> Union[None, str]:
         if len(coord.dims) == 1:
             return coord.dims[0]
         if name in coord.dims and name in self.dims:
             return name
         return self._bin_edge_dim(coord)
 
-    def _coord_to_attr(self, da: sc.DataArray, name: str, coord: sc.Variable) -> bool:
+    def _should_be_aligned(
+        self, da: sc.DataArray, name: str, coord: sc.Variable
+    ) -> bool:
         if name == 'depends_on':
-            return False
+            return True
         dim_of_coord = self._dim_of_coord(name, coord)
         if dim_of_coord is None:
-            return False
-        if dim_of_coord not in da.dims:
             return True
-        return False
+        if dim_of_coord not in da.dims:
+            return False
+        return True
 
     def _add_coords(self, da: sc.DataArray, coords: sc.DataGroup) -> sc.DataArray:
-        """Add coords to data array, converting to attrs in the same way as slicing
-        scipp.DataArray would."""
+        """Add coords to a data array.
+
+        Sets alignment in the same way as slicing scipp.DataArray would.
+        """
         for name, coord in coords.items():
             if not isinstance(coord, sc.Variable):
                 da.coords[name] = sc.scalar(coord)
-            # We need the shape *before* slicing to determine dims, so we get the
-            # field from the group for the conditional.
-            elif self._coord_to_attr(da, name, self._children[name]):
-                da.attrs[name] = coord
             else:
                 da.coords[name] = coord
+                # We need the shape *before* slicing to determine dims, so we get the
+                # field from the group for the conditional.
+                da.coords.set_aligned(
+                    name, self._should_be_aligned(da, name, self._children[name])
+                )
         return da
 
 
 def _squeeze_trailing(dims: Tuple[str, ...], shape: Tuple[int, ...]) -> Tuple[int, ...]:
     return shape[: len(dims)] + tuple(size for size in shape[len(dims) :] if size != 1)
```

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nxevent_data.py` & `scippnexus-23.7.0/src/scippnexus/v2/nxevent_data.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nxoff_geometry.py` & `scippnexus-23.7.0/src/scippnexus/v2/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nxsample.py` & `scippnexus-23.7.0/src/scippnexus/v2/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus/v2/nxtransformations.py` & `scippnexus-23.7.0/src/scippnexus/v2/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/src/scippnexus.egg-info/PKG-INFO` & `scippnexus-23.7.0/src/scippnexus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.5.1
+Version: 23.7.0
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.5.1/src/scippnexus.egg-info/SOURCES.txt` & `scippnexus-23.7.0/src/scippnexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/application_definition_test.py` & `scippnexus-23.7.0/tests/application_definition_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/conftest.py` & `scippnexus-23.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/externalfile.py` & `scippnexus-23.7.0/tests/externalfile.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/load_files_test.py` & `scippnexus-23.7.0/tests/load_files_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nexus_test.py` & `scippnexus-23.7.0/tests/nexus_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxcylindrical_geometry_test.py` & `scippnexus-23.7.0/tests/nxcylindrical_geometry_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxdata_test.py` & `scippnexus-23.7.0/tests/nxdata_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxdetector_test.py` & `scippnexus-23.7.0/tests/nxdetector_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxevent_data_test.py` & `scippnexus-23.7.0/tests/nxevent_data_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxlog_test.py` & `scippnexus-23.7.0/tests/nxlog_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxmonitor_test.py` & `scippnexus-23.7.0/tests/nxmonitor_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxoff_geometry_test.py` & `scippnexus-23.7.0/tests/nxoff_geometry_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxsample_test.py` & `scippnexus-23.7.0/tests/nxsample_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tests/nxtransformations_test.py` & `scippnexus-23.7.0/tests/nxtransformations_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.5.1/tox.ini` & `scippnexus-23.7.0/tox.ini`

 * *Files identical despite different names*

