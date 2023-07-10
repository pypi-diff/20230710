# Comparing `tmp/gvec-to-python-1.1.2.tar.gz` & `tmp/gvec-to-python-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvec-to-python-1.1.2.tar", last modified: Thu Jul  6 09:25:44 2023, max compression
+gzip compressed data, was "gvec-to-python-1.1.3.tar", last modified: Mon Jul 10 13:19:52 2023, max compression
```

## Comparing `gvec-to-python-1.1.2.tar` & `gvec-to-python-1.1.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.694323 gvec-to-python-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5847 2023-07-06 09:25:44.694323 gvec-to-python-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3987 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 09:25:44.694323 gvec-to-python-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.678323 gvec-to-python-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.682323 gvec-to-python-1.1.2/src/gvec_to_python/
--rw-rw-rw-   0 root         (0) root         (0)    34611 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/GVEC_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/base/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5015 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/base/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13375 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/base/fbase.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/base/make_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/base/sbase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/console/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/console/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/console/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/equilibrium/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/equilibrium/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4329 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/equilibrium/profiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/geometry/
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/geometry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    46341 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/geometry/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1785 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/geometry/kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/hylife/
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/basics/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/basics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6544 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py
--rw-rw-rw-   0 root         (0) root         (0)    20753 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py
--rw-rw-rw-   0 root         (0) root         (0)     9693 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/derivatives/
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/derivatives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5663 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py
--rw-rw-rw-   0 root         (0) root         (0)    15218 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/reader/
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/reader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13117 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/reader/gvec_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.686323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/circ_tok/
--rw-rw-rw-   0 root         (0) root         (0)    51408 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7519 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/circ_tok/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.682323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/
--rw-rw-rw-   0 root         (0) root         (0)    49404 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     6859 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/
--rw-rw-rw-   0 root         (0) root         (0)    68052 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     6859 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.682323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/
--rw-rw-rw-   0 root         (0) root         (0)    65028 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7253 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/
--rw-rw-rw-   0 root         (0) root         (0)    89724 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/
--rw-rw-rw-   0 root         (0) root         (0)   161316 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7249 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/util/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/util/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/util/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/writer/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/src/gvec_to_python/writer/paraview/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/writer/paraview/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31373 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/writer/paraview/mesh_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/src/gvec_to_python/writer/paraview/vtk_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.682323 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5847 2023-07-06 09:25:44.000000 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2934 2023-07-06 09:25:44.000000 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 09:25:44.000000 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-06 09:25:44.000000 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-06 09:25:44.000000 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 09:25:44.000000 gvec-to-python-1.1.2/src/gvec_to_python.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:25:44.690323 gvec-to-python-1.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/tests/test_gvec_domain.py
--rw-rw-rw-   0 root         (0) root         (0)    13089 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/tests/test_gvec_equil.py
--rw-rw-rw-   0 root         (0) root         (0)     3929 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/tests/test_gvec_profiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-07-06 08:32:37.000000 gvec-to-python-1.1.2/tests/test_splines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.462120 gvec-to-python-1.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5847 2023-07-10 13:19:52.462120 gvec-to-python-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-10 13:12:14.000000 gvec-to-python-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 13:19:52.462120 gvec-to-python-1.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.434120 gvec-to-python-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.442120 gvec-to-python-1.1.3/src/gvec_to_python/
+-rw-rw-rw-   0 root         (0) root         (0)    34611 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/GVEC_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-07-10 13:12:14.000000 gvec-to-python-1.1.3/src/gvec_to_python/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.442120 gvec-to-python-1.1.3/src/gvec_to_python/base/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5015 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/base/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13375 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/base/fbase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/base/make_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/base/sbase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.446120 gvec-to-python-1.1.3/src/gvec_to_python/console/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/console/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      680 2023-07-10 13:12:14.000000 gvec-to-python-1.1.3/src/gvec_to_python/console/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.446120 gvec-to-python-1.1.3/src/gvec_to_python/equilibrium/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/equilibrium/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/equilibrium/profiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.446120 gvec-to-python-1.1.3/src/gvec_to_python/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46341 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/geometry/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/geometry/kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.446120 gvec-to-python-1.1.3/src/gvec_to_python/hylife/
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.450120 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.450120 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/basics/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/basics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6544 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    20753 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py
+-rw-rw-rw-   0 root         (0) root         (0)     9693 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.450120 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/derivatives/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/derivatives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py
+-rw-rw-rw-   0 root         (0) root         (0)    15218 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.450120 gvec-to-python-1.1.3/src/gvec_to_python/reader/
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/reader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13117 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/reader/gvec_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.450120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.454120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/circ_tok/
+-rw-rw-rw-   0 root         (0) root         (0)    51408 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7519 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/circ_tok/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.438120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.454120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    49404 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     6859 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.454120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    68052 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     6859 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.438120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.454120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    65028 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7253 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.454120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    89724 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.458120 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)   161316 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.458120 gvec-to-python-1.1.3/src/gvec_to_python/util/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/util/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/util/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.458120 gvec-to-python-1.1.3/src/gvec_to_python/writer/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.462120 gvec-to-python-1.1.3/src/gvec_to_python/writer/paraview/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/writer/paraview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31373 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/writer/paraview/mesh_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/src/gvec_to_python/writer/paraview/vtk_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.442120 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5847 2023-07-10 13:19:52.000000 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-07-10 13:19:52.000000 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:19:52.000000 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-10 13:19:52.000000 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-10 13:19:52.000000 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 13:19:52.000000 gvec-to-python-1.1.3/src/gvec_to_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:19:52.462120 gvec-to-python-1.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/tests/test_gvec_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13089 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/tests/test_gvec_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)     3929 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/tests/test_gvec_profiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-07-06 08:32:37.000000 gvec-to-python-1.1.3/tests/test_splines.py
```

### Comparing `gvec-to-python-1.1.2/LICENSE` & `gvec-to-python-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/PKG-INFO` & `gvec-to-python-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvec-to-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parse GVEC output in Python
 Author: Tin Kei Cheng, Florian Hindenlang, Stefan Possanner
 Author-email: stefan.possanner@ipp.mpg.de, florian.hindenlang@ipp.mpg.de
 License: Copyright 2021 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software 
         and associated documentation files (the "Software"), to deal in the Software without restriction,
