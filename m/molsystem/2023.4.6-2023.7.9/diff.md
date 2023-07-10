# Comparing `tmp/molsystem-2023.4.6.tar.gz` & `tmp/molsystem-2023.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molsystem-2023.4.6.tar", last modified: Thu Apr  6 15:46:21 2023, max compression
+gzip compressed data, was "molsystem-2023.7.9.tar", last modified: Mon Jul 10 17:31:09 2023, max compression
```

## Comparing `molsystem-2023.4.6.tar` & `molsystem-2023.7.9.tar`

### file list

```diff
@@ -1,96 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.784197 molsystem-2023.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-06 15:46:03.000000 molsystem-2023.4.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-06 15:46:03.000000 molsystem-2023.4.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-06 15:46:03.000000 molsystem-2023.4.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-06 15:46:03.000000 molsystem-2023.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 15:46:03.000000 molsystem-2023.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-06 15:46:21.784197 molsystem-2023.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-06 15:46:03.000000 molsystem-2023.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.772196 molsystem-2023.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8695 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.772196 molsystem-2023.4.6/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/developer/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/developer/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/developer/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/developer/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/molsystem.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.772196 molsystem-2023.4.6/docs/user/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 15:46:03.000000 molsystem-2023.4.6/docs/user/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.784197 molsystem-2023.4.6/molsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-06 15:46:21.784197 molsystem-2023.4.6/molsystem/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    43965 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26481 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19758 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)    33626 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/cms_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    29373 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/configuration_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.776197 molsystem-2023.4.6/molsystem/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/data/standard_properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/frozencolumn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/molfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/openbabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26461 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/rdkit_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    32871 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/system_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/system_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    26849 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-04-06 15:46:03.000000 molsystem-2023.4.6/molsystem/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.776197 molsystem-2023.4.6/molsystem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-06 15:46:21.000000 molsystem-2023.4.6/molsystem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-06 15:46:21.000000 molsystem-2023.4.6/molsystem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:46:21.000000 molsystem-2023.4.6/molsystem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 15:46:21.000000 molsystem-2023.4.6/molsystem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 15:46:21.000000 molsystem-2023.4.6/molsystem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-06 15:46:21.784197 molsystem-2023.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-06 15:46:03.000000 molsystem-2023.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.780197 molsystem-2023.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:46:21.784197 molsystem-2023.4.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269083 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/data/1n9v.cif
--rw-r--r--   0 runner    (1001) docker     (123)  1055288 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/data/aa-variants-v1.cif
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/data/acy.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)   117392 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/data/aminoacids.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/data/hoh.mmcif
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_angiotensin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_configuration_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_molfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_openbabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_property_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_rdkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_system_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-06 15:46:03.000000 molsystem-2023.4.6/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-06 15:46:03.000000 molsystem-2023.4.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.740878 molsystem-2023.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 17:30:46.000000 molsystem-2023.7.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-10 17:30:46.000000 molsystem-2023.7.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-10 17:30:46.000000 molsystem-2023.7.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-10 17:30:46.000000 molsystem-2023.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-10 17:30:46.000000 molsystem-2023.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-10 17:31:09.740878 molsystem-2023.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-10 17:30:46.000000 molsystem-2023.7.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.724878 molsystem-2023.7.9/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 17:30:46.000000 molsystem-2023.7.9/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.744878 molsystem-2023.7.9/molsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 17:31:09.744878 molsystem-2023.7.9/molsystem/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26433 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33626 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/cms_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/configuration_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.732878 molsystem-2023.7.9/molsystem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/data/standard_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/frozencolumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/molfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28940 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/rdkit_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32852 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/system_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-07-10 17:30:46.000000 molsystem-2023.7.9/molsystem/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.732878 molsystem-2023.7.9/molsystem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 17:31:09.000000 molsystem-2023.7.9/molsystem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-10 17:31:09.740878 molsystem-2023.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-10 17:30:46.000000 molsystem-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.736878 molsystem-2023.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:31:09.740878 molsystem-2023.7.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269083 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/1n9v.cif
+-rw-r--r--   0 runner    (1001) docker     (123)  1055288 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/aa-variants-v1.cif
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/acy.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)   117392 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/aminoacids.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/data/hoh.mmcif
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_angiotensin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_configuration_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_molfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_property_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_system_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-10 17:30:46.000000 molsystem-2023.7.9/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-10 17:30:46.000000 molsystem-2023.7.9/versioneer.py
```

### Comparing `molsystem-2023.4.6/CONTRIBUTING.rst` & `molsystem-2023.7.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/HISTORY.rst` & `molsystem-2023.7.9/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =======
 History
 =======
 
+2023.7.9 -- Added JSON properties
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
+      
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.4.6/LICENSE` & `molsystem-2023.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/PKG-INFO` & `molsystem-2023.7.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2023.4.6
+Version: 2023.7.9
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -23,54 +23,79 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
 MolSystem
 =============
 
