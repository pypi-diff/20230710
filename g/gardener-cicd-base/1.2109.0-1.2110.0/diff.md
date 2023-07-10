# Comparing `tmp/gardener-cicd-base-1.2109.0.tar.gz` & `tmp/gardener-cicd-base-1.2110.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-base-1.2109.0.tar", last modified: Fri Jul  7 12:45:21 2023, max compression
+gzip compressed data, was "gardener-cicd-base-1.2110.0.tar", last modified: Mon Jul 10 09:11:52 2023, max compression
```

## Comparing `gardener-cicd-base-1.2109.0.tar` & `gardener-cicd-base-1.2110.0.tar`

### file list

```diff
@@ -1,77 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:45:21.707110 gardener-cicd-base-1.2109.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-07 12:45:21.707110 gardener-cicd-base-1.2109.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:45:21.703110 gardener-cicd-base-1.2109.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     6490 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10735 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/jira.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:45:21.703110 gardener-cicd-base-1.2109.0/ci/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3826 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ci/log.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ci/paths.py
--rw-r--r--   0 root         (0) root         (0)    15149 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ci/util.py
--rw-r--r--   0 root         (0) root         (0)     6456 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/ctx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:45:21.703110 gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-07 12:45:21.000000 gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-07 12:45:21.000000 gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 12:45:21.000000 gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-07 12:45:21.000000 gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 12:45:21.000000 gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:45:21.707110 gardener-cicd-base-1.2109.0/model/
--rw-r--r--   0 root         (0) root         (0)    24304 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     1135 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/aws.py
--rw-r--r--   0 root         (0) root         (0)     3567 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/azure.py
--rw-r--r--   0 root         (0) root         (0)     5241 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1062 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)      387 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/cam.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/ccee.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/checkmarx.py
--rw-r--r--   0 root         (0) root         (0)     2640 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/clamav.py
--rw-r--r--   0 root         (0) root         (0)    22034 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/concourse.py
--rw-r--r--   0 root         (0) root         (0)     7585 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/ctx_repository.py
--rw-r--r--   0 root         (0) root         (0)     3928 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/delivery.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/delivery_db.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/docker.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/email.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/gardenlinux_cache.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/gcp.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/github.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/gitlab.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/ingress.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/jira.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/oauth2_proxy.py
--rw-r--r--   0 root         (0) root         (0)     4034 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/protecode.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/proxy.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/pypi.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/secret.py
--rw-r--r--   0 root         (0) root         (0)     2848 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)     3152 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/signing_server.py
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/slack.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/tekton.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/tekton_dashboard_ingress.py
--rw-r--r--   0 root         (0) root         (0)     1166 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/victorops.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/model/webhook_dispatcher.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/setup.base.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-07 12:45:21.707110 gardener-cicd-base-1.2109.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/setup.py
--rw-r--r--   0 root         (0) root         (0)    15149 2023-07-07 12:44:29.000000 gardener-cicd-base-1.2109.0/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:11:52.188278 gardener-cicd-base-1.2110.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-10 09:11:52.188278 gardener-cicd-base-1.2110.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:11:52.180277 gardener-cicd-base-1.2110.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10735 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:11:52.180277 gardener-cicd-base-1.2110.0/ci/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ci/log.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ci/paths.py
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ci/util.py
+-rw-r--r--   0 root         (0) root         (0)     6456 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/ctx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:11:52.180277 gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-10 09:11:52.000000 gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-07-10 09:11:52.000000 gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 09:11:52.000000 gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 09:11:52.000000 gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-10 09:11:52.000000 gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 09:11:52.184278 gardener-cicd-base-1.2110.0/model/
+-rw-r--r--   0 root         (0) root         (0)    24304 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/aws.py
+-rw-r--r--   0 root         (0) root         (0)     3567 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/azure.py
+-rw-r--r--   0 root         (0) root         (0)     5241 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)      387 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/cam.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/ccee.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/checkmarx.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/clamav.py
+-rw-r--r--   0 root         (0) root         (0)    22034 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/ctx_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/delivery_db.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/docker.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/email.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/gardenlinux_cache.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/github.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/ingress.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/jira.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/oauth2_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/pypi.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/secret.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/signing_server.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/slack.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/tekton.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/tekton_dashboard_ingress.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/victorops.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/model/webhook_dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/setup.base.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-10 09:11:52.188278 gardener-cicd-base-1.2110.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-07-10 09:09:17.000000 gardener-cicd-base-1.2110.0/util.py
```

### Comparing `gardener-cicd-base-1.2109.0/LICENSE.md` & `gardener-cicd-base-1.2110.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/README.md` & `gardener-cicd-base-1.2110.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/__init__.py` & `gardener-cicd-base-1.2110.0/ccc/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/alicloud.py` & `gardener-cicd-base-1.2110.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/aws.py` & `gardener-cicd-base-1.2110.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/clamav.py` & `gardener-cicd-base-1.2110.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/concourse.py` & `gardener-cicd-base-1.2110.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/delivery.py` & `gardener-cicd-base-1.2110.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/elasticsearch.py` & `gardener-cicd-base-1.2110.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/gcp.py` & `gardener-cicd-base-1.2110.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/github.py` & `gardener-cicd-base-1.2110.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/grafeas_model.py` & `gardener-cicd-base-1.2110.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/jira.py` & `gardener-cicd-base-1.2110.0/model/aws.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import jira
+from model.base import (
+    NamedModelElement,
+)
 
