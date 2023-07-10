# Comparing `tmp/modelwhaleutils-0.5.1.6.tar.gz` & `tmp/modelwhaleutils-0.5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modelwhaleutils-0.5.1.6.tar", last modified: Fri May 12 06:10:37 2023, max compression
+gzip compressed data, was "dist/modelwhaleutils-0.5.2.0.tar", last modified: Mon Jul 10 04:04:37 2023, max compression
```

## Comparing `modelwhaleutils-0.5.1.6.tar` & `modelwhaleutils-0.5.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/
--rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/PKG-INFO
--rw-r--r--   0 YiranTao   (502) staff       (20)     3078 2021-04-16 07:51:27.000000 modelwhaleutils-0.5.1.6/README.md
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/
--rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/PKG-INFO
--rw-r--r--   0 YiranTao   (502) staff       (20)      360 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/SOURCES.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)        1 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/dependency_links.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)       35 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/requires.txt
--rw-r--r--   0 YiranTao   (502) staff       (20)        8 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/modelwhaleutils.egg-info/top_level.txt
-drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/mwutils/
--rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/__init__.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     1580 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/keras.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     4410 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/logs.py
--rw-r--r--   0 YiranTao   (502) staff       (20)    22758 2023-05-12 06:09:49.000000 modelwhaleutils-0.5.1.6/mwutils/run.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     6284 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/sys_stat.py
--rw-r--r--   0 YiranTao   (502) staff       (20)     1163 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/tf_utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)      562 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/torch_utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.1.6/mwutils/utils.py
--rw-r--r--   0 YiranTao   (502) staff       (20)       38 2023-05-12 06:10:37.000000 modelwhaleutils-0.5.1.6/setup.cfg
--rw-r--r--   0 YiranTao   (502) staff       (20)      512 2023-05-12 06:09:57.000000 modelwhaleutils-0.5.1.6/setup.py
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/
+-rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/PKG-INFO
+-rw-r--r--   0 YiranTao   (502) staff       (20)     3078 2021-04-16 07:51:27.000000 modelwhaleutils-0.5.2.0/README.md
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/
+-rw-r--r--   0 YiranTao   (502) staff       (20)      381 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/PKG-INFO
+-rw-r--r--   0 YiranTao   (502) staff       (20)      360 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/SOURCES.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)        1 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/dependency_links.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)       42 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/requires.txt
+-rw-r--r--   0 YiranTao   (502) staff       (20)        8 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/modelwhaleutils.egg-info/top_level.txt
+drwxr-xr-x   0 YiranTao   (502) staff       (20)        0 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/mwutils/
+-rw-r--r--   0 YiranTao   (502) staff       (20)        0 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/__init__.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     1580 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/keras.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     4062 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/logs.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)    21826 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/run.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     6285 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/sys_stat.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     1163 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/tf_utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)      562 2021-11-12 07:12:08.000000 modelwhaleutils-0.5.2.0/mwutils/torch_utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)     5203 2023-07-10 03:51:57.000000 modelwhaleutils-0.5.2.0/mwutils/utils.py
+-rw-r--r--   0 YiranTao   (502) staff       (20)       38 2023-07-10 04:04:37.000000 modelwhaleutils-0.5.2.0/setup.cfg
+-rw-r--r--   0 YiranTao   (502) staff       (20)      544 2023-07-10 04:04:34.000000 modelwhaleutils-0.5.2.0/setup.py
```

### Comparing `modelwhaleutils-0.5.1.6/README.md` & `modelwhaleutils-0.5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.6/mwutils/keras.py` & `modelwhaleutils-0.5.2.0/mwutils/keras.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.6/mwutils/logs.py` & `modelwhaleutils-0.5.2.0/mwutils/logs.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             f.write(json.dumps(entry))
 
 
 def append_logs_buf_to_remote(logs_buf, name, metadata, post_addr):
     json_struct = {"logs": logs_buf, "phase": name, "metadata": metadata}
     # try 3 times
     for _ in range(3):
+        print('append log', name)
         r = requests.post(post_addr, json=json_struct, headers={"Authorization": jwt.encode(
             {"whatever": "1"}, "857851b2-c28c-4d94-83c8-f607b50ccd03")})
         if r.status_code >= 400:
             # something wrong
             jb = ''
             try:
                 jb = r.json()
@@ -47,14 +48,15 @@
     def __init__(self, interval, function, *args, **kwargs):
         self._timer = None
         self.interval = interval
         self.function = function
         self.args = args
         self.kwargs = kwargs
         self.is_running = False