-
-.. image:: https://img.shields.io/travis/molssi-seamm/molsystem.svg
-           :target: https://travis-ci.org/molssi-seamm/molsystem
-	   :alt: Build Status
+.. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/dftbplus_step
+   :target: https://github.com/molssi-seamm/molsystem/pulls
+   :alt: GitHub pull requests
+
+.. image:: https://github.com/molssi-seamm/molsystem/workflows/CI/badge.svg
+   :target: https://github.com/molssi-seamm/molsystem/actions
+   :alt: Build Status
 
 .. image:: https://codecov.io/gh/molssi-seamm/molsystem/branch/master/graph/badge.svg
-	   :target: https://codecov.io/gh/molssi-seamm/molsystem
-	   :alt: Code Coverage
+   :target: https://codecov.io/gh/molssi-seamm/molsystem
+   :alt: Code Coverage
 
-.. image:: https://img.shields.io/lgtm/grade/python/g/molssi-seamm/molsystem.svg?logo=lgtm&logoWidth=18
-	   :target: https://lgtm.com/projects/g/molssi-seamm/molsystem/context:python
-	   :alt: Code Quality
-
-.. image:: https://readthedocs.org/projects/molsystem/badge/?version=latest
-           :target: https://molsystem.readthedocs.io/en/latest/?badge=latest
-	   :alt: Documentation Status
-
-.. image:: https://pyup.io/repos/github/molssi-seamm/molsystem/shield.svg
-	   :target: https://pyup.io/repos/github/molssi-seamm/molsystem/
-	   :alt: Updates for Dependencies
+.. image:: https://github.com/molssi-seamm/molsystem/workflows/CodeQL/badge.svg
+   :target: https://github.com/molssi-seamm/molsystem/security/code-scanning
+   :alt: Code Quality
 
-.. image:: https://img.shields.io/pypi/v/molsystem.svg
-           :target: https://pypi.python.org/pypi/molsystem
-	   :alt: PyPi VERSION
 
-Molsystem provides a general class for handling molecular and periodic systems
+.. image:: https://github.com/molssi-seamm/molsystem/workflows/Release/badge.svg
+   :target: https://molssi-seamm.github.io/molsystem/index.html
+   :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/v/molsystem.svg
+   :target: https://pypi.python.org/pypi/molsystem
+   :alt: PyPi VERSION
+
+Description
+-----------
+Molsystem provides a general class for handling molecular and periodic systems. This is
+the heart of SEAMM.
 
 * Free software: GNU Lesser General Public License v3+
 * Documentation: https://molsystem.readthedocs.io.
 
 
 Features
 --------
 
-* Complete the initial version!
-
-  * Remove the coordinates from the Atoms class and allow for multiple
-    sets of coordinates -- conformers, trajectories, etc.
-  * Provide a concept of the 'current' system
+* Supports molecular and periodic (crystalline) systems.
+* Support for pointgroup and spacegroup symmetry.
+* Implemented as a SQL database, currently using SQLite, which provides permanence and a
+  disk file.
+* Handles multiple systems, and for each system any number of
+  configurations. Configurations are different structures, generally having different
+  coordinates. Examples are conformers or frames in an MD trajectory.
+* Configurations can have differing bonds, supporting reactive forcefields such as
+  ReaxFF.
+* Configurations can also have differing numbers of atoms, supporting e.g. grand
+  canonical Monte Carlo.
+* Support for templates and subsets. Templates can be used for creating or finding
+  structures in systems and subsets hold substes of atoms. An atom can be in multiple
+  subsets. For proteins, subsets can be used for residues and chains; for polymers,
+  monomers; and for fluids the subsets can track individual molecules.
+* Subsets and templates handle the correspondance between atoms so if, for instance, the
+  ordering of atoms in residues are different, that can be handled using the
+  correspondances.
+* Direct connection to and support of RDKit and OpenBabel molecules, allowing direct
+  transfer back and forth between configurations and those libraries.
+* Properties of systems and configurations are stored in fact tables of integers,
+  floats, strings, and JSON, using a star schema. One of the dimensions is metadata
+  describing the property. This data warehousing approach is almost identical to that
+  used in CIF files, with the metadata being the CIF dictionaries.
+* Good support of CIF files, with the ability to store data other than the actual atoms
+  using the properties warehouse.
+* Direct support for SMILES, SMARTS and substructure searching.
+* Scales to millions of systems and configurations, and databases in excess of 100 GB.
 
 Credits
 ---------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -85,14 +110,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.9 -- Added JSON properties
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
+      
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.4.6/docs/Makefile` & `molsystem-2023.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/docs/conf.py` & `molsystem-2023.7.9/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,18 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.githubpages',
     'sphinx.ext.napoleon',
-    'sphinx.ext.viewcode'
+    'sphinx.ext.viewcode',
+    'sphinx_design',
+    'sphinx_copybutton',
+    'sphinx.ext.todo',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -57,15 +60,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'MolSystem'
-copyright = u"2020, Molecular Sciences Software Institute (MolSSI)"
+copyright = u"2020-2023, Molecular Sciences Software Institute (MolSSI)"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = molsystem.__version__
@@ -98,34 +101,54 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = 'default'
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built
 # documents.
 # keep_warnings = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'sphinx_rtd_theme'
