# Comparing `tmp/ospd_openvas-22.5.1.tar.gz` & `tmp/ospd_openvas-22.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospd_openvas-22.5.1.tar", max compression
+gzip compressed data, was "ospd_openvas-22.5.2.tar", max compression
```

## Comparing `ospd_openvas-22.5.1.tar` & `ospd_openvas-22.5.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0    12468 2023-05-08 11:02:34.054608 ospd_openvas-22.5.1/CHANGELOG.md
--rw-r--r--   0        0        0    34008 2023-05-08 11:02:34.054608 ospd_openvas-22.5.1/COPYING
--rw-r--r--   0        0        0     4883 2023-05-08 11:02:34.054608 ospd_openvas-22.5.1/README.md
--rw-r--r--   0        0        0      175 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/config/ospd-openvas.conf
--rw-r--r--   0        0        0      636 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/config/ospd-openvas.service
--rw-r--r--   0        0        0     4972 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/docs/ospd-openvas.8
--rw-r--r--   0        0        0      843 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/__init__.py
--rw-r--r--   0        0        0      844 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/__init__.py
--rw-r--r--   0        0        0    23225 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/command.py
--rw-r--r--   0        0        0     1686 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/initsubclass.py
--rw-r--r--   0        0        0     1130 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/command/registry.py
--rw-r--r--   0        0        0     1628 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/config.py
--rw-r--r--   0        0        0     5244 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/cvss.py
--rw-r--r--   0        0        0     4889 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/datapickler.py
--rw-r--r--   0        0        0     1835 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/errors.py
--rw-r--r--   0        0        0     3309 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/logger.py
--rw-r--r--   0        0        0     4480 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/main.py
--rw-r--r--   0        0        0     4511 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/misc.py
--rw-r--r--   0        0        0    16214 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/network.py
--rw-r--r--   0        0        0    49500 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/ospd.py
--rw-r--r--   0        0        0    10001 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/parser.py
--rw-r--r--   0        0        0    11393 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/protocol.py
--rw-r--r--   0        0        0     3934 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/resultlist.py
--rw-r--r--   0        0        0    21108 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/scan.py
--rw-r--r--   0        0        0     9188 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/server.py
--rw-r--r--   0        0        0     1867 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/timer.py
--rw-r--r--   0        0        0     4746 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/vtfilter.py
--rw-r--r--   0        0        0     6364 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/vts.py
--rw-r--r--   0        0        0     9266 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/xml.py
--rw-r--r--   0        0        0    12704 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd/xmlvt.py
--rw-r--r--   0        0        0      804 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/__init__.py
--rw-r--r--   0        0        0      103 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/__version__.py
--rw-r--r--   0        0        0    44267 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/daemon.py
--rw-r--r--   0        0        0    22646 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/db.py
--rw-r--r--   0        0        0     7104 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/dryrun.py
--rw-r--r--   0        0        0      984 2023-05-08 11:02:34.058608 ospd_openvas-22.5.1/ospd_openvas/errors.py
--rw-r--r--   0        0        0     4500 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/gpg_sha_verifier.py
--rw-r--r--   0        0        0     3939 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/lock.py
--rw-r--r--   0        0        0      737 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messages/__init__.py
--rw-r--r--   0        0        0     2911 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messages/message.py
--rw-r--r--   0        0        0     2888 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messages/result.py
--rw-r--r--   0        0        0      737 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/__init__.py
--rw-r--r--   0        0        0     5989 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/mqtt.py
--rw-r--r--   0        0        0     1099 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/publisher.py
--rw-r--r--   0        0        0     1203 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/messaging/subscriber.py
--rw-r--r--   0        0        0     9119 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/notus.py
--rw-r--r--   0        0        0     9770 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/nvticache.py
--rw-r--r--   0        0        0     6199 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/openvas.py
--rw-r--r--   0        0        0    29260 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/preferencehandler.py
--rw-r--r--   0        0        0     9008 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/ospd_openvas/vthelper.py
--rw-r--r--   0        0        0    71446 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/poetry.lock
--rw-r--r--   0        0        0       32 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/poetry.toml
--rw-r--r--   0        0        0     2390 2023-05-08 11:02:34.062608 ospd_openvas-22.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/__init__.py
--rw-r--r--   0        0        0      742 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/__init__.py
--rw-r--r--   0        0        0     2648 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/test_command.py
--rw-r--r--   0        0        0    17645 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/test_commands.py
--rw-r--r--   0        0        0     2045 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/command/test_registry.py
--rw-r--r--   0        0        0     6173 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/dummydaemon.py
--rw-r--r--   0        0        0     7066 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/helper.py
--rw-r--r--   0        0        0      737 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messages/__init__.py
--rw-r--r--   0        0        0     4824 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messages/test_message.py
--rw-r--r--   0        0        0     6495 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messages/test_result.py
--rw-r--r--   0        0        0      737 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messaging/__init__.py
--rw-r--r--   0        0        0     3343 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/messaging/test_mqtt.py
--rw-r--r--   0        0        0     5383 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_argument_parser.py
--rw-r--r--   0        0        0     1629 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_cvss.py
--rw-r--r--   0        0        0    23632 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_daemon.py
--rw-r--r--   0        0        0     4255 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_datapickler.py
--rw-r--r--   0        0        0    25291 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_db.py
--rw-r--r--   0        0        0     2403 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_errors.py
--rw-r--r--   0        0        0     3481 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_gpg.py
--rw-r--r--   0        0        0     3632 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_lock.py
--rw-r--r--   0        0        0     7461 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_notus.py
--rw-r--r--   0        0        0    11370 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_nvti_cache.py
--rw-r--r--   0        0        0    10912 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_openvas.py
--rw-r--r--   0        0        0    56927 2023-05-08 11:02:34.066609 ospd_openvas-22.5.1/tests/test_port_convert.py
--rw-r--r--   0        0        0    50659 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_preferencehandler.py
--rw-r--r--   0        0        0     1074 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_protocol.py
--rw-r--r--   0        0        0    55036 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_scan_and_result.py
--rw-r--r--   0        0        0     3875 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_target_convert.py
--rw-r--r--   0        0        0    10284 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_vthelper.py
--rw-r--r--   0        0        0     5518 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_vts.py
--rw-r--r--   0        0        0    15018 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/test_xml.py
--rw-r--r--   0        0        0      373 2023-05-08 11:02:34.070608 ospd_openvas-22.5.1/tests/testing.conf
--rw-r--r--   0        0        0     6447 1970-01-01 00:00:00.000000 ospd_openvas-22.5.1/PKG-INFO
+-rw-r--r--   0        0        0    12468 2023-07-10 07:32:16.012343 ospd_openvas-22.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0    34008 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/COPYING
+-rw-r--r--   0        0        0     4883 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/README.md
+-rw-r--r--   0        0        0      175 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/config/ospd-openvas.conf
+-rw-r--r--   0        0        0      636 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/config/ospd-openvas.service
+-rw-r--r--   0        0        0     4972 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/docs/ospd-openvas.8
+-rw-r--r--   0        0        0      197 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/__init__.py
+-rw-r--r--   0        0        0      222 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/__init__.py
+-rw-r--r--   0        0        0    22603 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/command.py
+-rw-r--r--   0        0        0     1064 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/initsubclass.py
+-rw-r--r--   0        0        0      508 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/command/registry.py
+-rw-r--r--   0        0        0     1006 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/config.py
+-rw-r--r--   0        0        0     4622 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/cvss.py
+-rw-r--r--   0        0        0     4267 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/datapickler.py
+-rw-r--r--   0        0        0     1213 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/errors.py
+-rw-r--r--   0        0        0     2687 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/logger.py
+-rw-r--r--   0        0        0     3858 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/main.py
+-rw-r--r--   0        0        0     3889 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/misc.py
+-rw-r--r--   0        0        0    15592 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/network.py
+-rw-r--r--   0        0        0    48878 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/ospd.py
+-rw-r--r--   0        0        0     9379 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/parser.py
+-rw-r--r--   0        0        0    10771 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/protocol.py
+-rw-r--r--   0        0        0     3312 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/resultlist.py
+-rw-r--r--   0        0        0    20486 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/scan.py
+-rw-r--r--   0        0        0     8566 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/server.py
+-rw-r--r--   0        0        0     1245 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/timer.py
+-rw-r--r--   0        0        0     4124 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/vtfilter.py
+-rw-r--r--   0        0        0     5742 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/vts.py
+-rw-r--r--   0        0        0     8644 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/xml.py
+-rw-r--r--   0        0        0    12082 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd/xmlvt.py
+-rw-r--r--   0        0        0      158 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/__version__.py
+-rw-r--r--   0        0        0    43210 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/daemon.py
+-rw-r--r--   0        0        0    22000 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/db.py
+-rw-r--r--   0        0        0     6462 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/dryrun.py
+-rw-r--r--   0        0        0      338 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/errors.py
+-rw-r--r--   0        0        0     4621 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/gpg_sha_verifier.py
+-rw-r--r--   0        0        0     3292 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/lock.py
+-rw-r--r--   0        0        0      120 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messages/__init__.py
+-rw-r--r--   0        0        0     2294 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messages/message.py
+-rw-r--r--   0        0        0     2271 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messages/result.py
+-rw-r--r--   0        0        0      120 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/__init__.py
+-rw-r--r--   0        0        0     5372 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/mqtt.py
+-rw-r--r--   0        0        0      482 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/publisher.py
+-rw-r--r--   0        0        0      586 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/messaging/subscriber.py
+-rw-r--r--   0        0        0     8473 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/notus.py
+-rw-r--r--   0        0        0     9123 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/nvticache.py
+-rw-r--r--   0        0        0     5553 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/openvas.py
+-rw-r--r--   0        0        0    28613 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/preferencehandler.py
+-rw-r--r--   0        0        0     8361 2023-07-10 07:32:16.016343 ospd_openvas-22.5.2/ospd_openvas/vthelper.py
+-rw-r--r--   0        0        0    69856 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/poetry.lock
+-rw-r--r--   0        0        0       32 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/poetry.toml
+-rw-r--r--   0        0        0     2295 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/__init__.py
+-rw-r--r--   0        0        0     2026 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/test_command.py
+-rw-r--r--   0        0        0    17023 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/test_commands.py
+-rw-r--r--   0        0        0     1423 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/command/test_registry.py
+-rw-r--r--   0        0        0     5527 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/dummydaemon.py
+-rw-r--r--   0        0        0     6420 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/helper.py
+-rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messages/__init__.py
+-rw-r--r--   0        0        0     4207 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messages/test_message.py
+-rw-r--r--   0        0        0     5878 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messages/test_result.py
+-rw-r--r--   0        0        0      120 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messaging/__init__.py
+-rw-r--r--   0        0        0     2726 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/messaging/test_mqtt.py
+-rw-r--r--   0        0        0     4761 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_argument_parser.py
+-rw-r--r--   0        0        0     1007 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_cvss.py
+-rw-r--r--   0        0        0    22986 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_daemon.py
+-rw-r--r--   0        0        0     3633 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_datapickler.py
+-rw-r--r--   0        0        0    24645 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_db.py
+-rw-r--r--   0        0        0     1781 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_errors.py
+-rw-r--r--   0        0        0     2864 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_gpg.py
+-rw-r--r--   0        0        0     2986 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_lock.py
+-rw-r--r--   0        0        0     6815 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_notus.py
+-rw-r--r--   0        0        0    10724 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_nvti_cache.py
+-rw-r--r--   0        0        0    10266 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_openvas.py
+-rw-r--r--   0        0        0    56305 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_port_convert.py
+-rw-r--r--   0        0        0    50013 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_preferencehandler.py
+-rw-r--r--   0        0        0      452 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_protocol.py
+-rw-r--r--   0        0        0    54414 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_scan_and_result.py
+-rw-r--r--   0        0        0     3253 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_target_convert.py
+-rw-r--r--   0        0        0     9638 2023-07-10 07:32:16.020343 ospd_openvas-22.5.2/tests/test_vthelper.py
+-rw-r--r--   0        0        0     4896 2023-07-10 07:32:16.024343 ospd_openvas-22.5.2/tests/test_vts.py
+-rw-r--r--   0        0        0    14396 2023-07-10 07:32:16.024343 ospd_openvas-22.5.2/tests/test_xml.py
+-rw-r--r--   0        0        0      373 2023-07-10 07:32:16.024343 ospd_openvas-22.5.2/tests/testing.conf
+-rw-r--r--   0        0        0     6207 1970-01-01 00:00:00.000000 ospd_openvas-22.5.2/PKG-INFO
```

### Comparing `ospd_openvas-22.5.1/CHANGELOG.md` & `ospd_openvas-22.5.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.1/COPYING` & `ospd_openvas-22.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.1/README.md` & `ospd_openvas-22.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.1/config/ospd-openvas.service` & `ospd_openvas-22.5.2/config/ospd-openvas.service`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.1/docs/ospd-openvas.8` & `ospd_openvas-22.5.2/docs/ospd-openvas.8`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.5.1/ospd/command/command.py` & `ospd_openvas-22.5.2/ospd/command/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import multiprocessing
 import re
 import logging
 import subprocess
 
 from decimal import Decimal