+        print('timer registerd')
         self.start()
 
     def _run(self):
         self.is_running = False
         self.start()
         self.function(*self.args, **self.kwargs)
 
@@ -69,15 +71,16 @@
         self.is_running = False
 
 
 class Logger():
     # Logger for metrics
     def __init__(self, name, sample_time_interval_seconds=10, metadata={}, local_path="", post_addr="", buffer_all=False):
         self._logs_buf = []
-        self._sample_time_interval_seconds = max(sample_time_interval_seconds, 2)
+        self._sample_time_interval_seconds = max(
+            sample_time_interval_seconds, 2)
         self.name = name
         self.metadata = metadata
         self.mutex = threading.Lock()
         self._thread = RepeatedTimer(
             self._sample_time_interval_seconds, self.flush)
         self.post_addr = post_addr
         self.remote = True if post_addr else False
@@ -132,23 +135,7 @@
             self.memoize_funcs.append(f)
 
     def show_buffer(self):
         print(self._logs_buf)
 
     def show_user_buffer(self):
         print(self._user_buf)
-
-
-if __name__ == "__main__":
-    lg = Logger("fake", sample_time_interval_seconds=1,
-                metadata={}, local_path="./what.json")
-    lg.start()
-    lg.log({"v1": 1, "v2": 2})
-    for i in range(30):
-        time.sleep(0.3)
-        lg.log({"v1": i, "v2": 100+2*i})
-        if i % 10 == 0:
-            lg.log([{"fucker": 1*i}, {"fucker2": 2*i+100}])
-        if i % 5 == 0:
-            lg.show_buffer()
-
-    lg.cancel()
```

### Comparing `modelwhaleutils-0.5.1.6/mwutils/run.py` & `modelwhaleutils-0.5.2.0/mwutils/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import jwt
 import warnings
 import requests
 import os
 from mwutils.sys_stat import SystemStats
 from mwutils.logs import Logger, mili_time
 import mwutils
+import mlflow
+from .utils import *
 
 
 _STEP = 'step'
 _EPOCH = 'epoch'
 _BATCH = 'batch'
 _LOSS = 'loss'
 _ACC = 'acc'
@@ -33,127 +35,32 @@
 MODEL_TYPE_KERAS = "keras"
 MODEL_TYPE_TORCH = "torch"
 MODEL_TYPE_CUSTOM = "custom"
 
 run_names = {}
 
 
