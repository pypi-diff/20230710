# Comparing `tmp/deprl-0.1.3.tar.gz` & `tmp/deprl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprl-0.1.3.tar", max compression
+gzip compressed data, was "deprl-0.1.4.tar", max compression
```

## Comparing `deprl-0.1.3.tar` & `deprl-0.1.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     1083 2023-06-02 09:47:22.460278 deprl-0.1.3/LICENSE
--rw-r--r--   0        0        0     8275 2023-07-03 13:07:50.974017 deprl-0.1.3/README.md
--rw-r--r--   0        0        0      529 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/__init__.py
--rw-r--r--   0        0        0     5819 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/custom_agents.py
--rw-r--r--   0        0        0     8956 2023-07-03 13:04:45.751697 deprl-0.1.3/deprl/custom_distributed.py
--rw-r--r--   0        0        0     3639 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/custom_mpo_torch.py
--rw-r--r--   0        0        0     3541 2023-07-03 13:04:45.755697 deprl-0.1.3/deprl/custom_test_environment.py
--rw-r--r--   0        0        0     1244 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/custom_torso.py
--rw-r--r--   0        0        0     5818 2023-07-03 13:04:43.611717 deprl-0.1.3/deprl/custom_trainer.py
--rw-r--r--   0        0        0     7373 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/dep_controller.py
--rw-r--r--   0        0        0      132 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/env_wrappers/__init__.py
--rw-r--r--   0        0        0     5830 2023-07-03 13:04:45.751697 deprl-0.1.3/deprl/env_wrappers/wrappers.py
--rw-r--r--   0        0        0     2175 2023-07-03 13:09:32.537103 deprl-0.1.3/deprl/log.py
--rw-r--r--   0        0        0     7722 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/main.py
--rw-r--r--   0        0        0      704 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/param_files/default_agents.json
--rw-r--r--   0        0        0     9038 2023-07-03 13:04:43.611717 deprl-0.1.3/deprl/play.py
--rw-r--r--   0        0        0    10215 2023-06-02 11:10:09.686883 deprl-0.1.3/deprl/play_plot.py
--rw-r--r--   0        0        0       80 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/plot.py
--rw-r--r--   0        0        0    12908 2023-06-02 13:04:44.683480 deprl-0.1.3/deprl/record_data_myoleg.py
--rw-r--r--   0        0        0      179 2023-07-03 13:04:45.751697 deprl-0.1.3/deprl/utils/__init__.py
--rw-r--r--   0        0        0     3053 2023-07-03 13:04:45.751697 deprl-0.1.3/deprl/utils/analysis_utils.py
--rw-r--r--   0        0        0     3741 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/utils/utils.py
--rw-r--r--   0        0        0       39 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/__init__.py
--rwxr-xr-x   0        0        0       80 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/.gitignore
--rw-r--r--   0        0        0     1110 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/LICENSE
--rw-r--r--   0        0        0      207 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/__init__.py
--rw-r--r--   0        0        0      178 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/agents/__init__.py
--rw-r--r--   0        0        0     1038 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/agents/agent.py
--rw-r--r--   0        0        0     3954 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/agents/basic.py
--rw-r--r--   0        0        0      293 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/environments/__init__.py
--rw-r--r--   0        0        0     5731 2023-07-03 13:04:45.751697 deprl-0.1.3/deprl/vendor/tonic/environments/builders.py
--rw-r--r--   0        0        0     6612 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/environments/distributed.py
--rw-r--r--   0        0        0     1914 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/environments/wrappers.py
--rw-r--r--   0        0        0      175 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/explorations/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/explorations/noisy.py
--rw-r--r--   0        0        0     8754 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/play.py
--rw-r--r--   0        0        0    18151 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/plot.py
--rw-r--r--   0        0        0      167 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/replays/__init__.py
--rw-r--r--   0        0        0     3636 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/replays/buffers.py
--rw-r--r--   0        0        0     2815 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/replays/segments.py
--rw-r--r--   0        0        0      821 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/replays/utils.py
--rw-r--r--   0        0        0      103 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/__init__.py
--rw-r--r--   0        0        0      303 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/__init__.py
--rw-r--r--   0        0        0     4630 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/a2c.py
--rw-r--r--   0        0        0      519 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/agent.py
--rw-r--r--   0        0        0     1456 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/d4pg.py
--rw-r--r--   0        0        0     4327 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/ddpg.py
--rw-r--r--   0        0        0     4089 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/mpo.py
--rw-r--r--   0        0        0     2452 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/ppo.py
--rw-r--r--   0        0        0     1868 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/sac.py
--rw-r--r--   0        0        0     2181 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/td3.py
--rw-r--r--   0        0        0     1448 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/td4.py
--rw-r--r--   0        0        0     3754 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/trpo.py
--rw-r--r--   0        0        0      819 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     6247 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/actor_critics.py
--rw-r--r--   0        0        0     4849 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/actors.py
--rw-r--r--   0        0        0     3046 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/critics.py
--rw-r--r--   0        0        0      734 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/encoders.py
--rw-r--r--   0        0        0      627 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/utils.py
--rw-r--r--   0        0        0       88 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
--rw-r--r--   0        0        0     2442 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1339 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/normalizers/returns.py
--rw-r--r--   0        0        0     1260 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/__init__.py
--rw-r--r--   0        0        0    19301 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/actors.py
--rw-r--r--   0        0        0    13820 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/critics.py
--rw-r--r--   0        0        0     4232 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
--rw-r--r--   0        0        0      193 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/utils.py
--rw-r--r--   0        0        0      103 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/__init__.py
--rw-r--r--   0        0        0      277 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/__init__.py
--rw-r--r--   0        0        0     5287 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/a2c.py
--rw-r--r--   0        0        0     1441 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/agent.py
--rw-r--r--   0        0        0     1522 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/d4pg.py
--rw-r--r--   0        0        0     4551 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/ddpg.py
--rw-r--r--   0        0        0     4446 2023-05-17 09:04:59.808056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/mpo.py
--rw-r--r--   0        0        0     2608 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/ppo.py
--rw-r--r--   0        0        0     2102 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/sac.py
--rw-r--r--   0        0        0     2315 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/td3.py
--rw-r--r--   0        0        0     4077 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/agents/trpo.py
--rw-r--r--   0        0        0      817 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/models/__init__.py
--rw-r--r--   0        0        0     5824 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/models/actor_critics.py
--rw-r--r--   0        0        0     4874 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/models/actors.py
--rw-r--r--   0        0        0     3177 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/models/critics.py
--rw-r--r--   0        0        0     1084 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/models/encoders.py
--rw-r--r--   0        0        0      791 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/models/utils.py
--rw-r--r--   0        0        0       88 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/normalizers/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/normalizers/mean_stds.py
--rw-r--r--   0        0        0     1429 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/normalizers/returns.py
--rw-r--r--   0        0        0     1156 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/updaters/__init__.py
--rw-r--r--   0        0        0    20504 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/updaters/actors.py
--rw-r--r--   0        0        0    11054 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/updaters/critics.py
--rw-r--r--   0        0        0     4317 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/updaters/optimizers.py
--rw-r--r--   0        0        0      156 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/torch/updaters/utils.py
--rw-r--r--   0        0        0     5722 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/train.py
--rw-r--r--   0        0        0      213 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/utils/__init__.py
--rw-r--r--   0        0        0      822 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/utils/csv_utils.py
--rw-r--r--   0        0        0     8867 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/utils/logger.py
--rw-r--r--   0        0        0     5477 2023-05-17 09:04:59.812056 deprl-0.1.3/deprl/vendor/tonic/utils/trainer.py
--rw-r--r--   0        0        0     1276 2023-07-03 13:08:40.689569 deprl-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9136 1970-01-01 00:00:00.000000 deprl-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-02 09:47:22.460278 deprl-0.1.4/LICENSE
+-rw-r--r--   0        0        0     8275 2023-07-03 13:07:50.974017 deprl-0.1.4/README.md
+-rw-r--r--   0        0        0      563 2023-07-10 12:45:43.022418 deprl-0.1.4/deprl/__init__.py
+-rw-r--r--   0        0        0     5819 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/custom_agents.py
+-rw-r--r--   0        0        0     8956 2023-07-03 13:04:45.751697 deprl-0.1.4/deprl/custom_distributed.py
+-rw-r--r--   0        0        0     3639 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/custom_mpo_torch.py
+-rw-r--r--   0        0        0     3541 2023-07-03 13:04:45.755697 deprl-0.1.4/deprl/custom_test_environment.py
+-rw-r--r--   0        0        0     1244 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/custom_torso.py
+-rw-r--r--   0        0        0     5818 2023-07-03 13:04:43.611717 deprl-0.1.4/deprl/custom_trainer.py
+-rw-r--r--   0        0        0     7373 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/dep_controller.py
+-rw-r--r--   0        0        0      132 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/env_wrappers/__init__.py
+-rw-r--r--   0        0        0     5830 2023-07-03 13:04:45.751697 deprl-0.1.4/deprl/env_wrappers/wrappers.py
+-rw-r--r--   0        0        0     2175 2023-07-03 13:09:32.537103 deprl-0.1.4/deprl/log.py
+-rw-r--r--   0        0        0     7722 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/main.py
+-rw-r--r--   0        0        0      704 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/param_files/default_agents.json
+-rw-r--r--   0        0        0     9034 2023-07-10 12:45:43.198417 deprl-0.1.4/deprl/play.py
+-rw-r--r--   0        0        0    10215 2023-06-02 11:10:09.686883 deprl-0.1.4/deprl/play_plot.py
+-rw-r--r--   0        0        0       80 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/plot.py
+-rw-r--r--   0        0        0    12908 2023-06-02 13:04:44.683480 deprl-0.1.4/deprl/record_data_myoleg.py
+-rw-r--r--   0        0        0      230 2023-07-10 12:45:43.202417 deprl-0.1.4/deprl/utils/__init__.py
+-rw-r--r--   0        0        0     3053 2023-07-03 13:04:45.751697 deprl-0.1.4/deprl/utils/analysis_utils.py
+-rw-r--r--   0        0        0     3931 2023-07-10 12:45:43.086418 deprl-0.1.4/deprl/utils/utils.py
+-rw-r--r--   0        0        0       39 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/__init__.py
+-rwxr-xr-x   0        0        0       80 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/.gitignore
+-rw-r--r--   0        0        0     1110 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/LICENSE
+-rw-r--r--   0        0        0      207 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/agents/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/agents/agent.py
+-rw-r--r--   0        0        0     3954 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/agents/basic.py
+-rw-r--r--   0        0        0      293 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/environments/__init__.py
+-rw-r--r--   0        0        0     5731 2023-07-03 13:04:45.751697 deprl-0.1.4/deprl/vendor/tonic/environments/builders.py
+-rw-r--r--   0        0        0     6612 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/environments/distributed.py
+-rw-r--r--   0        0        0     1914 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/environments/wrappers.py
+-rw-r--r--   0        0        0      175 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/explorations/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/explorations/noisy.py
+-rw-r--r--   0        0        0     8754 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/play.py
+-rw-r--r--   0        0        0    18151 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/plot.py
+-rw-r--r--   0        0        0      167 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/replays/__init__.py
+-rw-r--r--   0        0        0     3636 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/replays/buffers.py
+-rw-r--r--   0        0        0     2815 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/replays/segments.py
+-rw-r--r--   0        0        0      821 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/replays/utils.py
+-rw-r--r--   0        0        0      103 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/__init__.py
+-rw-r--r--   0        0        0      303 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/__init__.py
+-rw-r--r--   0        0        0     4630 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/a2c.py
+-rw-r--r--   0        0        0      519 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/agent.py
+-rw-r--r--   0        0        0     1456 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/d4pg.py
+-rw-r--r--   0        0        0     4327 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/ddpg.py
+-rw-r--r--   0        0        0     4089 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/mpo.py
+-rw-r--r--   0        0        0     2452 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/ppo.py
+-rw-r--r--   0        0        0     1868 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/sac.py
+-rw-r--r--   0        0        0     2181 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/td3.py
+-rw-r--r--   0        0        0     1448 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/td4.py
+-rw-r--r--   0        0        0     3754 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/trpo.py
+-rw-r--r--   0        0        0      819 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     6247 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/actor_critics.py
+-rw-r--r--   0        0        0     4849 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/actors.py
+-rw-r--r--   0        0        0     3046 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/critics.py
+-rw-r--r--   0        0        0      734 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/encoders.py
+-rw-r--r--   0        0        0      627 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/utils.py
+-rw-r--r--   0        0        0       88 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/normalizers/__init__.py
+-rw-r--r--   0        0        0     2442 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1339 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/normalizers/returns.py
+-rw-r--r--   0        0        0     1260 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/__init__.py
+-rw-r--r--   0        0        0    19301 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/actors.py
+-rw-r--r--   0        0        0    13820 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/critics.py
+-rw-r--r--   0        0        0     4232 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/optimizers.py
+-rw-r--r--   0        0        0      193 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/utils.py
+-rw-r--r--   0        0        0      103 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/__init__.py
+-rw-r--r--   0        0        0      277 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/__init__.py
+-rw-r--r--   0        0        0     5287 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/a2c.py
+-rw-r--r--   0        0        0     1441 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/agent.py
+-rw-r--r--   0        0        0     1522 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/d4pg.py
+-rw-r--r--   0        0        0     4551 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/ddpg.py
+-rw-r--r--   0        0        0     4446 2023-05-17 09:04:59.808056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/mpo.py
+-rw-r--r--   0        0        0     2608 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/ppo.py
+-rw-r--r--   0        0        0     2102 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/sac.py
+-rw-r--r--   0        0        0     2315 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/td3.py
+-rw-r--r--   0        0        0     4077 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/agents/trpo.py
+-rw-r--r--   0        0        0      817 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/models/__init__.py
+-rw-r--r--   0        0        0     5824 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/models/actor_critics.py
+-rw-r--r--   0        0        0     4874 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/models/actors.py
+-rw-r--r--   0        0        0     3177 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/models/critics.py
+-rw-r--r--   0        0        0     1084 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/models/encoders.py
+-rw-r--r--   0        0        0      791 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/models/utils.py
+-rw-r--r--   0        0        0       88 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/normalizers/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/normalizers/mean_stds.py
+-rw-r--r--   0        0        0     1429 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/normalizers/returns.py
+-rw-r--r--   0        0        0     1156 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/updaters/__init__.py
+-rw-r--r--   0        0        0    20504 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/updaters/actors.py
+-rw-r--r--   0        0        0    11054 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/updaters/critics.py
+-rw-r--r--   0        0        0     4317 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/updaters/optimizers.py
+-rw-r--r--   0        0        0      156 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/torch/updaters/utils.py
+-rw-r--r--   0        0        0     5722 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/train.py
+-rw-r--r--   0        0        0      213 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/utils/__init__.py
+-rw-r--r--   0        0        0      822 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/utils/csv_utils.py
+-rw-r--r--   0        0        0     8867 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/utils/logger.py
+-rw-r--r--   0        0        0     5477 2023-05-17 09:04:59.812056 deprl-0.1.4/deprl/vendor/tonic/utils/trainer.py
+-rw-r--r--   0        0        0     1246 2023-07-10 12:46:35.150019 deprl-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9136 1970-01-01 00:00:00.000000 deprl-0.1.4/PKG-INFO
```

### Comparing `deprl-0.1.3/LICENSE` & `deprl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/README.md` & `deprl-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/__init__.py` & `deprl-0.1.4/deprl/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import custom_agents, custom_mpo_torch, custom_trainer
 from .env_wrappers import apply_wrapper, env_tonic_compat