```

### Comparing `ospd_openvas-22.5.1/ospd/cvss.py` & `ospd_openvas-22.5.2/ospd/cvss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Common Vulnerability Scoring System handling class. """
 
 import logging
 
 import math
 from typing import List, Dict, Optional
```

### Comparing `ospd_openvas-22.5.1/ospd/errors.py` & `ospd_openvas-22.5.2/ospd/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ OSP class for handling errors.
 """
 
 from ospd.xml import simple_response_str
```

### Comparing `ospd_openvas-22.5.1/ospd/main.py` & `ospd_openvas-22.5.2/ospd/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 
 import os
 import sys
 import atexit
 import signal
```

### Comparing `ospd_openvas-22.5.1/ospd/misc.py` & `ospd_openvas-22.5.2/ospd/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable=too-many-lines
 
 """ Miscellaneous classes and functions related to OSPD.
 """
 
 import logging
```

### Comparing `ospd_openvas-22.5.1/ospd/network.py` & `ospd_openvas-22.5.2/ospd/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Helper module for network related functions
 """
 
 import binascii
 import collections
 import itertools
```

### Comparing `ospd_openvas-22.5.1/ospd/ospd.py` & `ospd_openvas-22.5.2/ospd/ospd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable=too-many-lines
 
 """ OSP Daemon core class.
 """
 
 import logging
```

### Comparing `ospd_openvas-22.5.1/ospd/parser.py` & `ospd_openvas-22.5.2/ospd/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import logging
 from pathlib import Path
 
 from ospd.config import Config
```

### Comparing `ospd_openvas-22.5.1/ospd/protocol.py` & `ospd_openvas-22.5.2/ospd/protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Helper classes for parsing and creating OSP XML requests and responses
 """
 
 from typing import Dict, Union, List, Any
 
 from xml.etree.ElementTree import SubElement, Element, XMLPullParser
```

### Comparing `ospd_openvas-22.5.1/ospd/scan.py` & `ospd_openvas-22.5.2/ospd/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import multiprocessing
 import time
 import uuid
 
 from pprint import pformat
```

### Comparing `ospd_openvas-22.5.1/ospd/server.py` & `ospd_openvas-22.5.2/ospd/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 Module for serving and streaming data
 """
 
 import logging
 import socket
```

### Comparing `ospd_openvas-22.5.1/ospd/vtfilter.py` & `ospd_openvas-22.5.2/ospd/vtfilter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Vulnerability Test Filter class.
 """
 import re
 import operator
 from typing import Dict, List, Optional
```

### Comparing `ospd_openvas-22.5.1/ospd/vts.py` & `ospd_openvas-22.5.2/ospd/vts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Classes for storing VTs
 """
 import logging
 import multiprocessing
 from hashlib import sha256
 import re
```

### Comparing `ospd_openvas-22.5.1/ospd/xml.py` & `ospd_openvas-22.5.2/ospd/xml.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ OSP XML utils class.
 """
 
 import re
 
 from typing import List, Dict, Any, Union
```

### Comparing `ospd_openvas-22.5.1/ospd/xmlvt.py` & `ospd_openvas-22.5.2/ospd/xmlvt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ OSP XML utils class for VTs.
 """
 import logging
 
 from typing import List, Dict, Optional
 from lxml.etree import Element, SubElement, tostring
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/daemon.py` & `ospd_openvas-22.5.2/ospd_openvas/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
-
 
 # pylint: disable=too-many-lines
 
 """ Setup for the OSP OpenVAS Server. """
 
 import logging
 import time
 import copy
 
 from typing import Optional, Dict, List, Tuple, Iterator, Any
 from datetime import datetime
 
 from pathlib import Path
-from os import geteuid, environ
+from os import geteuid
 
 import psutil
 
 from ospd.ospd import OSPDaemon
 from ospd.scan import ScanProgress, ScanStatus
 from ospd.server import BaseServer
 from ospd.main import main as daemon_main
@@ -50,26 +36,14 @@
 from ospd_openvas.db import MainDB, BaseDB
 from ospd_openvas.lock import LockFile
 from ospd_openvas.preferencehandler import PreferenceHandler
 from ospd_openvas.openvas import NASLCli, Openvas
 from ospd_openvas.vthelper import VtHelper
 from ospd_openvas.messaging.mqtt import MQTTClient, MQTTDaemon, MQTTSubscriber
 
-SENTRY_DSN_OSPD_OPENVAS = environ.get("SENTRY_DSN_OSPD_OPENVAS")
-if SENTRY_DSN_OSPD_OPENVAS:
-    # pylint: disable=import-error
-    import sentry_sdk
-
-    sentry_sdk.init(  # pylint: disable=abstract-class-instantiated
-        SENTRY_DSN_OSPD_OPENVAS,
-        traces_sample_rate=1.0,
-        server_name=environ.get('SENTRY_SERVER_NAME'),
-        environment=environ.get('SENTRY_ENVIRONMENT'),
-    )
-
 logger = logging.getLogger(__name__)
 
 
 OSPD_DESC = """
 This scanner runs OpenVAS to scan the target hosts.
 
 OpenVAS (Open Vulnerability Assessment Scanner) is a powerful scanner
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/db.py` & `ospd_openvas-22.5.2/ospd_openvas/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 """ Access management for redis-based OpenVAS Scanner Database."""
 import logging
 import sys
 import time
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/dryrun.py` & `ospd_openvas-22.5.2/ospd_openvas/dryrun.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2021 Greenbone AG
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
-
 
 # pylint: disable=too-many-lines
 
 """ Methods for dry run """
 
 import logging
 import time
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/gpg_sha_verifier.py` & `ospd_openvas-22.5.2/ospd_openvas/gpg_sha_verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
+#
+# SPDX-License-Identifier: AGPL-3.0-or-later
+
 import hashlib
 import os
 import logging
 from pathlib import Path
 from typing import Callable, Dict, Optional
 
 from dataclasses import dataclass
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/messages/result.py` & `ospd_openvas-22.5.2/ospd_openvas/messages/result.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
 from enum import Enum
 from typing import Dict, Union, Any, Optional
 from uuid import UUID
 
 from .message import Message, MessageType
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/messaging/mqtt.py` & `ospd_openvas-22.5.2/ospd_openvas/messaging/mqtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import json
 import logging
 
 from functools import partial
 from socket import gaierror, timeout
 from threading import Thread
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/notus.py` & `ospd_openvas-22.5.2/ospd_openvas/notus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from time import sleep
 from typing import Any, Dict, Iterator, Optional, Callable, Tuple
 from threading import Timer
 import json
 import logging
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/nvticache.py` & `ospd_openvas-22.5.2/ospd_openvas/nvticache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
-
 
 """ Provide functions to handle NVT Info Cache. """
 
 import logging
 
 from typing import List, Dict, Optional, Iterator, Tuple
 from pathlib import Path
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/openvas.py` & `ospd_openvas-22.5.2/ospd_openvas/openvas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Optional, Dict, Any
 
 import logging
 import subprocess
 import psutil
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/preferencehandler.py` & `ospd_openvas-22.5.2/ospd_openvas/preferencehandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
-
 
 # pylint: disable=too-many-lines
 
 """ Prepare the preferences to be used by OpenVAS. Get the data from the scan
 collection and store the data in a redis KB in the right format to be used by
 OpenVAS. """
