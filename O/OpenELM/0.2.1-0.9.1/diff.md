# Comparing `tmp/OpenELM-0.2.1.tar.gz` & `tmp/OpenELM-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenELM-0.2.1.tar", last modified: Wed Mar  8 01:48:37 2023, max compression
+gzip compressed data, was "OpenELM-0.9.1.tar", last modified: Mon Jul 10 19:36:48 2023, max compression
```

## Comparing `OpenELM-0.2.1.tar` & `OpenELM-0.9.1.tar`

### file list

```diff
@@ -1,137 +1,311 @@
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:36.000000 OpenELM-0.2.1/.github/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      834 2023-01-20 14:24:40.000000 OpenELM-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      595 2023-01-20 14:24:40.000000 OpenELM-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/.github/workflows/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-02-17 21:08:09.000000 OpenELM-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1919 2023-03-08 01:31:49.000000 OpenELM-0.2.1/.gitignore
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1162 2023-02-17 21:08:09.000000 OpenELM-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      686 2023-02-17 21:08:09.000000 OpenELM-0.2.1/.readthedocs.yml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      840 2023-02-17 21:08:09.000000 OpenELM-0.2.1/CITATION.cff
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5220 2023-01-20 14:24:40.000000 OpenELM-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3812 2023-01-20 14:24:40.000000 OpenELM-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1065 2023-01-20 14:24:40.000000 OpenELM-0.2.1/LICENSE
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4556 2023-03-08 01:48:37.000000 OpenELM-0.2.1/PKG-INFO
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3492 2023-02-17 21:08:09.000000 OpenELM-0.2.1/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/docs/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      638 2023-01-20 14:24:40.000000 OpenELM-0.2.1/docs/Makefile
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      804 2023-01-20 14:24:40.000000 OpenELM-0.2.1/docs/make.bat
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/docs/source/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2814 2023-02-17 21:08:09.000000 OpenELM-0.2.1/docs/source/conf.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/docs/source/images/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1150 2023-01-20 14:24:40.000000 OpenELM-0.2.1/docs/source/images/openelm_favicon.ico
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      448 2023-01-20 14:24:40.000000 OpenELM-0.2.1/docs/source/index.rst
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      267 2023-01-20 14:24:40.000000 OpenELM-0.2.1/docs/source/openelm.environments.rst
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      657 2023-01-20 14:24:40.000000 OpenELM-0.2.1/docs/source/openelm.rst
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2132 2023-03-08 01:48:30.000000 OpenELM-0.2.1/pyproject.toml
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      123 2023-01-28 16:16:16.000000 OpenELM-0.2.1/requirements.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      900 2023-03-08 01:31:49.000000 OpenELM-0.2.1/run_elm.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6590 2023-03-08 01:31:49.000000 OpenELM-0.2.1/run_p3.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       38 2023-03-08 01:48:37.000000 OpenELM-0.2.1/setup.cfg
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/OpenELM.egg-info/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4556 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/OpenELM.egg-info/PKG-INFO
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3921 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/OpenELM.egg-info/SOURCES.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        1 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/OpenELM.egg-info/dependency_links.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      387 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/OpenELM.egg-info/requires.txt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        8 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/OpenELM.egg-info/top_level.txt
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      152 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/benchmarks/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/benchmarks/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8366 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/benchmarks/benchmark_bugs.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9375 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/benchmarks/benchmark_crossover.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1538 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/benchmarks/benchmark_lm_speed.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1552 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/benchmarks/benchmark_sodarace_parallel.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12530 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/benchmarks/benchmark_tinygp.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2590 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/benchmarks/benchmarks_triton.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/codegen/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      147 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6269 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/codegen_triton.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4709 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/codegen/codegen_utilities.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2726 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/codegen/configuration_codegen.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28547 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/codegen/modelling_codegen.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3404 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/codegen_gptj_converter.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3705 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/config_template.pbtxt
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4127 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/convert_ft.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7460 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/gptj_ftconverter.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/readme.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      270 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/codegen/triton_utils/triton_start.sh
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3992 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/configs.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      166 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/constants.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2158 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/elm.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/environments/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2684 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/environments/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      603 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/environments/env_utils.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    22415 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/environments/environments.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1063 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/README.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6795 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55082 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/_framework_simulator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3346 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/helpers.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    25674 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/simulator.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      544 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/CPPN_fixed.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1267 2023-02-03 22:41:04.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/CPPN_mutable.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1099 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/README.md
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      214 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1284 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/galloper.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      918 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/radial.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      590 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/runner.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      957 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/square.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3085 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/walk_creator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      889 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/wheel.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11288 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/map_elites.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4101 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/mutation_model.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/sandbox/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      406 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/Dockerfile
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      162 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/Pipfile
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9266 2023-02-04 21:59:34.000000 OpenELM-0.2.1/src/openelm/sandbox/Pipfile.lock
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      931 2023-02-17 21:08:09.000000 OpenELM-0.2.1/src/openelm/sandbox/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/sandbox/scripts/
--rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       85 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/scripts/bootstrap.sh
--rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       33 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/scripts/build.sh
--rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)      107 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/scripts/launch.sh
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/sandbox/server/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/server/__init__.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:36.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      496 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/CPPN_fixed.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1230 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       71 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      881 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/radial.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      933 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/square.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2975 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/walk_creator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3625 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/sandbox/server/index.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10008 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/sandbox/server/sandbox_codex_execute.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/sandbox/server/templates/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-01-20 14:24:40.000000 OpenELM-0.2.1/src/openelm/sandbox/server/templates/index.html
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/src/openelm/utils/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      338 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/utils/__init__.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6124 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/utils/code_eval.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13343 2023-02-17 21:08:10.000000 OpenELM-0.2.1/src/openelm/utils/diff_eval.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      684 2023-03-08 01:31:49.000000 OpenELM-0.2.1/src/openelm/utils/utils.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/tests/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      849 2023-03-08 01:31:49.000000 OpenELM-0.2.1/tests/__test_mapelites.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      442 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/conftest.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1762 2023-03-08 01:31:49.000000 OpenELM-0.2.1/tests/test_code_execute.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/tests/test_data/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15732 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/test_data/cppn_fixed.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2604 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/test_data/square.json
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18081 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/test_diff.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4667 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/test_sodarace_env.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2583 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/test_sodarace_walkers.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      736 2023-02-17 21:08:10.000000 OpenELM-0.2.1/tests/test_truncate.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/trlx_example/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/README.md
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/trlx_example/configs/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2152 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/configs/ppo_softprompt_config.yml
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/trlx_example/model/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12827 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/model/accelerate_ppo_softprompt_model.py
-drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-03-08 01:48:37.000000 OpenELM-0.2.1/trlx_example/orchestrator/
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6254 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/orchestrator/ppo_softprompt_orchestrator.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1743 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/ppo_softprompt_long_completions.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1600 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/ppo_softprompt_sentiment.py
--rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1769 2023-01-20 14:24:40.000000 OpenELM-0.2.1/trlx_example/ppo_softprompt_short_completions.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/.github/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      834 2023-01-20 14:24:40.000000 OpenELM-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      595 2023-01-20 14:24:40.000000 OpenELM-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/.github/workflows/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-02-17 21:08:09.000000 OpenELM-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1919 2023-03-08 01:31:49.000000 OpenELM-0.9.1/.gitignore
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1162 2023-02-17 21:08:09.000000 OpenELM-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      686 2023-02-17 21:08:09.000000 OpenELM-0.9.1/.readthedocs.yml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      840 2023-02-17 21:08:09.000000 OpenELM-0.9.1/CITATION.cff
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5220 2023-01-20 14:24:40.000000 OpenELM-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3812 2023-01-20 14:24:40.000000 OpenELM-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1065 2023-01-20 14:24:40.000000 OpenELM-0.9.1/LICENSE
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1872346 2023-07-10 19:30:39.000000 OpenELM-0.9.1/OpenELM_Paper.pdf
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5792 2023-07-10 19:36:48.000000 OpenELM-0.9.1/PKG-INFO
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4723 2023-07-10 19:30:39.000000 OpenELM-0.9.1/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/docs/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      638 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/Makefile
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      804 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/make.bat
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/docs/source/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2814 2023-02-17 21:08:09.000000 OpenELM-0.9.1/docs/source/conf.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/docs/source/images/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1150 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/images/openelm_favicon.ico
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      448 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/index.rst
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      267 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/openelm.environments.rst
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      657 2023-01-20 14:24:40.000000 OpenELM-0.9.1/docs/source/openelm.rst
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2115 2023-07-10 19:34:59.000000 OpenELM-0.9.1/pyproject.toml
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      203 2023-07-10 19:30:39.000000 OpenELM-0.9.1/requirements.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      994 2023-07-10 19:30:39.000000 OpenELM-0.9.1/run_elm.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6298 2023-07-10 19:30:39.000000 OpenELM-0.9.1/run_p3.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       38 2023-07-10 19:36:48.000000 OpenELM-0.9.1/setup.cfg
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/OpenELM.egg-info/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5792 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/PKG-INFO
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15032 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/SOURCES.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        1 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/dependency_links.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      464 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/requires.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        8 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/OpenELM.egg-info/top_level.txt
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      152 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/algorithms/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/algorithms/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6037 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/algorithms/genetic.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    33376 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/algorithms/map_elites.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/benchmarks/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8971 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_bugs.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9429 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_crossover.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1538 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_lm_speed.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1552 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_sodarace_parallel.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12530 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmark_tinygp.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2590 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/benchmarks/benchmarks_triton.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/codegen/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      147 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6269 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/codegen_triton.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4265 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/codegen/codegen_utilities.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2726 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/codegen/configuration_codegen.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28547 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/codegen/modelling_codegen.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3404 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/codegen_gptj_converter.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3705 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/config_template.pbtxt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4127 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/convert_ft.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7460 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/gptj_ftconverter.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/readme.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      270 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/codegen/triton_utils/triton_start.sh
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6925 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/configs.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      166 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/constants.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3784 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/elm.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      118 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12516 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/base.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/p3/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6966 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/p3/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    24594 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/p3/p3.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6171 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/poetry.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      534 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      471 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      528 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      698 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      458 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      805 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      469 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      348 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      475 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      696 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      495 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      565 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      819 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      470 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      365 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      932 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      706 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      437 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      464 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      487 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      421 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      283 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      207 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1523 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/annotations/word_in_context.json
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   108445 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/addsub.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    51855 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/aqua.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   230302 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/coin_flip.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   385739 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/commonsensqa.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   103317 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/date_understanding.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   296065 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/gsm8k.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    86001 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/last_letters.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   200307 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/multiarith.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   368446 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/shuffled_objects.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   154726 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/singleeq.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   456229 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/strategyqa.csv
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   275766 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/cot_dataset/svamp.csv
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   124409 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    65651 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   159273 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   103263 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55791 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    56939 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   113139 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    72257 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    69787 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   136337 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    90713 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   102849 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    59593 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    56939 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   168475 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    99119 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63269 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    55791 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    61715 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   116251 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    64271 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63469 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    63877 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   158299 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/induction_input/word_in_context.json
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:47.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16216 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7440 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2867 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3553 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9496 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6556 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1777 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13878 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    20496 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    19956 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9973 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    28548 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    26905 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6556 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16857 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11210 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9832 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9450 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     7007 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    48523 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18183 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    17017 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16752 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    26219 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/execute/word_in_context.json
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   145630 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/active_to_passive.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   196170 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/antonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3009 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/cause_and_effect.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3944 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/common_concept.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   477101 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/diff.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   221131 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/first_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1891 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/informal_to_formal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   407339 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/larger_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   693976 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/letters_list.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   176741 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/negation.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1000548 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/num_to_verbal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   808766 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/orthography_starts_with.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1150469 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/rhymes.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   221131 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/second_word_letter.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   663715 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sentence_similarity.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   127802 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sentiment.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   194002 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/singular_to_plural.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   474622 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/sum.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   158942 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/synonyms.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1450171 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/taxonomy_animal.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   513349 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-de.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   459674 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-es.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)   471938 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/translation_en-fr.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)  1044414 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/datasets/raw/induce/word_in_context.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15671 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/prompt.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4494 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/prompt/utils.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1408 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/README.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6795 2023-07-06 23:17:33.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5450 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_draw.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11741 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/opencv_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16357 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3759 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pygame_gui.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    22633 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyglet_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    33046 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5189 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3094 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/pyqt4_gui.ui
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6770 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/backends/simple_framework.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18390 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/framework.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      103 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1226 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9332 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/app.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    15634 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/area.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4327 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/basic.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9967 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/button.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      667 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/const.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13556 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/container.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2375 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/deprecated.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     5042 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/dialog.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2620 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/document.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2630 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/form.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1127 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/group.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4684 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/input.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1840 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/keysym.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4901 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/layout.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3332 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/menus.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1049 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/misc.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      360 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/pguglobals.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       99 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/readme.txt
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4602 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/select.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11132 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/slider.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      991 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/style.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4488 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/surface.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12923 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/table.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11458 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/textarea.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    16553 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/theme.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    11434 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/pgu/gui/widget.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4196 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/box2d_examples/settings.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      722 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/environment_sandbox.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3346 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/helpers.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    25878 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/simulator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10542 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/sodarace.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      495 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/CPPN_fixed.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1267 2023-02-03 22:41:04.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/CPPN_mutable.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1099 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/README.md
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      214 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1322 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/galloper.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      923 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/radial.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      541 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/runner.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      957 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/square.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3401 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/walk_creator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      973 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/wheel.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      628 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/environments/utils.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9163 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/mutation_model.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      406 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/Dockerfile
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      162 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/Pipfile
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     9266 2023-02-04 21:59:34.000000 OpenELM-0.9.1/src/openelm/sandbox/Pipfile.lock
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      931 2023-02-17 21:08:09.000000 OpenELM-0.9.1/src/openelm/sandbox/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/
+-rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       85 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/bootstrap.sh
+-rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)       33 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/build.sh
+-rwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)      107 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/scripts/launch.sh
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/server/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)        0 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/server/__init__.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:46.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      496 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/CPPN_fixed.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1230 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)       71 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      881 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/radial.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      933 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/square.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2975 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/walk_creator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     3625 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/sandbox/server/index.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    10138 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/sandbox/server/sandbox_codex_execute.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/sandbox/server/templates/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      190 2023-01-20 14:24:40.000000 OpenELM-0.9.1/src/openelm/sandbox/server/templates/index.html
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/src/openelm/utils/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      338 2023-03-08 01:31:49.000000 OpenELM-0.9.1/src/openelm/utils/__init__.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6293 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/utils/code_eval.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    13343 2023-02-17 21:08:10.000000 OpenELM-0.9.1/src/openelm/utils/diff_eval.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      907 2023-07-10 19:30:39.000000 OpenELM-0.9.1/src/openelm/utils/utils.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/tests/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1018 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/conftest.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1762 2023-03-08 01:31:49.000000 OpenELM-0.9.1/tests/test_code_execute.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/tests/test_data/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    17990 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_data/cppn_fixed.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2532 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_data/square.json
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    18081 2023-02-17 21:08:10.000000 OpenELM-0.9.1/tests/test_diff.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     8668 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_mapelites.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     4628 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_sodarace_env.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2602 2023-07-10 19:30:39.000000 OpenELM-0.9.1/tests/test_sodarace_walkers.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)      736 2023-02-17 21:08:10.000000 OpenELM-0.9.1/tests/test_truncate.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2352 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/README.md
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/configs/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     2152 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/configs/ppo_softprompt_config.yml
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/model/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)    12827 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/model/accelerate_ppo_softprompt_model.py
+drwxr-xr-x   0 hyperion (424401733) Domain Users (424400513)        0 2023-07-10 19:36:48.000000 OpenELM-0.9.1/trlx_example/orchestrator/
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     6254 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/orchestrator/ppo_softprompt_orchestrator.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1743 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/ppo_softprompt_long_completions.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1600 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/ppo_softprompt_sentiment.py
+-rw-r--r--   0 hyperion (424401733) Domain Users (424400513)     1769 2023-01-20 14:24:40.000000 OpenELM-0.9.1/trlx_example/ppo_softprompt_short_completions.py
```

### Comparing `OpenELM-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `OpenELM-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `OpenELM-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/.github/workflows/build.yml` & `OpenELM-0.9.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/.gitignore` & `OpenELM-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/.pre-commit-config.yaml` & `OpenELM-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/.readthedocs.yml` & `OpenELM-0.9.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/CITATION.cff` & `OpenELM-0.9.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/CODE_OF_CONDUCT.md` & `OpenELM-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/CONTRIBUTING.md` & `OpenELM-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/LICENSE` & `OpenELM-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/docs/Makefile` & `OpenELM-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/docs/make.bat` & `OpenELM-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/docs/source/conf.py` & `OpenELM-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/docs/source/images/openelm_favicon.ico` & `OpenELM-0.9.1/docs/source/images/openelm_favicon.ico`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/docs/source/openelm.rst` & `OpenELM-0.9.1/docs/source/openelm.rst`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/pyproject.toml` & `OpenELM-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 [project]
 name = "OpenELM"
 description = "Evolution Through Large Models"
 authors = [{name = "CarperAI"}]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
