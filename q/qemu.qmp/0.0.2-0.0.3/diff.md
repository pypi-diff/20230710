# Comparing `tmp/qemu.qmp-0.0.2.tar.gz` & `tmp/qemu.qmp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qemu.qmp-0.0.2.tar", last modified: Tue Sep  6 14:32:45 2022, max compression
+gzip compressed data, was "qemu.qmp-0.0.3.tar", last modified: Mon Jul 10 17:50:12 2023, max compression
```

## Comparing `qemu.qmp-0.0.2.tar` & `qemu.qmp-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.940705 qemu.qmp-0.0.2/
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     2845 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/FILES.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    25381 2022-04-29 17:23:17.000000 qemu.qmp-0.0.2/LICENSE
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    17992 2022-04-29 17:23:17.000000 qemu.qmp-0.0.2/LICENSE_GPL2
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      217 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/MANIFEST.in
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     4191 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/Makefile
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     9692 2022-09-06 14:32:45.940705 qemu.qmp-0.0.2/PKG-INFO
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     8111 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/README.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      530 2022-07-15 22:10:44.000000 qemu.qmp-0.0.2/avocado.cfg
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.937705 qemu.qmp-0.0.2/docs/
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      634 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/Makefile
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     8576 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/docs/conf.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      762 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/docs/index.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      125 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/main.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      760 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/make.bat
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.937705 qemu.qmp-0.0.2/docs/man/
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      266 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/docs/man/qmp_shell.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      397 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/docs/man/qmp_shell_wrap.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     2017 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/overview.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      141 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.error.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      101 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.events.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      109 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.legacy.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      289 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.message.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      171 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.protocol.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      144 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.qmp_client.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      132 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/docs/qemu.qmp.util.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      109 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/docs/qmp_shell.rst
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      137 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/docs/qmp_shell_wrap.rst
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.937705 qemu.qmp-0.0.2/qemu/
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      301 2022-04-29 17:23:17.000000 qemu.qmp-0.0.2/qemu/README.rst
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.939705 qemu.qmp-0.0.2/qemu/qmp/
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1627 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/qemu/qmp/__init__.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1788 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/qemu/qmp/error.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    23757 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/qemu/qmp/events.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     9845 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/qemu/qmp/legacy.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     6495 2022-08-18 21:31:46.000000 qemu.qmp-0.0.2/qemu/qmp/message.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     4578 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/qemu/qmp/models.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    39331 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/qemu/qmp/protocol.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)        0 2022-04-29 17:23:17.000000 qemu.qmp-0.0.2/qemu/qmp/py.typed
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    25124 2022-08-18 21:31:46.000000 qemu.qmp-0.0.2/qemu/qmp/qmp_client.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    22076 2022-09-01 15:25:37.000000 qemu.qmp-0.0.2/qemu/qmp/qmp_shell.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    22411 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/qemu/qmp/qmp_tui.py
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     6365 2022-08-18 20:53:26.000000 qemu.qmp-0.0.2/qemu/qmp/util.py
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.938705 qemu.qmp-0.0.2/qemu.qmp.egg-info/
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     9692 2022-09-06 14:32:45.000000 qemu.qmp-0.0.2/qemu.qmp.egg-info/PKG-INFO
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      998 2022-09-06 14:32:45.000000 qemu.qmp-0.0.2/qemu.qmp.egg-info/SOURCES.txt
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)        1 2022-09-06 14:32:45.000000 qemu.qmp-0.0.2/qemu.qmp.egg-info/dependency_links.txt
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      138 2022-09-06 14:32:45.000000 qemu.qmp-0.0.2/qemu.qmp.egg-info/entry_points.txt
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)      221 2022-09-06 14:32:45.000000 qemu.qmp-0.0.2/qemu.qmp.egg-info/requires.txt
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)        5 2022-09-06 14:32:45.000000 qemu.qmp-0.0.2/qemu.qmp.egg-info/top_level.txt
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     3366 2022-09-06 14:32:45.941705 qemu.qmp-0.0.2/setup.cfg
--rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)     1197 2022-08-18 20:53:58.000000 qemu.qmp-0.0.2/setup.py
-drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2022-09-06 14:32:45.940705 qemu.qmp-0.0.2/tests/
--rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       37 2022-04-29 17:23:17.000000 qemu.qmp-0.0.2/tests/flake8.sh
--rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       39 2022-04-29 17:23:17.000000 qemu.qmp-0.0.2/tests/isort.sh
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1132 2022-08-18 20:54:58.000000 qemu.qmp-0.0.2/tests/minreqs.txt
--rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       37 2022-07-14 00:48:49.000000 qemu.qmp-0.0.2/tests/mypy.sh
--rw-r--r--   0 jsnow    (21266) jsnow    (21266)    18678 2022-08-11 00:31:31.000000 qemu.qmp-0.0.2/tests/protocol.py
--rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)      126 2022-08-10 21:46:09.000000 qemu.qmp-0.0.2/tests/pylint.sh
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.651737 qemu.qmp-0.0.3/
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     3164 2023-06-26 13:31:04.000000 qemu.qmp-0.0.3/FILES.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    25381 2022-04-29 17:23:17.000000 qemu.qmp-0.0.3/LICENSE
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    17992 2022-04-29 17:23:17.000000 qemu.qmp-0.0.3/LICENSE_GPL2
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      217 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/MANIFEST.in
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     4426 2023-07-06 21:43:22.000000 qemu.qmp-0.0.3/Makefile
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    11012 2023-07-10 17:50:12.651737 qemu.qmp-0.0.3/PKG-INFO
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     9430 2023-07-10 17:47:04.000000 qemu.qmp-0.0.3/README.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      530 2022-07-15 22:10:44.000000 qemu.qmp-0.0.3/avocado.cfg
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.648737 qemu.qmp-0.0.3/docs/
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      634 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/Makefile
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     8576 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/docs/conf.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      762 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/docs/index.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      125 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/main.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      760 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/make.bat
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.648737 qemu.qmp-0.0.3/docs/man/
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      266 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/docs/man/qmp_shell.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      397 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/docs/man/qmp_shell_wrap.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     2017 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/overview.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      141 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.error.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      101 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.events.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      109 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.legacy.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      289 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.message.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      171 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.protocol.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      144 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.qmp_client.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      132 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/docs/qemu.qmp.util.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      109 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/docs/qmp_shell.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      137 2022-09-01 15:25:37.000000 qemu.qmp-0.0.3/docs/qmp_shell_wrap.rst
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      152 2023-07-07 20:04:30.000000 qemu.qmp-0.0.3/pyproject.toml
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.648737 qemu.qmp-0.0.3/qemu/
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      301 2022-04-29 17:23:17.000000 qemu.qmp-0.0.3/qemu/README.rst
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.650737 qemu.qmp-0.0.3/qemu/qmp/
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1627 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/qemu/qmp/__init__.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1788 2022-08-18 20:54:58.000000 qemu.qmp-0.0.3/qemu/qmp/error.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    23757 2022-08-18 20:54:58.000000 qemu.qmp-0.0.3/qemu/qmp/events.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    10223 2023-06-21 21:13:17.000000 qemu.qmp-0.0.3/qemu/qmp/legacy.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     6495 2022-08-18 21:31:46.000000 qemu.qmp-0.0.3/qemu/qmp/message.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     4578 2022-08-18 20:53:26.000000 qemu.qmp-0.0.3/qemu/qmp/models.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    39771 2023-06-21 19:09:13.000000 qemu.qmp-0.0.3/qemu/qmp/protocol.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)        0 2022-04-29 17:23:17.000000 qemu.qmp-0.0.3/qemu/qmp/py.typed
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    25114 2023-06-06 17:00:14.000000 qemu.qmp-0.0.3/qemu/qmp/qmp_client.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    22063 2023-07-10 17:47:04.000000 qemu.qmp-0.0.3/qemu/qmp/qmp_shell.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    22579 2023-07-06 21:43:22.000000 qemu.qmp-0.0.3/qemu/qmp/qmp_tui.py
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     3720 2023-06-21 18:38:25.000000 qemu.qmp-0.0.3/qemu/qmp/util.py
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.649737 qemu.qmp-0.0.3/qemu.qmp.egg-info/
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    11012 2023-07-10 17:50:12.000000 qemu.qmp-0.0.3/qemu.qmp.egg-info/PKG-INFO
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1004 2023-07-10 17:50:12.000000 qemu.qmp-0.0.3/qemu.qmp.egg-info/SOURCES.txt
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)        1 2023-07-10 17:50:12.000000 qemu.qmp-0.0.3/qemu.qmp.egg-info/dependency_links.txt
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      138 2023-07-10 17:50:12.000000 qemu.qmp-0.0.3/qemu.qmp.egg-info/entry_points.txt
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)      275 2023-07-10 17:50:12.000000 qemu.qmp-0.0.3/qemu.qmp.egg-info/requires.txt
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)        5 2023-07-10 17:50:12.000000 qemu.qmp-0.0.3/qemu.qmp.egg-info/top_level.txt
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     3383 2023-07-10 17:50:12.652737 qemu.qmp-0.0.3/setup.cfg
+drwxr-xr-x   0 jsnow    (21266) jsnow    (21266)        0 2023-07-10 17:50:12.651737 qemu.qmp-0.0.3/tests/
+-rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       37 2022-04-29 17:23:17.000000 qemu.qmp-0.0.3/tests/flake8.sh
+-rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       39 2022-04-29 17:23:17.000000 qemu.qmp-0.0.3/tests/isort.sh
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)     1117 2023-07-06 21:43:22.000000 qemu.qmp-0.0.3/tests/minreqs.txt
+-rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       37 2022-07-14 00:48:49.000000 qemu.qmp-0.0.3/tests/mypy.sh
+-rw-r--r--   0 jsnow    (21266) jsnow    (21266)    18668 2023-06-21 18:38:25.000000 qemu.qmp-0.0.3/tests/protocol.py
+-rwxr-xr-x   0 jsnow    (21266) jsnow    (21266)       37 2023-06-26 13:31:04.000000 qemu.qmp-0.0.3/tests/pylint.sh
```

### Comparing `qemu.qmp-0.0.2/FILES.rst` & `qemu.qmp-0.0.3/FILES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,38 @@
 used. It's useful info for those contributing to this project, but not
 so much for those who just want to use the library.
 
 
 Much ado about packaging
 ------------------------
 