```

### Comparing `ospd_openvas-22.5.1/ospd_openvas/vthelper.py` & `ospd_openvas-22.5.2/ospd_openvas/vthelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
-
 
 """ Provide functions to handle VT Info. """
 
 from hashlib import sha256
 import logging
 from typing import Any, Optional, Dict, List, Tuple, Iterator
 from itertools import chain
```

### Comparing `ospd_openvas-22.5.1/poetry.lock` & `ospd_openvas-22.5.2/poetry.lock`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
 
 [[package]]
 name = "anyio"
 version = "3.6.2"
 description = "High level compatibility layer for multiple asynchronous event loop implementations"
-category = "dev"
 optional = false
 python-versions = ">=3.6.2"
 files = [
     {file = "anyio-3.6.2-py3-none-any.whl", hash = "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"},
     {file = "anyio-3.6.2.tar.gz", hash = "sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421"},
 ]
 
@@ -22,15 +21,14 @@
 test = ["contextlib2", "coverage[toml] (>=4.5)", "hypothesis (>=4.0)", "mock (>=4)", "pytest (>=7.0)", "pytest-mock (>=3.6.1)", "trustme", "uvloop (<0.15)", "uvloop (>=0.15)"]
 trio = ["trio (>=0.16,<0.22)"]
 
 [[package]]
 name = "astroid"
 version = "2.11.7"
 description = "An abstract syntax tree for Python with inference support."
-category = "dev"
 optional = false
 python-versions = ">=3.6.2"
 files = [
     {file = "astroid-2.11.7-py3-none-any.whl", hash = "sha256:86b0a340a512c65abf4368b80252754cda17c02cdbbd3f587dddf98112233e7b"},
     {file = "astroid-2.11.7.tar.gz", hash = "sha256:bb24615c77f4837c707669d16907331374ae8a964650a66999da3f5ca68dc946"},
 ]
 
@@ -41,30 +39,28 @@
 typing-extensions = {version = ">=3.10", markers = "python_version < \"3.10\""}
 wrapt = ">=1.11,<2"
 
 [[package]]
 name = "async-timeout"
 version = "4.0.2"
 description = "Timeout context manager for asyncio programs"
-category = "main"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "async-timeout-4.0.2.tar.gz", hash = "sha256:2163e1640ddb52b7a8c80d0a67a08587e5d245cc9c553a74a847056bc2976b15"},
     {file = "async_timeout-4.0.2-py3-none-any.whl", hash = "sha256:8ca1e4fcf50d07413d66d1a5e416e42cfdf5851c981d679a09851a6853383b3c"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = ">=3.6.5", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "autohooks"
 version = "23.1.0"
 description = "Library for managing git hooks"
-category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
     {file = "autohooks-23.1.0-py3-none-any.whl", hash = "sha256:bff89af36bc2a442a4d6198b7dbf4c6cc204b1b35c4a8d51e3c30e6bd12224bd"},
     {file = "autohooks-23.1.0.tar.gz", hash = "sha256:bf9da5e9155676edde49c795b7ad4bf3b4322da3ee9c9358811a2b497eb811c7"},
 ]
 
@@ -73,15 +69,14 @@
 rich = ">=12.5.1"
 tomlkit = ">=0.5.11"
 
 [[package]]
 name = "autohooks-plugin-black"
 version = "22.11.0"
 description = "An autohooks plugin for python code formatting via black"
-category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
     {file = "autohooks_plugin_black-22.11.0-py3-none-any.whl", hash = "sha256:e2fd93f1b8995c963356114dafa21ededbcb81f9f6273887a82f26bca5342fe7"},
     {file = "autohooks_plugin_black-22.11.0.tar.gz", hash = "sha256:c67cfe2a5c008b5596d109a5384c48aa9421a00cf0b49a67c1f380c6fe55155b"},
 ]
 
@@ -89,15 +84,14 @@
 autohooks = ">=21.6.0"
 black = ">=20.8"
 
 [[package]]
 name = "autohooks-plugin-pylint"
 version = "22.8.1"
 description = "An autohooks plugin for python code linting via pylint"
-category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
     {file = "autohooks-plugin-pylint-22.8.1.tar.gz", hash = "sha256:d348a61b2b027ad51275dace830ec3643cf14416519eb68167a4bdadfe44ac7e"},
     {file = "autohooks_plugin_pylint-22.8.1-py3-none-any.whl", hash = "sha256:a7195e0f6a568cd8e0e4a964ebcecf2eb4e457a17a8b3dbc6283dfc546a474c2"},
 ]
 
@@ -105,15 +99,14 @@
 autohooks = ">=2.2.0"
 pylint = ">=2.8.3,<3.0.0"
 
 [[package]]
 name = "black"
 version = "23.3.0"
 description = "The uncompromising code formatter."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
     {file = "black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
@@ -154,29 +147,27 @@
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "certifi"
-version = "2022.12.7"
+version = "2023.5.7"
 description = "Python package for providing Mozilla's CA Bundle."
-category = "main"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "certifi-2022.12.7-py3-none-any.whl", hash = "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"},
-    {file = "certifi-2022.12.7.tar.gz", hash = "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3"},
+    {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
+    {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
 ]
 
 [[package]]
 name = "click"
 version = "8.1.3"
 description = "Composable command line interface toolkit"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
     {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
 ]
 
@@ -184,102 +175,95 @@
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
-category = "dev"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "colorful"
 version = "0.5.5"
 description = "Terminal string styling done right, in Python."
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "colorful-0.5.5-py2.py3-none-any.whl", hash = "sha256:62c187e27c1433db9463ff93b1451898d1e7e23a7e553583fd9daeb6325182e4"},
     {file = "colorful-0.5.5.tar.gz", hash = "sha256:66f8c1264b2a26f7293b96a03bb7a76c4bc8b9634369a0bffdcd12d618056a1d"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "defusedxml"
 version = "0.7.1"
 description = "XML bomb protection for Python stdlib modules"
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 files = [
     {file = "defusedxml-0.7.1-py2.py3-none-any.whl", hash = "sha256:a352e7e428770286cc899e2542b6cdaedb2b4953ff269a210103ec58f6198a61"},
     {file = "defusedxml-0.7.1.tar.gz", hash = "sha256:1bb3032db185915b62d7c6209c5a8792be6a32ab2fedacc84e01b52c51aa3e69"},
 ]
 
 [[package]]
 name = "deprecated"
-version = "1.2.13"
+version = "1.2.14"
 description = "Python @deprecated decorator to deprecate old python classes, functions or methods."
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
-    {file = "Deprecated-1.2.13-py2.py3-none-any.whl", hash = "sha256:64756e3e14c8c5eea9795d93c524551432a0be75629f8f29e67ab8caf076c76d"},
-    {file = "Deprecated-1.2.13.tar.gz", hash = "sha256:43ac5335da90c31c24ba028af536a91d41d53f9e6901ddb021bcc572ce44e38d"},
+    {file = "Deprecated-1.2.14-py2.py3-none-any.whl", hash = "sha256:6fac8b097794a90302bdbb17b9b815e732d3c4720583ff1b198499d78470466c"},
+    {file = "Deprecated-1.2.14.tar.gz", hash = "sha256:e5323eb936458dccc2582dc6f9c322c852a775a27065ff2b0c4970b9d53d01b3"},
 ]
 
 [package.dependencies]
 wrapt = ">=1.10,<2"
 
 [package.extras]
-dev = ["PyTest", "PyTest (<5)", "PyTest-Cov", "PyTest-Cov (<2.6)", "bump2version (<1)", "configparser (<5)", "importlib-metadata (<3)", "importlib-resources (<4)", "sphinx (<2)", "sphinxcontrib-websupport (<2)", "tox", "zipp (<2)"]
+dev = ["PyTest", "PyTest-Cov", "bump2version (<1)", "sphinx (<2)", "tox"]
 
 [[package]]
 name = "dill"
 version = "0.3.6"
 description = "serialize all of python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "dill-0.3.6-py3-none-any.whl", hash = "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0"},
     {file = "dill-0.3.6.tar.gz", hash = "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"},
 ]
 
 [package.extras]
 graph = ["objgraph (>=1.7.2)"]
 
 [[package]]
 name = "h11"
 version = "0.14.0"
 description = "A pure-Python, bring-your-own-I/O implementation of HTTP/1.1"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "h11-0.14.0-py3-none-any.whl", hash = "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"},
     {file = "h11-0.14.0.tar.gz", hash = "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = "*", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "h2"
 version = "4.1.0"
 description = "HTTP/2 State-Machine based protocol implementation"
-category = "dev"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "h2-4.1.0-py3-none-any.whl", hash = "sha256:03a46bcf682256c95b5fd9e9a99c1323584c3eec6440d379b9903d709476bc6d"},
     {file = "h2-4.1.0.tar.gz", hash = "sha256:a83aca08fbe7aacb79fec788c9c0bac936343560ed9ec18b82a13a12c28d2abb"},
 ]
 
@@ -287,49 +271,46 @@
 hpack = ">=4.0,<5"
 hyperframe = ">=6.0,<7"
 
 [[package]]
 name = "hpack"
 version = "4.0.0"
 description = "Pure-Python HPACK header compression"
-category = "dev"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "hpack-4.0.0-py3-none-any.whl", hash = "sha256:84a076fad3dc9a9f8063ccb8041ef100867b1878b25ef0ee63847a5d53818a6c"},
     {file = "hpack-4.0.0.tar.gz", hash = "sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095"},
 ]
 
 [[package]]
 name = "httpcore"
 version = "0.16.3"
 description = "A minimal low-level HTTP client."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "httpcore-0.16.3-py3-none-any.whl", hash = "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"},
     {file = "httpcore-0.16.3.tar.gz", hash = "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb"},
 ]
 
 [package.dependencies]
 anyio = ">=3.0,<5.0"
 certifi = "*"
 h11 = ">=0.13,<0.15"
-sniffio = ">=1.0.0,<2.0.0"
+sniffio = "==1.*"
 
 [package.extras]
 http2 = ["h2 (>=3,<5)"]
-socks = ["socksio (>=1.0.0,<2.0.0)"]
+socks = ["socksio (==1.*)"]
 
 [[package]]
 name = "httpx"
 version = "0.23.3"
 description = "The next generation HTTP client."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "httpx-0.23.3-py3-none-any.whl", hash = "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"},
     {file = "httpx-0.23.3.tar.gz", hash = "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9"},
 ]
 
@@ -338,52 +319,49 @@
 h2 = {version = ">=3,<5", optional = true, markers = "extra == \"http2\""}
 httpcore = ">=0.15.0,<0.17.0"
 rfc3986 = {version = ">=1.3,<2", extras = ["idna2008"]}
 sniffio = "*"
 
 [package.extras]
 brotli = ["brotli", "brotlicffi"]
-cli = ["click (>=8.0.0,<9.0.0)", "pygments (>=2.0.0,<3.0.0)", "rich (>=10,<13)"]
+cli = ["click (==8.*)", "pygments (==2.*)", "rich (>=10,<13)"]
 http2 = ["h2 (>=3,<5)"]
-socks = ["socksio (>=1.0.0,<2.0.0)"]
+socks = ["socksio (==1.*)"]
 
 [[package]]
 name = "hyperframe"
 version = "6.0.1"
 description = "HTTP/2 framing layer for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "hyperframe-6.0.1-py3-none-any.whl", hash = "sha256:0ec6bafd80d8ad2195c4f03aacba3a8265e57bc4cff261e802bf39970ed02a15"},
     {file = "hyperframe-6.0.1.tar.gz", hash = "sha256:ae510046231dc8e9ecb1a6586f63d2347bf4c8905914aa84ba585ae85f28a914"},
 ]
 
 [[package]]
 name = "idna"
 version = "3.4"
 description = "Internationalized Domain Names in Applications (IDNA)"
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
     {file = "idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.0.0"
+version = "6.6.0"
 description = "Read metadata from Python packages"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "importlib_metadata-6.0.0-py3-none-any.whl", hash = "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad"},
-    {file = "importlib_metadata-6.0.0.tar.gz", hash = "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"},
+    {file = "importlib_metadata-6.6.0-py3-none-any.whl", hash = "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed"},
+    {file = "importlib_metadata-6.6.0.tar.gz", hash = "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
 zipp = ">=0.5"
 
 [package.extras]
@@ -391,15 +369,14 @@
 perf = ["ipython"]
 testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
 
 [[package]]
 name = "isort"
 version = "5.11.5"
 description = "A Python utility / library to sort Python imports."
-category = "dev"
 optional = false
 python-versions = ">=3.7.0"
 files = [
     {file = "isort-5.11.5-py3-none-any.whl", hash = "sha256:ba1d72fb2595a01c7895a5128f9585a5cc4b6d395f1c8d514989b9a7eb2a8746"},
     {file = "isort-5.11.5.tar.gz", hash = "sha256:6be1f76a507cb2ecf16c7cf14a37e41609ca082330be4e3436a18ef74add55db"},
 ]
 
@@ -409,15 +386,14 @@
 plugins = ["setuptools"]
 requirements-deprecated-finder = ["pip-api", "pipreqs"]
 
 [[package]]
 name = "lazy-object-proxy"
 version = "1.9.0"
 description = "A fast and thorough lazy object proxy."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "lazy-object-proxy-1.9.0.tar.gz", hash = "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae"},
     {file = "lazy_object_proxy-1.9.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7"},
     {file = "lazy_object_proxy-1.9.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4"},
     {file = "lazy_object_proxy-1.9.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd"},
@@ -455,15 +431,14 @@
     {file = "lazy_object_proxy-1.9.0-cp39-cp39-win_amd64.whl", hash = "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f"},
 ]
 
 [[package]]
 name = "lxml"
 version = "4.9.2"
 description = "Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API."
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*"
 files = [
     {file = "lxml-4.9.2-cp27-cp27m-macosx_10_15_x86_64.whl", hash = "sha256:76cf573e5a365e790396a5cc2b909812633409306c6531a6877c59061e42c4f2"},
     {file = "lxml-4.9.2-cp27-cp27m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b1f42b6921d0e81b1bcb5e395bc091a70f41c4d4e55ba99c6da2b31626c44892"},
     {file = "lxml-4.9.2-cp27-cp27m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:9f102706d0ca011de571de32c3247c6476b55bb6bc65a20f682f000b07a4852a"},
     {file = "lxml-4.9.2-cp27-cp27m-win32.whl", hash = "sha256:8d0b4612b66ff5d62d03bcaa043bb018f74dfea51184e53f067e6fdcba4bd8de"},
@@ -548,15 +523,14 @@
 htmlsoup = ["BeautifulSoup4"]
 source = ["Cython (>=0.29.7)"]
 
 [[package]]
 name = "markdown-it-py"
 version = "2.2.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
     {file = "markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
 ]
 
@@ -574,108 +548,100 @@
 rtd = ["attrs", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
 testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
 
 [[package]]
 name = "mccabe"
 version = "0.7.0"
 description = "McCabe checker, plugin for flake8"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
 name = "mdurl"
 version = "0.1.2"
 description = "Markdown URL utilities"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
     {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
 ]
 
 [[package]]
 name = "mypy-extensions"
-version = "0.4.3"
-description = "Experimental type system extensions for programs checked with the mypy typechecker."
-category = "dev"
+version = "1.0.0"
+description = "Type system extensions for programs checked with the mypy type checker."
 optional = false
-python-versions = "*"
+python-versions = ">=3.5"
 files = [
-    {file = "mypy_extensions-0.4.3-py2.py3-none-any.whl", hash = "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d"},
-    {file = "mypy_extensions-0.4.3.tar.gz", hash = "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"},
+    {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
+    {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "packaging"
 version = "23.1"
 description = "Core utilities for Python packages"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "paho-mqtt"
 version = "1.6.1"
 description = "MQTT version 5.0/3.1.1 client class"
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "paho-mqtt-1.6.1.tar.gz", hash = "sha256:2a8291c81623aec00372b5a85558a372c747cbca8e9934dfe218638b8eefc26f"},
 ]
 
 [package.extras]
 proxy = ["PySocks"]
 
 [[package]]
 name = "pathspec"
-version = "0.11.0"
+version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "pathspec-0.11.0-py3-none-any.whl", hash = "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229"},
-    {file = "pathspec-0.11.0.tar.gz", hash = "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"},
+    {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
+    {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "2.6.2"
+version = "3.5.1"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-2.6.2-py3-none-any.whl", hash = "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490"},
-    {file = "platformdirs-2.6.2.tar.gz", hash = "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"},
+    {file = "platformdirs-3.5.1-py3-none-any.whl", hash = "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"},
+    {file = "platformdirs-3.5.1.tar.gz", hash = "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f"},
 ]
 
 [package.dependencies]
-typing-extensions = {version = ">=4.4", markers = "python_version < \"3.8\""}
+typing-extensions = {version = ">=4.5", markers = "python_version < \"3.8\""}
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2023.3.27)", "proselint (>=0.13)", "sphinx (>=6.2.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pontos"
 version = "23.3.5"
 description = "Common utilities and tools maintained by Greenbone Networks"
-category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
     {file = "pontos-23.3.5-py3-none-any.whl", hash = "sha256:b82c6165c8d73ce66e234945ed52104b1895215e3dedac0fecee5326035a0df8"},
     {file = "pontos-23.3.5.tar.gz", hash = "sha256:f19f42718faa20af54096fe88a9210f285e89b7586ffeca665ad49c9e3c7ae69"},
 ]
 
@@ -689,15 +655,14 @@
 tomlkit = ">=0.5.11"
 typing-extensions = {version = ">=4.4.0,<5.0.0", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "psutil"
 version = "5.9.5"
 description = "Cross-platform lib for process and system monitoring in Python."
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
     {file = "psutil-5.9.5-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:be8929ce4313f9f8146caad4272f6abb8bf99fc6cf59344a3167ecd74f4f203f"},
     {file = "psutil-5.9.5-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ab8ed1a1d77c95453db1ae00a3f9c50227ebd955437bcf2a574ba8adbf6a74d5"},
     {file = "psutil-5.9.5-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:4aef137f3345082a3d3232187aeb4ac4ef959ba3d7c10c33dd73763fbc063da4"},
     {file = "psutil-5.9.5-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:ea8518d152174e1249c4f2a1c89e3e6065941df2fa13a1ab45327716a23c2b48"},
@@ -714,32 +679,30 @@
 ]
 
 [package.extras]
 test = ["enum34", "ipaddress", "mock", "pywin32", "wmi"]
 
 [[package]]
 name = "pygments"
-version = "2.14.0"
+version = "2.15.1"
 description = "Pygments is a syntax highlighting package written in Python."
-category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "Pygments-2.14.0-py3-none-any.whl", hash = "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"},
-    {file = "Pygments-2.14.0.tar.gz", hash = "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297"},
+    {file = "Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
+    {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pylint"
 version = "2.13.9"
 description = "python code static checker"
-category = "dev"
 optional = false
 python-versions = ">=3.6.2"
 files = [
     {file = "pylint-2.13.9-py3-none-any.whl", hash = "sha256:705c620d388035bdd9ff8b44c5bcdd235bfb49d276d488dd2c8ff1736aa42526"},
     {file = "pylint-2.13.9.tar.gz", hash = "sha256:095567c96e19e6f57b5b907e67d265ff535e588fe26b12b5ebe1fc5645b2c731"},
 ]
 
@@ -756,42 +719,39 @@
 [package.extras]
 testutil = ["gitpython (>3)"]
 
 [[package]]
 name = "python-dateutil"
 version = "2.8.2"
 description = "Extensions to the standard Python datetime module"
-category = "dev"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 files = [
     {file = "python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
     {file = "python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
 ]
 
 [package.dependencies]
 six = ">=1.5"
 
 [[package]]
 name = "python-gnupg"
 version = "0.5.0"
 description = "A wrapper for the Gnu Privacy Guard (GPG or GnuPG)"
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "python-gnupg-0.5.0.tar.gz", hash = "sha256:70758e387fc0e0c4badbcb394f61acbe68b34970a8fed7e0f7c89469fe17912a"},
     {file = "python_gnupg-0.5.0-py2.py3-none-any.whl", hash = "sha256:345723a03e67b82aba0ea8ae2328b2e4a3906fbe2c18c4082285c3b01068f270"},
 ]
 
 [[package]]
 name = "pytoolconfig"
 version = "1.2.5"
 description = "Python tool configuration"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytoolconfig-1.2.5-py3-none-any.whl", hash = "sha256:239ba9d3e537b91d0243275a497700ea39a5e259ddb80421c366e3b288bf30fe"},
     {file = "pytoolconfig-1.2.5.tar.gz", hash = "sha256:a50f9dfe23b03a9d40414c1fdf902fefbeae12f2ac75a3c8f915944d6ffac279"},
 ]
 
@@ -805,38 +765,36 @@
 doc = ["sphinx (>=4.5.0)", "tabulate (>=0.8.9)"]
 gendocs = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
 global = ["platformdirs (>=1.4.4)"]
 validation = ["pydantic (>=1.7.4)"]
 
 [[package]]
 name = "redis"
-version = "4.5.4"
+version = "4.6.0"
 description = "Python client for Redis database and key-value store"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "redis-4.5.4-py3-none-any.whl", hash = "sha256:2c19e6767c474f2e85167909061d525ed65bea9301c0770bb151e041b7ac89a2"},
-    {file = "redis-4.5.4.tar.gz", hash = "sha256:73ec35da4da267d6847e47f68730fdd5f62e2ca69e3ef5885c6a78a9374c3893"},
+    {file = "redis-4.6.0-py3-none-any.whl", hash = "sha256:e2b03db868160ee4591de3cb90d40ebb50a90dd302138775937f6a42b7ed183c"},
+    {file = "redis-4.6.0.tar.gz", hash = "sha256:585dc516b9eb042a619ef0a39c3d7d55fe81bdb4df09a52c9cdde0d07bf1aa7d"},
 ]
 
 [package.dependencies]
-async-timeout = {version = ">=4.0.2", markers = "python_version <= \"3.11.2\""}
+async-timeout = {version = ">=4.0.2", markers = "python_full_version <= \"3.11.2\""}
 importlib-metadata = {version = ">=1.0", markers = "python_version < \"3.8\""}
 typing-extensions = {version = "*", markers = "python_version < \"3.8\""}
 
 [package.extras]
 hiredis = ["hiredis (>=1.0.0)"]
 ocsp = ["cryptography (>=36.0.1)", "pyopenssl (==20.0.1)", "requests (>=2.26.0)"]
 
 [[package]]
 name = "rfc3986"
 version = "1.5.0"
 description = "Validating URI References per RFC 3986"
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "rfc3986-1.5.0-py2.py3-none-any.whl", hash = "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"},
     {file = "rfc3986-1.5.0.tar.gz", hash = "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835"},
 ]
 
@@ -844,175 +802,125 @@
 idna = {version = "*", optional = true, markers = "extra == \"idna2008\""}
 
 [package.extras]
 idna2008 = ["idna"]
 
 [[package]]
 name = "rich"
-version = "13.3.1"
+version = "13.3.5"
 description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
-category = "dev"
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "rich-13.3.1-py3-none-any.whl", hash = "sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9"},
-    {file = "rich-13.3.1.tar.gz", hash = "sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f"},
+    {file = "rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
+    {file = "rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
 ]
 
 [package.dependencies]
-markdown-it-py = ">=2.1.0,<3.0.0"
-pygments = ">=2.14.0,<3.0.0"
+markdown-it-py = ">=2.2.0,<3.0.0"
+pygments = ">=2.13.0,<3.0.0"
 typing-extensions = {version = ">=4.0.0,<5.0", markers = "python_version < \"3.9\""}
 
 [package.extras]
 jupyter = ["ipywidgets (>=7.5.1,<9)"]
 
 [[package]]
 name = "rope"
-version = "1.8.0"
+version = "1.9.0"
 description = "a python refactoring library..."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "rope-1.8.0-py3-none-any.whl", hash = "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd"},
-    {file = "rope-1.8.0.tar.gz", hash = "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"},
+    {file = "rope-1.9.0-py3-none-any.whl", hash = "sha256:2ed32d72cd2c4395bb1d569e38fd4f15d6080cfadd61b6e5c565fd39e3f677aa"},
+    {file = "rope-1.9.0.tar.gz", hash = "sha256:f48d708132c0e062b411308732ca13933b976486b4b53d1e804f94ed08d69503"},
 ]
 
 [package.dependencies]
 pytoolconfig = {version = ">=1.2.2", extras = ["global"]}
 
 [package.extras]
-dev = ["build (>=0.7.0)", "pip-tools (>=6.12.1)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)", "toml (>=0.10.2)"]
+dev = ["build (>=0.7.0)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)"]
 doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
+release = ["pip-tools (>=6.12.1)", "toml (>=0.10.2)", "twine (>=4.0.2)"]
 
 [[package]]
 name = "semver"
 version = "2.13.0"
 description = "Python helper for Semantic Versioning (http://semver.org/)"
-category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
     {file = "semver-2.13.0-py2.py3-none-any.whl", hash = "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4"},
     {file = "semver-2.13.0.tar.gz", hash = "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"},
 ]
 
 [[package]]
-name = "sentry-sdk"
-version = "1.22.1"
-description = "Python client for Sentry (https://sentry.io)"
-category = "main"
-optional = true
-python-versions = "*"
-files = [
-    {file = "sentry-sdk-1.22.1.tar.gz", hash = "sha256:052dff5069c6f0d836ee014323576824a9b40836fc003fb12489a1f19c60a3c9"},
-    {file = "sentry_sdk-1.22.1-py2.py3-none-any.whl", hash = "sha256:c6c6946f8c927adb00af1c5ab6921df38775b2199b9003816d5935a1310352d5"},
-]
-
-[package.dependencies]
-certifi = "*"
-urllib3 = {version = ">=1.26.11,<2.0.0", markers = "python_version >= \"3.6\""}
-
-[package.extras]
-aiohttp = ["aiohttp (>=3.5)"]
-arq = ["arq (>=0.23)"]
-beam = ["apache-beam (>=2.12)"]
-bottle = ["bottle (>=0.12.13)"]
-celery = ["celery (>=3)"]
-chalice = ["chalice (>=1.16.0)"]
-django = ["django (>=1.8)"]
-falcon = ["falcon (>=1.4)"]
-fastapi = ["fastapi (>=0.79.0)"]
-flask = ["blinker (>=1.1)", "flask (>=0.11)"]
-grpcio = ["grpcio (>=1.21.1)"]
-httpx = ["httpx (>=0.16.0)"]
-huey = ["huey (>=2)"]
-opentelemetry = ["opentelemetry-distro (>=0.35b0)"]
-pure-eval = ["asttokens", "executing", "pure-eval"]
-pymongo = ["pymongo (>=3.1)"]
-pyspark = ["pyspark (>=2.4.4)"]
-quart = ["blinker (>=1.1)", "quart (>=0.16.1)"]
-rq = ["rq (>=0.6)"]
-sanic = ["sanic (>=0.8)"]
-sqlalchemy = ["sqlalchemy (>=1.2)"]
-starlette = ["starlette (>=0.19.1)"]
-starlite = ["starlite (>=1.48)"]
-tornado = ["tornado (>=5)"]
-
-[[package]]
 name = "setuptools"
-version = "67.1.0"
+version = "67.8.0"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "setuptools-67.1.0-py3-none-any.whl", hash = "sha256:a7687c12b444eaac951ea87a9627c4f904ac757e7abdc5aac32833234af90378"},
-    {file = "setuptools-67.1.0.tar.gz", hash = "sha256:e261cdf010c11a41cb5cb5f1bf3338a7433832029f559a6a7614bd42a967c300"},
+    {file = "setuptools-67.8.0-py3-none-any.whl", hash = "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f"},
+    {file = "setuptools-67.8.0.tar.gz", hash = "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
-testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
+testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-ruff", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 description = "Python 2 and 3 compatibility utilities"
-category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 
 [[package]]
 name = "sniffio"
 version = "1.3.0"
 description = "Sniff out which async library your code is running under"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "sniffio-1.3.0-py3-none-any.whl", hash = "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"},
     {file = "sniffio-1.3.0.tar.gz", hash = "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101"},
 ]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tomlkit"
-version = "0.11.6"
+version = "0.11.8"
 description = "Style preserving TOML library"
-category = "dev"
 optional = false
-python-versions = ">=3.6"
+python-versions = ">=3.7"
 files = [
-    {file = "tomlkit-0.11.6-py3-none-any.whl", hash = "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b"},
-    {file = "tomlkit-0.11.6.tar.gz", hash = "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"},
+    {file = "tomlkit-0.11.8-py3-none-any.whl", hash = "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171"},
+    {file = "tomlkit-0.11.8.tar.gz", hash = "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"},
 ]
 
 [[package]]
 name = "typed-ast"
 version = "1.5.4"
 description = "a fork of Python 2 and 3 ast modules with type comment support"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "typed_ast-1.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:669dd0c4167f6f2cd9f57041e03c3c2ebf9063d0757dc89f79ba1daa2bfca9d4"},
     {file = "typed_ast-1.5.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62"},
     {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:267e3f78697a6c00c689c03db4876dd1efdfea2f251a5ad6555e82a26847b4ac"},
     {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:c542eeda69212fa10a7ada75e668876fdec5f856cd3d06829e6aa64ad17c8dfe"},
@@ -1036,131 +944,119 @@
     {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
     {file = "typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
     {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.4.0"
+version = "4.6.0"
 description = "Backported and Experimental Type Hints for Python 3.7+"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.4.0-py3-none-any.whl", hash = "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"},
-    {file = "typing_extensions-4.4.0.tar.gz", hash = "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa"},
-]
-
-[[package]]
-name = "urllib3"
-version = "1.26.14"
-description = "HTTP library with thread-safe connection pooling, file post, and more."
-category = "main"
-optional = true
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*"
-files = [
-    {file = "urllib3-1.26.14-py2.py3-none-any.whl", hash = "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"},
-    {file = "urllib3-1.26.14.tar.gz", hash = "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72"},
+    {file = "typing_extensions-4.6.0-py3-none-any.whl", hash = "sha256:6ad00b63f849b7dcc313b70b6b304ed67b2b2963b3098a33efe18056b1a9a223"},
+    {file = "typing_extensions-4.6.0.tar.gz", hash = "sha256:ff6b238610c747e44c268aa4bb23c8c735d665a63726df3f9431ce707f2aa768"},
 ]
 
-[package.extras]
-brotli = ["brotli (>=1.0.9)", "brotlicffi (>=0.8.0)", "brotlipy (>=0.6.0)"]
-secure = ["certifi", "cryptography (>=1.3.4)", "idna (>=2.0.0)", "ipaddress", "pyOpenSSL (>=0.14)", "urllib3-secure-extra"]
-socks = ["PySocks (>=1.5.6,!=1.5.7,<2.0)"]
-
 [[package]]
 name = "wrapt"
-version = "1.14.1"
+version = "1.15.0"
 description = "Module for decorators, wrappers and monkey patching."
-category = "main"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
 files = [
-    {file = "wrapt-1.14.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:1b376b3f4896e7930f1f772ac4b064ac12598d1c38d04907e696cc4d794b43d3"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:903500616422a40a98a5a3c4ff4ed9d0066f3b4c951fa286018ecdf0750194ef"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:5a9a0d155deafd9448baff28c08e150d9b24ff010e899311ddd63c45c2445e28"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:ddaea91abf8b0d13443f6dac52e89051a5063c7d014710dcb4d4abb2ff811a59"},
-    {file = "wrapt-1.14.1-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:36f582d0c6bc99d5f39cd3ac2a9062e57f3cf606ade29a0a0d6b323462f4dd87"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:7ef58fb89674095bfc57c4069e95d7a31cfdc0939e2a579882ac7d55aadfd2a1"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:e2f83e18fe2f4c9e7db597e988f72712c0c3676d337d8b101f6758107c42425b"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:ee2b1b1769f6707a8a445162ea16dddf74285c3964f605877a20e38545c3c462"},
-    {file = "wrapt-1.14.1-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:833b58d5d0b7e5b9832869f039203389ac7cbf01765639c7309fd50ef619e0b1"},
-    {file = "wrapt-1.14.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:80bb5c256f1415f747011dc3604b59bc1f91c6e7150bd7db03b19170ee06b320"},
-    {file = "wrapt-1.14.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:07f7a7d0f388028b2df1d916e94bbb40624c59b48ecc6cbc232546706fac74c2"},
-    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:02b41b633c6261feff8ddd8d11c711df6842aba629fdd3da10249a53211a72c4"},
-    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2fe803deacd09a233e4762a1adcea5db5d31e6be577a43352936179d14d90069"},
-    {file = "wrapt-1.14.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:257fd78c513e0fb5cdbe058c27a0624c9884e735bbd131935fd49e9fe719d310"},
-    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4fcc4649dc762cddacd193e6b55bc02edca674067f5f98166d7713b193932b7f"},
-    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:11871514607b15cfeb87c547a49bca19fde402f32e2b1c24a632506c0a756656"},
-    {file = "wrapt-1.14.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8ad85f7f4e20964db4daadcab70b47ab05c7c1cf2a7c1e51087bfaa83831854c"},
-    {file = "wrapt-1.14.1-cp310-cp310-win32.whl", hash = "sha256:a9a52172be0b5aae932bef82a79ec0a0ce87288c7d132946d645eba03f0ad8a8"},
-    {file = "wrapt-1.14.1-cp310-cp310-win_amd64.whl", hash = "sha256:6d323e1554b3d22cfc03cd3243b5bb815a51f5249fdcbb86fda4bf62bab9e164"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux1_i686.whl", hash = "sha256:43ca3bbbe97af00f49efb06e352eae40434ca9d915906f77def219b88e85d907"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux1_x86_64.whl", hash = "sha256:6b1a564e6cb69922c7fe3a678b9f9a3c54e72b469875aa8018f18b4d1dd1adf3"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux2010_i686.whl", hash = "sha256:00b6d4ea20a906c0ca56d84f93065b398ab74b927a7a3dbd470f6fc503f95dc3"},
-    {file = "wrapt-1.14.1-cp35-cp35m-manylinux2010_x86_64.whl", hash = "sha256:a85d2b46be66a71bedde836d9e41859879cc54a2a04fad1191eb50c2066f6e9d"},
-    {file = "wrapt-1.14.1-cp35-cp35m-win32.whl", hash = "sha256:dbcda74c67263139358f4d188ae5faae95c30929281bc6866d00573783c422b7"},
-    {file = "wrapt-1.14.1-cp35-cp35m-win_amd64.whl", hash = "sha256:b21bb4c09ffabfa0e85e3a6b623e19b80e7acd709b9f91452b8297ace2a8ab00"},
-    {file = "wrapt-1.14.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:9e0fd32e0148dd5dea6af5fee42beb949098564cc23211a88d799e434255a1f4"},
-    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9736af4641846491aedb3c3f56b9bc5568d92b0692303b5a305301a95dfd38b1"},
-    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5b02d65b9ccf0ef6c34cba6cf5bf2aab1bb2f49c6090bafeecc9cd81ad4ea1c1"},
-    {file = "wrapt-1.14.1-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21ac0156c4b089b330b7666db40feee30a5d52634cc4560e1905d6529a3897ff"},
-    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:9f3e6f9e05148ff90002b884fbc2a86bd303ae847e472f44ecc06c2cd2fcdb2d"},
-    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:6e743de5e9c3d1b7185870f480587b75b1cb604832e380d64f9504a0535912d1"},
-    {file = "wrapt-1.14.1-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:d79d7d5dc8a32b7093e81e97dad755127ff77bcc899e845f41bf71747af0c569"},
-    {file = "wrapt-1.14.1-cp36-cp36m-win32.whl", hash = "sha256:81b19725065dcb43df02b37e03278c011a09e49757287dca60c5aecdd5a0b8ed"},
-    {file = "wrapt-1.14.1-cp36-cp36m-win_amd64.whl", hash = "sha256:b014c23646a467558be7da3d6b9fa409b2c567d2110599b7cf9a0c5992b3b471"},
-    {file = "wrapt-1.14.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:88bd7b6bd70a5b6803c1abf6bca012f7ed963e58c68d76ee20b9d751c74a3248"},
-    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b5901a312f4d14c59918c221323068fad0540e34324925c8475263841dbdfe68"},
-    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d77c85fedff92cf788face9bfa3ebaa364448ebb1d765302e9af11bf449ca36d"},
-    {file = "wrapt-1.14.1-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d649d616e5c6a678b26d15ece345354f7c2286acd6db868e65fcc5ff7c24a77"},
-    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:7d2872609603cb35ca513d7404a94d6d608fc13211563571117046c9d2bcc3d7"},
-    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:ee6acae74a2b91865910eef5e7de37dc6895ad96fa23603d1d27ea69df545015"},
-    {file = "wrapt-1.14.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:2b39d38039a1fdad98c87279b48bc5dce2c0ca0d73483b12cb72aa9609278e8a"},
-    {file = "wrapt-1.14.1-cp37-cp37m-win32.whl", hash = "sha256:60db23fa423575eeb65ea430cee741acb7c26a1365d103f7b0f6ec412b893853"},
-    {file = "wrapt-1.14.1-cp37-cp37m-win_amd64.whl", hash = "sha256:709fe01086a55cf79d20f741f39325018f4df051ef39fe921b1ebe780a66184c"},
-    {file = "wrapt-1.14.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8c0ce1e99116d5ab21355d8ebe53d9460366704ea38ae4d9f6933188f327b456"},
-    {file = "wrapt-1.14.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e3fb1677c720409d5f671e39bac6c9e0e422584e5f518bfd50aa4cbbea02433f"},
-    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:642c2e7a804fcf18c222e1060df25fc210b9c58db7c91416fb055897fc27e8cc"},
-    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7b7c050ae976e286906dd3f26009e117eb000fb2cf3533398c5ad9ccc86867b1"},
-    {file = "wrapt-1.14.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef3f72c9666bba2bab70d2a8b79f2c6d2c1a42a7f7e2b0ec83bb2f9e383950af"},
-    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:01c205616a89d09827986bc4e859bcabd64f5a0662a7fe95e0d359424e0e071b"},
-    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:5a0f54ce2c092aaf439813735584b9537cad479575a09892b8352fea5e988dc0"},
-    {file = "wrapt-1.14.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2cf71233a0ed05ccdabe209c606fe0bac7379fdcf687f39b944420d2a09fdb57"},
-    {file = "wrapt-1.14.1-cp38-cp38-win32.whl", hash = "sha256:aa31fdcc33fef9eb2552cbcbfee7773d5a6792c137b359e82879c101e98584c5"},
-    {file = "wrapt-1.14.1-cp38-cp38-win_amd64.whl", hash = "sha256:d1967f46ea8f2db647c786e78d8cc7e4313dbd1b0aca360592d8027b8508e24d"},
-    {file = "wrapt-1.14.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3232822c7d98d23895ccc443bbdf57c7412c5a65996c30442ebe6ed3df335383"},
-    {file = "wrapt-1.14.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:988635d122aaf2bdcef9e795435662bcd65b02f4f4c1ae37fbee7401c440b3a7"},
-    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9cca3c2cdadb362116235fdbd411735de4328c61425b0aa9f872fd76d02c4e86"},
-    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d52a25136894c63de15a35bc0bdc5adb4b0e173b9c0d07a2be9d3ca64a332735"},
-    {file = "wrapt-1.14.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40e7bc81c9e2b2734ea4bc1aceb8a8f0ceaac7c5299bc5d69e37c44d9081d43b"},
-    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b9b7a708dd92306328117d8c4b62e2194d00c365f18eff11a9b53c6f923b01e3"},
-    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:6a9a25751acb379b466ff6be78a315e2b439d4c94c1e99cb7266d40a537995d3"},
-    {file = "wrapt-1.14.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:34aa51c45f28ba7f12accd624225e2b1e5a3a45206aa191f6f9aac931d9d56fe"},
-    {file = "wrapt-1.14.1-cp39-cp39-win32.whl", hash = "sha256:dee0ce50c6a2dd9056c20db781e9c1cfd33e77d2d569f5d1d9321c641bb903d5"},
-    {file = "wrapt-1.14.1-cp39-cp39-win_amd64.whl", hash = "sha256:dee60e1de1898bde3b238f18340eec6148986da0455d8ba7848d50470a7a32fb"},
-    {file = "wrapt-1.14.1.tar.gz", hash = "sha256:380a85cf89e0e69b7cfbe2ea9f765f004ff419f34194018a6827ac0e3edfed4d"},
+    {file = "wrapt-1.15.0-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1"},
+    {file = "wrapt-1.15.0-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29"},
+    {file = "wrapt-1.15.0-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2"},
+    {file = "wrapt-1.15.0-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46"},
+    {file = "wrapt-1.15.0-cp27-cp27m-manylinux2010_x86_64.whl", hash = "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c"},
+    {file = "wrapt-1.15.0-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09"},
+    {file = "wrapt-1.15.0-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079"},
+    {file = "wrapt-1.15.0-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e"},
+    {file = "wrapt-1.15.0-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a"},
+    {file = "wrapt-1.15.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923"},
+    {file = "wrapt-1.15.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee"},
+    {file = "wrapt-1.15.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727"},
+    {file = "wrapt-1.15.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7"},
+    {file = "wrapt-1.15.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0"},
+    {file = "wrapt-1.15.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec"},
+    {file = "wrapt-1.15.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90"},
+    {file = "wrapt-1.15.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975"},
+    {file = "wrapt-1.15.0-cp310-cp310-win32.whl", hash = "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1"},
+    {file = "wrapt-1.15.0-cp310-cp310-win_amd64.whl", hash = "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e"},
+    {file = "wrapt-1.15.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7"},
+    {file = "wrapt-1.15.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72"},
+    {file = "wrapt-1.15.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb"},
+    {file = "wrapt-1.15.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e"},
+    {file = "wrapt-1.15.0-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c"},
+    {file = "wrapt-1.15.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3"},
+    {file = "wrapt-1.15.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92"},
+    {file = "wrapt-1.15.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98"},
+    {file = "wrapt-1.15.0-cp311-cp311-win32.whl", hash = "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416"},
+    {file = "wrapt-1.15.0-cp311-cp311-win_amd64.whl", hash = "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705"},
+    {file = "wrapt-1.15.0-cp35-cp35m-manylinux1_i686.whl", hash = "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29"},
+    {file = "wrapt-1.15.0-cp35-cp35m-manylinux1_x86_64.whl", hash = "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd"},
+    {file = "wrapt-1.15.0-cp35-cp35m-manylinux2010_i686.whl", hash = "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb"},
+    {file = "wrapt-1.15.0-cp35-cp35m-manylinux2010_x86_64.whl", hash = "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248"},
+    {file = "wrapt-1.15.0-cp35-cp35m-win32.whl", hash = "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559"},
+    {file = "wrapt-1.15.0-cp35-cp35m-win_amd64.whl", hash = "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"},
+    {file = "wrapt-1.15.0-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba"},
+    {file = "wrapt-1.15.0-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752"},
+    {file = "wrapt-1.15.0-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364"},
+    {file = "wrapt-1.15.0-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475"},
+    {file = "wrapt-1.15.0-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8"},
+    {file = "wrapt-1.15.0-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418"},
+    {file = "wrapt-1.15.0-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2"},
+    {file = "wrapt-1.15.0-cp36-cp36m-win32.whl", hash = "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1"},
+    {file = "wrapt-1.15.0-cp36-cp36m-win_amd64.whl", hash = "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420"},
+    {file = "wrapt-1.15.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317"},
+    {file = "wrapt-1.15.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e"},
+    {file = "wrapt-1.15.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e"},
+    {file = "wrapt-1.15.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0"},
+    {file = "wrapt-1.15.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019"},
+    {file = "wrapt-1.15.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034"},
+    {file = "wrapt-1.15.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653"},
+    {file = "wrapt-1.15.0-cp37-cp37m-win32.whl", hash = "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0"},
+    {file = "wrapt-1.15.0-cp37-cp37m-win_amd64.whl", hash = "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e"},
+    {file = "wrapt-1.15.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145"},
+    {file = "wrapt-1.15.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f"},
+    {file = "wrapt-1.15.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd"},
+    {file = "wrapt-1.15.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b"},
+    {file = "wrapt-1.15.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f"},
+    {file = "wrapt-1.15.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6"},
+    {file = "wrapt-1.15.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094"},
+    {file = "wrapt-1.15.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7"},
+    {file = "wrapt-1.15.0-cp38-cp38-win32.whl", hash = "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b"},
+    {file = "wrapt-1.15.0-cp38-cp38-win_amd64.whl", hash = "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1"},
+    {file = "wrapt-1.15.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86"},
+    {file = "wrapt-1.15.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c"},
+    {file = "wrapt-1.15.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d"},
+    {file = "wrapt-1.15.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc"},
+    {file = "wrapt-1.15.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29"},
+    {file = "wrapt-1.15.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a"},
+    {file = "wrapt-1.15.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8"},
+    {file = "wrapt-1.15.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9"},
+    {file = "wrapt-1.15.0-cp39-cp39-win32.whl", hash = "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff"},
+    {file = "wrapt-1.15.0-cp39-cp39-win_amd64.whl", hash = "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6"},
+    {file = "wrapt-1.15.0-py3-none-any.whl", hash = "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640"},
+    {file = "wrapt-1.15.0.tar.gz", hash = "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a"},
 ]
 
 [[package]]
 name = "zipp"
-version = "3.12.0"
+version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "zipp-3.12.0-py3-none-any.whl", hash = "sha256:9eb0a4c5feab9b08871db0d672745b53450d7f26992fd1e4653aa43345e97b86"},
-    {file = "zipp-3.12.0.tar.gz", hash = "sha256:73efd63936398aac78fd92b6f4865190119d6c91b531532e798977ea8dd402eb"},
+    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
+    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["flake8 (<5)", "func-timeout", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
-
-[extras]
-tracking = ["sentry-sdk"]
+testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
-content-hash = "f2c0b0d7ab8865886401522547d31c1fcb2a86d85e335ac1c4a18d35a64ad1fc"
+content-hash = "81b6346120a9207a6e48a63b881bab362136bde38fbc80b3fdf4d78d35c1f7ee"
```

