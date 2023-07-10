# Comparing `tmp/cmcrameri-1.6.tar.gz` & `tmp/cmcrameri-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmcrameri-1.6.tar", last modified: Tue Jun 27 09:45:03 2023, max compression
+gzip compressed data, was "cmcrameri-1.7.tar", last modified: Mon Jul 10 08:45:34 2023, max compression
```

## Comparing `cmcrameri-1.6.tar` & `cmcrameri-1.7.tar`

### file list

```diff
@@ -1,82 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.885770 cmcrameri-1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.881770 cmcrameri-1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.881770 cmcrameri-1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-27 09:44:47.000000 cmcrameri-1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-27 09:44:47.000000 cmcrameri-1.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 09:44:47.000000 cmcrameri-1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.881770 cmcrameri-1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-27 09:44:47.000000 cmcrameri-1.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-27 09:44:47.000000 cmcrameri-1.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-27 09:44:47.000000 cmcrameri-1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-27 09:44:47.000000 cmcrameri-1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-27 09:44:47.000000 cmcrameri-1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 09:44:47.000000 cmcrameri-1.6/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-27 09:44:47.000000 cmcrameri-1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-27 09:45:03.885770 cmcrameri-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-27 09:44:47.000000 cmcrameri-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.881770 cmcrameri-1.6/cmcrameri/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-27 09:45:03.000000 cmcrameri-1.6/cmcrameri/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6082 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.885770 cmcrameri-1.6/cmcrameri/cmaps/
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/acton.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/actonS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bam.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bamO.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bamako.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bamakoS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/batlow.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/batlowK.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/batlowS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/batlowW.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/berlin.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bilbao.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bilbaoS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/broc.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/brocO.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/buda.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/budaS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/bukavu.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/cork.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/corkO.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/davos.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/davosS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/devon.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/devonS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/fes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/glasgow.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/grayC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/grayCS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/hawaii.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/hawaiiS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/imola.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/imolaS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/lajolla.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/lajollaS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/lapaz.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/lapazS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/lipari.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/lisbon.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/managua.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/navia.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/nuuk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/nuukS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/oleron.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/oslo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/osloS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/roma.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/romaO.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/tofino.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/tokyo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/tokyoS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/turku.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/turkuS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/vanimo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/vik.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/cmaps/vikO.txt
--rw-r--r--   0 runner    (1001) docker     (123)   147292 2023-06-27 09:44:47.000000 cmcrameri-1.6/cmcrameri/colormaps.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:45:03.885770 cmcrameri-1.6/cmcrameri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-27 09:45:03.000000 cmcrameri-1.6/cmcrameri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-27 09:44:47.000000 cmcrameri-1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 09:44:47.000000 cmcrameri-1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:45:03.885770 cmcrameri-1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.381150 cmcrameri-1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.369150 cmcrameri-1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.369150 cmcrameri-1.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 08:45:15.000000 cmcrameri-1.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 08:45:15.000000 cmcrameri-1.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 08:45:15.000000 cmcrameri-1.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.369150 cmcrameri-1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-10 08:45:15.000000 cmcrameri-1.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-10 08:45:15.000000 cmcrameri-1.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-10 08:45:15.000000 cmcrameri-1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 08:45:15.000000 cmcrameri-1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 08:45:15.000000 cmcrameri-1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 08:45:15.000000 cmcrameri-1.7/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 08:45:15.000000 cmcrameri-1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-10 08:45:34.377150 cmcrameri-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-10 08:45:15.000000 cmcrameri-1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.369150 cmcrameri-1.7/cmcrameri/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 08:45:34.000000 cmcrameri-1.7/cmcrameri/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6021 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.377150 cmcrameri-1.7/cmcrameri/cmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/acton.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/actonS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bam.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bamO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bamako.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bamakoS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/batlow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/batlowK.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/batlowKS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/batlowS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/batlowW.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/batlowWS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/berlin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bilbao.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bilbaoS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/broc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/brocO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/buda.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/budaS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/bukavu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/cork.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/corkO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/davos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/davosS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/devon.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/devonS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/fes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/glasgow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/glasgowS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/grayC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/grayCS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/hawaii.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/hawaiiS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/imola.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/imolaS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lajolla.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lajollaS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lapaz.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lapazS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lipari.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lipariS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/lisbon.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/managua.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/navia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/naviaS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/nuuk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/nuukS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/oleron.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/oslo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/osloS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/roma.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/romaO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/tofino.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/tokyo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/tokyoS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/turku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/turkuS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/vanimo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/vik.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/cmaps/vikO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   147292 2023-07-10 08:45:15.000000 cmcrameri-1.7/cmcrameri/colormaps.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:34.377150 cmcrameri-1.7/cmcrameri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-10 08:45:34.000000 cmcrameri-1.7/cmcrameri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-10 08:45:15.000000 cmcrameri-1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-10 08:45:15.000000 cmcrameri-1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:45:34.381150 cmcrameri-1.7/setup.cfg
```

### Comparing `cmcrameri-1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `cmcrameri-1.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/.github/workflows/pypi.yml` & `cmcrameri-1.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/.github/workflows/tests.yml` & `cmcrameri-1.7/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/provision-with-micromamba@v16
       with:
         environment-file: false
 
     - name: Python ${{ matrix.python-version }}
       shell: bash -l {0}
       run: >
         micromamba create --name TEST python=${{ matrix.python-version }} pytest --file requirements.txt --channel conda-forge
```