-``setup.py`` is used by ``pip`` to install this tooling to the current
-environment. ``setup.cfg`` provides the packaging configuration used by
-``setup.py``. You will generally invoke it by doing one of the following:
+``pyproject.toml`` defines the build backend and build dependencies.
+This project uses the ``setuptools.build_meta`` build backend.
+The backend reads the packaging configuration from ``setup.cfg``.
+Other than ``setuptools``, this package requires ``setuptools_scm`` at
+buildtime to determine the package version based on git metadata.
 
 1. ``pip3 install .`` will install these packages to your current
    environment. If you are inside a virtual environment, they will
    install there. If you are not, it will attempt to install to the
    global environment, which is **not recommended**.
 
 2. ``pip3 install --user .`` will install these packages to your user's
    local python packages. If you are inside of a virtual environment,
    this will fail; you want the first invocation above.
 
 If you append the ``--editable`` or ``-e`` argument to either invocation
 above, pip will install in "editable" mode. This installs the package as
-a forwarder ("qemu.qmp.egg-link") that points to the source tree. In so
+a forwarder that points to the source tree. In so
 doing, the installed package always reflects the latest version in your
 source tree.
+This feature requires pip 21.3 or newer.
+See `Development Mode (a.k.a. “Editable Installs”)
+<https://setuptools.pypa.io/en/latest/userguide/development_mode.html>`_
+in the Setuptools documentation for more information.
 
 Installing ".[devel]" instead of "." will additionally pull in required
 packages for testing this package. They are not runtime requirements,
 and are not needed to simply use these libraries.
 
 Running ``make develop`` will pull in all testing dependencies and
 install QEMU in editable mode to the current environment.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qemu.qmp-0.0.2/LICENSE` & `qemu.qmp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/LICENSE_GPL2` & `qemu.qmp-0.0.3/LICENSE_GPL2`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/Makefile` & `qemu.qmp-0.0.3/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 .PHONY: help
 help:
 	@echo "python packaging help:"
 	@echo ""
 	@echo "make check-minreqs:"
 	@echo "    Run tests in the minreqs virtual environment."
 	@echo "    These tests use the oldest dependencies."
-	@echo "    Requires: Python 3.6"
-	@echo "    Hint (Fedora): 'sudo dnf install python3.6'"
+	@echo "    Requires: Python 3.7"
+	@echo "    Hint (Fedora): 'sudo dnf install python3.7'"
 	@echo ""
 	@echo "make check-tox:"
 	@echo "    Run tests against multiple python versions."
 	@echo "    These tests use the newest dependencies."
-	@echo "    Requires: Python 3.6 - 3.10, and tox."
-	@echo "    Hint (Fedora): 'sudo dnf install python3-tox python3.10'"
+	@echo "    Requires: Python 3.7 - 3.12, and tox."
+	@echo "    Hint (Fedora): 'sudo dnf install python3-tox python3.12'"
 	@echo "    The variable QEMU_TOX_EXTRA_ARGS can be use to pass extra"
 	@echo "    arguments to tox".
 	@echo ""
 	@echo "make check-dev:"
 	@echo "    Run tests in a venv against your default python3 version."
 	@echo "    These tests use the newest dependencies."
 	@echo "    Requires: Python 3.x"
 	@echo ""
 	@echo "make check:"
 	@echo "    Run tests in your *current environment*."
 	@echo "    Performs no environment setup of any kind."
 	@echo ""
 	@echo "make develop:"
-	@echo "    Install deps needed for for 'make check',"
+	@echo "    Install deps needed for 'make check',"
 	@echo "    and install the qemu.qmp package in editable mode."
 	@echo "    (Can be used in or outside of a venv.)"
 	@echo ""
 	@echo "make min-venv"
 	@echo "    Creates the minreqs virtual environment ($(QEMU_MINVENV_DIR))"
 	@echo ""
 	@echo "make dev-venv"
@@ -50,26 +50,31 @@
 	@echo -e "Have a nice day ^_^\n"
 
 .PHONY: pipenv check-pipenv
 pipenv check-pipenv:
 	@echo "pipenv was dropped; try 'make check-minreqs' or 'make min-venv'"
 	@exit 1
 
+PIP_INSTALL = pip install --disable-pip-version-check
 .PHONY: min-venv
 min-venv: $(QEMU_MINVENV_DIR) $(QEMU_MINVENV_DIR)/bin/activate
 $(QEMU_MINVENV_DIR) $(QEMU_MINVENV_DIR)/bin/activate: setup.cfg tests/minreqs.txt
 	@echo "VENV $(QEMU_MINVENV_DIR)"
-	@python3.6 -m venv $(QEMU_MINVENV_DIR)
+	@python3.7 -m venv $(QEMU_MINVENV_DIR)
 	@(								\
 		echo "ACTIVATE $(QEMU_MINVENV_DIR)";			\
 		. $(QEMU_MINVENV_DIR)/bin/activate;			\
+		echo "Ensure pip supports editable installs"; 		\
+		$(PIP_INSTALL) 'pip>=21.3';				\
+		echo "INSTALL wheel $(QEMU_MINVENV_DIR)";               \
+		$(PIP_INSTALL) wheel 1>/dev/null;		               \
 		echo "INSTALL -r tests/minreqs.txt $(QEMU_MINVENV_DIR)";\
-		pip install -r tests/minreqs.txt 1>/dev/null;		\
-		echo "INSTALL -e qemu.qmp $(QEMU_MINVENV_DIR)";		\
-		pip install -e . 1>/dev/null;				\
+		$(PIP_INSTALL) -r tests/minreqs.txt 1>/dev/null;	\
+		echo "INSTALL -e qemu $(QEMU_MINVENV_DIR)";		\
+		$(PIP_INSTALL) -e . --config-settings=editable_mode=compat 1>/dev/null;			\
 	)
 	@touch $(QEMU_MINVENV_DIR)
 
 .PHONY: check-minreqs
 check-minreqs: min-venv
 	@(							\
 		echo "ACTIVATE $(QEMU_MINVENV_DIR)";		\
@@ -96,15 +101,15 @@
 		echo "ACTIVATE $(QEMU_VENV_DIR)";		\
 		. $(QEMU_VENV_DIR)/bin/activate;		\
 		make check;					\
 	)
 
 .PHONY: develop
 develop:
-	pip3 install --disable-pip-version-check -e .[devel]
+	$(PIP_INSTALL) -e .[devel] --config-settings=editable_mode=compat
 
 .PHONY: check
 check:
 	@avocado --config avocado.cfg run tests/
 
 .PHONY: check-tox
 check-tox:
@@ -116,34 +121,32 @@
 	@coverage combine
 	@coverage html
 	@coverage xml
 	@coverage report
 
 .PHONY: clean
 clean:
-	python3 setup.py clean --all
-	rm -f pyproject.toml
 	make -C docs clean
 
 .PHONY: distclean
 distclean: clean
-	rm -rf qemu.qmp.egg-info/ .eggs/ dist/
+	rm -rf qemu.qmp.egg-info/ dist/
 	rm -rf $(QEMU_VENV_DIR) $(QEMU_MINVENV_DIR) .tox/
 	rm -f .coverage coverage.xml .coverage.*
 	rm -rf htmlcov/ test-results/
 
 .PHONY: docs
 docs:
 	make -C docs html
 
 .PHONY: tag
 tag:
 	python3 scripts/package.py tag
 
-dist: setup.py setup.cfg MANIFEST.in README.rst scripts/package.py
+dist: setup.cfg MANIFEST.in README.rst scripts/package.py
 	python3 scripts/package.py build
 
 .PHONY: test-publish
 test-publish:
 	python3 scripts/package.py publish --test
 
 .PHONY: publish
```