### Comparing `ospd_openvas-22.5.1/pyproject.toml` & `ospd_openvas-22.5.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ospd-openvas"
-version = "22.5.1"
+version = "22.5.2"
 description = "ospd based scanner for openvas"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/ospd-openvas"
 repository = "https://github.com/greenbone/ospd-openvas"
 # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
@@ -43,32 +43,28 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 redis = ">=3.5.3,<5.0.0"
 psutil = "^5.5.1"
 packaging = ">=20.4,<24.0"
-sentry-sdk = {version="^1.1.0", optional=true}
 lxml = "^4.5.2"
 defusedxml = ">=0.6,<0.8"
 deprecated = "^1.2.10"
 paho-mqtt = ">=1.5.1"
 python-gnupg = ">=0.4.8,<0.6.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.13.9"
-rope = "^1.8.0"
+rope = "^1.9.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 pontos = ">=22.7.2"
 black = ">=22.6.0"
 
-[tool.poetry.extras]
-tracking = ["sentry-sdk"]
-
 [tool.poetry.scripts]
 ospd-openvas = "ospd_openvas.daemon:main"
 
 [tool.black]
 line-length = 80
 target-version = ['py37', 'py38']
 skip-string-normalization = true
```

### Comparing `ospd_openvas-22.5.1/tests/command/test_command.py` & `ospd_openvas-22.5.2/tests/command/test_command.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from unittest import TestCase
 
 from ospd.command.registry import get_commands, remove_command
 from ospd.command.command import BaseCommand
