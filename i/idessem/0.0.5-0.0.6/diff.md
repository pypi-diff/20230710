# Comparing `tmp/idessem-0.0.5.tar.gz` & `tmp/idessem-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idessem-0.0.5.tar", last modified: Thu Apr 27 19:25:55 2023, max compression
+gzip compressed data, was "idessem-0.0.6.tar", last modified: Mon Jul 10 15:21:49 2023, max compression
```

## Comparing `idessem-0.0.5.tar` & `idessem-0.0.6.tar`

### file list

```diff
@@ -1,87 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.489013 idessem-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-27 19:23:24.000000 idessem-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-27 19:25:55.489013 idessem-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-27 19:23:24.000000 idessem-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.473012 idessem-0.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.473012 idessem-0.0.5/idessem/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.477012 idessem-0.0.5/idessem/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_estatfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/log_matriz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/idessem/dessem/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/idessem/dessem/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/arquivos/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/avl_fpha1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/idessem/dessem/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/dataestudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/modelos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/dessem/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/idessem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.473012 idessem-0.0.5/idessem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 19:25:55.000000 idessem-0.0.5/idessem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:25:55.489013 idessem-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-27 19:23:24.000000 idessem-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.481012 idessem-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.485013 idessem-0.0.5/tests/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/dessem/test_polinjus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.485013 idessem-0.0.5/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:25:55.489013 idessem-0.0.5/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/arquivos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-27 19:23:24.000000 idessem-0.0.5/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 15:19:49.000000 idessem-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 15:21:49.484317 idessem-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-10 15:19:49.000000 idessem-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.472317 idessem-0.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.472317 idessem-0.0.6/idessem/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.476318 idessem-0.0.6/idessem/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/log_matriz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/idessem/dessem/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/idessem/dessem/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/arquivos/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/avl_fpha1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/idessem/dessem/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/dataestudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142870 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.476318 idessem-0.0.6/idessem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:21:49.484317 idessem-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-10 15:19:49.000000 idessem-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/tests/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_renovaveis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/mock_open.py
```

### Comparing `idessem-0.0.5/LICENSE.md` & `idessem-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/PKG-INFO` & `idessem-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.5/README.md` & `idessem-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/avl_altqueda.py` & `idessem-0.0.6/idessem/dessem/pdo_eco_usih.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,70 @@
-from idessem.dessem.modelos.avl_altqueda import TabelaAvlAltQueda
+from idessem.dessem.modelos.pdo_eco_usih import TabelaPdoEcoUsih
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class AvlAltQueda(ArquivoCSV):
+
+class PdoEcoUsih(ArquivoCSV):
     """
-    Armazena os dados das saídas referentes a altura de queda de usinas hidráulicas.
+    Armazena os dados de eco referentes as usinas hidráulicas.
 
-    Essa classe lida com as informações de saída fornecidas pelo arquivo AVL_ALTQUEDA.
+    Essa classe lida com as informações de saída fornecidas pelo arquivo PDO_ECO_USIH.
     """
 
-    BLOCKS = [VersaoModelo, DataEstudo, TabelaAvlAltQueda]
+    BLOCKS = [VersaoModelo, DataEstudo, TabelaPdoEcoUsih]
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="AVL_ALTQUEDA.DAT"
-    ) -> "AvlAltQueda":
-        return cls.read(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="PDO_ECO_USIH.DAT"
+    ) -> "PdoEcoUsih":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     @property
     def tabela(self):
         """
-        Obtém a tabela com informações referente a altura de queda.
+        Obtém a tabela com informações referente a caracaterísticas das usinas
+        hidrelétricas e topologia das cascatas.
 
-        - estagio (`int`)
-        - iteracao (`int`)
-        - ides (`str`)
-        - patamar (`str`)
         - indice_usina (`int`)
         - nome_usina (`str`)
-        - altura_montante (`float`)
-        - altura_jusante (`float`)
-        - altura_liquida (`float`)
-        - vazao_defluente_m3s (`float`)
-        - problema (`str`)
+        - submercado (`str`)
+        - indice_usina_jusante (`int`)
+        - indice_usina_desvio (`int`)
+        - indice_usina_jusante_earm (`int`)
+        - estagio_inicial (`int`)
+        - volume_morto_inicial_hm3 (`float`)
+        - volume_morto_inicial_percentual (`float`)
+        - volume_util_inicial_hm3 (`float`)
+        - volume_util_inicial_percentual (`float`)
+        - volume_armazenado_minimo_hm3 (`float`)
+        - volume_armazenado_maximo_hm3 (`float`)
+        - volume_soleira_vertedouro_hm3 (`float`)
+        - volume_soleira_vertedouro_util_percentual (`float`)
+        - volume_soleira_desvio_hm3 (`float`)
+        - volume_soleira_desvio_util_percentual (`float`)
+        - volume_referencia_hm3 (`float`)
+        - tipo_regularizacao (`str`)
+        - flag_evaporacao (`int`)
+        - numero_conjuntos (`int`)
+        - produtibilidade_especifica (`float`)
+        - tipo_perdas (`str`)
+        - perdas_hidraulicas (`float`)
+        - canal_fuga_medio (`float`)
+        - influencia_vertimento_canal_fuga (`int`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `idessem-0.0.5/idessem/dessem/avl_desvfpha.py` & `idessem-0.0.6/idessem/dessem/pdo_oper_uct.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,71 @@
-from idessem.dessem.modelos.avl_desvfpha import TabelaAvlDesvFpha
+from idessem.dessem.modelos.pdo_oper_uct import TabelaPdoOperUct
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class AvlDesvFpha(ArquivoCSV):
+
+class PdoOperUct(ArquivoCSV):
     """
-    Armazena os dados das saídas referentes aos desvios da função de produção.
+    Armazena os dados das saídas referentes as unidades térmicas.
 
-    Essa classe lida com as informações de saída fornecidas pelo arquivo AVL_DESVFPHA.
+    Essa classe lida com as informações de saída fornecidas pelo arquivo PDO_OPER_UCT.
     """
 
-    BLOCKS = [VersaoModelo, DataEstudo, TabelaAvlDesvFpha]
+    BLOCKS = [VersaoModelo, DataEstudo, TabelaPdoOperUct]
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="AVL_DESVFPHA.DAT"
-    ) -> "AvlDesvFpha":
-        return cls.read(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="PDO_OPER_UCT.DAT"
+    ) -> "PdoOperUct":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     @property
     def tabela(self):
         """
-        Obtém a tabela com informações referente aos desvios da função de produção.
+        Obtém a tabela com informações referente a operação das unidades térmicas.
 
         - estagio (`int`)
         - indice_usina (`int`)
+        - unidade (`int`)
         - nome_usina (`str`)
