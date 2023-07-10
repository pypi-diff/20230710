# Comparing `tmp/numpy_io-0.0.6-py3-none-any.whl.zip` & `tmp/numpy_io-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 27383 bytes, number of entries: 30
+Zip file size: 27451 bytes, number of entries: 30
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Apr-27 06:30 numpy_io/__init__.py
--rw-rw-rw-  2.0 fat      628 b- defN 23-Jul-06 09:11 numpy_io/setup.py
+-rw-rw-rw-  2.0 fat      629 b- defN 23-Jul-10 07:47 numpy_io/setup.py
 -rw-rw-rw-  2.0 fat       80 b- defN 23-Apr-27 06:30 numpy_io/core/__init__.py
--rw-rw-rw-  2.0 fat    19443 b- defN 23-Jul-04 03:27 numpy_io/core/numpyadapter.py
--rw-rw-rw-  2.0 fat     5457 b- defN 23-Apr-27 06:30 numpy_io/core/parallel.py
+-rw-rw-rw-  2.0 fat    19587 b- defN 23-Jul-10 07:41 numpy_io/core/numpyadapter.py
+-rw-rw-rw-  2.0 fat     5619 b- defN 23-Jul-10 07:52 numpy_io/core/parallel.py
 -rw-rw-rw-  2.0 fat     1894 b- defN 23-Apr-27 06:30 numpy_io/core/reader.py
--rw-rw-rw-  2.0 fat     2244 b- defN 23-Jul-04 02:33 numpy_io/core/writer.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Jul-10 07:54 numpy_io/core/writer.py
 -rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-27 06:30 numpy_io/examples/__init__.py
 -rw-rw-rw-  2.0 fat     3236 b- defN 23-Jul-03 23:35 numpy_io/examples/auto_parallel_writer.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 23-Apr-27 06:30 numpy_io/examples/auto_writer.py
 -rw-rw-rw-  2.0 fat     1778 b- defN 23-Apr-27 07:23 numpy_io/examples/leveldb_readwriter_example.py
 -rw-rw-rw-  2.0 fat     2218 b- defN 23-Apr-28 00:25 numpy_io/examples/lmdb_readwriter_example.py
 -rw-rw-rw-  2.0 fat     1198 b- defN 23-Apr-27 06:30 numpy_io/examples/memory_raw_readwriter_example.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-27 06:30 numpy_io/examples/memory_readwriter_example.py
@@ -21,12 +21,12 @@
 -rw-rw-rw-  2.0 fat     2658 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/lmdb_test.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Apr-27 06:30 numpy_io/examples/testing/test_mem.py
 -rw-rw-rw-  2.0 fat     2907 b- defN 23-Apr-27 07:08 numpy_io/examples/testing/test_mutiprocess.py
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Apr-28 00:25 numpy_io/pytorch_loader/__init__.py
 -rw-rw-rw-  2.0 fat    10309 b- defN 23-Jul-04 03:24 numpy_io/pytorch_loader/data_helper.py
 -rw-rw-rw-  2.0 fat     8940 b- defN 23-Jul-04 01:02 numpy_io/pytorch_loader/dataloaders.py
 -rw-rw-rw-  2.0 fat     3780 b- defN 23-May-25 05:42 numpy_io/pytorch_loader/tokenizer_config_helper.py
--rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2715 b- defN 23-Jul-06 09:12 numpy_io-0.0.6.dist-info/RECORD
-30 files, 82767 bytes uncompressed, 22931 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat      390 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2715 b- defN 23-Jul-10 07:55 numpy_io-0.0.7.dist-info/RECORD
+30 files, 83099 bytes uncompressed, 22999 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: numpy_io/pytorch_loader/dataloaders.py
 Comment: 
 
 Filename: numpy_io/pytorch_loader/tokenizer_config_helper.py
 Comment: 
 
-Filename: numpy_io-0.0.6.dist-info/METADATA
+Filename: numpy_io-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: numpy_io-0.0.6.dist-info/WHEEL
+Filename: numpy_io-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: numpy_io-0.0.6.dist-info/top_level.txt
+Filename: numpy_io-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: numpy_io-0.0.6.dist-info/RECORD
+Filename: numpy_io-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## numpy_io/setup.py