### Comparing `cmcrameri-1.6/.pre-commit-config.yaml` & `cmcrameri-1.7/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     - id: end-of-file-fixer
     - id: check-docstring-first
     - id: check-added-large-files
     - id: requirements-txt-fixer
     - id: file-contents-sorter
       files: requirements-dev.txt
 
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.260
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.0.276
   hooks:
     - id: ruff
 
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
@@ -27,22 +27,22 @@
 
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
     - id: blackdoc
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.5
   hooks:
     - id: codespell
       args:
         - --ignore-words-list=buda
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: "0.9.2"
+  rev: "0.13.0"
   hooks:
     - id: pyproject-fmt
 
 - repo: https://github.com/aio-libs/sort-all
   rev: "v1.2.0"
   hooks:
     - id: sort-all
```

### Comparing `cmcrameri-1.6/LICENSE.txt` & `cmcrameri-1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/PKG-INFO` & `cmcrameri-1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmcrameri
-Version: 1.6
+Version: 1.7
 Summary: Perceptually uniform colormaps by Fabio Crameri
 Author-email: Callum Rollo <c.rollo@outlook.com>
 License: MIT License
         
         Colormaps in cmcrameri/cm/cmaps:
         Copyright (c) 2020 Fabio Crameri
         
@@ -28,14 +28,21 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: documentation, https://callumrollo.github.io/cmcrameri
 Project-URL: homepage, https://pypi.org/project/cmcrameri/
 Project-URL: repository, https://github.com/callumrollo/cmcrameri
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![Python package](https://github.com/callumrollo/cmcrameri/workflows/Python%20package/badge.svg)
 
 [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)]()
@@ -54,15 +61,15 @@
 This is a Python wrapper around Fabio Crameri's perceptually uniform colormaps.
 
 <https://www.fabiocrameri.ch/colourmaps/>
 
 All credit for creating the colormaps to Fabio.
 Any errors in the Python implementation of colormaps are my own.
 