-version = "0.2.1"
-dynamic = ["dependencies"]
+dynamic = ["version", "dependencies"]
 classifiers=[
     # Trove classifiers
     # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
@@ -79,14 +78,12 @@
     "openai",
 ]
 docs = [
     "sphinx==5.3.0",
     "sphinx_rtd_theme",
     "sphinx_autodoc_typehints",
 ]
-trlx = [
-    "instruct-goose",
-]
 triton = [
     "tritonclient[all]",
 ]
 notebook = ["ipython"]
+sodaracer = ["pygame"]
```

### Comparing `OpenELM-0.2.1/src/openelm/benchmarks/benchmark_bugs.py` & `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_bugs.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,116 +9,124 @@
 import torch
 from hydra.core.config_store import ConfigStore
 from omegaconf import OmegaConf
 from tqdm import tqdm, trange
 
 from openelm.codegen import model_setup, sample, truncate
 from openelm.configs import BaseConfig
+from openelm.sandbox.server.sandbox_codex_execute import ExecResult
 from openelm.utils import apply_diff, eval_completions, mutate_code, split_diff
 
+os.environ["TRANSFORMERS_CACHE"] = "/fsx/hyperion/hf_cache"
+
 
 @dataclass
 class BenchmarkBugsConfig(BaseConfig):
     hydra: Any = field(
         default_factory=lambda: {
             "run": {"dir": "logs/benchmarks/bugs/${hydra.job.override_dirname}"}
         }
     )
