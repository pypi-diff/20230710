# Comparing `tmp/openapi_server_test-1.0.28.tar.gz` & `tmp/openapi_server_test-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_server_test-1.0.28.tar", last modified: Mon Jul 10 18:20:02 2023, max compression
+gzip compressed data, was "openapi_server_test-1.0.29.tar", last modified: Mon Jul 10 18:27:32 2023, max compression
```

## Comparing `openapi_server_test-1.0.28.tar` & `openapi_server_test-1.0.29.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.277335 openapi_server_test-1.0.28/
--rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-10 18:15:38.000000 openapi_server_test-1.0.28/MANIFEST.in
--rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-10 18:20:02.276849 openapi_server_test-1.0.28/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 openapi_server_test-1.0.28/README.md
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.239784 openapi_server_test-1.0.28/openapi_server/
--rw-r--r--   0 jialening   (501) staff       (20)     6148 2023-07-10 18:20:00.000000 openapi_server_test-1.0.28/openapi_server/.DS_Store
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/__main__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.240761 openapi_server_test-1.0.28/openapi_server/controllers/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/controllers/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/encoder.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.268797 openapi_server_test-1.0.28/openapi_server/models/
--rw-r--r--   0 jialening   (501) staff       (20)     3610 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/models/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/models/base_model_.py
--rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/config_templates_inner.py
--rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/container.py
--rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/container_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/container_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/deploy_resources.py
--rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/dingman_error.py
--rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/dingman_response.py
--rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/endpoint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/env_from_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/env_var.py
--rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/env_var_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/http_get.py
--rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/ingress.py
--rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/ingress_backend.py
--rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/ingress_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/ingress_tls.py
--rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/node_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/node_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/node_selector_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/object_field_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     4948 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/pod.py
--rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/pod_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/probe.py
--rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/relabel_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/resource_requirements.py
--rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/service.py
--rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/service_monitor.py
--rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/service_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/tcp_socket.py
--rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/update_strategy.py
--rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/volume.py
--rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/volume_device.py
--rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/volume_host_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/volume_mount.py
--rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)    10344 2023-07-10 18:19:55.000000 openapi_server_test-1.0.28/openapi_server/models/workload.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.269391 openapi_server_test-1.0.28/openapi_server/openapi/
--rw-r--r--   0 jialening   (501) staff       (20)   164349 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/openapi/openapi.yaml
--rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/openapi_version
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.271967 openapi_server_test-1.0.28/openapi_server/test/
--rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/test/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)   120299 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/typing_utils.py
--rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-10 18:19:56.000000 openapi_server_test-1.0.28/openapi_server/util.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:20:02.276024 openapi_server_test-1.0.28/openapi_server_test.egg-info/
--rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-10 18:20:02.000000 openapi_server_test-1.0.28/openapi_server_test.egg-info/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)     2989 2023-07-10 18:20:02.000000 openapi_server_test-1.0.28/openapi_server_test.egg-info/SOURCES.txt
--rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-10 18:20:02.000000 openapi_server_test-1.0.28/openapi_server_test.egg-info/dependency_links.txt
--rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-10 18:20:02.000000 openapi_server_test-1.0.28/openapi_server_test.egg-info/requires.txt
--rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-10 18:20:02.000000 openapi_server_test-1.0.28/openapi_server_test.egg-info/top_level.txt
--rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-10 18:20:02.277507 openapi_server_test-1.0.28/setup.cfg
--rw-r--r--   0 jialening   (501) staff       (20)     1426 2023-07-10 18:16:39.000000 openapi_server_test-1.0.28/setup.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.362705 openapi_server_test-1.0.29/
+-rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-10 18:15:38.000000 openapi_server_test-1.0.29/MANIFEST.in
+-rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-10 18:27:32.362203 openapi_server_test-1.0.29/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)      902 2023-06-15 21:30:55.000000 openapi_server_test-1.0.29/README.md
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.324318 openapi_server_test-1.0.29/openapi_server/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/__main__.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.325599 openapi_server_test-1.0.29/openapi_server/controllers/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/controllers/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/encoder.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.356926 openapi_server_test-1.0.29/openapi_server/models/
+-rw-r--r--   0 jialening   (501) staff       (20)     3610 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/models/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/models/base_model_.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/config_templates_inner.py
+-rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/container.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/container_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7015 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/dingman_error.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/dingman_response.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/endpoint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/env_from_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/env_var.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/env_var_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/http_get.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/ingress.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/node_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/node_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4948 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/pod.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/probe.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/relabel_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/service_monitor.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/service_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/update_strategy.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/volume.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/volume_device.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/volume_mount.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10344 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/models/workload.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.357313 openapi_server_test-1.0.29/openapi_server/openapi/
+-rw-r--r--   0 jialening   (501) staff       (20)   164349 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/openapi/openapi.yaml
+-rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/openapi_version
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.358318 openapi_server_test-1.0.29/openapi_server/test/
+-rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/test/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)   120299 2023-07-10 18:27:22.000000 openapi_server_test-1.0.29/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/typing_utils.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-10 18:27:23.000000 openapi_server_test-1.0.29/openapi_server/util.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-10 18:27:32.361408 openapi_server_test-1.0.29/openapi_server_test.egg-info/
+-rw-r--r--   0 jialening   (501) staff       (20)      201 2023-07-10 18:27:32.000000 openapi_server_test-1.0.29/openapi_server_test.egg-info/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)     2964 2023-07-10 18:27:32.000000 openapi_server_test-1.0.29/openapi_server_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-10 18:27:32.000000 openapi_server_test-1.0.29/openapi_server_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-10 18:27:32.000000 openapi_server_test-1.0.29/openapi_server_test.egg-info/requires.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-10 18:27:32.000000 openapi_server_test-1.0.29/openapi_server_test.egg-info/top_level.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-10 18:27:32.363001 openapi_server_test-1.0.29/setup.cfg
+-rw-r--r--   0 jialening   (501) staff       (20)     1444 2023-07-10 18:25:27.000000 openapi_server_test-1.0.29/setup.py
```

### Comparing `openapi_server_test-1.0.28/README.md` & `openapi_server_test-1.0.29/README.md`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/controllers/deploy_resources_controller.py` & `openapi_server_test-1.0.29/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/controllers/security_controller_.py` & `openapi_server_test-1.0.29/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/encoder.py` & `openapi_server_test-1.0.29/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/__init__.py` & `openapi_server_test-1.0.29/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/affinity.py` & `openapi_server_test-1.0.29/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/base_model_.py` & `openapi_server_test-1.0.29/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/config.py` & `openapi_server_test-1.0.29/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/config_templates_inner.py` & `openapi_server_test-1.0.29/openapi_server/models/config_templates_inner.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/container.py` & `openapi_server_test-1.0.29/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/container_life_cycle.py` & `openapi_server_test-1.0.29/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/container_port.py` & `openapi_server_test-1.0.29/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/container_sec_context.py` & `openapi_server_test-1.0.29/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/container_sec_context_capabilities.py` & `openapi_server_test-1.0.29/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/deploy_platform_resource.py` & `openapi_server_test-1.0.29/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/deploy_resources.py` & `openapi_server_test-1.0.29/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/dingman_error.py` & `openapi_server_test-1.0.29/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/dingman_response.py` & `openapi_server_test-1.0.29/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/endpoint.py` & `openapi_server_test-1.0.29/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/env_from_source.py` & `openapi_server_test-1.0.29/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/env_var.py` & `openapi_server_test-1.0.29/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/env_var_source.py` & `openapi_server_test-1.0.29/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/http_get.py` & `openapi_server_test-1.0.29/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/http_ingress_path.py` & `openapi_server_test-1.0.29/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/ingress.py` & `openapi_server_test-1.0.29/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/ingress_backend.py` & `openapi_server_test-1.0.29/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/ingress_backend_service.py` & `openapi_server_test-1.0.29/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/ingress_rule.py` & `openapi_server_test-1.0.29/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/ingress_tls.py` & `openapi_server_test-1.0.29/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/life_cycle_handler.py` & `openapi_server_test-1.0.29/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/node_affinity.py` & `openapi_server_test-1.0.29/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/node_selector.py` & `openapi_server_test-1.0.29/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/node_selector_term.py` & `openapi_server_test-1.0.29/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/object_field_selector.py` & `openapi_server_test-1.0.29/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/persistent_volume_claim.py` & `openapi_server_test-1.0.29/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/pod.py` & `openapi_server_test-1.0.29/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/pod_affinity.py` & `openapi_server_test-1.0.29/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/pod_affinity_term.py` & `openapi_server_test-1.0.29/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/pod_anti_affinity.py` & `openapi_server_test-1.0.29/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/preferred_scheduling_term.py` & `openapi_server_test-1.0.29/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/probe.py` & `openapi_server_test-1.0.29/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/ref_volume_source.py` & `openapi_server_test-1.0.29/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/relabel_config.py` & `openapi_server_test-1.0.29/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/resource_requirements.py` & `openapi_server_test-1.0.29/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/service.py` & `openapi_server_test-1.0.29/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/service_monitor.py` & `openapi_server_test-1.0.29/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/service_monitor_namespace_selector.py` & `openapi_server_test-1.0.29/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/service_port.py` & `openapi_server_test-1.0.29/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/tcp_socket.py` & `openapi_server_test-1.0.29/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/update_strategy.py` & `openapi_server_test-1.0.29/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/update_strategy_rolling_update_config.py` & `openapi_server_test-1.0.29/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/volume.py` & `openapi_server_test-1.0.29/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/volume_device.py` & `openapi_server_test-1.0.29/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/volume_empty_dir.py` & `openapi_server_test-1.0.29/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/volume_host_path.py` & `openapi_server_test-1.0.29/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/volume_mount.py` & `openapi_server_test-1.0.29/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/volume_persistent_volume_claim.py` & `openapi_server_test-1.0.29/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/weighted_pod_affinity_term.py` & `openapi_server_test-1.0.29/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/models/workload.py` & `openapi_server_test-1.0.29/openapi_server/models/workload.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/openapi/openapi.yaml` & `openapi_server_test-1.0.29/openapi_server/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/test/test_deploy_resources_controller.py` & `openapi_server_test-1.0.29/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/typing_utils.py` & `openapi_server_test-1.0.29/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server/util.py` & `openapi_server_test-1.0.29/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `openapi_server_test-1.0.28/openapi_server_test.egg-info/SOURCES.txt` & `openapi_server_test-1.0.29/openapi_server_test.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MANIFEST.in
 README.md
 setup.py
-openapi_server/.DS_Store
 openapi_server/__init__.py
 openapi_server/__main__.py
 openapi_server/encoder.py
 openapi_server/openapi_version
 openapi_server/typing_utils.py
 openapi_server/util.py
 openapi_server/controllers/__init__.py
```

### Comparing `openapi_server_test-1.0.28/setup.py` & `openapi_server_test-1.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     author="BD Data Sys IE CDN",
     description="CDN DMS Open API",
     url="https://code.byted.org/savanna/dingman_api_server",
     # package_data={
     #     "": ["openapi_version"],
     # },
     # packages=setuptools.find_packages("openapi_server"),
-    packages=['openapi_server.test', 'openapi_server.models', 'openapi_server.controllers'],
+    packages=['openapi_server', 'openapi_server.test', 'openapi_server.models', 'openapi_server.controllers'],
     # package_dir={"":"openapi_server"},
     include_package_data=True,
     python_requires=">=3.7",
     install_requires = [
         "flask"
     ],
 )
```