-This version is based on _Scientific colour maps_ [version 7.0](https://zenodo.org/record/4491293) (02.02.2021).
+This version is based on _Scientific colour maps_ [version 8.0](https://doi.org/10.5281/zenodo.8035877) (2023-06-14).
 
 ## Install
 
 With `pip`:
 
 ```sh
 python -m pip install cmcrameri
```

### Comparing `cmcrameri-1.6/README.md` & `cmcrameri-1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 This is a Python wrapper around Fabio Crameri's perceptually uniform colormaps.
 
 <https://www.fabiocrameri.ch/colourmaps/>
 
 All credit for creating the colormaps to Fabio.
 Any errors in the Python implementation of colormaps are my own.
 
-This version is based on _Scientific colour maps_ [version 7.0](https://zenodo.org/record/4491293) (02.02.2021).
+This version is based on _Scientific colour maps_ [version 8.0](https://doi.org/10.5281/zenodo.8035877) (2023-06-14).
 
 ## Install
 
 With `pip`:
 
 ```sh
 python -m pip install cmcrameri
```

### Comparing `cmcrameri-1.6/cmcrameri/cm.py` & `cmcrameri-1.7/cmcrameri/cm.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,15 @@
 
 _cmap_names_multi_sequential = (
     "oleron",
     "bukavu",
     "fes",
 )
 
-_cmap_base_names_categorical = tuple(
-    name for name in _cmap_names_sequential if name not in {"batlowW", "batlowK"}
-)
+_cmap_base_names_categorical = tuple(_cmap_names_sequential)
 _cmap_names_categorical = tuple(f"{name}S" for name in _cmap_base_names_categorical)
 
 _cmap_base_names_cyclic = (
     "roma",
     "bam",
     "broc",
     "cork",
```

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/acton.txt` & `cmcrameri-1.7/cmcrameri/cmaps/acton.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/actonS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/actonS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bam.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bam.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bamO.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bamO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bamako.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bamako.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bamakoS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bamakoS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/batlow.txt` & `cmcrameri-1.7/cmcrameri/cmaps/batlow.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/batlowK.txt` & `cmcrameri-1.7/cmcrameri/cmaps/batlowK.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/batlowS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/batlowS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/batlowW.txt` & `cmcrameri-1.7/cmcrameri/cmaps/batlowW.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/berlin.txt` & `cmcrameri-1.7/cmcrameri/cmaps/berlin.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bilbao.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bilbao.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bilbaoS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bilbaoS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/broc.txt` & `cmcrameri-1.7/cmcrameri/cmaps/broc.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/brocO.txt` & `cmcrameri-1.7/cmcrameri/cmaps/brocO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/buda.txt` & `cmcrameri-1.7/cmcrameri/cmaps/buda.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/budaS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/budaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/bukavu.txt` & `cmcrameri-1.7/cmcrameri/cmaps/bukavu.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/cork.txt` & `cmcrameri-1.7/cmcrameri/cmaps/cork.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/corkO.txt` & `cmcrameri-1.7/cmcrameri/cmaps/corkO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/davos.txt` & `cmcrameri-1.7/cmcrameri/cmaps/davos.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/davosS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/davosS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/devon.txt` & `cmcrameri-1.7/cmcrameri/cmaps/devon.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/devonS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/devonS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/fes.txt` & `cmcrameri-1.7/cmcrameri/cmaps/fes.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/glasgow.txt` & `cmcrameri-1.7/cmcrameri/cmaps/glasgow.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/grayC.txt` & `cmcrameri-1.7/cmcrameri/cmaps/grayC.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/grayCS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/grayCS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/hawaii.txt` & `cmcrameri-1.7/cmcrameri/cmaps/hawaii.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/hawaiiS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/hawaiiS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/imola.txt` & `cmcrameri-1.7/cmcrameri/cmaps/imola.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/imolaS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/imolaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/lajolla.txt` & `cmcrameri-1.7/cmcrameri/cmaps/lajolla.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/lajollaS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/lajollaS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/lapaz.txt` & `cmcrameri-1.7/cmcrameri/cmaps/lapaz.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/lapazS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/lapazS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/lipari.txt` & `cmcrameri-1.7/cmcrameri/cmaps/lipari.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/lisbon.txt` & `cmcrameri-1.7/cmcrameri/cmaps/lisbon.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/managua.txt` & `cmcrameri-1.7/cmcrameri/cmaps/managua.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/navia.txt` & `cmcrameri-1.7/cmcrameri/cmaps/navia.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/nuuk.txt` & `cmcrameri-1.7/cmcrameri/cmaps/nuuk.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/nuukS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/nuukS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/oleron.txt` & `cmcrameri-1.7/cmcrameri/cmaps/oleron.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/oslo.txt` & `cmcrameri-1.7/cmcrameri/cmaps/oslo.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/osloS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/osloS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/roma.txt` & `cmcrameri-1.7/cmcrameri/cmaps/roma.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/romaO.txt` & `cmcrameri-1.7/cmcrameri/cmaps/romaO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/tofino.txt` & `cmcrameri-1.7/cmcrameri/cmaps/tofino.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/tokyo.txt` & `cmcrameri-1.7/cmcrameri/cmaps/tokyo.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/tokyoS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/tokyoS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/turku.txt` & `cmcrameri-1.7/cmcrameri/cmaps/turku.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/turkuS.txt` & `cmcrameri-1.7/cmcrameri/cmaps/turkuS.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/vanimo.txt` & `cmcrameri-1.7/cmcrameri/cmaps/vanimo.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/vik.txt` & `cmcrameri-1.7/cmcrameri/cmaps/vik.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/cmaps/vikO.txt` & `cmcrameri-1.7/cmcrameri/cmaps/vikO.txt`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri/colormaps.png` & `cmcrameri-1.7/cmcrameri/colormaps.png`

 * *Files identical despite different names*

### Comparing `cmcrameri-1.6/cmcrameri.egg-info/SOURCES.txt` & `cmcrameri-1.7/cmcrameri.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 cmcrameri/cmaps/actonS.txt
 cmcrameri/cmaps/bam.txt
 cmcrameri/cmaps/bamO.txt
 cmcrameri/cmaps/bamako.txt
 cmcrameri/cmaps/bamakoS.txt
 cmcrameri/cmaps/batlow.txt
 cmcrameri/cmaps/batlowK.txt
+cmcrameri/cmaps/batlowKS.txt
 cmcrameri/cmaps/batlowS.txt
 cmcrameri/cmaps/batlowW.txt
+cmcrameri/cmaps/batlowWS.txt
 cmcrameri/cmaps/berlin.txt
 cmcrameri/cmaps/bilbao.txt
 cmcrameri/cmaps/bilbaoS.txt
 cmcrameri/cmaps/broc.txt
 cmcrameri/cmaps/brocO.txt
 cmcrameri/cmaps/buda.txt
 cmcrameri/cmaps/budaS.txt
@@ -37,28 +39,31 @@
 cmcrameri/cmaps/corkO.txt
 cmcrameri/cmaps/davos.txt
 cmcrameri/cmaps/davosS.txt
 cmcrameri/cmaps/devon.txt
 cmcrameri/cmaps/devonS.txt
 cmcrameri/cmaps/fes.txt
 cmcrameri/cmaps/glasgow.txt
+cmcrameri/cmaps/glasgowS.txt
 cmcrameri/cmaps/grayC.txt
 cmcrameri/cmaps/grayCS.txt
 cmcrameri/cmaps/hawaii.txt
 cmcrameri/cmaps/hawaiiS.txt
 cmcrameri/cmaps/imola.txt
 cmcrameri/cmaps/imolaS.txt
 cmcrameri/cmaps/lajolla.txt
 cmcrameri/cmaps/lajollaS.txt
 cmcrameri/cmaps/lapaz.txt
 cmcrameri/cmaps/lapazS.txt
 cmcrameri/cmaps/lipari.txt
+cmcrameri/cmaps/lipariS.txt
 cmcrameri/cmaps/lisbon.txt
 cmcrameri/cmaps/managua.txt
 cmcrameri/cmaps/navia.txt
+cmcrameri/cmaps/naviaS.txt
 cmcrameri/cmaps/nuuk.txt
 cmcrameri/cmaps/nuukS.txt
 cmcrameri/cmaps/oleron.txt
 cmcrameri/cmaps/oslo.txt
 cmcrameri/cmaps/osloS.txt
 cmcrameri/cmaps/roma.txt
 cmcrameri/cmaps/romaO.txt
```

### Comparing `cmcrameri-1.6/pyproject.toml` & `cmcrameri-1.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 description = "Perceptually uniform colormaps by Fabio Crameri"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Callum Rollo", email = "c.rollo@outlook.com"},
 ]
 requires-python = ">=3.6"
+classifiers = [
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.6",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+]
 dynamic = [
   "version",
 ]
 dependencies = [
   "matplotlib",
   "numpy",
   "packaging",
```