+html_theme = "pydata_sphinx_theme"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
+html_theme_options = {
+    "github_url": "https://github.com/molssi-seamm/molsystem",
+    "twitter_url": "https://twitter.com/MolSSI_NSF",
+    "icon_links": [],
+    "logo": {
+        "image_light": "SEAMM logo.png",
+        "image_dark": "SEAMM Inverted 288x181.png",
+        "text": "LAMMPS Step",
+        "molssi_light": "molssi_main_logo.png",
+        "molssi_dark": "molssi_main_logo_inverted_white.png",
+    },
+    "show_toc_level": 2,
+    "header_links_before_dropdown": 4,
+    "external_links": [
+        {"name": "SEAMM Documentation", "url": "https://molssi-seamm.github.io"},
+        {"name": "MolSSI", "url": "https://molssi.org"}
+    ],
+    "secondary_sidebar_items": ["page-toc", "sourcelink"],
+    "footer_items": [ "molssi_footer" ],
+}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
```

### Comparing `molsystem-2023.4.6/docs/developer/installation.rst` & `molsystem-2023.7.9/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/docs/make.bat` & `molsystem-2023.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/__init__.py` & `molsystem-2023.7.9/molsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/atoms.py` & `molsystem-2023.7.9/molsystem/atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """A dictionary-like object for holding atoms.
 """
 
 from itertools import zip_longest
 import logging
-import pprint  # noqa: F401
 from typing import Any, Dict, TypeVar
 
 import numpy
 import pandas
 
 from molsystem import elements
 from .column import _Column
@@ -22,16 +21,15 @@
 
 def grouped(iterable, n):
     "s -> (s0,s1,s2,...sn-1), (sn,sn+1,sn+2,...s2n-1), (s2n,...s3n-1), ..."
     return zip_longest(*[iter(iterable)] * n)
 
 
 class _Atoms(_Table):
-    """:meta public:
-    The atoms in a configuration of a system.
+    """The atoms in a configuration of a system.
 
     Parameters
     ----------
     configuration : _Configuration
         The configuration of interest.
     """
 
@@ -1038,26 +1036,22 @@
         columns = [f'at."{x}"' for x in atom_columns]
         columns += [f'co."{x}"' for x in coordinates_columns]
 
         return columns
 
 
 class _SubsetAtoms(_Atoms):
-    """:meta public:
-    The atoms in a subset.
+    """The atoms in a subset.
 
     Parameters
     ----------
     configuration : _Configuration
         The configuration of interest.
     subset_id : int
         The id of the subset.
-
-    Attributes
-    ----------
     template_order : bool
         Whether to return atoms and properties in the order of the template
         if the template is full. Defaults to True.
     """
 
     def __init__(self, configuration, subset_id) -> None:
         self._sid = subset_id
```

### Comparing `molsystem-2023.4.6/molsystem/bonds.py` & `molsystem-2023.7.9/molsystem/bonds.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 
 def grouped(iterable, n):
     "s -> (s0,s1,s2,...sn-1), (sn,sn+1,sn+2,...s2n-1), (s2n,...s3n-1), ..."
     return zip_longest(*[iter(iterable)] * n)
 
 
 class _Bonds(_Table):
-    """The Bonds class describes the bonds in the system.
-
-    :meta public:
-    """
+    """The Bonds class describes the bonds in the system."""
 
     def __init__(self, configuration):
         self._configuration = configuration
 
         self._system = None
 
         self._bondset = self._configuration.bondset
@@ -655,18 +652,15 @@
 
         df = pandas.DataFrame.from_dict(data, orient="index", columns=columns)
 
         return df
 
 
 class _SubsetBonds(_Bonds):
-    """The Bonds class describes the bonds in a subset
-
-    :meta public:
-    """
+    """The Bonds class describes the bonds in a subset"""
 
     def __init__(self, configuration, subset_id):
         self._sid = subset_id
 
         # Caching
         self._template_id = None
         self._template = None
```

### Comparing `molsystem-2023.4.6/molsystem/cell.py` & `molsystem-2023.7.9/molsystem/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,16 +428,14 @@
 
 
 class _Cell(Cell):
     """A class for handling cell parameters as part of MolSystem.
 
     Provides all the functionality of the Cell class, but keeps the cell
     data in the database.
-
-    :meta public:
     """
 
     def __init__(self, configuration):
         """Initialize from the database.
 
         Parameters
         ----------
```

### Comparing `molsystem-2023.4.6/molsystem/cif.py` & `molsystem-2023.7.9/molsystem/cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/cms_schema.py` & `molsystem-2023.7.9/molsystem/cms_schema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/column.py` & `molsystem-2023.7.9/molsystem/column.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/configuration.py` & `molsystem-2023.7.9/molsystem/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,18 +36,15 @@
     SMILESMixin,
     TopologyMixin,
     OpenBabelMixin,
     RDKitMixin,
     QCSchemaMixin,
     object,
 ):
-    """A configuration (conformer) of a system.
-
-    :meta public:
-    """
+    """A configuration (conformer) of a system."""
 
     def __init__(self, _id, system_db):
         self._id = _id
         self._system_db = system_db
 
         self._name = None
         self._system = None
```

### Comparing `molsystem-2023.4.6/molsystem/configuration_properties.py` & `molsystem-2023.7.9/molsystem/configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/data/standard_properties.csv` & `molsystem-2023.7.9/molsystem/data/standard_properties.csv`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/elements.py` & `molsystem-2023.7.9/molsystem/elements.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/frozencolumn.py` & `molsystem-2023.7.9/molsystem/frozencolumn.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/molfile.py` & `molsystem-2023.7.9/molsystem/molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/openbabel.py` & `molsystem-2023.7.9/molsystem/openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/pdb.py` & `molsystem-2023.7.9/molsystem/pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/properties.py` & `molsystem-2023.7.9/molsystem/properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import csv
+import json
 import logging
 from pathlib import Path
 import pkg_resources
-import pprint  # noqa: F401
 
 logger = logging.getLogger(__name__)
 standard_properties = {}
 
 
 def add_properties_from_file(path):
     """The standard properties recognized by SEAMM.