-class MLLoger(Logger):
-    def log(self, step=None, epoch=None, batch=None, loss=None, acc=None, custom_logs=None):
-        val = dict()
-        val[_TIMESTAMP] = int(time.time())
-        if step is not None:
-            val[_STEP] = step + 1
-        if epoch is not None:
-            val[_EPOCH] = epoch + 1
-        if batch is not None:
-            val[_BATCH] = batch + 1
-        if loss is not None:
-            val[_LOSS] = loss
-        if acc is not None:
-            val[_ACC] = acc
-
-        if acc:
-            if _MAX_ACC not in self.memoize and acc:
-                self.memoize[_MAX_ACC] = val
-            elif self.memoize[_MAX_ACC][_ACC] < val[_ACC]:
-                self.memoize[_MAX_ACC] = val
-
-        if loss:
-            best = False
-            if _MIN_LOSS not in self.memoize and loss:
-                self.memoize[_MIN_LOSS] = val
-                best = True
-            elif self.memoize[_MIN_LOSS][_LOSS] > val[_LOSS]:
-                self.memoize[_MIN_LOSS] = val
-                best = True
-            if best:
-                if step is not None:
-                    self.memoize["{}_{}".format(_BEST, _STEP)] = step+1
-                elif epoch is not None:
-                    self.memoize["{}_{}".format(_BEST, _EPOCH)] = epoch+1
-                elif batch is not None:
-                    self.memoize["{}_{}".format(_BEST, _BATCH)] = batch+1
-        if custom_logs:
-            if isinstance(custom_logs, dict):
-                for k, v in custom_logs.items():
-                    if k not in ['loss', 'acc', 'accuracy', 'val_loss', 'val_acc', 'val_accuracy']:
-                        if 'custom_keys' not in self.metadata['annotations']:
-                            self.metadata['annotations']['custom_keys'] = []
-                        if k not in self.metadata['annotations']['custom_keys']:
-                            self.metadata['annotations']['custom_keys'].append(
-                                k)
-                        val[k] = v
-        for k, _ in val.items():
-            if k not in self.metadata['annotations']['keys']:
-                self.metadata['annotations']['keys'].append(k)
-        super().log(val)
-
-
-def example_memoize_func(memoize_buf, val):
-    if "cost" in val:
-        if "min_cost" in memoize_buf and memoize_buf["min_cost"] > val["cost"]:
-            memoize_buf["min_cost"] = val["cost"]
-
-
-class CustomLogger(Logger):
-    pass
-
-
-def save_tf_ckpt(sess, directory, filename):
-    import tensorflow as tf
-    from tensorflow.python.framework import graph_util
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-    filepath = os.path.join(directory, filename + '.ckpt')
-    saver = tf.train.Saver()
-    saver.save(sess, filepath)
-    return filepath
-
-
-def save_as_pb(sess, directory, filename, output_node):
-    import tensorflow as tf
-    from tensorflow.python.tools import freeze_graph
-    if not os.path.exists(directory):
-        os.makedirs(directory)
-
-    # Save check point for graph frozen later
-    ckpt_filepath = save_tf_ckpt(sess, directory=directory, filename=filename)
-    pbtxt_filename = filename + '.pbtxt'
-    pbtxt_filepath = os.path.join(directory, pbtxt_filename)
-    pb_filepath = os.path.join(directory, filename + '.pb')
-    # This will only save the graph but the variables will not be saved.
-    # You have to freeze your model first.
-    tf.train.write_graph(
-        graph_or_graph_def=sess.graph_def,
-        logdir=directory,
-        name=pbtxt_filename,
-        as_text=True)
-
-    freeze_graph.freeze_graph(
-        input_graph=pbtxt_filepath,
-        input_saver='',
-        input_binary=False,
-        input_checkpoint=ckpt_filepath,
-        output_node_names=output_node,
-        restore_op_name='save/restore_all',
-        filename_tensor_name='save/Const:0',
-        output_graph=pb_filepath,
-        clear_devices=True,
-        initializer_nodes='')
-
-    return pb_filepath
-
-
 class Run():
