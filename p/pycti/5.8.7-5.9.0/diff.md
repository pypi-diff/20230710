# Comparing `tmp/pycti-5.8.7.tar.gz` & `tmp/pycti-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.8.7.tar", last modified: Thu Jun 29 07:13:55 2023, max compression
+gzip compressed data, was "pycti-5.9.0.tar", last modified: Mon Jul 10 16:03:45 2023, max compression
```

## Comparing `pycti-5.8.7.tar` & `pycti-5.9.0.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.718320 pycti-5.8.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-29 07:13:43.000000 pycti-5.8.7/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-29 07:13:55.718320 pycti-5.8.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-06-29 07:13:43.000000 pycti-5.8.7/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.706320 pycti-5.8.7/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4262 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.710320 pycti-5.8.7/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28410 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.710320 pycti-5.8.7/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45735 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.714320 pycti-5.8.7/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25217 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24565 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24546 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22913 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14162 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23077 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15944 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22348 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22667 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20971 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23782 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18371 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.718320 pycti-5.8.7/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6581 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   104930 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-06-29 07:13:43.000000 pycti-5.8.7/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 07:13:55.710320 pycti-5.8.7/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-29 07:13:55.000000 pycti-5.8.7/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-06-29 07:13:55.000000 pycti-5.8.7/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-29 07:13:55.000000 pycti-5.8.7/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-29 07:13:55.000000 pycti-5.8.7/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-29 07:13:55.000000 pycti-5.8.7/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-29 07:13:43.000000 pycti-5.8.7/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-06-29 07:13:55.718320 pycti-5.8.7/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.404688 pycti-5.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-10 16:03:33.000000 pycti-5.9.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-10 16:03:45.404688 pycti-5.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-10 16:03:33.000000 pycti-5.9.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.404688 pycti-5.9.0/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25352 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24724 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24705 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23072 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14162 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23083 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15950 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23099 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21404 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23941 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18610 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18872 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.404688 pycti-5.9.0/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6827 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106041 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-10 16:03:33.000000 pycti-5.9.0/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-10 16:03:45.396688 pycti-5.9.0/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-10 16:03:45.000000 pycti-5.9.0/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-10 16:03:33.000000 pycti-5.9.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-10 16:03:45.408688 pycti-5.9.0/setup.cfg
```

### Comparing `pycti-5.8.7/LICENSE` & `pycti-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/PKG-INFO` & `pycti-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.8.7
+Version: 5.9.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.8.7 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.0 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.8.7/README.md` & `pycti-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/__init__.py` & `pycti-5.9.0/pycti/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.8.7"
+__version__ = "5.9.0"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
@@ -41,14 +41,16 @@
 from .entities.opencti_stix_nested_ref_relationship import StixNestedRefRelationship
 from .entities.opencti_stix_object_or_stix_relationship import (
     StixObjectOrStixRelationship,
 )
 from .entities.opencti_stix_sighting_relationship import StixSightingRelationship
 from .entities.opencti_task import Task
 from .entities.opencti_threat_actor import ThreatActor
+from .entities.opencti_threat_actor_group import ThreatActorGroup
+from .entities.opencti_threat_actor_individual import ThreatActorIndividual
 from .entities.opencti_tool import Tool
 from .entities.opencti_vulnerability import Vulnerability
 from .utils.constants import (
     CustomObjectCaseIncident,
     CustomObjectTask,
     CustomObservableCryptocurrencyWallet,
     CustomObservableHostname,
@@ -107,14 +109,16 @@
     "StixCyberObservableTypes",
     "StixDomainObject",
     "StixMetaTypes",
     "MultipleRefRelationship",
     "StixObjectOrStixRelationship",
     "StixSightingRelationship",
     "ThreatActor",
+    "ThreatActorGroup",
+    "ThreatActorIndividual",
     "Tool",
     "Vulnerability",
     "get_config_variable",
     "CustomObjectCaseIncident",
     "CustomObjectTask",
     "StixCyberObservableTypes",
     "CustomObservableHostname",
```

### Comparing `pycti-5.8.7/pycti/api/opencti_api_client.py` & `pycti-5.9.0/pycti/api/opencti_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 )
 from pycti.entities.opencti_stix_object_or_stix_relationship import (
     StixObjectOrStixRelationship,
 )
 from pycti.entities.opencti_stix_sighting_relationship import StixSightingRelationship
 from pycti.entities.opencti_task import Task
 from pycti.entities.opencti_threat_actor import ThreatActor