-from .utils import load, load_baseline
+from .utils import load, load_baseline, mujoco_render
 from .vendor.tonic import (
     Trainer,
     agents,
     environments,
     explorations,
     logger,
     replays,
@@ -22,8 +22,9 @@
     environments,
     explorations,
     logger,
     replays,
     Trainer,
     load,
     load_baseline,
+    mujoco_render,
 ]
```

### Comparing `deprl-0.1.3/deprl/custom_agents.py` & `deprl-0.1.4/deprl/custom_agents.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/custom_distributed.py` & `deprl-0.1.4/deprl/custom_distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/custom_mpo_torch.py` & `deprl-0.1.4/deprl/custom_mpo_torch.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/custom_test_environment.py` & `deprl-0.1.4/deprl/custom_test_environment.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/custom_torso.py` & `deprl-0.1.4/deprl/custom_torso.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/custom_trainer.py` & `deprl-0.1.4/deprl/custom_trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/dep_controller.py` & `deprl-0.1.4/deprl/dep_controller.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/env_wrappers/wrappers.py` & `deprl-0.1.4/deprl/env_wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/log.py` & `deprl-0.1.4/deprl/log.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/main.py` & `deprl-0.1.4/deprl/main.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/param_files/default_agents.json` & `deprl-0.1.4/deprl/param_files/default_agents.json`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/play.py` & `deprl-0.1.4/deprl/play.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 import argparse
 import os
 
 import numpy as np
 import yaml
 
-from deprl import env_wrappers
+from deprl import env_wrappers, mujoco_render
 
 from .vendor.tonic import logger
 
 
 def play_gym(agent, environment):
     """Launches an agent in a Gym-based environment."""
     environment = env_wrappers.apply_wrapper(environment)
     observations = environment.reset()
     tendon_states = environment.tendon_states
-    environment.render()
 
     score = 0
     length = 0
     min_reward = float("inf")
     max_reward = -float("inf")
     global_min_reward = float("inf")
     global_max_reward = -float("inf")
@@ -31,15 +30,15 @@
         actions = agent.test_step(
             observations, tendon_states=tendon_states, steps=1e6
         )
         if len(actions.shape) > 1:
             actions = actions[0, :]
         observations, reward, done, info = environment.step(actions)
         tendon_states = environment.tendon_states
-        environment.render()
+        mujoco_render(environment)
 
         steps += 1
         score += reward
         min_reward = min(min_reward, reward)
         max_reward = max(max_reward, reward)
         global_min_reward = min(global_min_reward, reward)
         global_max_reward = max(global_max_reward, reward)
```