```diff
@@ -3,22 +3,22 @@
 
 from setuptools import setup, find_packages
 
 ignore = []
 
 setup(
     name='numpy-io',
-    version='0.0.6',
+    version='0.0.7',
     description='an easy training architecture',
     long_description='numpy-io: https://github.com/ssbuild/numpy-io.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/numpy-io',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=[
-        'fastdatasets>=0.9.14 , < 0.9.15',
+        'fastdatasets>=0.9.14 , <= 0.9.20',
         'numpy',
         'tqdm',
         'six'
     ],
     packages=[p for p in find_packages() if p not in ignore]
 )
```

## numpy_io/core/numpyadapter.py

```diff
@@ -12,22 +12,22 @@
 from fastdatasets.utils.py_features import Final
 from fastdatasets.record import writer as record_writer, RECORD, load_dataset as record_loader
 from fastdatasets.leveldb import writer as leveldb_writer, LEVELDB, load_dataset as leveldb_loader
 from fastdatasets.lmdb import writer as lmdb_writer, LMDB, load_dataset as lmdb_loader
 from fastdatasets.memory import writer as memory_writer, MEMORY, load_dataset as memory_loader
 from fastdatasets.arrow import writer as arrow_writer,load_dataset as arrow_loader
 from fastdatasets.parquet import writer as parquet_writer,load_dataset as parquet_loader
-from .parallel import ParallelStruct, parallel_apply
+from .parallel import ParallelNode, parallel_apply
 
 
 __all__ = [
     'E_file_backend',
     'NumpyWriterAdapter',
     'NumpyReaderAdapter',
-    'ParallelStruct',
+    'ParallelNode',
     'parallel_apply',
     'ParallelNumpyWriter'
 ]
 
 
 class E_file_backend(Enum):
     record = 0
@@ -330,17 +330,17 @@
             dataset = None
             warnings.warn('no support databackend')
         if with_parse_from_numpy and parse_flag:
             dataset = dataset.parse_from_numpy_writer()
         return dataset
 
 
-class ParallelNumpyWriter(ParallelStruct, metaclass=Final):
+class ParallelNumpyWriter(ParallelNode, metaclass=Final):
     def __init__(self, *args, **kwargs):
-        ParallelStruct.__init__(self, *args, **kwargs)
+        ParallelNode.__init__(self, *args, **kwargs)
         self.batch_keys = []
         self.batch_values = []
         self.total_num = 0
         self.numpy_writer = None
 
     def open(self, outfile: typing.Union[str, typing.List],
              backend: typing.Union[E_file_backend, str],
@@ -371,26 +371,31 @@
         self.backend = self.numpy_writer.backend
         self.backend_type = self.numpy_writer.backend_type
         self.is_kv_writer = self.numpy_writer.is_kv_writer
         self.is_table = self.numpy_writer.is_table
         self.schema = self.numpy_writer.schema
         self.write_batch_size = self.numpy_writer.buffer_batch_size
 
-    def write(self, data, input_hook_fn: typing.Callable, fn_args: typing.Union[typing.Tuple, typing.Dict],
+    def write(self,
+              data: typing.Union[typing.Sequence,typing.Iterator],
+              input_hook_fn: typing.Callable,
+              fn_args: typing.Union[typing.Tuple, typing.Dict],
               write_batch_size=None):
         self.input_hook_fn = input_hook_fn
         self.fn_args = fn_args
 
         assert self.numpy_writer is not None
         assert self.input_hook_fn is not None
 
         if write_batch_size is None or write_batch_size <= 0:
             write_batch_size = self.numpy_writer.buffer_batch_size
-            if write_batch_size >= len(data):
-                write_batch_size = len(data) // 2
+
+            if isinstance(data,typing.Sequence):
+                if write_batch_size >= len(data):
+                    write_batch_size = len(data) // 2
 
         if write_batch_size <= 0:
             write_batch_size = 1
 
         self.write_batch_size = write_batch_size
         parallel_apply(data, self)
```

## numpy_io/core/parallel.py

