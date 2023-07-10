# Comparing `tmp/emmet-api-0.58.2.tar.gz` & `tmp/emmet-api-0.59.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.58.2.tar", last modified: Fri Jul  7 20:11:51 2023, max compression
+gzip compressed data, was "emmet-api-0.59.0.tar", last modified: Mon Jul 10 21:09:14 2023, max compression
```

## Comparing `emmet-api-0.58.2.tar` & `emmet-api-0.59.0.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.813656 emmet-api-0.58.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-07 20:11:41.000000 emmet-api-0.58.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-07 20:11:51.809656 emmet-api-0.58.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-07 20:11:41.000000 emmet-api-0.58.2/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.753656 emmet-api-0.58.2/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.769656 emmet-api-0.58.2/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.773656 emmet-api-0.58.2/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.777656 emmet-api-0.58.2/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.781656 emmet-api-0.58.2/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.781656 emmet-api-0.58.2/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.781656 emmet-api-0.58.2/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.781656 emmet-api-0.58.2/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.781656 emmet-api-0.58.2/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.781656 emmet-api-0.58.2/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.785656 emmet-api-0.58.2/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/metal_binding/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/metal_binding/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.789656 emmet-api-0.58.2/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 20:11:41.000000 emmet-api-0.58.2/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.793656 emmet-api-0.58.2/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-07 20:11:50.000000 emmet-api-0.58.2/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-07 20:11:51.000000 emmet-api-0.58.2/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:11:50.000000 emmet-api-0.58.2/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:11:50.000000 emmet-api-0.58.2/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 20:11:50.000000 emmet-api-0.58.2/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 20:11:50.000000 emmet-api-0.58.2/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-07 20:11:41.000000 emmet-api-0.58.2/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-07-07 20:11:41.000000 emmet-api-0.58.2/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-07 20:11:41.000000 emmet-api-0.58.2/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.797656 emmet-api-0.58.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-07 20:11:41.000000 emmet-api-0.58.2/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:11:51.813656 emmet-api-0.58.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-07 20:11:41.000000 emmet-api-0.58.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-07 20:11:41.000000 emmet-api-0.58.2/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.797656 emmet-api-0.58.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.797656 emmet-api-0.58.2/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.797656 emmet-api-0.58.2/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.797656 emmet-api-0.58.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.765656 emmet-api-0.58.2/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.797656 emmet-api-0.58.2/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.769656 emmet-api-0.58.2/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.801656 emmet-api-0.58.2/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.805656 emmet-api-0.58.2/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/metal_binding/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:51.809656 emmet-api-0.58.2/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-07 20:11:41.000000 emmet-api-0.58.2/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.551370 emmet-api-0.59.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-10 21:09:03.000000 emmet-api-0.59.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-10 21:09:14.551370 emmet-api-0.59.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-10 21:09:03.000000 emmet-api-0.59.0/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.519369 emmet-api-0.59.0/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.527369 emmet-api-0.59.0/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.531369 emmet-api-0.59.0/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.535369 emmet-api-0.59.0/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-10 21:09:03.000000 emmet-api-0.59.0/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.539369 emmet-api-0.59.0/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-10 21:09:13.000000 emmet-api-0.59.0/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-10 21:09:14.000000 emmet-api-0.59.0/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:09:13.000000 emmet-api-0.59.0/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:09:13.000000 emmet-api-0.59.0/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-10 21:09:13.000000 emmet-api-0.59.0/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 21:09:13.000000 emmet-api-0.59.0/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 21:09:03.000000 emmet-api-0.59.0/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-07-10 21:09:03.000000 emmet-api-0.59.0/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-10 21:09:03.000000 emmet-api-0.59.0/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-10 21:09:03.000000 emmet-api-0.59.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:09:14.551370 emmet-api-0.59.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-10 21:09:03.000000 emmet-api-0.59.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 21:09:03.000000 emmet-api-0.59.0/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.523369 emmet-api-0.59.0/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.523369 emmet-api-0.59.0/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.543370 emmet-api-0.59.0/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:14.547370 emmet-api-0.59.0/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-10 21:09:03.000000 emmet-api-0.59.0/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.58.2/Dockerfile` & `emmet-api-0.59.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/app.py` & `emmet-api-0.59.0/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/core/api.py` & `emmet-api-0.59.0/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.59.0/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.59.0/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/core/documentation.py` & `emmet-api-0.59.0/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/core/global_header.py` & `emmet-api-0.59.0/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/core/settings.py` & `emmet-api-0.59.0/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.59.0/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.59.0/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.59.0/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.59.0/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.59.0/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/_messages/resources.py` & `emmet-api-0.59.0/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/dois/resources.py` & `emmet-api-0.59.0/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.59.0/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.59.0/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.59.0/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.59.0/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.59.0/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.59.0/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.59.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.59.0/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.59.0/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.59.0/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.59.0/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/metal_binding/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/metal_binding/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/metal_binding/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/tasks/utils.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/utils.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.59.0/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.59.0/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/legacy_resources.py` & `emmet-api-0.59.0/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/material_resources.py` & `emmet-api-0.59.0/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/molecule_resources.py` & `emmet-api-0.59.0/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/requirements/deployment.txt` & `emmet-api-0.59.0/requirements/deployment.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,25 @@
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -113,15 +113,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.15
+maggma==0.51.18
     # via emmet-api (emmet/emmet-api/setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -166,15 +166,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -252,15 +252,15 @@
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.8
     # via emmet-core
