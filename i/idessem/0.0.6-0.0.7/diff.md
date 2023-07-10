# Comparing `tmp/idessem-0.0.6.tar.gz` & `tmp/idessem-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idessem-0.0.6.tar", last modified: Mon Jul 10 15:21:49 2023, max compression
+gzip compressed data, was "idessem-0.0.7.tar", last modified: Mon Jul 10 19:16:35 2023, max compression
```

## Comparing `idessem-0.0.6.tar` & `idessem-0.0.7.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 15:19:49.000000 idessem-0.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 15:21:49.484317 idessem-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-10 15:19:49.000000 idessem-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.472317 idessem-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.472317 idessem-0.0.6/idessem/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.476318 idessem-0.0.6/idessem/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_estatfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/log_matriz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/idessem/dessem/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/idessem/dessem/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/arquivos/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/avl_fpha1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/idessem/dessem/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/dataestudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)   142870 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/modelos/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/dessem/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/idessem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.476318 idessem-0.0.6/idessem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 15:21:49.000000 idessem-0.0.6/idessem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:21:49.484317 idessem-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-10 15:19:49.000000 idessem-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.480317 idessem-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/tests/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/dessem/test_renovaveis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:21:49.484317 idessem-0.0.6/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/arquivos/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 15:19:49.000000 idessem-0.0.6/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.171421 idessem-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 19:14:47.000000 idessem-0.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 19:16:35.171421 idessem-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-10 19:14:47.000000 idessem-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.143421 idessem-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.143421 idessem-0.0.7/idessem/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.151421 idessem-0.0.7/idessem/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/log_matriz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.155421 idessem-0.0.7/idessem/dessem/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.155421 idessem-0.0.7/idessem/dessem/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/arquivos/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/avl_fpha1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.159421 idessem-0.0.7/idessem/dessem/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/dataestudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142870 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.143421 idessem-0.0.7/idessem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:16:35.171421 idessem-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-10 19:14:47.000000 idessem-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.159421 idessem-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.163421 idessem-0.0.7/tests/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_renovaveis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.163421 idessem-0.0.7/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.167421 idessem-0.0.7/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/mock_open.py
```

### Comparing `idessem-0.0.6/LICENSE.md` & `idessem-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/PKG-INFO` & `idessem-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.6/README.md` & `idessem-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/avl_altqueda.py` & `idessem-0.0.7/idessem/dessem/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/avl_desvfpha.py` & `idessem-0.0.7/idessem/dessem/pdo_sist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,63 @@
-from idessem.dessem.modelos.avl_desvfpha import TabelaAvlDesvFpha
+from idessem.dessem.modelos.pdo_sist import TabelaPdoSist
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class AvlDesvFpha(ArquivoCSV):
+class PdoSist(ArquivoCSV):
     """
-    Armazena os dados das saídas referentes aos desvios da função de produção.
+    Armazena os dados das saídas referentes aos submercados.
 
-    Essa classe lida com as informações de saída fornecidas pelo arquivo AVL_DESVFPHA.
+    Essa classe lida com as informações de saída fornecidas pelo arquivo PDO_SIST.
     """
 
-    BLOCKS = [VersaoModelo, DataEstudo, TabelaAvlDesvFpha]
+    BLOCKS = [VersaoModelo, DataEstudo, TabelaPdoSist]
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="AVL_DESVFPHA.DAT"
-    ) -> "AvlDesvFpha":
+        cls, diretorio: str, nome_arquivo="PDO_SIST.DAT"
+    ) -> "PdoSist":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
     @property
     def tabela(self):
         """
-        Obtém a tabela com informações referente aos desvios da função de produção.
+        Obtém a tabela com informações referente a operação por submercado.
 
         - estagio (`int`)
-        - indice_usina (`int`)
-        - nome_usina (`str`)
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
+        - patamar (`float`)
+        - submercado (`str`)
+        - cmo (`float`)
+        - demanda (`float`)
+        - perdas (`str`)
+        - geracao_pequenas_usinas (`float`)
+        - geracao_fixa_barra (`float`)
+        - geracao_renovavel (`float`)
+        - geracao_hidraulica (`float`)
+        - geracao_termica (`float`)
+        - consumo_elevatorias (`float`)
+        - importacao (`float`)
+        - exportacao (`float`)
+        - corte_carga (`float`)
+        - saldo (`float`)
+        - recebimento (`float`)
+        - geracao_termica_minima (`float`)
+        - geracao_termica_maxima (`float`)
+        - energia_armazenada (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `idessem-0.0.6/idessem/dessem/avl_fpha1.py` & `idessem-0.0.7/idessem/dessem/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/des_log_relato.py` & `idessem-0.0.7/idessem/dessem/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/dessemarq.py` & `idessem-0.0.7/idessem/dessem/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/entdados.py` & `idessem-0.0.7/idessem/dessem/entdados.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/hidr.py` & `idessem-0.0.7/idessem/dessem/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/log_matriz.py` & `idessem-0.0.7/idessem/dessem/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/arquivos/arquivocsv.py` & `idessem-0.0.7/idessem/dessem/modelos/arquivos/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/avl_altqueda.py` & `idessem-0.0.7/idessem/dessem/modelos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/avl_desvfpha.py` & `idessem-0.0.7/idessem/dessem/modelos/pdo_oper_uct.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 from cfinterface.components.line import Line
 from idessem.dessem.modelos.blocos.tabelacsv import TabelaCSV
 
 
-class TabelaAvlDesvFpha(TabelaCSV):
+class TabelaPdoOperUct(TabelaCSV):
     """