-    model: str = "Salesforce/codegen-2B-mono"
+    model_path: str = "CarperAI/diff-codegen-2b-v2"
     bugs_data_path: str = "/fsx/shared/diff_benchmark.json"
-    mode: str = "prompt"
+    mode: str = "diff"
     seed: Optional[int] = None
     deterministic: bool = False
     fp16: bool = True
     cuda: bool = True
     debug: bool = False
     gpus: int = 1
     processes: int = 12
     temp: float = 0.8
     top_p: float = 0.95
-    gen_max_len: int = 512
+    gen_max_len: int = 256
     batch_size: int = 32
-    n_trials: int = 3200
+    n_trials: int = 500
     n_bugs_trials: int = 100
     timeout: float = 5.0
     verbose: bool = True
     tasks: list[str] = field(default_factory=lambda: ["parity"])
-    n_bugs: list[int] = field(default_factory=lambda: [1, 2, 3, 4, 5])
-    temp_samples: list[float] = field(default_factory=lambda: [0.7, 0.8, 0.9])
+    n_bugs: list[int] = field(default_factory=lambda: [1])
+    temp_samples: list[float] = field(default_factory=lambda: [0.8])
     sweep: bool = False
 
 
 class BenchmarkBugs:
     def __init__(self, cfg: BenchmarkBugsConfig):
         self.cfg: BenchmarkBugsConfig = cfg
 
         os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
         self.device = torch.device("cuda")
         self.model, self.tokenizer, self.device = model_setup(cfg, self.device)
+        print("Number of parameters:", self.model.num_parameters())
 
     def benchmark_parity(self, n_bugs, **kwargs):
         mutated_str, function_str = mutate_code(
             n_bugs=n_bugs, task="parity", mutate_method=self.cfg.mode
         )
+        print(mutated_str)
         encoding = self.tokenizer(
             [mutated_str],
             truncation=True,
             padding=True,
             return_tensors="pt",
         ).to(self.device)
         token_len: int = encoding.input_ids.shape[1]
-        sample_idx: int = token_len - 1 if self.cfg.mode == "prompt" else 0
+        sample_idx: int = token_len - 16 if self.cfg.mode == "prompt" else 0
         num_batches: int = self.cfg.n_trials // self.cfg.batch_size
         results: list = []
         end_of_diff = re.compile("\n[^ +-@]+")
         for _ in trange(
             num_batches,
             desc=f"Running {self.cfg.mode} benchmark with {n_bugs} bugs",
             disable=not self.cfg.verbose,
         ):
             completions: list[str] = sample(
                 encoding,
                 self.cfg,
                 self.model,
                 self.tokenizer,
                 starting_idx=sample_idx,
+                num_return_sequences=1,
                 **kwargs,
             )
             if self.cfg.mode == "prompt":
                 eval_results: list[str] = list(map(truncate, completions))
             elif self.cfg.mode == "diff":
                 eval_results = []
                 for text in completions:
+                    # print(text)
                     # split the diff text according to <NME>, <BEF>, <MSG>, <DFF>.
                     parsed: dict = split_diff(text)
                     # truncate the diff hunk at the first line not starting with
                     # " ", "+", "-", or "@".
                     if parsed and all(
                         (s in parsed for s in ["name", "file", "message", "diff"])
                     ):
                         diff_hunk: str = end_of_diff.split(parsed["diff"])[0]
                         # We apply diff patch loosely:
                         #   1. it ignores the line numbers;
                         #   2. it ignores invalid lines (not starting with " ",
                         #   "+" or "-" and not being "@@ ... @@").
                         eval_results.append(apply_diff(function_str, diff_hunk))
+                        # print("Patched!")
                     else:
                         # Invalid format. No patching.
                         eval_results.append(function_str)
             results.extend(
                 eval_completions(
                     eval_results,
                     task="parity",
                     timeout=self.cfg.timeout,
                     processes=self.cfg.processes,
                     debug=self.cfg.debug,
                 )
             )
-        corr_cnt = results.count(0)
+        corr_cnt = results.count(ExecResult.VALID)
         if self.cfg.verbose:
             print(f"Number of bugs: {n_bugs}\n")
             print(f"Mutated code to be fixed:\n{function_str}\n")
             print(
                 f"Result: {corr_cnt} successful completions in {self.cfg.n_trials}",
                 f"trials, {(corr_cnt / self.cfg.n_trials) * 100}%",
             )
@@ -135,44 +143,54 @@
         i = 0
         num_evaluated_bugs = 0
         for _ in trange(
             self.cfg.n_bugs_trials * 2,
             desc=f"Running {self.cfg.batch_size} trials for each bug",
             disable=not self.cfg.verbose,
         ):
-            if i == 4:
+            if len(bugs[i]["prompt"][:-6]) > 1000:
+                i += 1
                 continue
             encoding = self.tokenizer(
                 [bugs[i]["prompt"][:-6]],
                 truncation=True,
                 padding=True,
                 return_tensors="pt",
             ).to(self.device)
+            print(bugs[i]["prompt"][:-6])
             completions: list[str] = sample(
-                encoding, self.cfg, self.model, self.tokenizer, starting_idx=0, **kwargs
+                encoding,
+                self.cfg,
+                self.model,
+                self.tokenizer,
+                starting_idx=0,
+                num_return_sequences=1,
+                **kwargs,
             )
             for _, text in enumerate(completions):
                 # split the diff text according to <NME>, <BEF>, <MSG>, <DFF>.
                 parsed: dict = split_diff(text)
                 # truncate the diff hunk at the first line not starting with " ",
                 # "+", "-", or "@".
                 if parsed and all(
                     (s in parsed for s in ["name", "file", "message", "diff"])
                 ):
                     diff_hunk: str = end_of_diff.split(parsed["diff"])[0]
                     nme_idx: int = diff_hunk.find("<NME>")
                     if nme_idx != -1:
                         diff_hunk = diff_hunk[:nme_idx]
                     res: str = apply_diff(bugs[i]["prompt_code"], diff_hunk)
+                    print(res)
                     if res == bugs[i]["correct_code"]:
                         results.append(0)
                     else:
                         results.append(1)
                     num_evaluated_bugs += 1
             i += 1
+            print(i)
             if i == self.cfg.n_bugs_trials:
                 i = 500
 
         print(len(bugs))
         print(num_evaluated_bugs)
         corr_cnt = results.count(0)
         if self.cfg.verbose:
```

### Comparing `OpenELM-0.2.1/src/openelm/benchmarks/benchmark_crossover.py` & `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_crossover.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 import hydra
 import numpy as np
 import torch
 from hydra.core.config_store import ConfigStore
 from omegaconf import OmegaConf
 from tqdm import trange
 
