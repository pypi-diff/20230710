# Comparing `tmp/clize-5.0.1.tar.gz` & `tmp/clize-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clize-5.0.1.tar", last modified: Fri Jul  7 06:53:52 2023, max compression
+gzip compressed data, was "clize-5.0.2.tar", last modified: Sun Jul  9 22:54:35 2023, max compression
```

## Comparing `clize-5.0.1.tar` & `clize-5.0.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.369161 clize-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 06:53:43.000000 clize-5.0.1/.bzrignore
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-07 06:53:43.000000 clize-5.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.353161 clize-5.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.357161 clize-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-07 06:53:43.000000 clize-5.0.1/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-07 06:53:43.000000 clize-5.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 06:53:43.000000 clize-5.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 06:53:43.000000 clize-5.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-07 06:53:43.000000 clize-5.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-07 06:53:43.000000 clize-5.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 06:53:43.000000 clize-5.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-07 06:53:43.000000 clize-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-07 06:53:52.369161 clize-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-07 06:53:43.000000 clize-5.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.357161 clize-5.0.1/clize/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 06:53:43.000000 clize-5.0.1/clize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-07 06:53:43.000000 clize-5.0.1/clize/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-07 06:53:43.000000 clize-5.0.1/clize/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-07 06:53:43.000000 clize-5.0.1/clize/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-07-07 06:53:43.000000 clize-5.0.1/clize/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-07 06:53:43.000000 clize-5.0.1/clize/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-07-07 06:53:43.000000 clize-5.0.1/clize/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    49704 2023-07-07 06:53:43.000000 clize-5.0.1/clize/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-07 06:53:43.000000 clize-5.0.1/clize/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.361161 clize-5.0.1/clize/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    58088 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_legacy_py3k.py
--rw-r--r--   0 runner    (1001) docker     (123)    26151 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    34022 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23083 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-07 06:53:43.000000 clize-5.0.1/clize/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-07-07 06:53:43.000000 clize-5.0.1/clize/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.357161 clize-5.0.1/clize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 06:53:52.000000 clize-5.0.1/clize.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.365161 clize-5.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-07 06:53:43.000000 clize-5.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.365161 clize-5.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 06:53:43.000000 clize-5.0.1/docs/_static/clize_style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.365161 clize-5.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-07 06:53:43.000000 clize-5.0.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-07-07 06:53:43.000000 clize-5.0.1/docs/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 06:53:43.000000 clize-5.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-07 06:53:43.000000 clize-5.0.1/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-07 06:53:43.000000 clize-5.0.1/docs/compositing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-07 06:53:43.000000 clize-5.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-07 06:53:43.000000 clize-5.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-07 06:53:43.000000 clize-5.0.1/docs/dispatching.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-07 06:53:43.000000 clize-5.0.1/docs/docstring-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-07 06:53:43.000000 clize-5.0.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-07 06:53:43.000000 clize-5.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-07 06:53:43.000000 clize-5.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-07 06:53:43.000000 clize-5.0.1/docs/interop.rst
--rw-r--r--   0 runner    (1001) docker     (123)  1242077 2023-07-07 06:53:43.000000 clize-5.0.1/docs/json
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-07 06:53:43.000000 clize-5.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-07 06:53:43.000000 clize-5.0.1/docs/parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-07 06:53:43.000000 clize-5.0.1/docs/porting.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-07-07 06:53:43.000000 clize-5.0.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-07-07 06:53:43.000000 clize-5.0.1/docs/releases.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-07 06:53:43.000000 clize-5.0.1/docs/why.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:52.369161 clize-5.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-07 06:53:43.000000 clize-5.0.1/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:53:43.000000 clize-5.0.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-07 06:53:43.000000 clize-5.0.1/examples/altcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 06:53:43.000000 clize-5.0.1/examples/argdeco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-07 06:53:43.000000 clize-5.0.1/examples/bfparam.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-07 06:53:43.000000 clize-5.0.1/examples/deco_add_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-07 06:53:43.000000 clize-5.0.1/examples/deco_provide_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 06:53:43.000000 clize-5.0.1/examples/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 06:53:43.000000 clize-5.0.1/examples/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-07 06:53:43.000000 clize-5.0.1/examples/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-07 06:53:43.000000 clize-5.0.1/examples/interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 06:53:43.000000 clize-5.0.1/examples/logparam.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-07 06:53:43.000000 clize-5.0.1/examples/mapped.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 06:53:43.000000 clize-5.0.1/examples/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-07 06:53:43.000000 clize-5.0.1/examples/multicommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-07 06:53:43.000000 clize-5.0.1/examples/naval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-07 06:53:43.000000 clize-5.0.1/examples/typed_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-07 06:53:43.000000 clize-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 06:53:52.369161 clize-5.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2061 2023-07-07 06:53:43.000000 clize-5.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 06:53:43.000000 clize-5.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.935359 clize-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-09 22:54:22.000000 clize-5.0.2/.bzrignore
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 22:54:22.000000 clize-5.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.919358 clize-5.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.919358 clize-5.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-09 22:54:22.000000 clize-5.0.2/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-09 22:54:22.000000 clize-5.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-09 22:54:22.000000 clize-5.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-09 22:54:22.000000 clize-5.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-09 22:54:22.000000 clize-5.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-09 22:54:22.000000 clize-5.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 22:54:22.000000 clize-5.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-09 22:54:22.000000 clize-5.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-09 22:54:35.935359 clize-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-09 22:54:22.000000 clize-5.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.923359 clize-5.0.2/clize/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-09 22:54:22.000000 clize-5.0.2/clize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-09 22:54:22.000000 clize-5.0.2/clize/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-09 22:54:22.000000 clize-5.0.2/clize/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-09 22:54:22.000000 clize-5.0.2/clize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-07-09 22:54:22.000000 clize-5.0.2/clize/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-09 22:54:22.000000 clize-5.0.2/clize/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-07-09 22:54:22.000000 clize-5.0.2/clize/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49704 2023-07-09 22:54:22.000000 clize-5.0.2/clize/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-07-09 22:54:22.000000 clize-5.0.2/clize/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.927358 clize-5.0.2/clize/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58088 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_legacy_py3k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26151 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34022 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23412 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-09 22:54:22.000000 clize-5.0.2/clize/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-07-09 22:54:22.000000 clize-5.0.2/clize/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.923359 clize-5.0.2/clize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-09 22:54:35.000000 clize-5.0.2/clize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 22:54:35.000000 clize-5.0.2/clize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:54:35.000000 clize-5.0.2/clize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-09 22:54:35.000000 clize-5.0.2/clize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 22:54:35.000000 clize-5.0.2/clize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.931359 clize-5.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-09 22:54:22.000000 clize-5.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.931359 clize-5.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-09 22:54:22.000000 clize-5.0.2/docs/_static/clize_style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.931359 clize-5.0.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-09 22:54:22.000000 clize-5.0.2/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-07-09 22:54:22.000000 clize-5.0.2/docs/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-09 22:54:22.000000 clize-5.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-09 22:54:22.000000 clize-5.0.2/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-09 22:54:22.000000 clize-5.0.2/docs/compositing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-09 22:54:22.000000 clize-5.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-09 22:54:22.000000 clize-5.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-09 22:54:22.000000 clize-5.0.2/docs/dispatching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-09 22:54:22.000000 clize-5.0.2/docs/docstring-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-09 22:54:22.000000 clize-5.0.2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-09 22:54:22.000000 clize-5.0.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-09 22:54:22.000000 clize-5.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-09 22:54:22.000000 clize-5.0.2/docs/interop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1242077 2023-07-09 22:54:22.000000 clize-5.0.2/docs/json
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-09 22:54:22.000000 clize-5.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-09 22:54:22.000000 clize-5.0.2/docs/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-09 22:54:22.000000 clize-5.0.2/docs/porting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-07-09 22:54:22.000000 clize-5.0.2/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-07-09 22:54:22.000000 clize-5.0.2/docs/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-09 22:54:22.000000 clize-5.0.2/docs/why.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:35.935359 clize-5.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-09 22:54:22.000000 clize-5.0.2/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:54:22.000000 clize-5.0.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-09 22:54:22.000000 clize-5.0.2/examples/altcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-09 22:54:22.000000 clize-5.0.2/examples/argdeco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-09 22:54:22.000000 clize-5.0.2/examples/bfparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-09 22:54:22.000000 clize-5.0.2/examples/deco_add_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-09 22:54:22.000000 clize-5.0.2/examples/deco_provide_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-09 22:54:22.000000 clize-5.0.2/examples/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-09 22:54:22.000000 clize-5.0.2/examples/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-09 22:54:22.000000 clize-5.0.2/examples/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-09 22:54:22.000000 clize-5.0.2/examples/interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-09 22:54:22.000000 clize-5.0.2/examples/logparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 22:54:22.000000 clize-5.0.2/examples/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-09 22:54:22.000000 clize-5.0.2/examples/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-09 22:54:22.000000 clize-5.0.2/examples/multicommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-09 22:54:22.000000 clize-5.0.2/examples/naval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-09 22:54:22.000000 clize-5.0.2/examples/typed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-09 22:54:22.000000 clize-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-09 22:54:35.935359 clize-5.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2061 2023-07-09 22:54:22.000000 clize-5.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-09 22:54:22.000000 clize-5.0.2/tox.ini
```

### Comparing `clize-5.0.1/.github/workflows/ci.yml` & `clize-5.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/AUTHORS` & `clize-5.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/COPYING` & `clize-5.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/LICENSE.txt` & `clize-5.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/PKG-INFO` & `clize-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clize
-Version: 5.0.1
+Version: 5.0.2
 Summary: Turn functions into command-line interfaces
 Home-page: https://github.com/epsy/clize
 Author: Yann Kaiser
 Author-email: kaiser.yann@gmail.com
 License: MIT
 Keywords: CLI,options,arguments,getopts,getopt,argparse,introspection,flags,decorator,subcommands
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `clize-5.0.1/README.rst` & `clize-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/__init__.py` & `clize-5.0.2/clize/__init__.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/_sphinx.py` & `clize-5.0.2/clize/_sphinx.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/converters.py` & `clize-5.0.2/clize/converters.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/errors.py` & `clize-5.0.2/clize/errors.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/help.py` & `clize-5.0.2/clize/help.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/legacy.py` & `clize-5.0.2/clize/legacy.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/parameters.py` & `clize-5.0.2/clize/parameters.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/parser.py` & `clize-5.0.2/clize/parser.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/runner.py` & `clize-5.0.2/clize/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,35 @@
     def __new__(cls, fn=None, **kwargs):
         if fn is None:
             return partial(cls, **kwargs)
         else:
             return super(Clize, cls).__new__(cls)
 
     def __init__(self, fn, owner=None, alt=(), extra=(),
-                 help_names=('help', 'h'), helper_class=None, hide_help=False):
+                 help_names=('help', 'h'), helper_class=None, hide_help=False,
+                 description=None,
+                 ):
         """
         :param sequence alt: Alternate actions the CLI will handle.
         :param help_names: Names to use to trigger the help.
         :type help_names: sequence of strings
         :param helper_class: A callable to produce a helper object to be
             used when the help is triggered. If unset, uses `.ClizeHelp`.
         :type helper_class: a type like `.ClizeHelp`
         :param bool hide_help: Mark the parameters used to trigger the help
             as undocumented.
         """
+        if description:
+            raise TypeError(
+                "description= is only accepted when using multiple same-level commands. "
+                "When only one main command is given, "
+                "you can set the description by updating the main command's docstring. See "
+                "https://clize.readthedocs.io/en/stable/basics.html#enhancing-the-help-message "
+                "for more information."
+            )
         update_wrapper(self, fn)
         self.func = fn
         self.owner = owner
         self.alt = util.dict_from_names(alt)
         self.extra = extra
         self.help_names = help_names
         self.help_aliases = [util.name_py2cli(s, kw=True) for s in help_names]
@@ -165,26 +175,25 @@
            the object, and its `cli <.SubcommandDispatcher.cli>` method
            is used.
 
         Most notably, `clize.run` uses this class method in order to interpret
         the given object(s).
         """
         try:
-            cli = obj.cli
+            return obj.cli
         except AttributeError:
-            if callable(obj):
-                cli = cls(obj, **kwargs)
-            else:
-                try:
-                    iter(obj)
-                except TypeError:
-                    raise TypeError("Don't know how to build a cli for "
-                                    + repr(obj))
-                cli = SubcommandDispatcher(obj, **kwargs).cli
-        return cli
+            pass
+        if callable(obj):
+            return cls(obj, **kwargs)
+        else:
+            try:
+                iter(obj)
+            except TypeError:
+                raise TypeError(f"Don't know how to build a cli for {obj!r}") from None
+            return SubcommandDispatcher(obj, **kwargs).cli
 
     @property
     def cli(self):
         """Returns the object itself, in order to be selected by `.get_cli`"""
         return self
 
     def __repr__(self):
```