```

### Comparing `ospd_openvas-22.5.1/tests/command/test_commands.py` & `ospd_openvas-22.5.2/tests/command/test_commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import time
 
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 
 from xml.etree import ElementTree as et
```

### Comparing `ospd_openvas-22.5.1/tests/helper.py` & `ospd_openvas-22.5.2/tests/helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable=unused-argument
 # pylint: disable=disallowed-name
 
 
 import time
```

### Comparing `ospd_openvas-22.5.1/tests/messages/test_result.py` & `ospd_openvas-22.5.2/tests/messages/test_result.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime, timezone
 from uuid import UUID
 
 from unittest import TestCase
 
 from ospd_openvas.messages.message import MessageType
```

### Comparing `ospd_openvas-22.5.1/tests/messaging/test_mqtt.py` & `ospd_openvas-22.5.2/tests/messaging/test_mqtt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
 from uuid import UUID
 
 from unittest import TestCase, mock
 
 from ospd_openvas.messages.result import ResultMessage
```

### Comparing `ospd_openvas-22.5.1/tests/test_argument_parser.py` & `ospd_openvas-22.5.2/tests/test_argument_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Test module for command line arguments.
 """
 
 import unittest
 
 from unittest.mock import patch
```

### Comparing `ospd_openvas-22.5.1/tests/test_daemon.py` & `ospd_openvas-22.5.2/tests/test_daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 # pylint: disable=invalid-name,line-too-long,no-value-for-parameter
 
 """ Unit Test for ospd-openvas """
 
 import io
```

### Comparing `ospd_openvas-22.5.1/tests/test_db.py` & `ospd_openvas-22.5.2/tests/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 # pylint: disable=unused-argument
 
 """ Unit Test for ospd-openvas """
 
 import logging
```

### Comparing `ospd_openvas-22.5.1/tests/test_notus.py` & `ospd_openvas-22.5.2/tests/test_notus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2021-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import threading
 from unittest import TestCase, mock
 from typing import Dict, Optional, Iterator
 
 from ospd_openvas.messages.result import ResultMessage
```

### Comparing `ospd_openvas-22.5.1/tests/test_nvti_cache.py` & `ospd_openvas-22.5.2/tests/test_nvti_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 # pylint: disable=unused-argument, protected-access, invalid-name
 
 """ Unit Test for ospd-openvas """
 
 import logging
```

### Comparing `ospd_openvas-22.5.1/tests/test_openvas.py` & `ospd_openvas-22.5.2/tests/test_openvas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 import subprocess
 
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
```

### Comparing `ospd_openvas-22.5.1/tests/test_port_convert.py` & `ospd_openvas-22.5.2/tests/test_port_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """ Test suites for Port manipulation.
 """
 
 import unittest
 
 import logging
```

### Comparing `ospd_openvas-22.5.1/tests/test_preferencehandler.py` & `ospd_openvas-22.5.2/tests/test_preferencehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable = too-many-lines
 
 import logging
 
 from unittest import TestCase
 from unittest.mock import call, patch, Mock, MagicMock
```

### Comparing `ospd_openvas-22.5.1/tests/test_scan_and_result.py` & `ospd_openvas-22.5.2/tests/test_scan_and_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable=too-many-lines
 
 """ Test module for scan runs
 """
 
 import time
```

### Comparing `ospd_openvas-22.5.1/tests/test_vthelper.py` & `ospd_openvas-22.5.2/tests/test_vthelper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone AG
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 from hashlib import sha256
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
 from tests.dummydaemon import DummyDaemon
```

### Comparing `ospd_openvas-22.5.1/tests/test_xml.py` & `ospd_openvas-22.5.2/tests/test_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-# Copyright (C) 2014-2021 Greenbone AG
+# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2014-2023 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as
-# published by the Free Software Foundation, either version 3 of the
-# License, or (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable=invalid-name
 
 from collections import OrderedDict
 import logging
 
 from unittest import TestCase
```

### Comparing `ospd_openvas-22.5.1/PKG-INFO` & `ospd_openvas-22.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ospd-openvas
-Version: 22.5.1
+Version: 22.5.2
 Summary: ospd based scanner for openvas
 Home-page: https://github.com/greenbone/ospd-openvas
 License: AGPL-3.0-or-later
 Keywords: openvas,Greenbone Vulnerability Management,Vulnerability Scanning,OSP,Open Scanner Protocol
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
@@ -14,27 +14,22 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: tracking
 Requires-Dist: defusedxml (>=0.6,<0.8)
 Requires-Dist: deprecated (>=1.2.10,<2.0.0)
 Requires-Dist: lxml (>=4.5.2,<5.0.0)
 Requires-Dist: packaging (>=20.4,<24.0)
 Requires-Dist: paho-mqtt (>=1.5.1)
 Requires-Dist: psutil (>=5.5.1,<6.0.0)
 Requires-Dist: python-gnupg (>=0.4.8,<0.6.0)
 Requires-Dist: redis (>=3.5.3,<5.0.0)
-Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0) ; extra == "tracking"
 Project-URL: Repository, https://github.com/greenbone/ospd-openvas
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # ospd-openvas
```