-import model.jira
 
+class AwsProfile(NamedModelElement):
+    def region(self):
+        return self.raw['region']
 
-def from_cfg(
-    jira_cfg:model.jira.JiraConfig
-):
-    raise NotImplementedError()
+    def access_key_id(self):
+        return self.raw['access_key_id']
 
+    def secret_access_key(self):
+        return self.raw['secret_access_key']
 
-def _from_cfg(
-    jira_cfg:model.jira.JiraConfig
-) -> jira.JIRA:
-    credentials = jira_cfg.credentials()
-    return jira.JIRA(
-        server=jira_cfg.base_url(),
-        basic_auth=credentials.as_tuple(),
-    )
+    def _required_attributes(self):
+        return ['region','access_key_id','secret_access_key']
```

### Comparing `gardener-cicd-base-1.2109.0/ccc/oci.py` & `gardener-cicd-base-1.2110.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/protecode.py` & `gardener-cicd-base-1.2110.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ccc/secrets_server.py` & `gardener-cicd-base-1.2110.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ci/__init__.py` & `gardener-cicd-base-1.2110.0/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ci/log.py` & `gardener-cicd-base-1.2110.0/ci/log.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ci/util.py` & `gardener-cicd-base-1.2110.0/ci/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/ctx.py` & `gardener-cicd-base-1.2110.0/ctx.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/gardener_cicd_base.egg-info/SOURCES.txt` & `gardener-cicd-base-1.2110.0/gardener_cicd_base.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ccc/clamav.py
 ccc/concourse.py
 ccc/delivery.py
 ccc/elasticsearch.py
 ccc/gcp.py
 ccc/github.py
 ccc/grafeas_model.py
-ccc/jira.py
 ccc/oci.py
 ccc/protecode.py
 ccc/secrets_server.py
 ccc/slack.py
 ci/__init__.py
 ci/log.py
 ci/paths.py
```

### Comparing `gardener-cicd-base-1.2109.0/model/__init__.py` & `gardener-cicd-base-1.2110.0/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/alicloud.py` & `gardener-cicd-base-1.2110.0/model/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/aws.py` & `gardener-cicd-base-1.2110.0/model/docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-# Copyright (c) 2019-2020 SAP SE or an SAP affiliate company. All rights reserved. This file is
+# Copyright (c) 2019-2021 SAP SE or an SAP affiliate company. All rights reserved. This file is
 # licensed under the Apache Software License, v. 2 except as noted otherwise in the LICENSE file
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from model.base import (
-    NamedModelElement,
-)
+from model.base import NamedModelElement
 
 
-class AwsProfile(NamedModelElement):
-    def region(self):
-        return self.raw['region']
+class DockerConfig(NamedModelElement):
+    def username(self):
+        return self.raw.get('username')
 
-    def access_key_id(self):
-        return self.raw['access_key_id']
+    def email_address(self):
+        return self.raw.get('email_address')
 
-    def secret_access_key(self):
-        return self.raw['secret_access_key']
+    def password(self):
+        return self.raw.get('password')
+
+    def access_tokens(self):
+        return self.raw.get('access_tokens')
 
     def _required_attributes(self):
