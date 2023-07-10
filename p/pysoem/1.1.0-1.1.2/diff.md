# Comparing `tmp/pysoem-1.1.0.tar.gz` & `tmp/pysoem-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoem-1.1.0.tar", last modified: Thu Jul  6 19:14:35 2023, max compression
+gzip compressed data, was "pysoem-1.1.2.tar", last modified: Mon Jul 10 18:33:13 2023, max compression
```

## Comparing `pysoem-1.1.0.tar` & `pysoem-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:14:35.870032 pysoem-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 19:14:24.000000 pysoem-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-06 19:14:24.000000 pysoem-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-06 19:14:35.870032 pysoem-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-06 19:14:24.000000 pysoem-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:14:35.866033 pysoem-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/basic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/find_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/firmware_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/read_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/read_sdo_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-06 19:14:24.000000 pysoem-1.1.0/examples/write_foe.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 19:14:24.000000 pysoem-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:14:35.870032 pysoem-1.1.0/pysoem/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 19:14:24.000000 pysoem-1.1.0/pysoem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-06 19:14:24.000000 pysoem-1.1.0/pysoem/cpysoem.pxd
--rw-r--r--   0 runner    (1001) docker     (123)  1335666 2023-07-06 19:14:35.000000 pysoem-1.1.0/pysoem/pysoem.c
--rw-r--r--   0 runner    (1001) docker     (123)    42367 2023-07-06 19:14:24.000000 pysoem-1.1.0/pysoem/pysoem.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:14:35.870032 pysoem-1.1.0/pysoem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-06 19:14:35.000000 pysoem-1.1.0/pysoem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 19:14:35.000000 pysoem-1.1.0/pysoem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:14:35.000000 pysoem-1.1.0/pysoem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 19:14:35.000000 pysoem-1.1.0/pysoem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:14:35.870032 pysoem-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-06 19:14:24.000000 pysoem-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.753751 pysoem-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 18:32:58.000000 pysoem-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 18:32:58.000000 pysoem-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-10 18:33:13.749751 pysoem-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-10 18:32:58.000000 pysoem-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.733750 pysoem-1.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/basic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/find_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/firmware_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/read_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/read_sdo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-10 18:32:58.000000 pysoem-1.1.2/examples/write_foe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 18:32:58.000000 pysoem-1.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/pysoem/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 18:32:58.000000 pysoem-1.1.2/pysoem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-10 18:32:58.000000 pysoem-1.1.2/pysoem/cpysoem.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)  1335710 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem/pysoem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    42367 2023-07-10 18:32:58.000000 pysoem-1.1.2/pysoem/pysoem.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/pysoem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 18:33:13.000000 pysoem-1.1.2/pysoem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:33:13.753751 pysoem-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-10 18:32:58.000000 pysoem-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/erika/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/erika/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/erika/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/intime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/intime/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/intime/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/linux/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/linux/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/macosx/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/macosx/osal_defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/osal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/rtems/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtems/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtems/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/rtk/
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtk/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/rtk/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/vxworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/vxworks/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/vxworks/osal_defs.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/osal/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/inttypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/osal.c
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/osal_defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/osal_win32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/osal/win32/stdint.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/oshw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/erika/
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/erika/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/intime/
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/intime/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/linux/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/macosx/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtems/
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtems/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtk/fec/
+-rw-r--r--   0 runner    (1001) docker     (123)    25509 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/fec/fec_ecat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/fec/fec_ecat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.741751 pysoem-1.1.2/soem/oshw/rtk/lw_mac/
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/lw_mac/lw_emac.c
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/lw_mac/lw_emac.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19522 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/rtk/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/vxworks/
+-rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/vxworks/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/nicdrv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/nicdrv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/oshw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/oshw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/oshw/win32/wpcap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/Packet32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/Win32-Extensions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/bittypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/ip6_misc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.745751 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/bluetooth.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/bpf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/namedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/pcap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/sll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/usb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap/vlan.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-bpf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-namedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap-stdinc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/pcap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/oshw/win32/wpcap/Include/remote-ext.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/soem/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatbase.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56267 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatcoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatcoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatconfig.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatconfig.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatconfiglist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatdc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatdc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercateoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercateoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatfoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatfoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    75008 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatmain.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatmain.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatprint.c
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatprint.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatsoe.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercatsoe.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/soem/ethercattype.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/test/intime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/intime/ec_master/
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/intime/ec_master/ec_master.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/aliastool.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/ebox/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/ebox/ebox.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/eepromtool/
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/eepromtool/eepromtool.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/eoe_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/eoe_test/eoe_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/firm_update/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/firm_update/firm_update.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/red_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/red_test/red_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/simple_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/simple_test/simple_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/linux/slaveinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/linux/slaveinfo/slaveinfo.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/rtk/
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/rtk/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.729750 pysoem-1.1.2/soem/test/win32/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/ebox/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/ebox/ebox.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/eepromtool/
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/eepromtool/eepromtool.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/firm_update/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/firm_update/firm_update.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/red_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/red_test/red_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/simple_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/simple_test/simple_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:33:13.749751 pysoem-1.1.2/soem/test/win32/slaveinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)    22856 2023-07-10 18:33:00.000000 pysoem-1.1.2/soem/test/win32/slaveinfo/slaveinfo.c
```

### Comparing `pysoem-1.1.0/LICENSE` & `pysoem-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/PKG-INFO` & `pysoem-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoem
-Version: 1.1.0
+Version: 1.1.2
 Summary: Cython wrapper for the SOEM Library
 Home-page: https://github.com/bnjmnp/pysoem
 Author: Benjamin Partzsch
 Author-email: benjamin_partzsch@web.de
 License: MIT
 Project-URL: Documentation, https://pysoem.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pysoem-1.1.0/README.rst` & `pysoem-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/examples/basic_example.py` & `pysoem-1.1.2/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/examples/firmware_update.py` & `pysoem-1.1.2/examples/firmware_update.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/examples/minimal_example.py` & `pysoem-1.1.2/examples/minimal_example.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/examples/read_eeprom.py` & `pysoem-1.1.2/examples/read_eeprom.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/examples/read_sdo_info.py` & `pysoem-1.1.2/examples/read_sdo_info.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/examples/write_foe.py` & `pysoem-1.1.2/examples/write_foe.py`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/pysoem/cpysoem.pxd` & `pysoem-1.1.2/pysoem/cpysoem.pxd`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/pysoem/pysoem.c` & `pysoem-1.1.2/pysoem/pysoem.c`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,17 @@
     "distutils": {
         "define_macros": [
             [
                 "EC_VER2",
                 ""
             ]
         ],
-        "depends": [],
+        "depends": [
+            "soem/soem/ethercat.h"
+        ],
         "include_dirs": [
             "./pysoem",
             "./soem/oshw/linux",
             "./soem/osal/linux",
             "./soem/oshw",
             "./soem/osal",
             "./soem/soem"
```

### Comparing `pysoem-1.1.0/pysoem/pysoem.pyx` & `pysoem-1.1.2/pysoem/pysoem.pyx`

 * *Files identical despite different names*

### Comparing `pysoem-1.1.0/pysoem.egg-info/PKG-INFO` & `pysoem-1.1.2/pysoem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoem
-Version: 1.1.0
+Version: 1.1.2
 Summary: Cython wrapper for the SOEM Library
 Home-page: https://github.com/bnjmnp/pysoem
 Author: Benjamin Partzsch
 Author-email: benjamin_partzsch@web.de
 License: MIT
 Project-URL: Documentation, https://pysoem.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pysoem-1.1.0/setup.py` & `pysoem-1.1.2/setup.py`

 * *Files identical despite different names*

