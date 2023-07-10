# Comparing `tmp/ntrfc-0.1.4.tar.gz` & `tmp/ntrfc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntrfc-0.1.4.tar", last modified: Sun Jun 25 19:22:03 2023, max compression
+gzip compressed data, was "ntrfc-0.1.5.tar", last modified: Mon Jul 10 19:50:19 2023, max compression
```

## Comparing `ntrfc-0.1.4.tar` & `ntrfc-0.1.5.tar`

### file list

```diff
@@ -1,161 +1,194 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.328661 ntrfc-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)      164 2022-12-20 22:13:31.000000 ntrfc-0.1.4/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-02-23 16:47:34.000000 ntrfc-0.1.4/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-06-25 19:18:31.000000 ntrfc-0.1.4/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-12-20 22:13:31.000000 ntrfc-0.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-02-23 16:47:34.000000 ntrfc-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3450 2023-06-25 19:22:03.328661 ntrfc-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2424 2023-03-11 02:07:32.000000 ntrfc-0.1.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.561651 ntrfc-0.1.4/data/
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-02-23 16:47:34.000000 ntrfc-0.1.4/data/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.705653 ntrfc-0.1.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)      606 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-03 20:46:33.000000 ntrfc-0.1.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      302 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1086 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      767 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.cascade_case.domain.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.cascade_case.rst
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.cascade_case.solution.case_modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.cascade_case.solution.rst
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.dictutils.rst
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.filehandling.rst
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.fluid.rst
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.geometry.rst
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.math.rst
--rw-rw-rw-   0 root         (0) root         (0)     1125 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.meshquality.rst
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.rst
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.timeseries.rst
--rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.turbo.airfoil_generators.rst
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-03 21:35:35.000000 ntrfc-0.1.4/docs/ntrfc.turbo.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-12-20 22:13:31.000000 ntrfc-0.1.4/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.741653 ntrfc-0.1.4/ntrfc/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-25 19:18:31.000000 ntrfc-0.1.4/ntrfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.768653 ntrfc-0.1.4/ntrfc/cascade_case/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/cascade_case/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.785654 ntrfc-0.1.4/ntrfc/cascade_case/casemeta/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 20:08:25.000000 ntrfc-0.1.4/ntrfc/cascade_case/casemeta/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-20 23:01:48.000000 ntrfc-0.1.4/ntrfc/cascade_case/casemeta/casemeta.py
--rw-rw-rw-   0 root         (0) root         (0)     3414 2023-06-20 23:01:48.000000 ntrfc-0.1.4/ntrfc/cascade_case/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-06-20 23:01:48.000000 ntrfc-0.1.4/ntrfc/cascade_case/solution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.832654 ntrfc-0.1.4/ntrfc/cascade_case/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 20:08:25.000000 ntrfc-0.1.4/ntrfc/cascade_case/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-19 20:08:25.000000 ntrfc-0.1.4/ntrfc/cascade_case/utils/domain_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-06-20 23:01:48.000000 ntrfc-0.1.4/ntrfc/cascade_case/utils/postprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-06-25 13:01:04.000000 ntrfc-0.1.4/ntrfc/cascade_case/utils/probecontainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-06-19 20:08:25.000000 ntrfc-0.1.4/ntrfc/cascade_case/utils/sliceseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.853655 ntrfc-0.1.4/ntrfc/filehandling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/filehandling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/filehandling/datafiles.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/filehandling/mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.878655 ntrfc-0.1.4/ntrfc/fluid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/fluid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2023-05-31 23:21:53.000000 ntrfc-0.1.4/ntrfc/fluid/fluid.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2023-05-31 23:21:53.000000 ntrfc-0.1.4/ntrfc/fluid/isentropic.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-05-31 23:21:53.000000 ntrfc-0.1.4/ntrfc/fluid/turbulence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.907655 ntrfc-0.1.4/ntrfc/geometry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/geometry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4515 2023-02-24 01:36:46.000000 ntrfc-0.1.4/ntrfc/geometry/alphashape.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/geometry/line.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/geometry/plane.py
--rw-rw-rw-   0 root         (0) root         (0)     2105 2023-06-21 06:18:33.000000 ntrfc-0.1.4/ntrfc/geometry/surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.916655 ntrfc-0.1.4/ntrfc/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5748 2023-02-24 01:36:46.000000 ntrfc-0.1.4/ntrfc/math/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7212 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/math/vectorcalc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.948656 ntrfc-0.1.4/ntrfc/meshquality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/meshquality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/meshquality/aspect_ratio.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/meshquality/grid_convergece_index.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/meshquality/meshexpansion.py
--rw-rw-rw-   0 root         (0) root         (0)     8206 2023-06-19 20:08:25.000000 ntrfc-0.1.4/ntrfc/meshquality/nondimensionals.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/meshquality/skewness.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-12-20 22:13:31.000000 ntrfc-0.1.4/ntrfc/ntrfc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.962656 ntrfc-0.1.4/ntrfc/timeseries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/timeseries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2292 2023-02-24 01:36:46.000000 ntrfc-0.1.4/ntrfc/timeseries/integral_scales.py
--rw-rw-rw-   0 root         (0) root         (0)    13578 2023-06-25 13:01:04.000000 ntrfc-0.1.4/ntrfc/timeseries/stationarity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.005657 ntrfc-0.1.4/ntrfc/turbo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/turbo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.024657 ntrfc-0.1.4/ntrfc/turbo/airfoil_generators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/turbo/airfoil_generators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9570 2023-02-24 01:36:46.000000 ntrfc-0.1.4/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-31 23:21:53.000000 ntrfc-0.1.4/ntrfc/turbo/bladeloading.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/turbo/cascade_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     5648 2023-06-21 06:18:33.000000 ntrfc-0.1.4/ntrfc/turbo/domaingen_cascade.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-02-23 16:47:34.000000 ntrfc-0.1.4/ntrfc/turbo/integrals.py
--rw-rw-rw-   0 root         (0) root         (0)     9047 2023-06-01 20:28:51.000000 ntrfc-0.1.4/ntrfc/turbo/pointcloud_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-03-10 23:35:04.000000 ntrfc-0.1.4/ntrfc/turbo/probegeneration.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-05-23 23:18:14.000000 ntrfc-0.1.4/ntrfc/turbo/profile_tele_extraction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:02.756653 ntrfc-0.1.4/ntrfc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3450 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4103 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      209 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-25 19:22:02.000000 ntrfc-0.1.4/ntrfc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-25 19:22:03.330661 ntrfc-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-25 19:18:31.000000 ntrfc-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.035657 ntrfc-0.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-12-20 22:13:31.000000 ntrfc-0.1.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.044657 ntrfc-0.1.4/tests/cascadecase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/cascadecase/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.045657 ntrfc-0.1.4/tests/cascadecase/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/cascadecase/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-19 20:08:25.000000 ntrfc-0.1.4/tests/cascadecase/domain/test_ntrfc_domaingen_cascade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.055657 ntrfc-0.1.4/tests/cascadecase/solution/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/cascadecase/solution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2023-06-20 23:01:48.000000 ntrfc-0.1.4/tests/cascadecase/solution/test_probecontainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3789 2023-06-20 23:01:48.000000 ntrfc-0.1.4/tests/cascadecase/solution/test_solution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.066657 ntrfc-0.1.4/tests/filehandling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/filehandling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/filehandling/test_ntrfc_datafiles.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/filehandling/test_ntrfc_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.130658 ntrfc-0.1.4/tests/fluid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-14 22:47:15.000000 ntrfc-0.1.4/tests/fluid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-05-31 23:21:53.000000 ntrfc-0.1.4/tests/fluid/test_ntrfc_fluid.py
--rw-rw-rw-   0 root         (0) root         (0)     2174 2023-05-31 23:21:53.000000 ntrfc-0.1.4/tests/fluid/test_ntrfc_isentropic.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-05-31 23:21:53.000000 ntrfc-0.1.4/tests/fluid/test_ntrfc_turbulence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.204659 ntrfc-0.1.4/tests/geometry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/geometry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1975 2023-03-10 23:35:04.000000 ntrfc-0.1.4/tests/geometry/test_ntrfc_alphashape.py
--rw-rw-rw-   0 root         (0) root         (0)     5126 2023-06-01 20:28:51.000000 ntrfc-0.1.4/tests/geometry/test_ntrfc_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/geometry/test_ntrfc_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/geometry/test_ntrfc_plane.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/geometry/test_ntrfc_surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.210659 ntrfc-0.1.4/tests/math/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/math/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8342 2023-06-01 20:28:51.000000 ntrfc-0.1.4/tests/math/test_ntrfc_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/math/test_ntrfc_vectorcalc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.245660 ntrfc-0.1.4/tests/meshquality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/meshquality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/meshquality/test_ntrfc_aspect_ratio.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/meshquality/test_ntrfc_grid_convergence_index.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/meshquality/test_ntrfc_meshexpansion.py
--rw-rw-rw-   0 root         (0) root         (0)    13631 2023-06-19 20:08:25.000000 ntrfc-0.1.4/tests/meshquality/test_ntrfc_nondimensionals.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/meshquality/test_ntrfc_skewness.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/test_ntrfc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.268660 ntrfc-0.1.4/tests/timeseries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/timeseries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/timeseries/test_ntrfc_integral_scales.py
--rw-rw-rw-   0 root         (0) root         (0)    10831 2023-05-31 23:21:53.000000 ntrfc-0.1.4/tests/timeseries/test_ntrfc_stationarity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.315661 ntrfc-0.1.4/tests/turbo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/turbo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:22:03.327661 ntrfc-0.1.4/tests/turbo/airfoil_generators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/turbo/airfoil_generators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-02-23 16:47:34.000000 ntrfc-0.1.4/tests/turbo/airfoil_generators/test_parsec_airfoil_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-05-31 23:21:53.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_bladeloading.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-03-10 23:35:04.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_cascade_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-21 06:18:33.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_domaingen_cascade.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_integrals.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-01 20:28:51.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_pointcloud_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-03-10 23:35:04.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_probegeneration.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-02-24 01:36:46.000000 ntrfc-0.1.4/tests/turbo/test_ntrfc_profile_tele_extraction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.780072 ntrfc-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2022-12-20 22:15:49.000000 ntrfc-0.1.5/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3646 2023-07-08 13:00:17.000000 ntrfc-0.1.5/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-08 13:00:17.000000 ntrfc-0.1.5/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2022-12-20 22:15:49.000000 ntrfc-0.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-03 23:16:07.000000 ntrfc-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-07-10 19:50:19.780072 ntrfc-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2023-07-08 13:00:17.000000 ntrfc-0.1.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.566007 ntrfc-0.1.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-03 20:43:18.000000 ntrfc-0.1.5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      302 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-07-08 13:00:17.000000 ntrfc-0.1.5/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      767 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-03 21:14:55.000000 ntrfc-0.1.5/docs/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.cascade_case.domain.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.cascade_case.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.cascade_case.solution.case_modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.cascade_case.solution.rst
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.dictutils.rst
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.filehandling.rst
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.fluid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.geometry.rst
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.math.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.meshquality.rst
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-03 21:14:55.000000 ntrfc-0.1.5/docs/ntrfc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.timeseries.rst
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.turbo.airfoil_generators.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-06-03 21:26:48.000000 ntrfc-0.1.5/docs/ntrfc.turbo.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)       65 2022-12-20 22:15:49.000000 ntrfc-0.1.5/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.638008 ntrfc-0.1.5/ntrfc/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-25 18:46:45.000000 ntrfc-0.1.5/ntrfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.696009 ntrfc-0.1.5/ntrfc/cascade_case/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/cascade_case/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.736010 ntrfc-0.1.5/ntrfc/cascade_case/casemeta/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 23:30:24.000000 ntrfc-0.1.5/ntrfc/cascade_case/casemeta/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-20 23:39:11.000000 ntrfc-0.1.5/ntrfc/cascade_case/casemeta/casemeta.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/cascade_case/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     7642 2023-07-03 19:37:19.000000 ntrfc-0.1.5/ntrfc/cascade_case/solution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.795011 ntrfc-0.1.5/ntrfc/cascade_case/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-18 22:04:59.000000 ntrfc-0.1.5/ntrfc/cascade_case/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/cascade_case/utils/domain_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-06-25 14:28:24.000000 ntrfc-0.1.5/ntrfc/cascade_case/utils/probecontainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-06-18 22:04:59.000000 ntrfc-0.1.5/ntrfc/cascade_case/utils/sliceseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.806012 ntrfc-0.1.5/ntrfc/data/
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.851012 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.149018 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/boundary/
+-rw-rw-rw-   0 root         (0) root         (0)   271732 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/boundary/blade_wall.vtp
+-rw-rw-rw-   0 root         (0) root         (0)     9792 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/boundary/inlet.vtp
+-rw-rw-rw-   0 root         (0) root         (0)    13301 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/boundary/outlet.vtp
+-rw-rw-rw-   0 root         (0) root         (0)  4359505 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/openfoam_cascade_case/internal.vtu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:15.775991 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:15.775991 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:15.775991 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.333022 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0/
+-rw-rw-rw-   0 root         (0) root         (0)    79550 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0/T
+-rw-rw-rw-   0 root         (0) root         (0)   235840 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0/U
+-rw-rw-rw-   0 root         (0) root         (0)    79550 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0/p
+-rw-rw-rw-   0 root         (0) root         (0)    79550 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0/rho
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.635028 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/
+-rw-rw-rw-   0 root         (0) root         (0)    68770 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/T
+-rw-rw-rw-   0 root         (0) root         (0)   203912 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/U
+-rw-rw-rw-   0 root         (0) root         (0)    68770 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/p
+-rw-rw-rw-   0 root         (0) root         (0)    68770 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/data/openfoam_probedata/postProcessing/probes/0.00943924517741/rho
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.725030 ntrfc-0.1.5/ntrfc/data/turbine_cascade/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/turbine_cascade/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8555 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/turbine_cascade/profilepoints.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.734030 ntrfc-0.1.5/ntrfc/data/turbine_cascade_2/
+-rw-rw-rw-   0 root         (0) root         (0)    14992 2023-07-05 19:37:09.000000 ntrfc-0.1.5/ntrfc/data/turbine_cascade_2/profilepoints.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.761031 ntrfc-0.1.5/ntrfc/data/v2500_compressorcascade/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/v2500_compressorcascade/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    52233 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/data/v2500_compressorcascade/profilepoints.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.802032 ntrfc-0.1.5/ntrfc/filehandling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/filehandling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/filehandling/datafiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2023-07-03 23:16:07.000000 ntrfc-0.1.5/ntrfc/filehandling/mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.823032 ntrfc-0.1.5/ntrfc/fluid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/fluid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2023-05-31 22:49:09.000000 ntrfc-0.1.5/ntrfc/fluid/fluid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2023-05-31 22:49:09.000000 ntrfc-0.1.5/ntrfc/fluid/isentropic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-05-31 22:49:09.000000 ntrfc-0.1.5/ntrfc/fluid/turbulence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.885033 ntrfc-0.1.5/ntrfc/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/geometry/alphashape.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/geometry/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/geometry/plane.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-07-03 19:37:19.000000 ntrfc-0.1.5/ntrfc/geometry/surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:17.897034 ntrfc-0.1.5/ntrfc/gmsh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/gmsh/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4755 2023-07-08 13:00:17.000000 ntrfc-0.1.5/ntrfc/gmsh/turbo_cascade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:18.003036 ntrfc-0.1.5/ntrfc/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5748 2023-02-25 01:17:42.000000 ntrfc-0.1.5/ntrfc/math/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7212 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/math/vectorcalc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:18.119038 ntrfc-0.1.5/ntrfc/meshquality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:28.000000 ntrfc-0.1.5/ntrfc/meshquality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/meshquality/aspect_ratio.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/meshquality/grid_convergece_index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/meshquality/meshexpansion.py
+-rw-rw-rw-   0 root         (0) root         (0)     8206 2023-06-18 22:04:59.000000 ntrfc-0.1.5/ntrfc/meshquality/nondimensionals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1655 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/meshquality/skewness.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2022-12-20 22:15:49.000000 ntrfc-0.1.5/ntrfc/ntrfc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:18.175039 ntrfc-0.1.5/ntrfc/timeseries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/timeseries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2292 2023-02-25 01:17:42.000000 ntrfc-0.1.5/ntrfc/timeseries/integral_scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    13540 2023-07-03 19:37:19.000000 ntrfc-0.1.5/ntrfc/timeseries/stationarity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:18.748051 ntrfc-0.1.5/ntrfc/turbo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/turbo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:18.887054 ntrfc-0.1.5/ntrfc/turbo/airfoil_generators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/turbo/airfoil_generators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9570 2023-02-25 01:17:42.000000 ntrfc-0.1.5/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-31 22:49:09.000000 ntrfc-0.1.5/ntrfc/turbo/bladeloading.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/turbo/cascade_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     5679 2023-07-05 19:37:09.000000 ntrfc-0.1.5/ntrfc/turbo/domaingen_cascade.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-02-23 16:54:29.000000 ntrfc-0.1.5/ntrfc/turbo/integrals.py
+-rw-rw-rw-   0 root         (0) root         (0)     9047 2023-03-11 00:37:14.000000 ntrfc-0.1.5/ntrfc/turbo/pointcloud_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-03-10 00:28:59.000000 ntrfc-0.1.5/ntrfc/turbo/probegeneration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-05-23 23:15:45.000000 ntrfc-0.1.5/ntrfc/turbo/profile_tele_extraction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:16.677009 ntrfc-0.1.5/ntrfc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5157 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      235 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-10 19:50:15.000000 ntrfc-0.1.5/ntrfc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-10 19:50:19.781072 ntrfc-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-07-08 13:00:17.000000 ntrfc-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:18.942055 ntrfc-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2022-12-20 22:15:49.000000 ntrfc-0.1.5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.002056 ntrfc-0.1.5/tests/cascadecase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/cascadecase/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.003056 ntrfc-0.1.5/tests/cascadecase/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/cascadecase/domain/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-27 19:49:04.000000 ntrfc-0.1.5/tests/cascadecase/domain/test_ntrfc_domaingen_cascade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.071057 ntrfc-0.1.5/tests/cascadecase/solution/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/cascadecase/solution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2023-06-20 23:39:11.000000 ntrfc-0.1.5/tests/cascadecase/solution/test_probecontainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3789 2023-06-20 23:39:11.000000 ntrfc-0.1.5/tests/cascadecase/solution/test_solution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.188060 ntrfc-0.1.5/tests/filehandling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/filehandling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/filehandling/test_ntrfc_datafiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/filehandling/test_ntrfc_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.324062 ntrfc-0.1.5/tests/fluid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 12:45:28.000000 ntrfc-0.1.5/tests/fluid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2023-05-31 22:49:09.000000 ntrfc-0.1.5/tests/fluid/test_ntrfc_fluid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2023-05-31 22:49:09.000000 ntrfc-0.1.5/tests/fluid/test_ntrfc_isentropic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-05-31 22:49:09.000000 ntrfc-0.1.5/tests/fluid/test_ntrfc_turbulence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.384064 ntrfc-0.1.5/tests/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2023-06-27 20:41:02.000000 ntrfc-0.1.5/tests/geometry/test_ntrfc_alphashape.py
+-rw-rw-rw-   0 root         (0) root         (0)     5126 2023-03-11 00:37:14.000000 ntrfc-0.1.5/tests/geometry/test_ntrfc_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/geometry/test_ntrfc_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/geometry/test_ntrfc_plane.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/geometry/test_ntrfc_surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.385064 ntrfc-0.1.5/tests/gmsh/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 13:00:17.000000 ntrfc-0.1.5/tests/gmsh/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-08 13:00:17.000000 ntrfc-0.1.5/tests/gmsh/test_meshing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.435065 ntrfc-0.1.5/tests/math/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/math/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8342 2023-02-27 23:54:57.000000 ntrfc-0.1.5/tests/math/test_ntrfc_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/math/test_ntrfc_vectorcalc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.510066 ntrfc-0.1.5/tests/meshquality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/meshquality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/meshquality/test_ntrfc_aspect_ratio.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/meshquality/test_ntrfc_grid_convergence_index.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/meshquality/test_ntrfc_meshexpansion.py
+-rw-rw-rw-   0 root         (0) root         (0)    13631 2023-06-18 22:04:59.000000 ntrfc-0.1.5/tests/meshquality/test_ntrfc_nondimensionals.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/meshquality/test_ntrfc_skewness.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/test_ntrfc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.532067 ntrfc-0.1.5/tests/timeseries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/timeseries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/timeseries/test_ntrfc_integral_scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    10882 2023-06-27 19:49:04.000000 ntrfc-0.1.5/tests/timeseries/test_ntrfc_stationarity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.628069 ntrfc-0.1.5/tests/turbo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/turbo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:50:19.674070 ntrfc-0.1.5/tests/turbo/airfoil_generators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/turbo/airfoil_generators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-02-23 16:54:29.000000 ntrfc-0.1.5/tests/turbo/airfoil_generators/test_parsec_airfoil_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-05-31 22:49:09.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_bladeloading.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-03-11 00:37:14.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_cascade_geometry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-06-20 23:39:11.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_domaingen_cascade.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_integrals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-03-11 00:37:14.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_pointcloud_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2023-03-11 00:37:14.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_probegeneration.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-02-25 01:17:42.000000 ntrfc-0.1.5/tests/turbo/test_ntrfc_profile_tele_extraction.py
```

### Comparing `ntrfc-0.1.4/CONTRIBUTING.rst` & `ntrfc-0.1.5/CONTRIBUTING.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at  https://github.com/MaNyh/ntrfc/issues
+Report bugs at  https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC/-/issues
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
 Fix Bugs
 ~~~~~~~~
 
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+Look through the issues for bugs. Anything tagged with "bug" and "help
 wanted" is open to whoever wants to implement it.
 
 Implement Features
 ~~~~~~~~~~~~~~~~~~
 
 Start your own feature development or look through the gitlab issues for feature-developments.
 Feel free to create feature branches and merge requests.