@@ -121,15 +121,15 @@
         ----
         If the property is registered in the list of standard properties, just
         give the name and the rest will be filled in from the standard property
         metadata.
         """
         if self.exists(name):
             if noerror:
-                return self.property_id(name)
+                return self.id(name)
             else:
                 raise ValueError(f"Property '{name}' already exists.")
 
         table = self.system_db["property"]
         if name in self.standard_properties:
             data = self.standard_properties[name]
             result = table.append(
@@ -250,14 +250,46 @@
             "CREATE INDEX str_data_idx_system_property  ON str_data(system, property)"
         )
         self.db.execute(
             "CREATE INDEX str_data_idx_configuration ON str_data(configuration)"
         )
         self.db.execute("CREATE INDEX str_data_idx_system ON str_data(system)")
 
+        # Integer facts
+        table = self.system_db["json_data"]
+        table.add_attribute("id", coltype="int", pk=True)
+        table.add_attribute("configuration", coltype="int", references="configuration")
+        table.add_attribute("system", coltype="int", references="system")
+        table.add_attribute("property", coltype="int", references="property")
+        table.add_attribute("value", coltype="str")
+
+        self.db.execute(
+            "CREATE INDEX json_data_idx_configuration_property_value"
+            "    ON json_data(configuration, property, value)"
+        )
+        self.db.execute(
+            "CREATE INDEX json_data_idx_system_property_value"
+            "    ON json_data(system, property, value)"
+        )
+        self.db.execute(
+            "CREATE INDEX json_data_idx_property_value"
+            "    ON json_data(property, value)"
+        )
+        self.db.execute(
+            "CREATE INDEX json_data_idx_configuration_property"
+            "    ON json_data(configuration, property)"
+        )
+        self.db.execute(
+            "CREATE INDEX json_data_idx_system_property ON json_data(system, property)"
+        )
+        self.db.execute(
+            "CREATE INDEX json_data_idx_configuration ON json_data(configuration)"
+        )
+        self.db.execute("CREATE INDEX json_data_idx_system ON json_data(system)")
+
     def description(self, _property):
         """The description of a property
 
         Parameters
         ----------
         _property : int or str
             The id or name of the property.
@@ -308,51 +340,66 @@
             sql += "SELECT name, type, value"
             sql += "  FROM property, int_data"
             sql += " WHERE int_data.property = property.id AND configuration = ?"
             sql += " UNION "
             sql += "SELECT name, type, value"
             sql += "  FROM property, str_data"
             sql += " WHERE str_data.property = property.id AND configuration = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, json_data"
+            sql += " WHERE json_data.property = property.id AND configuration = ?"
 
             self.cursor.execute(
-                sql, (configuration_id, configuration_id, configuration_id)
+                sql,
+                (
+                    configuration_id,
+                    configuration_id,
+                    configuration_id,
+                    configuration_id,
+                ),
             )
 
             result = {}
             for row in self.cursor:
                 name, _type, value = row
                 if _type == "float":
                     result[name] = float(value)
                 elif _type == "int":
                     result[name] = int(value)
+                elif _type == "json":
+                    result[name] = json.loads(value)
                 else:
                     result[name] = value
             return result
         else:
             if isinstance(_property, str):
                 if self.exists(_property):
-                    pid = self.property_id(_property)
+                    pid = self.id(_property)
                 else:
                     raise ValueError(f"Property '{_property}' does not exist.")
             else:
                 pid = _property
 
-            ptype = self.property_type(pid)
+            ptype = self.type(pid)
             sql = (
                 f"SELECT value FROM {ptype}_data"
                 "  WHERE configuration = ? AND property = ?"
             )
             self.cursor.execute(sql, (configuration_id, pid))
             result = self.cursor.fetchone()
             if result is None:
                 raise ValueError(
                     f"Property {_property} does not exist for configuration "
                     f"{configuration_id}"
                 )