### Comparing `clize-5.0.1/clize/tests/test_converters.py` & `clize-5.0.2/clize/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_help.py` & `clize-5.0.2/clize/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_legacy.py` & `clize-5.0.2/clize/tests/test_legacy.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_legacy_py3k.py` & `clize-5.0.2/clize/tests/test_legacy_py3k.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_parameters.py` & `clize-5.0.2/clize/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_parser.py` & `clize-5.0.2/clize/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_runner.py` & `clize-5.0.2/clize/tests/test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,21 @@
             })
         repr(ru)
         sd = ru.func.__self__
         self.assertTrue(isinstance(sd,
                                    runner.SubcommandDispatcher))
         self.assertEqual(set(sd.cmds_by_name), set(['2', '3']))
 
+    def test_deny_description_on_single(self):
+        def base(): raise NotImplementedError
+        def alt(): raise NotImplementedError
+        with self.assertRaises(TypeError) as cm:
+            runner.Clize.get_cli(base, alt=alt, description="not allowed")
+        self.assertIn("only one main command", str(cm.exception))
+
     def test_as_is(self):
         def func(): raise NotImplementedError
         ru = runner.Clize.get_cli(runner.Clize.as_is(func))
         repr(ru)
         self.assertEqual(ru, func)
 
     def test_as_is_desc(self):