-        return ['region','access_key_id','secret_access_key']
+        return (
+            'username',
+            'email_address',
+            'password',
+        )
+
+    def _optional_attributes(self):
+        return ('access_tokens',)
```

### Comparing `gardener-cicd-base-1.2109.0/model/azure.py` & `gardener-cicd-base-1.2110.0/model/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/base.py` & `gardener-cicd-base-1.2110.0/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/btp_application_certificate.py` & `gardener-cicd-base-1.2110.0/model/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/btp_service_binding.py` & `gardener-cicd-base-1.2110.0/model/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/ccee.py` & `gardener-cicd-base-1.2110.0/model/ccee.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/checkmarx.py` & `gardener-cicd-base-1.2110.0/model/checkmarx.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/clamav.py` & `gardener-cicd-base-1.2110.0/model/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/concourse.py` & `gardener-cicd-base-1.2110.0/model/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/container_registry.py` & `gardener-cicd-base-1.2110.0/model/container_registry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/ctx_repository.py` & `gardener-cicd-base-1.2110.0/model/ctx_repository.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/delivery.py` & `gardener-cicd-base-1.2110.0/model/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/delivery_db.py` & `gardener-cicd-base-1.2110.0/model/delivery_db.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/docker.py` & `gardener-cicd-base-1.2110.0/model/victorops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-# Copyright (c) 2019-2021 SAP SE or an SAP affiliate company. All rights reserved. This file is
+# Copyright (c) 2019-2020 SAP SE or an SAP affiliate company. All rights reserved. This file is
 # licensed under the Apache Software License, v. 2 except as noted otherwise in the LICENSE file
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from model.base import NamedModelElement
+from model.base import (
+    NamedModelElement,
+)
 
 
-class DockerConfig(NamedModelElement):
-    def username(self):
-        return self.raw.get('username')
+class VictoropsConfig(NamedModelElement):
+    def api_id(self):
+        return self.raw['api_token']
 
-    def email_address(self):
-        return self.raw.get('email_address')
+    def api_key(self):
+        return self.raw['api_key']
 
-    def password(self):
-        return self.raw.get('password')
+    def team_slug(self):
+        return self.raw['team_slug']
 
-    def access_tokens(self):
-        return self.raw.get('access_tokens')
+    def dod_policy_slug(self):
+        return self.raw['dod_policy_slug']
 
-    def _required_attributes(self):
-        return (
-            'username',
-            'email_address',
-            'password',
-        )
-
-    def _optional_attributes(self):
-        return ('access_tokens',)
+    def mod_policy_slug(self):
+        return self.raw['mod_policy_slug']
```

### Comparing `gardener-cicd-base-1.2109.0/model/elasticsearch.py` & `gardener-cicd-base-1.2110.0/model/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/email.py` & `gardener-cicd-base-1.2110.0/model/email.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/gardenlinux_cache.py` & `gardener-cicd-base-1.2110.0/model/gardenlinux_cache.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/gcp.py` & `gardener-cicd-base-1.2110.0/model/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/github.py` & `gardener-cicd-base-1.2110.0/model/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/gitlab.py` & `gardener-cicd-base-1.2110.0/model/gitlab.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/ingress.py` & `gardener-cicd-base-1.2110.0/model/ingress.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/jira.py` & `gardener-cicd-base-1.2110.0/model/jira.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/kubernetes.py` & `gardener-cicd-base-1.2110.0/model/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/oauth2_proxy.py` & `gardener-cicd-base-1.2110.0/model/oauth2_proxy.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/protecode.py` & `gardener-cicd-base-1.2110.0/model/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/proxy.py` & `gardener-cicd-base-1.2110.0/model/proxy.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/pypi.py` & `gardener-cicd-base-1.2110.0/model/pypi.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/secret.py` & `gardener-cicd-base-1.2110.0/model/secret.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/secrets_server.py` & `gardener-cicd-base-1.2110.0/model/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/signing_server.py` & `gardener-cicd-base-1.2110.0/model/signing_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/slack.py` & `gardener-cicd-base-1.2110.0/model/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/tekton.py` & `gardener-cicd-base-1.2110.0/model/tekton.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/tekton_dashboard_ingress.py` & `gardener-cicd-base-1.2110.0/model/tekton_dashboard_ingress.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/model/webhook_dispatcher.py` & `gardener-cicd-base-1.2110.0/model/webhook_dispatcher.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/setup.base.py` & `gardener-cicd-base-1.2110.0/setup.base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/setup.py` & `gardener-cicd-base-1.2110.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-base-1.2109.0/util.py` & `gardener-cicd-base-1.2110.0/util.py`

 * *Files identical despite different names*