-            return result[0]
+            if ptype == "json":
+                return json.loads(result[0])
+            else:
+                return result[0]
 
     def get_for_system(self, system_id, _property="all"):
         """Get the given property value(s) for the system.
 
         Parameters
         ----------
         system_id : int
@@ -373,40 +420,49 @@
             sql += "SELECT name, type, value"
             sql += "  FROM property, int_data"
             sql += " WHERE int_data.property = property.id AND system = ?"
             sql += " UNION "
             sql += "SELECT name, type, value"
             sql += "  FROM property, str_data"
             sql += " WHERE str_data.property = property.id AND system = ?"
+            sql += " UNION "
+            sql += "SELECT name, type, value"
+            sql += "  FROM property, json_data"
+            sql += " WHERE json_data.property = property.id AND system = ?"
 
-            self.cursor.execute(sql, (system_id, system_id, system_id))
+            self.cursor.execute(sql, (system_id, system_id, system_id, system_id))
 
             result = {}
             for row in self.cursor:
                 name, _type, value = row
                 if _type == "float":
                     result[name] = float(value)
                 elif _type == "int":
                     result[name] = int(value)
+                elif _type == "json":
+                    result[name] = json.loads(value)
                 else:
                     result[name] = value
         else:
             if isinstance(_property, str):
                 if self.exists(_property):
-                    pid = self.property_id(_property)
+                    pid = self.id(_property)
                 else:
                     raise ValueError(f"Property '{_property}' does not exist.")
             else:
                 pid = _property
-            ptype = self.property_type(pid)
+            ptype = self.type(pid)
 
             sql = f"SELECT value FROM {ptype}_data WHERE system = ? AND property = ?"
             result = []
             for row in self.db.execute(sql, (system_id, pid)):
-                result.append(row[0])
+                if ptype == "json":
+                    result.append(json.loads(row[0]))
+                else:
+                    result.append(row[0])
 
         return result
 
     def id(self, name):
         """The id for a property
 
         Parameters
@@ -511,18 +567,21 @@
         # Get the property id and type
         if isinstance(_property, str):
             if not self.exists(_property):
                 if _property in self.standard_properties:
                     self.add(_property)
                 else:
                     raise ValueError(f"Property '{_property}' does not exist.")
-            pid = self.property_id(_property)
+            pid = self.id(_property)
         else:
             pid = _property
-        ptype = self.property_type(pid)
+        ptype = self.type(pid)
+
+        if ptype == "json":
+            value = json.dumps(value, separators=(",", ":"))
 
         # Get the system id
         self.cursor.execute(
             "SELECT system FROM configuration WHERE id = ?", (configuration_id,)
         )
         system_id = self.cursor.fetchone()[0]
 
@@ -547,18 +606,21 @@
         # Get the property id and type
         if isinstance(_property, str):
             if not self.exists(_property):
                 if _property in self.standard_properties:
                     self.add(_property)
                 else:
                     raise ValueError(f"Property '{_property}' does not exist.")
-            pid = self.property_id(_property)
+            pid = self.id(_property)
         else:
             pid = _property
-        ptype = self.property_type(pid)
+        ptype = self.type(pid)
+
+        if ptype == "json":
+            value = json.dumps(value, separators=(",", ":"))
 
         sql = (
             f"INSERT INTO {ptype}_data (system, property, value)"
             "      VALUES(?, ?, ?)"
         )
         self.db.execute(sql, (system_id, pid, value))
 