+from openelm.algorithms.map_elites import MAPElites
 from openelm.codegen import model_setup, sample, truncate
-from openelm.configs import BaseConfig
-from openelm.environments import SQUARE_SEED
-from openelm.environments.environments import Sodarace, Sodaracer
+from openelm.configs import BaseConfig, MAPElitesConfig
 from openelm.environments.sodaracer import (
     CIRCLE,
     CPPN_FIXED,
     CPPN_MUTABLE,
     GALLOPER,
     GALLOPER_PREREQ,
     IMPORTS,
@@ -29,16 +28,16 @@
     RADIAL,
     RUNNER,
     SEEDS_DICT,
     SQUARE,
     SQUARE_PREREQ,
     WHEEL,
 )
+from openelm.environments.sodaracer.sodarace import Sodarace, Sodaracer
 from openelm.environments.sodaracer.walker import Walker
-from openelm.map_elites import MAPElites
 from openelm.utils.code_eval import pool_exec_processes
 
 INSTRUCTIONS = {
     0: "",
     1: "def make_walker():\n",
     2: "#Create a new walker by modifying the starting function above.\ndef make_walker():\n",
     3: "#Combine the ,starting programs above to make a new program.\ndef make_walker():\n",
@@ -122,20 +121,22 @@
             [prompt],
             truncation=True,
             padding=True,
             return_tensors="pt",
         ).to(self.device)
 
         sodarace_env = Sodarace(
-            seed=SQUARE_SEED,
+            seed=SEEDS_DICT["square"],
             config=self.cfg,
             diff_model=self.model,
             eval_ms=self.cfg.eval_ms,
         )
-        map_elites = MAPElites(env=sodarace_env, n_bins=12)
+        map_elites = MAPElites(
+            env=sodarace_env, config=MAPElitesConfig(map_grid_size=(12,))
+        )
 
         results: list[int] = []
         valid_fitnesses: list[float] = []
         local_scope_exec: bool = self.cfg.instruction != 0
         token_len: int = encoding.input_ids.shape[1]
         print("Benchmarking seeds: ", ", ".join(seeds))
         print(f"Prompt length: {token_len} tokens.")
```

### Comparing `OpenELM-0.2.1/src/openelm/benchmarks/benchmark_lm_speed.py` & `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_lm_speed.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/benchmarks/benchmark_sodarace_parallel.py` & `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_sodarace_parallel.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/benchmarks/benchmark_tinygp.py` & `OpenELM-0.9.1/src/openelm/benchmarks/benchmark_tinygp.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/benchmarks/benchmarks_triton.py` & `OpenELM-0.9.1/src/openelm/benchmarks/benchmarks_triton.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/codegen_triton.py` & `OpenELM-0.9.1/src/openelm/codegen/codegen_triton.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/codegen_utilities.py` & `OpenELM-0.9.1/src/openelm/codegen/codegen_utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 import os
 import random
 import re
 from typing import Optional
 
 import numpy as np
 import torch
-from transformers import AutoModelForCausalLM, AutoTokenizer
+from transformers import (
+    AutoConfig,
+    AutoModelForCausalLM,
+    AutoModelForSeq2SeqLM,
+    AutoTokenizer,
+)
 
 from openelm.configs import ModelConfig
 
 