### Comparing `qemu.qmp-0.0.2/PKG-INFO` & `qemu.qmp-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu.qmp
-Version: 0.0.2
+Version: 0.0.3
 Summary: QEMU Monitor Protocol library
 Home-page: https://gitlab.com/qemu-project/python-qemu-qmp
 Author: QEMU Project
 Author-email: qemu-devel@nongnu.org
 Maintainer: John Snow
 Maintainer-email: jsnow@redhat.com
 Project-URL: Homepage, https://www.qemu.org/
@@ -15,38 +15,38 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Emulators
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 Provides-Extra: tui
 License-File: LICENSE
 License-File: LICENSE_GPL2
 
 qemu.qmp: QEMU Monitor Protocol Library
 =======================================
 
 Welcome! ``qemu.qmp`` is a `QEMU Monitor Protocol
 <https://gitlab.com/qemu-project/qemu/-/blob/master/docs/interop/qmp-intro.txt>`_
 (“QMP”) library written in Python, using `asyncio
 <https://docs.python.org/3/library/asyncio.html>`_. It is used to send
 QMP messages to running `QEMU <https://www.qemu.org/>`_ emulators. It
-requires Python 3.6+ and has no mandatory dependencies.
+requires Python 3.7+ and has no mandatory dependencies.
 
 This library can be used to communicate with QEMU emulators, the `QEMU
 Guest Agent
 <https://qemu.readthedocs.io/en/latest/interop/qemu-ga.html>`_ (QGA),
 the `QEMU Storage Daemon
 <https://qemu.readthedocs.io/en/latest/tools/qemu-storage-daemon.html>`_
 (QSD), or any other utility or application that `speaks QMP
@@ -216,14 +216,40 @@
 will always be bugfixes, and minor updates will be reserved for
 backwards compatible feature changes.
 
 
 Changelog
 ---------
 
+0.0.3 (2023-07-10)
+^^^^^^^^^^^^^^^^^^
+
+This release addresses packaging issues associated with the forthcoming
+release of Python 3.12. This release adds Python 3.12 support, drops
+Python 3.6 support, and switches to PEP-517 native packaging.
+
+- `!25 <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/25>`_:
+  Drop Python 3.6 support
+- `#30 <https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/30>`_:
+  The read buffer limit has been increased from 256KiB to 10MiB for
+  parity with libvirt's default and to accommodate real-world replies
+  that may exceed the current limit.
+- `#29 <https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/29>`_:
+  The connect() call now accepts existing sockets as an 'address',
+  allowing for easier use of socketpairs to create client/server pairs.
+  This functionality was revised in `!22
+  <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/22>`_.
+- `!23 <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/23>`_:
+  Fix deadlock on disconnect under CPython 3.12.
+  See also `<https://github.com/python/cpython/issues/104344>`_.
+- `!24
+  <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/24>`_:
+  Switch to PEP517 native packaging to coincide with Python 3.12
+  dropping distutils, setuptools from ensurepip, etc.
+
 0.0.2 (2022-08-26)
 ^^^^^^^^^^^^^^^^^^
 
 This release primarily fixes development tooling, documentation, and
 packaging issues that have no impact on the library itself. A handful of
 small, runtime visible changes were added as polish.