@@ -575,50 +637,54 @@
         (property, operator, value). The property
         """
         sql = "SELECT"
         where = "WHERE"
         criteria = []
         tables = {}
         results = []
+        types = []
         n_tables = 0
         for i, item in enumerate(what):
             if i > 0:
                 sql += ","
             if isinstance(item, str):
                 if item == "configuration":
                     sql += " t0.configuration"
                     results.append("configuration_id")
+                    types.append["configuration"]
                 else:
-                    pid = self.property_id(item)
-                    ptype = self.property_type(pid)
+                    pid = self.id(item)
+                    ptype = self.type(pid)
                     table = ptype + "_data"
                     if table not in tables:
                         tables[table] = {pid: f"t{n_tables}"}
                         n_tables += 1
                     elif pid not in tables[table]:
                         tables[table][pid] = f"t{n_tables}"
                         n_tables += 1
                     alias = tables[table][pid]
                     sql += f" {alias}.value"
                     criteria.append(f"{alias}.property == {pid}")
                     results.append(item)
+                    types.append(ptype)
             elif isinstance(item, int):
                 pid = item
-                ptype = self.property_type(pid)
+                ptype = self.type(pid)
                 table = ptype + "_data"
                 if table not in tables:
                     tables[table] = {pid: f"t{n_tables}"}
                     n_tables += 1
                 elif pid not in tables[table]:
                     tables[table][pid] = f"t{n_tables}"
                     n_tables += 1
                 alias = tables[table][pid]
                 sql += f" {alias}.value"
                 criteria.append(f"{alias}.property == {pid}")
-                results.append(self.property_name(pid))
+                results.append(self.name(pid))
+                types.append(ptype)
 
         # And the WHERE clause ...
         where = {0: ""}
         items = iter(args)
         level = 0
         for item in items:
             if item == "(":
@@ -628,57 +694,54 @@
                 where[level] += ")"
                 where[level - 1] += where[level]
                 del where[level]
                 level -= 1
             else:
                 # Configuration or Property name or id
                 if isinstance(item, str):
-                    pid = self.property_id(item)
-                    ptype = self.property_type(pid)
-                    table = ptype + "_data"
-                    if table not in tables:
-                        tables[table] = {pid: f"t{n_tables}"}
-                        n_tables += 1
-                    elif pid not in tables[table]:
-                        tables[table][pid] = f"t{n_tables}"
-                        n_tables += 1
-                    alias = tables[table][pid]
-                    if where[level] != "" and where[level] != "( ":
-                        where[level] += " AND"
-                    where[level] += f" {alias}.property == {pid}"
-                elif isinstance(item, int):
+                    pid = self.id(item)
+                else:
                     pid = item
-                    ptype = self.property_type(pid)
-                    table = ptype + "_data"
-                    if table not in tables:
-                        tables[table] = {pid: f"t{n_tables}"}
-                        n_tables += 1
-                    elif pid not in tables[table]:
-                        tables[table][pid] = f"t{n_tables}"
-                        n_tables += 1
-                    alias = tables[table][pid]
-                    if where[level] != "" and where[level] != "( ":
-                        where[level] += " AND"
-                    where[level] += f" {alias}.property == {pid}"
+                ptype = self.type(pid)
+                table = ptype + "_data"
+                if table not in tables:
+                    tables[table] = {pid: f"t{n_tables}"}
+                    n_tables += 1
+                elif pid not in tables[table]:
+                    tables[table][pid] = f"t{n_tables}"
+                    n_tables += 1
+                alias = tables[table][pid]
+                if where[level] != "" and where[level] != "( ":
+                    where[level] += " AND"
+                where[level] += f" {alias}.property == {pid}"
 
                 operator = next(items)
                 if operator.lower() == "between":
                     if ptype == "str":
                         where[level] += (
                             f' AND {alias}.value BETWEEN "{next(items)}"'
                             f' AND "{next(items)}"'
                         )
+                    if ptype == "json":
+                        value1 = json.dumps(next(items), separator=(",", ":"))
+                        value2 = json.dumps(next(items), separator=(",", ":"))
+                        where[
+                            level
+                        ] += f' AND {alias}.value BETWEEN "{value1}" AND "{value2}"'
                     else:
                         where[level] += (
                             f" AND {alias}.value BETWEEN {next(items)}"
                             f" AND {next(items)}"
                         )
                 else:
                     if ptype == "str":
                         where[level] += f' AND {alias}.value {operator} "{next(items)}"'
+                    elif ptype == "json":
+                        value = json.dumps(next(items), separator=(",", ":"))
+                        where[level] += f' AND {alias}.value {operator} "{value}"'
                     else:
                         where[level] += f" AND {alias}.value {operator} {next(items)}"
 
         # Put it all together ... FROM clause plus needed criteria
         # if len(tables) == 0:
         #     # No tables ... so probably getting all configurations with properties
         #     tables = ["int_data", "float_data", "str_data"]
@@ -719,16 +782,19 @@
             print("")
             print(f"{tmp=}")
             print(f"{criteria=}")
             print(f"{where[0]=}")
             raise
 
         for row in self.cursor:
-            for item, value in zip(results, row):
-                result[item].append(value)
+            for item, ptype, value in zip(results, types, row):
+                if ptype == "json":
+                    result[item].append(json.loads(value))
+                else:
+                    result[item].append(value)
         return result
 
     def type(self, _property):
         """The type of a property
 
         Parameters
         ----------
```

### Comparing `molsystem-2023.4.6/molsystem/qcschema.py` & `molsystem-2023.7.9/molsystem/qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/rdkit_.py` & `molsystem-2023.7.9/molsystem/rdkit_.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/smiles.py` & `molsystem-2023.7.9/molsystem/smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/subset.py` & `molsystem-2023.7.9/molsystem/subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from .smiles import SMILESMixin
 from .template import _Template
 
 logger = logging.getLogger(__name__)
 
 
 class _Subset(SMILESMixin, OpenBabelMixin, object):
-    """:meta public:
-    A class providing the API for a subset.
+    """A class providing the API for a subset.
 
     Parameters
     ----------
     sid : int
         The id of the subset in the subset table.
     logger : logging.Logger = logger
         A logger to use in place of the one from this module.
```

### Comparing `molsystem-2023.4.6/molsystem/subsets.py` & `molsystem-2023.7.9/molsystem/subsets.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 
     Parameters
     ----------
     configuration : _Configuration
         The configuration to work with.
     logger : Logger
         The logger to use, defaults to the one for this module.
-
-    :meta public:
     """
 
     def __init__(self, configuration, logger=logger):
         self._configuration = configuration
         self.logger = logger
 
         self._cid = configuration.id
```

### Comparing `molsystem-2023.4.6/molsystem/symmetry.py` & `molsystem-2023.7.9/molsystem/symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 
 import spglib
 
 logger = logging.getLogger(__name__)
 
 
 class _Symmetry(object):
-    """A class to handle point and space group symmetry.
-
-    :meta public:
-    """
+    """A class to handle point and space group symmetry."""
 
     spgno_to_hall = None
     spgname_to_hall = None
 
     def __init__(self, configuration):
         """Initialize from the database.