+from pycti.entities.opencti_threat_actor_group import ThreatActorGroup
+from pycti.entities.opencti_threat_actor_individual import ThreatActorIndividual
 from pycti.entities.opencti_tool import Tool
 from pycti.entities.opencti_vocabulary import Vocabulary
 from pycti.entities.opencti_vulnerability import Vulnerability
 from pycti.utils.opencti_stix2 import OpenCTIStix2
 from pycti.utils.opencti_stix2_utils import OpenCTIStix2Utils
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -177,14 +179,16 @@
         self.stix_core_relationship = StixCoreRelationship(self)
         self.stix_sighting_relationship = StixSightingRelationship(self)
         self.stix_nested_ref_relationship = StixNestedRefRelationship(self)
         self.identity = Identity(self)
         self.event = Event(self)
         self.location = Location(self)
         self.threat_actor = ThreatActor(self)
+        self.threat_actor_group = ThreatActorGroup(self)
+        self.threat_actor_individual = ThreatActorIndividual(self)
         self.intrusion_set = IntrusionSet(self)
         self.infrastructure = Infrastructure(self)
         self.campaign = Campaign(self)
         self.case_incident = CaseIncident(self)
         self.feedback = Feedback(self)
         self.case_rfi = CaseRfi(self)
         self.case_rft = CaseRft(self)
@@ -403,15 +407,16 @@
         :return: returns `True` if the health check has been successful
         :rtype: bool
         """
         try:
             test = self.threat_actor.list(first=1)
             if test is not None:
                 return True
-        except:
+        except Exception as err:  # pylint: disable=broad-except
+            LOGGER.error("%s", err)
             return False
         return False
 
     def get_logs_worker_config(self):
         """get the logsWorkerConfig
 
         return: the logsWorkerConfig