-def set_seed(seed=None, deterministic=True) -> int:
+def set_seed(seed=None, deterministic=False) -> int:
     if seed is None:
         seed = np.random.default_rng().integers(2**32 - 1)
     random.seed(seed)
     os.environ["PYTHONHASHSEED"] = str(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     if torch.cuda.is_available():
         torch.backends.cudnn.deterministic = deterministic
         torch.backends.cudnn.benchmark = not deterministic
         # torch.use_deterministic_algorithms(deterministic)
     return seed
 
 
-def create_model(path=None, fp16=True):
-    if fp16:
-        return AutoModelForCausalLM.from_pretrained(
-            path, torch_dtype=torch.float16, low_cpu_mem_usage=True
-        )
-    else:
-        return AutoModelForCausalLM.from_pretrained(path)
-
-
 def truncate(completion: str, def_num=1, print_num=0, only_local_scope=False):
     def find_re(string, pattern, start_pos):
         m = pattern.search(string, start_pos)
         return m.start() if m else -1
 
     terminals = [
         re.compile(r, re.MULTILINE)
@@ -66,83 +62,77 @@
     if len(terminals_pos) > 0:
         return completion[: min(terminals_pos)]
     else:
         return completion
 
 
 def model_setup(cfg: ModelConfig, device=None, codegen_tokenizer: bool = True):
-    set_seed(cfg.seed, deterministic=True)
+    set_seed(cfg.seed)
     if device is None:
         device = torch.device("cuda")
-    use_fp16 = True
-    if not cfg.fp16 or device.type == "cpu":
-        use_fp16 = False
-
-    if "codegen-16B" in cfg.model_path:
-        use_fp16 = True
 
     tokenizer = AutoTokenizer.from_pretrained(cfg.model_path)
-    if codegen_tokenizer:
-        tokenizer.padding_side = "left"
-        tokenizer.pad_token = 50256
-
-    if cfg.gpus > 1:
-        model = torch.nn.DataParallel(
-            create_model(cfg.model_path, fp16=use_fp16),
-            device_ids=list(range(cfg.gpus)),
-        ).to(device)
+    # TODO: may need to check model type to determine padding
+    tokenizer.padding_side = "left"
+    tokenizer.pad_token = tokenizer.eos_token
+    if tokenizer.model_max_length > 32768:
+        tokenizer.model_max_length = 2048
+
+    tokenizer.pad_token = tokenizer.eos_token
+
+    autoconfig = AutoConfig.from_pretrained(
+        cfg.model_path, trust_remote_code=cfg.trust_remote_code
+    )
+
+    if autoconfig.model_type == "t5":
+        model_cls = AutoModelForSeq2SeqLM
     else:
-        model = create_model(cfg.model_path, fp16=use_fp16).to(device)
+        model_cls = AutoModelForCausalLM
+    model = model_cls.from_pretrained(
+        cfg.model_path,
+        torch_dtype=torch.float16 if cfg.fp16 else None,
+        low_cpu_mem_usage=cfg.fp16,
+        trust_remote_code=cfg.trust_remote_code,
+        # device_map="auto",
+    ).to(device)
+
     return model, tokenizer, device
 
 
 def sample(
     batch,
     cfg: ModelConfig,
     model,
     tokenizer,
     decode: bool = True,
     starting_idx: Optional[int] = None,
     num_return_sequences: Optional[int] = None,
-    **kwargs
+    **kwargs,
 ) -> list[str]:
     """Run a model on a batch of contexts for a particular task."""
     if num_return_sequences is None:
         num_return_sequences = cfg.batch_size
     device = kwargs.get("device", torch.device("cuda"))
     temperature = kwargs.get("temperature", cfg.temp)
     top_p = kwargs.get("top_p", cfg.top_p)
     gen_max_len = kwargs.get("gen_max_len", cfg.gen_max_len)
 
     input_ids_len = batch["input_ids"].shape[1]
     if starting_idx is None:
         starting_idx = input_ids_len
     with torch.inference_mode():
         batch = batch.to(device)
-        # TODO: num_gpus > 1
-        if cfg.gpus > 1:
-            tokens = model.module.generate(
-                **batch,
-                do_sample=True,
-                num_return_sequences=num_return_sequences,
-                temperature=temperature,
-                max_new_tokens=gen_max_len,
-                top_p=top_p,
-                pad_token_id=tokenizer.pad_token_id,
-                use_cache=True,
-            )
-        else:
-            tokens = model.generate(
-                **batch,
-                do_sample=True,
-                num_return_sequences=num_return_sequences,
-                temperature=temperature,
-                max_new_tokens=gen_max_len,
-                top_p=top_p,
-                pad_token_id=tokenizer.pad_token_id,
-                use_cache=True,
-            )
+        tokens = model.generate(
+            **batch,
+            do_sample=True,
+            num_return_sequences=num_return_sequences,
+            temperature=temperature,
+            max_new_tokens=gen_max_len,
+            top_p=top_p,
+            pad_token_id=tokenizer.pad_token_id,
+            use_cache=True,
+        )
         if decode:
             text: list[str] = tokenizer.batch_decode(tokens[:, starting_idx:, ...])
             return text
         else:
             return tokens[:, starting_idx:, ...]
```

### Comparing `OpenELM-0.2.1/src/openelm/codegen/configuration_codegen.py` & `OpenELM-0.9.1/src/openelm/codegen/configuration_codegen.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/modelling_codegen.py` & `OpenELM-0.9.1/src/openelm/codegen/modelling_codegen.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/triton_utils/codegen_gptj_converter.py` & `OpenELM-0.9.1/src/openelm/codegen/triton_utils/codegen_gptj_converter.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/triton_utils/config_template.pbtxt` & `OpenELM-0.9.1/src/openelm/codegen/triton_utils/config_template.pbtxt`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/triton_utils/convert_ft.py` & `OpenELM-0.9.1/src/openelm/codegen/triton_utils/convert_ft.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/triton_utils/gptj_ftconverter.py` & `OpenELM-0.9.1/src/openelm/codegen/triton_utils/gptj_ftconverter.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/codegen/triton_utils/readme.md` & `OpenELM-0.9.1/src/openelm/codegen/triton_utils/readme.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/environments/env_utils.py` & `OpenELM-0.9.1/src/openelm/environments/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 
 def get_image_target(name: str) -> np.ndarray:
     if name == "circle":
         target = np.zeros((32, 32, 3))
         for y in range(32):
             for x in range(32):
                 if (y - 16) ** 2 + (x - 16) ** 2 <= 100:  # a radius-10 circle
-                    target[y, x] = np.array([1, 1, 0])
+                    target[y, x] = np.array([255, 255, 0])
     else:
         raise NotImplementedError(f"Image target {name} not implemented")
     return target
 
 
 IMAGE_SEED: str = """
 def draw():
 \tpic = np.zeros((32, 32, 3))
 \tfor x in range(2, 30):
 \t\tfor y in range(2, 30):
 \t\t\tpic[x, y] = np.array([0, 0, 255])
 \treturn pic
 """
+
+NULL_SEED: str = ""
```

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/__init__.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/helpers.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/helpers.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/simulator.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,30 @@
 import math
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 from Box2D import Box2D as b2
 
+from openelm.environments.sodaracer.box2d_examples.framework import Framework, main
 from openelm.environments.sodaracer.helpers import (
     Bone,
     DistanceAccessor,
     Entity,
     Muscle,
 )
 
 
-class IESoRWorld:
+class IESoRWorld(Framework):
     """Class for the Sodarace simulation."""
 
-    def __init__(self, canvas_size: tuple[int, int] = (200, 150)):
+    name: "IESoRWorld"
+
+    def __init__(self, canvas_size: tuple[int, int] = (150, 200)):
+        # super(IESoRWorld, self).__init__()
         """
         Initialize the world.
 
         Args:
             canvas_size (tuple[int, int], optional): Size of the world canvas.
                 Defaults to (200, 150).
         """
@@ -47,32 +51,33 @@
         # keep a list of shape identifiers
         self.shape_list: list = []
         # keep a reference for every body according to IDs
         self.body_map: dict = {}
         self.bone_list: list = []
         self.muscle_list: list = []
 
-        self.gravity = b2.b2Vec2(0.0, -15.0)  # ??? Magic numbers.
+        self.gravity = b2.b2Vec2(0.0, -25.0)  # ??? Magic numbers.
         # Construct a world object, which will hold and simulate the rigid bodies.
 
+        # self.world.gravity = self.gravity
         self.world: b2.b2World = b2.b2World(self.gravity)
         self.world.autoClearForces = False
 
         self.groundBodyDef: b2.b2BodyDef = b2.b2BodyDef()
         self.groundBodyDef.type = b2.b2_staticBody
-        self.groundBodyDef.position = b2.b2Vec2(0.0, -18.0)
+        self.groundBodyDef.position = b2.b2Vec2(0.0, -100.0)
 
         # Add ground body to the world
         self.groundBody: b2.b2Body = self._add_body_to_world(
             "ground", self.groundBodyDef
         )
         # Define the ground box shape.
         self.groundBox: b2.b2PolygonShape = b2.b2PolygonShape()
         # The extents are the half-widths of the box.
-        self.groundBox.SetAsBox(350.0, 10.0)
+        self.groundBox.SetAsBox(3500.0, 10.0)
         # Add the ground fixture to the ground body.
         self._add_shape_to_body(self.groundBody, self.groundBox)
 
         self.canvas: b2.b2Vec2 = b2.b2Vec2(canvas_size[0], canvas_size[1])
 
     def get_world_json(self) -> str:
         """Generate a JSON string of the world and every entity in it."""
@@ -196,19 +201,17 @@
             # with the connections
             for muscle in self.muscle_list:
                 # Get our distance joint -- holder of physical joint info
                 distance_joint: b2.b2Joint = muscle.joint
                 # Fetch the original length of the distance joint, and add some
                 # fraction of that amount to the length, depending on the current
                 # location in the muscle cycle
-                length_calc: float = (
-                    1.0
-                    + muscle.amplitude
+                length_calc = muscle.original_length + (
+                    muscle.amplitude
                     * math.cos(self.radians + muscle.phase * 2 * math.pi)
-                    * muscle.original_length
                 )
                 # Set our length as the calculate value for this joint
                 DistanceAccessor.setLength(distance_joint, length_calc)
             # Frame rate, velocity iterations, position iterations
             self.world.Step(self.simulation_rate, 10, 10)
             # Manually clear forces when doing fixed time steps,
             # NOTE: that we disabled auto clear after step inside of the b2World
@@ -625,12 +628,16 @@
         _ = self.morphology["startX"]
         try:
             end = min(
                 [bone.joint.bodyA.position[0] for bone in self.world.bone_list]
                 + [muscle.joint.bodyA.position[0] for muscle in self.world.muscle_list]
             )
             return abs(end + self.morphology["offsetX"])
-        except Exception as e:
-            print(e)
+        except Exception:
+            # print(e)
             # print(self.world.bone_list)
             # print(self.world.muscle_list)
             return -np.inf
+
+
+if __name__ == "__main__":
+    main(IESoRWorld)
```

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/CPPN_mutable.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/CPPN_mutable.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/README.md` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/galloper.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/galloper.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     dy=0.0,
     ddr=0,
     ddc=1.6,
 ):
     wc = walker_creator()
     ends = [
         make_sensor(wc, 5 + dx, -1 + dy, ddr, ddc, 4.5),
-        make_sensor(wc, 0, -0.1, sid, 9.5, 0.03),
+        make_sensor(wc, 0, -0.1, 8.0, 9.5, 0.03),  # replace "sid" with 8.0 (from paper)
         make_sensor(wc, 5.5, -0.001, 5.0, 4.86 + 0.8, 0.07),
         make_sensor(wc, 5.5, -3.0, 6.0, 4.86 + 0.8, 0.07),
         make_sensor(wc, 0, dx, ddr, ddc, 1.0),
     ]
 
     sides = ends[0] + ends[1] + ends[2] + ends[-1] + ends[-2] + ends[-3]
 
@@ -37,9 +37,9 @@
     wc.add_muscle(sides[2], sides[4], 4.0, 0.8)
     for k in range(len(sides) - 2):
         wc.add_muscle(sides[k], sides[k + 2], 18.0, 60.0 / 5.5)
 
     for k in reversed(range(len(sides) - 6)):
         wc.add_muscle(sides[k], sides[k + 5], 4.0, 20.0 / 9.0)
 
-    wc.add_muscle(center, sides[7], 2, 0, 90.0 / 9.0)
+    wc.add_muscle(center, sides[7], 2.0, 90.0 / 9.0)
     return wc.get_walker()
```

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/radial.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/radial.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 def make_circle(wc, cx, cy, radius, num_points):
     """Approximate a circle with center (cx,cy) square with num_points points."""
     joints = []
 
     tot_ang = 3.14 * 2.0
 
     for idx in range(num_points):
-        ang = (tot_ang / num_points) * idx
+        ang = (tot_ang / (num_points - 1)) * idx
         x = math.cos(ang) * radius + cx
         y = math.sin(ang) * radius + cy
         joints.append(wc.add_joint(x, y))
 
     return joints
 
 
 def make_walker():
-
     wc = walker_creator()
 
     num_points = 8
     rad = 5.0
     cx, cy = (5, 5)
     # the main body is a square
     points = make_circle(wc, cx, cy, rad, num_points)
```

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/runner.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 
-from openelm.environments.sodaracer.walker import query_cppn
-from openelm.environments.sodaracer.walker import walker_creator
+from openelm.environments.sodaracer.walker import query_cppn, walker_creator
 
 
 def make_walker(p_scale=1):  # acrylic of current (m)
     wc = walker_creator()
 
     def connect(x1, y1, x2, y2):
         if -2 * x1 + x2 * 2 > 2:
```

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/square.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/square.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/walk_creator.py` & `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/walk_creator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 
         Returns:
             bool: Whether the walker is valid or not
         """
         max_muscles_per_joint: int = 10
         max_muscle_strength: int = 10
         min_joint_distance: float = 0.1
-        # Check that walker is not empty.
-        if len(self.joints) == 0 and len(self.muscles) == 0:
-            return False
         for m in self.muscles:
             # Check a) that the strength of muscles is limited
             if m[-1]["type"] == "muscle":
                 if m[-1]["amplitude"] > max_muscle_strength:
                     return False
         # Check b) that each joint is connected only to so many muscles
         for j in self.joints:
@@ -50,15 +47,19 @@
                 < min_joint_distance
             ):
                 return False
         return True
 
 
 class walker_creator:
-    """Walker Creator Referenced in ELM Paper - https://arxiv.org/abs/2206.08896 (pg.16)."""
+    """
+    Walker Creator Referenced in ELM Paper.
+
+    See https://arxiv.org/abs/2206.08896 (pg.16).
+    """
 
     def __init__(self):
         self.joints: list[tuple[float, float]] = []
         self.muscles: list[list] = []
 
     def add_joint(self, x: float, y: float) -> tuple[float, float]:
         """Add a spring/joint to the sodaracer."""
```

### Comparing `OpenELM-0.2.1/src/openelm/environments/sodaracer/walker/wheel.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/wheel.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 
 
 def make_circle(wc, cx, cy, radius, num_points):
     joints = []
     tot_ang = 3.14 * 2.0
     for idx in range(num_points):
         ang = tot_ang / (num_points + 1) * idx
-        x = math.cos(ang) * radius + cx
+        x = math.cos(ang) * radius + 0.5
         y = math.sin(ang) * radius + cy
         joints.append(wc.add_joint(x, y))
     return joints
 
 
 def make_walker():
     wc = walker_creator()
     num_points = 8
     rad = 3.0
     cx, cy = (11, 5)
     points = make_circle(wc, 0.6, -0.5, rad / 2, num_points)
     center = wc.add_joint(cx + 1, cy + 1)
     for j in range(num_points):
         for i in range(num_points - 5):
+            # removed 0.0 (old 3rd param value) as it was used in deprecated isDistance
             wc.add_muscle(
-                points[j], points[(i + j) % num_points], 0.0, 1.0, (j + 1) / num_points
+                points[j], points[(i + j) % num_points], 1.0, (j + 1) / num_points
             )
         wc.add_muscle(points[j], center, 3, (j + 1) / num_points)
     return wc.get_walker()
```

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/Pipfile.lock` & `OpenELM-0.9.1/src/openelm/sandbox/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/README.md` & `OpenELM-0.9.1/src/openelm/sandbox/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py` & `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/CPPN_mutable.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/radial.py` & `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/radial.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/square.py` & `OpenELM-0.9.1/src/openelm/sandbox/server/environments/walker/square.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/server/environments/walker/walk_creator.py` & `OpenELM-0.9.1/src/openelm/environments/sodaracer/walker/walk_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,19 @@
             c) that there is a minimum distance between joints
 
         Returns:
             bool: Whether the walker is valid or not
         """
         max_muscles_per_joint: int = 10
         max_muscle_strength: int = 10
-        min_joint_distance: float = 0.1
+        # Original min_joint_distance = 0.1
+        min_joint_distance: float = 0.003
+        # Check that walker is not empty.
+        if len(self.joints) == 0 and len(self.muscles) == 0:
+            return False
         for m in self.muscles:
             # Check a) that the strength of muscles is limited
             if m[-1]["type"] == "muscle":
                 if m[-1]["amplitude"] > max_muscle_strength:
                     return False
         # Check b) that each joint is connected only to so many muscles
         for j in self.joints:
@@ -46,28 +50,29 @@
                 math.sqrt(((j1[0] - j2[0]) ** 2 + (j1[1] - j2[1]) ** 2))
                 < min_joint_distance
             ):
                 return False
         return True
 
 
-class walker_creator:
-    """
-    Walker Creator Referenced in ELM Paper.
+# scaling quick fix to make seed programs slightly smaller in scale, potentially making the evolved programs more dynamic
+SCALE = 0.22
+
 
-    See https://arxiv.org/abs/2206.08896 (pg.16).
-    """
+class walker_creator:
+    """Walker Creator Referenced in ELM Paper - https://arxiv.org/abs/2206.08896 (pg.16)."""
 
     def __init__(self):
         self.joints: list[tuple[float, float]] = []
         self.muscles: list[list] = []
 
     def add_joint(self, x: float, y: float) -> tuple[float, float]:
         """Add a spring/joint to the sodaracer."""
-        j: tuple[float, float] = (x, y)
+        # flipped sign to make galloper move more closely to expected, without functional impact on ELM experiments
+        j: tuple[float, float] = (x * SCALE, -y * SCALE)
         self.joints.append(j)
         return j
 
     def add_muscle(
         self,
         j0: tuple[float, float],
         j1: tuple[float, float],
```

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/server/index.py` & `OpenELM-0.9.1/src/openelm/sandbox/server/index.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/sandbox/server/sandbox_codex_execute.py` & `OpenELM-0.9.1/src/openelm/sandbox/server/sandbox_codex_execute.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     TEST_FAILED = 1
     TIMEOUT_EXCEPTION = 2
     SYNTAX_ERROR = 3
     TYPE_ERROR = 4
     EXCEPTION = 5
 
 
+def isgenerator(iterable):
+    return hasattr(iterable, "__iter__") and not hasattr(iterable, "__len__")
+
+
 def unsafe_execute(
     code_str: str,
     func_name: Optional[str] = None,
     args: Optional[dict[str, Any]] = None,
     ground_truth: Optional[dict[tuple, Any]] = None,
     timeout: float = 5.0,
     debug: bool = False,
@@ -70,15 +74,15 @@
                     elif args is not None:
                         result = code_dct[func_name](**args)
 
                     # Multiprocessing.pool.map
                     # (in utils.code_eval.pool_exec_processes())
                     # cannot return 'generators'
                     # (this may not catch all 'invalid' generator uses)
-                    if isinstance(result, range):
+                    if isinstance(result, range) or isgenerator(result):
                         result = list(result)
 
                     return result
                 elif ground_truth is not None:
                     if all(
                         [
                             code_dct[func_name](*arguments) == res
```

### Comparing `OpenELM-0.2.1/src/openelm/utils/code_eval.py` & `OpenELM-0.9.1/src/openelm/utils/code_eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,46 +146,57 @@
 def quadratic(a, b, c, x):
     """Return quadratic: a,b,c are coefficients and x is the independent variable."""
     return a * x**2 + b * x + c
 
 
 def pass_at_k(n, c, k):
     """
+    Adapted from "Evaluating Large Language Models Trained on Code" (https://arxiv.org/abs/2107.03374)
+
     :param n: total number of samples
     :param c: number of correct samples
     :param k: k in pass@k
     """
-    if n - c < k: return 1.0
+    assert n >= k
+    if n - c < k:
+        return 1.0
     return 1.0 - np.prod(1.0 - k / np.arange(n - c + 1, n + 1))
 
+
 def type_check(typ, obj):
     """
-    Checks the object is the correct type. Supports only bool, int, float, str, and (possibly nested) lists of these
+    Checks the object is the correct type. Supports only bool, int, float, str,
+    and (possibly nested) lists of these
 
     From: https://github.com/microsoft/PythonProgrammingPuzzles/blob/v0.2/puzzle_generator.py
     """
     type_s = type_str(typ)  # convert to string if necessary
 
     nest_depth = type_s.count("List")
-    assert type_s.count("[") == nest_depth, "type_check only supports List for now, no Sets, Dicts, Tuples, ..."
+    assert (
+        type_s.count("[") == nest_depth
+    ), "type_check only supports List for now, no Sets, Dicts, Tuples, ..."
 
     assert type_s.startswith("List[" * nest_depth) and type_s.endswith("]" * nest_depth)
-    base_type = {"bool": bool, "int": int, "float": float, "str": str}[type_s[5 * nest_depth:len(type_s) - nest_depth]]
+    base_type = {"bool": bool, "int": int, "float": float, "str": str}[
+        type_s[5 * nest_depth : len(type_s) - nest_depth]
+    ]
 
     def helper(depth, o):
         if depth == 0:
             return type(o) is base_type
         else:
             return type(o) is list and all(helper(depth - 1, i) for i in o)
 
     return helper(nest_depth, obj)
 
+
 def type_str(ty: type) -> str:
     """
     Convert type ty to string.
     :param ty: str, typing.List[int] , typing.List[typing.List[bool]], etc.
     :return: string form of type, "str", "List[int]" , "List[List[bool]]", etc.
 
     From: https://github.com/microsoft/PythonProgrammingPuzzles/blob/v0.2/puzzle_generator.py
     """
     type_str = str(ty).replace("typing.", "")
-    return type_str[8:-2] if type_str.startswith("<class '") else type_str
+    return type_str[8:-2] if type_str.startswith("<class '") else type_str
```

### Comparing `OpenELM-0.2.1/src/openelm/utils/diff_eval.py` & `OpenELM-0.9.1/src/openelm/utils/diff_eval.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/src/openelm/utils/utils.py` & `OpenELM-0.9.1/src/openelm/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from dataclasses import is_dataclass
 from pathlib import Path
 
 from omegaconf import DictConfig, OmegaConf
 
 
 def validate_config(config):
@@ -18,7 +19,13 @@
     else:
         try:
             return OmegaConf.load(config)
         except IOError:
             raise IOError(
                 "Invalid config type. Must be a path to a yaml, a dict, or dataclass."
             )
+
+
+def safe_open_w(path, *args, **kwargs):
+    """Open "path" for writing, creating any parent directories as needed."""
+    os.makedirs(os.path.dirname(path), exist_ok=True)
+    return open(path, *args, **kwargs)
```

### Comparing `OpenELM-0.2.1/tests/test_code_execute.py` & `OpenELM-0.9.1/tests/test_code_execute.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/tests/test_data/square.json` & `OpenELM-0.9.1/tests/test_data/square.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9703125%*

 * *Differences: {"'joints'": "{'0': {'sourceOffset': {'x': 40.90172576904297, 'y': -88.04464721679688}, "*

 * *             "'targetOffset': {'x': 40.90939712524414, 'y': -17.783472061157227}}, '1': "*

 * *             "{'sourceOffset': {'x': 40.90939712524414, 'y': -17.783472061157227}, 'targetOffset': "*

 * *             "{'x': 109.09062194824219, 'y': -17.78347396850586}}, '2': {'sourceOffset': {'x': "*

 * *             "109.09062194824219, 'y': -17.78347396850586}, 'targetOffset': {'x': "*

 * *             "109.09828186035156, 'y': -88.0446472 […]*

```diff
@@ -1,198 +1,198 @@
 {
     "joints": {
         "0": {
             "sourceID": "1",
             "sourceOffset": {
-                "x": 99.33401489257812,
-                "y": -5.326292037963867
+                "x": 40.90172576904297,
+                "y": -88.04464721679688
             },
             "targetID": "2",
             "targetOffset": {
-                "x": 99.55862426757812,
-                "y": -30.737947463989258
+                "x": 40.90939712524414,
+                "y": -17.783472061157227
             }
         },
         "1": {
             "sourceID": "2",
             "sourceOffset": {
-                "x": 99.55862426757812,
-                "y": -30.737947463989258
+                "x": 40.90939712524414,
+                "y": -17.783472061157227
             },
             "targetID": "3",
             "targetOffset": {
-                "x": 100.44113159179688,
-                "y": -30.737947463989258
+                "x": 109.09062194824219,
+                "y": -17.78347396850586
             }
         },
         "2": {
             "sourceID": "3",
             "sourceOffset": {
-                "x": 100.44113159179688,
-                "y": -30.737947463989258
+                "x": 109.09062194824219,
+                "y": -17.78347396850586
             },
             "targetID": "4",
             "targetOffset": {
-                "x": 100.66622924804688,
-                "y": -5.326292514801025
+                "x": 109.09828186035156,
+                "y": -88.04464721679688
             }
         },
         "3": {
             "sourceID": "4",
             "sourceOffset": {
-                "x": 100.66622924804688,
-                "y": -5.326292514801025
+                "x": 109.09828186035156,
+                "y": -88.04464721679688
             },
             "targetID": "1",
             "targetOffset": {
-                "x": 99.33401489257812,
-                "y": -5.326292037963867
+                "x": 40.90172576904297,
+                "y": -88.04464721679688
             }
         },
         "4": {
             "sourceID": "4",
             "sourceOffset": {
-                "x": 100.66622924804688,
-                "y": -5.326292514801025
+                "x": 109.09828186035156,
+                "y": -88.04464721679688
             },
             "targetID": "5",
             "targetOffset": {
-                "x": 99.99993896484375,
-                "y": -5.269007205963135
+                "x": 75.0,
+                "y": -52.984947204589844
             }
         },
         "5": {
             "sourceID": "1",
             "sourceOffset": {
-                "x": 99.33401489257812,
-                "y": -5.326292037963867
+                "x": 40.90172576904297,
+                "y": -88.04464721679688
             },
             "targetID": "5",
             "targetOffset": {
-                "x": 99.99993896484375,
-                "y": -5.269007205963135
+                "x": 75.0,
+                "y": -52.984947204589844
             }
         },
         "6": {
             "sourceID": "2",
             "sourceOffset": {
-                "x": 99.55862426757812,
-                "y": -30.737947463989258
+                "x": 40.90939712524414,
+                "y": -17.783472061157227
             },
             "targetID": "5",
             "targetOffset": {
-                "x": 99.99993896484375,
-                "y": -5.269007205963135
+                "x": 75.0,
+                "y": -52.984947204589844
             }
         },
         "7": {
             "sourceID": "3",
             "sourceOffset": {
-                "x": 100.44113159179688,
-                "y": -30.737947463989258
+                "x": 109.09062194824219,
+                "y": -17.78347396850586
             },
             "targetID": "5",
             "targetOffset": {
-                "x": 99.99993896484375,
-                "y": -5.269007205963135
+                "x": 75.0,
+                "y": -52.984947204589844
             }
         }
     },
     "shapes": {
         "12": {
             "bodyOffset": {
-                "x": 99.33401489257812,
-                "y": -5.326292037963867
+                "x": 40.90172576904297,
+                "y": -88.04464721679688
             },
             "center": {
                 "x": 0.0,
                 "y": 0.0
             },
             "color": "#369",
-            "radius": 2.597402572631836,
+            "radius": 1.948051929473877,
             "rotation": 0.0,
             "type": "circle"
         },
         "23": {
             "bodyOffset": {
-                "x": 99.55862426757812,
-                "y": -30.737947463989258
+                "x": 40.90939712524414,
+                "y": -17.783472061157227
             },
             "center": {
                 "x": 0.0,
                 "y": 0.0
             },
             "color": "#369",
-            "radius": 2.597402572631836,
+            "radius": 1.948051929473877,
             "rotation": 0.0,
             "type": "circle"
         },
         "34": {
             "bodyOffset": {
-                "x": 100.44113159179688,
-                "y": -30.737947463989258
+                "x": 109.09062194824219,
+                "y": -17.78347396850586
             },
             "center": {
                 "x": 0.0,
                 "y": 0.0
             },
             "color": "#369",
-            "radius": 2.597402572631836,
+            "radius": 1.948051929473877,
             "rotation": 0.0,
             "type": "circle"
         },
         "45": {
             "bodyOffset": {
-                "x": 100.66622924804688,
-                "y": -5.326292514801025
+                "x": 109.09828186035156,
+                "y": -88.04464721679688
             },
             "center": {
                 "x": 0.0,
                 "y": 0.0
             },
             "color": "#369",
-            "radius": 2.597402572631836,
+            "radius": 1.948051929473877,
             "rotation": 0.0,
             "type": "circle"
         },
         "56": {
             "bodyOffset": {
-                "x": 99.99993896484375,
-                "y": -5.269007205963135
+                "x": 75.0,
+                "y": -52.984947204589844
             },
             "center": {
                 "x": 0.0,
                 "y": 0.0
             },
             "color": "#369",
-            "radius": 2.597402572631836,
+            "radius": 1.948051929473877,
             "rotation": 0.0,
             "type": "circle"
         },
         "ground1": {
             "bodyOffset": {
                 "x": 0.0,
-                "y": -18.00002098083496
+                "y": -100.0
             },
             "color": "#38F",
             "points": [
                 {
-                    "x": -350.0,
+                    "x": -3500.0,
                     "y": -10.0
                 },
                 {
-                    "x": 350.0,
+                    "x": 3500.0,
                     "y": -10.0
                 },
                 {
-                    "x": 350.0,
+                    "x": 3500.0,
                     "y": 10.0
                 },
                 {
-                    "x": -350.0,
+                    "x": -3500.0,
                     "y": 10.0
                 }
             ],
             "rotation": 0.0,
             "type": "polygon"
         }
     }
```

### Comparing `OpenELM-0.2.1/tests/test_diff.py` & `OpenELM-0.9.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/tests/test_sodarace_env.py` & `OpenELM-0.9.1/tests/test_sodarace_env.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,90 +45,86 @@
     square_world = IESoRWorld()
     radial_world = IESoRWorld()
     cppn_fixed_world = IESoRWorld()
     cppn_mutable_world = IESoRWorld()
 
     square_dict = square_world.load_body_into_world(square_walker.to_dict())
     assert square_dict == {
-        "width": 413.2231404958677,
-        "height": 240.0,
+        "width": 68.18181818181817,
+        "height": 70.4,
         "startX": 0.0,
-        "offsetX": -106.61157024793386,
-        "startY": -216.0,
-        "offsetY": 171.0,
-        "mass": 1136.0864722563908,
+        "startY": 32.0,
+        "offsetX": 40.909090909090914,
+        "offsetY": 32.8,
+        "mass": 241.58651363350822,
     }
 
     square_start, square_end = run_world(square_world, square_dict)
-    assert (square_start, square_end) == (0.0, 7.27755535535573)
+    assert (square_start, square_end) == (0.0, 81.81081667813388)
 
     radial_dict = radial_world.load_body_into_world(radial_walker.to_dict())
-
     assert radial_dict == {
-        "width": 413.2228784561031,
-        "height": 239.99961951834635,
-        "startX": 0.0002620397645793254,
-        "offsetX": -106.61170126781613,
-        "startY": -215.99996195182018,
-        "offsetY": 171.00015219264702,
-        "mass": 1182.4111517904973,
+        "width": 64.83262907589534,
+        "height": 68.62412927885356,
+        "startX": 3.349189105922829,
+        "startY": 32.90044749507858,
+        "offsetX": 39.2344963561295,
+        "offsetY": 32.78748786549464,
+        "mass": 252.54982123779916,
     }
 
     radial_start, radial_end = run_world(radial_world, radial_dict)
-    assert (radial_start, radial_end) == (0.0002620397645793254, 95.02245400562137)
+    assert (radial_start, radial_end) == (3.349189105922829, 87.38454747307286)
 
     cppn_fixed_dict = cppn_fixed_world.load_body_into_world(cppn_fixed_walker.to_dict())
-
     assert cppn_fixed_dict == {
-        "width": 433.8842975206611,
-        "height": 72.0,
+        "width": 71.59090909090908,
+        "height": 21.120000000000005,
         "startX": 0.0,
-        "offsetX": -116.94214876033055,
-        "startY": -48.0,
-        "offsetY": 87.0,
-        "mass": 2796.6059242043043,
+        "startY": 32.0,
+        "offsetX": 39.20454545454546,
+        "offsetY": 57.44,
+        "mass": 572.6414986337938,
     }
 
     cppn_fixed_start, cppn_fixed_end = run_world(cppn_fixed_world, cppn_fixed_dict)
-
-    assert (cppn_fixed_start, cppn_fixed_end) == (0.0, 37.73778779841649)
+    assert (cppn_fixed_start, cppn_fixed_end) == (0.0, 88.8606581254439)
 
     cppn_mutable_dict = cppn_mutable_world.load_body_into_world(
         cppn_mutable_walker.to_dict()
     )
-
     assert cppn_mutable_dict == {
-        "width": 433.8842975206611,
-        "height": 72.0,
+        "width": 71.59090909090908,
+        "height": 21.120000000000005,
         "startX": 0.0,
-        "offsetX": -116.94214876033055,
-        "startY": -48.0,
-        "offsetY": 87.0,
-        "mass": 2796.6059242043043,
+        "startY": 32.0,
+        "offsetX": 39.20454545454546,
+        "offsetY": 57.44,
+        "mass": 572.6414986337938,
     }
 
     cppn_mutable_start, cppn_mutable_end = run_world(
         cppn_mutable_world, cppn_mutable_dict
     )
-
-    assert (cppn_mutable_start, cppn_mutable_end) == (0.0, 29.67882020808446)
+    assert (cppn_mutable_start, cppn_mutable_end) == (0.0, 458.53709550337356)
 
 
 def test_square_draw_list(square_walker_dict):
     square_walker: Walker = make_walker_square()
     square_world = IESoRWorld()
     square_dict = square_world.load_body_into_world(square_walker.to_dict())
 
     _, _ = run_world(square_world, square_dict)
     square_draw_list_dict = ast.literal_eval(square_world.get_world_json())
+
     assert square_draw_list_dict == square_walker_dict
 
-# TODO: Remake cppn json
-# def test_cppn_fixed_draw_list(cppn_fixed_walker_dict):
-#     cppn_fixed_walker: Walker = make_walker_cppn_fixed()
-#     cppn_fixed_world = IESoRWorld()
-#     cppn_fixed_dict = cppn_fixed_world.load_body_into_world(cppn_fixed_walker.to_dict())
 
-#     _, _ = run_world(cppn_fixed_world, cppn_fixed_dict)
-#     cppn_draw_list_dict = ast.literal_eval(cppn_fixed_world.get_world_json())
+def test_cppn_fixed_draw_list(cppn_fixed_walker_dict):
+    cppn_fixed_walker: Walker = make_walker_cppn_fixed()
+    cppn_fixed_world = IESoRWorld()
+    cppn_fixed_dict = cppn_fixed_world.load_body_into_world(cppn_fixed_walker.to_dict())
+
+    _, _ = run_world(cppn_fixed_world, cppn_fixed_dict)
+    cppn_draw_list_dict = ast.literal_eval(cppn_fixed_world.get_world_json())
 
-#     assert cppn_draw_list_dict == cppn_fixed_walker_dict
+    assert cppn_draw_list_dict == cppn_fixed_walker_dict
```

### Comparing `OpenELM-0.2.1/tests/test_sodarace_walkers.py` & `OpenELM-0.9.1/tests/test_sodarace_walkers.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ]
     correct_muscle = [2, 4, {"type": "muscle", "amplitude": 2.0, "phase": 0.0}]
     assert square_walker.muscles[0] == correct_distance_joint
     assert square_walker.muscles[-1] == correct_muscle
 
     # Test full dictionary
     correct_square_dict: dict = {
-        "joints": [(0, 0), (0, 10), (10, 10), (10, 0), (5, 5)],
+        "joints": [(0.0, 0.0), (0.0, -2.2), (2.2, -2.2), (2.2, 0.0), (1.1, -1.1)],
         "muscles": [
             [0, 1, {"type": "distance", "amplitude": 0.0, "phase": 0.0}],
             [1, 2, {"type": "distance", "amplitude": 0.0, "phase": 0.0}],
             [2, 3, {"type": "distance", "amplitude": 0.0, "phase": 0.0}],
             [3, 0, {"type": "distance", "amplitude": 0.0, "phase": 0.0}],
             [3, 4, {"type": "distance", "amplitude": 0.0, "phase": 0.0}],
             [0, 4, {"type": "muscle", "amplitude": 5.0, "phase": 0.0}],
```

### Comparing `OpenELM-0.2.1/tests/test_truncate.py` & `OpenELM-0.9.1/tests/test_truncate.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/README.md` & `OpenELM-0.9.1/trlx_example/README.md`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/configs/ppo_softprompt_config.yml` & `OpenELM-0.9.1/trlx_example/configs/ppo_softprompt_config.yml`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/model/accelerate_ppo_softprompt_model.py` & `OpenELM-0.9.1/trlx_example/model/accelerate_ppo_softprompt_model.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/orchestrator/ppo_softprompt_orchestrator.py` & `OpenELM-0.9.1/trlx_example/orchestrator/ppo_softprompt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/ppo_softprompt_long_completions.py` & `OpenELM-0.9.1/trlx_example/ppo_softprompt_long_completions.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/ppo_softprompt_sentiment.py` & `OpenELM-0.9.1/trlx_example/ppo_softprompt_sentiment.py`

 * *Files identical despite different names*

### Comparing `OpenELM-0.2.1/trlx_example/ppo_softprompt_short_completions.py` & `OpenELM-0.9.1/trlx_example/ppo_softprompt_short_completions.py`

 * *Files identical despite different names*