```

### Comparing `molsystem-2023.4.6/molsystem/system.py` & `molsystem-2023.7.9/molsystem/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,16 +83,14 @@
     numbers or types of atoms in the system, or if the bonding changes,
     there will be multiple versions of the subset, each corresponding to
     a different set of atoms or bonds.
 
     One or more configurations are connected with each 'all' subset,
     which is how the atoms and bonding are connected to the
     configurations.
-
-    :meta public:
     """
 
     def __init__(self, system_db, _id, logger=logger):
         self._system_db = system_db
         self._id = _id
         self.logger = logger
         self._current_configuration_id = None  # The current configuration
```

### Comparing `molsystem-2023.4.6/molsystem/system_db.py` & `molsystem-2023.7.9/molsystem/system_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,14 @@
 
     bondset
         A set of bonds, used with a joining table to connect bonds
         with configurations.
 
     bondset_bond
         The joining table connecting bondsets with their bonds.
-
-    :meta public:
     """
 
     def __init__(self, parent=None, logger=logger, **kwargs):
         self._parent = parent
         self.logger = logger
         self._attached = {}
         self._current_system_id = None  # The id of the current system
```

### Comparing `molsystem-2023.4.6/molsystem/system_properties.py` & `molsystem-2023.7.9/molsystem/system_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem/table.py` & `molsystem-2023.7.9/molsystem/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
     This is a wrapper around an SQL table, with columns being the attributes.
 
     Attributes can be created, either from a list of predefined
     ones or by specifying the metadata required of an attribute. Attributes can
     also be deleted. See the method 'add_attribute' for more detail.
 
     Rows can be added ('append') or deleted ('delete').
-
-    :meta public:
     """
 
     def __init__(self, system_db, table: str, other=None, logger=logger):
         self._system_db = system_db
         self.logger = logger
         if "." in table:
             self._schema, self._table = table.split(".")
```

### Comparing `molsystem-2023.4.6/molsystem/template.py` & `molsystem-2023.7.9/molsystem/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from .openbabel import OpenBabelMixin
 from .smiles import SMILESMixin
 
 logger = logging.getLogger(__name__)
 
 
 class _Template(SMILESMixin, OpenBabelMixin, object):
-    """:meta public:
-    A class providing the API for templates.
+    """A class providing the API for templates.
 
     There are two types of templates:
 
     simple
         Which have a category and name, which together are unique.
     full
         Which have a category and name, which together are unique,
```

### Comparing `molsystem-2023.4.6/molsystem/templates.py` & `molsystem-2023.7.9/molsystem/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,14 @@
     provides a way to create new molecules or fragments from a
     template, or to transfer information from a template into a
     configuration. For example, this could be used to transfer
     canonical names and atom categories residue templates onto a
     protein molecule.
 
     This class handles the templates.
-
-    :meta public:
     """
 
     def __init__(self, system_db, logger=logger):
         """Initialize the instance."""
         super().__init__(system_db, table="template", logger=logger)
 
     # def __repr__(self):
```

### Comparing `molsystem-2023.4.6/molsystem/topology.py` & `molsystem-2023.7.9/molsystem/topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/molsystem.egg-info/PKG-INFO` & `molsystem-2023.7.9/molsystem.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2023.4.6
+Version: 2023.7.9
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -23,54 +23,79 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
 MolSystem
 =============
 
-
-.. image:: https://img.shields.io/travis/molssi-seamm/molsystem.svg
-           :target: https://travis-ci.org/molssi-seamm/molsystem
-	   :alt: Build Status
+.. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/dftbplus_step
+   :target: https://github.com/molssi-seamm/molsystem/pulls
+   :alt: GitHub pull requests
+
+.. image:: https://github.com/molssi-seamm/molsystem/workflows/CI/badge.svg
+   :target: https://github.com/molssi-seamm/molsystem/actions
+   :alt: Build Status
 
 .. image:: https://codecov.io/gh/molssi-seamm/molsystem/branch/master/graph/badge.svg
-	   :target: https://codecov.io/gh/molssi-seamm/molsystem
-	   :alt: Code Coverage
+   :target: https://codecov.io/gh/molssi-seamm/molsystem
+   :alt: Code Coverage
 
-.. image:: https://img.shields.io/lgtm/grade/python/g/molssi-seamm/molsystem.svg?logo=lgtm&logoWidth=18
-	   :target: https://lgtm.com/projects/g/molssi-seamm/molsystem/context:python
-	   :alt: Code Quality
-
-.. image:: https://readthedocs.org/projects/molsystem/badge/?version=latest
-           :target: https://molsystem.readthedocs.io/en/latest/?badge=latest
-	   :alt: Documentation Status
-
-.. image:: https://pyup.io/repos/github/molssi-seamm/molsystem/shield.svg
-	   :target: https://pyup.io/repos/github/molssi-seamm/molsystem/
-	   :alt: Updates for Dependencies
+.. image:: https://github.com/molssi-seamm/molsystem/workflows/CodeQL/badge.svg
+   :target: https://github.com/molssi-seamm/molsystem/security/code-scanning
+   :alt: Code Quality
 