```

### Comparing `gvec-to-python-1.1.2/README.md` & `gvec-to-python-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/pyproject.toml` & `gvec-to-python-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gvec-to-python"
-version = "1.1.2"
+version = "1.1.3"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   { name = "Tin Kei Cheng"},
   { name = "Florian Hindenlang"},
   { name = "Stefan Possanner"},
```

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/GVEC_functions.py` & `gvec-to-python-1.1.3/src/gvec_to_python/GVEC_functions.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/Makefile` & `gvec-to-python-1.1.3/src/gvec_to_python/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #--------------------------------------
 # CONFIGURATION
 #--------------------------------------
 
 PYTHON  := python3
 SO_EXT  := $(shell $(PYTHON) -c "import sysconfig; print(sysconfig.get_config_var('EXT_SUFFIX'))")
 LIBDIR  := $(shell $(PYTHON) -c "import sysconfig; print(sysconfig.get_config_var('LIBDIR'))")
-FLAGS            := --libdir $(LIBDIR) --conda-warnings off
+FLAGS            := --libdir $(LIBDIR) $(flags) 
 
 #--------------------------------------
 # SOURCE FILES 
 #--------------------------------------
 
 # Splines
 BK   := $(install_path)/hylife/utilities_FEEC/bsplines_kernels
```

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/__init__.py` & `gvec-to-python-1.1.3/src/gvec_to_python/__init__.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/base/base.py` & `gvec-to-python-1.1.3/src/gvec_to_python/base/base.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/base/fbase.py` & `gvec-to-python-1.1.3/src/gvec_to_python/base/fbase.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/base/make_base.py` & `gvec-to-python-1.1.3/src/gvec_to_python/base/make_base.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/base/sbase.py` & `gvec-to-python-1.1.3/src/gvec_to_python/base/sbase.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/equilibrium/profiles.py` & `gvec-to-python-1.1.3/src/gvec_to_python/equilibrium/profiles.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/geometry/__init__.py` & `gvec-to-python-1.1.3/src/gvec_to_python/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/geometry/domain.py` & `gvec-to-python-1.1.3/src/gvec_to_python/geometry/domain.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/geometry/kernels.py` & `gvec-to-python-1.1.3/src/gvec_to_python/geometry/kernels.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py` & `gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/basics/spline_evaluation_1d.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py` & `gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/bsplines.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py` & `gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/bsplines_kernels.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py` & `gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/derivatives/derivatives.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py` & `gvec-to-python-1.1.3/src/gvec_to_python/hylife/utilities_FEEC/spline_space.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/reader/gvec_reader.py` & `gvec-to-python-1.1.3/src/gvec_to_python/reader/gvec_reader.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/circ_tok/CIRC_TOK_State_0000_00010000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/circ_tok/parameter.ini` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/circ_tok/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_E1D6_M6N6_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E1D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_E4D6_M6N6_State_0001_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell/newBC_E4D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini` & `gvec-to-python-1.1.3/src/gvec_to_python/testcases/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/util/logger.py` & `gvec-to-python-1.1.3/src/gvec_to_python/util/logger.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/util/numpy_encoder.py` & `gvec-to-python-1.1.3/src/gvec_to_python/util/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/writer/paraview/mesh_creator.py` & `gvec-to-python-1.1.3/src/gvec_to_python/writer/paraview/mesh_creator.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python/writer/paraview/vtk_writer.py` & `gvec-to-python-1.1.3/src/gvec_to_python/writer/paraview/vtk_writer.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python.egg-info/PKG-INFO` & `gvec-to-python-1.1.3/src/gvec_to_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gvec-to-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parse GVEC output in Python
 Author: Tin Kei Cheng, Florian Hindenlang, Stefan Possanner
 Author-email: stefan.possanner@ipp.mpg.de, florian.hindenlang@ipp.mpg.de
 License: Copyright 2021 (c) T.K. Cheng, F. Hindenlang, S. Possanner | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software 
         and associated documentation files (the "Software"), to deal in the Software without restriction,
```

### Comparing `gvec-to-python-1.1.2/src/gvec_to_python.egg-info/SOURCES.txt` & `gvec-to-python-1.1.3/src/gvec_to_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/tests/test_gvec_domain.py` & `gvec-to-python-1.1.3/tests/test_gvec_domain.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/tests/test_gvec_equil.py` & `gvec-to-python-1.1.3/tests/test_gvec_equil.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/tests/test_gvec_profiles.py` & `gvec-to-python-1.1.3/tests/test_gvec_profiles.py`

 * *Files identical despite different names*

### Comparing `gvec-to-python-1.1.2/tests/test_splines.py` & `gvec-to-python-1.1.3/tests/test_splines.py`

 * *Files identical despite different names*