@@ -39,15 +39,15 @@
 ~~~~~~~~~~~~~~~~~~~
 
 NTRfC could always use more documentation, whether as part of the official NTRfC docs, in docstrings, or even on the web in blog posts, articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/MaNyh/ntrfc/issues.
+The best way to send feedback is to file an issue at https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC/-/issues .
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -79,21 +79,21 @@
 
     $ flake8 ntrfc tests
     $ python setup.py test or pytest
     $ tox
 
    To get flake8 and tox, just pip install them into your virtualenv.
 
-6. Commit your changes and push your branch to GitHub::
+6. Commit your changes and push your branch to GitLab::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
 
-7. Submit a pull request through the GitHub website.
+7. Submit a pull request through the GitLab website.
 
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
```

### Comparing `ntrfc-0.1.4/LICENSE` & `ntrfc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/PKG-INFO` & `ntrfc-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntrfc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Numerical Test Rig for Cascades. A workflows-library for cfd-analysis of cascade-flows
 Home-page: https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC
 Author: Malte Nyhuis
 Author-email: nyhuis@tfd.uni-hannover.de
 License: MIT license
 Keywords: ntrfc
 Classifier: Development Status :: 3 - Alpha
@@ -16,91 +16,110 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ============
 NTRfC README
 ============
 