-.. image:: https://img.shields.io/pypi/v/molsystem.svg
-           :target: https://pypi.python.org/pypi/molsystem
-	   :alt: PyPi VERSION
 
-Molsystem provides a general class for handling molecular and periodic systems
+.. image:: https://github.com/molssi-seamm/molsystem/workflows/Release/badge.svg
+   :target: https://molssi-seamm.github.io/molsystem/index.html
+   :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/v/molsystem.svg
+   :target: https://pypi.python.org/pypi/molsystem
+   :alt: PyPi VERSION
+
+Description
+-----------
+Molsystem provides a general class for handling molecular and periodic systems. This is
+the heart of SEAMM.
 
 * Free software: GNU Lesser General Public License v3+
 * Documentation: https://molsystem.readthedocs.io.
 
 
 Features
 --------
 
-* Complete the initial version!
-
-  * Remove the coordinates from the Atoms class and allow for multiple
-    sets of coordinates -- conformers, trajectories, etc.
-  * Provide a concept of the 'current' system
+* Supports molecular and periodic (crystalline) systems.
+* Support for pointgroup and spacegroup symmetry.
+* Implemented as a SQL database, currently using SQLite, which provides permanence and a
+  disk file.
+* Handles multiple systems, and for each system any number of
+  configurations. Configurations are different structures, generally having different
+  coordinates. Examples are conformers or frames in an MD trajectory.
+* Configurations can have differing bonds, supporting reactive forcefields such as
+  ReaxFF.
+* Configurations can also have differing numbers of atoms, supporting e.g. grand
+  canonical Monte Carlo.
+* Support for templates and subsets. Templates can be used for creating or finding
+  structures in systems and subsets hold substes of atoms. An atom can be in multiple
+  subsets. For proteins, subsets can be used for residues and chains; for polymers,
+  monomers; and for fluids the subsets can track individual molecules.
+* Subsets and templates handle the correspondance between atoms so if, for instance, the
+  ordering of atoms in residues are different, that can be handled using the
+  correspondances.
+* Direct connection to and support of RDKit and OpenBabel molecules, allowing direct
+  transfer back and forth between configurations and those libraries.
+* Properties of systems and configurations are stored in fact tables of integers,
+  floats, strings, and JSON, using a star schema. One of the dimensions is metadata
+  describing the property. This data warehousing approach is almost identical to that
+  used in CIF files, with the metadata being the CIF dictionaries.
+* Good support of CIF files, with the ability to store data other than the actual atoms
+  using the properties warehouse.
+* Direct support for SMILES, SMARTS and substructure searching.
+* Scales to millions of systems and configurations, and databases in excess of 100 GB.
 
 Credits
 ---------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -85,14 +110,17 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.9 -- Added JSON properties
+    * Added properties sotred as JSON, which allows, vectors, tensors, etc.
+      
 2023.4.6 -- Enhancements for CIF files
     * Handle uncertainties in CIF files expressed as '(x)' at end of value.
 
 2023.3.30 -- Enhancements to QCSchema support
     * Improved naming of molecule in QCSchema
     * Added creation of configurations from QCSchema objects.
```

### Comparing `molsystem-2023.4.6/setup.py` & `molsystem-2023.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/conftest.py` & `molsystem-2023.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/data/1n9v.cif` & `molsystem-2023.7.9/tests/data/1n9v.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/data/aa-variants-v1.cif` & `molsystem-2023.7.9/tests/data/aa-variants-v1.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/data/acy.mmcif` & `molsystem-2023.7.9/tests/data/acy.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/data/aminoacids.mmcif` & `molsystem-2023.7.9/tests/data/aminoacids.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/data/hoh.mmcif` & `molsystem-2023.7.9/tests/data/hoh.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_angiotensin.py` & `molsystem-2023.7.9/tests/test_angiotensin.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_atoms.py` & `molsystem-2023.7.9/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_bonds.py` & `molsystem-2023.7.9/tests/test_bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_cell.py` & `molsystem-2023.7.9/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_cif.py` & `molsystem-2023.7.9/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_configuration_properties.py` & `molsystem-2023.7.9/tests/test_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_configurations.py` & `molsystem-2023.7.9/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_molfile.py` & `molsystem-2023.7.9/tests/test_molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_openbabel.py` & `molsystem-2023.7.9/tests/test_openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_pdb.py` & `molsystem-2023.7.9/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_property_timings.py` & `molsystem-2023.7.9/tests/test_property_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_rdkit.py` & `molsystem-2023.7.9/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_smiles.py` & `molsystem-2023.7.9/tests/test_smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_subsets.py` & `molsystem-2023.7.9/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_system.py` & `molsystem-2023.7.9/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_system_db.py` & `molsystem-2023.7.9/tests/test_system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_table.py` & `molsystem-2023.7.9/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_templates.py` & `molsystem-2023.7.9/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_timings.py` & `molsystem-2023.7.9/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/tests/test_topology.py` & `molsystem-2023.7.9/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2023.4.6/versioneer.py` & `molsystem-2023.7.9/versioneer.py`

 * *Files identical despite different names*