-    def __init__(self, name="", user_id="", lab_id="", org_id="", user_token="", flush_interval_seconds=5,
+    def __init__(self, name="", user_id="", lab_id="", org_id="", user_token="", use_mlflow=False, is_debug=False, debug_uid="", flush_interval_seconds=5,
                  sys_stat_sample_size=1, sys_stat_sample_interval=2, local_path='', write_logs_to_local=False,
                  remote_path='', buffer_all_logs=False):
+        if use_mlflow == True:
+            active_run = mlflow.active_run()
+            if active_run is None:
+                raise MlFlowRunNotFould("没有找到已创建的 mlflow run")
+            else:
+                self.use_mlflow = True
+                self.mlflow_run = active_run
+        else:
+            self.use_mlflow = False
         if name == '':
-            name == '数据科学实验@' + str(randrange(999))
+            if self.use_mlflow == True and self.mlflow_run is not None:
+                name = self.mlflow_run.info.run_name
+            else:
+                name = '数据科学实验@' + str(randrange(999))
         if name in run_names:
             s = "name {} is already used in current session.".format(name)
             raise Exception(s)
         p = os.path.expanduser('~')
         _path = p + '/.ide/config.json'
         _data = None
         config_user_id = None
@@ -211,39 +118,104 @@
         if remote_path:
             self.remote_path = remote_path
         elif _remote_path:
             self.remote_path = _remote_path + '/api/runs'
         else:
             self.remote_path = 'https://www.heywhale.com/api/runs'
 
-        print('remotepath is', self.remote_path)
+        print('api 地址: ', self.remote_path)
         timestr = str(mili_time())
         if not (self.user_id and self.lab_id and self.org_id):
             s = "At least one of required fields is empty:\nuser_id: {}\norg_id: {}\nlab_id: {}\n".format(
                 user_id, org_id, lab_id)
             raise Exception(s)
         self.run_id = name + '_' + timestr
         self.flush_interval_seconds = max(5, flush_interval_seconds)
         self._sys_stat_sample_size = sys_stat_sample_size
         self._sys_stat_sample_interval_seconds = sys_stat_sample_interval
         self.local_path = local_path
         self.write_logs_to_local = write_logs_to_local
-        self.logs_remote_path = remote_path + '/logs' if remote_path else ''
-        self.conclude_remote_path = remote_path + '/conclude'
-        self.abort_remote_path = remote_path + "/abort"
+        self.logs_remote_path = self.remote_path + '/logs'
+        self.conclude_remote_path = self.remote_path + '/conclude'
+        self.abort_remote_path = self.remote_path + "/abort"
         self.buffer_all_logs = buffer_all_logs
         self.model_path = ""
-        self.metadata = {"name": name, "user_id": user_id,
-                         "lab_id": lab_id, "run_id": self.run_id, "org_id": org_id, "annotations": {"custom_keys": [], "keys": []}}
+        self.metadata = {"name": name, "user_id": self.user_id,
+                         "lab_id": self.lab_id, "run_id": self.run_id, "org_id": self.org_id, "annotations": {"custom_keys": [], "keys": []}}
         self.pid = None
         self.started = False
 
+        # INIT ML
+        self.pid = getpid()
+        train_path = path.join(
+            self.local_path, "train.json") if self.write_logs_to_local else ''
+        test_path = path.join(
+            self.local_path, "test.json") if self.write_logs_to_local else ''
+        val_path = path.join(
+            self.local_path, "val.json") if self.write_logs_to_local else ''
+        sys_path = path.join(
+            self.local_path, "sys.json") if self.write_logs_to_local else ''
+        self._loggers['train'] = MLLoger("train", sample_time_interval_seconds=self.flush_interval_seconds,
+                                         metadata=self.metadata, local_path=train_path, post_addr=self.logs_remote_path,
+                                         buffer_all=self.buffer_all_logs)
+        self._loggers['test'] = MLLoger("test", sample_time_interval_seconds=self.flush_interval_seconds,
+                                        metadata=self.metadata, local_path=test_path, post_addr=self.logs_remote_path,
+                                        buffer_all=self.buffer_all_logs)
+        self._loggers['val'] = MLLoger("val", sample_time_interval_seconds=self.flush_interval_seconds,
+                                       metadata=self.metadata, local_path=val_path, post_addr=self.logs_remote_path,
+                                       buffer_all=self.buffer_all_logs)
+        self._loggers['system'] = CustomLogger("system", sample_time_interval_seconds=self.flush_interval_seconds,
+                                               metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
+                                               buffer_all=self.buffer_all_logs)
+        self._loggers['meta'] = CustomLogger("meta", sample_time_interval_seconds=self.flush_interval_seconds,
+                                             metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
+                                             buffer_all=self.buffer_all_logs)
+        print('logger class registered')
+        # START ML
+        self.started = True
+        self.__register_signal_handlers()
+        for _, logger in self._loggers.items():
+            logger.start()
+        for _, clogger in self.custom_loggers.items():
+            clogger.start()
+        self.sys_stat = SystemStats(self)
+        self.sys_stat.start()
+
+        print('logger started')
+        # 创建一个 RUN
+        _request_meta = {
+            'metadata': {
+                'name': name,
+                'user_id': self.user_id,
+                'run_id': self.run_id,
+                'lab_id': self.lab_id,
+                'org_id': self.org_id
+            }
+        }
+        if is_debug == True:
+            _addr = self.remote_path + '/linkMLFlow'
+            _request_meta['use_mlflow'] = True
+            _request_meta['is_debug'] = True
+            _request_meta['mlflow_run'] = {'info': {'run_uuid': debug_uid}}
+            create_run(_request_meta, _addr)
+        else:
+            if self.use_mlflow:
+                _request_meta['is_debug'] = False
+                _addr = self.remote_path + '/linkMLFlow'
+                _request_meta['use_mlflow'] = True
+                _request_meta['mlflow_run'] = self.mlflow_run
+                create_run(_request_meta, _addr)
+            else:
+                _request_meta['use_mlflow'] = False
+                _request_meta['is_debug'] = False
+                create_run(_request_meta, self.logs_remote_path)
+
     def init_ml(self):
-        if self.pid:
-            return
+        # if self.pid:
+        #     return
         self.pid = getpid()
         train_path = path.join(
             self.local_path, "train.json") if self.write_logs_to_local else ''
         test_path = path.join(
             self.local_path, "test.json") if self.write_logs_to_local else ''
         val_path = path.join(
             self.local_path, "val.json") if self.write_logs_to_local else ''
@@ -450,15 +422,16 @@
                             else:
                                 print(
                                     'Torch Model detected, saving to ' + _save_path)
                                 import torch
                                 torch.save(target.state_dict(), _save_path)
                                 pass
                         except:
-                            print('model cannot be saved, please check format')
+                            print('模型文件无法保存，请检查格式。')
+                            pass
 
                 path_artifact = '/api/dataset-upload-token?subType=artifact'
                 endpoint_get_token = self.remote_path.replace(
                     '/api/runs', path_artifact) + '&token=' + self.user_token
                 r = requests.get(endpoint_get_token)
                 oss_config = json.loads(r.text)
                 AK = oss_config['accessKeyId']
@@ -493,14 +466,15 @@
                             print('uploading file: ', fullpath)
                             response = s3_client.upload_file(
                                 fullpath, bucket, object_name)
                             prefixes.append(object_name)
                         except ClientError as e:
                             logging.error(e)
                             print('Error uploading file ', file)
+                            pass
         if self.remote_path:
             tp = int(time.time())
             json_struct = {
                 "metadata": self.metadata,
                 "best": [{"phase": name, "val": logger.memoize, _TIMESTAMP: tp} for name, logger in self._loggers.items()],
             }
             if len(prefixes) > 0:
@@ -521,43 +495,12 @@
                     print(msg)
                     warnings.warn(msg)
                 else:
                     print("conclude remote call succeed. resp:", r)
                     break
         # if upload_model:
         #     self.__upload_model()
+        if self.use_mlflow:
+            mlflow.end_run()
         self.started = False
         self.run_id = "concluded"
-
-
-if __name__ == "__main__":
-    import time
-
-    def sys_memoize_func_maxcpu(memoize_buf, val):
-        if "cpu" in val:
-            if "max_cpu" in memoize_buf and memoize_buf["max_cpu"] < val["cpu"]:
-                memoize_buf["max_cpu"] = val["cpu"]
-            if "max_cpu" not in memoize_buf:
-                memoize_buf["max_cpu"] = val["cpu"]
-
-    def sys_memoize_func_mincpu(memoize_buf, val):
-        if "cpu" in val:
-            if "min_cpu" in memoize_buf and memoize_buf["min_cpu"] > val["cpu"]:
-                memoize_buf["min_cpu"] = val["cpu"]
-            if "min_cpu" not in memoize_buf:
-                memoize_buf["min_cpu"] = val["cpu"]
-
-    r = Run("test88", "testuser123", "proj123", "job123", flush_interval_seconds=5,
-            local_path="/Users/mk/heyw/github/mwutils/mwutils", sys_stat_sample_interval=5, sys_stat_sample_size=21, buffer_all_logs=True)
-    r.init_ml()
-    r.add_memoize_funcs_to_logger(
-        "system", [sys_memoize_func_maxcpu, sys_memoize_func_mincpu])
-
-    r.start_ml()
-
-    for i in range(150):
-        r.log_ml(step=i, acc=i*(1/150), loss=149-i)
-        time.sleep(0.2)
-    for i in range(20):
-        r.log_ml(epoch=i, acc=i*(1/40)+0.5, loss=1, phase='test')
-        time.sleep(0.2)
-    r.conclude()
+        print('记录已结束')
```

### Comparing `modelwhaleutils-0.5.1.6/mwutils/sys_stat.py` & `modelwhaleutils-0.5.2.0/mwutils/sys_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,12 +164,12 @@
 
                 except pynvml.NVMLError as err:
                     pass
 
             except pynvml.NVMLError as err:
                 pass
         if psutil:
-            #net = psutil.net_io_counters()
+            # net = psutil.net_io_counters()
             sysmem = psutil.virtual_memory()
             stats["cpu"] = psutil.cpu_percent()
             stats["memory"] = sysmem.percent
         return stats
```

### Comparing `modelwhaleutils-0.5.1.6/mwutils/tf_utils.py` & `modelwhaleutils-0.5.2.0/mwutils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.6/mwutils/torch_utils.py` & `modelwhaleutils-0.5.2.0/mwutils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.1.6/setup.py` & `modelwhaleutils-0.5.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import setuptools
 
 setuptools.setup(
     name="modelwhaleutils",
-    version="0.5.1.6",
+    version="0.5.2.0",
     author="modalwhale team",
     description="use in mw",
     url="https://github.com/Kesci/modelwhaleutils",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["PyJWT", "requests", "pynvml", "psutil", "boto3"],
+    install_requires=["PyJWT", "requests",
+                      "pynvml", "psutil", "boto3", "mlflow"],
     python_requires='>=3.6',
 )
```

