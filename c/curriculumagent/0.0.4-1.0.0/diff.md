# Comparing `tmp/curriculumagent-0.0.4.tar.gz` & `tmp/curriculumagent-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curriculumagent-0.0.4.tar", last modified: Sun Jul  9 16:30:47 2023, max compression
+gzip compressed data, was "curriculumagent-1.0.0.tar", last modified: Mon Jul 10 13:33:27 2023, max compression
```

## Comparing `curriculumagent-0.0.4.tar` & `curriculumagent-1.0.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.825581 curriculumagent-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-09 16:30:47.825581 curriculumagent-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.829581 curriculumagent-0.0.4/curriculumagent/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-09 16:30:47.829581 curriculumagent-0.0.4/curriculumagent/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.813581 curriculumagent-0.0.4/curriculumagent/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/baseline/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/baseline/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/baseline/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.813581 curriculumagent-0.0.4/curriculumagent/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/common/obs_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/common/score_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/common/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.813581 curriculumagent-0.0.4/curriculumagent/junior/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/junior/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.813581 curriculumagent-0.0.4/curriculumagent/junior/hyper_parameter_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/junior/hyper_parameter_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/junior/hyper_parameter_search/advanced_junior_student.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/junior/hyper_parameter_search/hyper_parameter_search_junior.py
--rw-r--r--   0 runner    (1001) docker     (123)    19532 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/junior/junior_student.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.817581 curriculumagent-0.0.4/curriculumagent/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/scripts/get_seed_wcci2022.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.817581 curriculumagent-0.0.4/curriculumagent/senior/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.817581 curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/alternative_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/senior_env_rllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/senior_model_rllib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/senior_student.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/senior/senior_student_advanced.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.821581 curriculumagent-0.0.4/curriculumagent/submission/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/submission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/submission/my_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.821581 curriculumagent-0.0.4/curriculumagent/teacher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/collect_teacher_experience.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.821581 curriculumagent-0.0.4/curriculumagent/teacher/submodule/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/submodule/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/submodule/encoded_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/submodule/topology_action_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teacher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.825581 curriculumagent-0.0.4/curriculumagent/teacher/teachers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teachers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher_n_minus_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher_sequential_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/teacher/teachers/tuple_triple_teacher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.825581 curriculumagent-0.0.4/curriculumagent/tutor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/collect_divergent_powerflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/collect_tutor_experience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/tutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.825581 curriculumagent-0.0.4/curriculumagent/tutor/tutors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/tutors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/tutors/general_tutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-09 16:28:23.000000 curriculumagent-0.0.4/curriculumagent/tutor/tutors/n_minus_one_tutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.809581 curriculumagent-0.0.4/curriculumagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-09 16:30:47.000000 curriculumagent-0.0.4/curriculumagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-09 16:30:47.000000 curriculumagent-0.0.4/curriculumagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:30:47.000000 curriculumagent-0.0.4/curriculumagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:30:47.000000 curriculumagent-0.0.4/curriculumagent.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-09 16:30:47.000000 curriculumagent-0.0.4/curriculumagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 16:30:47.000000 curriculumagent-0.0.4/curriculumagent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:30:47.825581 curriculumagent-0.0.4/paper_data_MPGTTA/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 16:28:25.000000 curriculumagent-0.0.4/paper_data_MPGTTA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-09 16:28:25.000000 curriculumagent-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-09 16:28:25.000000 curriculumagent-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-09 16:30:47.829581 curriculumagent-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-09 16:28:25.000000 curriculumagent-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-07-09 16:28:27.000000 curriculumagent-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/curriculumagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/curriculumagent/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.226027 curriculumagent-1.0.0/curriculumagent/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/baseline/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/baseline/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/baseline/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.226027 curriculumagent-1.0.0/curriculumagent/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/common/obs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/common/score_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/common/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.226027 curriculumagent-1.0.0/curriculumagent/junior/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/junior/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.226027 curriculumagent-1.0.0/curriculumagent/junior/hyper_parameter_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/junior/hyper_parameter_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/junior/hyper_parameter_search/advanced_junior_student.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/junior/hyper_parameter_search/hyper_parameter_search_junior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19532 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/junior/junior_student.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.226027 curriculumagent-1.0.0/curriculumagent/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/scripts/get_seed_wcci2022.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.230027 curriculumagent-1.0.0/curriculumagent/senior/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.230027 curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/alternative_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/senior_env_rllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/senior_model_rllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/senior_student.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/senior/senior_student_advanced.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.234027 curriculumagent-1.0.0/curriculumagent/submission/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/submission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/submission/my_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.234027 curriculumagent-1.0.0/curriculumagent/teacher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/collect_teacher_experience.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.234027 curriculumagent-1.0.0/curriculumagent/teacher/submodule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/submodule/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/submodule/encoded_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/submodule/topology_action_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.238027 curriculumagent-1.0.0/curriculumagent/teacher/teachers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teachers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher_n_minus_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher_sequential_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/teacher/teachers/tuple_triple_teacher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.238027 curriculumagent-1.0.0/curriculumagent/tutor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/collect_divergent_powerflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/collect_tutor_experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/tutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/curriculumagent/tutor/tutors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/tutors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/tutors/general_tutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-10 13:30:42.000000 curriculumagent-1.0.0/curriculumagent/tutor/tutors/n_minus_one_tutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.222027 curriculumagent-1.0.0/curriculumagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-10 13:33:27.000000 curriculumagent-1.0.0/curriculumagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-10 13:33:27.000000 curriculumagent-1.0.0/curriculumagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:33:27.000000 curriculumagent-1.0.0/curriculumagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:33:27.000000 curriculumagent-1.0.0/curriculumagent.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-10 13:33:27.000000 curriculumagent-1.0.0/curriculumagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 13:33:27.000000 curriculumagent-1.0.0/curriculumagent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/paper_data_MPGTTA/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:30:44.000000 curriculumagent-1.0.0/paper_data_MPGTTA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 13:30:44.000000 curriculumagent-1.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 13:30:44.000000 curriculumagent-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 13:33:27.242027 curriculumagent-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-10 13:30:44.000000 curriculumagent-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-07-10 13:30:46.000000 curriculumagent-1.0.0/versioneer.py
```

### Comparing `curriculumagent-0.0.4/LICENSE` & `curriculumagent-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/PKG-INFO` & `curriculumagent-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: curriculumagent
-Version: 0.0.4
+Version: 1.0.0
+Summary: CurriculumAgent is a cleanup and improved version of the NeurIPS 2020 Competition Agent by Binbinchen.The agent is build to extract action sets of the Grid2Op Environment and then use rule-based agent to train a Reinforcement Learning agent.
 Author: OE224