```diff
@@ -1,19 +1,19 @@
 # @Time    : 2022/11/5 19:34
 import random
 import typing
 from multiprocessing import Queue,Manager,Process
 
 __all__ = [
     'parallel_apply',
-    'ParallelStruct'
+    'ParallelNode'
 ]
 
 
-class ParallelStruct:
+class ParallelNode:
     def __init__(self,
                  num_process_worker: int = 4,
                  num_process_post_worker: int = 1,
                  input_queue_size: int = 200,
                  output_queue_size : int = 100,
                  shuffle = True,
                  desc: str='parallel'):
@@ -82,107 +82,115 @@
     def on_initalize(self,data):...
     '''
         main process callback
     '''
     def on_finalize(self):...
 
 
-def parallel_apply(data: typing.List, parallel_node: ParallelStruct):
+
+def produce_input(q_in: Queue,
+                  q_out: Queue,
+                  startup_fn: typing.Callable,
+                  process_fn: typing.Callable,
+                  cleanup_fn: typing.Callable,
+                  ):
+    startup_fn()
+    while True:
+        index,x = q_in.get()
+        if index is None:
+            q_out.put((None, None))
+            break
+        res = process_fn(x)
+        q_out.put((index,res))
+    cleanup_fn()
+
+def consume_output(q_out: Queue,
+                   total_producer: int,
+                   startup_fn: typing.Callable,
+                   process_fn: typing.Callable,
+                   cleanup_fn: typing.Callable):
+
+    startup_fn()
+    while total_producer > 0:
+        index,x = q_out.get()
+        if index is None:
+            total_producer -= 1
+        process_fn(x)
+    cleanup_fn()
+
+def parallel_apply(data: typing.Union[typing.Sequence,typing.Iterator],
+                   parallel_node: ParallelNode):
     Queue_CLASS = Manager().Queue if parallel_node.num_process_worker > 0 and parallel_node.num_process_worker > 0 else Queue
     q_in =Queue_CLASS(parallel_node.input_queue_size) if parallel_node.input_queue_size > 0 else Queue_CLASS()
     q_out = Queue_CLASS(parallel_node.output_queue_size) if parallel_node.output_queue_size > 0 else Queue_CLASS()
 
 
-    def produce_input(q_in: Queue, q_out: Queue,
-                      startup_fn: typing.Callable,
-                      process_fn: typing.Callable,
-                      cleanup_fn: typing.Callable,
-                      ):
-        startup_fn()
-        while True:
-            index,x = q_in.get()
-            if index is None:
-                break
-            res = process_fn(x)
-            q_out.put((index,res))
-        cleanup_fn()
-
-    def consume_output(q_out: Queue,
-                       total: int,
-                           startup_fn: typing.Callable,
-                           process_fn: typing.Callable,
-                           cleanup_fn: typing.Callable,
-                           ):
-
-        startup_fn()
-        __n__ = 0
-
-        flag = total > 0
-        while flag:
-            index,x = q_out.get()
-            process_fn(x)
-            __n__ += 1
-            if __n__ == total:
-                break
-        cleanup_fn()
-
 
 
     parallel_node.on_initalize(data)
+    if isinstance(data,typing.Sequence):
+        total = len(data)
+        ids = list(range(total))
+        if parallel_node.shuffle:
+            random.shuffle(ids)
+        try:
+            from tqdm import tqdm
+            ids = tqdm(ids, total=total, desc=parallel_node.desc if parallel_node.desc else 'parallel_apply')
+        except:
+            ...
+
 
-    total = len(data)
-    ids = list(range(total))
-    if parallel_node.shuffle:
-        random.shuffle(ids)
-    try:
-        from tqdm import tqdm
-        ids = tqdm(ids, total=total, desc=parallel_node.desc if parallel_node.desc else 'parallel_apply')
-    except:
-        ...
 
     #生成消费都是多进程
     if parallel_node.num_process_worker > 0 and parallel_node.num_process_worker > 0:
         pools = []
         for _ in range(parallel_node.num_process_worker):
-            p = Process(target=produce_input, args= (q_in,
-                                                    q_out,
-                                                    parallel_node.on_input_startup,
-                                                    parallel_node.on_input_process,
-                                                    parallel_node.on_input_cleanup,
-                                                    ))
+            p = Process(target=produce_input,
+                        args= (q_in,
+                               q_out,
+                               parallel_node.on_input_startup,
+                               parallel_node.on_input_process,
+                               parallel_node.on_input_cleanup))
             pools.append(p)
             p.start()
 
         for _ in range(parallel_node.num_process_post_worker):
-            p = Process(target=consume_output, args=(q_out,
-                                                    total,
-                                                    parallel_node.on_output_startup,
-                                                    parallel_node.on_output_process,
-                                                    parallel_node.on_output_cleanup
-                                                    ))
+            p = Process(target=consume_output,
+                        args=(q_out,
+                              parallel_node.num_process_worker,
+                              parallel_node.on_output_startup,
+                              parallel_node.on_output_process,
+                              parallel_node.on_output_cleanup))
             pools.append(p)
             p.start()
 
 
-        for i in ids:
-            q_in.put((i,data[i]))
+        if isinstance(data,typing.Sequence):
+            for i in ids:
+                q_in.put((i,data[i]))
+        else:
+            for i,d in enumerate(data):
+                q_in.put((i, d))
 
         for _ in range(parallel_node.num_process_worker):
             q_in.put((None, None))
 
         for p in pools:
             p.join()
     else:
-        #当前进程,弃用队列
+        #弃用队列
         parallel_node.on_input_startup()
-        for index in ids:
-            res = parallel_node.on_input_process(data[index])
-            parallel_node.on_output_process(res)
+        if isinstance(data, typing.Sequence):
+            for index in ids:
+                res = parallel_node.on_input_process(data[index])
+                parallel_node.on_output_process(res)
+        else:
+            for index,d in enumerate(data):
+                res = parallel_node.on_input_process(d)
+                parallel_node.on_output_process(res)
         parallel_node.on_output_cleanup()
-
     parallel_node.on_finalize()
-
     try:
         del q_in
         del q_out
     except:
         pass
```

