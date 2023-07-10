# Comparing `tmp/redco-0.4.5.tar.gz` & `tmp/redco-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redco-0.4.5.tar", last modified: Sat Jun 24 20:55:07 2023, max compression
+gzip compressed data, was "redco-0.4.6.tar", last modified: Mon Jul 10 12:38:55 2023, max compression
```

## Comparing `redco-0.4.5.tar` & `redco-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.5/LICENSE
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-24 20:55:07.360000 redco-0.4.5/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.5/README.md
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.5/redco/__init__.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/datasets/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.5/redco/datasets/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-06-20 03:18:51.000000 redco-0.4.5/redco/datasets/dataset.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-06-15 02:34:05.000000 redco-0.4.5/redco/datasets/jsonl_dataset.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/deployers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2064 2023-06-22 04:36:30.000000 redco-0.4.5/redco/deployers/data_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8110 2023-05-29 01:02:59.000000 redco-0.4.5/redco/deployers/deployer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2656 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/log_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/deployers/model_parallel_utils/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/model_parallel_utils/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5527 2023-06-22 04:36:30.000000 redco-0.4.5/redco/deployers/model_parallel_utils/mesh_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.5/redco/deployers/model_parallel_utils/partition_utils.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1835 2023-04-19 06:51:00.000000 redco-0.4.5/redco/deployers/opt_utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/predictors/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.5/redco/predictors/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4263 2023-06-20 20:03:17.000000 redco-0.4.5/redco/predictors/predictor.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.5/redco/predictors/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco/trainers/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.5/redco/trainers/__init__.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12128 2023-06-02 00:28:54.000000 redco-0.4.5/redco/trainers/trainer.py
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-04-19 06:51:00.000000 redco-0.4.5/redco/trainers/utils.py
-drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-06-24 20:55:07.360000 redco-0.4.5/redco.egg-info/
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-06-24 20:55:06.000000 redco-0.4.5/redco.egg-info/PKG-INFO
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-06-24 20:55:07.000000 redco-0.4.5/redco.egg-info/SOURCES.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-06-24 20:55:06.000000 redco-0.4.5/redco.egg-info/dependency_links.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-06-24 20:55:07.000000 redco-0.4.5/redco.egg-info/requires.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-06-24 20:55:07.000000 redco-0.4.5/redco.egg-info/top_level.txt
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-06-24 20:55:07.360000 redco-0.4.5/setup.cfg
--rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-06-24 20:54:53.000000 redco-0.4.5/setup.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    11358 2023-04-19 06:11:18.000000 redco-0.4.6/LICENSE
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-07-10 12:38:55.810000 redco-0.4.6/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3375 2023-05-13 23:56:05.000000 redco-0.4.6/README.md
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      693 2023-04-19 06:51:00.000000 redco-0.4.6/redco/__init__.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco/datasets/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      663 2023-04-19 06:51:00.000000 redco-0.4.6/redco/datasets/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      745 2023-06-20 03:18:51.000000 redco-0.4.6/redco/datasets/dataset.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1109 2023-06-15 02:34:05.000000 redco-0.4.6/redco/datasets/jsonl_dataset.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco/deployers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      625 2023-04-19 06:51:00.000000 redco-0.4.6/redco/deployers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2064 2023-06-22 04:36:30.000000 redco-0.4.6/redco/deployers/data_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     8501 2023-07-04 04:06:34.000000 redco-0.4.6/redco/deployers/deployer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2655 2023-07-04 00:08:18.000000 redco-0.4.6/redco/deployers/log_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco/deployers/model_parallel_utils/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      595 2023-04-19 06:51:00.000000 redco-0.4.6/redco/deployers/model_parallel_utils/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     5669 2023-07-04 02:05:17.000000 redco-0.4.6/redco/deployers/model_parallel_utils/mesh_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1854 2023-05-29 01:00:49.000000 redco-0.4.6/redco/deployers/model_parallel_utils/partition_utils.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1683 2023-07-04 04:06:34.000000 redco-0.4.6/redco/deployers/opt_utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco/predictors/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      628 2023-04-19 06:51:00.000000 redco-0.4.6/redco/predictors/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     4513 2023-07-04 01:28:07.000000 redco-0.4.6/redco/predictors/predictor.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1812 2023-04-19 06:51:00.000000 redco-0.4.6/redco/predictors/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco/trainers/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      624 2023-04-19 06:51:00.000000 redco-0.4.6/redco/trainers/__init__.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)    12182 2023-07-04 01:28:07.000000 redco-0.4.6/redco/trainers/trainer.py
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     2168 2023-07-03 04:04:51.000000 redco-0.4.6/redco/trainers/utils.py
+drwxr-xr-x   0 bowen     (1000) bowen     (1000)        0 2023-07-10 12:38:55.810000 redco-0.4.6/redco.egg-info/
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     3628 2023-07-10 12:38:55.000000 redco-0.4.6/redco.egg-info/PKG-INFO
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)      735 2023-07-10 12:38:55.000000 redco-0.4.6/redco.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        1 2023-07-10 12:38:55.000000 redco-0.4.6/redco.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       21 2023-07-10 12:38:55.000000 redco-0.4.6/redco.egg-info/requires.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)        6 2023-07-10 12:38:55.000000 redco-0.4.6/redco.egg-info/top_level.txt
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)       38 2023-07-10 12:38:55.810000 redco-0.4.6/setup.cfg
+-rwxr-xr-x   0 bowen     (1000) bowen     (1000)     1001 2023-07-10 12:38:25.000000 redco-0.4.6/setup.py
```

### Comparing `redco-0.4.5/LICENSE` & `redco-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/PKG-INFO` & `redco-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.5
+Version: 0.4.6
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.5/README.md` & `redco-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/__init__.py` & `redco-0.4.6/redco/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/datasets/__init__.py` & `redco-0.4.6/redco/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/datasets/dataset.py` & `redco-0.4.6/redco/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/datasets/jsonl_dataset.py` & `redco-0.4.6/redco/datasets/jsonl_dataset.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/deployers/__init__.py` & `redco-0.4.6/redco/deployers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/deployers/data_utils.py` & `redco-0.4.6/redco/deployers/data_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/deployers/deployer.py` & `redco-0.4.6/redco/deployers/deployer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 import jax.numpy as jnp
 from flax.jax_utils import replicate, unreplicate
 from flax.training.common_utils import shard_prng_key
 from flax.core.frozen_dict import unfreeze
 from flax.serialization import msgpack_serialize, msgpack_restore
 
 from .data_utils import get_host_examples, get_data_batches