-        - volume_medio_hm3 (`float`)
-        - volume_medio_percentual (`float`)
-        - vazao_turbinada_m3s (`float`)
-        - vazao_vertida_m3s (`float`)
-        - vazao_jusante_m3s (`float`)
-        - vazao_lateral_usina_m3s (`float`)
-        - vazao_lateral_posto_m3s (`float`)
-        - altura_jusante (`float`)
-        - altura_montante (`float`)
-        - produtibilidade_especifica (`float`)
-        - perdas_hidraulicas (`float`)
-        - influencia_vertimento_canal_fuga (`int`)
-        - afogamento_canal_fuga (`int`)
-        - geracao_fph (`float`)
-        - geracao_pl (`float`)
-        - geracao_fpha (`float`)
-        - desvio_absoluto_fph_pl (`float`)
-        - desvio_percentual_fph_pl (`float`)
-        - desvio_absoluto_fph_fpha (`float`)
-        - desvio_percentual_fph_fpha (`float`)
-
+        - submercado (`str`)
+        - barra (`int`)
+        - numero_maximo_oscilacoes (`int`)
+        - flag_geracao_minima_maxima (`int`)
+        - geracao_minima (`float`)
+        - geracao_minima_unidade (`float`)
+        - geracao_maxima (`float`)
+        - geracao_maxima_unidade (`float`)
+        - geracao_minima_acionamento (`float`)
+        - tempo_on (`int`)
+        - tempo_off (`int`)
+        - status (`int`)
+        - geracao (`float`)
+        - tempo (`float`)
+        - custo_linear (`float`)
+        - custo_partida_unidade (`float`)
+        - cmo (`float`)
+        - cmb (`float`)
+        - variavel_dual (`float`)
+        - titulacao (`str`)
+        - rampa_subida (`float`)
+        - rampa_descida (`float`)
+        - unidade_equivalente (`int`)
+        - rampa_transicao (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `idessem-0.0.5/idessem/dessem/des_log_relato.py` & `idessem-0.0.6/idessem/dessem/des_log_relato.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     VersaoModelo,
 )
 from cfinterface.files.blockfile import BlockFile
 from typing import Optional, Type, TypeVar
 from datetime import datetime
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class DesLogRelato(BlockFile):
     """
     Armazena os dados referentes ao resultado do processamentdo do DESSEM.
 
     Essa classe lida com as informações de saída fornecidas pelo arquivo DES_LOG_RELATO.
     """
@@ -28,15 +32,20 @@
     ENCODING = "iso-8859-1"
     T = TypeVar("T")
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="DES_LOG_RELATO.DAT"
     ) -> "DesLogRelato":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def _bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `idessem-0.0.5/idessem/dessem/hidr.py` & `idessem-0.0.6/idessem/dessem/hidr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from cfinterface.files.registerfile import RegisterFile
 from idessem.dessem.modelos.hidr import RegistroUHEHidr
 from idessem.config import MESES_ABREV
 import pandas as pd  # type: ignore
 
 
-from typing import TypeVar, List, Optional
+from typing import TypeVar, List, Optional, IO, Union
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
 class Hidr(RegisterFile):
     """
     Armazena os dados de entrada do DESSEM referentes ao cadastro das
     usinas hidroelétricas.
     """
@@ -20,19 +24,33 @@
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df: Optional[pd.DataFrame] = None
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="hidr.dat") -> "Hidr":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="hidr.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
+
+    def write(self, to: Union[str, IO], *args, **kwargs):
         self.__atualiza_registros()
-        self.write(diretorio, nome_arquivo)
+        super().write(to, *args, **kwargs)
 
     def __monta_df_de_registros(self) -> Optional[pd.DataFrame]:
         registros: List[RegistroUHEHidr] = [
             r for r in self.data.of_type(RegistroUHEHidr)
         ]
         if len(registros) == 0:
             return None
```

### Comparing `idessem-0.0.5/idessem/dessem/log_matriz.py` & `idessem-0.0.6/idessem/dessem/log_matriz.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from idessem.dessem.modelos.log_matriz import TabelaLogMatriz
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class LogMatriz(ArquivoCSV):
     """
     Armazena os dados das saídas referentes ao processo iterativo de resolução.
 
     Essa classe lida com as informações de saída fornecidas pelo arquivo LOG_MATRIZ.
     """
@@ -16,15 +20,20 @@
     BLOCKS = [VersaoModelo, DataEstudo, TabelaLogMatriz]
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="LOG_MATRIZ.DAT"
     ) -> "LogMatriz":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     @property
     def tabela(self):
         """
         Obtém a tabela com informações referente ao processo iterativo de convergência.
 
         - iteracao (`int`)
```

### Comparing `idessem-0.0.5/idessem/dessem/modelos/arquivos/arquivocsv.py` & `idessem-0.0.6/idessem/dessem/modelos/arquivos/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/avl_altqueda.py` & `idessem-0.0.6/idessem/dessem/modelos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/avl_desvfpha.py` & `idessem-0.0.6/idessem/dessem/modelos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/avl_fpha1.py` & `idessem-0.0.6/idessem/dessem/modelos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/blocos/dataestudo.py` & `idessem-0.0.6/idessem/dessem/modelos/blocos/dataestudo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/blocos/tabelacsv.py` & `idessem-0.0.6/idessem/dessem/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/blocos/versaomodelo.py` & `idessem-0.0.6/idessem/dessem/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/des_log_relato.py` & `idessem-0.0.6/idessem/dessem/modelos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/hidr.py` & `idessem-0.0.6/idessem/dessem/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/log_matriz.py` & `idessem-0.0.6/idessem/dessem/modelos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/operut.py` & `idessem-0.0.6/idessem/dessem/modelos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/pdo_eco_usih.py` & `idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/pdo_hidr.py` & `idessem-0.0.6/idessem/dessem/modelos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/pdo_oper_uct.py` & `idessem-0.0.6/idessem/dessem/modelos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/pdo_sist.py` & `idessem-0.0.6/idessem/dessem/modelos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/idessem/dessem/modelos/polinjus.py` & `idessem-0.0.6/idessem/dessem/modelos/polinjus.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from cfinterface.components.register import Register
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
+from cfinterface.components.literalfield import LiteralField
 
 from typing import Optional
 
 
 class HidreletricaCurvaJusante(Register):
     """ """
 
@@ -279,7 +280,76 @@
         :rtype: float | None
         """
         return self.data[9]
 
     @coeficiente_a4.setter
     def coeficiente_a4(self, c: float):
         self.data[9] = c
+
+
+class HidreletricaCurvaJusanteAfogamentoExplicitoUsina(Register):
+    """ """
+
+    IDENTIFIER = "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-USINA"
+    IDENTIFIER_DIGITS = 53
+    LINE = Line(
+        [
+            IntegerField(),
+            LiteralField(size=3),
+        ],
+        delimiter=";",
+    )
+
+    @property
+    def codigo_usina(self) -> Optional[int]:
+        """
+        O código da usina hidrelétrica relacionada ao polinômio.
+
+        :return: O código da usina
+        :rtype: int | None
+        """
+        return self.data[0]
+
+    @codigo_usina.setter
+    def codigo_usina(self, c: int):
+        self.data[0] = c
+
+    @property
+    def considera_afogamento(self) -> Optional[str]:
+        """
+        Habilitação do afogamento explícito.
+
+        :return: O flag da habilitação.
+        :rtype: str | None
+        """
+        return self.data[1]
+
+    @considera_afogamento.setter
+    def considera_afogamento(self, c: str):
+        self.data[1] = c
+
+
+class HidreletricaCurvaJusanteAfogamentoExplicitoPadrao(Register):
+    """ """
+
+    IDENTIFIER = "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-PADRAO"
+    IDENTIFIER_DIGITS = 54
+    LINE = Line(
+        [
+            LiteralField(size=3),
+        ],
+        delimiter=";",
+    )
+
+    @property
+    def considera_afogamento(self) -> Optional[str]:
+        """
+        Habilitação do afogamento explícito.
+
+        :return: O flag da habilitação.
+        :rtype: str | None
+        """
+        return self.data[0]
+
+    @considera_afogamento.setter
+    def considera_afogamento(self, c: str):
+        self.data[0] = c
```

### Comparing `idessem-0.0.5/idessem/dessem/operut.py` & `idessem-0.0.6/idessem/dessem/operut.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     BlocoTrataInviabIlha,
 )
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, List
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Operut(BlockFile):
     """
     Armazena os dados de entrada do DESSEM referentes às
     configurações da operação das usinas térmelétricas.
 
     """
