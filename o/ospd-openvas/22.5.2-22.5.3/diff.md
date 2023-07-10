# Comparing `tmp/ospd_openvas-22.5.2.tar.gz` & `tmp/ospd_openvas-22.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospd_openvas-22.5.2.tar", max compression
+gzip compressed data, was "ospd_openvas-22.5.3.tar", max compression
```

## Comparing `ospd_openvas-22.5.2.tar` & `ospd_openvas-22.5.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0    12468 2023-07-10 07:32:16.012343 ospd_openvas-22.5.2/CHANGELOG.md
--rw-r--r--   0        0        0    34008 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/COPYING
--rw-r--r--   0        0        0     4883 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/README.md
--rw-r--r--   0        0        0      175 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/config/ospd-openvas.conf
--rw-r--r--   0        0        0      636 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/config/ospd-openvas.service
--rw-r--r--   0        0        0     4972 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/docs/ospd-openvas.8
--rw-r--r--   0        0        0      197 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/__init__.py
--rw-r--r--   0        0        0      222 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/__init__.py
--rw-r--r--   0        0        0    22603 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/command.py
--rw-r--r--   0        0        0     1064 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/initsubclass.py
--rw-r--r--   0        0        0      508 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/registry.py
--rw-r--r--   0        0        0     1006 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/config.py
--rw-r--r--   0        0        0     4622 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/cvss.py
--rw-r--r--   0        0        0     4267 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/datapickler.py
--rw-r--r--   0        0        0     1213 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/errors.py
--rw-r--r--   0        0        0     2687 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/logger.py
--rw-r--r--   0        0        0     3858 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/main.py
--rw-r--r--   0        0        0     3889 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/misc.py
--rw-r--r--   0        0        0    15592 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/network.py
--rw-r--r--   0        0        0    48878 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/ospd.py
--rw-r--r--   0        0        0     9379 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/parser.py
--rw-r--r--   0        0        0    10771 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/protocol.py
--rw-r--r--   0        0        0     3312 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/resultlist.py
--rw-r--r--   0        0        0    20486 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/scan.py
--rw-r--r--   0        0        0     8566 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/server.py
--rw-r--r--   0        0        0     1245 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/timer.py
--rw-r--r--   0        0        0     4124 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/vtfilter.py
--rw-r--r--   0        0        0     5742 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/vts.py
--rw-r--r--   0        0        0     8644 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/xml.py
--rw-r--r--   0        0        0    12082 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/xmlvt.py
--rw-r--r--   0        0        0      158 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/__init__.py
--rw-r--r--   0        0        0      103 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/__version__.py
--rw-r--r--   0        0        0    43210 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/daemon.py
--rw-r--r--   0        0        0    22000 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/db.py
--rw-r--r--   0        0        0     6462 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/dryrun.py
--rw-r--r--   0        0        0      338 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/errors.py
--rw-r--r--   0        0        0     4621 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/gpg_sha_verifier.py
--rw-r--r--   0        0        0     3292 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/lock.py
--rw-r--r--   0        0        0      120 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messages/__init__.py
--rw-r--r--   0        0        0     2294 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messages/message.py
--rw-r--r--   0        0        0     2271 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messages/result.py
--rw-r--r--   0        0        0      120 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/__init__.py
--rw-r--r--   0        0        0     5372 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/mqtt.py
--rw-r--r--   0        0        0      482 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/publisher.py
--rw-r--r--   0        0        0      586 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/subscriber.py
--rw-r--r--   0        0        0     8473 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/notus.py
--rw-r--r--   0        0        0     9123 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/nvticache.py
--rw-r--r--   0        0        0     5553 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/openvas.py
--rw-r--r--   0        0        0    28613 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/preferencehandler.py
--rw-r--r--   0        0        0     8361 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/vthelper.py
--rw-r--r--   0        0        0    69856 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/poetry.lock
--rw-r--r--   0        0        0       32 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/poetry.toml
--rw-r--r--   0        0        0     2295 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/pyproject.toml
--rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/__init__.py
--rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/__init__.py
--rw-r--r--   0        0        0     2026 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/test_command.py
--rw-r--r--   0        0        0    17023 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/test_commands.py
--rw-r--r--   0        0        0     1423 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/test_registry.py
--rw-r--r--   0        0        0     5527 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/dummydaemon.py
--rw-r--r--   0        0        0     6420 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/helper.py
--rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messages/__init__.py
--rw-r--r--   0        0        0     4207 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messages/test_message.py
--rw-r--r--   0        0        0     5878 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messages/test_result.py
--rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messaging/__init__.py
--rw-r--r--   0        0        0     2726 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messaging/test_mqtt.py
--rw-r--r--   0        0        0     4761 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_argument_parser.py
--rw-r--r--   0        0        0     1007 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_cvss.py
--rw-r--r--   0        0        0    22986 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_daemon.py
--rw-r--r--   0        0        0     3633 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_datapickler.py
--rw-r--r--   0        0        0    24645 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_db.py
--rw-r--r--   0        0        0     1781 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_errors.py
--rw-r--r--   0        0        0     2864 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_gpg.py
--rw-r--r--   0        0        0     2986 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_lock.py
--rw-r--r--   0        0        0     6815 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_notus.py
--rw-r--r--   0        0        0    10724 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_nvti_cache.py
--rw-r--r--   0        0        0    10266 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_openvas.py
--rw-r--r--   0        0        0    56305 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_port_convert.py
--rw-r--r--   0        0        0    50013 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_preferencehandler.py
--rw-r--r--   0        0        0      452 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_protocol.py
--rw-r--r--   0        0        0    54414 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_scan_and_result.py
--rw-r--r--   0        0        0     3253 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_target_convert.py
--rw-r--r--   0        0        0     9638 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_vthelper.py
--rw-r--r--   0        0        0     4896 2023-07-10 07:32:16.024343 ospd_openvas-22.5.2/tests/test_vts.py
--rw-r--r--   0        0        0    14396 2023-07-10 07:32:16.024343 ospd_openvas-22.5.2/tests/test_xml.py
--rw-r--r--   0        0        0      373 2023-07-10 07:32:16.024343 ospd_openvas-22.5.2/tests/testing.conf
--rw-r--r--   0        0        0     6207 1970-01-01 00:00:00.000000 ospd_openvas-22.5.2/PKG-INFO
+-rw-r--r--   0        0        0    12468 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0    34008 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/COPYING
+-rw-r--r--   0        0        0     4883 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/README.md
+-rw-r--r--   0        0        0      175 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/config/ospd-openvas.conf
+-rw-r--r--   0        0        0      636 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/config/ospd-openvas.service
+-rw-r--r--   0        0        0     4972 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/docs/ospd-openvas.8
+-rw-r--r--   0        0        0      197 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/ospd/__init__.py
+-rw-r--r--   0        0        0      222 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/ospd/command/__init__.py
+-rw-r--r--   0        0        0    22603 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/ospd/command/command.py
+-rw-r--r--   0        0        0     1064 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/ospd/command/initsubclass.py
+-rw-r--r--   0        0        0      508 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/ospd/command/registry.py
+-rw-r--r--   0        0        0     1006 2023-07-10 11:02:46.533751 ospd_openvas-22.5.3/ospd/config.py
+-rw-r--r--   0        0        0     4622 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/cvss.py
+-rw-r--r--   0        0        0     4267 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/datapickler.py
+-rw-r--r--   0        0        0     1213 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/errors.py
+-rw-r--r--   0        0        0     2687 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/logger.py
+-rw-r--r--   0        0        0     3858 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/main.py
+-rw-r--r--   0        0        0     3889 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/misc.py
+-rw-r--r--   0        0        0    15592 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/network.py
+-rw-r--r--   0        0        0    48878 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/ospd.py
+-rw-r--r--   0        0        0     9379 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/parser.py
+-rw-r--r--   0        0        0    10771 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/protocol.py
+-rw-r--r--   0        0        0     3312 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/resultlist.py
+-rw-r--r--   0        0        0    20486 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/scan.py
+-rw-r--r--   0        0        0     8566 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/server.py
+-rw-r--r--   0        0        0     1245 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/timer.py
+-rw-r--r--   0        0        0     4124 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/vtfilter.py
+-rw-r--r--   0        0        0     5742 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/vts.py
+-rw-r--r--   0        0        0     8644 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/xml.py
+-rw-r--r--   0        0        0    12082 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd/xmlvt.py
+-rw-r--r--   0        0        0      158 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/__version__.py
+-rw-r--r--   0        0        0    43210 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/daemon.py
+-rw-r--r--   0        0        0    22000 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/db.py
+-rw-r--r--   0        0        0     6462 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/dryrun.py
+-rw-r--r--   0        0        0      338 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/errors.py
+-rw-r--r--   0        0        0     4621 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/gpg_sha_verifier.py
+-rw-r--r--   0        0        0     3292 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/lock.py
+-rw-r--r--   0        0        0      120 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messages/__init__.py
+-rw-r--r--   0        0        0     2294 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messages/message.py
+-rw-r--r--   0        0        0     2271 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messages/result.py
+-rw-r--r--   0        0        0      120 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messaging/__init__.py
+-rw-r--r--   0        0        0     5372 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messaging/mqtt.py
+-rw-r--r--   0        0        0      482 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messaging/publisher.py
+-rw-r--r--   0        0        0      586 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/messaging/subscriber.py
+-rw-r--r--   0        0        0     8473 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/notus.py
+-rw-r--r--   0        0        0     9123 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/nvticache.py
+-rw-r--r--   0        0        0     5553 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/openvas.py
+-rw-r--r--   0        0        0    28613 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/preferencehandler.py
+-rw-r--r--   0        0        0     8361 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/ospd_openvas/vthelper.py
+-rw-r--r--   0        0        0    69856 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/poetry.lock
+-rw-r--r--   0        0        0       32 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/poetry.toml
+-rw-r--r--   0        0        0     2295 2023-07-10 11:02:46.537751 ospd_openvas-22.5.3/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      120 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/command/__init__.py
+-rw-r--r--   0        0        0     2026 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/command/test_command.py
+-rw-r--r--   0        0        0    17023 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/command/test_commands.py
+-rw-r--r--   0        0        0     1423 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/command/test_registry.py
+-rw-r--r--   0        0        0     5527 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/dummydaemon.py
+-rw-r--r--   0        0        0     6420 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/helper.py
+-rw-r--r--   0        0        0      120 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/messages/__init__.py
+-rw-r--r--   0        0        0     4207 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/messages/test_message.py
+-rw-r--r--   0        0        0     5878 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/messages/test_result.py
+-rw-r--r--   0        0        0      120 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/messaging/__init__.py
+-rw-r--r--   0        0        0     2726 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/messaging/test_mqtt.py
+-rw-r--r--   0        0        0     4761 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_argument_parser.py
+-rw-r--r--   0        0        0     1007 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_cvss.py
+-rw-r--r--   0        0        0    22986 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_daemon.py
+-rw-r--r--   0        0        0     3633 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_datapickler.py
+-rw-r--r--   0        0        0    24645 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_db.py
+-rw-r--r--   0        0        0     1781 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_errors.py
+-rw-r--r--   0        0        0     2864 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_gpg.py
+-rw-r--r--   0        0        0     2986 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_lock.py
+-rw-r--r--   0        0        0     6815 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_notus.py
+-rw-r--r--   0        0        0    10724 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_nvti_cache.py
+-rw-r--r--   0        0        0    10266 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_openvas.py
+-rw-r--r--   0        0        0    56305 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_port_convert.py
+-rw-r--r--   0        0        0    50013 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_preferencehandler.py
+-rw-r--r--   0        0        0      452 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_protocol.py
+-rw-r--r--   0        0        0    54414 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_scan_and_result.py
+-rw-r--r--   0        0        0     3253 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_target_convert.py
+-rw-r--r--   0        0        0     9638 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_vthelper.py
+-rw-r--r--   0        0        0     4896 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_vts.py
+-rw-r--r--   0        0        0    14396 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/test_xml.py
+-rw-r--r--   0        0        0      373 2023-07-10 11:02:46.541751 ospd_openvas-22.5.3/tests/testing.conf
+-rw-r--r--   0        0        0     6207 1970-01-01 00:00:00.000000 ospd_openvas-22.5.3/PKG-INFO
```

### Comparing `ospd_openvas-22.5.2/CHANGELOG.md` & `ospd_openvas-22.5.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/COPYING` & `ospd_openvas-22.5.3/COPYING`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/README.md` & `ospd_openvas-22.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/config/ospd-openvas.service` & `ospd_openvas-22.5.3/config/ospd-openvas.service`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/docs/ospd-openvas.8` & `ospd_openvas-22.5.3/docs/ospd-openvas.8`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/command/command.py` & `ospd_openvas-22.5.3/ospd/command/command.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/command/initsubclass.py` & `ospd_openvas-22.5.3/ospd/command/initsubclass.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/config.py` & `ospd_openvas-22.5.3/ospd/config.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/cvss.py` & `ospd_openvas-22.5.3/ospd/cvss.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/datapickler.py` & `ospd_openvas-22.5.3/ospd/datapickler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/errors.py` & `ospd_openvas-22.5.3/ospd/errors.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/logger.py` & `ospd_openvas-22.5.3/ospd/logger.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/main.py` & `ospd_openvas-22.5.3/ospd/main.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/misc.py` & `ospd_openvas-22.5.3/ospd/misc.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/network.py` & `ospd_openvas-22.5.3/ospd/network.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/ospd.py` & `ospd_openvas-22.5.3/ospd/ospd.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/parser.py` & `ospd_openvas-22.5.3/ospd/parser.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/protocol.py` & `ospd_openvas-22.5.3/ospd/protocol.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/resultlist.py` & `ospd_openvas-22.5.3/ospd/resultlist.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/scan.py` & `ospd_openvas-22.5.3/ospd/scan.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/server.py` & `ospd_openvas-22.5.3/ospd/server.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/timer.py` & `ospd_openvas-22.5.3/ospd/timer.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/vtfilter.py` & `ospd_openvas-22.5.3/ospd/vtfilter.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/vts.py` & `ospd_openvas-22.5.3/ospd/vts.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/xml.py` & `ospd_openvas-22.5.3/ospd/xml.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd/xmlvt.py` & `ospd_openvas-22.5.3/ospd/xmlvt.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/daemon.py` & `ospd_openvas-22.5.3/ospd_openvas/daemon.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/db.py` & `ospd_openvas-22.5.3/ospd_openvas/db.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/dryrun.py` & `ospd_openvas-22.5.3/ospd_openvas/dryrun.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/gpg_sha_verifier.py` & `ospd_openvas-22.5.3/ospd_openvas/gpg_sha_verifier.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/lock.py` & `ospd_openvas-22.5.3/ospd_openvas/lock.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/messages/message.py` & `ospd_openvas-22.5.3/ospd_openvas/messages/message.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/messages/result.py` & `ospd_openvas-22.5.3/ospd_openvas/messages/result.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/messaging/mqtt.py` & `ospd_openvas-22.5.3/ospd_openvas/messaging/mqtt.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/messaging/subscriber.py` & `ospd_openvas-22.5.3/ospd_openvas/messaging/subscriber.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/notus.py` & `ospd_openvas-22.5.3/ospd_openvas/notus.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/nvticache.py` & `ospd_openvas-22.5.3/ospd_openvas/nvticache.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/openvas.py` & `ospd_openvas-22.5.3/ospd_openvas/openvas.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/preferencehandler.py` & `ospd_openvas-22.5.3/ospd_openvas/preferencehandler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/ospd_openvas/vthelper.py` & `ospd_openvas-22.5.3/ospd_openvas/vthelper.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/poetry.lock` & `ospd_openvas-22.5.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/pyproject.toml` & `ospd_openvas-22.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ospd-openvas"
-version = "22.5.2"
+version = "22.5.3"
 description = "ospd based scanner for openvas"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/ospd-openvas"
 repository = "https://github.com/greenbone/ospd-openvas"
 # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
```