-Numerical Test Rig for Cascades.
+**Numerical Test Rig for Cascades.**
 
 
 * Free software: MIT license
 * Documentation: https://ntrfc.readthedocs.io.
 * NTRfC is the base of the (NTRFlows)[https://gitlab.uni-hannover.de/tfd_public/tools/NTRFlows] repository, a workflow for cfd parameter studies
 
 
 
-Features
+**Features**
 
 Easy geometry and post-processing visualization and manipulation with pyvista.
 Tested methods and functions for math, time-series, and mesh quality analysis.
 
-Dependencies
+**Dependencies**
 
-NTRfC v0.1.0 and any following version is based on Python 3.10. Only older versions can be used with older versions of Python. Library requirements will be installed with the package itself.
+- libgl1-mesa-glx (graphics driver)
+- xvfb (virtual Display)
+- libglu1-mesa (gmsh dependency)
+- libxcursor1 (gmsh dependency)
+- libxinerama1 (gmsh dependency)
+
+Current NTRfC versions are based on Python 3.10. Only versions <v0.1.0 can be used with older versions of Python. Library requirements will be installed with the package itself.
 Installation
 
 NTRfC is utilizing powerful and complex dependencies like pyvista and gmsh. We strongly recommend using virtual or conda environments for installation.
 
 For more information, see:
 
     virtualenv: https://pypi.org/project/virtualenv/
     miniconda: https://docs.conda.io/en/latest/miniconda.html
     anaconda: https://docs.anaconda.com/anaconda/install/index.html
     mamba: https://mamba.readthedocs.io/en/latest/installation.html
 
 
+**Installation**
+
+Installation from pypi
+
+```
+pip install ntrfc
+```
 
-### Installation from gitlab with pip
+Installation from gitlab with pip
 
 ```
 pip install git+https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC.git
 ```
 
-### Installation from source
+Installation from source
 
 After cloning the repository, go to the project root dir and type
 
 ```
 python setup.py install
 ```
 
-
-### Editable installation from source with pip
+Editable installation from source with pip
 
 After cloning the repository, go to the project root dir and type
 
 ```
 pip install -e .
 ```
 
 This way you have NTRfC installed but the code is not installed, but linked to the source-code.
 You don't have to reinstall the package after your edits.
 This speeds up testing and will lead to less debugging time.
 
-### Singularity releases
+**Singularity releases**
 
-use a singularity container from ntrfc singularity releases:  https://cloud.sylabs.io/library/nyhuma/ntrflows/ntr.sif].
+Use a singularity container from ntrfc singularity releases:  https://cloud.sylabs.io/library/nyhuma/ntrflows/ntr.sif].
 The containers will come with a virtual graphics card and a xvfb display-server, enabling you to render on hpc-systems and any other unprepared system with limited graphics capability.
 
-## Credits
+**Credits**
 
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template. It uses the following libraries:
 
 - [pyvista](https://github.com/pyvista)
 - [gmsh](http://gmsh.info/)
 - [Cookiecutter](https://github.com/audreyr/cookiecutter)
 - [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
 
 
 =======
 History
 =======
 
-0.1.3 (2023-06-25)
+0.1.5 (2023-07-04)
+------------------
+- bugfixes alphashape
+- initial gmsh intigration
+- jupyternotebook testing
+- improved codecov
+
+0.1.4 (2023-06-25)
 ------------------
 - cleaner structure, more reliability
 - pypi deployment
 - sphynx docs
 - removed bugs
 
 0.1.3 (2023-03-11)
```

### Comparing `ntrfc-0.1.4/README.rst` & `ntrfc-0.1.5/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,86 @@
 ============
 NTRfC README
 ============
 
-Numerical Test Rig for Cascades.
+**Numerical Test Rig for Cascades.**
 
 
 * Free software: MIT license
 * Documentation: https://ntrfc.readthedocs.io.
 * NTRfC is the base of the (NTRFlows)[https://gitlab.uni-hannover.de/tfd_public/tools/NTRFlows] repository, a workflow for cfd parameter studies
 
 
 
-Features
+**Features**
 
 Easy geometry and post-processing visualization and manipulation with pyvista.
 Tested methods and functions for math, time-series, and mesh quality analysis.
 
-Dependencies
+**Dependencies**
 
-NTRfC v0.1.0 and any following version is based on Python 3.10. Only older versions can be used with older versions of Python. Library requirements will be installed with the package itself.
+- libgl1-mesa-glx (graphics driver)
+- xvfb (virtual Display)
+- libglu1-mesa (gmsh dependency)
+- libxcursor1 (gmsh dependency)
+- libxinerama1 (gmsh dependency)
+
+Current NTRfC versions are based on Python 3.10. Only versions <v0.1.0 can be used with older versions of Python. Library requirements will be installed with the package itself.
 Installation
 
 NTRfC is utilizing powerful and complex dependencies like pyvista and gmsh. We strongly recommend using virtual or conda environments for installation.
 
 For more information, see:
 
     virtualenv: https://pypi.org/project/virtualenv/
     miniconda: https://docs.conda.io/en/latest/miniconda.html
     anaconda: https://docs.anaconda.com/anaconda/install/index.html
     mamba: https://mamba.readthedocs.io/en/latest/installation.html
 
 
+**Installation**
+
+Installation from pypi
+
+```
+pip install ntrfc
+```
 
-### Installation from gitlab with pip
+Installation from gitlab with pip
 
 ```
 pip install git+https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC.git
 ```
 
-### Installation from source
+Installation from source
 
 After cloning the repository, go to the project root dir and type
 
 ```
 python setup.py install
 ```
 
-
-### Editable installation from source with pip
+Editable installation from source with pip
 
 After cloning the repository, go to the project root dir and type
 
 ```
 pip install -e .
 ```
 
 This way you have NTRfC installed but the code is not installed, but linked to the source-code.
 You don't have to reinstall the package after your edits.
 This speeds up testing and will lead to less debugging time.
 
-### Singularity releases
+**Singularity releases**
 
-use a singularity container from ntrfc singularity releases:  https://cloud.sylabs.io/library/nyhuma/ntrflows/ntr.sif].
+Use a singularity container from ntrfc singularity releases:  https://cloud.sylabs.io/library/nyhuma/ntrflows/ntr.sif].
 The containers will come with a virtual graphics card and a xvfb display-server, enabling you to render on hpc-systems and any other unprepared system with limited graphics capability.
 
-## Credits
+**Credits**
 
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template. It uses the following libraries:
 
 - [pyvista](https://github.com/pyvista)
 - [gmsh](http://gmsh.info/)
 - [Cookiecutter](https://github.com/audreyr/cookiecutter)
 - [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
```

### Comparing `ntrfc-0.1.4/docs/Makefile` & `ntrfc-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/conf.py` & `ntrfc-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/installation.rst` & `ntrfc-0.1.5/docs/installation.rst`

 * *Files 25% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
 
 From sources
 ------------
 
-The sources for NTRfC can be downloaded from the `Github repo`_.
+The sources for NTRfC can be downloaded from the `https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/MaNyh/ntrfc
+    $ git clone https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC.git
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl -OJL https://github.com/MaNyh/ntrfc/tarball/master
+    $ curl -OJL https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
-.. _Github repo: https://github.com/MaNyh/ntrfc
-.. _tarball: https://github.com/MaNyh/ntrfc/tarball/master
+.. _Github repo: https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC.git
+.. _tarball: https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC.git/tarball/master
```

### Comparing `ntrfc-0.1.4/docs/make.bat` & `ntrfc-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.cascade_case.domain.rst` & `ntrfc-0.1.5/docs/ntrfc.cascade_case.domain.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.cascade_case.solution.case_modules.rst` & `ntrfc-0.1.5/docs/ntrfc.cascade_case.solution.case_modules.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.cascade_case.solution.rst` & `ntrfc-0.1.5/docs/ntrfc.cascade_case.solution.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.filehandling.rst` & `ntrfc-0.1.5/docs/ntrfc.filehandling.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.fluid.rst` & `ntrfc-0.1.5/docs/ntrfc.fluid.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.geometry.rst` & `ntrfc-0.1.5/docs/ntrfc.geometry.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.meshquality.rst` & `ntrfc-0.1.5/docs/ntrfc.meshquality.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.timeseries.rst` & `ntrfc-0.1.5/docs/ntrfc.timeseries.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.turbo.airfoil_generators.rst` & `ntrfc-0.1.5/docs/ntrfc.turbo.airfoil_generators.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/docs/ntrfc.turbo.rst` & `ntrfc-0.1.5/docs/ntrfc.turbo.rst`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/cascade_case/domain.py` & `ntrfc-0.1.5/ntrfc/cascade_case/domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 
 
 @dataclass
 class CascadeDomain2D:
     casemeta: CaseMeta = CaseMeta(tempfile.mkdtemp())
     pressureside: pv.PolyData = None
     suctionside: pv.PolyData = None
+    profilepoints: pv.PolyData = None
+    le_index: int = None
+    te_index: int = None
     yperiodic_low: pv.PolyData = None
     yperiodic_high: pv.PolyData = None
     inlet: pv.PolyData = None
     outlet: pv.PolyData = None
 
+
     def generate_from_cascade_parameters(self, domainparams: DomainParameters):
         # Use params attributes to generate attributes of CascadeDomain2D
-
+        self.profilepoints = domainparams.profile_points
+        self.le_index = domainparams.leading_edge_index
+        self.te_index = domainparams.trailing_edge_index
         x_mids = domainparams.midspoly.points[::, 0]
         y_mids = domainparams.midspoly.points[::, 1]
         beta_leading = domainparams.beta_in
         beta_trailing = domainparams.beta_out
         x_inlet = domainparams.xinlet
         x_outlet = domainparams.xoutlet
         pitch = domainparams.pitch
@@ -78,10 +84,9 @@
         plotter.add_mesh(self.pressureside, color='r', show_edges=True)
         plotter.add_mesh(self.yperiodic_low)
         plotter.add_mesh(self.yperiodic_high)
         plotter.add_mesh(self.inlet)
         plotter.add_mesh(self.outlet)
 
         plotter.add_axes()
-        camera = plotter.camera
-        camera.roll += 90
+        plotter.view_xy()
         plotter.screenshot(os.path.join(self.casemeta.case_root_directory, "domain.png"))
```

### Comparing `ntrfc-0.1.4/ntrfc/cascade_case/utils/domain_utils.py` & `ntrfc-0.1.5/ntrfc/cascade_case/utils/domain_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import tempfile
 from dataclasses import dataclass
-
+import os
 import pyvista as pv
 
 from ntrfc.turbo.pointcloud_methods import extract_geo_paras
 
 
 @dataclass
 class DomainParameters:
@@ -37,34 +38,39 @@
     beta_in: float = None
     beta_out: float = None
     alpha: float = None
     profile_points: pv.PolyData = None
     leading_edge_index: int = None
     trailing_edge_index: int = None
 
-    def plot_domainparas(self):
+    def plot_domainparas(self, figurepath=tempfile.mkdtemp() + "/plot.png"):
         """
         Plot the domain parameters using PyVista.
 
 
         Returns:
             pv.Plotter: The PyVista plotter object used for plotting.
         """
-        plotter = pv.Plotter()
-        plotter.window_size = 6400, 6400
+        if os.getenv('DISPLAY') is None:
+            pv.start_xvfb()  # Start X virtual framebuffer (Xvfb)
+        pv.set_plot_theme('document')
+        plotter = pv.Plotter(off_screen=True)
+        plotter.window_size = 1600, 1600
         # Plot the suction side and pressure side polys
         plotter.add_mesh(self.sspoly, color='b', show_edges=True, label="suction-side")
         plotter.add_mesh(self.pspoly, color='r', show_edges=True, label="pressure-side")
         plotter.add_mesh(self.midspoly, color='k', label="camber")
 
         # Plot the profile points
         plotter.add_points(self.profile_points, point_size=1, color='w', opacity=0.8)
         plotter.add_legend()
         plotter.add_axes()
-        plotter.show(cpos=(0, 0, 1))
+        plotter.view_xy()
+        plotter.screenshot(figurepath)
+        return figurepath
 
     def generate_params_by_pointcloud(self, points, alpha=None):
         sortedPoly, psPoly, ssPoly, ind_vk, ind_hk, midsPoly, beta_leading, beta_trailing, camber_angle, alpha = extract_geo_paras(
             points, alpha)
 
         self.profile_points = sortedPoly
         self.sspoly = ssPoly
```

### Comparing `ntrfc-0.1.4/ntrfc/cascade_case/utils/probecontainer.py` & `ntrfc-0.1.5/ntrfc/cascade_case/utils/probecontainer.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/cascade_case/utils/sliceseries.py` & `ntrfc-0.1.5/ntrfc/cascade_case/utils/sliceseries.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/filehandling/datafiles.py` & `ntrfc-0.1.5/ntrfc/filehandling/datafiles.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/filehandling/mesh.py` & `ntrfc-0.1.5/ntrfc/filehandling/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         The file path to the mesh file to be loaded. The file extension should be one of ".vtk", ".vtp", ".vtu", ".vtm", or ".cgns".
 
     Returns
     -------
     mesh : pyvista.UnstructuredGrid or pyvista.StructuredGrid
         The mesh object constructed from the input file.
     """
-    assert os.path.isfile(path_to_mesh), path_to_mesh + " is not a valid file"
+    assert os.path.isfile(path_to_mesh), f"{path_to_mesh} is not a valid file"
     extension = os.path.splitext(path_to_mesh)[1]
     if extension == ".vtk" or extension == ".vtp" or extension == ".vtu":
         mesh = read_vtk(path_to_mesh)
     elif extension == ".vtm":
         mesh = read_vtm(path_to_mesh)
     elif extension == ".cgns":
         mesh = read_cgns(path_to_mesh)
```

### Comparing `ntrfc-0.1.4/ntrfc/fluid/fluid.py` & `ntrfc-0.1.5/ntrfc/fluid/fluid.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/fluid/isentropic.py` & `ntrfc-0.1.5/ntrfc/fluid/isentropic.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/fluid/turbulence.py` & `ntrfc-0.1.5/ntrfc/fluid/turbulence.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/geometry/alphashape.py` & `ntrfc-0.1.5/ntrfc/geometry/alphashape.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
-from scipy.optimize import minimize
+from scipy import optimize
 from scipy.spatial import Delaunay
+from scipy.spatial.distance import cdist
+from scipy.spatial import distance
 
 
 def calc_concavehull(x, y, alpha):
     """
     origin: https://stackoverflow.com/questions/50549128/boundary-enclosing-a-given-set-of-points/50714300#50714300
     """
     points = []
@@ -107,22 +109,43 @@
     if not len(boundary_lst) == 0:
         for i in range(len(boundary_lst[0])):
             x_new.append(points[boundary_lst[0][i][0]][0])
             y_new.append(points[boundary_lst[0][i][0]][1])
 
     return x_new, y_new
 
-
 def auto_concaveHull(xs, ys):
     # Define the loss function
     def loss(alpha, xs, ys):
         xd, yd = calc_concavehull(xs, ys, alpha)
-        loss = abs(len(xs) - len(xd))
+        if len(xd)==0:
+            return 1e10
+        closed_points = np.stack([xd+[xd[0]], yd+[yd[0]]]).T
+        points_orig = np.stack([xs , ys ]).T
+        centers = (closed_points[:-1] + closed_points[1:]) / 2
+        distances = distance.cdist(centers,points_orig).min(axis=0)
+        loss = np.max(distances)
         return loss
 
-    points = np.stack([xs, ys, np.zeros(len(xs))]).T
-
-    dist = np.max(np.sqrt(np.sum((points[:, None, :] - points) ** 2, axis=-1))) / 2
-
-    result = minimize(loss, dist, args=(xs, ys,), method='nelder-mead').x[0]
+    points = np.column_stack((xs, ys))
+    # Compute the pairwise distances between all points
+    distances = cdist(points, points)
+
+    # Get the smallest and largest distances
+    smallest_distance = np.min(distances[np.nonzero(distances)])  # Ignore zero distances
+    largest_distance = np.max(distances)
+
+    bounds = [(smallest_distance, largest_distance * 4)]
+    x0 = np.mean(distances)
+    stepsize = largest_distance*4
+    result_first_stage = optimize.basinhopping(func=loss, x0=x0,niter=2000,interval=25,niter_success=300,stepsize=stepsize,
+                                   minimizer_kwargs={'args': (xs, ys,), 'method': 'SLSQP', "bounds": bounds},
+                                   disp=False).x[0]
+
+    x0= result_first_stage*.8
+    stepsize = result_first_stage*4
+    bounds = [(result_first_stage/4, result_first_stage * 4)]
+    result= optimize.basinhopping(func=loss, x0=x0,niter=10000,interval=120,niter_success=600,stepsize=stepsize,
+                                   minimizer_kwargs={'args': (xs, ys,), 'method': 'SLSQP', "bounds": bounds},
+                                   disp=False).x[0]
     xans, yans = calc_concavehull(xs, ys, result)
     return xans, yans, result
```

### Comparing `ntrfc-0.1.4/ntrfc/geometry/line.py` & `ntrfc-0.1.5/ntrfc/geometry/line.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/geometry/plane.py` & `ntrfc-0.1.5/ntrfc/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/geometry/surface.py` & `ntrfc-0.1.5/ntrfc/geometry/surface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy as np
+
+
 # import pyvista as pv
 
 
 def calc_dist_from_surface(surface_primary, surface_secondary, verbose=False):
     """
     Distance Between Two Surfaces / A Surface and a Pointcloud
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `ntrfc-0.1.4/ntrfc/math/methods.py` & `ntrfc-0.1.5/ntrfc/math/methods.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/math/vectorcalc.py` & `ntrfc-0.1.5/ntrfc/math/vectorcalc.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/meshquality/aspect_ratio.py` & `ntrfc-0.1.5/ntrfc/meshquality/aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/meshquality/grid_convergece_index.py` & `ntrfc-0.1.5/ntrfc/meshquality/grid_convergece_index.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/meshquality/meshexpansion.py` & `ntrfc-0.1.5/ntrfc/meshquality/meshexpansion.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/meshquality/nondimensionals.py` & `ntrfc-0.1.5/ntrfc/meshquality/nondimensionals.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/meshquality/skewness.py` & `ntrfc-0.1.5/ntrfc/meshquality/skewness.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/timeseries/integral_scales.py` & `ntrfc-0.1.5/ntrfc/timeseries/integral_scales.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/timeseries/stationarity.py` & `ntrfc-0.1.5/ntrfc/timeseries/stationarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pandas as pd
-from matplotlib import pyplot as plt
 from scipy import signal
 from sklearn.decomposition import PCA
 
 from ntrfc.math.methods import minmax_normalize
 
 
 def optimal_bin_width(sample1, sample2):
@@ -132,15 +131,15 @@
     assert len(opt_window) == opt_window_size * 2
     probability_similiarity = smd_probability_compare(opt_window[:opt_window_size], opt_window[opt_window_size:])
 
     if probability_similiarity < 0.96:
         return False, False, False
 
     # Compute the period of the time series
-    freqs, psd = signal.welch(opt_window.T, fs=1, nperseg=opt_window_size  // 2)
+    freqs, psd = signal.welch(opt_window.T, fs=1, nperseg=opt_window_size // 2)
     maxpsdid = np.argmax(psd)
 
     if maxpsdid != 0:
         tperiod = freqs[np.argmax(psd)] ** -1
         nperiods = (opt_window_size + (-opt_window_size % tperiod)) // tperiod
     else:
         tperiod = np.inf
```

### Comparing `ntrfc-0.1.4/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py` & `ntrfc-0.1.5/ntrfc/turbo/airfoil_generators/naca_airfoil_creator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py` & `ntrfc-0.1.5/ntrfc/turbo/airfoil_generators/parsec_airfoil_creator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/turbo/bladeloading.py` & `ntrfc-0.1.5/ntrfc/turbo/bladeloading.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/turbo/cascade_geometry.py` & `ntrfc-0.1.5/ntrfc/turbo/cascade_geometry.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/turbo/domaingen_cascade.py` & `ntrfc-0.1.5/ntrfc/turbo/domaingen_cascade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import tempfile
+
 import numpy as np
 import pyvista as pv
-import tempfile
 
 from ntrfc.turbo.pointcloud_methods import extract_geo_paras, calcMidPassageStreamLine
 
 
 def cascade_2d_domain(profilepoints2d, x_inlet, x_outlet, pitch, unit, blade_shift, alpha, path=False):
     """
     profilepoints2d = 2d numpy array
@@ -56,21 +57,21 @@
 
     inletPoly = pv.Line(*inlet_pts)
     outlet_pts = np.array([per_y_lower.points[per_y_lower.points[::, 0].argmax()],
                            per_y_upper.points[per_y_upper.points[::, 0].argmax()]])
 
     outletPoly = pv.Line(*outlet_pts)
 
-
     p = pv.Plotter(off_screen=True)
     p.add_mesh(outletPoly, color="r")
     p.add_mesh(inletPoly, color="r")
     p.add_mesh(per_y_lower, color="r")
     p.add_mesh(per_y_upper, color="r")
     p.add_mesh(profilepoints2d, color="k")
+    p.view_xy()
     p.screenshot(path)
 
     return sortedPoly, psPoly, ssPoly, per_y_upper, per_y_lower, inletPoly, outletPoly
 
 
 def cascade_3d_domain(sortedPoly, psPoly, ssPoly, per_y_upper, per_y_lower, inletPoly, outletPoly, zspan, avdr=1,
                       path=None):
@@ -109,27 +110,27 @@
 
     inletPoly_lowz = transform(avdr, inletPoly, x_lower, x_upper, zspan, -1)
     inletPoly_highz = transform(avdr, inletPoly, x_lower, x_upper, zspan, 1)
 
     outletPoly_lowz = transform(avdr, outletPoly, x_lower, x_upper, zspan, -1)
     outletPoly_highz = transform(avdr, outletPoly, x_lower, x_upper, zspan, 1)
 
-
     p = pv.Plotter(off_screen=True)
     p.add_mesh(psPoly_lowz, color="r")
     p.add_mesh(psPoly_highz, opacity=0.9)
     p.add_mesh(ssPoly_lowz, opacity=0.9)
     p.add_mesh(ssPoly_highz, opacity=0.9, color="white")
     p.add_mesh(per_y_upper_lowz, opacity=0.9, color="white")
     p.add_mesh(per_y_upper_highz, opacity=0.9, color="white")
     p.add_mesh(per_y_lower_lowz, opacity=0.9, color="white")
     p.add_mesh(per_y_lower_highz, opacity=0.9, color="white")
     p.add_mesh(inletPoly_lowz, opacity=0.9, color="white")
     p.add_mesh(inletPoly_highz, opacity=0.9, color="white")
     p.add_mesh(outletPoly_lowz, opacity=0.9, color="white")
     p.add_mesh(outletPoly_highz, opacity=0.9, color="white")
+    p.view_xy()
     p.screenshot(path)
 
     return sortedPoly_lowz, sortedPoly_high, per_y_upper_lowz, per_y_upper_highz, \
            per_y_lower_lowz, per_y_lower_highz, \
            inletPoly_lowz, inletPoly_highz, \
            outletPoly_lowz, outletPoly_highz
```

### Comparing `ntrfc-0.1.4/ntrfc/turbo/pointcloud_methods.py` & `ntrfc-0.1.5/ntrfc/turbo/pointcloud_methods.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/turbo/probegeneration.py` & `ntrfc-0.1.5/ntrfc/turbo/probegeneration.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc/turbo/profile_tele_extraction.py` & `ntrfc-0.1.5/ntrfc/turbo/profile_tele_extraction.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/ntrfc.egg-info/PKG-INFO` & `ntrfc-0.1.5/ntrfc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntrfc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Numerical Test Rig for Cascades. A workflows-library for cfd-analysis of cascade-flows
 Home-page: https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC
 Author: Malte Nyhuis
 Author-email: nyhuis@tfd.uni-hannover.de
 License: MIT license
 Keywords: ntrfc
 Classifier: Development Status :: 3 - Alpha
@@ -16,91 +16,110 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ============
 NTRfC README
 ============
 
-Numerical Test Rig for Cascades.
+**Numerical Test Rig for Cascades.**
 
 
 * Free software: MIT license
 * Documentation: https://ntrfc.readthedocs.io.
 * NTRfC is the base of the (NTRFlows)[https://gitlab.uni-hannover.de/tfd_public/tools/NTRFlows] repository, a workflow for cfd parameter studies
 
 
 
-Features
+**Features**
 
 Easy geometry and post-processing visualization and manipulation with pyvista.
 Tested methods and functions for math, time-series, and mesh quality analysis.
 
-Dependencies
+**Dependencies**
 
-NTRfC v0.1.0 and any following version is based on Python 3.10. Only older versions can be used with older versions of Python. Library requirements will be installed with the package itself.
+- libgl1-mesa-glx (graphics driver)
+- xvfb (virtual Display)
+- libglu1-mesa (gmsh dependency)
+- libxcursor1 (gmsh dependency)
+- libxinerama1 (gmsh dependency)
+
+Current NTRfC versions are based on Python 3.10. Only versions <v0.1.0 can be used with older versions of Python. Library requirements will be installed with the package itself.
 Installation
 
 NTRfC is utilizing powerful and complex dependencies like pyvista and gmsh. We strongly recommend using virtual or conda environments for installation.
 
 For more information, see:
 
     virtualenv: https://pypi.org/project/virtualenv/
     miniconda: https://docs.conda.io/en/latest/miniconda.html
     anaconda: https://docs.anaconda.com/anaconda/install/index.html
     mamba: https://mamba.readthedocs.io/en/latest/installation.html
 
 
+**Installation**
+
+Installation from pypi
+
+```
+pip install ntrfc
+```
 
-### Installation from gitlab with pip
+Installation from gitlab with pip
 
 ```
 pip install git+https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC.git
 ```
 
-### Installation from source
+Installation from source
 
 After cloning the repository, go to the project root dir and type
 
 ```
 python setup.py install
 ```
 
-
-### Editable installation from source with pip
+Editable installation from source with pip
 
 After cloning the repository, go to the project root dir and type
 
 ```
 pip install -e .
 ```
 
 This way you have NTRfC installed but the code is not installed, but linked to the source-code.
 You don't have to reinstall the package after your edits.
 This speeds up testing and will lead to less debugging time.
 
-### Singularity releases
+**Singularity releases**
 
-use a singularity container from ntrfc singularity releases:  https://cloud.sylabs.io/library/nyhuma/ntrflows/ntr.sif].
+Use a singularity container from ntrfc singularity releases:  https://cloud.sylabs.io/library/nyhuma/ntrflows/ntr.sif].
 The containers will come with a virtual graphics card and a xvfb display-server, enabling you to render on hpc-systems and any other unprepared system with limited graphics capability.
 
-## Credits
+**Credits**
 
 This package was created with Cookiecutter and the `audreyr/cookiecutter-pypackage` project template. It uses the following libraries:
 
 - [pyvista](https://github.com/pyvista)
 - [gmsh](http://gmsh.info/)
 - [Cookiecutter](https://github.com/audreyr/cookiecutter)
 - [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
 
 
 =======
 History
 =======
 
-0.1.3 (2023-06-25)
+0.1.5 (2023-07-04)
+------------------
+- bugfixes alphashape
+- initial gmsh intigration
+- jupyternotebook testing
+- improved codecov
+
+0.1.4 (2023-06-25)
 ------------------
 - cleaner structure, more reliability
 - pypi deployment
 - sphynx docs
 - removed bugs
 
 0.1.3 (2023-03-11)
```

### Comparing `ntrfc-0.1.4/setup.py` & `ntrfc-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,18 @@
             'ntrfc=ntrfc.cli:main',
         ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
+    package_data={
+        'ntrfc': ['data/*'],
+    },
     keywords='ntrfc',
     packages=find_packages(include=['ntrfc', 'ntrfc.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://gitlab.uni-hannover.de/tfd_public/tools/NTRfC',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

### Comparing `ntrfc-0.1.4/tests/cascadecase/domain/test_ntrfc_domaingen_cascade.py` & `ntrfc-0.1.5/tests/cascadecase/domain/test_ntrfc_domaingen_cascade.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import os
+
+ON_CI = 'CI' in os.environ
+
 def test_cascade_2d_domain():
     import pyvista as pv
     import numpy as np
     from ntrfc.cascade_case.utils.domain_utils import DomainParameters
     from ntrfc.cascade_case.domain import CascadeDomain2D
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
     xs, ys = naca("6510", 256)
@@ -9,10 +13,11 @@
     alpha = 1
     domainparas = DomainParameters()
     domainparas.generate_params_by_pointcloud(points, alpha=alpha)
     domainparas.xinlet = -3
     domainparas.xoutlet = 4
     domainparas.pitch = 2
     domainparas.blade_yshift = 0.1
+    domainparas.plot_domainparas()
     domain2d = CascadeDomain2D()
     domain2d.generate_from_cascade_parameters(domainparas)
     domain2d.plot_domain()
```

### Comparing `ntrfc-0.1.4/tests/cascadecase/solution/test_probecontainer.py` & `ntrfc-0.1.5/tests/cascadecase/solution/test_probecontainer.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/cascadecase/solution/test_solution.py` & `ntrfc-0.1.5/tests/cascadecase/solution/test_solution.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/filehandling/test_ntrfc_datafiles.py` & `ntrfc-0.1.5/tests/filehandling/test_ntrfc_datafiles.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/filehandling/test_ntrfc_mesh.py` & `ntrfc-0.1.5/tests/filehandling/test_ntrfc_mesh.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/fluid/test_ntrfc_fluid.py` & `ntrfc-0.1.5/tests/fluid/test_ntrfc_fluid.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/fluid/test_ntrfc_isentropic.py` & `ntrfc-0.1.5/tests/fluid/test_ntrfc_isentropic.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/fluid/test_ntrfc_turbulence.py` & `ntrfc-0.1.5/tests/fluid/test_ntrfc_turbulence.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/geometry/test_ntrfc_alphashape.py` & `ntrfc-0.1.5/tests/geometry/test_ntrfc_alphashape.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     import pyvista as pv
     from ntrfc.turbo.airfoil_generators.naca_airfoil_creator import naca
 
     square = pv.Plane()
     boxedges = square.extract_feature_edges()
 
     boxedges.rotate_z(np.random.randint(0, 360), inplace=True)
-    boxpoints = boxedges.points
+    boxpoints = boxedges.points*np.random.randn()*1000
 
     np.random.shuffle(boxpoints)
 
     xs_raw = boxpoints[:, 0]
     ys_raw = boxpoints[:, 1]
 
     xs, ys, alpha = auto_concaveHull(xs_raw, ys_raw)
@@ -61,12 +61,12 @@
     assert len(xs) == len(xs_raw)
     assert any([yi in ys_raw for yi in ys])
 
     digit_string = "6509"
 
     res = 240
     X, Y = naca(digit_string, res, half_cosine_spacing=True)
-    points = np.stack((X[:], Y[:], np.zeros(res * 2))).T
+    points = np.stack((X[:], Y[:], np.zeros(res * 2))).T*np.random.randn()*1000
 
     xs, ys, alpha = auto_concaveHull(points[::, 0], points[::, 1])
 
     assert len(xs) == len(X)
```

### Comparing `ntrfc-0.1.4/tests/geometry/test_ntrfc_geometry.py` & `ntrfc-0.1.5/tests/geometry/test_ntrfc_geometry.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/geometry/test_ntrfc_line.py` & `ntrfc-0.1.5/tests/geometry/test_ntrfc_line.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/geometry/test_ntrfc_plane.py` & `ntrfc-0.1.5/tests/geometry/test_ntrfc_plane.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/math/test_ntrfc_methods.py` & `ntrfc-0.1.5/tests/math/test_ntrfc_methods.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/math/test_ntrfc_vectorcalc.py` & `ntrfc-0.1.5/tests/math/test_ntrfc_vectorcalc.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/meshquality/test_ntrfc_aspect_ratio.py` & `ntrfc-0.1.5/tests/meshquality/test_ntrfc_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/meshquality/test_ntrfc_grid_convergence_index.py` & `ntrfc-0.1.5/tests/meshquality/test_ntrfc_grid_convergence_index.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/meshquality/test_ntrfc_meshexpansion.py` & `ntrfc-0.1.5/tests/meshquality/test_ntrfc_meshexpansion.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/meshquality/test_ntrfc_nondimensionals.py` & `ntrfc-0.1.5/tests/meshquality/test_ntrfc_nondimensionals.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/meshquality/test_ntrfc_skewness.py` & `ntrfc-0.1.5/tests/meshquality/test_ntrfc_skewness.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/timeseries/test_ntrfc_integral_scales.py` & `ntrfc-0.1.5/tests/timeseries/test_ntrfc_integral_scales.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/timeseries/test_ntrfc_stationarity.py` & `ntrfc-0.1.5/tests/timeseries/test_ntrfc_stationarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
+import pyvista as pv
 
 ON_CI = 'CI' in os.environ
 
+if ON_CI:
+    pv.start_xvfb()
 
 def test_optimal_timewindow(verbose=False):
     from ntrfc.timeseries.stationarity import optimal_window_size
     import numpy as np
     # sine
     res = 10000
```

### Comparing `ntrfc-0.1.4/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py` & `ntrfc-0.1.5/tests/turbo/airfoil_generators/test_naca_airfoil_creator.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_bladeloading.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_bladeloading.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_cascade_geometry.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_cascade_geometry.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_domaingen_cascade.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_domaingen_cascade.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_integrals.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_integrals.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_pointcloud_methods.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_pointcloud_methods.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_probegeneration.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_probegeneration.py`

 * *Files identical despite different names*

### Comparing `ntrfc-0.1.4/tests/turbo/test_ntrfc_profile_tele_extraction.py` & `ntrfc-0.1.5/tests/turbo/test_ntrfc_profile_tele_extraction.py`

 * *Files identical despite different names*