@@ -34,18 +38,29 @@
     BLOCKS = [BlocoUctPar, BlocoUcTerm, BlocoPint, BlocoInitUT, BlocoOper]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="operut.dat") -> "Operut":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="operut.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `idessem-0.0.5/idessem/dessem/pdo_hidr.py` & `idessem-0.0.6/idessem/dessem/pdo_hidr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from idessem.dessem.modelos.pdo_hidr import TabelaPdoHidr
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class PdoHidr(ArquivoCSV):
     """
     Armazena os dados das saídas referentes as unidades hidráulicas.
 
     Essa classe lida com as informações de saída fornecidas pelo arquivo PDO_HIDR.
     """
@@ -16,15 +20,20 @@
     BLOCKS = [VersaoModelo, DataEstudo, TabelaPdoHidr]
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="PDO_HIDR.DAT"
     ) -> "PdoHidr":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     @property
     def tabela(self):
         """
         Obtém a tabela com informações referente a operação das unidades hidráulicas.
 
         - estagio (`int`)
```

### Comparing `idessem-0.0.5/idessem/dessem/pdo_sist.py` & `idessem-0.0.6/idessem/dessem/pdo_sist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from idessem.dessem.modelos.pdo_sist import TabelaPdoSist
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class PdoSist(ArquivoCSV):
     """
     Armazena os dados das saídas referentes aos submercados.
 
     Essa classe lida com as informações de saída fornecidas pelo arquivo PDO_SIST.
     """
@@ -16,15 +20,20 @@
     BLOCKS = [VersaoModelo, DataEstudo, TabelaPdoSist]
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="PDO_SIST.DAT"
     ) -> "PdoSist":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     @property
     def tabela(self):
         """
         Obtém a tabela com informações referente a operação por submercado.
 
         - estagio (`int`)
```

### Comparing `idessem-0.0.5/idessem/dessem/polinjus.py` & `idessem-0.0.6/idessem/dessem/polinjus.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,36 +2,55 @@
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 import pandas as pd  # type: ignore
 from idessem.dessem.modelos.polinjus import (
     HidreletricaCurvaJusante,
     HidreletricaCurvaJusantePolinomioPorPartes,
     HidreletricaCurvaJusantePolinomioPorPartesSegmento,
+    HidreletricaCurvaJusanteAfogamentoExplicitoUsina,
+    HidreletricaCurvaJusanteAfogamentoExplicitoPadrao,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Polinjus(RegisterFile):
     """ """
 
     T = TypeVar("T")
 
     REGISTERS = [
         HidreletricaCurvaJusantePolinomioPorPartesSegmento,
         HidreletricaCurvaJusantePolinomioPorPartes,
+        HidreletricaCurvaJusanteAfogamentoExplicitoUsina,
+        HidreletricaCurvaJusanteAfogamentoExplicitoPadrao,
         HidreletricaCurvaJusante,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="polinjus.csv"
     ) -> "Polinjus":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="polinjus.csv"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
@@ -254,7 +273,66 @@
                 limite_superior_vazao_jusante=limite_superior_vazao_jusante,
                 coeficiente_a0=coeficiente_a0,
                 coeficiente_a1=coeficiente_a1,
                 coeficiente_a2=coeficiente_a2,
                 coeficiente_a3=coeficiente_a3,
                 coeficiente_a4=coeficiente_a4,
             )