-    Bloco com as informações da tabela do arquivo AVL_DESVFPHA.
+    Bloco com as informações da tabela do arquivo PDO_OPER_UCT.
     """
 
     BEGIN_PATTERN = "-----;-----;"
     LINE_MODEL = Line(
         [
             IntegerField(size=5),
             IntegerField(size=5),
+            IntegerField(size=6),
             LiteralField(size=14),
-            FloatField(size=10, decimal_digits=2),
-            FloatField(size=10, decimal_digits=2),
+            LiteralField(size=8),
+            IntegerField(size=8),
+            IntegerField(size=7),
+            IntegerField(size=8),
             FloatField(size=9, decimal_digits=2),
-            FloatField(size=12, decimal_digits=2),
             FloatField(size=9, decimal_digits=2),
+            FloatField(size=9, decimal_digits=3),
             FloatField(size=9, decimal_digits=2),
             FloatField(size=9, decimal_digits=2),
+            IntegerField(size=5),
+            IntegerField(size=5),
+            IntegerField(size=3),
+            FloatField(size=9, decimal_digits=2),
+            FloatField(size=10, decimal_digits=1),
             FloatField(size=9, decimal_digits=2),
             FloatField(size=9, decimal_digits=2),
-            FloatField(size=15, decimal_digits=6),
-            FloatField(size=7, decimal_digits=2),
-            IntegerField(size=6),
-            IntegerField(size=4),
-            FloatField(size=10, decimal_digits=2),
-            FloatField(size=10, decimal_digits=2),
             FloatField(size=10, decimal_digits=2),
-            FloatField(size=14, decimal_digits=2),
-            FloatField(size=15, decimal_digits=2),
-            FloatField(size=14, decimal_digits=2),
-            FloatField(size=15, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            LiteralField(size=30),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            IntegerField(size=5),
+            FloatField(size=12, decimal_digits=2),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
         "estagio",
         "indice_usina",
+        "unidade",
         "nome_usina",
-        "volume_medio_hm3",
-        "volume_medio_percentual",
-        "vazao_turbinada_m3s",
-        "vazao_vertida_m3s",
-        "vazao_jusante_m3s",
-        "vazao_lateral_usina_m3s",
-        "vazao_lateral_posto_m3s",
-        "altura_jusante",
-        "altura_montante",
-        "produtibilidade_especifica",
-        "perdas_hidraulicas",
-        "influencia_vertimento_canal_fuga",
-        "afogamento_canal_fuga",
-        "geracao_fph",
-        "geracao_pl",
-        "geracao_fpha",
-        "desvio_absoluto_fph_pl",
-        "desvio_percentual_fph_pl",
-        "desvio_absoluto_fph_fpha",
-        "desvio_percentual_fph_fpha",
+        "submercado",
+        "barra",
+        "numero_maximo_oscilacoes",
+        "flag_geracao_minima_maxima",
+        "geracao_minima",
+        "geracao_minima_unidade",
+        "geracao_maxima",
+        "geracao_maxima_unidade",
+        "geracao_minima_acionamento",
+        "tempo_on",
+        "tempo_off",
+        "status",
+        "geracao",
+        "tempo",
+        "custo_linear",
+        "custo_partida_unidade",
+        "cmo",
+        "cmb",
+        "variavel_dual",
+        "titulacao",
+        "rampa_subida",
+        "rampa_descida",
+        "unidade_equivalente",
+        "rampa_transicao",
     ]
     END_PATTERN = ""
```

### Comparing `idessem-0.0.6/idessem/dessem/modelos/avl_fpha1.py` & `idessem-0.0.7/idessem/dessem/modelos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/blocos/dataestudo.py` & `idessem-0.0.7/idessem/dessem/modelos/blocos/dataestudo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/blocos/tabelacsv.py` & `idessem-0.0.7/idessem/dessem/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/blocos/versaomodelo.py` & `idessem-0.0.7/idessem/dessem/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/des_log_relato.py` & `idessem-0.0.7/idessem/dessem/modelos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/dessemarq.py` & `idessem-0.0.7/idessem/dessem/modelos/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/entdados.py` & `idessem-0.0.7/idessem/dessem/modelos/entdados.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/hidr.py` & `idessem-0.0.7/idessem/dessem/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/log_matriz.py` & `idessem-0.0.7/idessem/dessem/modelos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/operut.py` & `idessem-0.0.7/idessem/dessem/modelos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/pdo_eco_fcfcortes.py` & `idessem-0.0.7/idessem/dessem/modelos/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih.py` & `idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,87 @@
 from cfinterface.components.floatfield import FloatField
 from cfinterface.components.line import Line
 from idessem.dessem.modelos.blocos.tabelacsv import TabelaCSV
 
 
 class TabelaPdoEcoUsih(TabelaCSV):
     """
-    Bloco com as informações da tabela do arquivo PDO_ECO_USIH.
+    Bloco com as informações da tabela do arquivo PDO_ECO_USIH,
+    válido a partir da versão 19.4.2.
+    """
+
+    BEGIN_PATTERN = "-----;--------------;"
+    LINE_MODEL = Line(
+        [
+            IntegerField(size=5),
+            LiteralField(size=14),
+            LiteralField(size=8),
+            IntegerField(size=7),
+            IntegerField(size=7),
+            IntegerField(size=8),
+            IntegerField(size=5),
+            FloatField(size=9, decimal_digits=2),
+            FloatField(size=9, decimal_digits=2),
+            FloatField(size=10, decimal_digits=2),
+            FloatField(size=10, decimal_digits=2),
+            FloatField(size=9, decimal_digits=2),
+            FloatField(size=9, decimal_digits=2),
+            FloatField(size=11, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=11, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=9, decimal_digits=2),
+            LiteralField(size=7),
+            LiteralField(size=7),
+            IntegerField(size=7),
+            IntegerField(size=3),
+            FloatField(size=15, decimal_digits=6),
+            LiteralField(size=5),
+            FloatField(size=7, decimal_digits=3),
+            FloatField(size=8, decimal_digits=2),
+            IntegerField(size=6),
+        ],
+        delimiter=";",
+    )
+    COLUMN_NAMES = [
+        "indice_usina",
+        "nome_usina",
+        "submercado",
+        "indice_usina_jusante",
+        "indice_usina_desvio",
+        "indice_usina_jusante_earm",
+        "estagio_inicial",
+        "volume_morto_inicial_hm3",
+        "volume_morto_inicial_percentual",
+        "volume_util_inicial_hm3",
+        "volume_util_inicial_percentual",
+        "volume_armazenado_minimo_hm3",
+        "volume_armazenado_maximo_hm3",
+        "volume_soleira_vertedouro_hm3",
+        "volume_soleira_vertedouro_util_percentual",
+        "volume_soleira_desvio_hm3",
+        "volume_soleira_desvio_util_percentual",
+        "volume_referencia_hm3",
+        "tipo_reservatorio",
+        "tipo_regularizacao",
+        "flag_evaporacao",
+        "numero_conjuntos",
+        "produtibilidade_especifica",
+        "tipo_perdas",
+        "perdas_hidraulicas",
+        "canal_fuga_medio",
+        "influencia_vertimento_canal_fuga",
+    ]
+    END_PATTERN = ""
+
+
+class TabelaPdoEcoUsih190301(TabelaCSV):
+    """
+    Bloco com as informações da tabela do arquivo PDO_ECO_USIH,
+    válido a partir da versão 19.3.1.
     """
 
     BEGIN_PATTERN = "-----;--------------;"
     LINE_MODEL = Line(
         [
             IntegerField(size=5),
             LiteralField(size=14),
```

### Comparing `idessem-0.0.6/idessem/dessem/modelos/pdo_eco_usih_polin.py` & `idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/pdo_hidr.py` & `idessem-0.0.7/idessem/dessem/modelos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/pdo_oper_uct.py` & `idessem-0.0.7/idessem/dessem/modelos/pdo_sist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,61 @@
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 from cfinterface.components.line import Line
 from idessem.dessem.modelos.blocos.tabelacsv import TabelaCSV
 
 
-class TabelaPdoOperUct(TabelaCSV):
+class TabelaPdoSist(TabelaCSV):
     """