-rpds-py==0.8.8
+rpds-py==0.8.10
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.17.32
     # via
     #   pymatgen
     #   robocrys
@@ -340,12 +340,12 @@
     # via emmet-api (emmet/emmet-api/setup.py)
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.15.0
+zipp==3.16.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.10.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.9.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
     # via starlette
 attrs==23.1.0
     # via
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,25 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -88,15 +88,19 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==6.0.0
+    # via matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -113,15 +117,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -163,15 +167,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -182,15 +186,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -313,22 +317,25 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
+    #   aioitertools
+    #   bytecode
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -336,11 +343,13 @@
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,26 +68,26 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -150,15 +150,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -251,15 +251,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -270,23 +270,23 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.11.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
     # via starlette
 attrs==23.1.0
     # via
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,21 +55,25 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.99.1
+exceptiongroup==1.1.2
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -109,15 +113,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -159,15 +163,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -178,15 +182,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -309,14 +313,15 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,21 +68,21 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -145,15 +145,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -246,15 +246,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -265,23 +265,23 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.8.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,25 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -91,15 +91,15 @@
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
@@ -120,15 +120,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -170,15 +170,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -191,15 +191,15 @@
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,26 +68,26 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -120,15 +120,15 @@
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
@@ -160,15 +160,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -261,15 +261,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -282,23 +282,23 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.9.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
     # via starlette
 attrs==23.1.0
     # via
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,25 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -91,15 +91,15 @@
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
@@ -117,15 +117,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -167,15 +167,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -186,15 +186,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,26 +68,26 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -120,15 +120,15 @@
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
@@ -157,15 +157,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -258,15 +258,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -277,23 +277,23 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,25 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -113,15 +113,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -163,15 +163,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -182,15 +182,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,26 +68,26 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -150,15 +150,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -251,15 +251,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -270,23 +270,23 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.59.0/requirements/macos-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
     # via starlette
 attrs==23.1.0
     # via
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,21 +55,21 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -109,15 +109,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -159,15 +159,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -178,15 +178,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,21 +68,21 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -145,15 +145,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -246,15 +246,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -265,23 +265,23 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,25 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -91,15 +91,15 @@
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
@@ -120,15 +120,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -170,15 +170,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -191,15 +191,15 @@
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,26 +68,26 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -120,15 +120,15 @@
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
@@ -160,15 +160,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -261,15 +261,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -282,23 +282,23 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.7.1
     # via starlette
 attrs==23.1.0
     # via
@@ -14,33 +14,33 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.2
     # via ddtrace
 cattrs==23.1.2
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mongogrant
     #   uvicorn-tschaume
 contourpy==1.1.0
@@ -55,25 +55,21 @@
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.2
-    # via
-    #   anyio
-    #   cattrs
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.40.0
     # via matplotlib
@@ -88,19 +84,15 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==7.0.0
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -117,15 +109,15 @@
     #   maggma
 jsonschema-specifications==2023.6.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 matminer==0.9.0
     # via robocrys
@@ -167,15 +159,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
@@ -186,15 +178,15 @@
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
 plotly==5.15.0
     # via pymatgen
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -317,25 +309,21 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.7.1
     # via
-    #   aioitertools
-    #   bytecode
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   inflect
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -343,13 +331,11 @@
 werkzeug==2.3.6
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.58.2/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.59.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.28.0
+boto3==1.28.1
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.31.0
+botocore==1.31.1
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
 bytecode==0.14.2
     # via ddtrace
@@ -36,15 +36,15 @@
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
 click==8.1.4
     # via
     #   flask
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
@@ -68,26 +68,26 @@
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.58.1
+emmet-core[all]==0.58.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.2
     # via
     #   anyio
     #   cattrs
     #   pytest
-fastapi==0.99.1
+fastapi==0.100.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -120,15 +120,15 @@
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
     #   mkdocstrings
     #   opentelemetry-api
-importlib-resources==5.12.0
+importlib-resources==6.0.0
     # via matplotlib
 inflect==7.0.0
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
@@ -157,15 +157,15 @@
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.51.14
+maggma==0.51.17
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -258,15 +258,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.9.1
+orjson==3.9.2
     # via maggma
 packaging==23.1
     # via
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
@@ -277,23 +277,23 @@
     # via
     #   matminer
     #   pymatgen
 paramiko==3.2.0
     # via sshtunnel
 pillow==10.0.0
     # via matplotlib
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via virtualenv
 plotly==5.15.0
     # via pymatgen
 pluggy==1.2.0
     # via pytest
 pre-commit==3.3.3
     # via emmet-api (setup.py)
-protobuf==4.23.3
+protobuf==4.23.4
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
```

### Comparing `emmet-api-0.58.2/setup.py` & `emmet-api-0.59.0/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/_consumer/test_query_operators.py` & `emmet-api-0.59.0/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/_general_store/test_query_operators.py` & `emmet-api-0.59.0/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/core/test_mapi.py` & `emmet-api-0.59.0/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.59.0/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/electrodes/test_utils.py` & `emmet-api-0.59.0/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/materials/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/materials/test_utils.py` & `emmet-api-0.59.0/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/summary/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.59.0/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.59.0/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/synthesis/test_utils.py` & `emmet-api-0.59.0/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/tasks/test_utils.py` & `emmet-api-0.59.0/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/materials/xas/test_query_operators.py` & `emmet-api-0.59.0/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/metal_binding/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/metal_binding/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/tasks/test_utils.py` & `emmet-api-0.59.0/tests/molecules/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.58.2/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.59.0/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

