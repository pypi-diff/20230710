# Comparing `tmp/estival-0.3.1.tar.gz` & `tmp/estival-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.3.1.tar", max compression
+gzip compressed data, was "estival-0.3.2.tar", max compression
```

## Comparing `estival-0.3.1.tar` & `estival-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       79 2023-06-30 01:05:55.108051 estival-0.3.1/estival/__init__.py
--rw-r--r--   0        0        0     4837 2023-06-30 01:03:28.991433 estival-0.3.1/estival/model.py
--rw-r--r--   0        0        0     4396 2023-06-30 01:03:28.992428 estival-0.3.1/estival/priors.py
--rw-r--r--   0        0        0       69 2023-06-26 23:53:46.119711 estival-0.3.1/estival/sampling/__init__.py
--rw-r--r--   0        0        0      220 2023-06-27 02:39:58.936134 estival-0.3.1/estival/sampling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2987 2023-06-30 01:06:23.734552 estival-0.3.1/estival/sampling/__pycache__/tools.cpython-310.pyc
--rw-r--r--   0        0        0     3617 2023-06-30 01:03:28.992928 estival-0.3.1/estival/sampling/tools.py
--rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.3.1/estival/targets.py
--rw-r--r--   0        0        0       24 2023-06-30 01:01:37.182961 estival-0.3.1/estival/utils/__init__.py
--rw-r--r--   0        0        0      170 2023-06-30 01:06:23.736049 estival-0.3.1/estival/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1696 2023-06-30 01:06:23.739049 estival-0.3.1/estival/utils/__pycache__/parallel.cpython-310.pyc
--rw-r--r--   0        0        0     1636 2023-06-30 01:03:28.993428 estival-0.3.1/estival/utils/parallel.py
--rw-r--r--   0        0        0       31 2023-06-30 01:01:24.074862 estival-0.3.1/estival/wrappers/__init__.py
--rw-r--r--   0        0        0      189 2023-06-30 01:06:23.741049 estival-0.3.1/estival/wrappers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3048 2023-06-30 01:06:23.747549 estival-0.3.1/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     3465 2023-06-30 01:06:23.744049 estival-0.3.1/estival/wrappers/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0     2906 2023-06-30 01:03:28.994438 estival-0.3.1/estival/wrappers/nevergrad.py
--rw-r--r--   0        0        0     3091 2023-06-30 01:03:28.994927 estival-0.3.1/estival/wrappers/pymc.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.3.1/LICENSE
--rw-r--r--   0        0        0     1034 2023-06-30 01:07:19.748623 estival-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      883 2023-06-30 01:07:12.285115 estival-0.3.1/README.md
--rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 estival-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2023-06-30 01:05:55.108051 estival-0.3.2/estival/__init__.py
+-rw-r--r--   0        0        0     4964 2023-07-04 01:20:36.989633 estival-0.3.2/estival/model.py
+-rw-r--r--   0        0        0     4396 2023-06-30 01:03:28.992428 estival-0.3.2/estival/priors.py
+-rw-r--r--   0        0        0       69 2023-06-26 23:53:46.119711 estival-0.3.2/estival/sampling/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-27 02:39:58.936134 estival-0.3.2/estival/sampling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5152 2023-07-04 00:57:59.489148 estival-0.3.2/estival/sampling/__pycache__/tools.cpython-310.pyc
+-rw-r--r--   0        0        0     5553 2023-07-10 03:11:03.316571 estival-0.3.2/estival/sampling/tools.py
+-rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.3.2/estival/targets.py
+-rw-r--r--   0        0        0       24 2023-06-30 01:01:37.182961 estival-0.3.2/estival/utils/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-30 01:06:23.736049 estival-0.3.2/estival/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1696 2023-06-30 01:06:23.739049 estival-0.3.2/estival/utils/__pycache__/parallel.cpython-310.pyc
+-rw-r--r--   0        0        0     1691 2023-07-10 03:10:22.130496 estival-0.3.2/estival/utils/parallel.py
+-rw-r--r--   0        0        0       31 2023-06-30 01:01:24.074862 estival-0.3.2/estival/wrappers/__init__.py
+-rw-r--r--   0        0        0      189 2023-06-30 01:06:23.741049 estival-0.3.2/estival/wrappers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3052 2023-07-01 05:32:17.468204 estival-0.3.2/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-06-30 01:06:23.744049 estival-0.3.2/estival/wrappers/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0     2920 2023-07-01 05:31:37.705798 estival-0.3.2/estival/wrappers/nevergrad.py
+-rw-r--r--   0        0        0     3091 2023-06-30 01:03:28.994927 estival-0.3.2/estival/wrappers/pymc.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1034 2023-07-10 03:13:12.233880 estival-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      978 2023-07-10 03:13:05.170700 estival-0.3.2/README.md
+-rw-r--r--   0        0        0     2108 1970-01-01 00:00:00.000000 estival-0.3.2/PKG-INFO
```

### Comparing `estival-0.3.1/estival/model.py` & `estival-0.3.2/estival/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 from dataclasses import dataclass
 
 from summer2 import CompartmentalModel
 
 from jax import jit
+import numpy as np
 
 import pandas as pd
 
 
 @dataclass
 class ResultsData:
     derived_outputs: pd.DataFrame
@@ -42,18 +43,22 @@
         self._build_logll_funcs(extra_ll)
 
     def _build_logll_funcs(self, extra_ll=None):
         model_params = self.model.get_input_parameters()
         dyn_params = list(model_params.intersection(set(self.priors)))
         self.model.set_derived_outputs_whitelist(list(self.targets))
 
-        self._ll_runner = self.model.get_runner(self.parameters, dyn_params)
+        self._ll_runner = self.model.get_runner(
+            self.parameters, dyn_params, include_full_outputs=False
+        )
 
         self.model.set_derived_outputs_whitelist([])
-        self._full_runner = self.model.get_runner(self.parameters, dyn_params)
+        self._full_runner = self.model.get_runner(
+            self.parameters, dyn_params, include_full_outputs=False
+        )
 
         self._evaluators = {}
         for k, t in self.targets.items():
             tev = t.get_evaluator(self._ref_idx, self.epoch)
             self._evaluators[k] = tev.evaluate
 
         @jit