+
+    def hidreletrica_curvajusante_afogamentoexplicito_usina(
+        self,
+        codigo_usina: Optional[int] = None,
+        considera_afogamento: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[
+        Union[
+            HidreletricaCurvaJusanteAfogamentoExplicitoUsina,
+            List[HidreletricaCurvaJusanteAfogamentoExplicitoUsina],
+            pd.DataFrame,
+        ]
+    ]:
+        """
+        Obtém registros que habilitam ou desabilitam a consideração
+        do tratamento do afogamento explícito por usina. Opcionalmente,
+        o retorno pode ser transformado em um `DataFrame`, apenas
+        para leitura das informações.
+
+        :param codigo_usina: código que especifica a usina
+        :type codigo_usina: int | None
+        :param considera_afogamento: habilitação do afogamento
+        :type considera_afogamento: str | None
+        :type df: bool
+        :return: Um ou mais registros, se existirem.
+        :rtype: `HidreletricaCurvaJusante` |
+            List[`HidreletricaCurvaJusante`] | `None` | `DataFrame`
+        """
+        if df:
+            return self._as_df(
+                HidreletricaCurvaJusanteAfogamentoExplicitoUsina
+            )
+        else:
+            return self.__obtem_registros_com_filtros(
+                HidreletricaCurvaJusanteAfogamentoExplicitoUsina,
+                codigo_usina=codigo_usina,
+                considera_afogamento=considera_afogamento,
+            )
+
+    def hidreletrica_curvajusante_afogamentoexplicito_padrao(
+        self,
+        considera_afogamento: Optional[str] = None,
+    ) -> Optional[
+        Union[
+            HidreletricaCurvaJusanteAfogamentoExplicitoPadrao,
+            List[HidreletricaCurvaJusanteAfogamentoExplicitoPadrao],
+        ]
+    ]:
+        """
+        Obtém registros que habilitam ou desabilitam a consideração
+        do tratamento do afogamento explícito padrão.
+
+        :param considera_afogamento: habilitação do afogamento
+        :type considera_afogamento: str | None
+        """
+        return self.__obtem_registros_com_filtros(
+            HidreletricaCurvaJusanteAfogamentoExplicitoPadrao,
+            considera_afogamento=considera_afogamento,
+        )
```

### Comparing `idessem-0.0.5/idessem.egg-info/PKG-INFO` & `idessem-0.0.6/idessem.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.5
+Version: 0.0.6
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.5/idessem.egg-info/SOURCES.txt` & `idessem-0.0.6/idessem.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,62 +12,82 @@
 idessem.egg-info/top_level.txt
 idessem/dessem/__init__.py
 idessem/dessem/avl_altqueda.py
 idessem/dessem/avl_desvfpha.py
 idessem/dessem/avl_estatfpha.py
 idessem/dessem/avl_fpha1.py
 idessem/dessem/des_log_relato.py
+idessem/dessem/dessemarq.py
+idessem/dessem/entdados.py
 idessem/dessem/hidr.py
 idessem/dessem/log_matriz.py
 idessem/dessem/operut.py
+idessem/dessem/pdo_eco_fcfcortes.py
 idessem/dessem/pdo_eco_usih.py
+idessem/dessem/pdo_eco_usih_polin.py
 idessem/dessem/pdo_hidr.py
 idessem/dessem/pdo_oper_uct.py
 idessem/dessem/pdo_sist.py
 idessem/dessem/polinjus.py
+idessem/dessem/renovaveis.py
 idessem/dessem/modelos/__init__.py
 idessem/dessem/modelos/avl_altqueda.py
 idessem/dessem/modelos/avl_desvfpha.py
 idessem/dessem/modelos/avl_fpha1.py
 idessem/dessem/modelos/des_log_relato.py
+idessem/dessem/modelos/dessemarq.py
+idessem/dessem/modelos/entdados.py
 idessem/dessem/modelos/hidr.py
 idessem/dessem/modelos/log_matriz.py
 idessem/dessem/modelos/operut.py
+idessem/dessem/modelos/pdo_eco_fcfcortes.py
 idessem/dessem/modelos/pdo_eco_usih.py
+idessem/dessem/modelos/pdo_eco_usih_polin.py
 idessem/dessem/modelos/pdo_hidr.py
 idessem/dessem/modelos/pdo_oper_uct.py
 idessem/dessem/modelos/pdo_sist.py
 idessem/dessem/modelos/polinjus.py
+idessem/dessem/modelos/renovaveis.py
 idessem/dessem/modelos/arquivos/__init__.py
 idessem/dessem/modelos/arquivos/arquivocsv.py
 idessem/dessem/modelos/blocos/__init__.py
 idessem/dessem/modelos/blocos/dataestudo.py
 idessem/dessem/modelos/blocos/tabelacsv.py
 idessem/dessem/modelos/blocos/versaomodelo.py
 tests/__init__.py
 tests/dessem/__init__.py
 tests/dessem/test_avl_altqueda.py
 tests/dessem/test_avl_desvfpha.py
 tests/dessem/test_avl_fpha1.py
 tests/dessem/test_des_log_relato.py
+tests/dessem/test_dessemarq.py
+tests/dessem/test_entdados.py
 tests/dessem/test_hidr.py
 tests/dessem/test_log_matriz.py
 tests/dessem/test_operut.py
+tests/dessem/test_pdo_eco_fcfcortes.py
 tests/dessem/test_pdo_eco_usih.py
+tests/dessem/test_pdo_eco_usih_polin.py
 tests/dessem/test_pdo_hidr.py
 tests/dessem/test_pdo_oper_uct.py
 tests/dessem/test_pdo_sist.py
 tests/dessem/test_polinjus.py
+tests/dessem/test_renovaveis.py
 tests/mocks/__init__.py
 tests/mocks/mock_open.py
 tests/mocks/arquivos/__init__.py
 tests/mocks/arquivos/avl_altqueda.py
 tests/mocks/arquivos/avl_desvfpha.py
 tests/mocks/arquivos/avl_fpha1.py
 tests/mocks/arquivos/des_log_relato.py
+tests/mocks/arquivos/dessemarq.py
+tests/mocks/arquivos/entdados.py
 tests/mocks/arquivos/log_matriz.py
 tests/mocks/arquivos/operut.py
+tests/mocks/arquivos/pdo_eco_fcfcortes.py
 tests/mocks/arquivos/pdo_eco_usih.py
+tests/mocks/arquivos/pdo_eco_usih_polin.py
 tests/mocks/arquivos/pdo_hidr.py
 tests/mocks/arquivos/pdo_oper_uct.py
 tests/mocks/arquivos/pdo_sist.py
-tests/mocks/arquivos/polinjus.py
+tests/mocks/arquivos/polinjus.py
+tests/mocks/arquivos/renovaveis.py
```

### Comparing `idessem-0.0.5/setup.py` & `idessem-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/dessem/test_avl_altqueda.py` & `idessem-0.0.6/tests/dessem/test_avl_altqueda.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.avl_altqueda import MockAvlAltqueda
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_avl_altqueda():
     m: MagicMock = mock_open(read_data="".join(MockAvlAltqueda))
     with patch("builtins.open", m):
-        log = AvlAltQueda.le_arquivo("")
+        log = AvlAltQueda.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_avl_altqueda():
     m: MagicMock = mock_open(read_data="".join(MockAvlAltqueda))
     with patch("builtins.open", m):
-        log = AvlAltQueda.le_arquivo("")
+        log = AvlAltQueda.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_avl_altqueda():
     m: MagicMock = mock_open(read_data="".join(MockAvlAltqueda))
     with patch("builtins.open", m):
-        log = AvlAltQueda.le_arquivo("")
+        log = AvlAltQueda.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_avl_altqueda():
     m: MagicMock = mock_open(read_data="".join(MockAvlAltqueda))
     with patch("builtins.open", m):
-        log = AvlAltQueda.le_arquivo("")
+        log = AvlAltQueda.read(ARQ_TESTE)
         assert log.tabela.at[0, "estagio"] == 1
         assert log.tabela.at[0, "iteracao"] == 1
         assert log.tabela.at[0, "ides"] == "S"
         assert log.tabela.at[0, "patamar"] == "LEVE"
         assert log.tabela.at[0, "indice_usina"] == 1
         assert log.tabela.at[0, "nome_usina"] == "CAMARGOS"
         assert log.tabela.at[0, "altura_montante"] == 911.78
@@ -46,19 +48,19 @@
         assert log.tabela.at[0, "vazao_defluente_m3s"] == 160.50
         assert log.tabela.at[0, "problema"] is None
 
 
 def test_eq_avl_altqueda():
     m: MagicMock = mock_open(read_data="".join(MockAvlAltqueda))
     with patch("builtins.open", m):
-        log1 = AvlAltQueda.le_arquivo("")
-        log2 = AvlAltQueda.le_arquivo("")
+        log1 = AvlAltQueda.read(ARQ_TESTE)
+        log2 = AvlAltQueda.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_avl_altqueda():
     m: MagicMock = mock_open(read_data="".join(MockAvlAltqueda))
     with patch("builtins.open", m):
-        log1 = AvlAltQueda.le_arquivo("")
-        log2 = AvlAltQueda.le_arquivo("")
+        log1 = AvlAltQueda.read(ARQ_TESTE)
+        log2 = AvlAltQueda.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_avl_desvfpha.py` & `idessem-0.0.6/tests/dessem/test_avl_desvfpha.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.avl_desvfpha import MockAvlDesvfpha
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_avl_desvfpha():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
     with patch("builtins.open", m):
-        log = AvlDesvFpha.le_arquivo("")
+        log = AvlDesvFpha.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_avl_desvfpha():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
     with patch("builtins.open", m):
-        log = AvlDesvFpha.le_arquivo("")
+        log = AvlDesvFpha.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_avl_desvfpha():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
     with patch("builtins.open", m):
-        log = AvlDesvFpha.le_arquivo("")
+        log = AvlDesvFpha.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_avl_desvfpha():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
     with patch("builtins.open", m):
-        log = AvlDesvFpha.le_arquivo("")
+        log = AvlDesvFpha.read(ARQ_TESTE)
         assert log.tabela.at[0, "estagio"] == 1
         assert log.tabela.at[0, "indice_usina"] == 1
         assert log.tabela.at[0, "nome_usina"] == "CAMARGOS"
         assert log.tabela.at[0, "volume_medio_hm3"] == 700.64
         assert log.tabela.at[0, "volume_medio_percentual"] == 86.40
         assert log.tabela.at[0, "vazao_turbinada_m3s"] == 160.50
         assert log.tabela.at[0, "vazao_vertida_m3s"] == 0.0
@@ -58,19 +60,19 @@
         assert log.tabela.at[0, "desvio_absoluto_fph_fpha"] == 0.0
         assert log.tabela.at[0, "desvio_percentual_fph_fpha"] == -0.01
 
 
 def test_eq_avl_desvfpha():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
     with patch("builtins.open", m):
-        log1 = AvlDesvFpha.le_arquivo("")
-        log2 = AvlDesvFpha.le_arquivo("")
+        log1 = AvlDesvFpha.read(ARQ_TESTE)
+        log2 = AvlDesvFpha.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_avl_desvfpha():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
     with patch("builtins.open", m):
-        log1 = AvlDesvFpha.le_arquivo("")
-        log2 = AvlDesvFpha.le_arquivo("")
+        log1 = AvlDesvFpha.read(ARQ_TESTE)
+        log2 = AvlDesvFpha.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_avl_fpha1.py` & `idessem-0.0.6/tests/dessem/test_avl_fpha1.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,121 +2,123 @@
 
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.avl_fpha1 import MockAvlFpha1, MockAvlFpha1v190300
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_avl_fpha1():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_avl_fpha1():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_avl_fpha1():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_avl_fpha1():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
     with patch("builtins.open", m):
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.tabela.at[0, "indice_usina"] == 1
         assert log.tabela.at[0, "nome_usina"] == "CAMARGOS"
         assert log.tabela.at[0, "segmento_fpha"] == 1
         assert log.tabela.at[0, "fator_correcao"] == 1.0
         assert log.tabela.at[0, "vazao_lateral_media"] == 0
         assert log.tabela.at[0, "rhs"] == -11.8461
         assert log.tabela.at[0, "coeficiente_volume_util"] == 0.020604
         assert log.tabela.at[0, "coeficiente_vazao_turbinada"] == 0.224440
         assert log.tabela.at[0, "coeficiente_vazao_lateral"] == 0.0
 
 
 def test_eq_avl_fpha1():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
     with patch("builtins.open", m):
-        log1 = AvlFpha1.le_arquivo("")
-        log2 = AvlFpha1.le_arquivo("")
+        log1 = AvlFpha1.read(ARQ_TESTE)
+        log2 = AvlFpha1.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_avl_fpha1():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1))
     with patch("builtins.open", m):
