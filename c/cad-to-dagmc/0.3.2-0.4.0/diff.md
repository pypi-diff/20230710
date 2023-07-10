# Comparing `tmp/cad_to_dagmc-0.3.2.tar.gz` & `tmp/cad_to_dagmc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cad_to_dagmc-0.3.2.tar", last modified: Thu Jun  1 21:41:48 2023, max compression
+gzip compressed data, was "cad_to_dagmc-0.4.0.tar", last modified: Mon Jul 10 06:06:31 2023, max compression
```

## Comparing `cad_to_dagmc-0.3.2.tar` & `cad_to_dagmc-0.4.0.tar`

### file list

```diff
@@ -1,76 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.270050 cad_to_dagmc-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/anaconda-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_object_and_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/create_stp_files_for_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/curved_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/multiple_cadquery_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/multiple_stp_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/single_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/single_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/single_stp_file_multiple_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/src/cad_to_dagmc/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/brep_part_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/brep_to_h5m.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/vertices_to_h5m.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.278050 cad_to_dagmc-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    71272 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/ENDFB-7.1-NNDC_H1.h5
--rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/extrude_rectangle.stp
--rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/multi_volume_cylinders.stp
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/single_cube.stp
--rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/single_volume_thin.stp
--rw-r--r--   0 runner    (1001) docker     (123)  2013134 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/single_volume_thin.vtk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.278050 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/
--rw-r--r--   0 runner    (1001) docker     (123)   267095 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/ball_reactor.brep
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_brep_part_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_id_with_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/create_brep_file_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/one_cube.brep
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_brep_file.brep
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_h5m_in_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_python_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_joined_cubes.brep
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_sep_cubes.brep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/
--rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/extrude_rectangle.stp
--rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/multi_volume_cylinders.stp
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_cube.stp
--rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_volume_thin.stp
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_in_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_connected_cubes.stp
--rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_disconnected_cubes.stp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/tests/test_vertices_to_h5m/
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_vertices_to_h5m/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/two_connected_cubes.stp
--rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.677799 cad_to_dagmc-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.665799 cad_to_dagmc-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.669799 cad_to_dagmc-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/.github/workflows/anaconda-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-10 06:06:31.677799 cad_to_dagmc-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.669799 cad_to_dagmc-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/cadquery_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/cadquery_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/cadquery_object_and_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/cadquery_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/create_stp_files_for_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/curved_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/multiple_cadquery_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/multiple_stp_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/single_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/single_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/examples/single_stp_file_multiple_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:06:31.677799 cad_to_dagmc-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.669799 cad_to_dagmc-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 06:06:31.000000 cad_to_dagmc-0.4.0/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.669799 cad_to_dagmc-0.4.0/src/cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc/brep_part_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc/brep_to_h5m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc/vertices_to_h5m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.669799 cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-10 06:06:31.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-10 06:06:31.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:06:31.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 06:06:31.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 06:06:31.000000 cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.673799 cad_to_dagmc-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    71272 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/ENDFB-7.1-NNDC_H1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (123)  2013134 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/single_volume_thin.vtk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.673799 cad_to_dagmc-0.4.0/tests/test_brep_part_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)   267095 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_part_finder/ball_reactor.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.673799 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/create_brep_file_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/one_cube.brep
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_brep_file.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_h5m_in_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_python_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_two_joined_cubes.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_two_sep_cubes.brep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.677799 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (123)  1760716 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/curved_extrude.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/test_h5m_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/test_h5m_in_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:06:31.677799 cad_to_dagmc-0.4.0/tests/test_vertices_to_h5m/
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/test_vertices_to_h5m/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-07-10 06:06:16.000000 cad_to_dagmc-0.4.0/tests/two_disconnected_cubes.stp
```

### Comparing `cad_to_dagmc-0.3.2/.github/workflows/anaconda-publish.yml` & `cad_to_dagmc-0.4.0/.github/workflows/anaconda-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/.github/workflows/black.yml` & `cad_to_dagmc-0.4.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/.github/workflows/python-publish.yml` & `cad_to_dagmc-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/.gitignore` & `cad_to_dagmc-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/LICENSE` & `cad_to_dagmc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/PKG-INFO` & `cad_to_dagmc-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: cad_to_dagmc
-Version: 0.3.2
-Summary: Converts CAD files to a DAGMC h5m file
-Author-email: Jonathan Shimwell <mail@jshimwell.com>
-Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
-Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
-Keywords: dagmc,geometry,plot,slice
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 
 [![N|Python](https://www.python.org/static/community_logos/python-powered-w-100x40.png)](https://www.python.org)
 
 [![CI with install](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml)
 
 [![Upload Python Package](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml)
 
@@ -30,60 +14,82 @@
 
 This particular method of producing DAGMC compatible h5m files from CAD geometry
 is intended to convert STP files or [CadQuery](https://cadquery.readthedocs.io) objects to h5m file.
 
 One unique feature of this package is the ability to combine STP files with CadQuery objects.
 This allows for the addition of parametric geometry to static geometry.
 
-# Install (Conda)
+# Installation
+
+In principle, any Conda distribution will work. 
+
 
-Creates a new empty Conda environment and activate it
+# Install using Conda and pip
+
+This example uses Conda to install some dependencies that are not available via PyPi.
+
+Create a new conda environment
+```bash
+conda create --name new_env python=3.9 -y
+```
+
+Activate the environment
 ```bash
-conda create --name new_env python=3.9
 conda activate new_env
 ```
 
-Installs cad_to_dagmc and dependencies
+Install the dependencies
 ```bash
-conda install -c conda-forge cad_to_dagmc
+conda install -c conda-forge moab multimethod typish ezdxf nptyping nlopt casadi gmsh python-gmsh ocp>=7.7.1 -y
+conda install -c cadquery -c conda-forge cadquery=master --no-deps -y
 ```
-# Install (Mamba)
 
-Creates a new empty Conda environment and activate it
+Then you can install the cad_to_dagmc package with ```pip```
 ```bash
-conda create --name new_env python=3.9
-conda activate new_env
+pip install cad_to_dagmc
 ```
 
-Installs Mamba
+You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).You can run ```conda install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
 ```bash
-conda install -c conda-forge mamba
+conda install -c conda-forge -y "openmc=0.13.3=dagmc*nompi*"
 ```
 
-Installs cad_to_dagmc and dependencies
+
+# Install using Mamba and pip
+
+This example uses Mamba to install some dependencies that are not available via PyPi.
+
+Create a new conda environment, I've chosen Python 3.9 here but new versions are
+also supported.
 ```bash
-mamba install -c conda-forge cad_to_dagmc
+conda create --name new_env python=3.9 -y
 ```
 
-# Install (Conda + pip)
+Activate the environment
+```bash
+mamba activate new_env
+```
 
-You will need to install some dependencies that are not available via PyPi.
-This example uses Conda but Mamba could also be used.
+Install the dependencies
 ```bash
-conda install -c conda-forge moab
-conda install -c conda-forge gmsh
-conda install -c conda-forge python-gmsh
+conda install -c conda-forge mamba -y
+mamba install -c conda-forge moab multimethod typish ezdxf nptyping nlopt casadi gmsh python-gmsh ocp>=7.7.1 -y
+mamba install -c cadquery -c conda-forge cadquery=master --no-deps -y
 ```
 
 Then you can install the cad_to_dagmc package with ```pip```
-
 ```bash
 pip install cad_to_dagmc
 ```
 
-# Usage
+You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).You can run ```conda install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
+```bash
+mamba install -c conda-forge -y "openmc=0.13.3=dagmc*nompi*"
+```
 
-To use the h5m geometry you will need a transport code with DAGMC enabled such as OpenMC.
-Just to note that currently the conda install for CadQuery and OpenMC can't be installed in the same conda environment.
-A work around for this is to create the h5m geometry in one conda environment and simulate with OpenMC in another conda environment.
+# Usage - creation of DAGMC h5m files
 
 For examples see the [examples folder](https://github.com/fusion-energy/cad_to_dagmc/tree/main/examples)
+
+# Usage - simulation with transport code
+
+For examples see the CAD tasks in the [neutronics-workshop](https://github.com/fusion-energy/neutronics-workshop)
```

### Comparing `cad_to_dagmc-0.3.2/examples/cadquery_compound.py` & `cad_to_dagmc-0.4.0/examples/cadquery_compound.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/examples/create_stp_files_for_examples.py` & `cad_to_dagmc-0.4.0/examples/create_stp_files_for_examples.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/examples/curved_cadquery_object.py` & `cad_to_dagmc-0.4.0/examples/curved_cadquery_object.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/pyproject.toml` & `cad_to_dagmc-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 keywords = ["dagmc", "geometry", "plot", "slice"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "cadquery>=2.2.0",
     "trimesh",
     "networkx",
 ]
 dynamic = ["version"]
 
 
 [tool.setuptools_scm]
```

### Comparing `cad_to_dagmc-0.3.2/src/cad_to_dagmc/__init__.py` & `cad_to_dagmc-0.4.0/src/cad_to_dagmc/__init__.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/src/cad_to_dagmc/core.py` & `cad_to_dagmc-0.4.0/src/cad_to_dagmc/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from tempfile import mkstemp
-
 import typing
 from cadquery import importers
-from cadquery import Assembly
-from OCP.GCPnts import GCPnts_QuasiUniformDeflection
+
+# from cadquery import Assembly
+# from OCP.GCPnts import GCPnts_QuasiUniformDeflection
 
 # from cadquery.occ_impl import shapes
 import OCP
 import cadquery as cq
-from OCP.TopLoc import TopLoc_Location
-from OCP.BRep import BRep_Tool
-from OCP.TopAbs import TopAbs_Orientation
 
-from .brep_to_h5m import brep_to_h5m
+# from OCP.TopLoc import TopLoc_Location
+# from OCP.BRep import BRep_Tool
+# from OCP.TopAbs import TopAbs_Orientation
+
+from .brep_to_h5m import mesh_brep, mesh_to_h5m_in_memory_method
 from .brep_part_finder import (
-    get_part_properties_from_shapes,
-    get_part_properties_from_shapes,
-    get_matching_part_ids,
+    get_ids_from_assembly,
+    get_ids_from_imprinted_assembly,
+    order_material_ids_by_brep_order,
 )
 
 
 class CadToDagmc:
     def __init__(self):
         self.parts = []
         self.material_tags = []
@@ -41,15 +41,15 @@
                 STP file and match the material tags used in the neutronics
                 code (e.g. OpenMC).
             scale_factor: a scaling factor to apply to the geometry that can be
                 used to increase the size or decrease the size of the geometry.
                 Useful when converting the geometry to cm for use in neutronics
                 simulations.
         """
-
+        print(f"loading stp file {filename}")
         part = importers.importStep(str(filename)).val()
 
         if scale_factor == 1:
             scaled_part = part
         else:
             scaled_part = part.scale(scale_factor)
         self.add_cadquery_object(object=scaled_part, material_tags=material_tags)
@@ -90,75 +90,82 @@
             self.material_tags.append(material_tag)
 
     def export_dagmc_h5m_file(
         self,
         filename: str = "dagmc.h5m",
         min_mesh_size: float = 1,
         max_mesh_size: float = 10,
-        verbose: bool = False,
-        volume_atol: float = 0.000001,
-        center_atol: float = 0.000001,
-        bounding_box_atol: float = 0.000001,
+        mesh_algorithm: int = 1,
     ):
-        brep_shape = self._merge_surfaces()
-
-        tmp_brep_filename = mkstemp(suffix=".brep", prefix="paramak_")[1]
-        brep_shape.exportBrep(tmp_brep_filename)
-
-        if verbose:
-            print(f"Brep file saved to {tmp_brep_filename}")
-
-        brep_file_part_properties = get_part_properties_from_shapes(brep_shape)
+        assembly = cq.Assembly()
+        for part in self.parts:
+            assembly.add(part)
+
+        (
+            imprinted_assembly,
+            imprinted_solids_with_original_id,
+        ) = cq.occ_impl.assembly.imprint(assembly)
+
+        original_ids = get_ids_from_assembly(assembly)
+        scrambled_ids = get_ids_from_imprinted_assembly(
+            imprinted_solids_with_original_id
+        )
 
-        shape_properties = get_part_properties_from_shapes(self.parts)
+        # both id lists should be the same length as each other and the same
+        # length as the self.material_tags
 
-        brep_and_shape_part_ids = get_matching_part_ids(
-            brep_part_properties=brep_file_part_properties,
-            shape_properties=shape_properties,
-            volume_atol=volume_atol,
-            center_atol=center_atol,
-            bounding_box_atol=bounding_box_atol,
+        material_tags_in_brep_order = order_material_ids_by_brep_order(
+            original_ids, scrambled_ids, self.material_tags
         )
 
-        material_tags_in_brep_order = []
-        for brep_id, shape_id in brep_and_shape_part_ids:
-            material_tags_in_brep_order.append(self.material_tags[shape_id - 1])
+        gmsh, volumes = mesh_brep(
+            brep_object=imprinted_assembly.wrapped._address(),
+            min_mesh_size=min_mesh_size,
+            max_mesh_size=max_mesh_size,
+            mesh_algorithm=mesh_algorithm,
+        )
 
-        brep_to_h5m(
-            brep_filename=tmp_brep_filename,
+        h5m_filename = mesh_to_h5m_in_memory_method(
+            volumes=volumes,
             material_tags=material_tags_in_brep_order,
             h5m_filename=filename,
-            min_mesh_size=min_mesh_size,
-            max_mesh_size=max_mesh_size,
         )
+        return h5m_filename
 
-    def _merge_surfaces(self):
-        """Merges surfaces in the geometry that are the same. More details on
-        the merging process in the DAGMC docs
-        https://svalinn.github.io/DAGMC/usersguide/cubit_basics.html"""
 
-        # solids = geometry.Solids()
+def merge_surfaces(parts):
+    """Merges surfaces in the geometry that are the same. More details on
+    the merging process in the DAGMC docs
+    https://svalinn.github.io/DAGMC/usersguide/cubit_basics.html"""
 
-        bldr = OCP.BOPAlgo.BOPAlgo_Splitter()
+    # solids = geometry.Solids()
 
-        if len(self.parts) == 1:
-            # merged_solid = cq.Compound(solids)
-            return self.parts[0]
+    bldr = OCP.BOPAlgo.BOPAlgo_Splitter()
 
-        for solid in self.parts:
-            # checks if solid is a compound as .val() is not needed for compounds
-            if isinstance(
-                solid, (cq.occ_impl.shapes.Compound, cq.occ_impl.shapes.Solid)
-            ):
-                bldr.AddArgument(solid.wrapped)
-            else:
-                bldr.AddArgument(solid.val().wrapped)
+    if len(parts) == 1:
+        # merged_solid = cq.Compound(solids)
+
+        if isinstance(
+            parts[0], (cq.occ_impl.shapes.Compound, cq.occ_impl.shapes.Solid)
+        ):
+            # stp file
+            return parts[0], parts[0].wrapped
+        else:
+            return parts[0], parts[0].toOCC()
+
+    # else:
+    for solid in parts:
+        # checks if solid is a compound as .val() is not needed for compounds
+        if isinstance(solid, (cq.occ_impl.shapes.Compound, cq.occ_impl.shapes.Solid)):
+            bldr.AddArgument(solid.wrapped)
+        else:
+            bldr.AddArgument(solid.val().wrapped)
 
-        bldr.SetNonDestructive(True)
+    bldr.SetNonDestructive(True)
 
-        bldr.Perform()
+    bldr.Perform()
 
-        bldr.Images()
+    bldr.Images()
 
-        merged_solid = cq.Compound(bldr.Shape())
+    merged_solid = cq.Compound(bldr.Shape())
 
-        return merged_solid
+    return merged_solid, merged_solid.wrapped
```

### Comparing `cad_to_dagmc-0.3.2/src/cad_to_dagmc/vertices_to_h5m.py` & `cad_to_dagmc-0.4.0/src/cad_to_dagmc/vertices_to_h5m.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,7 +203,9 @@
     all_sets = moab_core.get_entities_by_handle(0)
 
     file_set = moab_core.create_meshset()
 
     moab_core.add_entities(file_set, all_sets)
 
     moab_core.write_file(h5m_filename)
+
+    return h5m_filename
```

### Comparing `cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/PKG-INFO` & `cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cad-to-dagmc
-Version: 0.3.2
+Version: 0.4.0
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,60 +30,82 @@
 
 This particular method of producing DAGMC compatible h5m files from CAD geometry
 is intended to convert STP files or [CadQuery](https://cadquery.readthedocs.io) objects to h5m file.
 
 One unique feature of this package is the ability to combine STP files with CadQuery objects.
 This allows for the addition of parametric geometry to static geometry.
 
-# Install (Conda)
+# Installation
 
-Creates a new empty Conda environment and activate it
+In principle, any Conda distribution will work. 
+
+
+# Install using Conda and pip
+
+This example uses Conda to install some dependencies that are not available via PyPi.
+
+Create a new conda environment
+```bash
+conda create --name new_env python=3.9 -y
+```
+
+Activate the environment
 ```bash
-conda create --name new_env python=3.9
 conda activate new_env
 ```
 
-Installs cad_to_dagmc and dependencies
+Install the dependencies
 ```bash
-conda install -c conda-forge cad_to_dagmc
+conda install -c conda-forge moab multimethod typish ezdxf nptyping nlopt casadi gmsh python-gmsh ocp>=7.7.1 -y
+conda install -c cadquery -c conda-forge cadquery=master --no-deps -y
 ```
-# Install (Mamba)
 
-Creates a new empty Conda environment and activate it
+Then you can install the cad_to_dagmc package with ```pip```
 ```bash
-conda create --name new_env python=3.9
-conda activate new_env
+pip install cad_to_dagmc
 ```
 
-Installs Mamba
+You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).You can run ```conda install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
 ```bash
-conda install -c conda-forge mamba
+conda install -c conda-forge -y "openmc=0.13.3=dagmc*nompi*"
 ```
 
-Installs cad_to_dagmc and dependencies
+
+# Install using Mamba and pip
+
+This example uses Mamba to install some dependencies that are not available via PyPi.
+
+Create a new conda environment, I've chosen Python 3.9 here but new versions are
+also supported.
 ```bash
-mamba install -c conda-forge cad_to_dagmc
+conda create --name new_env python=3.9 -y
 ```
 
-# Install (Conda + pip)
+Activate the environment
+```bash
+mamba activate new_env
+```
 
-You will need to install some dependencies that are not available via PyPi.
-This example uses Conda but Mamba could also be used.
+Install the dependencies
 ```bash
-conda install -c conda-forge moab
-conda install -c conda-forge gmsh
-conda install -c conda-forge python-gmsh
+conda install -c conda-forge mamba -y
+mamba install -c conda-forge moab multimethod typish ezdxf nptyping nlopt casadi gmsh python-gmsh ocp>=7.7.1 -y
+mamba install -c cadquery -c conda-forge cadquery=master --no-deps -y
 ```
 
 Then you can install the cad_to_dagmc package with ```pip```
-
 ```bash
 pip install cad_to_dagmc
 ```
 
-# Usage
+You may also want to install OpenMC with DAGMC to make use of the h5m geometry files produced in simulations. However you could also use other supported particle transport codes such as MCNP, FLUKA and others [link to DAGMC documentation](https://svalinn.github.io/DAGMC/).You can run ```conda install -c conda-forge openmc``` however this more specific command makes sure the latest version of OpenMC which contains DAGMC is chosen by conda / mamba
+```bash
+mamba install -c conda-forge -y "openmc=0.13.3=dagmc*nompi*"
+```
 
-To use the h5m geometry you will need a transport code with DAGMC enabled such as OpenMC.
-Just to note that currently the conda install for CadQuery and OpenMC can't be installed in the same conda environment.
-A work around for this is to create the h5m geometry in one conda environment and simulate with OpenMC in another conda environment.
+# Usage - creation of DAGMC h5m files
 
 For examples see the [examples folder](https://github.com/fusion-energy/cad_to_dagmc/tree/main/examples)
+
+# Usage - simulation with transport code
+
+For examples see the CAD tasks in the [neutronics-workshop](https://github.com/fusion-energy/neutronics-workshop)
```

### Comparing `cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/SOURCES.txt` & `cad_to_dagmc-0.4.0/src/cad_to_dagmc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .gitignore
 LICENSE
 README.md
-environment.yml
 pyproject.toml
 .github/workflows/anaconda-publish.yml
 .github/workflows/black.yml
 .github/workflows/ci_with_install.yml
 .github/workflows/python-publish.yml
 examples/cadquery_assembly.py
 examples/cadquery_compound.py
@@ -34,26 +33,23 @@
 tests/multi_volume_cylinders.stp
 tests/single_cube.stp
 tests/single_volume_thin.stp
 tests/single_volume_thin.vtk
 tests/two_connected_cubes.stp
 tests/two_disconnected_cubes.stp
 tests/test_brep_part_finder/ball_reactor.brep
-tests/test_brep_part_finder/test_get_brep_part_properties.py
-tests/test_brep_part_finder/test_get_matching_part_id.py
-tests/test_brep_part_finder/test_get_matching_part_id_with_file.py
-tests/test_brep_part_finder/test_get_matching_part_ids.py
 tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py
 tests/test_brep_to_h5m/create_brep_file_for_testing.py
 tests/test_brep_to_h5m/one_cube.brep
 tests/test_brep_to_h5m/test_brep_file.brep
 tests/test_brep_to_h5m/test_h5m_in_transport.py
 tests/test_brep_to_h5m/test_python_api.py
 tests/test_brep_to_h5m/test_two_joined_cubes.brep
 tests/test_brep_to_h5m/test_two_sep_cubes.brep
+tests/test_cad_to_dagmc/curved_extrude.stp
 tests/test_cad_to_dagmc/extrude_rectangle.stp
 tests/test_cad_to_dagmc/multi_volume_cylinders.stp
 tests/test_cad_to_dagmc/single_cube.stp
 tests/test_cad_to_dagmc/single_volume_thin.stp
 tests/test_cad_to_dagmc/test_h5m_creation.py
 tests/test_cad_to_dagmc/test_h5m_in_simulation.py
 tests/test_cad_to_dagmc/test_version.py
```

### Comparing `cad_to_dagmc-0.3.2/tests/ENDFB-7.1-NNDC_H1.h5` & `cad_to_dagmc-0.4.0/tests/ENDFB-7.1-NNDC_H1.h5`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/extrude_rectangle.stp` & `cad_to_dagmc-0.4.0/tests/extrude_rectangle.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/multi_volume_cylinders.stp` & `cad_to_dagmc-0.4.0/tests/multi_volume_cylinders.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/single_cube.stp` & `cad_to_dagmc-0.4.0/tests/single_cube.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/single_volume_thin.stp` & `cad_to_dagmc-0.4.0/tests/single_volume_thin.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/single_volume_thin.vtk` & `cad_to_dagmc-0.4.0/tests/single_volume_thin.vtk`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/ball_reactor.brep` & `cad_to_dagmc-0.4.0/tests/test_brep_part_finder/ball_reactor.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/create_brep_file_for_testing.py` & `cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/create_brep_file_for_testing.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/one_cube.brep` & `cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/one_cube.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_brep_file.brep` & `cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_brep_file.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_joined_cubes.brep` & `cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_two_joined_cubes.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_sep_cubes.brep` & `cad_to_dagmc-0.4.0/tests/test_brep_to_h5m/test_two_sep_cubes.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/extrude_rectangle.stp` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/extrude_rectangle.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/multi_volume_cylinders.stp` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/multi_volume_cylinders.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_cube.stp` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/single_cube.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_volume_thin.stp` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/single_volume_thin.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_creation.py` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/test_h5m_creation.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,31 +43,37 @@
                 vol_mat[id] = group_name
     return vol_mat
 
 
 def test_h5m_with_single_volume_list():
     """Simple geometry, a single 4 sided shape"""
 
-    stp_files = [
-        "tests/test_cad_to_dagmc/extrude_rectangle.stp",
-        "tests/test_cad_to_dagmc/single_cube.stp",
-        # "tests/test_cad_to_dagmc/single_volume_thin.stp", currently slow to mesh
-    ]
-    h5m_files = [
-        "tests/test_cad_to_dagmc/extrude_rectangle.h5m",
-        "tests/test_cad_to_dagmc/single_cube.h5m",
-        # "tests/test_cad_to_dagmc/single_volume_thin.h5m", currently slow to mesh
-    ]
+    h5m_file = "tests/test_cad_to_dagmc/single_cube.h5m"
+
+    my_model = CadToDagmc()
+    my_model.add_stp_file(
+        filename="tests/test_cad_to_dagmc/single_cube.stp", material_tags=["mat1"]
+    )
+    my_model.export_dagmc_h5m_file(filename=h5m_file)
+
+    assert get_volumes_and_materials_from_h5m(h5m_file) == {1: "mat:mat1"}
+
+
+def test_h5m_with_single_volume_2():
+    """Simple geometry, a single 4 sided shape"""
+
+    h5m_file = "tests/test_cad_to_dagmc/curved_extrude.h5m"
 
-    for stp_file, h5m_file in zip(stp_files, h5m_files):
-        my_model = CadToDagmc()
-        my_model.add_stp_file(filename=stp_file, material_tags=["mat1"])
-        my_model.export_dagmc_h5m_file(filename=h5m_file)
+    my_model = CadToDagmc()
+    my_model.add_stp_file(
+        filename="tests/test_cad_to_dagmc/curved_extrude.stp", material_tags=["mat1"]
+    )
+    my_model.export_dagmc_h5m_file(filename=h5m_file)
 
-        assert get_volumes_and_materials_from_h5m(h5m_file) == {1: "mat:mat1"}
+    assert get_volumes_and_materials_from_h5m(h5m_file) == {1: "mat:mat1"}
 
 
 def test_h5m_with_multi_volume_not_touching():
     stp_files = [
         "tests/test_cad_to_dagmc/two_disconnected_cubes.stp",
     ]
     material_tags = [
```

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_in_simulation.py` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/test_h5m_in_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     my_model.run()
 
 
 def test_h5m_with_single_volume_list():
     """The simplest geometry, a single 4 sided shape with lists instead of np arrays"""
 
     h5m_files = [
-        "tests/test_cad_to_dagmc/extrude_rectangle.h5m",
+        # "tests/test_cad_to_dagmc/extrude_rectangle.h5m",
         "tests/test_cad_to_dagmc/single_cube.h5m",
         # "tests/test_cad_to_dagmc/single_volume_thin.h5m",
     ]
 
     for h5m_file in h5m_files:
         transport_particles_on_h5m_geometry(
             h5m_filename=h5m_file,
```

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_version.py` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/test_version.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_connected_cubes.stp` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/two_connected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_disconnected_cubes.stp` & `cad_to_dagmc-0.4.0/tests/test_cad_to_dagmc/two_disconnected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/test_vertices_to_h5m/test_package.py` & `cad_to_dagmc-0.4.0/tests/test_vertices_to_h5m/test_package.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/two_connected_cubes.stp` & `cad_to_dagmc-0.4.0/tests/two_connected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.2/tests/two_disconnected_cubes.stp` & `cad_to_dagmc-0.4.0/tests/two_disconnected_cubes.stp`

 * *Files identical despite different names*