-Project-URL: JIRA, https://applik-20-dmz.iee.fraunhofer.de/
-Project-URL: GITLAB, https://gitlab.cc-asp.fraunhofer.de/iee_oe224/aidev/grid2op/curriculumagent
-Classifier: Development Status :: 3 - Alpha
+Project-URL: GITHUB, https://github.com/FraunhoferIEE/curriculumagent/
+Project-URL: Readthedocs, https://curriculumagent.readthedocs.io/en/latest/
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -41,15 +42,15 @@
 All requirements are listed in `requirements.txt`.
 
 Installing the package should already give you all needed requirements.
 
 Usage/Documentation
 -------------------
 
-Please take a look at our [sphinx documentation](#) on how to use the package.
+Please take a look at our [sphinx documentation](https://curriculumagent.readthedocs.io/en/latest/) on how to use the package.
 
 We also provide several jupyter notebooks in `./jupyter_notebooks` to get you started quickly.
 
 
 
 License
 -------
```

### Comparing `curriculumagent-0.0.4/README.md` & `curriculumagent-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 All requirements are listed in `requirements.txt`.
 
 Installing the package should already give you all needed requirements.
 
 Usage/Documentation
 -------------------
 
-Please take a look at our [sphinx documentation](#) on how to use the package.
+Please take a look at our [sphinx documentation](https://curriculumagent.readthedocs.io/en/latest/) on how to use the package.
 
 We also provide several jupyter notebooks in `./jupyter_notebooks` to get you started quickly.
 
 
 
 License
 -------
```

### Comparing `curriculumagent-0.0.4/curriculumagent/baseline/baseline.py` & `curriculumagent-1.0.0/curriculumagent/baseline/baseline.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/baseline/evaluate.py` & `curriculumagent-1.0.0/curriculumagent/baseline/evaluate.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/baseline/train.py` & `curriculumagent-1.0.0/curriculumagent/baseline/train.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/common/obs_converter.py` & `curriculumagent-1.0.0/curriculumagent/common/obs_converter.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/common/score_agent.py` & `curriculumagent-1.0.0/curriculumagent/common/score_agent.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/common/utilities.py` & `curriculumagent-1.0.0/curriculumagent/common/utilities.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/junior/hyper_parameter_search/hyper_parameter_search_junior.py` & `curriculumagent-1.0.0/curriculumagent/junior/hyper_parameter_search/hyper_parameter_search_junior.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/junior/junior_student.py` & `curriculumagent-1.0.0/curriculumagent/junior/junior_student.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/scripts/get_seed_wcci2022.py` & `curriculumagent-1.0.0/curriculumagent/scripts/get_seed_wcci2022.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/alternative_rewards.py` & `curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/alternative_rewards.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/senior_env_rllib.py` & `curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/senior_env_rllib.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/senior/rllib_execution/senior_model_rllib.py` & `curriculumagent-1.0.0/curriculumagent/senior/rllib_execution/senior_model_rllib.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/senior/senior_student.py` & `curriculumagent-1.0.0/curriculumagent/senior/senior_student.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/senior/senior_student_advanced.py` & `curriculumagent-1.0.0/curriculumagent/senior/senior_student_advanced.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/submission/my_agent.py` & `curriculumagent-1.0.0/curriculumagent/submission/my_agent.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/collect_teacher_experience.py` & `curriculumagent-1.0.0/curriculumagent/teacher/collect_teacher_experience.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/submodule/common.py` & `curriculumagent-1.0.0/curriculumagent/teacher/submodule/common.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/submodule/encoded_action.py` & `curriculumagent-1.0.0/curriculumagent/teacher/submodule/encoded_action.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/submodule/topology_action_search.py` & `curriculumagent-1.0.0/curriculumagent/teacher/submodule/topology_action_search.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/teacher.py` & `curriculumagent-1.0.0/curriculumagent/teacher/teacher.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher1.py` & `curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher1.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher2.py` & `curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher2.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher_n_minus_1.py` & `curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher_n_minus_1.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/teachers/teacher_sequential_actions.py` & `curriculumagent-1.0.0/curriculumagent/teacher/teachers/teacher_sequential_actions.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/teacher/teachers/tuple_triple_teacher.py` & `curriculumagent-1.0.0/curriculumagent/teacher/teachers/tuple_triple_teacher.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/tutor/collect_divergent_powerflow.py` & `curriculumagent-1.0.0/curriculumagent/tutor/collect_divergent_powerflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,10 +184,9 @@
 
     # Now concatenate the result:
     all_experience = np.concatenate(out_result, axis=0)
     if save_path.is_dir():
         now = datetime.now().strftime("%d%m%Y_%H%M%S")
         save_path = save_path / f"divergent_powerflow_{now}.npy"
 
-    # TODO: Should use savez_compressed since data has low entropy, have to adapt junior as well
     np.save(save_path, all_experience)
     logging.info(f"Divergent PF teacher_experience has been saved to {save_path}")
```

### Comparing `curriculumagent-0.0.4/curriculumagent/tutor/collect_tutor_experience.py` & `curriculumagent-1.0.0/curriculumagent/tutor/collect_tutor_experience.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/tutor/tutor.py` & `curriculumagent-1.0.0/curriculumagent/tutor/tutor.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/tutor/tutors/general_tutor.py` & `curriculumagent-1.0.0/curriculumagent/tutor/tutors/general_tutor.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent/tutor/tutors/n_minus_one_tutor.py` & `curriculumagent-1.0.0/curriculumagent/tutor/tutors/n_minus_one_tutor.py`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/curriculumagent.egg-info/PKG-INFO` & `curriculumagent-1.0.0/curriculumagent.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: curriculumagent
-Version: 0.0.4
+Version: 1.0.0
+Summary: CurriculumAgent is a cleanup and improved version of the NeurIPS 2020 Competition Agent by Binbinchen.The agent is build to extract action sets of the Grid2Op Environment and then use rule-based agent to train a Reinforcement Learning agent.
 Author: OE224
-Project-URL: JIRA, https://applik-20-dmz.iee.fraunhofer.de/
-Project-URL: GITLAB, https://gitlab.cc-asp.fraunhofer.de/iee_oe224/aidev/grid2op/curriculumagent
-Classifier: Development Status :: 3 - Alpha
+Project-URL: GITHUB, https://github.com/FraunhoferIEE/curriculumagent/
+Project-URL: Readthedocs, https://curriculumagent.readthedocs.io/en/latest/
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -41,15 +42,15 @@
 All requirements are listed in `requirements.txt`.
 
 Installing the package should already give you all needed requirements.
 
 Usage/Documentation
 -------------------
 
-Please take a look at our [sphinx documentation](#) on how to use the package.
+Please take a look at our [sphinx documentation](https://curriculumagent.readthedocs.io/en/latest/) on how to use the package.
 
 We also provide several jupyter notebooks in `./jupyter_notebooks` to get you started quickly.
 
 
 
 License
 -------
```

### Comparing `curriculumagent-0.0.4/curriculumagent.egg-info/SOURCES.txt` & `curriculumagent-1.0.0/curriculumagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curriculumagent-0.0.4/setup.py` & `curriculumagent-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,22 +31,20 @@
         'sphinx-autodoc-typehints',  # use typehints to provide types
     ],
     'dev': [
         r for r in requirements_dev if not r.startswith('-r ')
     ],
 }
 
-URLS = {
-    'JIRA': 'https://applik-20-dmz.iee.fraunhofer.de/',  # TODO: add link to project
-    'GITLAB': 'https://gitlab.cc-asp.fraunhofer.de/iee_oe224/aidev/grid2op/curriculumagent',  # TODO add link for this to coookiecutter props?
-    # 'Documentation': '???',  # should link to the docs
+URLS = {'GITHUB': 'https://github.com/FraunhoferIEE/curriculumagent/',
+        'Readthedocs': 'https://curriculumagent.readthedocs.io/en/latest/'
 }
 SCRIPTS = []  # no scripts necessary
 CLASSIFIERS = [
-    'Development Status :: 3 - Alpha',  # TODO: change classifiers
+    'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3.10',
 ]
 
 # ======================================================================================
 # No configurable options below this line
 
 # Get current version etc. from the `__about__.py` file --------------------------------
@@ -66,15 +64,15 @@
 #    raise RuntimeError("Unable to find version string for the package.")
 
 
 if __name__ == '__main__':
     setup(
         # General ---
         name=PACKAGE_NAME,
-        verion=versioneer.get_version(),
+        version=versioneer.get_version(),
         cmdclass=versioneer.get_cmdclass(),
 
         packages=find_packages(exclude=['docs', 'tests', 'tests.*']),
         namespace_packages=([NAMESPACE] if NAMESPACE else []),
         scripts=SCRIPTS,
 
         install_requires=requirements['install'],
```

### Comparing `curriculumagent-0.0.4/versioneer.py` & `curriculumagent-1.0.0/versioneer.py`

 * *Files identical despite different names*