-        log1 = AvlFpha1.le_arquivo("")
-        log2 = AvlFpha1.le_arquivo("")
+        log1 = AvlFpha1.read(ARQ_TESTE)
+        log2 = AvlFpha1.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
 
 
 def test_atributos_encontrados_avl_fpha1_v190300():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1v190300))
     with patch("builtins.open", m):
         AvlFpha1.set_version("19.3")
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_avl_fpha1_v190300():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1v190300))
     with patch("builtins.open", m):
         AvlFpha1.set_version("19.3")
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_avl_fpha1_v190300():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1v190300))
     with patch("builtins.open", m):
         AvlFpha1.set_version("19.3")
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_avl_fpha1_v190300():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1v190300))
     with patch("builtins.open", m):
         AvlFpha1.set_version("19.3")
-        log = AvlFpha1.le_arquivo("")
+        log = AvlFpha1.read(ARQ_TESTE)
         assert log.tabela.at[0, "indice_usina"] == 1
         assert log.tabela.at[0, "nome_usina"] == "CAMARGOS"
         assert log.tabela.at[0, "segmento_fpha"] == 1
         assert log.tabela.at[0, "fator_correcao"] == 1.0
         assert log.tabela.at[0, "rhs"] == -11.8461
         assert log.tabela.at[0, "coeficiente_volume_util"] == 0.020604
         assert log.tabela.at[0, "coeficiente_vazao_turbinada"] == 0.224440
         assert log.tabela.at[0, "coeficiente_vazao_lateral"] == 0.0
 
 
 def test_eq_avl_fpha1_v190300():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1v190300))
     with patch("builtins.open", m):
         AvlFpha1.set_version("193")
-        log1 = AvlFpha1.le_arquivo("")
-        log2 = AvlFpha1.le_arquivo("")
+        log1 = AvlFpha1.read(ARQ_TESTE)
+        log2 = AvlFpha1.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_avl_fpha1_v190300():
     m: MagicMock = mock_open(read_data="".join(MockAvlFpha1v190300))
     with patch("builtins.open", m):
         AvlFpha1.set_version("19.3")
-        log1 = AvlFpha1.le_arquivo("")
-        log2 = AvlFpha1.le_arquivo("")
+        log1 = AvlFpha1.read(ARQ_TESTE)
+        log2 = AvlFpha1.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_des_log_relato.py` & `idessem-0.0.6/tests/dessem/test_des_log_relato.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,46 +8,48 @@
 from unittest.mock import MagicMock, patch
 from tests.mocks.arquivos.des_log_relato import (
     MockDesLogRelato,
     MockBlocoVariaveisOtimizacao,
     MockBlocoTempoProcessamento,
 )
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_des_log_relato():
     m: MagicMock = mock_open(read_data="".join(MockDesLogRelato))
     with patch("builtins.open", m):
-        log = DesLogRelato.le_arquivo("")
+        log = DesLogRelato.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tempo_processamento is not None
         assert log.variaveis_otimizacao is not None
 
 
 def test_atributos_naoencontrados_des_log_relato():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        log = DesLogRelato.le_arquivo("")
+        log = DesLogRelato.read(ARQ_TESTE)
         assert log.versao is None
         assert log.data_estudo is None
         assert log.tempo_processamento is None
         assert log.variaveis_otimizacao is None
 
 
 def test_versao_des_log_relato():
     m: MagicMock = mock_open(read_data="".join(MockDesLogRelato))
     with patch("builtins.open", m):
-        log = DesLogRelato.le_arquivo("")
+        log = DesLogRelato.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_des_log_relato():
     m: MagicMock = mock_open(read_data="".join(MockDesLogRelato))
     with patch("builtins.open", m):
-        log = DesLogRelato.le_arquivo("")
+        log = DesLogRelato.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_eq_blocovariaveisotimizacao():
     m: MagicMock = mock_open(read_data="".join(MockBlocoVariaveisOtimizacao))
     b1 = BlocoVariaveisOtimizacao()
     with patch("builtins.open", m):
```

### Comparing `idessem-0.0.5/tests/dessem/test_log_matriz.py` & `idessem-0.0.6/tests/dessem/test_log_matriz.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.log_matriz import MockLogMatriz
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_log_matriz():
     m: MagicMock = mock_open(read_data="".join(MockLogMatriz))
     with patch("builtins.open", m):
-        log = LogMatriz.le_arquivo("")
+        log = LogMatriz.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_log_matriz():
     m: MagicMock = mock_open(read_data="".join(MockLogMatriz))
     with patch("builtins.open", m):
-        log = LogMatriz.le_arquivo("")
+        log = LogMatriz.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_log_matriz():
     m: MagicMock = mock_open(read_data="".join(MockLogMatriz))
     with patch("builtins.open", m):
-        log = LogMatriz.le_arquivo("")
+        log = LogMatriz.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_log_matriz():
     m: MagicMock = mock_open(read_data="".join(MockLogMatriz))
     with patch("builtins.open", m):
-        log = LogMatriz.le_arquivo("")
+        log = LogMatriz.read(ARQ_TESTE)
         assert log.tabela.at[0, "iteracao"] == 1
         assert log.tabela.at[0, "tipo"] == "PL"
         assert log.tabela.at[0, "variaveis"] == 489633
         assert log.tabela.at[0, "variaveis_inteiras"] == 0
         assert log.tabela.at[0, "restricoes"] == 114133
         assert log.tabela.at[0, "restricoes_inteiras"] == 0
         assert log.tabela.at[0, "elementos"] == 1486191
@@ -45,19 +47,19 @@
         assert log.tabela.at[0, "funcao_objetivo"] == -12925383.197
         assert log.tabela.at[0, "status"] == 1
 
 
 def test_eq_log_matriz():
     m: MagicMock = mock_open(read_data="".join(MockLogMatriz))
     with patch("builtins.open", m):