```

### Comparing `qemu.qmp-0.0.2/README.rst` & `qemu.qmp-0.0.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 =======================================
 
 Welcome! ``qemu.qmp`` is a `QEMU Monitor Protocol
 <https://gitlab.com/qemu-project/qemu/-/blob/master/docs/interop/qmp-intro.txt>`_
 (“QMP”) library written in Python, using `asyncio
 <https://docs.python.org/3/library/asyncio.html>`_. It is used to send
 QMP messages to running `QEMU <https://www.qemu.org/>`_ emulators. It
-requires Python 3.6+ and has no mandatory dependencies.
+requires Python 3.7+ and has no mandatory dependencies.
 
 This library can be used to communicate with QEMU emulators, the `QEMU
 Guest Agent
 <https://qemu.readthedocs.io/en/latest/interop/qemu-ga.html>`_ (QGA),
 the `QEMU Storage Daemon
 <https://qemu.readthedocs.io/en/latest/tools/qemu-storage-daemon.html>`_
 (QSD), or any other utility or application that `speaks QMP
@@ -180,14 +180,40 @@
 will always be bugfixes, and minor updates will be reserved for
 backwards compatible feature changes.
 
 
 Changelog
 ---------
 
+0.0.3 (2023-07-10)
+^^^^^^^^^^^^^^^^^^
+
+This release addresses packaging issues associated with the forthcoming
+release of Python 3.12. This release adds Python 3.12 support, drops
+Python 3.6 support, and switches to PEP-517 native packaging.
+
+- `!25 <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/25>`_:
+  Drop Python 3.6 support
+- `#30 <https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/30>`_:
+  The read buffer limit has been increased from 256KiB to 10MiB for
+  parity with libvirt's default and to accommodate real-world replies
+  that may exceed the current limit.
+- `#29 <https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/29>`_:
+  The connect() call now accepts existing sockets as an 'address',
+  allowing for easier use of socketpairs to create client/server pairs.
+  This functionality was revised in `!22
+  <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/22>`_.
+- `!23 <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/23>`_:
+  Fix deadlock on disconnect under CPython 3.12.
+  See also `<https://github.com/python/cpython/issues/104344>`_.
+- `!24
+  <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/24>`_:
+  Switch to PEP517 native packaging to coincide with Python 3.12
+  dropping distutils, setuptools from ensurepip, etc.
+
 0.0.2 (2022-08-26)
 ^^^^^^^^^^^^^^^^^^
 
 This release primarily fixes development tooling, documentation, and
 packaging issues that have no impact on the library itself. A handful of
 small, runtime visible changes were added as polish.
```

### Comparing `qemu.qmp-0.0.2/avocado.cfg` & `qemu.qmp-0.0.3/avocado.cfg`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/docs/Makefile` & `qemu.qmp-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/docs/conf.py` & `qemu.qmp-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/docs/index.rst` & `qemu.qmp-0.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/docs/make.bat` & `qemu.qmp-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/docs/overview.rst` & `qemu.qmp-0.0.3/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/qemu/qmp/__init__.py` & `qemu.qmp-0.0.3/qemu/qmp/__init__.py`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/qemu/qmp/error.py` & `qemu.qmp-0.0.3/qemu/qmp/error.py`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/qemu/qmp/events.py` & `qemu.qmp-0.0.3/qemu/qmp/events.py`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/qemu/qmp/legacy.py` & `qemu.qmp-0.0.3/qemu/qmp/legacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  John Snow <jsnow@redhat.com>
 #
 # This work is licensed under the terms of the GNU GPL, version 2.  See
 # the LICENSE_GPL2 file in the top-level directory.
 #
 
 import asyncio
+import socket
 from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Dict,
     List,
     Optional,
@@ -63,31 +64,38 @@
 
 
 class QEMUMonitorProtocol:
     """
     Provide an API to connect to QEMU via QEMU Monitor Protocol (QMP)
     and then allow to handle commands and events.
 
-    :param address:  QEMU address, can be either a unix socket path (string)
-                     or a tuple in the form ( address, port ) for a TCP
-                     connection
+    :param address:  QEMU address, can be a unix socket path (string), a tuple
+                     in the form ( address, port ) for a TCP connection, or an
+                     existing `socket.socket` object.
     :param server:   Act as the socket server. (See 'accept')
+                     Not applicable when passing a socket directly.
     :param nickname: Optional nickname used for logging.
     """
 