```

### Comparing `pycti-5.8.7/pycti/api/opencti_api_connector.py` & `pycti-5.9.0/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/api/opencti_api_work.py` & `pycti-5.9.0/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/connector/opencti_connector.py` & `pycti-5.9.0/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/connector/opencti_connector_helper.py` & `pycti-5.9.0/pycti/connector/opencti_connector_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1053,15 +1053,15 @@
         # Send the message
         try:
             channel.basic_publish(
                 exchange=self.connector_config["push_exchange"],
                 routing_key=self.connector_config["push_routing"],
                 body=json.dumps(message),
                 properties=pika.BasicProperties(
-                    delivery_mode=2,  # make message persistent
+                    delivery_mode=2, content_encoding="utf-8"  # make message persistent
                 ),
             )
         except (UnroutableError, NackError) as e:
             LOGGER.error("Unable to send bundle, retry...%s", e)
             self._send_bundle(channel, bundle, **kwargs)
 
     def stix2_get_embedded_objects(self, item) -> Dict:
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_attack_pattern.py` & `pycti-5.9.0/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_campaign.py` & `pycti-5.9.0/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_case_incident.py` & `pycti-5.9.0/pycti/entities/opencti_case_incident.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             modified
             name
             description
             rating
             severity
             priority
             response_types
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -206,14 +206,17 @@
                         }
                         ... on DataComponent {
                             name
                         }
                         ... on DataSource {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_case_rfi.py` & `pycti-5.9.0/pycti/entities/opencti_case_rfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             revoked
             confidence
             created
             modified
             name
             description
             information_types
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -203,14 +203,17 @@
                         }
                         ... on DataComponent {
                             name
                         }
                         ... on DataSource {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                        
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_case_rft.py` & `pycti-5.9.0/pycti/entities/opencti_case_rft.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             revoked
             confidence
             created
             modified
             name
             description
             takedown_types
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -203,14 +203,17 @@
                         }
                         ... on DataComponent {
                             name
                         }
                         ... on DataSource {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                        
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_channel.py` & `pycti-5.9.0/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_course_of_action.py` & `pycti-5.9.0/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_data_component.py` & `pycti-5.9.0/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_data_source.py` & `pycti-5.9.0/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_event.py` & `pycti-5.9.0/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_external_reference.py` & `pycti-5.9.0/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_feedback.py` & `pycti-5.9.0/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_grouping.py` & `pycti-5.9.0/pycti/entities/opencti_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             confidence
             created
             modified
             name
             description
             context
             x_opencti_aliases
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -186,14 +186,17 @@
                         }
                         ... on Vulnerability {
                             name
                         }
                         ... on Incident {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                        
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_identity.py` & `pycti-5.9.0/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_incident.py` & `pycti-5.9.0/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_indicator.py` & `pycti-5.9.0/pycti/entities/opencti_indicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         read can be either used with a known OpenCTI entity `id` or by using a
         valid filter to search and return a single Indicator entity or None.
 
         The list method accepts the following kwargs.
 
         Note: either `id` or `filters` is required.
 
-        :param str id: the id of the Threat-Actor
+        :param str id: the id of the Threat-Actor-Group
         :param list filters: the filters to apply if no id provided
 
         :return: Indicator object
         :rtype: Indicator
         """
 
         id = kwargs.get("id", None)
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_infrastructure.py` & `pycti-5.9.0/pycti/entities/opencti_infrastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         read can be either used with a known OpenCTI entity `id` or by using a
         valid filter to search and return a single Infrastructure entity or None.
 
         The list method accepts the following kwargs.
 
         Note: either `id` or `filters` is required.
 
-        :param str id: the id of the Threat-Actor
+        :param str id: the id of the Threat-Actor-Group
         :param list filters: the filters to apply if no id provided
         """
 
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_intrusion_set.py` & `pycti-5.9.0/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.9.0/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_label.py` & `pycti-5.9.0/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_language.py` & `pycti-5.9.0/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_location.py` & `pycti-5.9.0/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_malware.py` & `pycti-5.9.0/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_malware_analysis.py` & `pycti-5.9.0/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_marking_definition.py` & `pycti-5.9.0/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_narrative.py` & `pycti-5.9.0/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_note.py` & `pycti-5.9.0/pycti/entities/opencti_note.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             created
             modified
             attribute_abstract
             content
             authors
             note_types
             likelihood
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -209,21 +209,30 @@
                         }
                         ... on DataSource {
                             name
                         }
                         ... on Case {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                        
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
+                       ... on StixSightingRelationship {
+                            standard_id
+                            spec_version
+                            created_at
+                            updated_at
+                        }                        
                     }
                 }
             }
             importFiles {
                 edges {
                     node {
                         id
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_observed_data.py` & `pycti-5.9.0/pycti/entities/opencti_observed_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             revoked
             confidence
             created
             modified
             first_observed
             last_observed
             number_observed
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -206,20 +206,29 @@
                         }
                         ... on DataSource {
                             name
                         }
                         ... on Case {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                               
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                         }
+                       ... on StixSightingRelationship {
+                            standard_id
+                            spec_version
+                            created_at
+                            updated_at
+                        }                        
                     }
                 }
             }
             importFiles {
                 edges {
                     node {
                         id
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_opinion.py` & `pycti-5.9.0/pycti/entities/opencti_opinion.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             revoked
             confidence
             created
             modified
             explanation
             authors
             opinion
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -186,21 +186,30 @@
                         }
                         ... on Incident {
                             name
                         }
                         ... on Case {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                               
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
+                       ... on StixSightingRelationship {
+                            standard_id
+                            spec_version
+                            created_at
+                            updated_at
+                        }                         
                     }
                 }
             }
             importFiles {
                 edges {
                     node {
                         id
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_report.py` & `pycti-5.9.0/pycti/entities/opencti_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             confidence
             created
             modified
             name
             description
             report_types
             published
-            objects {
+            objects(all: true) {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
                         }
@@ -209,14 +209,17 @@
                         }
                         ... on DataSource {
                             name
                         }
                         ... on Case {
                             name
                         }
+                        ... on StixCyberObservable {
+                            observable_value
+                        }                        
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix.py` & `pycti-5.9.0/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_core_object.py` & `pycti-5.9.0/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.9.0/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.9.0/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.9.0/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.9.0/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.9.0/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.9.0/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_task.py` & `pycti-5.9.0/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_threat_actor.py` & `pycti-5.9.0/pycti/entities/opencti_threat_actor_individual.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from typing import Union
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
 
-class ThreatActor:
-    """Main ThreatActor class for OpenCTI
+class ThreatActorIndividual:
+    """Main ThreatActorIndividual class for OpenCTI
 
     :param opencti: instance of :py:class:`~pycti.api.opencti_api_client.OpenCTIApiClient`
     """
 
     def __init__(self, opencti):
-        """Create an instance of ThreatActor"""
+        """Create an instance of ThreatActorIndividual"""
 
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -151,15 +151,15 @@
         name = name.lower().strip()
         data = {"name": name}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "threat-actor--" + id
 
     def list(self, **kwargs) -> dict:
-        """List Threat-Actor objects
+        """List Threat-Actor-Individual objects
 
         The list method accepts the following kwargs:
 
         :param list filters: (optional) the filters to apply
         :param str search: (optional) a search keyword to apply for the listing
         :param int first: (optional) return the first n rows from the `after` ID
                             or the beginning if not set
@@ -178,22 +178,24 @@
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 500
 
-        LOGGER.info("Listing Threat-Actors with filters %s.", json.dumps(filters))
+        LOGGER.info(
+            "Listing Threat-Actors-Individual with filters %s.", json.dumps(filters)
+        )
         query = (
             """
-            query ThreatActors($filters: [ThreatActorsFiltering], $search: String, $first: Int, $after: ID, $orderBy: ThreatActorsOrdering, $orderMode: OrderingMode) {
-                threatActors(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
-                    edges {
-                        node {
-                            """
+                query ThreatActorsIndividual($filters: [ThreatActorsIndividualFiltering!], $search: String, $first: Int, $after: ID, $orderBy: ThreatActorsIndividualOrdering, $orderMode: OrderingMode) {
+                    threatActorsIndividuals(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+                        edges {
+                            node {
+                                """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
                     pageInfo {
                         startCursor
                         endCursor
@@ -213,98 +215,102 @@
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
         return self.opencti.process_multiple(
-            result["data"]["threatActors"], with_pagination
+            result["data"]["threatActorsIndividuals"], with_pagination
         )
 
     def read(self, **kwargs) -> Union[dict, None]:
-        """Read a Threat-Actor object
+        """Read a Threat-Actor-Individual object
 
         read can be either used with a known OpenCTI entity `id` or by using a
-        valid filter to search and return a single Threat-Actor entity or None.
+        valid filter to search and return a single Threat-Actor-Group entity or None.
 
         The list method accepts the following kwargs.
 
         Note: either `id` or `filters` is required.
 
-        :param str id: the id of the Threat-Actor
+        :param str id: the id of the Threat-Actor-Individual
         :param list filters: the filters to apply if no id provided
         """
 
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            LOGGER.info("Reading Threat-Actor {%s}.", id)
+            LOGGER.info("Reading Threat-Actor-Individual {%s}.", id)
             query = (
                 """
-                query ThreatActor($id: String!) {
-                    threatActor(id: $id) {
-                        """
+                    query ThreatActorIndividual($id: String!) {
+                        threatActorIndividual(id: $id) {
+                            """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(result["data"]["threatActor"])
+            return self.opencti.process_multiple_fields(
+                result["data"]["threatActorIndividual"]
+            )
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
         else:
-            LOGGER.error("[opencti_threat_actor] Missing parameters: id or filters")
+            LOGGER.error(
+                "[opencti_threat_actor_individual] Missing parameters: id or filters"
+            )
             return None
 
     def create(self, **kwargs):
-        """Create a Threat-Actor object
+        """Create a Threat-Actor-Individual object
 
-        The Threat-Actor entity will only be created if it doesn't exists
+        The Threat-Actor-Individual entity will only be created if it doesn't exists
         By setting `update` to `True` it acts like an upsert and updates
-        fields of an existing Threat-Actor entity.
+        fields of an existing Threat-Actor-Individual entity.
 
         The create method accepts the following kwargs.
 
         Note: `name` and `description` or `stix_id` is required.
 
-        :param str stix_id: stix2 id reference for the Threat-Actor entity
+        :param str stix_id: stix2 id reference for the Threat-Actor-Individual entity
         :param str createdBy: (optional) id of the organization that created the knowledge
         :param list objectMarking: (optional) list of OpenCTI markin definition ids
         :param list objectLabel: (optional) list of OpenCTI label ids
         :param list externalReferences: (optional) list of OpenCTI external references ids
         :param bool revoked: is this entity revoked
         :param int confidence: confidence level
         :param str lang: language
         :param str created: (optional) date in OpenCTI date format
         :param str modified: (optional) date in OpenCTI date format
-        :param str name: name of the threat actor
-        :param str description: description of the threat actor
-        :param list aliases: (optional) list of alias names for the Threat-Actor
+        :param str name: name of the threat actor individual
+        :param str description: description of the threat actor individual
+        :param list aliases: (optional) list of alias names for the Threat-Actor-Individual
         :param list threat_actor_types: (optional) list of threat actor types
         :param str first_seen: (optional) date in OpenCTI date format
         :param str last_seen: (optional) date in OpenCTI date format
         :param list roles: (optional) list of roles
         :param list goals: (optional) list of goals
         :param str sophistication: (optional) describe the actors sophistication in text
         :param str resource_level: (optional) describe the actors resource_level in text
         :param str primary_motivation: (optional) describe the actors primary_motivation in text
         :param list secondary_motivations: (optional) describe the actors secondary_motivations in list of string
         :param list personal_motivations: (optional) describe the actors personal_motivations in list of strings
-        :param bool update: (optional) choose to updated an existing Threat-Actor entity, default `False`
+        :param bool update: (optional) choose to updated an existing Threat-Actor-Individual entity, default `False`
         """
 
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
         external_references = kwargs.get("externalReferences", None)
@@ -326,18 +332,18 @@
         secondary_motivations = kwargs.get("secondary_motivations", None)
         personal_motivations = kwargs.get("personal_motivations", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
-            LOGGER.info("Creating Threat-Actor {%s}.", name)
+            LOGGER.info("Creating Threat-Actor-Individual {%s}.", name)
             query = """
-                mutation ThreatActorAdd($input: ThreatActorAddInput!) {
-                    threatActorAdd(input: $input) {
+                mutation ThreatActorIndividualAdd($input: ThreatActorIndividualAddInput!) {
+                    threatActorIndividualAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
             """
@@ -370,23 +376,23 @@
                         "personal_motivations": personal_motivations,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
                         "update": update,
                     }
                 },
             )
             return self.opencti.process_multiple_fields(
-                result["data"]["threatActorAdd"]
+                result["data"]["threatActorIndividualAdd"]
             )
         else:
             LOGGER.error(
-                "[opencti_threat_actor] Missing parameters: name and description"
+                "[opencti_threat_actor_individual] Missing parameters: name and description"
             )
 
     """
-        Import an Threat-Actor object from a STIX2 object
+        Import an Threat-Actor-Individual object from a STIX2 object
 
         :param stixObject: the Stix-Object Intrusion-Set
         :return Intrusion-Set object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
@@ -461,8 +467,10 @@
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            LOGGER.error("[opencti_threat_actor] Missing parameters: stixObject")
+            LOGGER.error(
+                "[opencti_threat_actor_individual] Missing parameters: stixObject"
+            )
```

### Comparing `pycti-5.8.7/pycti/entities/opencti_tool.py` & `pycti-5.9.0/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_vocabulary.py` & `pycti-5.9.0/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/entities/opencti_vulnerability.py` & `pycti-5.9.0/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/utils/constants.py` & `pycti-5.9.0/pycti/utils/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,23 @@
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
         return value.lower() in lower_attr
 
 
+class ThreatActorTypes(Enum):
+    THREAT_ACTOR_GROUP = "Threat-Actor-Group"
+
+    @classmethod
+    def has_value(cls, value):
+        lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
+        return value.lower() in lower_attr
+
+
 class LocationTypes(Enum):
     REGION = "Region"
     COUNTRY = "Country"
     ADMINISTRATIVE_AREA = "Administrative-Area"
     CITY = "City"
     POSITION = "Position"
```

### Comparing `pycti-5.8.7/pycti/utils/opencti_stix2.py` & `pycti-5.9.0/pycti/utils/opencti_stix2.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pycti.api import LOGGER as API_LOGGER
 from pycti.entities.opencti_identity import Identity
 from pycti.utils.constants import (
     IdentityTypes,
     LocationTypes,
     MultipleRefRelationship,
     StixCyberObservableTypes,
+    ThreatActorTypes,
 )
 from pycti.utils.opencti_stix2_splitter import OpenCTIStix2Splitter
 from pycti.utils.opencti_stix2_update import OpenCTIStix2Update
 from pycti.utils.opencti_stix2_utils import (
     OBSERVABLES_VALUE_INT,
     STIX_CYBER_OBSERVABLE_MAPPING,
 )
@@ -178,15 +179,15 @@
         :type types: list, optional
         :return: list of imported stix2 objects
         :rtype: List
         """
         if not os.path.isfile(file_path):
             API_LOGGER.error("The bundle file does not exists")
             return None
-        with open(os.path.join(file_path)) as file:
+        with open(os.path.join(file_path), encoding="utf-8") as file:
             data = json.load(file)
         return self.import_bundle(data, update, types)
 
     def import_bundle_from_json(
         self,
         json_data: Union[str, bytes],
         update: bool = False,
@@ -556,15 +557,15 @@
                             file_name=file["name"],
                             data=base64.b64decode(file["data"]),
                             mime_type=file["mime_type"],
                         )
                 self.mapping_cache[generated_ref_id] = generated_ref_id
                 external_references_ids.append(external_reference_id)
                 if stix_object["type"] in [
-                    "threat-actor",
+                    "threat-actor-group",
                     "intrusion-set",
                     "campaign",
                     "incident",
                     "malware",
                     "relationship",
                 ] and (types is not None and "external-reference-as-report" in types):
                     # Add a corresponding report
@@ -1232,18 +1233,28 @@
             return None
 
     # endregion
 
     # region export
     def generate_export(self, entity: Dict, no_custom_attributes: bool = False) -> Dict:
         # Handle model deviation
+        original_entity_type = entity["entity_type"]
+
         # Identities
         if IdentityTypes.has_value(entity["entity_type"]):
             entity["entity_type"] = "Identity"
 
+        # Threat-Actors
+        if ThreatActorTypes.has_value(entity["entity_type"]):
+            if not no_custom_attributes:
+                entity["x_opencti_type"] = entity["entity_type"]
+            if entity["entity_type"] == "Threat-Actor-Group":
+                entity["threat_actor_group"] = entity["name"]
+            entity["entity_type"] = "Threat-Actor"
+
         # Locations
         if LocationTypes.has_value(entity["entity_type"]):
             if not no_custom_attributes:
                 entity["x_opencti_location_type"] = entity["entity_type"]
             if entity["entity_type"] == "City":
                 entity["city"] = entity["name"]
             elif entity["entity_type"] == "Country":
@@ -1253,14 +1264,20 @@
             entity["entity_type"] = "Location"
 
         # Malware
         if entity["entity_type"] == "Malware":
             if "is_family" not in entity or not isinstance(entity["is_family"], bool):
                 entity["is_family"] = True
 
+        # Threat Actor
+        if entity["entity_type"] == "Threat-Actor-Group":
+            entity["entity_type"] = "Threat-Actor"
+        if entity["entity_type"] == "Threat-Actor-Individual":
+            entity["entity_type"] = "Threat-Actor"
+
         # Files
         if entity["entity_type"] == "StixFile":
             entity["entity_type"] = "File"
 
         # Case Incident
         if entity["entity_type"] == "Case-Incident":
             entity["standard_id"] = "x-opencti-" + entity["standard_id"]
@@ -1394,14 +1411,15 @@
             entity["hashes"] = {}
             for hash in hashes:
                 entity["hashes"][hash["algorithm"]] = hash["hash"]
 
         # Final
         if not no_custom_attributes:
             entity["x_opencti_id"] = entity["id"]
+            entity["x_opencti_type"] = original_entity_type
         entity["id"] = entity["standard_id"]
         entity["type"] = entity["entity_type"].lower()
         del entity["standard_id"]
         del entity["entity_type"]
         del entity["parent_types"]
         if "created_at" in entity:
             del entity["created_at"]
@@ -1554,35 +1572,35 @@
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
                     entity["type"] == "grouping"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
-                    entity["type"] == "case-incident"
+                    entity["type"] == "x-opencti-case-incident"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
-                    entity["type"] == "feedback"
+                    entity["type"] == "x-opencti-feedback"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
-                    entity["type"] == "case-rfi"
+                    entity["type"] == "x-opencti-case-rfi"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
-                    entity["type"] == "case-rft"
+                    entity["type"] == "x-opencti-case-rft"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
                 elif (
-                    entity["type"] == "task"
+                    entity["type"] == "x-opencti-task"
                     and "stix-ref-relationship" not in entity_object["parent_types"]
                 ):
                     entity["object_refs"].append(entity_object["standard_id"])
         if "objects" in entity:
             del entity["objects"]
             del entity["objectsIds"]
         # Stix Sighting Relationship
@@ -1824,15 +1842,16 @@
                 "Indicator": self.opencti.indicator.read,
                 "Infrastructure": self.opencti.infrastructure.read,
                 "Intrusion-Set": self.opencti.intrusion_set.read,
                 "Location": self.opencti.location.read,
                 "Language": self.opencti.language.read,
                 "Malware": self.opencti.malware.read,
                 "Malware-Analysis": self.opencti.malware_analysis.read,
-                "Threat-Actor": self.opencti.threat_actor.read,
+                "Threat-Actor-Group": self.opencti.threat_actor_group.read,
+                "Threat-Actor-Individual": self.opencti.threat_actor_individual.read,
                 "Tool": self.opencti.tool.read,
                 "Vulnerability": self.opencti.vulnerability.read,
                 "Incident": self.opencti.incident.read,
                 "Stix-Core-Object": self.opencti.stix_core_object.read,
                 "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
                 "Stix-Domain-Object": self.opencti.stix_domain_object.read,
                 "stix-core-relationship": self.opencti.stix_core_relationship.read,
@@ -1992,15 +2011,16 @@
             "Indicator": self.opencti.indicator.read,
             "Infrastructure": self.opencti.infrastructure.read,
             "Intrusion-Set": self.opencti.intrusion_set.read,
             "Location": self.opencti.location.read,
             "Language": self.opencti.language.read,
             "Malware": self.opencti.malware.read,
             "Malware-Analysis": self.opencti.malware_analysis.read,
-            "Threat-Actor": self.opencti.threat_actor.read,
+            "Threat-Actor-Group": self.opencti.threat_actor_group.read,
+            "Threat-Actor-Individual": self.opencti.threat_actor_individual.read,
             "Tool": self.opencti.tool.read,
             "Narrative": self.opencti.narrative.read,
             "Vulnerability": self.opencti.vulnerability.read,
             "Incident": self.opencti.incident.read,
             "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
             "stix-core-relationship": self.opencti.stix_core_relationship.read,
         }
@@ -2135,15 +2155,16 @@
             "Indicator": self.opencti.indicator.list,
             "Infrastructure": self.opencti.infrastructure.list,
             "Intrusion-Set": self.opencti.intrusion_set.list,
             "Location": self.opencti.location.list,
             "Language": self.opencti.language.list,
             "Malware": self.opencti.malware.list,
             "Malware-Analysis": self.opencti.malware_analysis.list,
-            "Threat-Actor": self.opencti.threat_actor.list,
+            "Threat-Actor-Group": self.opencti.threat_actor_group.list,
+            "Threat-Actor-Individual": self.opencti.threat_actor_individual.list,
             "Tool": self.opencti.tool.list,
             "Narrative": self.opencti.narrative.list,
             "Vulnerability": self.opencti.vulnerability.list,
             "Incident": self.opencti.incident.list,
             "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.list,
             "stix-sighting-relationship": self.opencti.stix_sighting_relationship.list,
             "stix-core-relationship": self.opencti.stix_core_relationship.list,
```

### Comparing `pycti-5.8.7/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.9.0/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/utils/opencti_stix2_update.py` & `pycti-5.9.0/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti/utils/opencti_stix2_utils.py` & `pycti-5.9.0/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pycti.egg-info/PKG-INFO` & `pycti-5.9.0/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.8.7
+Version: 5.9.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.8.7 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.0 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.8.7/pycti.egg-info/SOURCES.txt` & `pycti-5.9.0/pycti.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 pycti/entities/opencti_stix_cyber_observable.py
 pycti/entities/opencti_stix_domain_object.py
 pycti/entities/opencti_stix_nested_ref_relationship.py
 pycti/entities/opencti_stix_object_or_stix_relationship.py
 pycti/entities/opencti_stix_sighting_relationship.py
 pycti/entities/opencti_task.py
 pycti/entities/opencti_threat_actor.py
+pycti/entities/opencti_threat_actor_group.py
+pycti/entities/opencti_threat_actor_individual.py
 pycti/entities/opencti_tool.py
 pycti/entities/opencti_vocabulary.py
 pycti/entities/opencti_vulnerability.py
 pycti/utils/__init__.py
 pycti/utils/constants.py
 pycti/utils/opencti_stix2.py
 pycti/utils/opencti_stix2_splitter.py
```

### Comparing `pycti-5.8.7/pycti.egg-info/requires.txt` & `pycti-5.9.0/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/pyproject.toml` & `pycti-5.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.8.7/setup.cfg` & `pycti-5.9.0/setup.cfg`

 * *Files identical despite different names*