## numpy_io/core/writer.py

```diff
@@ -17,15 +17,14 @@
                  input_fn: typing.Callable[[typing.Any, tuple], typing.Union[typing.Dict, typing.List, typing.Tuple]],
                  input_fn_args: typing.Union[typing.Tuple,typing.Dict],
                  outfile: typing.Union[str,list],
                  backend='record',
                  num_process_worker=0,
                  shuffle=True):
         assert E_file_backend.from_string(backend) is not None
-
         self.input_fn = input_fn
         self.input_fn_args = input_fn_args
         self.outfile = outfile
         self._backend_type = backend
         self._parallel_writer = ParallelNumpyWriter(num_process_worker=num_process_worker,shuffle=shuffle)
 
     @property
@@ -33,23 +32,22 @@
         return self._backend_type
 
     @backend_type.setter
     def backend_type(self, value):
         self._backend_type = value
 
     # 多进程写大文件
-    def save(self,data: list,
+    def save(self,data: typing.Union[typing.Sequence,typing.Iterator],
              options=None,
              parquet_options: typing.Optional = None,
              schema: typing.Optional[typing.Dict] = None,
              leveldb_write_buffer_size=1024 * 1024 * 512,
              leveldb_max_file_size=10 * 1024 * 1024 * 1024,
              lmdb_map_size=1024 * 1024 * 1024 * 150,
-             batch_size=None
-             ):
+             batch_size=None):
 
         self._parallel_writer.open(self.outfile ,
                                    backend=self.backend_type,
                                    schema=schema,
                                    parquet_options=parquet_options,
                                    options=options,
                                    leveldb_write_buffer_size=leveldb_write_buffer_size,
```

## Comparing `numpy_io-0.0.6.dist-info/RECORD` & `numpy_io-0.0.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 numpy_io/__init__.py,sha256=aCtpF76c1Jz1-xvsEqeV_ze4a40-KqaqUtIrFy3BTcU,77
-numpy_io/setup.py,sha256=YhzOCMf8CH_tZ3wBAQ04mm0IW69Z3ONR7Ci-1BOWRtY,628
+numpy_io/setup.py,sha256=6TqGB3Ng4epHGUoDZslKtuRSB0nAR5ljlActQLaJsT0,629
 numpy_io/core/__init__.py,sha256=gvmkt5S6jF7SlAsFM1e9qGGXV96a5yTB5lBavIVjuKo,80