-    def __init__(self, address: SocketAddrT,
+    def __init__(self,
+                 address: Union[SocketAddrT, socket.socket],
                  server: bool = False,
                  nickname: Optional[str] = None):
 
+        if server and isinstance(address, socket.socket):
+            raise ValueError(
+                "server argument should be False when passing a socket")
+
         self._qmp = QMPClient(nickname)
         self._aloop = asyncio.get_event_loop()
         self._address = address
         self._timeout: Optional[float] = None
 
         if server:
+            assert not isinstance(self._address, socket.socket)
             self._sync(self._qmp.start_server(self._address))
 
     _T = TypeVar('_T')
 
     def _sync(
             self, future: Awaitable[_T], timeout: Optional[float] = None
     ) -> _T:
```

### Comparing `qemu.qmp-0.0.2/qemu/qmp/message.py` & `qemu.qmp-0.0.3/qemu/qmp/message.py`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/qemu/qmp/models.py` & `qemu.qmp-0.0.3/qemu/qmp/models.py`

 * *Files identical despite different names*

### Comparing `qemu.qmp-0.0.2/qemu/qmp/protocol.py` & `qemu.qmp-0.0.3/qemu/qmp/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 """
 
 # It's all the docstrings ... ! It's long for a good reason ^_^;
 # pylint: disable=too-many-lines
 
 import asyncio
 from asyncio import StreamReader, StreamWriter
+from contextlib import asynccontextmanager
 from enum import Enum
 from functools import wraps
 from inspect import iscoroutinefunction
 import logging
+import socket
 from ssl import SSLContext
 from typing import (
     Any,
+    AsyncGenerator,
     Awaitable,
     Callable,
     Generic,
     List,
     Optional,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 from .error import QMPError
 from .util import (
     bottom_half,
-    create_task,
     exception_summary,
     flush,
-    is_closing,
     pretty_traceback,
     upper_half,
-    wait_closed,
 )
 
 
 T = TypeVar('T')
 _U = TypeVar('_U')
 _TaskFN = Callable[[], Awaitable[None]]  # aka ``async def func() -> None``
 
@@ -222,15 +222,15 @@
     """
     # pylint: disable=too-many-instance-attributes
 
     #: Logger object for debugging messages from this connection.
     logger = logging.getLogger(__name__)
 
     # Maximum allowable size of read buffer
-    _limit = (64 * 1024)
+    _limit = 64 * 1024
 
     # -------------------------
     # Section: Public interface
     # -------------------------
 
     def __init__(self, name: Optional[str] = None) -> None:
         self._name: Optional[str]
@@ -353,17 +353,16 @@
         :raise StateError: When the `Runstate` is not `IDLE`.
         :raise ConnectError:
             When the server could not start listening on this address.
 
             This exception will wrap a more concrete one. In most cases,
             the wrapped exception will be `OSError`.
         """
-        await self._session_guard(
-            self._do_start_server(address, ssl),
-            'Failed to establish connection')
+        async with self._session_guard('Failed to establish connection'):
+            await self._do_start_server(address, ssl)
         assert self.runstate == Runstate.CONNECTING
 
     @upper_half
     @require(Runstate.CONNECTING)
     async def accept(self) -> None:
         """
         Accept an incoming connection and begin processing message queues.
@@ -380,25 +379,23 @@
             This exception will wrap a more concrete one. In most cases,
             the wrapped exception will be `OSError` or `EOFError`. If a
             protocol-level failure occurs while establishing a new
             session, the wrapped error may also be an `QMPError`.
         """
         if self._accepted is None:
             raise QMPError("Cannot call accept() before start_server().")
-        await self._session_guard(
-            self._do_accept(),
-            'Failed to establish connection')
-        await self._session_guard(
-            self._establish_session(),
-            'Failed to establish session')
+        async with self._session_guard('Failed to establish connection'):
+            await self._do_accept()
+        async with self._session_guard('Failed to establish session'):
+            await self._establish_session()
         assert self.runstate == Runstate.RUNNING
 
     @upper_half
     @require(Runstate.IDLE)
-    async def connect(self, address: SocketAddrT,
+    async def connect(self, address: Union[SocketAddrT, socket.socket],
                       ssl: Optional[SSLContext] = None) -> None:
         """
         Connect to the server and begin processing message queues.
 
         If this call fails, `runstate` is guaranteed to be set back to `IDLE`.
 
         :param address:
@@ -410,20 +407,18 @@
             When a connection or session cannot be established.
 
             This exception will wrap a more concrete one. In most cases,
             the wrapped exception will be `OSError` or `EOFError`. If a
             protocol-level failure occurs while establishing a new
             session, the wrapped error may also be an `QMPError`.
         """
-        await self._session_guard(
-            self._do_connect(address, ssl),
-            'Failed to establish connection')
-        await self._session_guard(
-            self._establish_session(),
-            'Failed to establish session')
+        async with self._session_guard('Failed to establish connection'):
+            await self._do_connect(address, ssl)
+        async with self._session_guard('Failed to establish session'):
+            await self._establish_session()
         assert self.runstate == Runstate.RUNNING
 
     @upper_half
     async def disconnect(self) -> None:
         """
         Disconnect and wait for all tasks to fully stop.
 
@@ -440,15 +435,16 @@
         self._schedule_disconnect()
         await self._wait_disconnect()
 
     # --------------------------
     # Section: Session machinery
     # --------------------------
 
-    async def _session_guard(self, coro: Awaitable[None], emsg: str) -> None:
+    @asynccontextmanager
+    async def _session_guard(self, emsg: str) -> AsyncGenerator[None, None]:
         """
         Async guard function used to roll back to `IDLE` on any error.
 
         On any Exception, the state machine will be reset back to
         `IDLE`. Most Exceptions will be wrapped with `ConnectError`, but
         `BaseException` events will be left alone (This includes
         asyncio.CancelledError, even prior to Python 3.8).
@@ -457,18 +453,17 @@
             Human-readable string describing what connection phase failed.
 
         :raise BaseException:
             When `BaseException` occurs in the guarded block.
         :raise ConnectError:
             When any other error is encountered in the guarded block.
         """
-        # Note: After Python 3.6 support is removed, this should be an
-        # @asynccontextmanager instead of accepting a callback.
         try:
-            await coro
+            # Caller's code runs here.
+            yield
         except BaseException as err:
             self.logger.error("%s: %s", emsg, exception_summary(err))
             self.logger.debug("%s:\n%s\n", emsg, pretty_traceback())
             try:
                 # Reset the runstate back to IDLE.
                 await self.disconnect()
             except:
@@ -533,15 +528,14 @@
         """
         if self._server is None:
             return
 
         try:
             self.logger.debug("Stopping server.")
             self._server.close()
-            await self._server.wait_closed()
             self.logger.debug("Server stopped.")
         finally:
             self._server = None
 
     @bottom_half  # However, it does not run from the R/W tasks.
     async def _incoming(self,
                         reader: asyncio.StreamReader,
@@ -639,15 +633,15 @@
         await self._accepted.wait()
         assert self._server is None
         self._accepted = None
 
         self.logger.debug("Connection accepted.")
 
     @upper_half
-    async def _do_connect(self, address: SocketAddrT,
+    async def _do_connect(self, address: Union[SocketAddrT, socket.socket],
                           ssl: Optional[SSLContext] = None) -> None:
         """
         Acting as the transport client, initiate a connection to a server.
 
         :param address:
             Address to connect to; UNIX socket path or TCP address/port.
         :param ssl: SSL context to use, if any.
@@ -658,31 +652,40 @@
         self._set_state(Runstate.CONNECTING)
 
         # Allow runstate watchers to witness 'CONNECTING' state; some
         # failures in the streaming layer are synchronous and will not
         # otherwise yield.
         await asyncio.sleep(0)
 
-        self.logger.debug("Connecting to %s ...", address)
-
-        if isinstance(address, tuple):
+        if isinstance(address, socket.socket):
+            self.logger.debug("Connecting with existing socket: "
+                              "fd=%d, family=%r, type=%r",
+                              address.fileno(), address.family, address.type)
+            connect = asyncio.open_connection(
+                limit=self._limit,
+                ssl=ssl,
+                sock=address,
+            )
+        elif isinstance(address, tuple):
+            self.logger.debug("Connecting to %s ...", address)
             connect = asyncio.open_connection(
                 address[0],
                 address[1],
                 ssl=ssl,
                 limit=self._limit,
             )
         else:
+            self.logger.debug("Connecting to file://%s ...", address)
             connect = asyncio.open_unix_connection(
                 path=address,
                 ssl=ssl,
                 limit=self._limit,
             )
-        self._reader, self._writer = await connect
 
+        self._reader, self._writer = await connect
         self.logger.debug("Connected.")
 
     @upper_half
     async def _establish_session(self) -> None:
         """
         Establish a new session.
 
@@ -693,16 +696,16 @@
         assert self.runstate == Runstate.CONNECTING
 
         self._outgoing = asyncio.Queue()
 
         reader_coro = self._bh_loop_forever(self._bh_recv_message, 'Reader')
         writer_coro = self._bh_loop_forever(self._bh_send_message, 'Writer')
 
-        self._reader_task = create_task(reader_coro)
-        self._writer_task = create_task(writer_coro)
+        self._reader_task = asyncio.create_task(reader_coro)
+        self._writer_task = asyncio.create_task(writer_coro)
 
         self._bh_tasks = asyncio.gather(
             self._reader_task,
             self._writer_task,
         )
 
         self._set_state(Runstate.RUNNING)
@@ -719,15 +722,15 @@
         case of unhandled exceptions in the reader/writer tasks.
 
         It can be invoked no matter what the `runstate` is.
         """
         if not self._dc_task:
             self._set_state(Runstate.DISCONNECTING)
             self.logger.debug("Scheduling disconnect.")
-            self._dc_task = create_task(self._bh_disconnect())
+            self._dc_task = asyncio.create_task(self._bh_disconnect())
 
     @upper_half
     async def _wait_disconnect(self) -> None:
         """
         Waits for a previously scheduled disconnect to finish.
 
         This method will gather any bottom half exceptions and re-raise
@@ -851,25 +854,25 @@
         await self._outgoing.join()
         if self._writer is not None:
             self.logger.debug("Flushing the StreamWriter ...")
             await flush(self._writer)
 
     @bottom_half
     async def _bh_close_stream(self, error_pathway: bool = False) -> None:
-        # NB: Closing the writer also implcitly closes the reader.
+        # NB: Closing the writer also implicitly closes the reader.
         if not self._writer:
             return
 
-        if not is_closing(self._writer):
+        if not self._writer.is_closing():
             self.logger.debug("Closing StreamWriter.")
             self._writer.close()
 
         self.logger.debug("Waiting for StreamWriter to close ...")
         try:
-            await wait_closed(self._writer)
+            await self._writer.wait_closed()
         except Exception:  # pylint: disable=broad-except
             # It's hard to tell if the Stream is already closed or
             # not. Even if one of the tasks has failed, it may have
             # failed for a higher-layered protocol reason. The
             # stream could still be open and perfectly fine.
             # I don't know how to discern its health here.
```

### Comparing `qemu.qmp-0.0.2/qemu/qmp/qmp_client.py` & `qemu.qmp-0.0.3/qemu/qmp/qmp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,16 +232,16 @@
 
     See `qmp.events` for more detail on event handling patterns.
 
     """
     #: Logger object used for debugging messages.
     logger = logging.getLogger(__name__)
 
-    # Read buffer limit; large enough to accept query-qmp-schema
-    _limit = (256 * 1024)
+    # Read buffer limit; 10MB like libvirt default
+    _limit = 10 * 1024 * 1024
 
     # Type alias for pending execute() result items
     _PendingT = Union[Message, ExecInterruptedError]
 
     def __init__(self, name: Optional[str] = None) -> None:
         super().__init__(name)
         Events.__init__(self)
```

### Comparing `qemu.qmp-0.0.2/qemu/qmp/qmp_shell.py` & `qemu.qmp-0.0.3/qemu/qmp/qmp_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 --------
 
 Autocomplete of command names using <tab> is supported. Pressing <tab>
 at a blank CLI prompt will show you a list of all available commands
 that the connected QEMU instance supports.
 
 For documentation on QMP commands and their arguments, please see
-`interop/qemu-qmp-ref`.
+`qmp ref`.
 
 Events
 ------
 
 qmp-shell will display events received from the server, but this version
 does not do so asynchronously. To check for new events from the server,
 press <enter> on a blank line::
```

### Comparing `qemu.qmp-0.0.2/qemu/qmp/qmp_tui.py` & `qemu.qmp-0.0.3/qemu/qmp/qmp_tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     sys.exit(1)
 
 from .error import ProtocolError
 from .legacy import QEMUMonitorProtocol, QMPBadPortError
 from .message import DeserializationError, Message, UnexpectedTypeError
 from .protocol import ConnectError, Runstate
 from .qmp_client import ExecInterruptedError, QMPClient
-from .util import create_task, pretty_traceback
+from .util import pretty_traceback
 
 
 # The name of the signal that is used to update the history list
 UPDATE_MSG: str = 'UPDATE_MSG'
 
 
 palette = [
@@ -78,15 +78,15 @@
     """
     Formats valid/invalid multi-line JSON message into a single-line message.
 
     Formatting is first tried using the standard json module. If that fails
     due to an decoding error then a simple string manipulation is done to
     achieve a single line JSON string.
 
-    Converting into single line is more asthetically pleasing when looking
+    Converting into single line is more aesthetically pleasing when looking
     along with error messages.
 
     Eg:
     Input:
           [ 1,
             true,
             3 ]
@@ -98,15 +98,15 @@
           true,
           3 ]: QMP message is not a JSON object.
 
     whereas in singleline mode we get the following
 
         [1, true, 3]: QMP message is not a JSON object.
 
-    The single line mode is more asthetically pleasing.
+    The single line mode is more aesthetically pleasing.
 
     :param msg:
         The message to formatted into single line.
 
     :return: Formatted singleline message.
     """
     try:
@@ -232,15 +232,15 @@
         :param raw_msg:
             The raw string message to be sent to the server.
 
         :raise Exception: When an unhandled exception is caught.
         """
         try:
             msg = Message(bytes(raw_msg, encoding='utf-8'))
-            create_task(self._send_to_server(msg))
+            asyncio.create_task(self._send_to_server(msg))
         except (DeserializationError, UnexpectedTypeError) as err:
             raw_msg = format_json(raw_msg)
             logging.info('Invalid message: %s', err.error_message)
             self.add_to_history(f'{raw_msg}: {err.error_message}', 'ERROR')
 
     def unhandled_input(self, key: str) -> None:
         """
@@ -253,15 +253,15 @@
             self.kill_app()
 
     def kill_app(self) -> None:
         """
         Initiates killing of app. A bridge between asynchronous and synchronous
         code.
         """
-        create_task(self._kill_app())
+        asyncio.create_task(self._kill_app())
 
     async def _kill_app(self) -> None:
         """
         This coroutine initiates the actual disconnect process and calls
         urwid.ExitMainLoop() to kill the TUI.
 
         :raise Exception: When an unhandled exception is caught.
@@ -353,15 +353,18 @@
                 else:
                     addr = self._get_formatted_address()
                     self._set_status(f'[Connected {addr}]')
             elif self.runstate == Runstate.DISCONNECTING:
                 self._set_status('[Disconnected]')
                 await self.disconnect()
                 # check if a retry is needed
-                if self.runstate == Runstate.IDLE:
+                # mypy 1.4.0 doesn't believe runstate can change after
+                # disconnect(), hence the cast.
+                state = cast(Runstate, self.runstate)
+                if state == Runstate.IDLE:
                     continue
             await self.runstate_changed()
 
     async def connect_server(self) -> Optional[ConnectError]:
         """
         Initiates a connection to the server at address `self.address`
         and in case of a failure, sets the status to the respective error.
@@ -397,15 +400,15 @@
         main_loop = urwid.MainLoop(urwid.AttrMap(self.window, 'background'),
                                    unhandled_input=self.unhandled_input,
                                    screen=screen,
                                    palette=palette,
                                    handle_mouse=True,
                                    event_loop=event_loop)
 
-        create_task(self.manage_connection(), self.aloop)
+        self.aloop.create_task(self.manage_connection())
         try:
             main_loop.run()
         except Exception as err:
             logging.error('%s\n%s\n', str(err), pretty_traceback())
             raise err
 
 
@@ -505,15 +508,15 @@
     def __init__(self, parent: App) -> None:
         super().__init__(Editor(parent), valign='top')
 
 
 class HistoryBox(urwid.ListBox):
     """
     This widget is modelled using the ListBox widget, contains the list of
-    all messages both QMP messages and log messsages to be shown in the TUI.
+    all messages both QMP messages and log messages to be shown in the TUI.
 
     The messages are urwid.Text widgets. On every append of a message, the
     focus is shifted to the last appended message.
 
     :param parent: Reference to the TUI object.
     """
     def __init__(self, parent: App) -> None:
```

### Comparing `qemu.qmp-0.0.2/qemu.qmp.egg-info/PKG-INFO` & `qemu.qmp-0.0.3/qemu.qmp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu.qmp
-Version: 0.0.2
+Version: 0.0.3
 Summary: QEMU Monitor Protocol library
 Home-page: https://gitlab.com/qemu-project/python-qemu-qmp
 Author: QEMU Project
 Author-email: qemu-devel@nongnu.org
 Maintainer: John Snow
 Maintainer-email: jsnow@redhat.com
 Project-URL: Homepage, https://www.qemu.org/
@@ -15,38 +15,38 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Emulators
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 Provides-Extra: tui
 License-File: LICENSE
 License-File: LICENSE_GPL2
 
 qemu.qmp: QEMU Monitor Protocol Library
 =======================================
 
 Welcome! ``qemu.qmp`` is a `QEMU Monitor Protocol
 <https://gitlab.com/qemu-project/qemu/-/blob/master/docs/interop/qmp-intro.txt>`_
 (“QMP”) library written in Python, using `asyncio
 <https://docs.python.org/3/library/asyncio.html>`_. It is used to send
 QMP messages to running `QEMU <https://www.qemu.org/>`_ emulators. It
-requires Python 3.6+ and has no mandatory dependencies.
+requires Python 3.7+ and has no mandatory dependencies.
 
 This library can be used to communicate with QEMU emulators, the `QEMU
 Guest Agent
 <https://qemu.readthedocs.io/en/latest/interop/qemu-ga.html>`_ (QGA),
 the `QEMU Storage Daemon
 <https://qemu.readthedocs.io/en/latest/tools/qemu-storage-daemon.html>`_
 (QSD), or any other utility or application that `speaks QMP
@@ -216,14 +216,40 @@
 will always be bugfixes, and minor updates will be reserved for
 backwards compatible feature changes.
 
 
 Changelog
 ---------
 
+0.0.3 (2023-07-10)
+^^^^^^^^^^^^^^^^^^
+
+This release addresses packaging issues associated with the forthcoming
+release of Python 3.12. This release adds Python 3.12 support, drops
+Python 3.6 support, and switches to PEP-517 native packaging.
+
+- `!25 <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/25>`_:
+  Drop Python 3.6 support
+- `#30 <https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/30>`_:
+  The read buffer limit has been increased from 256KiB to 10MiB for
+  parity with libvirt's default and to accommodate real-world replies
+  that may exceed the current limit.
+- `#29 <https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/29>`_:
+  The connect() call now accepts existing sockets as an 'address',
+  allowing for easier use of socketpairs to create client/server pairs.
+  This functionality was revised in `!22
+  <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/22>`_.
+- `!23 <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/23>`_:
+  Fix deadlock on disconnect under CPython 3.12.
+  See also `<https://github.com/python/cpython/issues/104344>`_.
+- `!24
+  <https://gitlab.com/qemu-project/python-qemu-qmp/-/merge_requests/24>`_:
+  Switch to PEP517 native packaging to coincide with Python 3.12
+  dropping distutils, setuptools from ensurepip, etc.
+
 0.0.2 (2022-08-26)
 ^^^^^^^^^^^^^^^^^^
 
 This release primarily fixes development tooling, documentation, and
 packaging issues that have no impact on the library itself. A handful of
 small, runtime visible changes were added as polish.
```

### Comparing `qemu.qmp-0.0.2/setup.cfg` & `qemu.qmp-0.0.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -19,40 +19,40 @@
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 	License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: System :: Emulators
 	Typing :: Typed
 
 [options]
-setup_requires = setuptools_scm
-python_requires = >= 3.6
+python_requires = >= 3.7
 packages = 
 	qemu.qmp
 
 [options.package_data]
 * = py.typed
 
 [options.extras_require]
 devel = 
 	avocado-framework >= 90.0
 	coverage >= 6.1.0
-	flake8 >= 3.6.0
+	flake8 >= 5.0.4
 	isort >= 5.1.2
-	mypy >= 0.780
-	pylint >= 2.8.0
+	mypy >= 1.4.0
+	pylint >= 2.17.3
+	setuptools >= 66.1.0; python_version>="3.12"
 	tox >= 3.18.0
 	urwid >= 2.1.2
 	urwid-readline >= 0.13
 	Pygments >= 2.9.0
 tui = 
 	urwid >= 2.1.2
 	urwid-readline >= 0.13
@@ -61,20 +61,20 @@
 [options.entry_points]
 console_scripts = 
 	qmp-shell = qemu.qmp.qmp_shell:main
 	qmp-shell-wrap = qemu.qmp.qmp_shell:main_wrap
 	qmp-tui = qemu.qmp.qmp_tui:main [tui]
 
 [flake8]
-extend-ignore = E722  # Prefer pylint's bare-except checks to flake8's
+extend-ignore = E722
 exclude = __pycache__,
 
 [mypy]
 strict = True
-python_version = 3.6
+python_version = 3.7
 warn_unused_configs = True
 namespace_packages = True
 warn_unused_ignores = False
 
 [mypy-qemu.qmp.qmp_tui]
 allow_subclassing_any = True
 
@@ -102,14 +102,15 @@
 	ex,
 	Run,
 	_,   # By convention: Unused variable
 	fh,  # fh = open(...)
 	fd,  # fd = os.open(...)
 	c,   # for c in string: ...
 	T,   # for TypeVars. See pylint#3401
+	SocketAddrT,  # Type Alias, won't change it now.
 
 [pylint.similarities]
 ignore-imports = yes
 ignore-signatures = yes
 min-similarity-lines = 6
 
 [isort]
@@ -117,15 +118,15 @@
 force_sort_within_sections = True
 include_trailing_comma = True
 line_length = 72
 lines_after_imports = 2
 multi_line_output = 3
 
 [tox:tox]
-envlist = py36, py37, py38, py39, py310, py311
+envlist = py37, py38, py39, py310, py311, py312
 skip_missing_interpreters = true
 
 [testenv]
 allowlist_externals = make
 deps = 
 	.[devel]
 	.[tui]   # Workaround to trigger tox venv rebuild
```

### Comparing `qemu.qmp-0.0.2/tests/minreqs.txt` & `qemu.qmp-0.0.3/tests/minreqs.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file lists the ***oldest possible dependencies*** needed to run
-# "make check" successfully under ***Python 3.6***. It is used primarily
+# "make check" successfully under ***Python 3.7***. It is used primarily
 # by GitLab CI to ensure that our stated minimum versions in setup.cfg
 # are truthful and regularly validated.
 #
 # This file should not contain any dependencies that are not expressed
 # by the [devel] section of setup.cfg, except for transitive
 # dependencies which must be enumerated here explicitly to eliminate
 # dependency resolution ambiguity.
@@ -16,27 +16,26 @@
 urwid-readline==0.13
 Pygments==2.9.0
 
 # Test-runners, utilities, etc.
 avocado-framework==90.0
 
 # Linters
-flake8==3.6.0
+flake8==5.0.4
 isort==5.1.2
-mypy==0.780
-pylint==2.8.0
+mypy==1.4.0
+pylint==2.17.3
 
 # Transitive flake8 dependencies
-mccabe==0.6.0
-pycodestyle==2.4.0
-pyflakes==2.0.0
+mccabe==0.7.0
+pycodestyle==2.9.1
+pyflakes==2.5.0
 
 # Transitive mypy dependencies
-mypy-extensions==0.4.3
-typed-ast==1.4.0
-typing-extensions==3.7.4
+mypy-extensions==1.0.0
+typing-extensions==4.7.1
 
 # Transitive pylint dependencies
-astroid==2.5.4
+astroid==2.15.4
 lazy-object-proxy==1.4.0
 toml==0.10.0
-wrapt==1.12.1
+wrapt==1.14.0
```

### Comparing `qemu.qmp-0.0.2/tests/protocol.py` & `qemu.qmp-0.0.3/tests/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import socket
 from tempfile import TemporaryDirectory
 
 import avocado
 
 from qemu.qmp import ConnectError, Runstate
 from qemu.qmp.protocol import AsyncProtocol, StateError
-from qemu.qmp.util import asyncio_run, create_task
 
 
 class NullProtocol(AsyncProtocol[None]):
     """
     NullProtocol is a test mockup of an AsyncProtocol implementation.
 
     It adds a fake_session instance variable that enables a code path
@@ -120,15 +119,15 @@
     async def _runner():
         try:
             await coro
         except asyncio.CancelledError:
             if allow_cancellation:
                 return
             raise
-    return create_task(_runner())
+    return asyncio.create_task(_runner())
 
 
 @contextmanager
 def jammed_socket():
     """
     Opens up a random unused TCP port on localhost, then jams it.
     """
@@ -267,15 +266,15 @@
                 new_state = await self.proto.runstate_changed()
                 self.assertEqual(
                     new_state,
                     state,
                     msg=f"Expected state '{state.name}'",
                 )
 
-        self.runstate_watcher = create_task(_watcher())
+        self.runstate_watcher = asyncio.create_task(_watcher())
         # Kick the loop and force the task to block on the event.
         await asyncio.sleep(0)
 
 
 class State(TestBase):
 
     @TestBase.async_test
@@ -585,12 +584,13 @@
             pass
         await super()._asyncTearDown()
 
     @TestBase.async_test
     async def testSmoke(self):
         with TemporaryDirectory(suffix='.qmp') as tmpdir:
             sock = os.path.join(tmpdir, type(self.proto).__name__ + ".sock")
-            server_task = create_task(self.server.start_server_and_accept(sock))
+            server_task = asyncio.create_task(
+                self.server.start_server_and_accept(sock))
 
             # give the server a chance to start listening [...]
             await asyncio.sleep(0)
             await self.proto.connect(sock)
```