-    Bloco com as informações da tabela do arquivo PDO_OPER_UCT.
+    Bloco com as informações da tabela do arquivo PDO_SIST.
     """
 
-    BEGIN_PATTERN = "-----;-----;"
+    BEGIN_PATTERN = "------;--------;"
     LINE_MODEL = Line(
         [
-            IntegerField(size=5),
-            IntegerField(size=5),
             IntegerField(size=6),
-            LiteralField(size=14),
             LiteralField(size=8),
-            IntegerField(size=8),
-            IntegerField(size=7),
-            IntegerField(size=8),
-            FloatField(size=9, decimal_digits=2),
-            FloatField(size=9, decimal_digits=2),
-            FloatField(size=9, decimal_digits=3),
-            FloatField(size=9, decimal_digits=2),
-            FloatField(size=9, decimal_digits=2),
-            IntegerField(size=5),
-            IntegerField(size=5),
-            IntegerField(size=3),
-            FloatField(size=9, decimal_digits=2),
-            FloatField(size=10, decimal_digits=1),
-            FloatField(size=9, decimal_digits=2),
-            FloatField(size=9, decimal_digits=2),
-            FloatField(size=10, decimal_digits=2),
+            LiteralField(size=6),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            LiteralField(size=12),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
+            FloatField(size=12, decimal_digits=2),
             FloatField(size=12, decimal_digits=2),
             FloatField(size=12, decimal_digits=2),
-            LiteralField(size=30),
             FloatField(size=12, decimal_digits=2),
             FloatField(size=12, decimal_digits=2),
-            IntegerField(size=5),
             FloatField(size=12, decimal_digits=2),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
         "estagio",
-        "indice_usina",
-        "unidade",
-        "nome_usina",
+        "patamar",
         "submercado",
-        "barra",
-        "numero_maximo_oscilacoes",
-        "flag_geracao_minima_maxima",
-        "geracao_minima",
-        "geracao_minima_unidade",
-        "geracao_maxima",
-        "geracao_maxima_unidade",
-        "geracao_minima_acionamento",
-        "tempo_on",
-        "tempo_off",
-        "status",
-        "geracao",
-        "tempo",
-        "custo_linear",
-        "custo_partida_unidade",
         "cmo",
-        "cmb",
-        "variavel_dual",
-        "titulacao",
-        "rampa_subida",
-        "rampa_descida",
-        "unidade_equivalente",
-        "rampa_transicao",
+        "demanda",
+        "perdas",
+        "geracao_pequenas_usinas",
+        "geracao_fixa_barra",
+        "geracao_renovavel",
+        "geracao_hidraulica",
+        "geracao_termica",
+        "consumo_elevatorias",
+        "importacao",
+        "exportacao",
+        "corte_carga",
+        "saldo",
+        "recebimento",
+        "geracao_termica_minima",
+        "geracao_termica_maxima",
+        "energia_armazenada",
     ]
     END_PATTERN = ""
```

### Comparing `idessem-0.0.6/idessem/dessem/modelos/polinjus.py` & `idessem-0.0.7/idessem/dessem/modelos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/modelos/renovaveis.py` & `idessem-0.0.7/idessem/dessem/modelos/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/operut.py` & `idessem-0.0.7/idessem/dessem/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/pdo_eco_fcfcortes.py` & `idessem-0.0.7/idessem/dessem/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/pdo_eco_usih.py` & `idessem-0.0.7/idessem/dessem/pdo_eco_usih.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from idessem.dessem.modelos.pdo_eco_usih import TabelaPdoEcoUsih
+from idessem.dessem.modelos.pdo_eco_usih import (
+    TabelaPdoEcoUsih,
+    TabelaPdoEcoUsih190301,
+)
 from idessem.dessem.modelos.arquivos.arquivocsv import (
     DataEstudo,
     VersaoModelo,
     ArquivoCSV,
 )
 
 # Para compatibilidade - até versão 1.0.0
@@ -14,14 +17,18 @@
     """
     Armazena os dados de eco referentes as usinas hidráulicas.
 
     Essa classe lida com as informações de saída fornecidas pelo arquivo PDO_ECO_USIH.
     """
 
     BLOCKS = [VersaoModelo, DataEstudo, TabelaPdoEcoUsih]
+    VERSIONS = {
+        "19.3.1": [VersaoModelo, DataEstudo, TabelaPdoEcoUsih190301],
+        "19.4.2": [VersaoModelo, DataEstudo, TabelaPdoEcoUsih],
+    }
     ENCODING = "iso-8859-1"
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="PDO_ECO_USIH.DAT"
     ) -> "PdoEcoUsih":
         msg = (
@@ -51,14 +58,15 @@
         - volume_armazenado_minimo_hm3 (`float`)
         - volume_armazenado_maximo_hm3 (`float`)
         - volume_soleira_vertedouro_hm3 (`float`)
         - volume_soleira_vertedouro_util_percentual (`float`)
         - volume_soleira_desvio_hm3 (`float`)
         - volume_soleira_desvio_util_percentual (`float`)
         - volume_referencia_hm3 (`float`)
+        - tipo_reservatorio (`str`)
         - tipo_regularizacao (`str`)
         - flag_evaporacao (`int`)
         - numero_conjuntos (`int`)
         - produtibilidade_especifica (`float`)
         - tipo_perdas (`str`)
         - perdas_hidraulicas (`float`)
         - canal_fuga_medio (`float`)
```

### Comparing `idessem-0.0.6/idessem/dessem/pdo_eco_usih_polin.py` & `idessem-0.0.7/idessem/dessem/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/pdo_hidr.py` & `idessem-0.0.7/idessem/dessem/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/pdo_oper_uct.py` & `idessem-0.0.7/idessem/dessem/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/polinjus.py` & `idessem-0.0.7/idessem/dessem/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem/dessem/renovaveis.py` & `idessem-0.0.7/idessem/dessem/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/idessem.egg-info/PKG-INFO` & `idessem-0.0.7/idessem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.6
+Version: 0.0.7
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.6/idessem.egg-info/SOURCES.txt` & `idessem-0.0.7/idessem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/setup.py` & `idessem-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_avl_altqueda.py` & `idessem-0.0.7/tests/dessem/test_avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_avl_desvfpha.py` & `idessem-0.0.7/tests/dessem/test_pdo_oper_uct.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,84 @@
-from idessem.dessem.avl_desvfpha import AvlDesvFpha
-
+from idessem.dessem.pdo_oper_uct import PdoOperUct
+import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.avl_desvfpha import MockAvlDesvfpha
+from tests.mocks.arquivos.pdo_oper_uct import MockPdoOperUct
 
 ARQ_TESTE = "./tests/__init__.py"
 
 
-def test_atributos_encontrados_avl_desvfpha():
-    m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
+def test_atributos_encontrados_pdo_oper_uct():
+    m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
     with patch("builtins.open", m):
-        log = AvlDesvFpha.read(ARQ_TESTE)
-        assert log.versao is not None
-        assert log.data_estudo is not None
-        assert log.tabela is not None
-
-
-def test_versao_avl_desvfpha():
-    m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
-    with patch("builtins.open", m):
-        log = AvlDesvFpha.read(ARQ_TESTE)
-        assert log.versao == "19.3"
-
-
-def test_data_estudo_avl_desvfpha():
-    m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
-    with patch("builtins.open", m):
-        log = AvlDesvFpha.read(ARQ_TESTE)
-        assert log.data_estudo == datetime(year=2022, month=8, day=11)
-
-
-def test_tabela_avl_desvfpha():
-    m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
-    with patch("builtins.open", m):
-        log = AvlDesvFpha.read(ARQ_TESTE)
-        assert log.tabela.at[0, "estagio"] == 1
-        assert log.tabela.at[0, "indice_usina"] == 1
-        assert log.tabela.at[0, "nome_usina"] == "CAMARGOS"
-        assert log.tabela.at[0, "volume_medio_hm3"] == 700.64
-        assert log.tabela.at[0, "volume_medio_percentual"] == 86.40
-        assert log.tabela.at[0, "vazao_turbinada_m3s"] == 160.50
-        assert log.tabela.at[0, "vazao_vertida_m3s"] == 0.0
-        assert log.tabela.at[0, "vazao_jusante_m3s"] == 160.0
-        assert log.tabela.at[0, "vazao_lateral_usina_m3s"] == 0.0
-        assert log.tabela.at[0, "vazao_lateral_posto_m3s"] == 0.0
-        assert log.tabela.at[0, "altura_jusante"] == 886.10
-        assert log.tabela.at[0, "altura_montante"] == 911.78
-        assert log.tabela.at[0, "produtibilidade_especifica"] == 0.008767
-        assert log.tabela.at[0, "perdas_hidraulicas"] == 0.0
-        assert log.tabela.at[0, "influencia_vertimento_canal_fuga"] == 0
-        assert log.tabela.at[0, "afogamento_canal_fuga"] == 0
-        assert log.tabela.at[0, "geracao_fph"] == 36.14
-        assert log.tabela.at[0, "geracao_pl"] == 36.14
-        assert log.tabela.at[0, "geracao_fpha"] == 36.14
-        assert log.tabela.at[0, "desvio_absoluto_fph_pl"] == 0.0
-        assert log.tabela.at[0, "desvio_percentual_fph_pl"] == -0.01
-        assert log.tabela.at[0, "desvio_absoluto_fph_fpha"] == 0.0
-        assert log.tabela.at[0, "desvio_percentual_fph_fpha"] == -0.01
-
-
-def test_eq_avl_desvfpha():
-    m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
-    with patch("builtins.open", m):
-        log1 = AvlDesvFpha.read(ARQ_TESTE)
-        log2 = AvlDesvFpha.read(ARQ_TESTE)
-        assert log1 == log2
-
-
-def test_neq_avl_desvfpha():
-    m: MagicMock = mock_open(read_data="".join(MockAvlDesvfpha))
-    with patch("builtins.open", m):
-        log1 = AvlDesvFpha.read(ARQ_TESTE)
-        log2 = AvlDesvFpha.read(ARQ_TESTE)
-        log1.tabela.iloc[0, 0] = -1
-        assert log1 != log2
+        pdo = PdoOperUct.read(ARQ_TESTE)
+        assert pdo.versao is not None
+        assert pdo.data_estudo is not None
+        assert pdo.tabela is not None
+
+
+def test_versao_pdo_oper_uct():
+    m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
+    with patch("builtins.open", m):
+        pdo = PdoOperUct.read(ARQ_TESTE)
+        assert pdo.versao == "19.0.42"
+
+
+def test_data_estudo_pdo_oper_uct():
+    m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
+    with patch("builtins.open", m):
+        pdo = PdoOperUct.read(ARQ_TESTE)
+        assert pdo.data_estudo == datetime(year=2022, month=8, day=8)
+
+
+def test_tabela_pdo_oper_uct():
+    m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
+    with patch("builtins.open", m):
+        pdo = PdoOperUct.read(ARQ_TESTE)
+
+        assert pdo.tabela.at[0, "estagio"] == 1
+        assert pdo.tabela.at[0, "indice_usina"] == 1
+        assert pdo.tabela.at[0, "unidade"] == 1
+        assert pdo.tabela.at[0, "nome_usina"] == "ANGRA 1"
+        assert pdo.tabela.at[0, "submercado"] == "SE"
+        assert pdo.tabela.at[0, "barra"] == 10
+        assert pdo.tabela.at[0, "numero_maximo_oscilacoes"] == 0
+        assert pdo.tabela.at[0, "flag_geracao_minima_maxima"] == 0
+        assert pdo.tabela.at[0, "geracao_minima"] == 605.00
+        assert pdo.tabela.at[0, "geracao_minima_unidade"] == 0
+        assert pdo.tabela.at[0, "geracao_maxima"] == 605.00
+        assert pdo.tabela.at[0, "geracao_maxima_unidade"] == 640.00
+        assert pdo.tabela.at[0, "geracao_minima_acionamento"] == 520.00
+        assert pdo.tabela.at[0, "tempo_on"] == 168
+        assert pdo.tabela.at[0, "tempo_off"] == 168
+        assert pdo.tabela.at[0, "status"] == 1
+        assert pdo.tabela.at[0, "geracao"] == 605.00
+        assert pdo.tabela.at[0, "tempo"] == 1512.5
+        assert pdo.tabela.at[0, "custo_linear"] == 31.17
+        assert pdo.tabela.at[0, "custo_partida_unidade"] == 0.00
+        assert pdo.tabela.at[0, "cmo"] == 90.02
+        assert pdo.tabela.at[0, "cmb"] == 90.03
+        assert pdo.tabela.at[0, "variavel_dual"] == 0
+        assert pdo.tabela.at[0, "titulacao"] == "Ordem de merito"
+        assert pdo.tabela.at[0, "rampa_subida"] == 1000000.00
+        assert pdo.tabela.at[0, "rampa_descida"] == 1000000.00
+        assert pdo.tabela.at[0, "unidade_equivalente"] == 0
+        assert pd.isna(pdo.tabela.at[0, "rampa_transicao"])
+
+
+def test_eq_pdo_oper_uct():
+    m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
+    with patch("builtins.open", m):
+        pdo1 = PdoOperUct.read(ARQ_TESTE)
+        pdo2 = PdoOperUct.read(ARQ_TESTE)
+        assert pdo1 == pdo2
+
+
+def test_neq_pdo_oper_uct():
+    m: MagicMock = mock_open(read_data="".join(MockPdoOperUct))
+    with patch("builtins.open", m):
+        pdo1 = PdoOperUct.read(ARQ_TESTE)
+        pdo2 = PdoOperUct.read(ARQ_TESTE)
+        pdo1.tabela.iloc[0, 0] = -1
+        assert pdo1 != pdo2
```

### Comparing `idessem-0.0.6/tests/dessem/test_avl_fpha1.py` & `idessem-0.0.7/tests/dessem/test_avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_des_log_relato.py` & `idessem-0.0.7/tests/dessem/test_des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_dessemarq.py` & `idessem-0.0.7/tests/dessem/test_dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_entdados.py` & `idessem-0.0.7/tests/dessem/test_entdados.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_hidr.py` & `idessem-0.0.7/tests/dessem/test_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_log_matriz.py` & `idessem-0.0.7/tests/dessem/test_log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_operut.py` & `idessem-0.0.7/tests/dessem/test_operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_pdo_eco_fcfcortes.py` & `idessem-0.0.7/tests/dessem/test_pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_pdo_eco_usih.py` & `idessem-0.0.7/tests/dessem/test_pdo_eco_usih_polin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,73 @@
-from idessem.dessem.pdo_eco_usih import PdoEcoUsih
+from idessem.dessem.pdo_eco_usih_polin import PdoEcoUsihPolin
 import pandas as pd  # type: ignore
 from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.pdo_eco_usih import MockPdoEcoUsih
+from tests.mocks.arquivos.pdo_eco_usih_polin import MockPdoEcoUsihPolin
 
 ARQ_TESTE = "./tests/__init__.py"
 
 
-def test_atributos_encontrados_pdo_eco_usih():
-    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
+def test_atributos_encontrados_pdo_eco_usih_polin():
+    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsihPolin))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.read(ARQ_TESTE)
+        pdo = PdoEcoUsihPolin.read(ARQ_TESTE)
         assert pdo.versao is not None
         assert pdo.data_estudo is not None
         assert pdo.tabela is not None
 
 
-def test_versao_pdo_eco_usih():
-    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
+def test_versao_pdo_eco_usih_polin():
+    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsihPolin))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.read(ARQ_TESTE)
-        assert pdo.versao == "19.3.1"
+        pdo = PdoEcoUsihPolin.read(ARQ_TESTE)
+        assert pdo.versao == "19.4.1"
 
 
-def test_data_estudo_pdo_eco_usih():
-    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
+def test_data_estudo_pdo_eco_usih_polin():
+    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsihPolin))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.read(ARQ_TESTE)
-        assert pdo.data_estudo == datetime(year=2022, month=8, day=11)
+        pdo = PdoEcoUsihPolin.read(ARQ_TESTE)
+        assert pdo.data_estudo == datetime(year=2023, month=6, day=13)
 
 
-def test_tabela_pdo_eco_usih():
-    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
+def test_tabela_pdo_eco_usih_polin():
+    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsihPolin))
     with patch("builtins.open", m):
-        pdo = PdoEcoUsih.read(ARQ_TESTE)
+        pdo = PdoEcoUsihPolin.read(ARQ_TESTE)
 
         assert pdo.tabela.at[0, "indice_usina"] == 1
         assert pdo.tabela.at[0, "nome_usina"] == "CAMARGOS"
-        assert pdo.tabela.at[0, "submercado"] == "SE"
-        assert pdo.tabela.at[0, "indice_usina_jusante"] == 2
-        # assert pdo.tabela.at[0, "indice_usina_desvio"] == "-"
-        assert pd.isna(pdo.tabela.at[0, "indice_usina_desvio"])
-        assert pdo.tabela.at[0, "indice_usina_jusante_earm"] == 2
-        assert pdo.tabela.at[0, "estagio_inicial"] == 1
-        # assert pdo.tabela.at[0, "volume_morto_inicial_hm3"] == "-"
-        assert pd.isna(pdo.tabela.at[0, "volume_morto_inicial_hm3"])
-        # assert pdo.tabela.at[0, "volume_morto_inicial_percentual"] == "-"
-        assert pd.isna(pdo.tabela.at[0, "volume_morto_inicial_percentual"])
-        assert pdo.tabela.at[0, "volume_util_inicial_hm3"] == 580.74
-        assert pdo.tabela.at[0, "volume_util_inicial_percentual"] == 86.42
-        assert pdo.tabela.at[0, "volume_armazenado_minimo_hm3"] == 120.00
-        assert pdo.tabela.at[0, "volume_armazenado_maximo_hm3"] == 792.00
-        assert pdo.tabela.at[0, "volume_soleira_vertedouro_hm3"] == 120.00
-        assert (
-            pdo.tabela.at[0, "volume_soleira_vertedouro_util_percentual"] == 0
-        )
-        assert pdo.tabela.at[0, "volume_soleira_desvio_hm3"] == 120.00
-        assert (
-            pdo.tabela.at[0, "volume_soleira_desvio_util_percentual"] == 0.00
-        )
-        assert pdo.tabela.at[0, "volume_referencia_hm3"] == 792.00
-        assert pdo.tabela.at[0, "tipo_regularizacao"] == "M"
-        assert pdo.tabela.at[0, "flag_evaporacao"] == 1
-        assert pdo.tabela.at[0, "numero_conjuntos"] == 1
-        assert pdo.tabela.at[0, "produtibilidade_especifica"] == 0.008767
-        assert pdo.tabela.at[0, "tipo_perdas"] == "m"
-        assert pdo.tabela.at[0, "perdas_hidraulicas"] == 0.09
-        assert pdo.tabela.at[0, "canal_fuga_medio"] == 885.73
-        assert pdo.tabela.at[0, "influencia_vertimento_canal_fuga"] == 0
+        assert pdo.tabela.at[0, "indice_coeficiente"] == 0
+        assert pdo.tabela.at[0, "coeficiente_cota_volume"] == 0.89296997e03
+        assert pdo.tabela.at[0, "coeficiente_area_cota"] == 0.13334300e05
+        assert pdo.tabela.at[0, "cota_vazao_hjus1"] == 0.88609998e03
+        assert pdo.tabela.at[0, "hjus1"] == 0.00
+        assert pdo.tabela.at[0, "cota_vazao_hjus2"] == 0.00000000e00
+        assert pdo.tabela.at[0, "hjus2"] == 0.00
+        assert pdo.tabela.at[0, "cota_vazao_hjus3"] == 0.00000000e00
+        assert pdo.tabela.at[0, "hjus3"] == 0.00
+        assert pdo.tabela.at[0, "cota_vazao_hjus4"] == 0.00000000e00
+        assert pdo.tabela.at[0, "hjus4"] == 0.00
+        assert pdo.tabela.at[0, "cota_vazao_hjus5"] == 0.00000000e00
+        assert pdo.tabela.at[0, "hjus5"] == 0.00
+        assert pdo.tabela.at[0, "cota_vazao_hjus6"] == 0.00000000e00
+        assert pdo.tabela.at[0, "hjus6"] == 0.00
 
 
-def test_eq_pdo_eco_usih():
-    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
+def test_eq_pdo_eco_usih_polin():
+    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsihPolin))
     with patch("builtins.open", m):
-        log1 = PdoEcoUsih.read(ARQ_TESTE)
-        log2 = PdoEcoUsih.read(ARQ_TESTE)
+        log1 = PdoEcoUsihPolin.read(ARQ_TESTE)
+        log2 = PdoEcoUsihPolin.read(ARQ_TESTE)
         assert log1 == log2
 
 
-def test_neq_pdo_eco_usih():
-    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsih))
+def test_neq_pdo_eco_usih_polin():
+    m: MagicMock = mock_open(read_data="".join(MockPdoEcoUsihPolin))
     with patch("builtins.open", m):
-        log1 = PdoEcoUsih.read(ARQ_TESTE)
-        log2 = PdoEcoUsih.read(ARQ_TESTE)
+        log1 = PdoEcoUsihPolin.read(ARQ_TESTE)
+        log2 = PdoEcoUsihPolin.read(ARQ_TESTE)
         log1.tabela.iloc[0, 0] = -1
         assert log1 != log2
```

### Comparing `idessem-0.0.6/tests/dessem/test_pdo_hidr.py` & `idessem-0.0.7/tests/dessem/test_pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_pdo_sist.py` & `idessem-0.0.7/tests/dessem/test_pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_polinjus.py` & `idessem-0.0.7/tests/dessem/test_polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/dessem/test_renovaveis.py` & `idessem-0.0.7/tests/dessem/test_renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/avl_altqueda.py` & `idessem-0.0.7/tests/mocks/arquivos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/avl_fpha1.py` & `idessem-0.0.7/tests/mocks/arquivos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/des_log_relato.py` & `idessem-0.0.7/tests/mocks/arquivos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/dessemarq.py` & `idessem-0.0.7/tests/mocks/arquivos/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/log_matriz.py` & `idessem-0.0.7/tests/mocks/arquivos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/operut.py` & `idessem-0.0.7/tests/mocks/arquivos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/pdo_eco_fcfcortes.py` & `idessem-0.0.7/tests/mocks/arquivos/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih.py` & `idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,83 @@
 MockPdoEcoUsih = [
     "***********************************************************************\n",
     "*                                                                     *\n",
     "*            CEPEL - CENTRO DE PESQUISAS DE ENERGIA ELETRICA          *\n",
+    "*  MODELO DESSEM     - VERSAO 19.4.2 -  Junho  de 2023 (CPLEX)                       *\n",
+    "*                                                                     *\n",
+    "***********************************************************************\n",
+    "\n",
+    "\n",
+    "   PROGRAMA LICENCIADO PARA ONS                                                                                                                                                   \n",
+    "\n",
+    "\n",
+    "____________________________________________________________________\n",
+    "\n",
+    "  TE  PMO - JUNHO/23 - JULHO/23 - REV 2 - FCF COM CVAR - 12 REE - VALOR ESPERADO - Data do Caso: 13/06/2023                                                       \n",
+    "____________________________________________________________________\n",
+    "\n",
+    "-------------------------------------------------------------------\n",
+    "Caracteristicas das usinas hidroeletricas e  topologia das cascatas             \n",
+    "-------------------------------------------------------------------\n",
+    "----------------------------------------------------------------------------------------------\n",
+    "USIH:         Numero de cadastro da usina hidroeletrica                                                                                                                                                 \n",
+    "NomeUsih:     Nome de cadastro da usina hidroeletrica                                                                                                                                                   \n",
+    "NomeSist:     Nome do subsistema                                                                                                                                                                        \n",
+    "UsihJus:      Numero de cadastro da usina hidroeletrica de jusante                                                                                                                                      \n",
+    "UsihDes:      Numero de cadastro da usina hidroeletrica de desvio                                                                                                                                       \n",
+    "UsihJusE:     Numero de cadastro da usina hidroeletrica de jusante para calculo da energia arm                                                                                                          \n",
+    "IperInic:     Indice do periodo inicial de operacao                                                                                                                                                     \n",
+    "VmorInic:     Volume morto Inicial                                                                                                                                                                      \n",
+    "VutilInic:    Volume Util Inicial                                                                                                                                                                       \n",
+    "VarmMin:      Volume Armazenado Minimo                                                                                                                                                                  \n",
+    "VarmMax:      Volume Armazenado Maximo                                                                                                                                                                  \n",
+    "VarmSolVert:  Volume armazenado (total) referente a soleira do vertedouro                                                                                                                               \n",
+    "VutilSolVert: Volume util referente a soleira do vertedouro                                                                                                                                             \n",
+    "VarmSolDesv:  Volume armazenado (total) referente a soleira de desvio                                                                                                                                   \n",
+    "VutilSolDesv: Volume util referente a soleira de desvio                                                                                                                                                 \n",
+    "VarmRef:      Volume Armazenado de Referencia                                                                                                                                                           \n",
+    "TipResv:      Tipo de usina hidroeletrica: (RV: Reservatório; FD: Fio d´agua)                                                                                                                           \n",
+    "TpRegul:      Tipo de Regularizacao:                                                                                                                                                                    \n",
+    "              D: Diaria                                                                                                                                                                                 \n",
+    "              S: Semanal                                                                                                                                                                                \n",
+    "              M: Mensal                                                                                                                                                                                 \n",
+    "FlgEvap:      Flag para consideracao de evaporacao(0: nao; 1: sim)                                                                                                                                      \n",
+    "NCj:          Numero de conjuntos de maquinas                                                                                                                                                           \n",
+    "PdtEsp:       Produtibilidade Especifica                                                                                                                                                                \n",
+    "Tperd:        Tipo de Perda Hidraulica                                                                                                                                                                  \n",
+    "              %: Em % da queda bruta                                                                                                                                                                    \n",
+    "              m: Em metros                                                                                                                                                                              \n",
+    "PerdHid:      Valor da Perda Hidraulica                                                                                                                                                                 \n",
+    "CfugMed:      Cota media do canal de fuga                                                                                                                                                               \n",
+    "Vtfuga:       Flag para indicar se o vertimento influencia na cota do canal de fuga                                                                                                                     \n",
+    "----------------------------------------------------------------------------------------------\n",
+    "\n",
+    "-----;--------------;--------;-------;-------;--------;-----;---------;---------;----------;----------;---------;---------;-----------;------------;-----------;------------;---------;-------;-------;-------;---;---------------;-----;-------;--------;------;\n",
+    "USIH ;   NomeUsih   ;NomeSist;UsihJus;UsihDes;UsihJusE;IperI;VmorInic ;VmorInic ;VutilInic ;VutilInic ; VarmMin ; VarmMax ;VarmSolVert;VutilSolVert;VarmSolDesv;VutilSolDesv; VarmRef ;TipResv;TpRegul;FlgEvap;NCj;    PdtEsp     ;Tperd;PerdHid;CfugMed ;Vtfuga;\n",
+    "  -  ;      -       ;   -    ;   -   ;   -   ;   -    ;  -  ;  (hm3)  ; (%Vmin) ;  (hm3)   ;   (%)    ;  (hm3)  ;  (hm3)  ;   (hm3)   ;    (%)     ;   (hm3)   ;    (%)     ;  (hm3)  ;   -   ;  (-)  ;  (-)  ; - ;(MW/((m3/s).m));  -  ;(tperd);  (m)   ;  -   ;\n",
+    "-----;--------------;--------;-------;-------;--------;-----;---------;---------;----------;----------;---------;---------;-----------;------------;-----------;------------;---------;-------;-------;-------;---;---------------;-----;-------;--------;------;\n",
+    " 001 ; CAMARGOS     ; SE     ;  002  ;   -   ;  002   ; 001 ;    -    ;     -   ;   646.93 ;    96.27 ;   120.00;   792.00;    120.00 ;      0.00  ;    120.00 ;      0.00  ;   792.00;RV     ;   M   ;   1   ; 1 ;    0.008767   ;  m  ;  0.095;  885.73;   1  ;\n",
+    " 002 ; ITUTINGA     ; SE     ;  004  ;   -   ;  004   ; 001 ;    -    ;     -   ;    -     ;     -    ;    11.00;    11.00;     11.00 ;            ;     11.00 ;            ;    10.64;FD     ;   D   ;   1   ; 3 ;    0.008649   ;  m  ;  0.631;  856.85;   1  ;\n",
+    " 004 ; FUNIL-GRANDE ; SE     ;  006  ;   -   ;  006   ; 001 ;    -    ;     -   ;    -     ;     -    ;   304.00;   304.00;    304.00 ;            ;    304.00 ;            ;   265.86;FD     ;   D   ;   1   ; 1 ;    0.009010   ;  m  ;  0.394;  768.13;   1  ;\n",
+    " 006 ; FURNAS       ; SE     ;  007  ;   -   ;  007   ; 001 ;    -    ;     -   ; 17087.87 ;    99.25 ;  5733.00; 22950.00;   6173.76 ;      2.56  ;   5733.00 ;      0.00  ; 22950.00;RV     ;   M   ;   1   ; 2 ;    0.008996   ;  m  ;  0.803;  672.20;   1  ;\n",
+    " 007 ; M. DE MORAES ; SE     ;  008  ;   -   ;  008   ; 001 ;    -    ;     -   ;  2417.25 ;    96.69 ;  1540.00;  4040.00;   1895.00 ;     14.20  ;   1540.00 ;      0.00  ;  4040.00;RV     ;   M   ;   1   ; 4 ;    0.008657   ;  m  ;  1.141;  621.10;   1  ;\n",
+    " 008 ; ESTREITO     ; SE     ;  009  ;   -   ;  009   ; 001 ;    -    ;     -   ;   133.58 ;    74.98 ;  1245.00;  1423.15;   1423.00 ;     99.92  ;   1423.00 ;     99.92  ;  1331.40;RV     ;   D   ;   1   ; 1 ;    0.008890   ;  m  ;  0.899;  558.40;   1  ;\n",
+    " 009 ; JAGUARA      ; SE     ;  010  ;   -   ;  010   ; 001 ;    -    ;     -   ;    59.40 ;    66.00 ;   360.00;   450.00;    450.00 ;    100.00  ;    450.00 ;    100.00  ;   418.20;RV     ;   D   ;   1   ; 1 ;    0.008944   ;  m  ;  0.502;  512.84;   1  ;\n",
+    " 010 ; IGARAPAVA    ; SE     ;  011  ;   -   ;  011   ; 001 ;    -    ;     -   ;    -     ;     -    ;   480.00;   480.00;    480.00 ;            ;    480.00 ;            ;   234.83;FD     ;   D   ;   1   ; 1 ;    0.008996   ;  m  ;  0.170;  494.91;   1  ;\n",
+    " 011 ; VOLTA GRANDE ; SE     ;  012  ;   -   ;  012   ; 001 ;    -    ;     -   ;   230.48 ;    86.00 ;  1976.00;  2244.00;   2244.00 ;    100.00  ;   2244.00 ;    100.00  ;  2200.40;RV     ;   D   ;   1   ; 1 ;    0.008996   ;  m  ;  0.168;  466.63;   1  ;\n",
+    " 012 ; P. COLOMBIA  ; SE     ;  017  ;   -   ;  017   ; 001 ;    -    ;     -   ;   204.62 ;    87.63 ;  1291.00;  1524.50;   1524.00 ;     99.79  ;   1524.00 ;     99.79  ;  1420.84;RV     ;   D   ;   1   ; 1 ;    0.009071   ;  m  ;  0.228;  444.05;   1  ;\n",
+    " 014 ; CACONDE      ; SE     ;  015  ;   -   ;  015   ; 001 ;    -    ;     -   ;   478.20 ;    94.88 ;    51.00;   555.00;    363.98 ;     62.10  ;     51.00 ;      0.00  ;   555.00;RV     ;   M   ;   1   ; 2 ;    0.008558   ;  m  ;  0.869;  751.19;   1  ;\n",
+    " 015 ; E. DA CUNHA  ; SE     ;  016  ;   -   ;  016   ; 001 ;    -    ;     -   ;    -     ;     -    ;    14.00;    14.00;     14.00 ;            ;     14.00 ;            ;    12.79;FD     ;   D   ;   1   ; 1 ;    0.008602   ;  m  ;  0.726;  576.55;   1  ;\n",
+    " 016 ; A.S.OLIVEIRA ; SE     ;  017  ;   -   ;  017   ; 001 ;    -    ;     -   ;    -     ;     -    ;    25.00;    25.00;     25.00 ;            ;     25.00 ;            ;    22.75;FD     ;   D   ;   1   ; 1 ;    0.008599   ;  m  ;  0.186;  546.61;   1  ;\n",
+]
+
+MockPdoEcoUsih190301 = [
+    "***********************************************************************\n",
+    "*                                                                     *\n",
+    "*            CEPEL - CENTRO DE PESQUISAS DE ENERGIA ELETRICA          *\n",
     "*  MODELO DESSEM     - VERSAO 19.3.1 - Fevereiro de 2023 (CPLEX)                     *\n",
     "*                                                                     *\n",
     "***********************************************************************\n",
     "\n",
     "\n",
     "   PROGRAMA LICENCIADO PARA ONS                                                                                                                                                   \n",
     "\n",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idessem-0.0.6/tests/mocks/arquivos/pdo_eco_usih_polin.py` & `idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/pdo_hidr.py` & `idessem-0.0.7/tests/mocks/arquivos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/pdo_oper_uct.py` & `idessem-0.0.7/tests/mocks/arquivos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/pdo_sist.py` & `idessem-0.0.7/tests/mocks/arquivos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/polinjus.py` & `idessem-0.0.7/tests/mocks/arquivos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/arquivos/renovaveis.py` & `idessem-0.0.7/tests/mocks/arquivos/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.6/tests/mocks/mock_open.py` & `idessem-0.0.7/tests/mocks/mock_open.py`

 * *Files identical despite different names*