```

### Comparing `clize-5.0.1/clize/tests/test_testutil.py` & `clize-5.0.2/clize/tests/test_testutil.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/test_util.py` & `clize-5.0.2/clize/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/tests/util.py` & `clize-5.0.2/clize/tests/util.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize/util.py` & `clize-5.0.2/clize/util.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/clize.egg-info/PKG-INFO` & `clize-5.0.2/clize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clize
-Version: 5.0.1
+Version: 5.0.2
 Summary: Turn functions into command-line interfaces
 Home-page: https://github.com/epsy/clize
 Author: Yann Kaiser
 Author-email: kaiser.yann@gmail.com
 License: MIT
 Keywords: CLI,options,arguments,getopts,getopt,argparse,introspection,flags,decorator,subcommands
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `clize-5.0.1/clize.egg-info/SOURCES.txt` & `clize-5.0.2/clize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/Makefile` & `clize-5.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/alternatives.rst` & `clize-5.0.2/docs/alternatives.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/api.rst` & `clize-5.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/basics.rst` & `clize-5.0.2/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/compositing.rst` & `clize-5.0.2/docs/compositing.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/conf.py` & `clize-5.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/contributing.rst` & `clize-5.0.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/dispatching.rst` & `clize-5.0.2/docs/dispatching.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/docstring-reference.rst` & `clize-5.0.2/docs/docstring-reference.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/faq.rst` & `clize-5.0.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/history.rst` & `clize-5.0.2/docs/history.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/index.rst` & `clize-5.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/interop.rst` & `clize-5.0.2/docs/interop.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/json` & `clize-5.0.2/docs/json`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/make.bat` & `clize-5.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/parser.rst` & `clize-5.0.2/docs/parser.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/porting.rst` & `clize-5.0.2/docs/porting.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/reference.rst` & `clize-5.0.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/releases.rst` & `clize-5.0.2/docs/releases.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/docs/why.rst` & `clize-5.0.2/docs/why.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/README.rst` & `clize-5.0.2/examples/README.rst`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/argdeco.py` & `clize-5.0.2/examples/argdeco.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/bfparam.py` & `clize-5.0.2/examples/bfparam.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/deco_add_param.py` & `clize-5.0.2/examples/deco_add_param.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/deco_provide_arg.py` & `clize-5.0.2/examples/deco_provide_arg.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/echo.py` & `clize-5.0.2/examples/echo.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/interop.py` & `clize-5.0.2/examples/interop.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/logparam.py` & `clize-5.0.2/examples/logparam.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/naval.py` & `clize-5.0.2/examples/naval.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/examples/typed_cli.py` & `clize-5.0.2/examples/typed_cli.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/setup.py` & `clize-5.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `clize-5.0.1/tox.ini` & `clize-5.0.2/tox.ini`

 * *Files identical despite different names*