-numpy_io/core/numpyadapter.py,sha256=snEnLu1oEEcn15fr7-FDaYYktCvhKVQPTAzAZdRFQ0Q,19443
-numpy_io/core/parallel.py,sha256=7pxBQ7w26H5wo1gHEMJwFwrkl57PDUA7rF3y8GD5kjM,5457
+numpy_io/core/numpyadapter.py,sha256=-hxHnhsbA4nF5HO-zytYUl3-UQOR1O4fqTwL9bbaVI0,19587
+numpy_io/core/parallel.py,sha256=-m_FKZegXe1q22A0nB3xgVE1edaRzjqYKlGroI0xgFA,5619
 numpy_io/core/reader.py,sha256=-i7NiW3s1gPFwaM03tDWT0NLVG6FEkz6fOuo_nWB3r8,1894
-numpy_io/core/writer.py,sha256=h0aobGbE2_QvM0bNVBg6gWz0uSR8gPrd8At6j56OJOA,2244
+numpy_io/core/writer.py,sha256=Oh81NqgmbesSEACUaymNKYm4YJln91rzELhLs9UjDWs,2268
 numpy_io/examples/__init__.py,sha256=H6PH5pOOHNUW3_RuUpgWfpv6_Pijqyy_3U1JCTLl6jg,54
 numpy_io/examples/auto_parallel_writer.py,sha256=geSpDCFHxe4skPd3Vk45lhc3azuJEPviGhcYtUlTid4,3236
 numpy_io/examples/auto_writer.py,sha256=vyvCXOJ5zroUweOOT0CFJnA8M_5nC8qJR0pxRv_8p88,3241
 numpy_io/examples/leveldb_readwriter_example.py,sha256=SKE4a3Wx67GPMbTmIlg8tIWT6JSxVc7QIRAi_gjOGvQ,1778
 numpy_io/examples/lmdb_readwriter_example.py,sha256=ZmZGfjy1o8c_O61JxXvKUrf6N_WSBGHHU1QCTK6DwH4,2218
 numpy_io/examples/memory_raw_readwriter_example.py,sha256=3LJzlLFFtDQdHyXM1dP7PupfnPb_0nM3qG4i7MF0MZg,1198
 numpy_io/examples/memory_readwriter_example.py,sha256=QAlov1poEZOYxmWNYgQkundKtST3VsFH10hTy3TE92w,1285
@@ -20,11 +20,11 @@
 numpy_io/examples/testing/lmdb_test.py,sha256=rQvokJAIDW9esAesab9wHs03OcG2TPImAuybnCO-LBA,2658
 numpy_io/examples/testing/test_mem.py,sha256=gteaDLS79vwwfJETTeL-JCxn3VhRT3So59y5AV4ah9w,613
 numpy_io/examples/testing/test_mutiprocess.py,sha256=rgO758tNAycWGYxyJl2AM2jkffNQs-AjRU9peSotGzQ,2907
 numpy_io/pytorch_loader/__init__.py,sha256=oRU1cnNHyp22vA9HkEYfoPtpdQdU4D9scv9KtgxYVdE,73
 numpy_io/pytorch_loader/data_helper.py,sha256=oVjtyWRobAYx1DMc5FePqQRyiQnoCpS60iidwHxN6k4,10309
 numpy_io/pytorch_loader/dataloaders.py,sha256=ov1DvKCv8GO4QGuoj09-BdUlDFop_4DScXMNv4B-jl0,8940
 numpy_io/pytorch_loader/tokenizer_config_helper.py,sha256=8hoofhL7uMyE8pT-U_3WNKDyy5DBOqQhDwJMZri-InY,3780
-numpy_io-0.0.6.dist-info/METADATA,sha256=EjlBsnnuFx7h8dywruUxxTWdHEF3S262-lHkyXTUqF8,389
-numpy_io-0.0.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-numpy_io-0.0.6.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
-numpy_io-0.0.6.dist-info/RECORD,,
+numpy_io-0.0.7.dist-info/METADATA,sha256=pn3IEZTtVh1PAzeiHFi22Ge32Xui9cblwLiQ4lpanaY,390
+numpy_io-0.0.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+numpy_io-0.0.7.dist-info/top_level.txt,sha256=mV0ZVKt8HA3kBLuj9iZkff1sq-cR9hE36TgSw_7Mr4E,9
+numpy_io-0.0.7.dist-info/RECORD,,
```