-from .opt_utils import get_multistep_adamw_optimizer
+from .opt_utils import get_lr_schedule_fn
 from .log_utils import get_logger, log_info, save_outputs
 from .model_parallel_utils.mesh_utils import (
     get_mesh,
     shard_params_and_opt_state,
+    shard_params,
     gather_params_to_cpu,
     get_param_spec,
     get_sharding_rules)
 
 
 class Deployer:
     def __init__(self,
@@ -41,15 +42,15 @@
         if workdir is not None:
             os.makedirs(workdir, exist_ok=True)
 
         self._verbose = verbose
         self._workdir = workdir
         self._logger = get_logger(verbose=verbose, workdir=workdir)
 
-        if run_tensorboard:
+        if run_tensorboard and jax.process_index() == 0:
             from flax.metrics import tensorboard
             self._summary_writer = tensorboard.SummaryWriter(workdir)
         else:
             self._summary_writer = None
 
         self._rng = jax.random.PRNGKey(seed=jax_seed)
         self._mesh = get_mesh(n_model_shards=n_model_shards)
@@ -118,32 +119,38 @@
 
     def process_to_deliver(self, x):
         if self._mesh is None:
             return unreplicate(x)
         else:
             return x
 
-    def get_adamw_optimizer(self,
-                            train_size,
-                            per_device_batch_size,
-                            n_epochs,
-                            learning_rate,
-                            accumulate_grad_batches,
-                            warmup_rate,
-                            weight_decay):
+    def get_lr_schedule_fn(self,
+                           train_size,
+                           per_device_batch_size,
+                           n_epochs,
+                           learning_rate,
+                           schedule_type='linear',
+                           warmup_rate=0.,
+                           warmup_steps=None,
+                           init_learning_rate=0.,
+                           end_learning_rate=0.):
         _, global_batch_size = self.process_batch_size(
             per_device_batch_size=per_device_batch_size)
-        return get_multistep_adamw_optimizer(
-            train_size=train_size,
-            global_batch_size=global_batch_size,
-            n_epochs=n_epochs,
+        total_train_steps = n_epochs * (train_size // global_batch_size)
+
+        if warmup_steps is None:
+            warmup_steps = int(total_train_steps * warmup_rate)
+
+        return get_lr_schedule_fn(
+            schedule_type=schedule_type,
+            total_train_steps=total_train_steps,
+            warmup_steps=warmup_steps,
+            init_learning_rate=init_learning_rate,
             learning_rate=learning_rate,
-            accumulate_grad_batches=accumulate_grad_batches,
-            warmup_rate=warmup_rate,
-            weight_decay=weight_decay)
+            end_learning_rate=end_learning_rate)
 
     def get_sharding_rules(self, params):
         if self._mesh is None:
             return None
         else:
             sharding_rules = get_sharding_rules(
                 params=params, mesh_model_shards=self._mesh.shape['mp'])
@@ -154,14 +161,18 @@
 
             return sharding_rules
 
     def get_params_spec(self, params, params_sharding_rules):
         return get_param_spec(
             params=params, params_sharding_rules=params_sharding_rules)
 
+    def shard_params(self, params, params_spec):
+        return shard_params(
+            params=params, params_spec=params_spec, mesh=self._mesh)
+
     def shard_params_and_opt_state(self, params, params_spec, optimizer):
         return shard_params_and_opt_state(
             params=params,
             params_spec=params_spec,
             mesh=self._mesh,
             optimizer=optimizer)
 
@@ -182,15 +193,15 @@
                 info=info,
                 title=title,
                 logger=self._logger,
                 summary_writer=self._summary_writer,
                 step=step)
 
     def log_metrics(self, metrics, step):
-        if jax.process_index() == 0 and self._summary_writer is not None:
+        if self._summary_writer is not None:
             for metric_name, value in metrics.items():
                 self._summary_writer.scalar(metric_name, value, step=step)
 
     def save_outputs(self, outputs, desc, step):
         if self._workdir is not None and jax.process_index() == 0:
             save_outputs(
                 workdir=self._workdir,
```

### Comparing `redco-0.4.5/redco/deployers/log_utils.py` & `redco-0.4.6/redco/deployers/log_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         logger.info('=' * max_len)
         logger.info(f'### {title_}')
         logger.info('-' * max_len)
         for t in info.split('\n'):
             logger.info(t)
         logger.info('=' * max_len)
 
-
     else:
         logger.info(info)
 
 
 def save_outputs(outputs, workdir, desc, logger, summary_writer, step):
     outputs = jax.tree_util.tree_map(str, outputs)
     json.dump(outputs, open(f'{workdir}/outputs_{desc}.json', 'w'), indent=4)
```

### Comparing `redco-0.4.5/redco/deployers/model_parallel_utils/__init__.py` & `redco-0.4.6/redco/deployers/model_parallel_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/deployers/model_parallel_utils/mesh_utils.py` & `redco-0.4.6/redco/deployers/model_parallel_utils/mesh_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,22 @@
         self.dtype = dtype
 
 
 def get_param_spec(params, params_sharding_rules):
     return set_partitions(unfreeze(params), params_sharding_rules)
 
 
+def shard_params(params, params_spec, mesh):
+    shard_fn = pjit(
+        lambda x: x, in_shardings=(None,), out_shardings=params_spec)
+
+    with mesh:
+        return shard_fn(params)
+
+
 def shard_params_and_opt_state(params, params_spec, mesh, optimizer):
     def init_fn(params_):
         opt_state_ = optimizer.init(params_)
         return opt_state_, params_
 
     def get_opt_spec(x):
         if isinstance(x, (dict, FrozenDict,)):
@@ -65,29 +73,27 @@
 
     opt_state_spec, _ = jax.tree_util.tree_map(
         get_opt_spec, state_shapes,
         is_leaf=lambda x: isinstance(x, (dict, FrozenDict, optax.EmptyState,)))
 
     p_get_initial_state = pjit(
         init_fn,
-        in_axis_resources=(params_spec,),
-        out_axis_resources=(opt_state_spec, params_spec))
+        in_shardings=(params_spec,),
+        out_shardings=(opt_state_spec, params_spec))
 
     with mesh:
         opt_state, params = p_get_initial_state(params)
 
     return params, opt_state, opt_state_spec
 
 
 def gather_params_to_cpu(params, params_spec, mesh):
     def param_gather_fn(param_spec):
         return pjit(
-            lambda x: x,
-            in_axis_resources=(param_spec, ),
-            out_axis_resources=None)
+            lambda x: x, in_shardings=(param_spec, ), out_shardings=None)
 
     gather_fns = jax.tree_util.tree_map(
         lambda param_spec: param_gather_fn(param_spec),
         params_spec,
         is_leaf=lambda x: x is None or isinstance(x, P))
 
     with mesh:
```

### Comparing `redco-0.4.5/redco/deployers/model_parallel_utils/partition_utils.py` & `redco-0.4.6/redco/deployers/model_parallel_utils/partition_utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/predictors/__init__.py` & `redco-0.4.6/redco/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/predictors/predictor.py` & `redco-0.4.6/redco/predictors/predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,25 +24,24 @@
 
 class Predictor:
     def __init__(self,
                  deployer,
                  collate_fn,
                  pred_fn,
                  output_fn=None,
-                 params=None,
                  params_sharding_rules=None):
         self._deployer = deployer
         self._collate_fn = partial(collate_fn_wrapper, collate_fn=collate_fn)
 
-        self._params = params
         self._params_sharding_rules = params_sharding_rules
         self._pred_fn = partial(
             pred_fn_wrapper,
             pred_fn=pred_fn,
             under_pmap=self._deployer.mesh is None)
+        self._params_spec = None
         self._p_pred_step = None
 
         if output_fn is None:
             self._output_fn = default_output_fn
         else:
             self._output_fn = output_fn
 
@@ -55,25 +54,28 @@
             self._p_pred_step = jax.pmap(pred_fn, axis_name='batch')
         else:
             data_spec = {
                 key: P(*(('dp',) + (None,) * (len(value.shape) - 1)))
                 for key, value in dummy_batch.items()
             }
 