-        log1 = LogMatriz.le_arquivo("")
-        log2 = LogMatriz.le_arquivo("")
+        log1 = LogMatriz.read(ARQ_TESTE)
+        log2 = LogMatriz.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_log_matriz():
     m: MagicMock = mock_open(read_data="".join(MockLogMatriz))
     with patch("builtins.open", m):
-        log1 = LogMatriz.le_arquivo("")
-        log2 = LogMatriz.le_arquivo("")
+        log1 = LogMatriz.read(ARQ_TESTE)
+        log2 = LogMatriz.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_operut.py` & `idessem-0.0.6/tests/dessem/test_operut.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,27 +37,29 @@
     MockBlocoTolerIlh,
     MockBlocoCrossover,
     MockBlocoEngolimento,
     MockBlocoTrataInviabIlha,
 )
 import pandas as pd
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_operut():
     m: MagicMock = mock_open(read_data="".join(MockOperut))
     with patch("builtins.open", m):
-        op = Operut.le_arquivo("")
+        op = Operut.read(ARQ_TESTE)
         assert op.condicoes_iniciais is not None
         assert op.limites_e_condicoes_operativas is not None
 
 
 def test_atributos_nao_encontrados_operut():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        op = Operut.le_arquivo("")
+        op = Operut.read(ARQ_TESTE)
         assert op.condicoes_iniciais is None
         assert op.limites_e_condicoes_operativas is None
 
 
 # Bloco INIT
 def test_eq_blocoinit():
     m: MagicMock = mock_open(read_data="".join(MockBlocoInit))
@@ -694,20 +696,20 @@
     assert b.data == 1
 
 
 # Leitura e escrita
 def test_leitura_escrita_operut():
     m_leitura: MagicMock = mock_open(read_data="".join(MockOperut))
     with patch("builtins.open", m_leitura):
-        op1 = Operut.le_arquivo("")
+        op1 = Operut.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        op1.escreve_arquivo("", "")
+        op1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        op2 = Operut.le_arquivo("")
+        op2 = Operut.read(ARQ_TESTE)
         assert op1 == op2
```

### Comparing `idessem-0.0.5/tests/dessem/test_pdo_eco_usih.py` & `idessem-0.0.6/tests/dessem/test_pdo_eco_usih.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.pdo_eco_usih import MockPdoEcoUsih
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_pdo_eco_usih():
     m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.le_arquivo("")
+        pdo = PdoEcoUsih.read(ARQ_TESTE)
         assert pdo.versao is not None
         assert pdo.data_estudo is not None
         assert pdo.tabela is not None
 
 
 def test_versao_pdo_eco_usih():
     m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.le_arquivo("")
+        pdo = PdoEcoUsih.read(ARQ_TESTE)
         assert pdo.versao == "19.3.1"
 
 
 def test_data_estudo_pdo_eco_usih():
     m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.le_arquivo("")
+        pdo = PdoEcoUsih.read(ARQ_TESTE)
         assert pdo.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_pdo_eco_usih():
     m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.le_arquivo("")
+        pdo = PdoEcoUsih.read(ARQ_TESTE)
 
         assert pdo.tabela.at[0, "indice_usina"] == 1
         assert pdo.tabela.at[0, "nome_usina"] == "CAMARGOS"
         assert pdo.tabela.at[0, "submercado"] == "SE"
         assert pdo.tabela.at[0, "indice_usina_jusante"] == 2
         # assert pdo.tabela.at[0, "indice_usina_desvio"] == "-"
         assert pd.isna(pdo.tabela.at[0, "indice_usina_desvio"])
@@ -69,19 +71,19 @@
         assert pdo.tabela.at[0, "canal_fuga_medio"] == 885.73
         assert pdo.tabela.at[0, "influencia_vertimento_canal_fuga"] == 0
 
 
 def test_eq_pdo_eco_usih():
     m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
     with patch("builtins.open", m):
-        log1 = PdoEcoUsih.le_arquivo("")
-        log2 = PdoEcoUsih.le_arquivo("")
+        log1 = PdoEcoUsih.read(ARQ_TESTE)
+        log2 = PdoEcoUsih.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_pdo_eco_usih():
     m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
     with patch("builtins.open", m):
-        log1 = PdoEcoUsih.le_arquivo("")
-        log2 = PdoEcoUsih.le_arquivo("")
+        log1 = PdoEcoUsih.read(ARQ_TESTE)
+        log2 = PdoEcoUsih.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_pdo_hidr.py` & `idessem-0.0.6/tests/dessem/test_pdo_hidr.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.pdo_hidr import MockPdoHidr
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_pdo_hidr():
     m: MagicMock = mock_open(read_data="".join(MockPdoHidr))
     with patch("builtins.open", m):
-        log = PdoHidr.le_arquivo("")
+        log = PdoHidr.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_pdo_hidr():
     m: MagicMock = mock_open(read_data="".join(MockPdoHidr))
     with patch("builtins.open", m):
-        log = PdoHidr.le_arquivo("")
+        log = PdoHidr.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_pdo_hidr():
     m: MagicMock = mock_open(read_data="".join(MockPdoHidr))
     with patch("builtins.open", m):
-        log = PdoHidr.le_arquivo("")
+        log = PdoHidr.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_pdo_hidr():
     m: MagicMock = mock_open(read_data="".join(MockPdoHidr))
     with patch("builtins.open", m):
-        log = PdoHidr.le_arquivo("")
+        log = PdoHidr.read(ARQ_TESTE)
         assert log.tabela.at[2, "estagio"] == 1
         assert log.tabela.at[2, "patamar"] == "LEVE"
         assert log.tabela.at[2, "indice_usina"] == 1
         assert log.tabela.at[2, "nome_usina"] == "CAMARGOS"
         assert log.tabela.at[2, "submercado"] == "SE"
         assert log.tabela.at[2, "conjunto"] == 99
         assert log.tabela.at[2, "unidade"] == 99
@@ -73,19 +75,19 @@
         assert log.tabela.at[2, "perdas_hidraulicas"] == 0.0
         assert log.tabela.at[2, "altura_queda"] == 25.68
 
 
 def test_eq_pdo_hidr():
     m: MagicMock = mock_open(read_data="".join(MockPdoHidr))
     with patch("builtins.open", m):
-        log1 = PdoHidr.le_arquivo("")
-        log2 = PdoHidr.le_arquivo("")
+        log1 = PdoHidr.read(ARQ_TESTE)
+        log2 = PdoHidr.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_pdo_hidr():
     m: MagicMock = mock_open(read_data="".join(MockPdoHidr))
     with patch("builtins.open", m):
-        log1 = PdoHidr.le_arquivo("")
-        log2 = PdoHidr.le_arquivo("")
+        log1 = PdoHidr.read(ARQ_TESTE)
+        log2 = PdoHidr.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_pdo_oper_uct.py` & `idessem-0.0.6/tests/dessem/test_pdo_oper_uct.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.pdo_oper_uct import MockPdoOperUct
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_pdo_oper_uct():
     m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        pdo = PdoOperUct.le_arquivo("")
+        pdo = PdoOperUct.read(ARQ_TESTE)
         assert pdo.versao is not None
         assert pdo.data_estudo is not None
         assert pdo.tabela is not None
 
 
 def test_versao_pdo_oper_uct():
     m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        pdo = PdoOperUct.le_arquivo("")