@@ -90,15 +95,15 @@
 
         self._logll_multi = logll_multi
         self.loglikelihood = logll
 
     def logprior(self, **parameters):
         lp = 0.0
         for k, p in self.priors.items():
-            lp += p.logpdf(parameters[k])
+            lp += np.sum(p.logpdf(parameters[k]))
         return lp
 
     def logposterior(self, **parameters):
         return self.loglikelihood(**parameters) + self.logprior(**parameters)
 
     def run(self, parameters: dict, include_extras=False) -> ResultsData:
         """Run the model for a given set of parameters.
```

### Comparing `estival-0.3.1/estival/priors.py` & `estival-0.3.2/estival/priors.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.1/estival/targets.py` & `estival-0.3.2/estival/targets.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.1/estival/utils/__pycache__/parallel.cpython-310.pyc` & `estival-0.3.2/estival/utils/__pycache__/parallel.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.3.1/estival/utils/parallel.py` & `estival-0.3.2/estival/utils/parallel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-from typing import Callable, Iterable
-
-from multiprocessing import Pool, cpu_count
-
-import cloudpickle
-
-
-# initialize a worker in the process pool
-def process_init_cloudpickle(custom_cpkl):
-    """Initialize a mp.Process with custom cloudpickled data
-
-    Args:
-        custom_cpkl: The cloudpickle.dumps output of the custom data
-    """
-    # declare global variable
-    global custom_data
-    # assign the global variable
-    custom_data = cloudpickle.loads(custom_cpkl)
-
-
-def generic_cpkl_worker(*args):
-    """Worker function to be used with multiprocessing pools, where
-    custom_data is a global initialized to a function, usually via
-    process_init_cloudpickle
-
-    Returns:
-        Return type of the custom global function
-    """
-    global custom_data
-    run_func = custom_data
-
-    return run_func(*args)
-
-
-def map_parallel(run_func: Callable, input_iterator: Iterable, n_workers: int = None):
-    """Map the values of input_iterator over a function run_func, using n_workers parallel workers
-
-    Args:
-        run_func: The function to call over the mapped inputs
-        input_iterator: An iterable containing the values to map
-        n_workers: Number of processes used by Pool
-
-    Returns:
-        A list of values return by run_func
-    """
-
-    if n_workers is None:
-        n_workers = int(cpu_count() / 2)
-
-    with Pool(
-        n_workers, initializer=process_init_cloudpickle, initargs=(cloudpickle.dumps(run_func),)
-    ) as pool:
-        pres = pool.map(generic_cpkl_worker, input_iterator)
-        pool.close()
-        pool.join()
-    return pres
+from typing import Callable, Iterable
+
+from multiprocessing import Pool, cpu_count
+
+import cloudpickle
+
+
+# initialize a worker in the process pool
+def process_init_cloudpickle(custom_cpkl):
+    """Initialize a mp.Process with custom cloudpickled data
+
+    Args:
+        custom_cpkl: The cloudpickle.dumps output of the custom data
+    """
+    # declare global variable
+    global custom_data
+    # assign the global variable
+    custom_data = cloudpickle.loads(custom_cpkl)
+
+
+def generic_cpkl_worker(*args):
+    """Worker function to be used with multiprocessing pools, where
+    custom_data is a global initialized to a function, usually via
+    process_init_cloudpickle
+
+    Returns:
+        Return type of the custom global function
+    """
+    global custom_data
+    run_func = custom_data
+
+    return run_func(*args)
+
+
+def map_parallel(run_func: Callable, input_iterator: Iterable, n_workers: int = None):
+    """Map the values of input_iterator over a function run_func, using n_workers parallel workers
+
+    Args:
+        run_func: The function to call over the mapped inputs
+        input_iterator: An iterable containing the values to map
+        n_workers: Number of processes used by Pool
+
+    Returns:
+        A list of values return by run_func
+    """
+
+    if n_workers is None:
+        n_workers = int(cpu_count() / 2)
+
+    with Pool(
+        n_workers, initializer=process_init_cloudpickle, initargs=(cloudpickle.dumps(run_func),)
+    ) as pool:
+        pres = pool.map(generic_cpkl_worker, input_iterator)
+        # +++ We seem to get intermittent hanging here, and the context manager _should_ handle cleanup...
+        # pool.close()
+        # pool.join()
+    return pres
```

### Comparing `estival-0.3.1/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.3.2/estival/wrappers/__pycache__/nevergrad.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 01:03:28 2023 UTC, .py size: 2906 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e029 9e64 5a0b 0000  o........).dZ...
+00000000: 6f0d 0d0a 0000 0000 39ba 9f64 680b 0000  o.......9..dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a07 6400 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 7a06 6400 6404 6c0a 5a0b  m.Z...z.d.d.l.Z.
 00000070: 5700 6e04 0100 0100 0100 5900 6417 6407  W.n.......Y.d.d.
@@ -14,178 +14,178 @@
 000000d0: 5a14 6404 5300 2918 e900 0000 0029 01da  Z.d.S.)......)..
 000000e0: 0843 616c 6c61 626c 6529 01da 0766 7574  .Callable)...fut
 000000f0: 7572 6573 2901 da09 6370 755f 636f 756e  ures)...cpu_coun
 00000100: 744e 2901 da1a 4261 7965 7369 616e 436f  tN)...BayesianCo
 00000110: 6d70 6172 746d 656e 7461 6c4d 6f64 656c  mpartmentalModel
 00000120: da08 6d69 6470 6f69 6e74 6303 0000 0000  ..midpointc.....
 00000130: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
-00000140: 0000 0073 f800 0000 6900 7d03 7c01 6400  ...s....i.}.|.d.
+00000140: 0000 0073 fc00 0000 6900 7d03 7c01 6400  ...s....i.}.|.d.
 00000150: 7500 7208 6900 7d01 6900 7d04 7c00 a000  u.r.i.}.i.}.|...
-00000160: a100 4400 5d35 5c02 7d05 7d06 7c01 a001  ..D.]5\.}.}.|...
-00000170: 7c05 a101 0400 7d07 721e 7c07 7c04 7c05  |.....}.r.|.|.|.
-00000180: 3c00 710e 7c02 6401 6b02 722a 7402 a003  <.q.|.d.k.r*t...
-00000190: 6402 7c06 6a04 a102 7d08 6e12 7c02 6403  d.|.j...}.n.|.d.
-000001a0: 6b02 7237 7402 6a05 6a06 7c06 6a04 6404  k.r7t.j.j.|.j.d.
-000001b0: 8d01 7d08 6e05 7407 6405 7c02 8302 8201  ..}.n.t.d.|.....
-000001c0: 7c06 a008 7c08 a101 7c04 7c05 3c00 710e  |...|...|.|.<.q.
-000001d0: 7c00 a000 a100 4400 5d2a 5c02 7d05 7d06  |.....D.]*\.}.}.
-000001e0: 7c06 a009 a100 5c02 7d09 7d0a 7c06 6a04  |.....\.}.}.|.j.
-000001f0: 6406 6b02 7265 740a 6a0b 6a0c 7c04 7c05  d.k.ret.j.j.|.|.
-00000200: 1900 7c09 7c0a 6407 8d03 7c03 7c05 3c00  ..|.|.d...|.|.<.
-00000210: 7148 740a 6a0b 6a0d 7c04 7c05 1900 7c09  qHt.j.j.|.|...|.
-00000220: 7c0a 6407 8d03 7c03 7c05 3c00 7148 740a  |.d...|.|.<.qHt.
-00000230: 6a0b 6a0e 6408 6900 7c03 a401 8e01 5300  j.j.d.i.|.....S.
-00000240: 2909 4e72 0600 0000 6700 0000 0000 00e0  ).Nr....g.......
-00000250: 3fda 0775 6e69 666f 726d 2901 da04 7369  ?..uniform)...si
-00000260: 7a65 7a13 496e 7661 6c69 6420 696e 6974  zez.Invalid init
-00000270: 206d 6574 686f 64e9 0100 0000 2903 da04   method.....)...
-00000280: 696e 6974 da05 6c6f 7765 72da 0575 7070  init..lower..upp
-00000290: 6572 a900 290f da05 6974 656d 73da 0367  er..)...items..g
-000002a0: 6574 da02 6e70 da06 7265 7065 6174 7208  et..np..repeatr.
-000002b0: 0000 00da 0672 616e 646f 6d72 0700 0000  .....randomr....
-000002c0: da0a 5661 6c75 6545 7272 6f72 da03 7070  ..ValueError..pp
-000002d0: 66da 0662 6f75 6e64 73da 026e 67da 0170  f..bounds..ng..p
-000002e0: da06 5363 616c 6172 da05 4172 7261 795a  ..Scalar..ArrayZ
-000002f0: 0f49 6e73 7472 756d 656e 7461 7469 6f6e  .Instrumentation
-00000300: 290b da06 7072 696f 7273 da09 7375 6767  )...priors..sugg
-00000310: 6573 7465 64da 0b69 6e69 745f 6d65 7468  ested..init_meth
-00000320: 6f64 5a05 6964 6963 745a 0f73 7461 7274  odZ.idictZ.start
-00000330: 696e 675f 706f 696e 7473 da02 706b 7217  ing_points..pkr.
-00000340: 0000 005a 0673 7567 5f70 74da 0270 7072  ...Z.sug_pt..ppr
-00000350: 0b00 0000 720c 0000 0072 0d00 0000 720d  ....r....r....r.
-00000360: 0000 00fa 3043 3a5c 6465 765c 454d 555c  ....0C:\dev\EMU\
-00000370: 6573 7469 7661 6c5c 6573 7469 7661 6c5c  estival\estival\
-00000380: 7772 6170 7065 7273 5c6e 6576 6572 6772  wrappers\nevergr
-00000390: 6164 2e70 79da 1367 6574 5f69 6e73 7472  ad.py..get_instr
-000003a0: 756d 656e 7461 7469 6f6e 1100 0000 7326  umentation....s&
-000003b0: 0000 0004 0108 0204 0104 0210 010e 010a  ................
-000003c0: 0108 0210 0108 0112 010a 0210 0110 020c  ................
-000003d0: 010a 011c 011c 0212 0272 2000 0000 6300  .........r ...c.
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-000003f0: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
-00000400: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
-00000410: 8400 5a04 6405 5300 2906 da09 4f70 7452  ..Z.d.S.)...OptR
-00000420: 756e 6e65 7263 0400 0000 0000 0000 0000  unnerc..........
-00000430: 0000 0400 0000 0200 0000 4300 0000 7316  ..........C...s.
-00000440: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
-00000450: 037c 005f 0264 0053 0029 014e 2903 da09  .|._.d.S.).N)...
-00000460: 6f70 7469 6d69 7a65 72da 086d 696e 5f66  optimizer..min_f
-00000470: 756e 63da 0b6e 756d 5f77 6f72 6b65 7273  unc..num_workers
-00000480: 2904 da04 7365 6c66 7222 0000 0072 2300  )...selfr"...r#.
-00000490: 0000 7224 0000 0072 0d00 0000 720d 0000  ..r$...r....r...
-000004a0: 0072 1f00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
-000004b0: 2f00 0000 7306 0000 0006 0106 010a 017a  /...s..........z
-000004c0: 124f 7074 5275 6e6e 6572 2e5f 5f69 6e69  .OptRunner.__ini
-000004d0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-000004e0: 0500 0000 0800 0000 4300 0000 735a 0000  ........C...sZ..
-000004f0: 007c 006a 006a 017d 027c 027c 0117 007c  .|.j.j.}.|.|...|
-00000500: 006a 005f 0274 036a 047c 006a 0564 018d  .j._.t.j.|.j.d..
-00000510: 018f 127d 037c 006a 006a 067c 006a 077c  ...}.|.j.j.|.j.|
-00000520: 0364 028d 027d 0457 0064 0004 0004 0083  .d...}.W.d......
-00000530: 0301 007c 0453 0031 0073 2677 0101 0001  ...|.S.1.s&w....
-00000540: 0001 0059 0001 007c 0453 0029 034e 2901  ...Y...|.S.).N).
-00000550: da0b 6d61 785f 776f 726b 6572 7329 01da  ..max_workers)..
-00000560: 0865 7865 6375 746f 7229 0872 2200 0000  .executor).r"...
-00000570: 5a07 6e75 6d5f 6173 6bda 0662 7564 6765  Z.num_ask..budge
-00000580: 7472 0300 0000 da12 5468 7265 6164 506f  tr......ThreadPo
-00000590: 6f6c 4578 6563 7574 6f72 7224 0000 00da  olExecutorr$....
-000005a0: 086d 696e 696d 697a 6572 2300 0000 2905  .minimizer#...).
-000005b0: 7225 0000 0072 2900 0000 5a07 6375 725f  r%...r)...Z.cur_
-000005c0: 6173 6b72 2800 0000 da03 7265 6372 0d00  askr(.....recr..
-000005d0: 0000 720d 0000 0072 1f00 0000 722b 0000  ..r....r....r+..
-000005e0: 0034 0000 0073 1000 0000 0801 0c01 1001  .4...s..........
-000005f0: 1401 0aff 0402 10fe 0402 7a12 4f70 7452  ..........z.OptR
-00000600: 756e 6e65 722e 6d69 6e69 6d69 7a65 4e29  unner.minimizeN)
-00000610: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000620: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000630: 616d 655f 5f72 2600 0000 722b 0000 0072  ame__r&...r+...r
-00000640: 0d00 0000 720d 0000 0072 0d00 0000 721f  ....r....r....r.
-00000650: 0000 0072 2100 0000 2e00 0000 7306 0000  ...r!.......s...
-00000660: 0008 0008 010c 0572 2100 0000 69e8 0300  .......r!...i...
-00000670: 0054 da03 6263 6d72 2900 0000 7224 0000  .T..bcmr)...r$..
-00000680: 0072 1b00 0000 721c 0000 00da 0c6f 626a  .r....r......obj
-00000690: 5f66 756e 6374 696f 6e63 0800 0000 0000  _functionc......
-000006a0: 0000 0000 0000 0c00 0000 0500 0000 4300  ..............C.
-000006b0: 0000 736a 0000 007c 0373 0974 0074 0183  ..sj...|.s.t.t..
-000006c0: 0064 011b 0083 017d 0374 027c 006a 037c  .d.....}.t.|.j.|
-000006d0: 047c 0583 037d 0864 0264 0384 007d 097c  .|...}.d.d...}.|
-000006e0: 0664 0075 0072 1b7c 006a 047d 067c 0772  .d.u.r.|.j.}.|.r
-000006f0: 2274 057c 0683 017d 066e 047c 097c 0683  "t.|...}.n.|.|..
-00000700: 017d 067c 067d 0a7c 027c 087c 017c 0364  .}.|.}.|.|.|.|.d
-00000710: 048d 037d 0b74 067c 0b7c 0a7c 0383 0353  ...}.t.|.|.|...S
-00000720: 0029 054e e902 0000 0063 0100 0000 0000  .).N.....c......
-00000730: 0000 0000 0000 0200 0000 0300 0000 1300  ................
-00000740: 0000 7310 0000 0087 0066 0164 0164 0284  ..s......f.d.d..
-00000750: 087d 017c 0153 0029 034e 6300 0000 0000  .}.|.S.).Nc.....
-00000760: 0000 0000 0000 0001 0000 0005 0000 001b  ................
-00000770: 0000 0073 1200 0000 7400 8800 6401 6900  ...s....t...d.i.
-00000780: 7c00 a401 8e01 8301 5300 2902 4e72 0d00  |.......S.).Nr..
-00000790: 0000 a901 da05 666c 6f61 7429 01da 0a70  ......float)...p
-000007a0: 6172 616d 6574 6572 73a9 01da 0777 7261  arameters....wra
-000007b0: 7070 6564 720d 0000 0072 1f00 0000 da0d  ppedr....r......
-000007c0: 666c 6f61 745f 7772 6170 7065 724c 0000  float_wrapperL..
-000007d0: 0073 0200 0000 1201 7a37 6f70 7469 6d69  .s......z7optimi
-000007e0: 7a65 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  ze_model.<locals
-000007f0: 3e2e 6173 5f66 6c6f 6174 2e3c 6c6f 6361  >.as_float.<loca
-00000800: 6c73 3e2e 666c 6f61 745f 7772 6170 7065  ls>.float_wrappe
-00000810: 7272 0d00 0000 2902 7237 0000 0072 3800  rr....).r7...r8.
-00000820: 0000 720d 0000 0072 3600 0000 721f 0000  ..r....r6...r...
-00000830: 00da 0861 735f 666c 6f61 744b 0000 0073  ...as_floatK...s
-00000840: 0400 0000 0c01 0403 7a20 6f70 7469 6d69  ........z optimi
-00000850: 7a65 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  ze_model.<locals
-00000860: 3e2e 6173 5f66 6c6f 6174 2903 5a0f 7061  >.as_float).Z.pa
-00000870: 7261 6d65 7472 697a 6174 696f 6e72 2900  rametrizationr).
-00000880: 0000 7224 0000 0029 07da 0369 6e74 7204  ..r$...)...intr.
-00000890: 0000 0072 2000 0000 721a 0000 00da 0d6c  ...r ...r......l
-000008a0: 6f67 6c69 6b65 6c69 686f 6f64 da08 6e65  oglikelihood..ne
-000008b0: 6761 7469 7665 7221 0000 0029 0c72 3000  gativer!...).r0.
-000008c0: 0000 7229 0000 005a 096f 7074 5f63 6c61  ..r)...Z.opt_cla
-000008d0: 7373 7224 0000 0072 1b00 0000 721c 0000  ssr$...r....r...
-000008e0: 0072 3100 0000 5a0f 696e 7665 7274 5f66  .r1...Z.invert_f
-000008f0: 756e 6374 696f 6e5a 0769 6e73 7472 756d  unctionZ.instrum
-00000900: 7239 0000 0072 2300 0000 7222 0000 0072  r9...r#...r"...r
-00000910: 0d00 0000 720d 0000 0072 1f00 0000 da0e  ....r....r......
-00000920: 6f70 7469 6d69 7a65 5f6d 6f64 656c 3c00  optimize_model<.
-00000930: 0000 7318 0000 0004 0a0e 010e 0208 0208  ..s.............
-00000940: 0606 0104 010a 0108 0204 020e 010c 0172  ...............r
-00000950: 3d00 0000 6301 0000 0000 0000 0000 0000  =...c...........
-00000960: 0004 0000 0003 0000 000f 0000 0073 1000  .............s..
-00000970: 0000 8700 6601 6401 6402 8408 7d03 7c03  ....f.d.d...}.|.
-00000980: 5300 2903 7a7c 5772 6170 2061 2070 6f73  S.).z|Wrap a pos
-00000990: 6974 6976 6520 6675 6e63 7469 6f6e 2073  itive function s
-000009a0: 7563 6820 7468 6174 2061 206d 696e 696d  uch that a minim
-000009b0: 697a 6162 6c65 2076 6572 7369 6f6e 2069  izable version i
-000009c0: 7320 7265 7475 726e 6564 2069 6e73 7465  s returned inste
-000009d0: 6164 0a0a 2020 2020 4172 6773 3a0a 2020  ad..    Args:.  
-000009e0: 2020 2020 2020 663a 2054 6865 2063 616c        f: The cal
-000009f0: 6c61 626c 6520 746f 2077 7261 700a 2020  lable to wrap.  
-00000a00: 2020 6300 0000 0000 0000 0000 0000 0002    c.............
-00000a10: 0000 0006 0000 001f 0000 0073 1600 0000  ...........s....
-00000a20: 7400 6401 8800 7c00 6900 7c01 a401 8e01  t.d...|.i.|.....
-00000a30: 1800 8301 5300 2902 4e67 0000 0000 0000  ....S.).Ng......
-00000a40: 0000 7233 0000 0029 02da 0461 7267 73da  ..r3...)...args.
-00000a50: 066b 7761 7267 73a9 01da 0166 720d 0000  .kwargs....fr...
-00000a60: 0072 1f00 0000 da0a 5f72 6566 6c65 6374  .r......_reflect
-00000a70: 6564 6400 0000 7302 0000 0016 017a 1c6e  edd...s......z.n
-00000a80: 6567 6174 6976 652e 3c6c 6f63 616c 733e  egative.<locals>
-00000a90: 2e5f 7265 666c 6563 7465 6472 0d00 0000  ._reflectedr....
-00000aa0: 2904 7241 0000 0072 3e00 0000 723f 0000  ).rA...r>...r?..
-00000ab0: 0072 4200 0000 720d 0000 0072 4000 0000  .rB...r....r@...
-00000ac0: 721f 0000 0072 3c00 0000 5d00 0000 7304  r....r<...]...s.
-00000ad0: 0000 000c 0704 0372 3c00 0000 2902 4e72  .......r<...).Nr
-00000ae0: 0600 0000 2915 da06 7479 7069 6e67 7202  ....)...typingr.
-00000af0: 0000 00da 0a63 6f6e 6375 7272 656e 7472  .....concurrentr
-00000b00: 0300 0000 da0f 6d75 6c74 6970 726f 6365  ......multiproce
-00000b10: 7373 696e 6772 0400 0000 da05 6e75 6d70  ssingr......nump
-00000b20: 7972 1000 0000 5a0d 6573 7469 7661 6c2e  yr....Z.estival.
-00000b30: 6d6f 6465 6c72 0500 0000 da09 6e65 7665  modelr......neve
-00000b40: 7267 7261 6472 1600 0000 7220 0000 0072  rgradr....r ...r
-00000b50: 2100 0000 5a0a 6f70 7469 6d69 7a65 7273  !...Z.optimizers
-00000b60: 5a05 4e47 4f70 7472 3a00 0000 da04 6469  Z.NGOptr:.....di
-00000b70: 6374 da03 7374 7272 3d00 0000 723c 0000  ct..strr=...r<..
-00000b80: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000b90: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000ba0: 0000 0073 4000 0000 0c00 0c02 0c01 0802  ...s@...........
-00000bb0: 0c02 0203 0c01 0601 0201 0a03 0e1d 0210  ................
-00000bc0: 0601 0201 0201 0201 0201 0201 04f8 0201  ................
-00000bd0: 02ff 0202 02fe 0204 02fc 0205 02fb 0206  ................
-00000be0: 02fa 0207 0af9 0c21                      .......!
+00000160: a100 4400 5d37 5c02 7d05 7d06 7c01 a001  ..D.]7\.}.}.|...
+00000170: 7c05 a101 0400 7d07 6400 7501 7220 7c07  |.....}.d.u.r |.
+00000180: 7c04 7c05 3c00 710e 7c02 6401 6b02 722c  |.|.<.q.|.d.k.r,
+00000190: 7402 a003 6402 7c06 6a04 a102 7d08 6e12  t...d.|.j...}.n.
+000001a0: 7c02 6403 6b02 7239 7402 6a05 6a06 7c06  |.d.k.r9t.j.j.|.
+000001b0: 6a04 6404 8d01 7d08 6e05 7407 6405 7c02  j.d...}.n.t.d.|.
+000001c0: 8302 8201 7c06 a008 7c08 a101 7c04 7c05  ....|...|...|.|.
+000001d0: 3c00 710e 7c00 a000 a100 4400 5d2a 5c02  <.q.|.....D.]*\.
+000001e0: 7d05 7d06 7c06 a009 a100 5c02 7d09 7d0a  }.}.|.....\.}.}.
+000001f0: 7c06 6a04 6406 6b02 7267 740a 6a0b 6a0c  |.j.d.k.rgt.j.j.
+00000200: 7c04 7c05 1900 7c09 7c0a 6407 8d03 7c03  |.|...|.|.d...|.
+00000210: 7c05 3c00 714a 740a 6a0b 6a0d 7c04 7c05  |.<.qJt.j.j.|.|.
+00000220: 1900 7c09 7c0a 6407 8d03 7c03 7c05 3c00  ..|.|.d...|.|.<.
+00000230: 714a 740a 6a0b 6a0e 6408 6900 7c03 a401  qJt.j.j.d.i.|...
+00000240: 8e01 5300 2909 4e72 0600 0000 6700 0000  ..S.).Nr....g...
+00000250: 0000 00e0 3fda 0775 6e69 666f 726d 2901  ....?..uniform).
+00000260: da04 7369 7a65 7a13 496e 7661 6c69 6420  ..sizez.Invalid 
+00000270: 696e 6974 206d 6574 686f 64e9 0100 0000  init method.....
+00000280: 2903 da04 696e 6974 da05 6c6f 7765 72da  )...init..lower.
+00000290: 0575 7070 6572 a900 290f da05 6974 656d  .upper..)...item
+000002a0: 73da 0367 6574 da02 6e70 da06 7265 7065  s..get..np..repe
+000002b0: 6174 7208 0000 00da 0672 616e 646f 6d72  atr......randomr
+000002c0: 0700 0000 da0a 5661 6c75 6545 7272 6f72  ......ValueError
+000002d0: da03 7070 66da 0662 6f75 6e64 73da 026e  ..ppf..bounds..n
+000002e0: 67da 0170 da06 5363 616c 6172 da05 4172  g..p..Scalar..Ar
+000002f0: 7261 795a 0f49 6e73 7472 756d 656e 7461  rayZ.Instrumenta
+00000300: 7469 6f6e 290b da06 7072 696f 7273 da09  tion)...priors..
+00000310: 7375 6767 6573 7465 64da 0b69 6e69 745f  suggested..init_
+00000320: 6d65 7468 6f64 5a05 6964 6963 745a 0f73  methodZ.idictZ.s
+00000330: 7461 7274 696e 675f 706f 696e 7473 da02  tarting_points..
+00000340: 706b 7217 0000 005a 0673 7567 5f70 74da  pkr....Z.sug_pt.
+00000350: 0270 7072 0b00 0000 720c 0000 0072 0d00  .ppr....r....r..
+00000360: 0000 720d 0000 00fa 3043 3a5c 6465 765c  ..r.....0C:\dev\
+00000370: 454d 555c 6573 7469 7661 6c5c 6573 7469  EMU\estival\esti
+00000380: 7661 6c5c 7772 6170 7065 7273 5c6e 6576  val\wrappers\nev
+00000390: 6572 6772 6164 2e70 79da 1367 6574 5f69  ergrad.py..get_i
+000003a0: 6e73 7472 756d 656e 7461 7469 6f6e 1100  nstrumentation..
+000003b0: 0000 7326 0000 0004 0108 0204 0104 0210  ..s&............
+000003c0: 0112 010a 0108 0210 0108 0112 010a 0210  ................
+000003d0: 0110 020c 010a 011c 011c 0212 0272 2000  .............r .
+000003e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000003f0: 0000 0002 0000 0040 0000 0073 1c00 0000  .......@...s....
+00000400: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+00000410: 6403 6404 8400 5a04 6405 5300 2906 da09  d.d...Z.d.S.)...
+00000420: 4f70 7452 756e 6e65 7263 0400 0000 0000  OptRunnerc......
+00000430: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+00000440: 0000 7316 0000 007c 017c 005f 007c 027c  ..s....|.|._.|.|
+00000450: 005f 017c 037c 005f 0264 0053 0029 014e  ._.|.|._.d.S.).N
+00000460: 2903 da09 6f70 7469 6d69 7a65 72da 086d  )...optimizer..m
+00000470: 696e 5f66 756e 63da 0b6e 756d 5f77 6f72  in_func..num_wor
+00000480: 6b65 7273 2904 da04 7365 6c66 7222 0000  kers)...selfr"..
+00000490: 0072 2300 0000 7224 0000 0072 0d00 0000  .r#...r$...r....
+000004a0: 720d 0000 0072 1f00 0000 da08 5f5f 696e  r....r......__in
+000004b0: 6974 5f5f 2f00 0000 7306 0000 0006 0106  it__/...s.......
+000004c0: 010a 017a 124f 7074 5275 6e6e 6572 2e5f  ...z.OptRunner._
+000004d0: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+000004e0: 0000 0000 0500 0000 0800 0000 4300 0000  ............C...
+000004f0: 735a 0000 007c 006a 006a 017d 027c 027c  sZ...|.j.j.}.|.|
+00000500: 0117 007c 006a 005f 0274 036a 047c 006a  ...|.j._.t.j.|.j
+00000510: 0564 018d 018f 127d 037c 006a 006a 067c  .d.....}.|.j.j.|
+00000520: 006a 077c 0364 028d 027d 0457 0064 0004  .j.|.d...}.W.d..
+00000530: 0004 0083 0301 007c 0453 0031 0073 2677  .......|.S.1.s&w
+00000540: 0101 0001 0001 0059 0001 007c 0453 0029  .......Y...|.S.)
+00000550: 034e 2901 da0b 6d61 785f 776f 726b 6572  .N)...max_worker
+00000560: 7329 01da 0865 7865 6375 746f 7229 0872  s)...executor).r
+00000570: 2200 0000 5a07 6e75 6d5f 6173 6bda 0662  "...Z.num_ask..b
+00000580: 7564 6765 7472 0300 0000 da12 5468 7265  udgetr......Thre
+00000590: 6164 506f 6f6c 4578 6563 7574 6f72 7224  adPoolExecutorr$
+000005a0: 0000 00da 086d 696e 696d 697a 6572 2300  .....minimizer#.
+000005b0: 0000 2905 7225 0000 0072 2900 0000 5a07  ..).r%...r)...Z.
+000005c0: 6375 725f 6173 6b72 2800 0000 da03 7265  cur_askr(.....re
+000005d0: 6372 0d00 0000 720d 0000 0072 1f00 0000  cr....r....r....
+000005e0: 722b 0000 0034 0000 0073 1000 0000 0801  r+...4...s......
+000005f0: 0c01 1001 1401 0aff 0402 10fe 0402 7a12  ..............z.
+00000600: 4f70 7452 756e 6e65 722e 6d69 6e69 6d69  OptRunner.minimi
+00000610: 7a65 4e29 05da 085f 5f6e 616d 655f 5fda  zeN)...__name__.
+00000620: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000630: 7561 6c6e 616d 655f 5f72 2600 0000 722b  ualname__r&...r+
+00000640: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000650: 0000 721f 0000 0072 2100 0000 2e00 0000  ..r....r!.......
+00000660: 7306 0000 0008 0008 010c 0572 2100 0000  s..........r!...
+00000670: 69e8 0300 0054 da03 6263 6d72 2900 0000  i....T..bcmr)...
+00000680: 7224 0000 0072 1b00 0000 721c 0000 00da  r$...r....r.....
+00000690: 0c6f 626a 5f66 756e 6374 696f 6e63 0800  .obj_functionc..
+000006a0: 0000 0000 0000 0000 0000 0c00 0000 0500  ................
+000006b0: 0000 4300 0000 736a 0000 007c 0373 0974  ..C...sj...|.s.t
+000006c0: 0074 0183 0064 011b 0083 017d 0374 027c  .t...d.....}.t.|
+000006d0: 006a 037c 047c 0583 037d 0864 0264 0384  .j.|.|...}.d.d..
+000006e0: 007d 097c 0664 0075 0072 1b7c 006a 047d  .}.|.d.u.r.|.j.}
+000006f0: 067c 0772 2274 057c 0683 017d 066e 047c  .|.r"t.|...}.n.|
+00000700: 097c 0683 017d 067c 067d 0a7c 027c 087c  .|...}.|.}.|.|.|
+00000710: 017c 0364 048d 037d 0b74 067c 0b7c 0a7c  .|.d...}.t.|.|.|
+00000720: 0383 0353 0029 054e e902 0000 0063 0100  ...S.).N.....c..
+00000730: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000740: 0000 1300 0000 7310 0000 0087 0066 0164  ......s......f.d
+00000750: 0164 0284 087d 017c 0153 0029 034e 6300  .d...}.|.S.).Nc.
+00000760: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00000770: 0000 001b 0000 0073 1200 0000 7400 8800  .......s....t...
+00000780: 6401 6900 7c00 a401 8e01 8301 5300 2902  d.i.|.......S.).
+00000790: 4e72 0d00 0000 a901 da05 666c 6f61 7429  Nr........float)
+000007a0: 01da 0a70 6172 616d 6574 6572 73a9 01da  ...parameters...
+000007b0: 0777 7261 7070 6564 720d 0000 0072 1f00  .wrappedr....r..
+000007c0: 0000 da0d 666c 6f61 745f 7772 6170 7065  ....float_wrappe
+000007d0: 724c 0000 0073 0200 0000 1201 7a37 6f70  rL...s......z7op
+000007e0: 7469 6d69 7a65 5f6d 6f64 656c 2e3c 6c6f  timize_model.<lo
+000007f0: 6361 6c73 3e2e 6173 5f66 6c6f 6174 2e3c  cals>.as_float.<
+00000800: 6c6f 6361 6c73 3e2e 666c 6f61 745f 7772  locals>.float_wr
+00000810: 6170 7065 7272 0d00 0000 2902 7237 0000  apperr....).r7..
+00000820: 0072 3800 0000 720d 0000 0072 3600 0000  .r8...r....r6...
+00000830: 721f 0000 00da 0861 735f 666c 6f61 744b  r......as_floatK
+00000840: 0000 0073 0400 0000 0c01 0403 7a20 6f70  ...s........z op
+00000850: 7469 6d69 7a65 5f6d 6f64 656c 2e3c 6c6f  timize_model.<lo
+00000860: 6361 6c73 3e2e 6173 5f66 6c6f 6174 2903  cals>.as_float).
+00000870: 5a0f 7061 7261 6d65 7472 697a 6174 696f  Z.parametrizatio
+00000880: 6e72 2900 0000 7224 0000 0029 07da 0369  nr)...r$...)...i
+00000890: 6e74 7204 0000 0072 2000 0000 721a 0000  ntr....r ...r...
+000008a0: 00da 0d6c 6f67 6c69 6b65 6c69 686f 6f64  ...loglikelihood
+000008b0: da08 6e65 6761 7469 7665 7221 0000 0029  ..negativer!...)
+000008c0: 0c72 3000 0000 7229 0000 005a 096f 7074  .r0...r)...Z.opt
+000008d0: 5f63 6c61 7373 7224 0000 0072 1b00 0000  _classr$...r....
+000008e0: 721c 0000 0072 3100 0000 5a0f 696e 7665  r....r1...Z.inve
+000008f0: 7274 5f66 756e 6374 696f 6e5a 0769 6e73  rt_functionZ.ins
+00000900: 7472 756d 7239 0000 0072 2300 0000 7222  trumr9...r#...r"
+00000910: 0000 0072 0d00 0000 720d 0000 0072 1f00  ...r....r....r..
+00000920: 0000 da0e 6f70 7469 6d69 7a65 5f6d 6f64  ....optimize_mod
+00000930: 656c 3c00 0000 7318 0000 0004 0a0e 010e  el<...s.........
+00000940: 0208 0208 0606 0104 010a 0108 0204 020e  ................
+00000950: 010c 0172 3d00 0000 6301 0000 0000 0000  ...r=...c.......
+00000960: 0000 0000 0004 0000 0003 0000 000f 0000  ................
+00000970: 0073 1000 0000 8700 6601 6401 6402 8408  .s......f.d.d...
+00000980: 7d03 7c03 5300 2903 7a7c 5772 6170 2061  }.|.S.).z|Wrap a
+00000990: 2070 6f73 6974 6976 6520 6675 6e63 7469   positive functi
+000009a0: 6f6e 2073 7563 6820 7468 6174 2061 206d  on such that a m
+000009b0: 696e 696d 697a 6162 6c65 2076 6572 7369  inimizable versi
+000009c0: 6f6e 2069 7320 7265 7475 726e 6564 2069  on is returned i
+000009d0: 6e73 7465 6164 0a0a 2020 2020 4172 6773  nstead..    Args
+000009e0: 3a0a 2020 2020 2020 2020 663a 2054 6865  :.        f: The
+000009f0: 2063 616c 6c61 626c 6520 746f 2077 7261   callable to wra
+00000a00: 700a 2020 2020 6300 0000 0000 0000 0000  p.    c.........
+00000a10: 0000 0002 0000 0006 0000 001f 0000 0073  ...............s
+00000a20: 1600 0000 7400 6401 8800 7c00 6900 7c01  ....t.d...|.i.|.
+00000a30: a401 8e01 1800 8301 5300 2902 4e67 0000  ........S.).Ng..
+00000a40: 0000 0000 0000 7233 0000 0029 02da 0461  ......r3...)...a
+00000a50: 7267 73da 066b 7761 7267 73a9 01da 0166  rgs..kwargs....f
+00000a60: 720d 0000 0072 1f00 0000 da0a 5f72 6566  r....r......_ref
+00000a70: 6c65 6374 6564 6400 0000 7302 0000 0016  lectedd...s.....
+00000a80: 017a 1c6e 6567 6174 6976 652e 3c6c 6f63  .z.negative.<loc
+00000a90: 616c 733e 2e5f 7265 666c 6563 7465 6472  als>._reflectedr
+00000aa0: 0d00 0000 2904 7241 0000 0072 3e00 0000  ....).rA...r>...
+00000ab0: 723f 0000 0072 4200 0000 720d 0000 0072  r?...rB...r....r
+00000ac0: 4000 0000 721f 0000 0072 3c00 0000 5d00  @...r....r<...].
+00000ad0: 0000 7304 0000 000c 0704 0372 3c00 0000  ..s........r<...
+00000ae0: 2902 4e72 0600 0000 2915 da06 7479 7069  ).Nr....)...typi
+00000af0: 6e67 7202 0000 00da 0a63 6f6e 6375 7272  ngr......concurr
+00000b00: 656e 7472 0300 0000 da0f 6d75 6c74 6970  entr......multip
+00000b10: 726f 6365 7373 696e 6772 0400 0000 da05  rocessingr......
+00000b20: 6e75 6d70 7972 1000 0000 5a0d 6573 7469  numpyr....Z.esti
+00000b30: 7661 6c2e 6d6f 6465 6c72 0500 0000 da09  val.modelr......
+00000b40: 6e65 7665 7267 7261 6472 1600 0000 7220  nevergradr....r 
+00000b50: 0000 0072 2100 0000 5a0a 6f70 7469 6d69  ...r!...Z.optimi
+00000b60: 7a65 7273 5a05 4e47 4f70 7472 3a00 0000  zersZ.NGOptr:...
+00000b70: da04 6469 6374 da03 7374 7272 3d00 0000  ..dict..strr=...
+00000b80: 723c 0000 0072 0d00 0000 720d 0000 0072  r<...r....r....r
+00000b90: 0d00 0000 721f 0000 00da 083c 6d6f 6475  ....r......<modu
+00000ba0: 6c65 3e01 0000 0073 4000 0000 0c00 0c02  le>....s@.......
+00000bb0: 0c01 0802 0c02 0203 0c01 0601 0201 0a03  ................
+00000bc0: 0e1d 0210 0601 0201 0201 0201 0201 0201  ................
+00000bd0: 04f8 0201 02ff 0202 02fe 0204 02fc 0205  ................
+00000be0: 02fb 0206 02fa 0207 0af9 0c21            ...........!
```

### Comparing `estival-0.3.1/estival/wrappers/__pycache__/pymc.cpython-310.pyc` & `estival-0.3.2/estival/wrappers/__pycache__/pymc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.3.1/estival/wrappers/nevergrad.py` & `estival-0.3.2/estival/wrappers/nevergrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     idict = {}
 
     if suggested is None:
         suggested = {}
 
     starting_points = {}
     for pk, p in priors.items():
-        if sug_pt := suggested.get(pk):
+        if (sug_pt := suggested.get(pk)) is not None:
             starting_points[pk] = sug_pt
         else:
             if init_method == "midpoint":
                 pp = np.repeat(0.5, p.size)
             elif init_method == "uniform":
                 pp = np.random.uniform(size=p.size)
             else:
```

### Comparing `estival-0.3.1/estival/wrappers/pymc.py` & `estival-0.3.2/estival/wrappers/pymc.py`

 * *Files identical despite different names*

### Comparing `estival-0.3.1/LICENSE` & `estival-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.3.1/pyproject.toml` & `estival-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.3.1"
+version = "0.3.2"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
```

### Comparing `estival-0.3.1/README.md` & `estival-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,8 +22,11 @@
 - 0.3.0
 Note - breaking changes!
 Remove old AuTuMN MCMC implementation
 Move nevergrad/pymc -> wrappers
 Expand likelihood output tools
 Include parallelism framework
 - 0.3.1
-Bugfix (submodules not properly exported)
+Bugfix (submodules not properly exported)
+- 0.3.2
+SampleIterator tools (better support for shaped priors)
+Attempted map_parallel bugfix
```

### Comparing `estival-0.3.1/PKG-INFO` & `estival-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estival
-Version: 0.3.1
+Version: 0.3.2
 Summary: A set of calibration and probabilistic programming tools for use with summerepi2
 Home-page: https://github.com/monash-emu/estival
 License: BSD-2-Clause
 Keywords: calibration,optimization,bayesian,compartmental modelling,summerepi
 Author: David Shipman
 Author-email: dshipman@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -51,7 +51,11 @@
 Note - breaking changes!
 Remove old AuTuMN MCMC implementation
 Move nevergrad/pymc -> wrappers
 Expand likelihood output tools
 Include parallelism framework
 - 0.3.1
 Bugfix (submodules not properly exported)
+- 0.3.2
+SampleIterator tools (better support for shaped priors)
+Attempted map_parallel bugfix
+
```