-            params_spec = self._deployer.get_params_spec(
+            self._params_spec = self._deployer.get_params_spec(
                 params=params, params_sharding_rules=params_sharding_rules)
 
             self._p_pred_step = pjit(
                 pred_fn,
-                in_axis_resources=(None, params_spec, data_spec),
+                in_axis_resources=(None, self._params_spec, data_spec),
                 out_axis_resources=None)
 
-    def predict(self, examples, per_device_batch_size, params=None, desc=''):
-        if params is None:
-            params = self._params
+    def predict(self,
+                examples,
+                per_device_batch_size,
+                params,
+                params_meshed=False,
+                desc=''):
         params = freeze(params)
 
         raw_n_inputs = len(examples)
         _, global_batch_size = self._deployer.process_batch_size(
             per_device_batch_size=per_device_batch_size)
         examples = examples + [examples[0]] * (global_batch_size - 1)
         examples = add_idxes(examples=examples)
@@ -93,14 +95,19 @@
             if self._p_pred_step is None:
                 self.setup_running_step(
                     pred_fn=self._pred_fn,
                     dummy_batch=batch,
                     params=params,
                     params_sharding_rules=self._params_sharding_rules)
 
+            if (self._params_spec is not None) and (not params_meshed):
+                params = self._deployer.shard_params(
+                    params=params, params_spec=self._params_spec)
+                params_meshed = True
+
             pred_rng = self._deployer.process_to_run_model(
                 self._deployer.gen_rng(), is_prng_key=True)
 
             batch_preds_with_idxes = self._deployer.run_model_step(
                 step_fn=self._p_pred_step,
                 input_args=(pred_rng, params, batch))
```

### Comparing `redco-0.4.5/redco/predictors/utils.py` & `redco-0.4.6/redco/predictors/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/trainers/__init__.py` & `redco-0.4.6/redco/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco/trainers/trainer.py` & `redco-0.4.6/redco/trainers/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from functools import partial
 import json
 import numpy as np
 import jax
 from jax.experimental.pjit import pjit
 from jax.sharding import PartitionSpec as P
 from flax.jax_utils import replicate
-from flax.training.train_state import TrainState
+from flax.training import train_state
 from flax.traverse_util import flatten_dict
 from flax.core.frozen_dict import freeze
 from .utils import default_train_step, default_eval_step
 from ..predictors import Predictor
 
 
 class Trainer:
@@ -49,48 +49,47 @@
         self._state_spec = None
         self._p_train_step = None
         self._p_eval_step = None
 
         self.create_train_state(
             apply_fn=apply_fn, params=params, optimizer=optimizer)
 
-        n_params = \
-            sum(np.prod(param.shape) for param in flatten_dict(params).values())
+        n_params = sum([param.size for param in flatten_dict(params).values()])
         self._deployer.log_info(f'{n_params:,}', title='Training parameters')
 
         self._default_predictor_fn = partial(
             Predictor,
             deployer=deployer,
             collate_fn=collate_fn,
             params_sharding_rules=params_sharding_rules)
 
     def create_train_state(self, apply_fn, params, optimizer):
         params = freeze(params)
 
         if self._deployer.mesh is None:
-            self._state = TrainState.create(
+            self._state = train_state.TrainState.create(
                 apply_fn=apply_fn, params=params, tx=optimizer)
             self._state = replicate(self._state)
         else:
             params_spec = self._deployer.get_params_spec(
                 params=params,
                 params_sharding_rules=self._params_sharding_rules)
 
             params, opt_state, opt_state_spec = \
                 self._deployer.shard_params_and_opt_state(
                     params=params, params_spec=params_spec, optimizer=optimizer)
 
-            self._state = TrainState(
+            self._state = train_state.TrainState(
                 apply_fn=apply_fn,
                 params=params,
                 tx=optimizer,
                 opt_state=opt_state,
                 step=0)
 
-            self._state_spec = TrainState(
+            self._state_spec = train_state.TrainState(
                 apply_fn=apply_fn,
                 params=params_spec,
                 tx=optimizer,
                 opt_state=opt_state_spec,
                 step=None)
 
     def setup_running_step(self, dummy_batch):
@@ -103,16 +102,14 @@
 
         eval_step_fn = partial(
             default_eval_step,
             loss_fn=self._loss_fn,
             under_pmap=(self._deployer.mesh is None))
 
         if self._deployer.mesh is None:
-            del dummy_batch
-
             self._p_train_step = jax.pmap(train_step_fn, axis_name='batch')
             self._p_eval_step = jax.pmap(eval_step_fn, axis_name='batch')
         else:
             data_spec = {
                 key: P(*(('dp',) + (None,) * (len(value.shape) - 1)))
                 for key, value in dummy_batch.items()
             }
@@ -167,15 +164,15 @@
 
             metrics = self._deployer.run_model_step(
                 step_fn=self._p_eval_step, input_args=(self._state, batch))
 
             metrics = self._deployer.process_to_deliver(metrics)
             data_batches.set_postfix(**metrics)
 
-            losses.append(metrics['loss'])
+            losses.append(metrics['loss'].item())
 
         return np.mean(losses).item()
 
     def fit(self,
             train_examples,
             per_device_batch_size,
             n_epochs,
@@ -221,14 +218,15 @@
                         desc=f'epoch {epoch_idx} / {n_epochs}')
                     eval_metrics['loss'] = loss
 
                 if eval_predictor is not None:
                     preds = eval_predictor.predict(
                         examples=eval_examples,
                         params=self.params,
+                        params_meshed=(self._deployer.mesh is not None),
                         per_device_batch_size=eval_per_device_batch_size,
                         desc=f'epoch {epoch_idx} / {n_epochs}')
 
                     if eval_metric_fn is not None:
                         eval_metrics.update(eval_metric_fn(
                             examples=eval_examples, preds=preds))
```

### Comparing `redco-0.4.5/redco/trainers/utils.py` & `redco-0.4.6/redco/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/redco.egg-info/PKG-INFO` & `redco-0.4.6/redco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redco
-Version: 0.4.5
+Version: 0.4.6
 Summary: UNKNOWN
 Home-page: https://github.com/tanyuqian/redco
 Author: Bowen Tan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `redco-0.4.5/redco.egg-info/SOURCES.txt` & `redco-0.4.6/redco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redco-0.4.5/setup.py` & `redco-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="redco",
-    version="0.4.5",
+    version="0.4.6",
     author="Bowen Tan",
     packages=find_packages(),
     install_requires=['jax', 'flax', 'optax', 'numpy'],
     include_package_data=True,
     python_requires=">=3.8",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