+        pdo = PdoOperUct.read(ARQ_TESTE)
         assert pdo.versao == "19.0.42"
 
 
 def test_data_estudo_pdo_oper_uct():
     m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        pdo = PdoOperUct.le_arquivo("")
+        pdo = PdoOperUct.read(ARQ_TESTE)
         assert pdo.data_estudo == datetime(year=2022, month=8, day=8)
 
 
 def test_tabela_pdo_oper_uct():
     m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        pdo = PdoOperUct.le_arquivo("")
+        pdo = PdoOperUct.read(ARQ_TESTE)
 
         assert pdo.tabela.at[0, "estagio"] == 1
         assert pdo.tabela.at[0, "indice_usina"] == 1
         assert pdo.tabela.at[0, "unidade"] == 1
         assert pdo.tabela.at[0, "nome_usina"] == "ANGRA 1"
         assert pdo.tabela.at[0, "submercado"] == "SE"
         assert pdo.tabela.at[0, "barra"] == 10
@@ -64,19 +66,19 @@
         assert pdo.tabela.at[0, "unidade_equivalente"] == 0
         assert pd.isna(pdo.tabela.at[0, "rampa_transicao"])
 
 
 def test_eq_pdo_oper_uct():
     m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        pdo1 = PdoOperUct.le_arquivo("")
-        pdo2 = PdoOperUct.le_arquivo("")
+        pdo1 = PdoOperUct.read(ARQ_TESTE)
+        pdo2 = PdoOperUct.read(ARQ_TESTE)
         assert pdo1 == pdo2
 
 
 def test_neq_pdo_oper_uct():
     m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        pdo1 = PdoOperUct.le_arquivo("")
-        pdo2 = PdoOperUct.le_arquivo("")
+        pdo1 = PdoOperUct.read(ARQ_TESTE)
+        pdo2 = PdoOperUct.read(ARQ_TESTE)
         pdo1.tabela.iloc[0, 0] = -1
         assert pdo1 != pdo2
```

### Comparing `idessem-0.0.5/tests/dessem/test_pdo_sist.py` & `idessem-0.0.6/tests/dessem/test_pdo_sist.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.pdo_sist import MockPdoSist
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_pdo_sist():
     m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = PdoSist.le_arquivo("")
+        log = PdoSist.read(ARQ_TESTE)
         assert log.versao is not None
         assert log.data_estudo is not None
         assert log.tabela is not None
 
 
 def test_versao_pdo_sist():
     m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = PdoSist.le_arquivo("")
+        log = PdoSist.read(ARQ_TESTE)
         assert log.versao == "19.3"
 
 
 def test_data_estudo_pdo_sist():
     m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = PdoSist.le_arquivo("")
+        log = PdoSist.read(ARQ_TESTE)
         assert log.data_estudo == datetime(year=2022, month=8, day=11)
 
 
 def test_tabela_pdo_sist():
     m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log = PdoSist.le_arquivo("")
+        log = PdoSist.read(ARQ_TESTE)
         assert log.tabela.at[0, "estagio"] == 1
         assert log.tabela.at[0, "patamar"] == "LEVE"
         assert log.tabela.at[0, "submercado"] == "SE"
         assert log.tabela.at[0, "cmo"] == 71.48
         assert log.tabela.at[0, "demanda"] == 36935.91
         assert log.tabela.at[0, "perdas"] == "-"
         assert log.tabela.at[0, "geracao_pequenas_usinas"] == 0.0
@@ -55,19 +57,19 @@
         assert log.tabela.at[0, "geracao_termica_maxima"] == 9489.79
         assert log.tabela.at[0, "energia_armazenada"] == 122020.78
 
 
 def test_eq_pdo_sist():
     m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log1 = PdoSist.le_arquivo("")
-        log2 = PdoSist.le_arquivo("")
+        log1 = PdoSist.read(ARQ_TESTE)
+        log2 = PdoSist.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_pdo_sist():
     m: MagicMock = mock_open(read_data="".join(MockPdoSist))
     with patch("builtins.open", m):
-        log1 = PdoSist.le_arquivo("")
-        log2 = PdoSist.le_arquivo("")
+        log1 = PdoSist.read(ARQ_TESTE)
+        log2 = PdoSist.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/dessem/test_polinjus.py` & `idessem-0.0.6/tests/dessem/test_polinjus.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from idessem.dessem.polinjus import Polinjus
 from idessem.dessem.polinjus import (
     HidreletricaCurvaJusante,
     HidreletricaCurvaJusantePolinomioPorPartes,
     HidreletricaCurvaJusantePolinomioPorPartesSegmento,
+    HidreletricaCurvaJusanteAfogamentoExplicitoUsina,
+    HidreletricaCurvaJusanteAfogamentoExplicitoPadrao,
 )
 import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.polinjus import (
     MockPolinjus,
     MockHidreletricaCurvaJusante,
     MockHidreletricaCurvaJusantePolinomio,
     MockHidreletricaCurvaJusantePolinomioSegmento,
+    MockHidreletricaCurvaJusanteAfogamentoExplicitoUsina,
+    MockHidreletricaCurvaJusanteAfogamentoExplicitoPadrao,
 )
 
+ARQ_TESTE = "./tests/__init__.py"
+
 
 def test_atributos_encontrados_polinjus():
     m: MagicMock = mock_open(read_data="".join(MockPolinjus))
     with patch("builtins.open", m):
-        polinjus = Polinjus.le_arquivo("")
+        polinjus = Polinjus.read(ARQ_TESTE)
         assert polinjus.hidreletrica_curvajusante() is not None
         assert polinjus.hidreletrica_curvajusante_polinomio() is not None
         assert (
             polinjus.hidreletrica_curvajusante_polinomio_segmento() is not None
         )
+        assert (
+            polinjus.hidreletrica_curvajusante_afogamentoexplicito_usina()
+            is not None
+        )
+        assert (
+            polinjus.hidreletrica_curvajusante_afogamentoexplicito_padrao()
+            is not None
+        )
 
 
 def test_df_polinjus_hidreletrica_curvajusante():
     m: MagicMock = mock_open(read_data="".join(MockPolinjus))
     with patch("builtins.open", m):
-        polinjus = Polinjus.le_arquivo("")
+        polinjus = Polinjus.read(ARQ_TESTE)
         df_curvajusante = polinjus.hidreletrica_curvajusante(df=True)
         assert df_curvajusante.at[2, "codigo_usina"] == 1
         assert df_curvajusante.at[2, "indice_familia"] == 3
         assert df_curvajusante.at[2, "nivel_montante_referencia"] == 885.70
 
 
 def test_registro_polinjus_hidreletrica_curvajusante():
@@ -56,15 +70,15 @@
     r.nivel_montante_referencia = 0
     assert r.nivel_montante_referencia == 0
 
 
 def test_df_polinjus_hidreletrica_curvajusante_polinomio():
     m: MagicMock = mock_open(read_data="".join(MockPolinjus))
     with patch("builtins.open", m):
-        polinjus = Polinjus.le_arquivo("")
+        polinjus = Polinjus.read(ARQ_TESTE)
         df_curvajusante_polinomio = (
             polinjus.hidreletrica_curvajusante_polinomio(df=True)
         )
         assert df_curvajusante_polinomio.at[2, "codigo_usina"] == 1
         assert df_curvajusante_polinomio.at[2, "indice_familia"] == 3
         assert df_curvajusante_polinomio.at[2, "numero_polinomios"] == 3
 