### Comparing `deprl-0.1.3/deprl/play_plot.py` & `deprl-0.1.4/deprl/play_plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/record_data_myoleg.py` & `deprl-0.1.4/deprl/record_data_myoleg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/utils/analysis_utils.py` & `deprl-0.1.4/deprl/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/utils/utils.py` & `deprl-0.1.4/deprl/utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -114,7 +114,14 @@
 
     # Load the experiment configuration.
     arguments_path = os.path.join(path, "config.yaml")
     with open(arguments_path, "r") as config_file:
         config = yaml.load(config_file, Loader=yaml.FullLoader)
     config = argparse.Namespace(**config)
     return config, checkpoint_path
+
+
+def mujoco_render(env, *args, **kwargs):
+    if "mujoco_py" in str(type(env.sim)):
+        env.render(*args, **kwargs)
+    else:
+        env.sim.renderer.render_to_window(*args, **kwargs)
```

### Comparing `deprl-0.1.3/deprl/vendor/tonic/LICENSE` & `deprl-0.1.4/deprl/vendor/tonic/LICENSE`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/agents/agent.py` & `deprl-0.1.4/deprl/vendor/tonic/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/agents/basic.py` & `deprl-0.1.4/deprl/vendor/tonic/agents/basic.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/environments/builders.py` & `deprl-0.1.4/deprl/vendor/tonic/environments/builders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/environments/distributed.py` & `deprl-0.1.4/deprl/vendor/tonic/environments/distributed.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/environments/wrappers.py` & `deprl-0.1.4/deprl/vendor/tonic/environments/wrappers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/explorations/noisy.py` & `deprl-0.1.4/deprl/vendor/tonic/explorations/noisy.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/play.py` & `deprl-0.1.4/deprl/vendor/tonic/play.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/plot.py` & `deprl-0.1.4/deprl/vendor/tonic/plot.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/replays/buffers.py` & `deprl-0.1.4/deprl/vendor/tonic/replays/buffers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/replays/segments.py` & `deprl-0.1.4/deprl/vendor/tonic/replays/segments.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/replays/utils.py` & `deprl-0.1.4/deprl/vendor/tonic/replays/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/a2c.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/agent.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/d4pg.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/ddpg.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/mpo.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/ppo.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/sac.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/td3.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/td4.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/td4.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/agents/trpo.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/__init__.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/actor_critics.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/actors.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/critics.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/encoders.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/models/utils.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/normalizers/returns.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/__init__.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/actors.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/critics.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/tensorflow/updaters/optimizers.py` & `deprl-0.1.4/deprl/vendor/tonic/tensorflow/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/a2c.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/a2c.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/agent.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/d4pg.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/d4pg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/ddpg.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/ddpg.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/mpo.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/mpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/ppo.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/sac.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/sac.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/td3.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/td3.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/agents/trpo.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/agents/trpo.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/models/__init__.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/models/actor_critics.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/models/actor_critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/models/actors.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/models/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/models/critics.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/models/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/models/encoders.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/models/utils.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/models/utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/normalizers/mean_stds.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/normalizers/mean_stds.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/normalizers/returns.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/normalizers/returns.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/updaters/__init__.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/updaters/actors.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/updaters/actors.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/updaters/critics.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/updaters/critics.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/torch/updaters/optimizers.py` & `deprl-0.1.4/deprl/vendor/tonic/torch/updaters/optimizers.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/train.py` & `deprl-0.1.4/deprl/vendor/tonic/train.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/utils/csv_utils.py` & `deprl-0.1.4/deprl/vendor/tonic/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/utils/logger.py` & `deprl-0.1.4/deprl/vendor/tonic/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/deprl/vendor/tonic/utils/trainer.py` & `deprl-0.1.4/deprl/vendor/tonic/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `deprl-0.1.3/pyproject.toml` & `deprl-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deprl"
-version = "0.1.3"
+version = "0.1.4"
 description = "DEP-RL, a method for robust control of musculoskeletal systems."
 authors = ["Pierre Schumacher <pierre.schumacher@tuebingen.mpg.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
@@ -22,15 +22,15 @@
 pudb = "*"
 pre-commit = "*"
 wandb = "^0.13.11"
 ostrichrl = {git = "https://github.com/P-Schumacher/ostrichrl.git", branch="fix/setuptools"}
 warmup = {git = "https://github.com/P-Schumacher/warmup.git"}
 gym = "0.13.0"
 free-mujoco-py = "*"
-myosuite = {path = "../myosuite", develop = true}
+myosuite = "^1.6.1"
 
 [tool.poetry.scripts]
 log = "deprl.log:main"
 plot = "deprl.plot:main"
 
 [tool.black]
 line-length = 79
```

### Comparing `deprl-0.1.3/PKG-INFO` & `deprl-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprl
-Version: 0.1.3
+Version: 0.1.4
 Summary: DEP-RL, a method for robust control of musculoskeletal systems.
 License: MIT
 Author: Pierre Schumacher
 Author-email: pierre.schumacher@tuebingen.mpg.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