### Comparing `ospd_openvas-22.5.2/tests/command/test_command.py` & `ospd_openvas-22.5.3/tests/command/test_command.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/command/test_commands.py` & `ospd_openvas-22.5.3/tests/command/test_commands.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/command/test_registry.py` & `ospd_openvas-22.5.3/tests/command/test_registry.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/dummydaemon.py` & `ospd_openvas-22.5.3/tests/dummydaemon.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/helper.py` & `ospd_openvas-22.5.3/tests/helper.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/messages/test_message.py` & `ospd_openvas-22.5.3/tests/messages/test_message.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/messages/test_result.py` & `ospd_openvas-22.5.3/tests/messages/test_result.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/messaging/test_mqtt.py` & `ospd_openvas-22.5.3/tests/messaging/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_argument_parser.py` & `ospd_openvas-22.5.3/tests/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_cvss.py` & `ospd_openvas-22.5.3/tests/test_cvss.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_daemon.py` & `ospd_openvas-22.5.3/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_datapickler.py` & `ospd_openvas-22.5.3/tests/test_datapickler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_db.py` & `ospd_openvas-22.5.3/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_errors.py` & `ospd_openvas-22.5.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_gpg.py` & `ospd_openvas-22.5.3/tests/test_gpg.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_lock.py` & `ospd_openvas-22.5.3/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_notus.py` & `ospd_openvas-22.5.3/tests/test_notus.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_nvti_cache.py` & `ospd_openvas-22.5.3/tests/test_nvti_cache.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_openvas.py` & `ospd_openvas-22.5.3/tests/test_openvas.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_port_convert.py` & `ospd_openvas-22.5.3/tests/test_port_convert.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_preferencehandler.py` & `ospd_openvas-22.5.3/tests/test_preferencehandler.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_scan_and_result.py` & `ospd_openvas-22.5.3/tests/test_scan_and_result.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_target_convert.py` & `ospd_openvas-22.5.3/tests/test_target_convert.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_vthelper.py` & `ospd_openvas-22.5.3/tests/test_vthelper.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_vts.py` & `ospd_openvas-22.5.3/tests/test_vts.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/tests/test_xml.py` & `ospd_openvas-22.5.3/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.2/PKG-INFO` & `ospd_openvas-22.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospd-openvas
-Version: 22.5.2
+Version: 22.5.3
 Summary: ospd based scanner for openvas
 Home-page: https://github.com/greenbone/ospd-openvas
 License: AGPL-3.0-or-later
 Keywords: openvas,Greenbone Vulnerability Management,Vulnerability Scanning,OSP,Open Scanner Protocol
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
```