@@ -89,15 +103,15 @@
     r.numero_polinomios = 0
     assert r.numero_polinomios == 0
 
 
 def test_df_polinjus_hidreletrica_curvajusante_polinomio_segmento():
     m: MagicMock = mock_open(read_data="".join(MockPolinjus))
     with patch("builtins.open", m):
-        polinjus = Polinjus.le_arquivo("")
+        polinjus = Polinjus.read(ARQ_TESTE)
         df_curvajusante_polinomio_segmento = (
             polinjus.hidreletrica_curvajusante_polinomio_segmento(df=True)
         )
         assert df_curvajusante_polinomio_segmento.at[2, "codigo_usina"] == 1
         assert df_curvajusante_polinomio_segmento.at[2, "indice_familia"] == 2
         assert (
             df_curvajusante_polinomio_segmento.at[2, "indice_polinomio"] == 1
@@ -185,24 +199,80 @@
     r.coeficiente_a3 = -1
     assert r.coeficiente_a3 == -1
     assert r.coeficiente_a4 == 0.00000000000000e01
     r.coeficiente_a4 = -1
     assert r.coeficiente_a4 == -1
 
 
+def test_df_polinjus_hidreletrica_curvajusante_afogamentoexplicito_usina():
+    m: MagicMock = mock_open(read_data="".join(MockPolinjus))
+    with patch("builtins.open", m):
+        polinjus = Polinjus.read(ARQ_TESTE)
+        df_curvajusante_afogamentoexplicito_usina = (
+            polinjus.hidreletrica_curvajusante_afogamentoexplicito_usina(
+                df=True
+            )
+        )
+        assert (
+            df_curvajusante_afogamentoexplicito_usina.at[2, "codigo_usina"]
+            == 54
+        )
+        assert (
+            df_curvajusante_afogamentoexplicito_usina.at[
+                2, "considera_afogamento"
+            ]
+            == "nao"
+        )
+
+
+def test_registro_polinjus_hidreletrica_curvajusante_afogamentoexplicito_usina():
+    m: MagicMock = mock_open(
+        read_data="".join(MockHidreletricaCurvaJusanteAfogamentoExplicitoUsina)
+    )
+    r = HidreletricaCurvaJusanteAfogamentoExplicitoUsina()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
+
+    assert r.data == [22, "sim"]
+    assert r.codigo_usina == 22
+    r.codigo_usina = 0
+    assert r.codigo_usina == 0
+    assert r.considera_afogamento == "sim"
+    r.considera_afogamento = "nao"
+    assert r.considera_afogamento == "nao"
+
+
+def test_registro_polinjus_hidreletrica_curvajusante_afogamentoexplicito_padrao():
+    m: MagicMock = mock_open(
+        read_data="".join(
+            MockHidreletricaCurvaJusanteAfogamentoExplicitoPadrao
+        )
+    )
+    r = HidreletricaCurvaJusanteAfogamentoExplicitoPadrao()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
+
+    assert r.data == ["nao"]
+    assert r.considera_afogamento == "nao"
+    r.considera_afogamento = "sim"
+    assert r.considera_afogamento == "sim"
+
+
 def test_eq_polinjus():
     m: MagicMock = mock_open(read_data="".join(MockPolinjus))
     with patch("builtins.open", m):
-        log1 = Polinjus.le_arquivo("")
-        log2 = Polinjus.le_arquivo("")
+        log1 = Polinjus.read(ARQ_TESTE)
+        log2 = Polinjus.read(ARQ_TESTE)
         assert log1 == log2
 
 
 def test_neq_polinjus():
     m: MagicMock = mock_open(read_data="".join(MockPolinjus))
     with patch("builtins.open", m):
-        log1 = Polinjus.le_arquivo("")
-        log2 = Polinjus.le_arquivo("")
+        log1 = Polinjus.read(ARQ_TESTE)
+        log2 = Polinjus.read(ARQ_TESTE)
         log1.hidreletrica_curvajusante_polinomio_segmento()[
             0
         ].codigo_usina = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.5/tests/mocks/arquivos/avl_altqueda.py` & `idessem-0.0.6/tests/mocks/arquivos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/avl_desvfpha.py` & `idessem-0.0.6/tests/mocks/arquivos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/avl_fpha1.py` & `idessem-0.0.6/tests/mocks/arquivos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/des_log_relato.py` & `idessem-0.0.6/tests/mocks/arquivos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/log_matriz.py` & `idessem-0.0.6/tests/mocks/arquivos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/operut.py` & `idessem-0.0.6/tests/mocks/arquivos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/pdo_eco_usih.py` & `idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/pdo_hidr.py` & `idessem-0.0.6/tests/mocks/arquivos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/pdo_oper_uct.py` & `idessem-0.0.6/tests/mocks/arquivos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/pdo_sist.py` & `idessem-0.0.6/tests/mocks/arquivos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.5/tests/mocks/arquivos/polinjus.py` & `idessem-0.0.6/tests/mocks/arquivos/polinjus.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,18 +199,30 @@
     "HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES-SEGMENTO;0010;001; 1;               0.000;            3931.811;4.93556500000000E+02;1.45685300000000E-03;3.82077800000000E-08;-7.6535160000000E-11;9.61812000000000E-15\n",
     "HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES-SEGMENTO;0010;001; 2;            3931.811;           11252.960;4.93953400000000E+02;1.39952600000000E-03;-1.6274530000000E-07;1.06834400000000E-11;-2.8370270000000E-16\n",
     " &\n",
     "HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES-SEGMENTO;0010;002; 1;               0.000;             946.902;4.93572500000000E+02;2.09901800000000E-03;-1.3804510000000E-06;6.95680500000000E-10;0.00000000000000E+00\n",
     "HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES-SEGMENTO;0010;002; 2;             946.902;            3931.811;4.93556500000000E+02;1.45685300000000E-03;3.82077800000000E-08;-7.6535160000000E-11;9.61812000000000E-15\n",
     "HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES-SEGMENTO;0010;002; 3;            3931.811;           11252.960;4.93953400000000E+02;1.39952600000000E-03;-1.6274530000000E-07;1.06834400000000E-11;-2.8370270000000E-16\n",
     " &\n",
+    "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-USINA;0022;sim\n",
+    "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-USINA;0044;sim\n",
+    "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-USINA;0054;nao\n",
+    "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-PADRAO;nao\n",
 ]
 
 MockHidreletricaCurvaJusante = (
     " HIDRELETRICA-CURVAJUSANTE                   ;0001;001;  885.3052"
 )
 
 MockHidreletricaCurvaJusantePolinomio = (
     " HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES;0001;001;002"
 )
 
 MockHidreletricaCurvaJusantePolinomioSegmento = "HIDRELETRICA-CURVAJUSANTE-POLINOMIOPORPARTES-SEGMENTO;0001;001; 1;               0.000;             408.649;0.88530520000000E+03;-.31521360000000E-17;0.19686530000000E-04;-.25518040000000E-07;0.00000000000000E+01"
+
+MockHidreletricaCurvaJusanteAfogamentoExplicitoUsina = (
+    "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-USINA;0022;sim"
+)
+
+MockHidreletricaCurvaJusanteAfogamentoExplicitoPadrao = (
+    "HIDRELETRICA-CURVAJUSANTE-AFOGAMENTO-EXPLICITO-PADRAO;nao"
+)
```

### Comparing `idessem-0.0.5/tests/mocks/mock_open.py` & `idessem-0.0.6/tests/mocks/mock_open.py`

 * *Files identical despite different names*

