# Comparing `tmp/devops_trabalho-0.0.1.tar.gz` & `tmp/devops_trabalho-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devops_trabalho-0.0.1.tar", last modified: Mon Jul 10 03:34:37 2023, max compression
+gzip compressed data, was "devops_trabalho-0.0.4.tar", last modified: Mon Jul 10 04:35:42 2023, max compression
```

## Comparing `devops_trabalho-0.0.1.tar` & `devops_trabalho-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 03:34:37.468414 devops_trabalho-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-07-08 04:28:04.000000 devops_trabalho-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      556 2023-07-10 03:34:37.467411 devops_trabalho-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-07-08 04:14:04.000000 devops_trabalho-0.0.1/README.md
--rw-rw-rw-   0        0        0      700 2023-07-10 03:31:42.000000 devops_trabalho-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       61 2023-07-10 03:32:34.000000 devops_trabalho-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 03:34:37.469424 devops_trabalho-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 03:34:37.366413 devops_trabalho-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 03:34:37.452415 devops_trabalho-0.0.1/src/devops_trabalho.egg-info/
--rw-rw-rw-   0        0        0      556 2023-07-10 03:34:37.000000 devops_trabalho-0.0.1/src/devops_trabalho.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-10 03:34:37.000000 devops_trabalho-0.0.1/src/devops_trabalho.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 03:34:37.000000 devops_trabalho-0.0.1/src/devops_trabalho.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-10 03:34:37.000000 devops_trabalho-0.0.1/src/devops_trabalho.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-10 03:34:37.000000 devops_trabalho-0.0.1/src/devops_trabalho.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 03:34:37.459410 devops_trabalho-0.0.1/src/stringstandard/
--rw-rw-rw-   0        0        0        0 2023-07-08 14:13:07.000000 devops_trabalho-0.0.1/src/stringstandard/__init__.py
--rw-rw-rw-   0        0        0      162 2023-07-08 15:40:44.000000 devops_trabalho-0.0.1/src/stringstandard/stringstd.py
-drwxrwxrwx   0        0        0        0 2023-07-10 03:34:37.463414 devops_trabalho-0.0.1/test/
--rw-rw-rw-   0        0        0      177 2023-07-08 17:44:05.000000 devops_trabalho-0.0.1/test/test_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/src/devops_trabalho.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 04:35:42.000000 devops_trabalho-0.0.4/src/devops_trabalho.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 04:35:42.000000 devops_trabalho-0.0.4/src/devops_trabalho.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:35:42.000000 devops_trabalho-0.0.4/src/devops_trabalho.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 04:35:42.000000 devops_trabalho-0.0.4/src/devops_trabalho.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 04:35:42.000000 devops_trabalho-0.0.4/src/devops_trabalho.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/src/stringstandard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/src/stringstandard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/src/stringstandard/stringstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:35:42.709856 devops_trabalho-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-10 04:35:30.000000 devops_trabalho-0.0.4/test/test_string.py
```

