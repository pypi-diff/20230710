# Comparing `tmp/pepid-1.1.0.tar.gz` & `tmp/pepid-1.2.0.tar.gz`

## Comparing `pepid-1.1.0.tar` & `pepid-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,50 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/__main__.py
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/blackboard.py
--rw-r--r--   0        0        0    12846 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/db.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/db_node.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/drop_columns.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/drop_node.py
--rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/example_proteometools.cfg
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/example_proteometools_ml.cfg
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/example_yeast.cfg
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/extensions.py
--rw-r--r--   0        0        0     9943 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/finetune_rf_rescorer.py
--rw-r--r--   0        0        0    20150 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/gen_fdp_report.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/gen_fdp_report_debug.py
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/gen_fdr_report.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/main.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/node.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/output_node.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_compare.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_files.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_io.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_mgf_meta.py
--rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_mp.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_percolator.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_postprocess.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_randomforest.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_rescore.py
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_search.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pepid_utils.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/pin_node.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/post_node.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/queries.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/queries_node.py
--rw-r--r--   0        0        0    24915 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/search.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/search_node.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/test_model.py
--rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/train_rf_rescorer.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/data/default.cfg
--rw-r--r--   0        0        0     8142 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/ml/best_lgt_model.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 pepid-1.1.0/pepid/ml/train_best_lgt_model.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pepid-1.1.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pepid-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 pepid-1.1.0/README.md
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 pepid-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 pepid-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/__main__.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/blackboard.py
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/db.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/db_node.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/drop_columns.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/drop_node.py
+-rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/example_proteometools.cfg
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/example_proteometools_ml.cfg
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/example_yeast.cfg
+-rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/extensions.py
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/finetune_rf_rescorer.py
+-rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/gen_fdp_report.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/gen_fdp_report_debug.py
+-rw-r--r--   0        0        0    18207 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/gen_fdr_report.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/main.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/node.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/output_node.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_compare.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_files.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_io.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_mgf_meta.py
+-rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_mp.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_percolator.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_postprocess.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_randomforest.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_rescore.py
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_search.py
+-rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pepid_utils.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/pin_node.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/post_node.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/queries.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/queries_node.py
+-rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/scratch.py
+-rw-r--r--   0        0        0    25533 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/search.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/search_node.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/test_model.py
+-rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/test_specgen.py
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/data/default.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/ml/__init__.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/ml/best_lgt_model.py
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/ml/specgen.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/ml/train_best_lgt_model.py
+-rw-r--r--   0        0        0    10931 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/ml/train_rf_rescorer.py
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 pepid-1.2.0/pepid/ml/train_specgen.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pepid-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pepid-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 pepid-1.2.0/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 pepid-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9898 2020-02-02 00:00:00.000000 pepid-1.2.0/PKG-INFO
```

### Comparing `pepid-1.1.0/pepid/blackboard.py` & `pepid-1.2.0/pepid/blackboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 
 LOG = None
 CONN = None
 RES_CONN = None
 META_CONN = None
 LOCK = None
 
-def pin_template():
-    return ["PSMId", "Label", "ScanNr" ,"expMass", "calcMass", "FEATURES", "Peptide", "Proteins"]
-
 FEATS_BLACKLIST = set(["seq", "modseq", "title", "desc", "decoy", "file"]) # Set of keys generated by our default scoring functions to ignore during pin generation XXX needs cleanup/generalization
 
-config = configparser.ConfigParser(inline_comment_prefixes="#")
+config = configparser.ConfigParser(inline_comment_prefixes="#", allow_no_value=True)
 
 DB_TYPES = None
 RES_TYPES = None
 META_TYPES = None
 QUERY_TYPES = None
 DB_COLS = None
 RES_COLS = None
@@ -37,23 +34,14 @@
 RES_DB_FNAME = None
 META_DB_FNAME = None
 DB_PATH = None
 RES_DB_PATH = None
 META_DB_PATH = None
 TMP_PATH = None
 
-# Simple wrapper to hook into the sqlite3 auto-conversion system...
-class Spectrum(object):
-    def __init__(self, x):
-        self.data = x
-
-class Meta(object):
-    def __init__(self, x):
-        self.data = x
-
 def create_table_str(table_name, table_cols, table_types, extra=[]):
     return "CREATE TABLE IF NOT EXISTS {} ({});".format(table_name, ",".join(list(map(lambda x: "{} {}".format(x[0], x[1]), zip(table_cols, table_types))) + extra))
 
 def insert_all_str(table_name, table_cols):
     return "INSERT INTO {} ({}) VALUES ({});".format(table_name, ",".join(table_cols), ",".join(["?"]*len(table_cols)))
 
 def insert_dict_str(table_name, table_cols):
@@ -163,24 +151,18 @@
     RES_COLS = ["title", "desc", "seq", "modseq", "score", "query_charge", "query_mass", "cand_mass", "candrow", "qrow", "file", "rrow"]
     RES_TYPES = ["TEXT", "TEXT", "TEXT", "BLOB", "REAL", "INTEGER", "REAL", "REAL", "INTEGER", "INTEGER", "TEXT", "INTEGER"]
 
     META_COLS = ["qrow", "candrow", "data", "extra", "score", "rrow"] # score is used to mirror insertion exclusion via CHECK(score > 0) from the 'data' db
     META_TYPES = ["INTEGER", "INTEGER", "BLOB", "BLOB", "REAL", "INTEGER"]
 
     DB_COLS = ["desc", "decoy", "rt", "length", "mass", "seq", "mods", "spec", "meta"]
-    DB_TYPES = ["TEXT", "INTEGER", "REAL", "INTEGER", "REAL", "TEXT", "AUTOBLOB", "SPECTRUM", "META"]
+    DB_TYPES = ["TEXT", "INTEGER", "REAL", "INTEGER", "REAL", "TEXT", "BLOB", "BLOB", "BLOB"]
 
     QUERY_COLS = ["title", "rt", "charge", "mass", "spec", "min_mass", "max_mass", "meta"]
-    QUERY_TYPES = ["TEXT", "REAL", "INTEGER", "REAL", "SPECTRUM", "REAL", "REAL", "META"]
-
-    sqlite3.register_adapter(Spectrum, lambda x: pickle.dumps(x.data))
-    sqlite3.register_adapter(Meta, lambda x: msgpack.dumps(x.data))
-    sqlite3.register_converter("spectrum", lambda x: Spectrum(pickle.loads(x)))
-    sqlite3.register_converter("meta", lambda x: Meta(msgpack.loads(x)))
-    sqlite3.register_converter("autoblob", lambda x: msgpack.loads(x))
+    QUERY_TYPES = ["TEXT", "REAL", "INTEGER", "REAL", "BLOB", "REAL", "REAL", "META"]
 
     DB_FNAME = list(filter(lambda x: len(x) > 0, config['data']['database'].split('/')))[-1].rsplit('.', 1)[0]
     RES_DB_FNAME = DB_FNAME + ".sqlite"
     META_DB_FNAME = DB_FNAME + "_meta.sqlite"
 
     workdir = config['data']['workdir']
     try:
@@ -264,15 +246,27 @@
 def subprocess(args):
     extra_args = list(filter(lambda x: len(x) != 0, config['performance']['extra args'].strip().split(" ")))
     args = list(filter(lambda x: len(x) != 0, args))
     payload = [config['performance']['python']] + extra_args + args
     proc = sp.Popen(payload)
     return proc
 
-def lock():
-    fcntl.lockf(LOCK, fcntl.LOCK_EX)
-
-def unlock():
-    fcntl.lockf(LOCK, fcntl.LOCK_UN)
+def lock(f=None):
+    if f is None:
+        f = LOCK
+    fcntl.lockf(f, fcntl.LOCK_EX)
+
+def unlock(f=None):
+    if f is None:
+        f = LOCK
+    fcntl.lockf(f, fcntl.LOCK_UN)
+
+def acquire_lock(f=None):
+    if f is None:
+        f = os.path.join(TMP_PATH, ".lock")
+    else:
+        f = os.path.join(TMP_PATH, ".lock_" + f)
+    lock_file = open(f, "wb")
+    return lock_file
 
 def here(path):
     return os.path.join(os.path.dirname(os.path.abspath(__file__)), path)
```

### Comparing `pepid-1.1.0/pepid/db.py` & `pepid-1.2.0/pepid/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from os import path
 import math
 import time
 import os
 import random
 import copy
 import msgpack
+import pickle
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_utils
+    from pepid import blackboard
+    from pepid import pepid_utils
 else:
     from . import blackboard
     from . import pepid_utils
 
 class DbSettings():
     def __init__(self):
         pass
@@ -71,114 +72,146 @@
 def pred_rt(cands):
     """
     Dummy function for retention time prediction that just outputs 0.
     """
 
     return [0.0] * len(cands)
 
-def ml_spectrum(cands):
-    """
-    Spectrum prediction based on deep learning model
-    """
-
-    if __package__ is None or __package__ == '':
-        import spectrum_generator_sparse as spectrum_generator
-    else:
-        from . import spectrum_generator_sparse as spectrum_generator
-    import torch
-
-    global MODEL
-    try:
-        MODEL
-    except:
-        MODEL = None
-
-    if MODEL is None:
-        MODEL = spectrum_generator.Model().cuda()
-        MODEL.load_state_dict(torch.load("ml/spectrum_generator_sparse.pkl", map_location='cuda:0'))
-
-    cterm = blackboard.config['processing.db'].getfloat('cterm cleavage')
-    nterm = blackboard.config['processing.db'].getfloat('nterm cleavage')
-    max_charge = blackboard.config['processing.db'].getint('max charge')
-
-    out = []
-    for j in range(1, max_charge+1):
-        embs = []
-        for i in range(len(cands)):
-            embs.append(spectrum_generator.embed({"pep": cands[i]['seq'],
-                                                "mods": cands[i]['mods'],
-                                                "charge": j,
-                                                "mass": pepid_utils.neutral_mass(cands[i]['seq'], cands[i]['mods'], nterm, cterm, j)}))
-        embs = torch.FloatTensor(numpy.asarray(embs)).cuda()
-        out.append(MODEL(embs).view(len(cands), -1))
-        out[-1] = (out[-1] * (out[-1] >= 1e-3)).detach().cpu().numpy()
-    out = numpy.stack(out, axis=1)
-
-    import scipy
-    import scipy.sparse
-    return [scipy.sparse.csr_matrix(x) for x in out]
+MODEL = None
+class post_ml_spectrum(object):
+    required_fields = {'candidates': ['seq', 'mods']}
+
+    def __new__(cls, cands):
+        if __package__ is None or __package__ == '':
+            import pepid
+            from pepid.ml import specgen as specgen
+        else:
+            from .ml import specgen as specgen
+        import torch
+
+        batch_size = blackboard.config['processing.db.post_ml_spectrum'].getint('batch size')
+        device = blackboard.config['processing.db.post_ml_spectrum']['device']
+        if device is None:
+            device = 'cpu'
+
+        if 'cuda' in device:
+            blackboard.lock()
+            gpu_lock = blackboard.acquire_lock(device)
+
+            blackboard.lock(gpu_lock)
+
+            blackboard.unlock()
+
+        global MODEL
+
+        max_peaks = 500
+
+        if MODEL is None:
+            MODEL = specgen.Model().eval().to(device)
+            MODEL.load_state_dict(torch.load(blackboard.here("ml/best_specgen.pkl"), map_location=device))
+
+        cterm = blackboard.config['processing.db'].getfloat('cterm cleavage')
+        nterm = blackboard.config['processing.db'].getfloat('nterm cleavage')
+
+        payloads = []
+        out = numpy.zeros((len(cands), specgen.MAX_CHARGE, max_peaks, 2), dtype='float32')
+
+        for ic, c in enumerate(cands):
+            mods = msgpack.loads(c['mods'])
+            payloads.append({'pep': c['seq'], 'mods': mods, 'mass': pepid_utils.neutral_mass(c['seq'], mods, nterm, cterm, z=1)})
+
+            if (ic != 0 and ic % batch_size == 0) or (ic == len(cands)-1):
+                embs = specgen.embed_all(payloads)
+                payloads = []
+
+                with torch.no_grad():
+                    pred = MODEL(torch.FloatTensor(embs).to(device)).detach().cpu().numpy()
+                    sparsed = pepid_utils.dense_to_sparse(pred.reshape((-1, pred.shape[-1])), n_max = max_peaks)
+                    sparsed = sparsed.reshape((-1, pred.shape[1], sparsed.shape[-2], 2))
+                    out[ic-len(embs)+1:ic+1] = sparsed
+
+        if 'cuda' in device:
+            import gc
+            del MODEL
+            MODEL = None
+            gc.collect()
+            torch.cuda.empty_cache()
+            blackboard.unlock(gpu_lock)
+
+        for o in range(len(out)):
+            assert (o < len(cands)) and (o < len(out)), "WTF! {} {} {}".format(o, len(cands), len(out))
+            cands[o]['meta'] = pickle.dumps({'MLSpec': out[o]})
+        return cands
+
+class theoretical_spectrum(object):
+    required_fields = {'candidates': ['seq', 'mods']}
+
+    def __new__(cls, cands):
+        """
+        Spectrum prediction function generating b- and y-series ions
+        with charged variants
+        """
+
+        cterm = blackboard.config['processing.db'].getfloat('cterm cleavage')
+        nterm = blackboard.config['processing.db'].getfloat('nterm cleavage')
+        max_charge = blackboard.config['processing.db'].getint('max charge')
+        exclude_end = blackboard.config['processing.db.theoretical_spectrum'].getboolean('exclude last aa')
+        weights = eval(blackboard.config['processing.db.theoretical_spectrum']['weights'])
+
+        ret = []
+
+        for cand in cands:
+            seq = cand['seq']
+            mod = msgpack.loads(cand['mods'])
+            masses = pepid_utils.theoretical_masses(seq, mod, nterm, cterm, charge=max_charge, exclude_end=exclude_end, weights=weights)
+            ret.append(masses)
 
-def theoretical_spectrum(cands):
-    """
-    Spectrum prediction function generating b- and y-series ions
-    with charged variants
-    """
-
-    cterm = blackboard.config['processing.db'].getfloat('cterm cleavage')
-    nterm = blackboard.config['processing.db'].getfloat('nterm cleavage')
-    max_charge = blackboard.config['processing.db'].getint('max charge')
-    exclude_end = blackboard.config['processing.db.theoretical_spectrum'].getboolean('exclude last aa')
-    weights = eval(blackboard.config['processing.db.theoretical_spectrum']['weights'])
-
-    ret = []
-
-    for cand in cands:
-        seq = cand['seq']
-        mod = cand['mods']
-        masses = pepid_utils.theoretical_masses(seq, mod, nterm, cterm, charge=max_charge, exclude_end=exclude_end, weights=weights)
-        ret.append(masses)
-
-    return ret
+        return ret
 
 def stub(x):
     return x
 
 def user_processing(start, end):
     """
     Parses the spectrum prediction and rt prediction functions from config
     and applies them to the candidate peptides, adding the result to the corresponding candidate
     entry in the temporary database.
     """
 
+    import msgpack
+
     cur = blackboard.CONN.cursor()
     max_charge = blackboard.config['processing.db'].getint('max charge')
 
-    rt_fn = pepid_utils.import_or(blackboard.config['processing.db']['rt function'], pred_rt)
-    spec_fn = pepid_utils.import_or(blackboard.config['processing.db']['spectrum function'], theoretical_spectrum)
-    user_fn = pepid_utils.import_or(blackboard.config['processing.db']['postprocessing function'], stub)
+    rt_fn = pepid_utils.import_or(blackboard.config['processing.db']['rt function'].strip(), pred_rt)
+    spec_fn = pepid_utils.import_or(blackboard.config['processing.db']['spectrum function'].strip(), theoretical_spectrum)
+    user_fn = pepid_utils.import_or(blackboard.config['processing.db']['postprocessing function'].strip(), stub)
+
+    rows = set()
+    rows.add('rowid')
+    rows.update(getattr(user_fn, 'required_fields', {}).get('candidates', []))
+    rows.update(getattr(rt_fn, 'required_fields', {}).get('candidates', []))
+    rows.update(getattr(spec_fn, 'required_fields', {}).get('candidates', []))
 
-    blackboard.execute(cur, blackboard.select_str("candidates", blackboard.DB_COLS, "WHERE rowid BETWEEN ? AND ?"), (start+1, end))
+    blackboard.execute(cur, "SELECT {} FROM candidates WHERE rowid BETWEEN ? AND ?;".format(",".join(rows)), (start+1, end))
     data = cur.fetchall()
     data = list(map(dict, data))
 
     rts = rt_fn(data)
     specs = spec_fn(data)
 
-    specs = [blackboard.Spectrum(spec) for spec in specs]
+    specs = [pickle.dumps(spec) for spec in specs]
     
     for i in range(len(data)):
         data[i]['spec'] = specs[i]
         data[i]['rt'] = rts[i]
     ret = user_fn(data)
-    #rowids = list(range(start+1, end+1))
-    for r in ret:
-        r['mods'] = msgpack.dumps(r['mods'])
 
-    #blackboard.executemany(cur, "UPDATE candidates SET rt = ?, spec = ? WHERE rowid = ?;", list(zip(rts, specs, rowids)))
-    blackboard.executemany(cur, "REPLACE INTO candidates ({}) VALUES ({});".format(",".join(blackboard.DB_COLS), ",".join(list(map(lambda x: ":" + x, blackboard.DB_COLS)))), ret)
+    blackboard.executemany(cur, "UPDATE candidates SET {} WHERE rowid = :rowid;".format(",".join(["{} = :{}".format(k, k) for k in ret[0].keys()])), ret)
+    #blackboard.executemany(cur, "REPLACE INTO candidates ({}) VALUES ({});".format(",".join(blackboard.DB_COLS), ",".join(list(map(lambda x: ":" + x, blackboard.DB_COLS)))), ret)
     blackboard.commit()
 
 def process_entry(description, buff, settings):
     return process_entry_core(description, buff, settings, 'normal')
 
 def process_entry_decoy(description, buff, settings):
     return process_entry_core(description, buff, settings, 'decoy')
@@ -253,32 +286,32 @@
                                 if aa == mod and m == 0:
                                     var_list.append((curr_nmods+1, curr_mods[:iaa] + [sum(settings.var_mods[mod])] + curr_mods[iaa+1:]))
                   
             var_set = set(map(lambda x: tuple(x[1]), var_list)) # can't use lists in sets......
             for var in var_set:
                 mass = pepid_utils.theoretical_mass(peps[j], var, settings.nterm, settings.cterm)
                 if settings.min_mass <= mass <= settings.max_mass:
-                    data.append({"desc": description.split(" ", 1)[0], "decoy": seq_type == "decoy", "seq": peps[j], "mods": msgpack.dumps(var), "rt": 0.0, "length": len(peps[j]), "mass": mass, "spec": blackboard.Spectrum(None), 'meta': blackboard.Meta(None)})
+                    data.append({"desc": description.split(" ", 1)[0], "decoy": seq_type == "decoy", "seq": peps[j], "mods": msgpack.dumps(var), "rt": 0.0, "length": len(peps[j]), "mass": mass, "spec": pickle.dumps(None), 'meta': msgpack.dumps(None)})
     return data
 
 def fill_db(start, end, seq_type):
     """
     Processes database entries, performing digestion and generating variable mods as needed.
     Also applies config-specified mass and length filtering.
     Data is inserted in the temporary database.
 
     Peptide retention time prediction and peptide spectrum prediction are generated based on config at this stage.
     """
 
     batch_size = blackboard.config['processing.db'].getint('batch size')
     input_file = open(blackboard.config['data']['database'])
     if seq_type == 'decoy':
-        process_protein_fn = pepid_utils.import_or(blackboard.config['processing.db']['decoy protein processing function'], process_entry_decoy)
+        process_protein_fn = pepid_utils.import_or(blackboard.config['processing.db']['decoy protein processing function'].strip(), process_entry_decoy)
     else:
-        process_protein_fn = pepid_utils.import_or(blackboard.config['processing.db']['protein processing function'], process_entry)
+        process_protein_fn = pepid_utils.import_or(blackboard.config['processing.db']['protein processing function'].strip(), process_entry)
 
     settings = DbSettings()
     settings.load_settings()
 
     data = []
     buff = ""
     description = ""
```

### Comparing `pepid-1.1.0/pepid/db_node.py` & `pepid-1.2.0/pepid/pin_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,78 @@
 import struct
 import os
 import time
+import sys
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import node
+    from pepid import node
+    from pepid import blackboard
+    from pepid import pepid_utils
 else:
-    from . import blackboard
     from . import node
+    from . import blackboard
+    from . import pepid_utils
 
-class DbNode(node.Node):
+class PINNode(node.Node):
     def __init__(self, unix_sock):
         super().__init__(unix_sock)
         self.path = None
+        self.file = None
         self.messages[0x00] = [None, self.prepare]
-        self.messages[0x01] = [None, self.do]
-        self.messages[0x02] = ["!QQc", self.do_post]
+        self.messages[0x01] = ["!QQc", self.do]
 
-    def do(self, msg):
-        start, end = struct.unpack("!QQ", msg[:16])
-        if __package__ is None or __package__ == '':
-            import db
-        else:
-            from . import db
+    def do(self, start, end, _):
         if not self.path:
             raise ValueError("'do' message received before 'prepare' message, aborting.")
 
-        # leftover msg = decoy or normal
-        lgt = struct.unpack("!I", msg[16:20])[0]
-        db.fill_db(start, end, struct.unpack("!{}sc".format(lgt), msg[20:])[0].decode('utf-8'))
-        blackboard.CONN.commit()
-
-    def do_post(self, start, end, _):
-        if __package__ is None or __package__ == '':
-            import db
-        else:
-            from . import db
-        db.user_processing(start, end)
-        blackboard.CONN.commit()
+        in_fname = blackboard.config['data']['output']
+        fname, fext = in_fname.rsplit('.', 1)
+        suffix = blackboard.config['rescoring']['suffix']
+        pin_name = fname + suffix + "_pin.tsv"
+
+        fin = open(in_fname, 'r')
+
+        log_level = blackboard.config['logging']['level'].lower()
+
+        header = next(fin).strip().split("\t")
+        title_idx = header.index("title")
+
+        lines = []
+        cnt = -1
+        prev = None
+        for il, l in enumerate(fin):
+            line = l.strip().split("\t")
+            if line[title_idx] != prev:
+                prev = line[title_idx]
+                cnt += 1
+                if cnt < start:
+                    continue
+                if cnt >= end:
+                    break
+                lines.append([])
+            if start <= cnt < end:
+                lines[-1].append(l.strip().split("\t"))
+
+        fin.close()
+     
+        lines = pepid_utils.tsv_to_pin(header, lines, start)
+        for l in lines:
+            string = ""
+            for ll in l:
+                string += "\t".join(ll) + "\n"
+
+            blackboard.lock()
+            pin = open(pin_name, 'a')
+            pin.write(string)
+            pin.close()
+            blackboard.unlock()
 
     def prepare(self, msg):
         lgt = struct.unpack("!I", msg[:4])[0]
-        self.path = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
-        blackboard.TMP_PATH = self.path
+        blackboard.TMP_PATH = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
+        self.path = blackboard.TMP_PATH
         blackboard.setup_constants()
-        blackboard.LOCK = open(os.path.join(blackboard.TMP_PATH, ".lock"), "wb")
+        blackboard.LOCK = blackboard.acquire_lock()
         blackboard.prepare_connection()
 
 if __name__ == '__main__':
-    node.init(DbNode)
+    node.init(PINNode)
```

### Comparing `pepid-1.1.0/pepid/drop_columns.py` & `pepid-1.2.0/pepid/drop_columns.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/drop_node.py` & `pepid-1.2.0/pepid/drop_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,12 +44,12 @@
                 conn.close()
 
     def prepare(self, msg):
         lgt = struct.unpack("!I", msg[:4])[0]
         self.path = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
         blackboard.TMP_PATH = self.path
         blackboard.setup_constants()
-        blackboard.LOCK = open(os.path.join(blackboard.TMP_PATH, ".lock"), "wb")
+        blackboard.LOCK = blackboard.acquire_lock()
         blackboard.prepare_connection()
 
 if __name__ == '__main__':
     node.init(PostNode)
```

### Comparing `pepid-1.1.0/pepid/example_proteometools.cfg` & `pepid-1.2.0/pepid/example_proteometools.cfg`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/example_proteometools_ml.cfg` & `pepid-1.2.0/pepid/example_proteometools_ml.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 max mass = 6000
 max charge = 4 # Max charge for spectra
 min charge = 2 # Min charge for spectra
 
 [processing.db]
 enabled = true
 workers = 8
-postprocessing workers = 32
+postprocessing workers = 1
 protein processing function = db.process_entry
 decoy protein processing function = db.process_entry_decoy
-postprocessing function = db.stub
+postprocessing function = db.post_ml_spectrum
 batch size = 1180
 variable modifications = M+15.994915 # Comma-separated mod list (default: M(ox))
 max variable modifications = 3
 # Digestion rule as a regular expression
 max missed cleavages = 2
 # required digested peptide properties for inclusion below
 min length = 7
@@ -61,14 +61,22 @@
 # Missing values are considered to be 1.0
 # Example:
 # {"y": {"P": 5.0}, "b": {"D": 5.0, "N": 2.0, "V": 3.0, "E": 3.0, "Q": 2.0, "I": 3.0, "L": 3.0}} # x!tandem "synthesis"
 # An empty dict is {}, not the empty string.
 #weights = {"y": {"P": 5.0}, "b": {"D": 5.0, "N": 2.0, "V": 3.0, "E": 3.0, "Q": 2.0, "I": 3.0, "L": 3.0}} # x!tandem "synthesis"
 weights = {"y": {"P": 5.0}, "b": {"D": 5.0, "N": 2.0, "V": 3.0, "E": 3.0, "Q": 2.0, "I": 3.0, "L": 3.0}}
 
+[processing.db.post_ml_spectrum]
+batch size = 16
+device = cuda:0
+
+[postprocessing.length]
+batch size = 32
+device = cuda:0
+
 [postprocessing]
 enabled = true
 db = true
 queries = true
 
 # -> search.scoring
 [scoring]
@@ -158,15 +166,15 @@
 descending = true
 model = ml/rescorer_rf.pkl
 preprocessor = ml/rescorer_preproc.pkl
 
 [misc.tsv_to_pin]
 enabled = true
 use extra = true # Whether to insert the 'extra' metadata (inserted by postprocessors)
-user function = None # Function used to generate extra feature based on the input tsv lines
+user function = extensions.specgen_features # Function used to generate extra feature based on the input tsv lines
 max scores = 10 # Keep only top `max scores` PSMs in pin output
 
 [pipeline]
 search = true
 postsearch = true
 output = true
 report = true
```

### Comparing `pepid-1.1.0/pepid/example_yeast.cfg` & `pepid-1.2.0/pepid/example_yeast.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 [output]
 # Note that output operates at the db file level, mind the batch size!
 max retained candidates = 10
 workers = 64
 batch size = 16
 
 [rescoring]
-#function = pepid_randomforest.rescore
 function = pepid_percolator.rescore
 suffix = _final # Suffix to use to generate the rescored results filename. Cannot be empty.
 batch size = 1180 # Batch size for rescoring, in spectra
 
 [pipeline]
 search = true
 postsearch = true
```

### Comparing `pepid-1.1.0/pepid/extensions.py` & `pepid-1.2.0/pepid/extensions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,155 @@
 import numpy
 import time
 import msgpack
+import pickle
+import sys
 
 if __package__ is None or __package__ == '':
-    import blackboard
+    from pepid import blackboard
+    from pepid import pepid_utils
 else:
     from . import blackboard
+    from . import pepid_utils
 
-# This is an example user script containing user functions that may be specified in the config
+import numba
 
-model = None
-def predict_length(queries):
-    batch_size = blackboard.config['postprocessing.length'].getint('batch size')
-    device = blackboard.config['postprocessing.length']['device']
-    import torch
+@numba.njit(locals={'max_mz': numba.int32, 'mult': numba.float32, 'corr': numba.float32, 'sqr_ml': numba.float32, 'sqr_blit': numba.float32, 'mlspec': numba.float32[:,::1], 'blit': numba.float32[::1]})
+def correlate_spectra(blit, mlspec, max_mz, mult):
+    corr = 0
+    sqr_ml = 0
+    sqr_blit = 0
+    for mz, intens in mlspec:
+        if int(mz) >= max_mz / mult:
+            break
+        blit_int = blit[int(mz)]
+        corr += blit_int * intens
+        sqr_ml += intens**2
+        sqr_blit += blit_int**2
+    corr /= (numpy.sqrt(sqr_blit) * numpy.sqrt(sqr_ml) + 1e-10)
+
+    return corr
+
+def specgen_features(header, lines):
+    import sqlite3
+
+    batch_size = blackboard.config['pin.specgen_features'].getint('batch size')
+
+    cand_file = blackboard.DB_PATH + "_cands.sqlite"
+    qfile = blackboard.DB_PATH + "_q.sqlite"
 
     if __package__ is None or __package__ == '':
-        from ml import best_lgt_model as length_model
+        import pepid
+        from pepid.ml import specgen
     else:
-        from .ml import best_lgt_model as length_model
+        from .ml import specgen
 
-    global model
-    if model is None:      
-        model = length_model.Model()
-        model.to(device)
-        model.load_state_dict(torch.load(blackboard.here('ml/best_lgt_model.pkl'), map_location=device))
+    conn = sqlite3.connect(cand_file)
+    connq = sqlite3.connect(qfile)
+    conn.row_factory = sqlite3.Row
+    connq.row_factory = sqlite3.Row
+    cur = conn.cursor()
+    curq = connq.cursor()
 
     ret = []
-    batch = []
-    for iq, query in enumerate(queries):
-        spec = query['spec'].data
-        spec = spec[:length_model.PROT_TGT_LEN]
-        precmass = query['mass']
-
-        spec_raw = numpy.zeros((length_model.PROT_TGT_LEN,), dtype='float32')
-        for mz, intens in spec:
-            if mz == 0:
-                break
-            if mz / length_model.SIZE_RESOLUTION_FACTOR >= length_model.PROT_TGT_LEN - 0.5:
+
+    for i in range(0, len(lines), batch_size):
+        the_lines = lines[i:i+batch_size]
+        cands = [l[header.index('candrow')] for ll in the_lines for l in ll]
+        quers = [l[header.index('qrow')] for ll in the_lines for l in ll]
+        cur.execute("SELECT rowid, meta FROM candidates WHERE rowid IN ({}) ORDER BY rowid;".format(",".join(cands)))
+        curq.execute("SELECT rowid, spec FROM queries WHERE rowid in ({}) ORDER BY rowid;".format(",".join(quers)))
+        allcands = cur.fetchall()
+        extras = {r['rowid'] : pickle.loads(r['meta'])['MLSpec'] for r in allcands}
+        specs = {r['rowid'] : numpy.asarray(pickle.loads(r['spec']), dtype='float32') for r in curq.fetchall()}
+
+        for query_lines in lines[i:i+batch_size]:
+            if len(query_lines) == 0:
                 break
-            spec_raw[int(numpy.round(mz / length_model.SIZE_RESOLUTION_FACTOR))] += intens
-        max = spec_raw.max()
-        if max != 0:
-            spec_raw /= max
-
-        extra = query['meta'].data
-
-        batch.append([spec_raw, precmass, extra])
-        if len(batch) % batch_size == 0 or (len(batch) > 0 and iq == len(queries)-1):
-            spec_batch = numpy.array([b[0] for b in batch])
-            precmass_batch = numpy.array([b[1] for b in batch]).reshape((-1, 1)) / 2000.
-            out = model(torch.FloatTensor(spec_batch).to(device), torch.FloatTensor(precmass_batch).to(device))
-            preds = numpy.exp(out['pred'].view(-1, length_model.GT_MAX_LGT-length_model.GT_MIN_LGT+1).detach().cpu().numpy()).tolist()
-            for ib in range(len(batch)):
-                if batch[ib][-1] is not None:
-                    ret.append({**batch[ib][-1], 'LgtPred': preds[ib]})
-                else:
-                    ret.append({'LgtPred': preds[ib]})
-            batch = []
+            ret.append([])
+            for line in query_lines:
+                charge = int(line[header.index('query_charge')])-1
+                spec = specs[int(line[header.index('qrow')])]
+                blit = specgen.prepare_spec(spec)
+                mlspec = extras[int(line[header.index('candrow')])][min(charge, specgen.MAX_CHARGE-1)]
+                corr = correlate_spectra(blit, mlspec, specgen.MAX_MZ, 1.0 / specgen.SIZE_RESOLUTION_FACTOR)
+                ret[-1].append({'MLCorr': corr})
     return ret
 
-def insert_gt_length(queries):
-    ret = []
-    for iq, query in enumerate(queries):
-        extra = query['meta'].data
-        if 'mgf:SEQ' not in extra:
-            blackboard.LOG.error("Missing key 'mgf:SEQ' for insert_gt_length. Did you forget to run pepid_mgf_meta?")
-            sys.exit(-2)
+model = None
+class predict_length(object):
+    required_fields = {'queries': ['spec', 'mass', 'meta']}
+
+    def __new__(cls, queries):
+        batch_size = blackboard.config['postprocessing.length'].getint('batch size')
+        device = blackboard.config['postprocessing.length']['device']
+        if 'cuda' in device:
+            blackboard.lock()
+            gpu_lock = blackboard.acquire_lock(device)
+
+            blackboard.lock(gpu_lock)
+
+            blackboard.unlock()
+
+        import torch
+
+        if __package__ is None or __package__ == '':
+            import pepid
+            from pepid.ml import best_lgt_model as length_model
         else:
-            lgt = len(extra['mgf:SEQ'].replace("M(ox)", "1"))
-            pred = numpy.zeros((40-6+1), dtype='float32')
-            pred[lgt-6] = 1.
-            extra['LgtPred'] = pred.tolist()
-        ret.append(extra)
-    return ret
+            from .ml import best_lgt_model as length_model
+
+        global model
+        if model is None:      
+            model = length_model.Model().eval().to(device)
+            model.load_state_dict(torch.load(blackboard.here('ml/best_lgt_model.pkl'), map_location=device))
+
+        ret = []
+        batch = []
+        for iq, query in enumerate(queries):
+            spec = pickle.loads(query['spec'])
+            spec = numpy.asarray(spec[:length_model.PROT_TGT_LEN], dtype='float32')
+            precmass = query['mass']
+
+            spec_raw = pepid_utils.blit_spectrum(spec, length_model.PROT_TGT_LEN, length_model.SIZE_RESOLUTION_FACTOR)
+            extra = pickle.loads(query['meta'])
+
+            batch.append([spec_raw, precmass, extra])
+            if len(batch) % batch_size == 0 or (len(batch) > 0 and iq == len(queries)-1):
+                spec_batch = numpy.array([b[0] for b in batch])
+                precmass_batch = numpy.array([b[1] for b in batch]).reshape((-1, 1)) / 2000.
+                with torch.no_grad():
+                    out = model(torch.FloatTensor(spec_batch).to(device), torch.FloatTensor(precmass_batch).to(device))
+                    preds = numpy.exp(out['pred'].view(-1, length_model.GT_MAX_LGT-length_model.GT_MIN_LGT+1).detach().cpu().numpy())
+                for ib in range(len(batch)):
+                    if batch[ib][-1] is not None:
+                        ret.append({**batch[ib][-1], 'LgtPred': preds[ib]})
+                    else:
+                        ret.append({'LgtPred': preds[ib]})
+                batch = []
+        if 'cuda' in device:
+            import gc
+
+            del model
+            model = None
+            gc.collect()
+
+            torch.cuda.empty_cache()
+            blackboard.unlock(gpu_lock)
+
+        return ret
 
 def postprocess_for_length(start, end):
     import glob
     import os
     import sqlite3
 
     if __package__ is None or __package__ == '':
-        from ml import best_lgt_model as length_model
+        import pepid
+        from pepid.ml import best_lgt_model as length_model
     else:
         from .ml import best_lgt_model as length_model
 
     fname_pattern = list(filter(lambda x: len(x) > 0, blackboard.config['data']['database'].split('/')))[-1].rsplit('.', 1)[0] + "_*_pepidpart.sqlite"
     fname_path = os.path.join(blackboard.TMP_PATH, fname_pattern)
 
     files = sorted(glob.glob(fname_path))[start:end]
@@ -142,46 +206,50 @@
 
             new_meta = []
             for idata, data in enumerate(results):
                 cand_lgt = len(results_base[idata]['seq'])
                 m = msgpack.loads(data['extra'])
                 if m is None:
                     m = {}
-                preds = numpy.asarray(qmeta[results_base[idata]['qrow']].data['LgtPred'])
+                preds = pickle.loads(qmeta[results_base[idata]['qrow']])['LgtPred']
+                #preds = numpy.asarray(msgpack.loads(qmeta[results_base[idata]['qrow']])['LgtPred'], dtype='float32')
                 bests = numpy.argsort(preds, axis=-1)[::-1]
                 m['LgtPred'] = float(preds.argmax(axis=-1) + length_model.GT_MIN_LGT)
                 m['LgtProb'] = float(preds[cand_lgt - length_model.GT_MIN_LGT] if (length_model.GT_MIN_LGT <= cand_lgt <= length_model.GT_MAX_LGT) else 0)
                 m['LgtRelProb'] = float(m['LgtProb'] / preds.max(axis=-1))
                 m['LgtDelta'] = float(m['LgtPred'] - cand_lgt)
                 m['LgtDeltaAbs'] = float(abs(m['LgtPred'] - cand_lgt))
                 m['LgtScore'] = float(m['LgtProb'] * results_base[idata]['score'])
                 m['LgtRelScore'] = float(m['LgtRelProb'] * results_base[idata]['score'])
                 m['LgtProbDeltaBest'] = float(m['LgtProb'] - preds[bests[0]])
                 m['LgtProbDeltaWorst'] = float(m['LgtProb'] - preds[bests[-1]])
-                m['LgtProbDeltaPrev'] = float(0 if m['LgtProb'] == 0 else (m['LgtProb'] - preds[max(preds[bests].tolist().index(preds[cand_lgt - length_model.GT_MIN_LGT]) - 1, 0)]))
-                m['LgtProbDeltaNext'] = float(0 if m['LgtProb'] == 0 else (m['LgtProb'] - preds[min(preds[bests].tolist().index(preds[cand_lgt - length_model.GT_MIN_LGT]) + 1, len(preds)-1)]))
+                m['LgtProbDeltaPrev'] = float(0 if m['LgtProb'] == 0 else (m['LgtProb'] - preds[max(preds[bests].searchsorted(preds[cand_lgt - length_model.GT_MIN_LGT]) - 1, 0)]))
+                m['LgtProbDeltaNext'] = float(0 if m['LgtProb'] == 0 else (m['LgtProb'] - preds[min(preds[bests].searchsorted(preds[cand_lgt - length_model.GT_MIN_LGT]) + 1, len(preds)-1)]))
                 new_meta.append({'rrow': data['rrow'], 'data': msgpack.dumps(m)})
             blackboard.executemany(cur_meta_mod, 'UPDATE meta SET extra = :data WHERE rrow = :rrow;', new_meta)
             conn_meta.commit()
 
         del cur
         del conn
         del cur_meta
         del conn_meta
 
-def length_filter(cands, query):
-    meta = query['meta'].data
+class length_filter(object):
+    required_fileds = {'candidates': ['length'], 'queries': ['meta']}
 
-    best_lgts = numpy.argsort(meta['LgtPred'])[::-1] + 6
+    def __new__(cls, cands, query):
+        meta = msgpack.loads(query['meta'])
 
-    ret = []
-    for c in cands:
-        probs = numpy.asarray([meta['LgtPred'][b-6] for b in best_lgts])
-        if (probs[c['length']-6] >= 0.25):
-            if c['length'] in best_lgts[:2]:
+        best_lgts = numpy.argsort(meta['LgtPred'])[::-1] + 6
+
+        ret = []
+        for c in cands:
+            probs = numpy.asarray([meta['LgtPred'][b-6] for b in best_lgts])
+            if (probs[c['length']-6] >= 0.25):
+                if c['length'] in best_lgts[:2]:
+                    ret.append(c)
+            else:
                 ret.append(c)
-        else:
-            ret.append(c)
-    return ret
+        return ret
 
 def stub(*args):
     return None
```

### Comparing `pepid-1.1.0/pepid/finetune_rf_rescorer.py` & `pepid-1.2.0/pepid/finetune_rf_rescorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,45 @@
 import math
 import pickle
 import msgpack
 import tqdm
 import struct
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_utils
-    import queries
-    import pepid_mp
+    from pepid import blackboard
+    from pepid import pepid_utils
+    from pepid import queries
+    from pepid import pepid_mp
 else:
     from . import blackboard
     from . import pepid_utils
     from . import queries
     from . import pepid_mp
 
 def run(cfg):
     blackboard.config.read(blackboard.here("data/default.cfg"))
     blackboard.config.read(cfg)
 
     blackboard.setup_constants()
 
     log_level = blackboard.config['logging']['level'].lower()
     if blackboard.config['misc.tsv_to_pin'].getboolean('enabled'):
+        in_fname = blackboard.config['data']['output']
+        fname, fext = in_fname.rsplit('.', 1)
+        suffix = blackboard.config['rescoring']['suffix']
+        pin_name = fname + suffix + "_pin.tsv"
+ 
+        inf = open(in_fname, 'r')
+        header = next(inf).strip().split("\t")
+        line = next(inf).strip().split('\t')
+        inf.close()
+        pinf = open(pin_name, 'w')
+        pinf.write("\t".join(pepid_utils.generate_pin_header(header, line)) + "\n")
+        pinf.close()
+
         nworkers = blackboard.config['rescoring.finetune_rf'].getint('pin workers')
         batch_size = blackboard.config['rescoring.finetune_rf'].getint('pin batch size')
         n_total = queries.count_queries()
         n_batches = math.ceil(n_total / batch_size)
         spec = [(blackboard.here("pin_node.py"), nworkers, n_batches,
                         [struct.pack("!cI{}sc".format(len(blackboard.TMP_PATH)), bytes([0x00]), len(blackboard.TMP_PATH), blackboard.TMP_PATH.encode("utf-8"), "$".encode("utf-8")) for _ in range(nworkers)],
                         [struct.pack("!cQQc", bytes([0x01]), b * batch_size, min((b+1) * batch_size, n_total), "$".encode("utf-8")) for b in range(n_batches)],
@@ -37,37 +50,41 @@
         pepid_mp.handle_nodes("PIN Generation", spec, cfg_file=cfg, tqdm_silence=log_level in ['fatal', 'error', 'warning'])
 
     in_fname = blackboard.config['data']['output']
     fname, fext = in_fname.rsplit('.', 1)
     suffix = blackboard.config['rescoring']['suffix']
     pin_fname = fname + suffix + "_pin.tsv"
 
-    model_path = blackboard.config['rescoring.finetune_rf']['model']
-    preprocessor_path = blackboard.config['rescoring.finetune_rf']['preprocessor']
+    n_jobs = blackboard.config['rescoring.finetune_rf']['workers'].strip()
+    if n_jobs == '':
+        n_jobs = -1
+    else:
+        n_jobs = blackboard.config['rescoring.finetune_rf'].getint('workers')
 
+    model_path = blackboard.config['rescoring.finetune_rf']['model']
     model = pickle.load(open(blackboard.here(model_path), "rb"))
-    scaler = pickle.load(open(blackboard.here(preprocessor_path), "rb"))
 
     f = open(pin_fname, 'r')
     header = next(f).strip().split("\t")
     feats = header
-    del feats[feats.index('LgtRelScore')] # XXX HACK for now, delete when model gets retrained on Massive
 
-    f.close()
+    feats = [f for f in model['feats'] if f in header]
+    if any([x != y for x, y in zip(feats, model['feats'])]) or len(feats) != len(model['feats']):
+        blackboard.LOG.fatal("Incompatible features between model ({}) and pin file ({})".format(", ".join(model['feats']), ", ".join(header)))
+        sys.exit(-2)
 
-    template = blackboard.pin_template()
-    feats = [x for x in feats if x not in template]
+    f.close()
 
     import glob
 
     data = []
 
     import sqlite3
-    connq = sqlite3.connect("/scratch/zumerj/tmp/pepidrun_yeast/human_q.sqlite", detect_types=1)
-    connc = sqlite3.connect("/scratch/zumerj/tmp/pepidrun_yeast/human_cands.sqlite", detect_types=1)
+    connq = sqlite3.connect(blackboard.DB_PATH + "_q.sqlite", detect_types=1)
+    connc = sqlite3.connect(blackboard.DB_PATH + "_cands.sqlite", detect_types=1)
     connq.row_factory = sqlite3.Row
     connc.row_factory = sqlite3.Row
     curq = connq.cursor()
     curc = connc.cursor()
 
     f = open(pin_fname, 'r')
     header = next(f).strip().split("\t")
@@ -95,75 +112,81 @@
 
     blackboard.LOG.info("Fitting...")
 
     best_dir = True # i.e. bigger = better
     best_feat = 's'
     best_score = 0
 
-    feat_ipt = blackboard.config['rescoring.finetune_rf']['score']
-    feat_dir = blackboard.config['rescoring.finetune_rf'].getboolean('descending')
+    feat_ipt = blackboard.config['rescoring.finetune_rf']['score'].strip()
+    feat_dir = blackboard.config['rescoring.finetune_rf']['descending'].strip()
+    if feat_dir == '':
+        feat_dir = None
+    else:
+        feat_dir = blackboard.config['rescoring.finetune_rf'].getboolean('descending')
+    if feat_ipt == '':
+        feat_ipt = None
 
     if feat_ipt is None:
         for feat in feats + ['s']:
             for direction in [False, True]:
                 every.sort(order=[feat, 'target'])
                 if direction:
                     every = every[::-1]
 
                 fdrs = numpy.asarray(pepid_utils.calc_qval(every[feat], every['target'] > 0))
                 aw = numpy.argwhere(fdrs <= 0.01)
-                min_s = every[feat][(aw.reshape((-1,))[-1])+1] if len(aw) > 0 else (every[feat].max()+1) if direction else (every[feat].min()-1)
+                min_s = every[feat][(aw.reshape((-1,))[-1])] if len(aw) > 0 else (every[feat].max()+1) if direction else (every[feat].min()-1)
 
                 score = (every[feat] > min_s).sum() if direction else (every[feat] < min_s).sum()
                 if score > best_score:
                     best_dir = direction
                     best_feat = feat
 
                 blackboard.LOG.debug("[{}|{}] Identified past 1% FDR: {}".format(feat, ("+" if direction else "-"), score))
     else:
         best_feat = feat_ipt
-        direction = feat_dir
+        best_dir = feat_dir
 
     feat = best_feat
     direction = best_dir
 
     if not direction:
         every[feat] = -every[feat]
 
     every.sort(order=[feat, 'target'])
     every = every[::-1]
 
     fdrs = numpy.asarray(pepid_utils.calc_qval(every[feat], every['target'] > 0))
     aw = numpy.argwhere(fdrs <= 0.01)
-    min_s = every[feat][aw.reshape((-1,))[-1]+1] if len(aw) > 0 else every[feat].max()+1
+    min_s = every[feat][aw.reshape((-1,))[-1]] if len(aw) > 0 else every[feat].max()+1
 
     keys = numpy.unique(every['title'])
     grouped_data = {k: [] for k in keys}
     for d in every:
         if len(grouped_data[d['title']]) >= 1:
             continue
         grouped_data[d['title']].append(d)
     data = numpy.hstack([grouped_data[group] for group in grouped_data])
 
     data.sort(order=[feat, 'target'])
     data = data[::-1]
 
     fdrs = numpy.asarray(pepid_utils.calc_qval(data[feat], data['target'] > 0))
     aw = numpy.argwhere(fdrs <= 0.01)
-    min_st = data[feat][aw.reshape((-1,))[-1]+1] if len(aw) > 0 else data[feat].max()+1
+    min_st = data[feat][aw.reshape((-1,))[-1]] if len(aw) > 0 else data[feat].max()+1
 
     blackboard.LOG.info("Total: {}".format(len(every)))
     blackboard.LOG.info("[{}] Identified past 1% FDR: {}".format(feat, (every[feat] > min_s).sum()))
     blackboard.LOG.info("Top-1: [{}] Identified past 1% FDR: {}".format(feat, (data[feat] > min_st).sum()))
 
     out_transformed = numpy.zeros((every.shape[0],), dtype='float32')
 
     fdrs = numpy.asarray(pepid_utils.calc_qval(every[feat], every['target'] > 0))
     aw = numpy.argwhere(fdrs <= 0.01)
-    min_s = every[feat][aw.reshape((-1,))[-1]+1] if len(aw) > 0 else every[feat].max()+1
+    min_s = every[feat][aw.reshape((-1,))[-1]] if len(aw) > 0 else every[feat].max()+1
 
     lvl = every[int(0.5 * len(every))][feat]
 
     every_groups = []
     prev_title = None
     idx = -1
     for title in every['title']:
@@ -182,17 +205,17 @@
     for i, (train_idxs, test_idxs) in enumerate(fold.split(every, groups=every_groups)):
         blackboard.LOG.debug("Fold {}: Init data".format(i+1))
 
         train_feats = every_feats[train_idxs] #[is_index[train_idxs]]
         train_labs = every_labs[train_idxs] #[is_index[train_idxs]]
 
         blackboard.LOG.debug("Fold {}: Train".format(i+1))
-        rf_gt = model
-        rf_finetune = ensemble.RandomForestClassifier(n_jobs=-1)
-        scaler = scaler
+        rf_gt = model['model']
+        rf_finetune = ensemble.RandomForestClassifier(n_jobs=n_jobs)
+        scaler = model['scaler']
 
         train_labs = [1 if (t[feat] >= lvl and t['target'] > 0.5) else 0 for t in every[train_idxs]]
 
         rf_finetune.fit(scaler.transform(every_feats[train_idxs]), train_labs)
 
         blackboard.LOG.debug("Fold {}: Test".format(i+1))
 
@@ -216,15 +239,15 @@
         data.append(grouped_data[g][numpy.argmax([gg[0] for gg in grouped_data[g]])])
     data = numpy.asarray(data, dtype=[('s', numpy.float32), ('title', object), ('seq', object), ('target', numpy.int32)])
     data.sort(order=['s', 'target'])
     data = data[::-1]
 
     fdrs = numpy.asarray(pepid_utils.calc_qval(data['s'], data['target'] > 0))
     aw = numpy.argwhere(fdrs <= 0.01)
-    min_st = data['s'][min(len(data)-1, aw.reshape((-1,))[-1]+1)] if len(aw) > 0 else data['s'].max()+1
+    min_st = data['s'][min(len(data)-1, aw.reshape((-1,))[-1])] if len(aw) > 0 else data['s'].max()+1
     blackboard.LOG.debug("FDRS/target: {} {}".format(fdrs[0], fdrs[-1]))
 
     blackboard.LOG.info("Identified past 1% FDR: {}".format((data['s'] > min_st).sum()))
 
     fin = open(in_fname, "r")
     assoc = {}
     in_header = next(fin).strip().split("\t")
```

### Comparing `pepid-1.1.0/pepid/gen_fdp_report.py` & `pepid-1.2.0/pepid/gen_fdp_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import numpy
 import sys
 import os
 import tqdm
 import math
 import sqlite3
 
+import pickle
+
 if __package__ is None or __package__ == '':
-    import pepid_utils
+    from pepid import pepid_utils
 else:
     from . import pepid_utils
 
 # TODO: Currently only handles mgf:SEQ based on the proteometools mega-mgf I generated with a SEQ= line
 # This could be made more general by requiring mgf:SEQ to be in the same format as immplied by the modifications settings instead
 # In addition, the field (e.g. mgf:SEQ) could be made more dynamic
 # This could tie into future plans to allow combining multiple custom functions through providing a function list + a 'resolver' function that combines all
 # the outputs into one payload, which will affect how metadata postprocessing functions are handled.
 
 if __package__ is None or __package__ == '':
-    import blackboard
+    from pepid import blackboard
 else:
     from . import blackboard
 
 def tda_fdr(rescored=False):
     fname, fext = blackboard.config['data']['output'].rsplit(".", 1)
     full_fname = (fname + "." + fext) if not rescored else (fname + blackboard.config['rescoring']['suffix'] + "." + fext)
     decoy_prefix = blackboard.config['processing.db']['decoy prefix']
@@ -96,15 +98,15 @@
     batch_size = 10000
     for i in range(0, len(ndata), batch_size):
         rowids = [str(x) for x in numpy.unique(ndata['qrow'][i:i+batch_size]).tolist()]
         qcur.execute("SELECT rowid, meta FROM queries WHERE rowid IN ({}) ORDER BY rowid;".format(",".join(rowids)))
         meta = qcur.fetchall()
         mm = {}
         for m in meta:
-            mm[m['rowid']] = m['meta'].data
+            mm[m['rowid']] = pickle.loads(m['meta'])
             if 'mgf:SEQ' not in mm[m['rowid']]:
                 blackboard.LOG.error("Required key 'mgf:SEQ' not found (first error at {})".format(m['rowid']))
                 sys.exit(-2)
 
         for d in ndata[i:i+batch_size]:
             meta = mm[d['qrow']]
             d['lgt'] = len(meta['mgf:SEQ'].replace("M(ox)", "1"))
@@ -130,18 +132,18 @@
 
     if len(fdrs) == 0:
         blackboard.LOG.warning("Empty fdr levels in fdr report")
         fdrss = numpy.array([0])
 
     fdr_limit = float(blackboard.config['report']['fdr threshold'])
     aw = numpy.argwhere(fdrs <= fdr_limit)
-    idx = min(len(data)-1, aw.reshape((-1,))[-1]+1) if len(aw) > 0 else -1
+    idx = min(len(data)-1, aw.reshape((-1,))[-1]) if len(aw) > 0 else -1
 
-    blackboard.LOG.info("Overall FDR: {}; FDR range: {}-{}; PSM@{}%: {}".format(fdr, fdrs[0], fdrs[-1], int(fdr_limit * 100.), (data['score'] > data['score'][idx]).sum() if idx >= 0 else 0))
-    blackboard.LOG.info("Unique peps@{}%: {}".format(int(fdr_limit * 100.), len(numpy.unique(data[(data['score'] > data['score'][idx])]['seq'])) if idx >= 0 else 0))
+    blackboard.LOG.info("Overall FDR: {}; FDR range: {}-{}; PSM@{}%: {}".format(fdr, fdrs[0], fdrs[-1], int(fdr_limit * 100.), (data['score'] >= data['score'][idx]).sum() if idx >= 0 else 0))
+    blackboard.LOG.info("Unique peps@{}%: {}".format(int(fdr_limit * 100.), len(numpy.unique(data[(data['score'] >= data['score'][idx])]['modseq'])) if idx >= 0 else 0))
 
     ufdrs = numpy.unique(fdrs)
     levels = []
     for u in ufdrs:
         levels.append((fdrs <= u).sum())
 
     return {
```

### Comparing `pepid-1.1.0/pepid/gen_fdp_report_debug.py` & `pepid-1.2.0/pepid/gen_fdp_report_debug.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/gen_fdr_report.py` & `pepid-1.2.0/pepid/gen_fdr_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy
 import sys
 import os
 import tqdm
 import math
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_utils
+    from pepid import blackboard
+    from pepid import pepid_utils
 else:
     from . import blackboard
     from . import pepid_utils
 
 def tda_fdr(rescored=False):
     fname, fext = blackboard.config['data']['output'].rsplit(".", 1)
     full_fname = (fname + "." + fext) if not rescored else (fname + blackboard.config['rescoring']['suffix'] + "." + fext)
@@ -55,15 +55,15 @@
                         if n >= topN:
                             break
                         data.append(staged[idx])
                     del idxs
                     del staged
                     staged = []
             if not math.isinf(score):
-                staged.append((title, seq, score, desc.startswith(decoy_prefix), qrow, candrow, len(seq), charge, mass))
+                staged.append((title, modseq, score, desc.startswith(decoy_prefix), qrow, candrow, len(seq), charge, mass))
 
     idxs = numpy.argsort([s[2] for s in staged])[::-1]
     for n, idx in enumerate(idxs):
         if n >= topN:
             break
         data.append(staged[idx])
     del staged
@@ -95,18 +95,18 @@
 
     if len(fdrs) == 0:
         blackboard.LOG.warning("Empty fdr levels in fdr report")
         fdrs = numpy.array([0])
 
     fdr_limit = float(blackboard.config['report']['fdr threshold'])
     aw = numpy.argwhere(fdrs <= fdr_limit)
-    idx = min(len(data)-1, aw.reshape((-1,))[-1]+1) if len(aw) > 0 else -1
+    idx = min(len(data)-1, aw.reshape((-1,))[-1]) if len(aw) > 0 else -1
 
-    blackboard.LOG.info("Overall FDR: {}; FDR range: {}-{}; PSM@{}%: {}".format(fdr, fdrs[0], fdrs[-1], int(fdr_limit * 100.), (data['score'] > data['score'][idx]).sum() if idx >= 0 else 0))
-    blackboard.LOG.info("Unique peps@{}%: {}".format(int(fdr_limit * 100.), len(numpy.unique(data[(data['score'] > data['score'][idx])]['seq'])) if idx >= 0 else 0))
+    blackboard.LOG.info("Overall FDR: {}; FDR range: {}-{}; PSM@{}%: {}".format(fdr, fdrs[0], fdrs[-1], int(fdr_limit * 100.), (data['score'] >= data['score'][idx]).sum() if idx >= 0 else 0))
+    blackboard.LOG.info("Unique peps@{}%: {}".format(int(fdr_limit * 100.), len(numpy.unique(data[(data['score'] >= data['score'][idx])]['seq'])) if idx >= 0 else 0))
 
     ufdrs = numpy.unique(fdrs)
     levels = []
     for u in ufdrs:
         levels.append((fdrs <= u).sum())
 
     return {
```

### Comparing `pepid-1.1.0/pepid/main.py` & `pepid-1.2.0/pepid/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import time
 import os
 
 if __package__ is None or __package__ == '':
-    import blackboard
+    from pepid import blackboard
     from blackboard import here
 else:
     from . import blackboard
     from .blackboard import here
 
 def run(cfg):
     ret = 0
@@ -102,14 +102,15 @@
 
     finally:
         if log_level in ['debug', 'info']:
             sys.stderr.write("Cleaning up...\n")
         import os
         os.system("rm -rf {}".format(os.path.join(blackboard.config['data']['tmpdir'], "pepid_socket*")))
         os.system("rm -rf {}".format(os.path.join(blackboard.config['data']['workdir'], ".lock")))
+        os.system("rm -rf {}".format(os.path.join(blackboard.config['data']['workdir'], ".lock_*"))) # Locks possibly created for e.g. devices
 
         sys.exit(ret)
 
 if __name__ == '__main__':
     if len(sys.argv) != 2:
         print("USAGE: {} config.cfg".format(sys.argv[0]))
         sys.exit(-1)
```

### Comparing `pepid-1.1.0/pepid/node.py` & `pepid-1.2.0/pepid/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import struct
 import os
 import uuid
 import numpy
 import tempfile
 
 if __package__ is None or __package__ == '':
-    import blackboard
+    from pepid import blackboard
 else:
     from . import blackboard
 
 # Messages:
 # 0xff: acknowledged, followed by message code being acknowledged
 # 0xfe: done, followed by code of task done
 # 0xfd: error (next 4 bytes are size of incoming error message, followed by message as utf-8)
```

### Comparing `pepid-1.1.0/pepid/output_node.py` & `pepid-1.2.0/pepid/search_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import struct
 import os
 import time
 import sys
 
 if __package__ is None or __package__ == '':
-    import node
-    import blackboard
+    from pepid import blackboard
+    from pepid import node
 else:
-    from . import node
     from . import blackboard
+    from . import node
+
 
-class OutputNode(node.Node):
+class SearchNode(node.Node):
     def __init__(self, unix_sock):
         super().__init__(unix_sock)
         self.path = None
-        self.file = None
         self.messages[0x00] = [None, self.prepare]
         self.messages[0x01] = ["!QQc", self.do]
 
     def do(self, start, end, _):
         if __package__ is None or __package__ == '':
-            import pepid_io
+            from pepid import search
         else:
-            from . import pepid_io
+            from . import search
 
         if not self.path:
             raise ValueError("'do' message received before 'prepare' message, aborting.")
 
-        pepid_io.write_output(start, end)
+        search.search_core(start, end)
 
     def prepare(self, msg):
         lgt = struct.unpack("!I", msg[:4])[0]
         blackboard.TMP_PATH = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
         self.path = blackboard.TMP_PATH
         blackboard.setup_constants()
-        blackboard.LOCK = open(os.path.join(blackboard.TMP_PATH, ".lock"), "wb")
+        blackboard.LOCK = blackboard.acquire_lock()
         blackboard.prepare_connection()
 
 if __name__ == '__main__':
-    node.init(OutputNode)
+    node.init(SearchNode)
```

### Comparing `pepid-1.1.0/pepid/pepid_compare.py` & `pepid-1.2.0/pepid/pepid_compare.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/pepid_files.py` & `pepid-1.2.0/pepid/pepid_files.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/pepid_io.py` & `pepid-1.2.0/pepid/pepid_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sqlite3
 
 import struct
 import glob
 import math
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import queries
+    from pepid import blackboard
+    from pepid import queries
 else:
     from . import blackboard
     from . import queries
 
 def write_output(start, end):
     """
     Exports search results to tsv format as per the config settings.
@@ -102,15 +102,15 @@
     blackboard.config.read(sys.argv[1])
 
     cfg_file = sys.argv[1]
 
     blackboard.setup_constants()
 
     if __package__ is None or __package__ == '':
-        import pepid_mp 
+        from pepid import pepid_mp 
     else:
         from . import pepid_mp
 
     log_level = blackboard.config['logging']['level'].lower()
 
     out_fname = blackboard.config['data']['output']
```

### Comparing `pepid-1.1.0/pepid/pepid_mgf_meta.py` & `pepid-1.2.0/pepid/pepid_mgf_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import numpy
 import time
 import pickle
+import msgpack
 import sqlite3
 
 # This is an example script to show how a 'multistaged' pepid operation mode might work.
 # Two config files (example_proteometools_stage1.cfg and example_proteometools_stage2.cfg) are provided.
 # To operate the pipeline, one may do `python -mpepid proteometools_stage1.cfg && /path/to/pepid_mgf_meta.py && python -mpepid proteometools_stage2.cfg`, for example.
 # (after copying, renaming, and fixing the parameters in, the example configs).
 # This operation mode was used to generate some fdp measures for pepid validation with great success.
 
 if __package__ is None or __package__ == '':
-    import blackboard
+    from pepid import blackboard
 else:
     from . import blackboard
 
 def insert_mgf_field(cfg, key):
     blackboard.config.read(blackboard.here("data/default.cfg"))
     blackboard.config.read(cfg)
     blackboard.setup_constants()
@@ -66,19 +67,19 @@
     while True:
         queries = cur.fetchmany(620000)
         if len(queries) == 0:
             break
 
         for query in queries:
             query = dict(query)
-            extra = query['meta'].data
+            extra = pickle.loads(query['meta'])
             if extra is None:
                 extra = {}
             extra['mgf:' + key] = mgf[query['title']]
-            ret.append({'rowid': query['rowid'], 'data': blackboard.Meta(extra)})
+            ret.append({'rowid': query['rowid'], 'data': pickle.dumps(extra)})
 
         update_cur.executemany("UPDATE queries SET meta=:data WHERE rowid=:rowid;", ret)
         conn.commit()
         ret = []
 
 if __name__ == '__main__':
     import sys
```

### Comparing `pepid-1.1.0/pepid/pepid_mp.py` & `pepid-1.2.0/pepid/pepid_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import select
 import os
 import sys
 import time
 import tqdm
 
 if __package__ is None or __package__ == '':
-    import blackboard
+    from pepid import blackboard
 else:
     from . import blackboard
 
 # exit codes:
 # 0: success
 # 1: args incorrect
 # 2: invalid config parameter (fatal)
```

### Comparing `pepid-1.1.0/pepid/pepid_percolator.py` & `pepid-1.2.0/pepid/pepid_percolator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sqlite3
 import os
 import numpy
 import subprocess
 import re
 import math
 import msgpack
+import pepid_utils
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_mp
-    import queries
+    from pepid import blackboard
+    from pepid import pepid_mp
+    from pepid import queries
 else:
     from . import blackboard
     from . import pepid_mp
     from . import queries
 
 import struct
 import math
@@ -56,15 +57,15 @@
     ff = open(f, 'r')
     for il, l in enumerate(ff): pass
     ff.close()
     return il
 
 def rescore(cfg_file):
     if __package__ is None or __package__ == '':
-        import blackboard
+        from pepid import blackboard
     else:
         from . import blackboard
     import sys
 
     use_extra = blackboard.config['rescoring.percolator'].getboolean('use extra')
 
     in_fname = blackboard.config['data']['output']
@@ -75,45 +76,26 @@
     pepout_name = fname + suffix + "_pout_pep.tsv"
     psmout_name = fname + suffix + "_pout_psm.tsv"
     psmdout_name = fname + suffix + "_pout_decoys_psm.tsv"
 
     artifacts = [pin_name, pout_name, pepout_name, psmout_name, psmdout_name]
 
     # Dirty little hack to get the header right before we start multiprocessing
-    fin = open(in_fname, 'r')
-    header = next(fin).strip().split('\t')
-    first = next(fin).strip().split('\t')
-    fin.close()
-
-    conn = sqlite3.connect("file:" + os.path.join(blackboard.TMP_PATH, first[header.index('file')] + "_meta.sqlite") + "?cache=shared", detect_types=1, uri=True) 
-    conn.row_factory = sqlite3.Row
-    cur = conn.cursor()
-    cur.execute("SELECT data, extra FROM meta LIMIT 1;")
-    res = cur.fetchone()
-    first = msgpack.loads(res['data'])
-    if use_extra:
-        second = msgpack.loads(res['extra'])
-        if second is not None:
-            first = {**first, **second}
-    feats = sorted(list(first.keys()))
-    if 'score' in feats:
-        feats.append('deltLCn')
-    feats = [x for x in feats if x not in blackboard.FEATS_BLACKLIST]
-
-    fpin = open(pin_name, 'w')
-    pin_template = blackboard.pin_template()
-    pin_template[pin_template.index("FEATURES")] = "\t".join(feats)
-    fpin.write("\t".join(pin_template) + "\n")
-    fpin.close()
-
-    cur.close()
-    conn.close()
-
     log_level = blackboard.config['logging']['level'].lower()
     if blackboard.config['misc.tsv_to_pin'].getboolean('enabled'):
+        fin = open(in_fname, 'r')
+        header = next(fin).strip().split('\t')
+        first = next(fin).strip().split('\t')
+        fin.close()
+
+        header = pepid_utils.generate_pin_header(header, first)
+        fpin = open(pin_name, 'w')
+        fpin.write("\t".join(header) + "\n")
+        fpin.close()
+
         nworkers = blackboard.config['rescoring.percolator'].getint('pin workers')
         batch_size = blackboard.config['rescoring.percolator'].getint('pin batch size')
         n_total = queries.count_queries()
         n_batches = math.ceil(n_total / batch_size)
         spec = [(blackboard.here("pin_node.py"), nworkers, n_batches,
                         [struct.pack("!cI{}sc".format(len(blackboard.TMP_PATH)), bytes([0x00]), len(blackboard.TMP_PATH), blackboard.TMP_PATH.encode("utf-8"), "$".encode("utf-8")) for _ in range(nworkers)],
                         [struct.pack("!cQQc", bytes([0x01]), b * batch_size, min((b+1) * batch_size, n_total), "$".encode("utf-8")) for b in range(n_batches)],
```

### Comparing `pepid-1.1.0/pepid/pepid_postprocess.py` & `pepid-1.2.0/pepid/pepid_postprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 import os
 import glob
 import math
 import struct
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_mp
+    from pepid import blackboard
+    from pepid import pepid_mp
 else:
     from . import blackboard
     from . import pepid_mp
 
 if __name__ == "__main__":
     cfg_file = sys.argv[1]
```

### Comparing `pepid-1.1.0/pepid/pepid_randomforest.py` & `pepid-1.2.0/pepid/pepid_randomforest.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/pepid_search.py` & `pepid-1.2.0/pepid/pepid_search.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 import sys
 import numpy
 import pickle
 import glob
 
 if __package__ is None:
-    import blackboard
-    import pepid_mp
+    from pepid import blackboard
+    from pepid import pepid_mp
 else:
     from . import blackboard
     from . import pepid_mp
 
 import logging
 import os
 import math
@@ -19,17 +19,17 @@
 
 def run(cfg_file):
     """
     Entry point
     """
 
     if __package__ is None:
-        import queries
-        import db
-        import search
+        from pepid import queries
+        from pepid import db
+        from pepid import search
     else:
         from . import queries
         from . import db
         from . import search
 
     log.info("Search phases to run: | " + ("Query Processing | " if blackboard.config['processing.query'].getboolean('enabled') else "") +
                                 ("DB Processing | " if blackboard.config['processing.db'].getboolean('enabled') else "") +
@@ -180,10 +180,10 @@
     blackboard.TMP_PATH = os.path.join(blackboard.config['data']['tmpdir'], "pepidrun_" + next(tempfile._get_candidate_names()))
     blackboard.setup_constants() # overrides TMP_PATH if workdir setting points to a directory to reuse
     log = blackboard.LOG
 
     if(not os.path.exists(blackboard.TMP_PATH)):
         os.mkdir(blackboard.TMP_PATH)
 
-    blackboard.LOCK = open(os.path.join(blackboard.TMP_PATH, ".lock"), "wb")
+    blackboard.LOCK = blackboard.acquire_lock()
 
     run(cfg_file)
```

### Comparing `pepid-1.1.0/pepid/pepid_utils.py` & `pepid-1.2.0/pepid/pepid_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy
+import importlib
+import sys
 
 AA_TABLE = {
 '_': 999999999.0
 }
 
 MASS_H = 1.007825035
 MASS_O = 15.99491463
@@ -91,20 +93,34 @@
                 raise ValueError("Series '{}' not supported, available series are {}".format(s, list(cterm_generators.keys()) + list(nterm_generators.keys())))
 
             if s in weights and "series" in weights[s]:
                 masses[-1][:,1] *= weights[s]['series']
     return masses
 
 def import_or(s, default):
+    if s.strip() == '':
+        return default
+
+    modstr = s.rsplit('.', 1)
+
+    if len(modstr) == 1:
+        sys.stderr.write("Invalid callable '{}', using default value instead\n".format(s))
+        return default
+
     try:
-        mod, fn = s.rsplit('.', 1)
-        return getattr(__import__(mod, fromlist=[fn]), fn)
-    except:
-        import sys
-        sys.stderr.write("Could not find '{}', using default value instead\n".format(s))
+        return getattr(__import__(modstr[0], locals(), globals(), fromlist=[modstr[1]]), modstr[1])
+    except ModuleNotFoundError:
+        if __package__ is not None and __package__ != '':
+            try:
+                return getattr(__import__(__package__ + "." + modstr[0], locals(), globals(), fromlist=[modstr[1]]), modstr[1])
+            except:
+                sys.stderr.write("Could not find '{}' locally or in Pepid namespace, using default value instead\n".format(s))
+                return default
+
+        sys.stderr.write("Could not find '{}' locally and no package environment available, using default value instead\n".format(s))
         return default
 
 # Requires (matching) scores and labels (is_target) to be sorted by scores in the appropriate direction (i.e. best first, worst last)
 def calc_fdr(scores, is_target):
     fdrs = []
 
     n_targets = 0
@@ -131,21 +147,112 @@
     fdrs = calc_fdr(scores, is_target)
     running = fdrs[-1]
     for i in range(len(fdrs)-1, -1, -1):
         running = min(running, fdrs[i])
         fdrs[i] = running
     return fdrs
 
-def tsv_to_pin(header, lines, start=0):
-    import blackboard
+import numba
+# Do not use numba, it slows down this version by ~50%
+def dense_to_sparse(spec, n_max=500):
+ ret = numpy.zeros((spec.shape[0], n_max, 2), dtype='float32')
+ for i in range(spec.shape[0]):
+  nz = numpy.sort(numpy.argpartition(-spec[i], n_max)[:n_max])
+  if len(nz) > 0:
+   ret[i,:len(nz),:] = numpy.asarray(list(zip(nz, spec[i][nz])), dtype='float32')
+ return ret
+
+@numba.njit()
+def sparse_to_dense(spec, n_max=20000):
+    ret = numpy.zeros((n_max,), dtype='float32')
+    for mz, intens in spec:
+        if mz < n_max:
+            ret[int(mz)] += intens
+        else:
+            break
+    return ret
+
+@numba.njit(locals={'mult': numba.float32, 'size': numba.int32})
+def blit_spectrum(spec, size, mult):
+    spec_raw = numpy.zeros((size,), dtype='float32')
+    for mz, intens in spec:
+        idx = int(numpy.round(mz / mult))
+        if idx >= size:
+            break
+        spec_raw[idx] += intens
+    max = spec_raw.max()
+    if max != 0:
+        spec_raw /= max
+
+    return spec_raw
+
+def generate_pin_header(header, line):
+    if __package__ is None or __package__ == '':
+        from pepid import blackboard
+    else:
+        from . import blackboard
+
+    extra_fn = blackboard.config['misc.tsv_to_pin']['user function'].strip()
+    use_extra = blackboard.config['misc.tsv_to_pin'].getboolean('use extra')
+    extra_fn = import_or(extra_fn, None)
+
+    user_extra = None
+    if extra_fn is not None:
+        user_extra = extra_fn(header, [[line]])[0][0]
+
     import sqlite3
     import os
     import msgpack
+    conn = sqlite3.connect("file:" + os.path.join(blackboard.TMP_PATH, line[header.index('file')] + "_meta.sqlite") + "?cache=shared", detect_types=1, uri=True) 
+    conn.row_factory = sqlite3.Row
+    cur = conn.cursor()
+
+    cur.execute("SELECT rrow, data, extra FROM meta LIMIT 1;")
+    meta = cur.fetchone()
+
+    the_meta = msgpack.loads(meta['data'])
+    parsed_meta = None
+    if the_meta is not None:
+        parsed_meta = {k: v for k, v in the_meta.items() if type(v) != str}
+    if use_extra:
+        extras = msgpack.loads(meta['extra'])
+        if parsed_meta is not None:
+            parsed_meta = {**parsed_meta, **extras}
+        else:
+            parsed_meta = extras
+    if user_extra is not None:
+        if parsed_meta is not None:
+            parsed_meta = {**parsed_meta, **user_extra}
+        else:
+            parsed_meta = user_extra
 
-    feats = None
+    if parsed_meta is None:
+        parsed_meta = {}
+
+    feats = sorted(list(parsed_meta.keys()))
+    if 'score' in feats:
+        feats.append('deltLCn')
+
+    head = ['PSMId', 'Label', 'ScanNr']
+    if 'expMass' in feats and 'calcMass' in feats:
+        head.extend(['expMass', 'calcMass'])
+    head.extend(feats)
+    head.extend(['Peptide', 'Proteins'])
+
+    return head
+
+def tsv_to_pin(header, lines, start=0):
+    if __package__ == '' or __package__ is None:
+        from pepid import blackboard
+    else:
+        from . import blackboard
+
+    import sqlite3
+    import os
+    import msgpack
 
     score_idx = header.index('score')
     file_idx = header.index('file')
     rrow_idx = header.index('rrow')
     qrow_idx = header.index('qrow')
     seq_idx = header.index('modseq')
     title_idx = header.index('title')
@@ -167,27 +274,29 @@
     feats = None
     scores = []
 
     out_lines = []
 
     newlines = []
     for qlines in lines:
+        if len(qlines) == 0:
+            break
         idxs = numpy.argsort([float(line[score_idx]) for line in qlines])[::-1][:max_scores]
         newlines.append([qlines[idx] for idx in idxs])
     lines = newlines
 
     extra_fn = blackboard.config['misc.tsv_to_pin']['user function']
-    if extra_fn != 'None':
+    if extra_fn.strip() != '':
         extra_fn = import_or(extra_fn, None)
     else:
         extra_fn = None
 
     user_extra = None
     if extra_fn is not None:
-        user_extra = extra_fn(lines)
+        user_extra = extra_fn(header, lines)
 
     for il, qlines in enumerate(lines):
         if len(qlines) == 0:
             break
         out_lines.append([])
         if conn is not None:
             cur.close()
@@ -201,15 +310,15 @@
 
         for i, (rrow, m, e) in enumerate(metas):
             parsed_metas.append({k: v for k, v in msgpack.loads(m).items() if type(v) != str})
             if use_extra:
                 extras = msgpack.loads(e)
                 parsed_metas[-1] = {**parsed_metas[-1], **extras}
             if user_extra is not None:
-                parsed_metas[-1] = {**parsed_metas[-1], **user_extra[i]}
+                parsed_metas[-1] = {**parsed_metas[-1], **user_extra[il][i]}
             if feats is None:
                 feats = sorted(list(parsed_metas[-1].keys()))
                 if 'score' in feats:
                     feats.append('deltLCn')
             if 'score' in feats: # XXX: HACK for comet-like deltLCn feature should depend on config...
                 scores.append(parsed_metas[-1]['score'])
 
@@ -218,11 +327,10 @@
                 m['deltLCn'] = (m['score'] - numpy.min(scores)) / (m['score'] if m['score'] != 0 else 1)
 
             extraVals = [0.0, 0.0]
             if 'expMass' in m and 'calcMass' in m:
                 extraVals = [m['expMass'], m['calcMass']]
 
             out_lines[-1].append(list(map(str, [qlines[j][title_idx], (1 - qlines[j][desc_idx].startswith(decoy_prefix)) * 2 - 1, start+il, *extraVals])))
-
             out_lines[-1][-1].extend(list(map(lambda k: numpy.format_float_positional(m[k], trim='0', precision=12), feats))) # percolator breaks if too many digits are provided
             out_lines[-1][-1].extend(["-." + qlines[j][seq_idx] + ".-", qlines[j][desc_idx]])
     return out_lines
```

### Comparing `pepid-1.1.0/pepid/post_node.py` & `pepid-1.2.0/pepid/output_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 import struct
 import os
 import time
+import sys
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import node
-    import pepid_utils
+    from pepid import node
+    from pepid import blackboard
 else:
-    from . import blackboard
     from . import node
-    from . import pepid_utils
+    from . import blackboard
 
-class PostNode(node.Node):
+class OutputNode(node.Node):
     def __init__(self, unix_sock):
         super().__init__(unix_sock)
         self.path = None
+        self.file = None
         self.messages[0x00] = [None, self.prepare]
-        self.messages[0x01] = [None, self.do]
-
-    def do(self, msg):
-        start, end = struct.unpack("!QQ", msg[:16])
+        self.messages[0x01] = ["!QQc", self.do]
 
-        post_fn = pepid_utils.import_or(blackboard.config['postsearch']['function'], None)
+    def do(self, start, end, _):
+        if __package__ is None or __package__ == '':
+            from pepid import pepid_io
+        else:
+            from . import pepid_io
 
         if not self.path:
             raise ValueError("'do' message received before 'prepare' message, aborting.")
 
-        if post_fn is not None:
-            post_fn(start, end)
-            blackboard.CONN.commit()
-        else:
-            blackboard.LOG.warning("Could not find postprocessing function '{}', not applying postprocessing".format(blackboard.config['postsearch']['function']))
-            return
+        pepid_io.write_output(start, end)
 
     def prepare(self, msg):
         lgt = struct.unpack("!I", msg[:4])[0]
-        self.path = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
-        blackboard.TMP_PATH = self.path
+        blackboard.TMP_PATH = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
+        self.path = blackboard.TMP_PATH
         blackboard.setup_constants()
-        blackboard.LOCK = open(os.path.join(blackboard.TMP_PATH, ".lock"), "wb")
+        blackboard.LOCK = blackboard.acquire_lock()
         blackboard.prepare_connection()
 
 if __name__ == '__main__':
-    node.init(PostNode)
+    node.init(OutputNode)
```

### Comparing `pepid-1.1.0/pepid/queries.py` & `pepid-1.2.0/pepid/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy
 from os import path
 import random
 import time
 import random
 import os
+import pickle
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_utils
+    from pepid import blackboard
+    from pepid import pepid_utils
 else:
     from . import blackboard
     from . import pepid_utils
 
 def count_queries():
     """
     Opens the file speficied in config and counts how many spectra are present.
@@ -71,18 +72,18 @@
                 data.append({k:None for k in blackboard.QUERY_COLS})
                 delta_l = tol_l if not is_ppm else pepid_utils.calc_rev_ppm(precmass, tol_l)
                 delta_r = tol_r if not is_ppm else pepid_utils.calc_rev_ppm(precmass, tol_r)
                 data[-1]['title'] = title
                 data[-1]['rt'] = rt
                 data[-1]['charge'] = charge
                 data[-1]['mass'] = precmass
-                data[-1]['spec'] = blackboard.Spectrum(list(zip(mz_arr, intens_arr)))
+                data[-1]['spec'] = pickle.dumps(list(zip(mz_arr, intens_arr)))
                 data[-1]['min_mass'] = precmass + delta_l
                 data[-1]['max_mass'] = precmass + delta_r
-                data[-1]['meta'] = blackboard.Meta(None)
+                data[-1]['meta'] = pickle.dumps(None)
         elif '0' <= l[0] <= '9':
             mz, intens = l.split(maxsplit=1)
             mz_arr.append(float(mz))
             intens_arr.append(float(intens))
     cur = blackboard.CONN.cursor()
     blackboard.executemany(cur, blackboard.insert_dict_str("queries", blackboard.QUERY_COLS), data)
     cur.close()
@@ -99,25 +100,31 @@
     The query object is a database row, which functions similarly to a database and whose
     keys are as defined in `blackboard.py`
 
     The output metadata object should be anything such that eval(expr(metadata)) == metadata, where == is defined
     in the sense of the user scoring function (metadata is not otherwise consulted).
     """
     
-    metadata_fn = pepid_utils.import_or(blackboard.config['processing.query']['postprocessing function'], None)
+    metadata_fn = pepid_utils.import_or(blackboard.config['processing.query']['postprocessing function'].strip(), None)
 
     if metadata_fn is None:
         return
 
     cur = blackboard.CONN.cursor()
-    blackboard.execute(cur, blackboard.select_str("queries", blackboard.QUERY_COLS + ["rowid"], "WHERE rowid BETWEEN ? AND ?"), (start+1, end))
+
+    rows = set()
+    rows.add('rowid')
+    rows.update(getattr(metadata_fn, 'required_fields', {}).get('queries', []))
+
+    blackboard.execute(cur, "SELECT {} FROM queries WHERE rowid BETWEEN ? AND ?;".format(",".join(rows)), (start+1, end))
+
     data = cur.fetchall()
     meta = metadata_fn(data)
     if meta is not None:
-        blackboard.executemany(cur, "UPDATE queries SET meta = ? WHERE rowid = ?;", zip(map(blackboard.Meta, meta), map(lambda x: x['rowid'], data)))
+        blackboard.executemany(cur, "UPDATE queries SET meta = ? WHERE rowid = ?;", zip(map(pickle.dumps, meta), map(lambda x: x['rowid'], data)))
     cur.close()
 
 def prepare_db():
     """
     Creates the required tables in the temporary database for queries processing
     """
```

### Comparing `pepid-1.1.0/pepid/queries_node.py` & `pepid-1.2.0/pepid/queries_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import struct
 import os
 import time
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import node
+    from pepid import blackboard
+    from pepid import node
 else:
     from . import blackboard
     from . import node
 
 class QueryNode(node.Node):
     def __init__(self, unix_sock):
         super().__init__(unix_sock)
         self.path = None
         self.messages[0x00] = [None, self.prepare]
         self.messages[0x01] = ["!QQc", self.do]
         self.messages[0x02] = ["!QQc", self.do_post]
 
     def do(self, start, end, _):
         if __package__ is None or __package__ == '':
-            import queries
+            from pepid import queries
         else:
             from . import queries
 
         if not self.path:
             raise ValueError("'do' message received before 'prepare' message, aborting.")
 
         queries.fill_queries(start, end)
         blackboard.CONN.commit()
 
     def do_post(self, start, end, _):
         if __package__ is None or __package__ == '':
-            import queries
+            from pepid import queries
         else:
             from . import queries
 
         if not self.path:
             raise ValueError("'do_post' message received before 'prepare' message, aborting.")
 
         queries.user_processing(start, end)
         blackboard.CONN.commit()
 
     def prepare(self, msg):
         lgt = struct.unpack("!I", msg[:4])[0]
         self.path = struct.unpack("!{}sc".format(lgt), msg[4:])[0].decode('utf-8')
         blackboard.TMP_PATH = self.path
         blackboard.setup_constants()
-        blackboard.LOCK = open(os.path.join(blackboard.TMP_PATH, ".lock"), "wb")
+        blackboard.LOCK = blackboard.acquire_lock()
         blackboard.prepare_connection()
 
 if __name__ == '__main__':
     node.init(QueryNode)
```

### Comparing `pepid-1.1.0/pepid/search.py` & `pepid-1.2.0/pepid/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,145 +1,129 @@
 import numpy
 import numpy.linalg
 import re
 import numba
 import numba.typed
 import sys
 import msgpack
+import pickle
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_utils
+    from pepid import blackboard
+    from pepid import pepid_utils
 else:
     from . import blackboard
     from . import pepid_utils
 
-def cosine(cands, q):
-    """
-    Simple cosine distance between two spectra.
-    Requires both spectra to be simple (mz, intensity) lists.
-    """
+class hyperscore(object):
+    required_fields = {'candidates': ['spec', 'mass', 'seq', 'mods', 'desc'], 'queries': ['title', 'spec', 'mass', 'charge']}
 
-    blit_q = numpy.zeros((len(cands), 20000)) 
-
-    for i in range(len(cands)):
-        for mz, intens in q[i]['spec'].data:
-            if mz >= 2000-0.5 or mz == 0:
-                break
-            blit_q[i, round(mz * 10)] = intens
-
-    blit_cand = numpy.vstack([numpy.asarray(cands[i]['spec'].data[q[i]['charge']-1].todense()) for i in range(len(cands))])
-    score = ((blit_q * blit_cand) / numpy.maximum(1e-5, (numpy.linalg.norm(blit_q, axis=-1, keepdims=True) * numpy.linalg.norm(blit_cand, axis=-1, keepdims=True)))).sum(axis=-1).reshape((-1,))
-
-    ret = [{'score': score[i], 'theoretical': q[i]['spec'].data, 'spec': cands[i]['spec'].data[q[i]['charge']-1], 'sumI': 0, 'dist': None, 'total_matched': 0, 'title': q[i]['title'], 'desc': cands[i]['desc'], 'seq': cands[i]['seq'], 'modseq': "".join([s if m == 0 else s + "[{}]".format(m) for s,m in zip(cands[i]['seq'], cands[i]['mods'])])} for i in range(len(cands))]
-    return ret
+    def __new__(cls, qcands, qs):
+        """
+        Sample scoring function: rnhs from identipy (with norm type = sum) or hyperscore from x!tandem (with norm type = max).
+        Score output is a dictionary. If the score function will be rescored by percolator,
+        the dictionary keys corresponding to the percolator parameters will be used for that purpose.
+        """
+
+        ret = []
+
+        norm_type = blackboard.config['scoring.hyperscore']['norm type']
+        ignore_weights = blackboard.config['scoring.hyperscore'].getboolean('ignore weights')
+
+        acc_ppm = blackboard.config['scoring.hyperscore']['peak matching unit'] == 'ppm'
+        acc = blackboard.config['scoring.hyperscore'].getfloat('peak matching tolerance')
+
+        cutoff = blackboard.config['scoring.hyperscore'].getfloat('cutoff')
+
+        match_mult = blackboard.config['scoring.hyperscore'].getfloat('match multiplier')
+        disjoint = blackboard.config['scoring.hyperscore'].getboolean('disjoint model')
+        max_best = blackboard.config['scoring.hyperscore'].getint('max best')
+        if max_best <= 0:
+            blackboard.LOG.fatal("Hyperscore: max best must be >= 0, got '{}'".format(max_best))
+            sys.exit(-1)
+        criterion = blackboard.config['scoring.hyperscore']['criterion best']
+        type_best = blackboard.config['scoring.hyperscore']['type best']
+        type_charge = type_best == 'charge'
+        type_series = type_best == 'series'
+        type_both = type_best == 'both'
+        if (type_charge + type_series + type_both) != 1:
+            blackboard.LOG.fatal("Hyperscore: type best must be exactly one of charge, series or both, got '{}'".format(type_best))
+            sys.exit(-1)
+        series_count = blackboard.config['scoring.hyperscore'].getint('series count')
+        match_all = not blackboard.config['scoring.hyperscore'].getboolean('match only closest peak')
 
-def hyperscore(qcands, qs):
-    """
-    Sample scoring function: rnhs from identipy (with norm type = sum) or hyperscore from x!tandem (with norm type = max).
-    Score output is a dictionary. If the score function will be rescored by percolator,
-    the dictionary keys corresponding to the percolator parameters will be used for that purpose.
-    """
+        for q, cands in zip(qs, qcands):
+            ret.append([])
 
-    ret = []
+            spectrum = numpy.asarray(pickle.loads(q['spec']), dtype='float32')
+            mz_array = spectrum[:,0]
+            intens = spectrum[:,1]
+            norm = intens.sum() if norm_type == 'sum' else intens.max()
+            charge = q['charge']
+            qmass = q['mass']
+
+            for i in range(len(cands)):
+                c = cands[i]
+
+                theoretical = pickle.loads(c['spec'])
+                seqs = c['seq']
+                seq_mass = c['mass']
+
+                score = 0
+                total_matched = 0
+                sumI = 0
+
+                theoretical = numpy.asarray(theoretical, dtype='float32')[:int((charge-1) * series_count)]
+
+                sumis, series_matches = hyperscore_score(spectrum, theoretical, norm, acc, acc_ppm, cutoff, match_mult, type_charge, type_series, type_both, series_count, ignore_weights, match_all)
+                sumI = float((sumis * norm).sum())
+
+                # Select only the best N series/charges/match-lists
+                selection = numpy.argsort(series_matches if criterion == 'matches' else sumis)[-max_best:]
+                total_matched = series_matches.sum()
+                series_matches = series_matches[selection]
 
-    norm_type = blackboard.config['scoring.hyperscore']['norm type']
-    ignore_weights = blackboard.config['scoring.hyperscore'].getboolean('ignore weights')
+                if series_matches.sum() == 0:
+                    ret[-1].append({'score': 0})
+                    continue
 
-    acc_ppm = blackboard.config['scoring.hyperscore']['peak matching unit'] == 'ppm'
-    acc = blackboard.config['scoring.hyperscore'].getfloat('peak matching tolerance')
+                mults = numpy.ones(selection.shape, dtype='float32')
+                import sys
+                float_lim = sys.float_info.max
+                for j, matches in enumerate(series_matches):
+                    if matches > 0:
+                        mults[j] = min(numpy.math.factorial(min(20, matches)), float_lim)
+                if not disjoint:
+                    s = sumis.sum()
+                    score = 1
+                    for m in mults:
+                        score *= s * m
+                else:
+                    score = sumis.sum()
+                    for m in mults:
+                        score *= m
+                score = float(min(score, float_lim))
 
-    cutoff = blackboard.config['scoring.hyperscore'].getfloat('cutoff')
-
-    match_mult = blackboard.config['scoring.hyperscore'].getfloat('match multiplier')
-    disjoint = blackboard.config['scoring.hyperscore'].getboolean('disjoint model')
-    max_best = blackboard.config['scoring.hyperscore'].getint('max best')
-    if max_best <= 0:
-        blackboard.LOG.fatal("Hyperscore: max best must be >= 0, got '{}'".format(max_best))
-        sys.exit(-1)
-    criterion = blackboard.config['scoring.hyperscore']['criterion best']
-    type_best = blackboard.config['scoring.hyperscore']['type best']
-    type_charge = type_best == 'charge'
-    type_series = type_best == 'series'
-    type_both = type_best == 'both'
-    if (type_charge + type_series + type_both) != 1:
-        blackboard.LOG.fatal("Hyperscore: type best must be exactly one of charge, series or both, got '{}'".format(type_best))
-        sys.exit(-1)
-    series_count = blackboard.config['scoring.hyperscore'].getint('series count')
-    match_all = not blackboard.config['scoring.hyperscore'].getboolean('match only closest peak')
-
-    for q, cands in zip(qs, qcands):
-        ret.append([])
-
-        spectrum = numpy.asarray(q['spec'].data, dtype='float32')
-        mz_array = spectrum[:,0]
-        intens = spectrum[:,1]
-        norm = intens.sum() if norm_type == 'sum' else intens.max()
-        charge = q['charge']
-        qmass = q['mass']
-
-        for i in range(len(cands)):
-            c = cands[i]
-
-            theoretical = c['spec'].data
-            seqs = c['seq']
-            seq_mass = c['mass']
-
-            score = 0
-            total_matched = 0
-            sumI = 0
-
-            theoretical = numpy.asarray(theoretical, dtype='float32')[:int((charge-1) * series_count)]
-
-            sumis, series_matches = hyperscore_score(spectrum, theoretical, norm, acc, acc_ppm, cutoff, match_mult, type_charge, type_series, type_both, series_count, ignore_weights, match_all)
-            sumI = float((sumis * norm).sum())
-
-            # Select only the best N series/charges/match-lists
-            selection = numpy.argsort(series_matches if criterion == 'matches' else sumis)[-max_best:]
-            total_matched = series_matches.sum()
-            series_matches = series_matches[selection]
+                logsumI = numpy.log10(sumI) # note: x!tandem uses a factor 4 to multiply this by default
 
-            if series_matches.sum() == 0:
-                ret[-1].append({'score': 0})
-                continue
-
-            mults = numpy.ones(selection.shape, dtype='float32')
-            import sys
-            float_lim = sys.float_info.max
-            for j, matches in enumerate(series_matches):
-                if matches > 0:
-                    mults[j] = min(numpy.math.factorial(min(20, matches)), float_lim)
-            if not disjoint:
-                s = sumis.sum()
-                score = 1
-                for m in mults:
-                    score *= s * m
-            else:
-                score = sumis.sum()
-                for m in mults:
-                    score *= m
-            score = float(min(score, float_lim))
-
-            logsumI = numpy.log10(sumI) # note: x!tandem uses a factor 4 to multiply this by default
-
-            ret[-1].append({"dM": float((c['mass'] - q['mass']) / c['mass']),
-                        "absdM": float(abs((c['mass'] - q['mass']) / c['mass'])),
-                        "peplen": len(c['seq']),
-                        "ionFrac": float(total_matched / (theoretical.shape[0] * theoretical.shape[1])),
-                        #'relIntTotMatch': sumI / norm,
-                        'charge': int(q['charge']),
-                        'z2': int(q['charge'] == 2),
-                        'z3': int(q['charge'] == 3),
-                        'z4': int(q['charge'] == 4),
-                        'rawscore': float(score),
-                        #'xcorr': xcorr,
-                        'expMass': float(q['mass']),
-                        'calcMass': float(c['mass']),
-                'score': float(score), 'sumI': float(logsumI), 'total_matched': int(total_matched), 'title': q['title'], 'desc': c['desc'], 'seq': c['seq'], 'modseq': "".join([s if m == 0 else s + "[{}]".format(m) for s, m in zip(c['seq'], c['mods'])])})
-    return ret
+                ret[-1].append({"dM": float((c['mass'] - q['mass']) / c['mass']),
+                            "absdM": float(abs((c['mass'] - q['mass']) / c['mass'])),
+                            "peplen": len(c['seq']),
+                            "ionFrac": float(total_matched / (theoretical.shape[0] * theoretical.shape[1])),
+                            #'relIntTotMatch': sumI / norm,
+                            'charge': int(q['charge']),
+                            'z2': int(q['charge'] == 2),
+                            'z3': int(q['charge'] == 3),
+                            'z4': int(q['charge'] == 4),
+                            'rawscore': float(score),
+                            #'xcorr': xcorr,
+                            'expMass': float(q['mass']),
+                            'calcMass': float(c['mass']),
+                    'score': float(score), 'sumI': float(logsumI), 'total_matched': int(total_matched), 'title': q['title'], 'desc': c['desc'], 'seq': c['seq'], 'modseq': "".join([s if m == 0 else s + "[{}]".format(m) for s, m in zip(c['seq'], msgpack.loads(c['mods']))])})
+        return ret
 
 @numba.njit(locals={'spectrum': numba.float32[:,::1], 'theoretical': numba.float32[:,:,::1], 'acc': numba.float32, 'delta': numba.float32, 'series_count': numba.int32, 'norm': numba.float32, 'spec_idx': numba.int32})
 def hyperscore_score(spectrum, theoretical, norm, acc=10, acc_ppm=True, cutoff=0.01, match_mult=100.0, type_charge=False, type_series=False, type_both=True, series_count=2, ignore_weights=False, match_all=False):
     mz_array = spectrum[:,0]
     intens = spectrum[:,1]
 
     series_matches = numpy.zeros((((len(theoretical) // series_count) if type_charge else series_count if type_series else len(theoretical)),), dtype='int32')
@@ -189,115 +173,118 @@
                         sumis[idx] += val
                         series_matches[idx] += 1
                 elif delta < 0: # anything else will be increasingly further away, bail
                     break
 
     return sumis, series_matches
 
-def xcorr(qcands, qs):
-    """
-    Sample scoring function: Xcorr
-    """
+class xcorr(object):
+    required_fields = {'candidates': ['spec', 'mass', 'seq', 'mods', 'desc'], 'queries': ['title', 'spec', 'mass', 'charge']}
 
-    bin_ppm = blackboard.config['scoring.xcorr']['bin matching unit'] == 'ppm'
-    ppm_mode = blackboard.config['scoring.xcorr']['ppm mode']
-    window_size = blackboard.config['scoring.xcorr'].getint('correlation window size')
-    norm_windows = blackboard.config['scoring.xcorr'].getint('norm window count')
-    bin_resolution_setting = blackboard.config['scoring.xcorr'].getfloat('bin resolution')
-    max_mass = blackboard.config['processing.query'].getfloat('max mass')
-    min_resolution = max(0, blackboard.config['scoring.xcorr'].getfloat('min bin width'))
-    series_count = blackboard.config['scoring.xcorr'].getint('series count')
-    ignore_weights = blackboard.config['scoring.xcorr'].getboolean('ignore weights')
-
-    if bin_ppm and ppm_mode == 'bins':
-        if min_resolution == 0:
-            blackboard.LOG.fatal("Xcorr in ppm bins mode must have a non-zero min bin width, got {} (i.e. 0)".format(blackboard.config['scoring.xcorr']['min bin width']))
+    def __new__(cls, qcands, qs):
+        """
+        Sample scoring function: Xcorr
+        """
+
+        bin_ppm = blackboard.config['scoring.xcorr']['bin matching unit'] == 'ppm'
+        ppm_mode = blackboard.config['scoring.xcorr']['ppm mode']
+        window_size = blackboard.config['scoring.xcorr'].getint('correlation window size')
+        norm_windows = blackboard.config['scoring.xcorr'].getint('norm window count')
+        bin_resolution_setting = blackboard.config['scoring.xcorr'].getfloat('bin resolution')
+        max_mass = blackboard.config['processing.query'].getfloat('max mass')
+        min_resolution = max(0, blackboard.config['scoring.xcorr'].getfloat('min bin width'))
+        series_count = blackboard.config['scoring.xcorr'].getint('series count')
+        ignore_weights = blackboard.config['scoring.xcorr'].getboolean('ignore weights')
+
+        if bin_ppm and ppm_mode == 'bins':
+            if min_resolution == 0:
+                blackboard.LOG.fatal("Xcorr in ppm bins mode must have a non-zero min bin width, got {} (i.e. 0)".format(blackboard.config['scoring.xcorr']['min bin width']))
+                sys.exit(-1)
+
+        flank_mode = blackboard.config['scoring.xcorr']['flank mode']
+        flank_length = blackboard.config['scoring.xcorr'].getint('flank length')
+        if flank_length < 0:
+            blackboard.LOG.fatal("Xcorr flank length must be positive, got {}".format(blackboard.config['scoring.xcorr']['flank length']))
             sys.exit(-1)
+        intensity_cutoff = blackboard.config['scoring.xcorr'].getfloat('intensity cutoff')
+        match_mult = blackboard.config['scoring.xcorr'].getfloat('match multiplier')
 
-    flank_mode = blackboard.config['scoring.xcorr']['flank mode']
-    flank_length = blackboard.config['scoring.xcorr'].getint('flank length')
-    if flank_length < 0:
-        blackboard.LOG.fatal("Xcorr flank length must be positive, got {}".format(blackboard.config['scoring.xcorr']['flank length']))
-        sys.exit(-1)
-    intensity_cutoff = blackboard.config['scoring.xcorr'].getfloat('intensity cutoff')
-    match_mult = blackboard.config['scoring.xcorr'].getfloat('match multiplier')
-
-    bins = []
-    if bin_ppm and ppm_mode != 'bins':
-        curr_mass = max_mass
-        gap = curr_mass
-        while curr_mass > 0:
-            bins.append(curr_mass)
-            gap = max((bin_resolution_setting * 1e-6) * curr_mass, min_resolution)
-            curr_mass -= gap
-        bins.append(0)
-        bins = bins[::-1][:-1]
-    bins = numpy.asarray(bins, dtype='float32')
-
-    ret = []
-
-    bin_resolution = bin_resolution_setting
-    for q, cands in zip(qs, qcands):
-        ret.append([])
-
-        charge = q['charge']
-        spectrum = numpy.asarray(q['spec'].data, dtype='float32')
-        mass = q['mass']
-
-        if bin_ppm and ppm_mode == 'mass':
-            bin_resolution = max(mass * 1e-6 * bin_resolution_setting, min_resolution)
-        elif bin_ppm and ppm_mode == 'max':
-            bin_resolution = max(spectrum[:,0].max() * 1e-6 * bin_resolution_setting, min_resolution)
-
-        filtered_spectrum = spectrum[spectrum[:,0] < mass + 50]
-
-        binned = xcorr_normalize_spec(spectrum, mass, window_size, bin_resolution, norm_windows, bin_ppm and ppm_mode == 'bins', bins, intensity_cutoff, match_mult)
-        corrected = xcorr_correct_spec(binned, window_size, flank_mode, flank_length)
-        if corrected is None:
-            blackboard.LOG.fatal("Unrecognized flank mode '{}', aborting.".format(flank_mode))
-            sys.exit(-2)
-
-        for i in range(len(cands)):
-            c = cands[i]
-            frag = numpy.asarray(c['spec'].data, dtype='float32')
-            # index 0 is charge 1, so charge-1 must be used
-            frag = numpy.ascontiguousarray(frag[:(charge-1)*2])
-
-            n_matches = 0
-            score = 0
-            n_series = 0
-            sumI = 0
-            total_lgt = 0
-
-            score, sumis, series_matches = xcorr_score(frag, corrected, binned, bin_resolution, bin_ppm and ppm_mode == 'bins', bins, ignore_weights)
-            sumI = sumis.sum()
-            n_matches = series_matches.sum()
+        bins = []
+        if bin_ppm and ppm_mode != 'bins':
+            curr_mass = max_mass
+            gap = curr_mass
+            while curr_mass > 0:
+                bins.append(curr_mass)
+                gap = max((bin_resolution_setting * 1e-6) * curr_mass, min_resolution)
+                curr_mass -= gap
+            bins.append(0)
+            bins = bins[::-1][:-1]
+        bins = numpy.asarray(bins, dtype='float32')
+
+        ret = []
+
+        bin_resolution = bin_resolution_setting
+        for q, cands in zip(qs, qcands):
+            ret.append([])
+
+            charge = q['charge']
+            spectrum = numpy.asarray(pickle.loads(q['spec']), dtype='float32')
+            mass = q['mass']
+
+            if bin_ppm and ppm_mode == 'mass':
+                bin_resolution = max(mass * 1e-6 * bin_resolution_setting, min_resolution)
+            elif bin_ppm and ppm_mode == 'max':
+                bin_resolution = max(spectrum[:,0].max() * 1e-6 * bin_resolution_setting, min_resolution)
+
+            filtered_spectrum = spectrum[spectrum[:,0] < mass + 50]
+
+            binned = xcorr_normalize_spec(spectrum, mass, window_size, bin_resolution, norm_windows, bin_ppm and ppm_mode == 'bins', bins, intensity_cutoff, match_mult)
+            corrected = xcorr_correct_spec(binned, window_size, flank_mode, flank_length)
+            if corrected is None:
+                blackboard.LOG.fatal("Unrecognized flank mode '{}', aborting.".format(flank_mode))
+                sys.exit(-2)
+
+            for i in range(len(cands)):
+                c = cands[i]
+                frag = numpy.asarray(pickle.loads(c['spec']), dtype='float32')
+                # index 0 is charge 1, so charge-1 must be used
+                frag = numpy.ascontiguousarray(frag[:(charge-1)*2])
+
+                n_matches = 0
+                score = 0
+                n_series = 0
+                sumI = 0
+                total_lgt = 0
+
+                score, sumis, series_matches = xcorr_score(frag, corrected, binned, bin_resolution, bin_ppm and ppm_mode == 'bins', bins, ignore_weights)
+                sumI = sumis.sum()
+                n_matches = series_matches.sum()
 
-            n_series = frag.shape[0] // series_count
-            total_lgt = frag.shape[1] * frag.shape[0]
+                n_series = frag.shape[0] // series_count
+                total_lgt = frag.shape[1] * frag.shape[0]
 
-            if score <= 0:
-                ret[-1].append({'score': 0})
-                continue
-            else:
-                ret[-1].append({"dM": float((c['mass'] - q['mass']) / c['mass']),
-                            "absdM": abs((c['mass'] - q['mass']) / c['mass']),
-                            "peplen": len(c['seq']),
-                            "ionFrac": float(n_matches / total_lgt),
-                            #'relIntTotMatch': sumI / norm,
-                            'charge': int(q['charge']),
-                            'z2': int(q['charge'] == 2),
-                            'z3': int(q['charge'] == 3),
-                            'z4': int(q['charge'] == 4),
-                            'rawscore': float(score),
-                            #'xcorr': xcorr,
-                            'expMass': float(q['mass']),
-                            'calcMass': float(c['mass']),
-                            'score': float(score), 'sumI': float(sumI), 'total_matched': int(n_matches), 'title': q['title'], 'desc': c['desc'], 'seq': c['seq'], 'modseq': "".join([s if m == 0 else s + "[{}]".format(m) for s, m in zip(c['seq'], c['mods'])])})
-    return ret
+                if score <= 0:
+                    ret[-1].append({'score': 0})
+                    continue
+                else:
+                    ret[-1].append({"dM": float((c['mass'] - q['mass']) / c['mass']),
+                                "absdM": abs((c['mass'] - q['mass']) / c['mass']),
+                                "peplen": len(c['seq']),
+                                "ionFrac": float(n_matches / total_lgt),
+                                #'relIntTotMatch': sumI / norm,
+                                'charge': int(q['charge']),
+                                'z2': int(q['charge'] == 2),
+                                'z3': int(q['charge'] == 3),
+                                'z4': int(q['charge'] == 4),
+                                'rawscore': float(score),
+                                #'xcorr': xcorr,
+                                'expMass': float(q['mass']),
+                                'calcMass': float(c['mass']),
+                                'score': float(score), 'sumI': float(sumI), 'total_matched': int(n_matches), 'title': q['title'], 'desc': c['desc'], 'seq': c['seq'], 'modseq': "".join([s if m == 0 else s + "[{}]".format(m) for s, m in zip(c['seq'], msgpack.loads(c['mods']))])})
+        return ret
 
 @numba.njit(locals={'scale': numba.int32, 'i': numba.int32, 'bins': numba.float32[::1]})
 def get_bin_index(mass, bins):
     if len(bins) == 0:
         return len(bins)
     if mass < bins[0]:
         return len(bins)
@@ -409,28 +396,31 @@
             ret += corrected[idx] * (weight if not ignore_weights else 1)
             if normed[idx] > 1e-10 or normed[idx] < -1e-10:
                 sumis[i] += normed[idx]
                 nmatches[i] += 1
             seen.add(idx)
     return ret, sumis, nmatches
 
-def xcorr_hyperscore(qcands, qs):
-    """
-    Sample scoring function: Xcorr
-    """
-
-    ret_xcorr = xcorr(qcands, qs)
-    ret_hscore = hyperscore(qcands, qs)
+class xcorr_hyperscore(object):
+    required_fields = {'candidates': ['spec', 'mass', 'seq', 'mods', 'desc'], 'queries': ['title', 'spec', 'mass', 'charge']}
 
-    ret = [[{**rh, **rx, 'xcorr': rx['score'], 'hyperscore': rh['score']} for rx, rh in zip(retx, reth)] for retx, reth in zip(ret_xcorr, ret_hscore)]
-    for re in ret:
-        for r in re:
-            r['score'] = float(max(0, r['xcorr'], numpy.sqrt(numpy.log10(r['hyperscore'] + 1)), r['xcorr'] * numpy.sqrt(numpy.log10(r['hyperscore'] + 1))))
+    def __new__(cls, qcands, qs):
+        """
+        Sample scoring function: Xcorr
+        """
+
+        ret_xcorr = xcorr(qcands, qs)
+        ret_hscore = hyperscore(qcands, qs)
+
+        ret = [[{**rh, **rx, 'xcorr': rx['score'], 'hyperscore': rh['score']} for rx, rh in zip(retx, reth)] for retx, reth in zip(ret_xcorr, ret_hscore)]
+        for re in ret:
+            for r in re:
+                r['score'] = float(max(0, r['xcorr'], numpy.sqrt(numpy.log10(r['hyperscore'] + 1)), r['xcorr'] * numpy.sqrt(numpy.log10(r['hyperscore'] + 1))))
 
-    return ret
+        return ret
 
 def stub_filter(cands, q):
     return cands
 
 def search_core(start, end):
     """
     Core search algorithm: collects and finalizes the data, then
@@ -443,21 +433,28 @@
 
     blackboard.init_results_db(generate=True, base_dir=blackboard.TMP_PATH)
     shard_level = blackboard.config['scoring'].getint('sharding threshold')
 
     scoring_fn = pepid_utils.import_or(blackboard.config['scoring']['function'], xcorr)
     select_fn = pepid_utils.import_or(blackboard.config['scoring']['candidate filtering function'], stub_filter)
 
+    rows = set()
+    rows.add('rowid')
+    rows.add('min_mass')
+    rows.add('max_mass')
+    rows.update(getattr(scoring_fn, 'required_fields', {}).get('queries', []))
+    rows.update(getattr(select_fn, 'required_fields', {}).get('queries', []))
+
     batch_size = blackboard.config['scoring'].getint('batch size')
 
     cur = blackboard.CONN.cursor()
     res_cur = blackboard.RES_CONN.cursor()
     m_cur = blackboard.META_CONN.cursor()
 
-    blackboard.execute(cur, blackboard.select_str("queries", ["rowid"] + blackboard.QUERY_COLS, "WHERE rowid BETWEEN ? AND ?"), (start+1, end))
+    blackboard.execute(cur, "SELECT {} FROM queries WHERE rowid BETWEEN ? AND ?;".format(",".join(rows)), (start+1, end))
     queries = cur.fetchall()
 
     rrow = 1
 
     fname_prefix = blackboard.RES_DB_FNAME.rsplit(".", 1)[0]
 
     n_cands = 0
@@ -498,18 +495,24 @@
                 blackboard.META_CONN.close()
                 blackboard.init_results_db(generate=True, base_dir=blackboard.TMP_PATH)
                 res_cur = blackboard.RES_CONN.cursor()
                 m_cur = blackboard.META_CONN.cursor()
                 fname_prefix = blackboard.RES_DB_FNAME.rsplit(".", 1)[0]
         return rrow
 
+    rows = set()
+    rows.add('rowid')
+    rows.update(getattr(scoring_fn, 'required_fields', {}).get('candidates', []))
+    rows.update(getattr(select_fn, 'required_fields', {}).get('candidates', []))
+
     for iq, q in enumerate(queries):
         quers.append(q)
         cands.append([])
-        blackboard.execute(cur, blackboard.select_str("candidates", ["rowid"] + blackboard.DB_COLS, "WHERE mass BETWEEN ? AND ?"), (q['min_mass'], q['max_mass']))
+
+        blackboard.execute(cur, "SELECT {} FROM candidates WHERE mass BETWEEN ? AND ?;".format(",".join(rows)), (q['min_mass'], q['max_mass']))
         
         while True:
             raw_set = cur.fetchmany(batch_size)
             if len(raw_set) == 0:
                 break
             cand_set = select_fn([dict(o) for o in raw_set], q)
             if len(cand_set) == 0:
```

### Comparing `pepid-1.1.0/pepid/test_model.py` & `pepid-1.2.0/pepid/test_model.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/pepid/train_rf_rescorer.py` & `pepid-1.2.0/pepid/ml/train_rf_rescorer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,170 @@
 import sys
 import numpy
 import math
 import pickle
 import msgpack
 import tqdm
+import os
+import sqlite3
+import struct
 
 if __package__ is None or __package__ == '':
-    import blackboard
-    import pepid_utils
-    import queries
+    from pepid import blackboard
+    from pepid import pepid_utils
+    from pepid import queries
+    from pepid import pepid_mp
 else:
-    from . import blackboard
-    from . import pepid_utils
-    from . import queries
+    from .. import blackboard
+    from .. import pepid_utils
+    from .. import queries
+    from .. import pepid_mp
 
-def run():
+def run(cfg_file):
     log_level = blackboard.config['logging']['level'].lower()
     if blackboard.config['misc.tsv_to_pin'].getboolean('enabled'):
+        in_fname = blackboard.config['data']['output']
+        fname, fext = in_fname.rsplit('.', 1)
+        suffix = blackboard.config['rescoring']['suffix']
+        pin_name = fname + suffix + "_pin.tsv"
+
+        fin = open(in_fname, 'r')
+        header = next(fin).strip().split('\t')
+        first = next(fin).strip().split('\t')
+        fin.close()
+
+        header = pepid_utils.generate_pin_header(header, first)
+        fpin = open(pin_name, 'w')
+        fpin.write("\t".join(header) + "\n")
+        fpin.close()
+ 
         nworkers = blackboard.config['rescoring.finetune_rf'].getint('pin workers')
         batch_size = blackboard.config['rescoring.finetune_rf'].getint('pin batch size')
         n_total = queries.count_queries()
         n_batches = math.ceil(n_total / batch_size)
         spec = [(blackboard.here("pin_node.py"), nworkers, n_batches,
                         [struct.pack("!cI{}sc".format(len(blackboard.TMP_PATH)), bytes([0x00]), len(blackboard.TMP_PATH), blackboard.TMP_PATH.encode("utf-8"), "$".encode("utf-8")) for _ in range(nworkers)],
                         [struct.pack("!cQQc", bytes([0x01]), b * batch_size, min((b+1) * batch_size, n_total), "$".encode("utf-8")) for b in range(n_batches)],
                         [struct.pack("!cc", bytes([0x7f]), "$".encode("utf-8")) for _ in range(nworkers)])]
 
         pepid_mp.handle_nodes("PIN Generation", spec, cfg_file=cfg_file, tqdm_silence=log_level in ['fatal', 'error', 'warning'])
 
     in_fname = blackboard.config['data']['output']
     fname, fext = in_fname.rsplit('.', 1)
+    suffix = blackboard.config['rescoring']['suffix']
     pin_fname = fname + suffix + "_pin.tsv"
 
     f = open(pin_fname)
+    pin_header = next(f).strip().split('\t')
     
     import glob
 
     data = []
 
-    import sqlite3
-    conn = sqlite3.connect("/scratch/zumerj/tmp/pepidrun_massive/human_q.sqlite", detect_types=1)
+    conn = sqlite3.connect(blackboard.DB_PATH + "_q.sqlite", detect_types=1)
     conn.row_factory = sqlite3.Row
     cur = conn.cursor()
 
+    forbidden_feats = set(['PSMId', 'Proteins', 'Peptide', 'ScanNr', 'Label'])
+    length_feats = set(['LgtDelta', 'LgtDeltaAbs', 'LgtPred', 'LgtProb', 'LgtProbDeltaBest', 'LgtProbDeltaNext', 'LgtProbDeltaPrev', 'LgtProbDeltaWorst', 'LgtRelProb', 'LgtRelScore', 'LgtScore'])
+    specgen_feats = set(['MLCorr'])
+
+    # XXX: To disable length and/or specgen feats to generate the partial rescorers:
+    forbidden_feats |= length_feats
+    forbidden_feats |= specgen_feats
+
+    the_feats = [f for f in pin_header if f not in forbidden_feats]
+    the_feats = numpy.unique(the_feats).tolist()
+
     staged = []
     prev_title = None
-    for li, l in tqdm.tqdm(enumerate(f), desc="reading from pin...", tqdm_silence=(log_level in ['fatal', 'error', 'warning'])):
+    for li, l in tqdm.tqdm(enumerate(f), desc="reading from pin...", disable=(log_level in ['fatal', 'error', 'warning'])):
         fields = l.strip().split("\t")
-        score = float(fields[header.index('score')])
-        title = fields[header.index('PSMId')]
+        score = float(fields[pin_header.index('score')])
+        title = fields[pin_header.index('PSMId')]
         if title != prev_title:
             prev_title = title
             if len(staged) > 0:
                 data.extend(staged)
                 del staged
                 staged = []
         if not math.isinf(score):
-            staged.append((title, fields[header.index("Peptide")][2:-2], score, *[float(fields[header.index(f)]) for f in feats], float(fields[header.index('Label')]), -1))
+            staged.append((title, fields[pin_header.index("Peptide")][2:-2], score, *[float(fields[pin_header.index(f)]) for f in the_feats], float(fields[pin_header.index('Label')]), -1))
 
     data.extend(staged)
     del staged
 
-    data = numpy.asarray(data, dtype=[('title', object), ('seq', object), ('s', 'float32'), *[(feat, 'float32') for feat in feats], ('target', 'float32'), ('gt', 'float32')])
+    data = numpy.asarray(data, dtype=[('title', object), ('seq', object), ('s', 'float32'), *[(feat, 'float32') for feat in the_feats], ('target', 'float32'), ('gt', 'float32')])
 
     bs = 100000
     meta = {}
-    for i in tqdm.tqdm(range(0, len(data), bs), desc='collecting metadata', total = numpy.ceil(len(data) / bs)):
+    for i in tqdm.tqdm(range(0, len(data), bs), desc='collecting metadata', total = numpy.ceil(len(data) / bs), disable=(log_level in ['warning', 'error', 'fatal'])):
         cur.execute("SELECT title, meta FROM queries WHERE title IN ({});".format(",".join(["\"{}\"".format(t) for t in data['title'][i:i+bs]])))
         things = cur.fetchall()
-        meta = meta | {m['title'] : msgpack.loads(m['meta'])['mgf:SEQ'] for m in things}
+        meta = meta | {m['title'] : pickle.loads(m['meta'])['mgf:SEQ'] for m in things}
 
-    for di in tqdm.tqdm(range(len(data)), desc='adding gt info', total = len(data)):
+    for di in tqdm.tqdm(range(len(data)), desc='adding gt info', total = len(data), disable=(log_level in ['warning', 'error', 'fatal'])):
         seq = meta[data[di]['title']]
         data[di]['gt'] = ((seq.replace("M(ox)", "M[15.994915]").replace("C", "C[57.0215]") == data[di]['seq']) - 0.5)*2
 
     cur.close()
     conn.close()
 
     numpy.random.shuffle(data)
     every = data
 
     names = every.dtype.names
-    feats = header.split("\t")
-    feats_template = blackboard.pin_template()
-    for f in feats_template:
-        try:
-            del feats[feats.index(f)]
-        except:
-            continue
-    feat_idxs = [names.index(feat) for feat in feats]
+    feat_idxs = [names.index(feat) for feat in the_feats]
 
     import sklearn
     from sklearn import preprocessing
     from sklearn import ensemble
     from sklearn import model_selection
 
     blackboard.LOG.info("Fitting...")
 
     best_dir = True # i.e. bigger = better
     best_feat = 's'
     best_score = 0
 
-    for feat in feats + ['s']:
-        for direction in [False, True]:
-            every.sort(order=[feat, 'target'])
-            if direction:
-                every = every[::-1]
-
-            fdrs = numpy.asarray(pepid_utils.calc_qval(every[feat], every['target'] > 0))
-            aw = numpy.argwhere(fdrs <= 0.01)
-            min_s = every[feat][(aw.reshape((-1,))[-1])+1] if len(aw) > 0 else (every[feat].max()+1) if direction else (every[feat].min()-1)
-
-            score = (every[feat] > min_s).sum() if direction else (every[feat] < min_s).sum()
-            if score > best_score:
-                best_dir = direction
-                best_feat = feat
-
-            blackboard.LOG.debug("[{}|{}] Identified past 1% FDR:".format(feat, "+" if direction else "-"), score)
+    n_jobs = blackboard.config['rescoring.finetune_rf']['workers'].strip()
+    if n_jobs == '':
+        n_jobs = -1
+    else:
+        n_jobs = blackboard.config['rescoring.finetune_rf'].getint('workers')
+
+    feat_ipt = blackboard.config['rescoring.finetune_rf']['score']
+    if feat_ipt == '':
+        feat_ipt = None
+    feat_dir = blackboard.config['rescoring.finetune_rf']['descending'].strip()
+    if feat_dir == '':
+        feat_dir = None
+    else:
+        feat_dir = blackboard.config['rescoring.finetune_rf'].getboolean('descending')
+
+    if feat_ipt is None:
+        for feat in the_feats + ['s']:
+            for direction in [False, True]:
+                every.sort(order=[feat, 'target'])
+                if direction:
+                    every = every[::-1]
+
+                fdrs = numpy.asarray(pepid_utils.calc_qval(every[feat], every['target'] > 0))
+                aw = numpy.argwhere(fdrs <= 0.01)
+                min_s = every[feat][(aw.reshape((-1,))[-1])+1] if len(aw) > 0 else (every[feat].max()+1) if direction else (every[feat].min()-1)
+
+                score = (every[feat] > min_s).sum() if direction else (every[feat] < min_s).sum()
+                if score > best_score:
+                    best_dir = direction
+                    best_feat = feat
+
+                blackboard.LOG.debug("[{}|{}] Identified past 1% FDR: {}".format(feat, "+" if direction else "-", score))
+    else:
+        best_feat = feat_ipt
+        best_dir = feat_dir
 
     feat = best_feat
     direction = best_dir
 
     if not direction:
         every[feat] = -every[feat]
 
@@ -147,17 +191,17 @@
     min_st = data[feat][aw.reshape((-1,))[-1]+1] if len(aw) > 0 else data[feat].max()+1
 
     fdrs = numpy.asarray(pepid_utils.calc_qval(data[feat], data['gt'] > 0))
     aw = numpy.argwhere(fdrs <= 0.01)
     min_sgt = data[feat][aw.reshape((-1,))[-1]+1] if len(aw) > 0 else data[feat].max()+1
 
     blackboard.LOG.info("Total: {}".format(len(every)))
-    blackboard.LOG.info("[{}] Identified past 1% FDR:".format(feat), (every[feat] > min_s).sum())
-    blackboard.LOG.info("Top-1: [{}] Identified past 1% FDR:".format(feat), (data[feat] > min_st).sum())
-    blackboard.LOG.info("Top-1: [{}] Identified past 1% FDP:".format(feat), (data[feat] > min_sgt).sum())
+    blackboard.LOG.info("[{}] Identified past 1% FDR: {}".format(feat, (every[feat] > min_s).sum()))
+    blackboard.LOG.info("Top-1: [{}] Identified past 1% FDR: {}".format(feat, (data[feat] > min_st).sum()))
+    blackboard.LOG.info("Top-1: [{}] Identified past 1% FDP: {}".format(feat, (data[feat] > min_sgt).sum()))
 
     fdrs = numpy.asarray(pepid_utils.calc_qval(every[feat], every['target'] > 0))
     aw = numpy.argwhere(fdrs <= 0.01)
     min_s = every[feat][aw.reshape((-1,))[-1]+1] if len(aw) > 0 else every[feat].max()+1
 
     every_groups = []
     prev_title = None
@@ -165,15 +209,15 @@
     for title in every['title']:
         if prev_title != title:
             prev_title = title
             idx += 1
         every_groups.append(idx) 
 
     is_index = numpy.asarray([(t['target'] < -0.5 or (t[feat] > min_s)) for t in every])
-    every_feats = numpy.asarray([t[feats] for t in every]).view('float32').reshape((-1, len(feats)))
+    every_feats = numpy.asarray([t[the_feats] for t in every]).view('float32').reshape((-1, len(the_feats)))
     every_labs = numpy.asarray([1 if t['target'] > 0.5 else -1 for t in every])
 
     n_folds = 10
     fold = model_selection.GroupKFold(n_splits=n_folds)
 
     best_model = None
     best_idx = -1
@@ -181,65 +225,49 @@
     for i, (train_idxs, test_idxs) in enumerate(fold.split(every, groups=every_groups)):
         blackboard.LOG.debug("Fold {}: Init data".format(i+1))
 
         train_feats = every_feats[train_idxs][is_index[train_idxs]]
         train_labs = every_labs[train_idxs][is_index[train_idxs]]
 
         blackboard.LOG.debug("Fold {}: Train".format(i+1))
-        rf = ensemble.RandomForestClassifier(n_jobs=-1)
+        rf = ensemble.RandomForestClassifier(n_jobs=n_jobs)
         scaler = preprocessing.StandardScaler()
         scaler.fit(train_feats)
 
-        rf.fit(scaler.transform(every_feats[train_idxs]), [1 if t['gt'] > 0.5 else 0 for t in every[train_idxs]])
+        labs = numpy.asarray([1 if t['gt'] > 0.5 else 0 for t in every[train_idxs]])
+        assert ((1 in labs) and (0 in labs))
+        rf.fit(scaler.transform(every_feats[train_idxs]), labs)
 
         blackboard.LOG.debug("Fold {}: Test".format(i+1))
         test_feats = every_feats[test_idxs]
-        test_out = numpy.asarray(rf.predict_proba(scaler.transform(test_feats))[:,1])
+        preds = rf.predict_proba(scaler.transform(test_feats))
+        test_out = numpy.asarray(preds[:,1])
 
         fdrs = numpy.asarray(pepid_utils.calc_qval(test_out, every[test_idxs]['gt'] > 0.5))
         aw = numpy.argwhere(fdrs <= 0.01)
-        min_idx = aw.reshape((-1,))[-1]
+        min_idx = aw.reshape((-1,))
+        if len(min_idx) > 0:
+            min_idx = min_idx[-1]
+        else:
+            min_idx = -1
 
         if min_idx > best_idx:
             best_model = rf
 
         blackboard.LOG.debug("Fold {}: Done".format(i+1))
 
     blackboard.LOG.debug("Done")
 
-    keys = numpy.unique(every['title'])
-    grouped_data = {k: [] for k in keys}
-    data = []
-    for i in range(len(every)):
-        grouped_data[every[i]['title']].append((out_transformed[i], every[i]['title'], every[i]['seq'], every[i]['target'], every[i]['gt']))
-    for g in grouped_data:
-        data.append(grouped_data[g][numpy.argmax([gg[0] for gg in grouped_data[g]])])
-    data = numpy.asarray(data, dtype=[('s', numpy.float32), ('title', object), ('seq', object), ('target', numpy.int32), ('gt', numpy.int32)])
-    data.sort(order=['s', 'target'])
-    data = data[::-1]
-
-    fdrs = numpy.asarray(pepid_utils.calc_qval(data['s'], data['target'] > 0))
-    aw = numpy.argwhere(fdrs <= 0.01)
-    min_st = data['s'][min(len(data)-1, aw.reshape((-1,))[-1]+1)] if len(aw) > 0 else data['s'].max()+1
-    blackboard.LOG.debug("FDRS/target:", fdrs[0], fdrs[-1])
-
-    fdrs = numpy.asarray(pepid_utils.calc_qval(data['s'], data['gt'] > 0))
-    aw = numpy.argwhere(fdrs <= 0.01)
-    min_sgt = data['s'][min(len(data)-1, aw.reshape((-1,))[-1]+1)] if len(aw) > 0 else data['s'].max()+1
-
-    blackboard.LOG.info("Identified past 1% FDR:", (data['s'] > min_st).sum())
-    blackboard.LOG.info("Identified past 1% FDP:", (data['s'] > min_sgt).sum())
-
-    pickle.dump(best_model, open(blackboard.here("ml/rescorer_rf.pkl"), "wb"))
-    pickle.dump(scaler, open(blackboard.here("ml/rescorer_preproc.pkl"), "wb"))
+    # we save the feats in order so we can correctly reorder feats and check if they're really present at load time... while the rescorer is very specific, this should give slightly more flexibility.
+    pickle.dump({'model': best_model, 'scaler': scaler, 'feats': the_feats}, open(blackboard.here("ml/rescorer_rf.pkl"), "wb"))
 
 if __name__ == '__main__':
     if len(sys.argv) != 2:
         blackboard.LOG.error("USAGE: {} config.cfg\n".format(sys.argv[0]))
         sys.exit(-1)
 
     blackboard.config.read(blackboard.here("data/default.cfg"))
     blackboard.config.read(sys.argv[1])
 
     blackboard.setup_constants()
 
-    run()
+    run(sys.argv[1])
```

### Comparing `pepid-1.1.0/pepid/data/default.cfg` & `pepid-1.2.0/pepid/data/default.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # Basic workflow:
 # - simultaneous processing (db, query)
 # - simultaneous postprocessing (db, query)
 # - search
-# - postsearch
-# - output (tsv, then report, then rescoring, then final report)
-
 # Format for functions is: importable.module:function_name
 # See below for examples
 
 [performance]
 python = python # path to python/pypy/etc. executable
 extra args =
 
@@ -22,30 +19,34 @@
 workdir = false # this should be the path to the generated work files' directory if using, else 'false'
 tmpdir = /tmp/ # where to put temporary files
 
 [processing.query]
 enabled = true
 workers = 32
 postprocessing function = extensions.stub
+# or extensions.predict_length to enable length prediction
 postprocessing workers = 32
+# Note that you will probably want only 1 postprocessing worker for GPU-based modules like length
+# and spectrum predictions.
 batch size = 1180 # batch size for parallel processing
 max peaks = 9999 # Discard spectra with more than this many peaks
 min peaks = 0 # Discard spectra with fewer than this many peaks
 min mass = 250 # Queries with precursor masses below this level are omitted
 max mass = 6000 # Queries with precursor mass above this level are omitted
 max charge = 4 # Max charge for spectra
 min charge = 2 # Min charge for spectra
 
 [processing.db]
 enabled = true
 workers = 32
 postprocessing workers = 32
 protein processing function = db.process_entry
 decoy protein processing function = db.process_entry_decoy
-postprocessing function = db.stub # After rt and spectrum generation, which user function to apply (db.stub: identity function)
+postprocessing function = db.stub # After rt and theoretical spectrum, which user function to apply (db.stub: identity function)
+# for spectrum generation, use db.post_ml_spectrum
 batch size = 1180
 variable modifications = M+15.994915 # Comma-separated mod list (default: M(ox))
 fixed modifications = C+57.0215 # Comma-separated mod list (default: CAM)
 nterm cleavage = 1.007825
 cterm cleavage = 17.002735
 max variable modifications = 3
 # Digestion rule as a regular expression
@@ -75,19 +76,26 @@
 # Missing values are considered to be 1.0
 # Example:
 # {"y": {"P": 5.0}, "b": {"D": 5.0, "N": 2.0, "V": 3.0, "E": 3.0, "Q": 2.0, "I": 3.0, "L": 3.0}} # x!tandem "synthesis"
 # An empty dict is {}, not the empty string.
 #weights = {"y": {"P": 5.0}, "b": {"D": 5.0, "N": 2.0, "V": 3.0, "E": 3.0, "Q": 2.0, "I": 3.0, "L": 3.0}} # x!tandem "synthesis"
 weights = {}
 
+[processing.db.post_ml_spectrum]
+batch size = 486
+device = cuda:0
+
 [postprocessing]
 enabled = true
 db = true
 queries = true
 
+[postprocessing.length]
+batch size = 64
+device = cuda:0
 [scoring]
 enabled = true
 workers = 64
 batch size = 23000
 sharding threshold = 1000000 # create a new shard after X (default: 1m) results stored in this shard
 candidate filtering tolerance = -100,100 # left and right side tolerance for candidate filtering previous to search
 filtering unit = ppm
@@ -154,32 +162,45 @@
 
 [postsearch]
 # Postprocessing step operating over the search results
 workers = 13
 batch size = 45
 function = extensions.stub
 
+[misc.tsv_to_pin]
+enabled = true
+use extra = false
+user function = #extensions.specgen_features
+max scores = 10
+
+[pin.specgen_features]
+batch size = 1024
+
 [rescoring]
 function = pepid_percolator.rescore
+#function = finetune_rf_rescorer.run # For the rf-based rescorer
 suffix = _final # Suffix to use to generate the rescored results filename. Cannot be empty.
+max scores = 10 # Keep only top `max scores` PSMs for each spectrum before training, rescoring and outputting.
 batch size = 1180 # Batch size for rescoring, in spectra
 
 [rescoring.percolator]
 percolator = percolator # point to the percolator executable
+generate pin = true # Whether to reuse existing pin or generate a new one (should be true if max scores in [rescoring] changes for instance)
 pin batch size = 100000
 pin workers = 64
 options = -Y --trainFDR 0.01 --testFDR 0.01 -i 10 # Extra command-line options for percolator binary
 cleanup = false # whether to delete the percolator .pin and .pout output at the end
 
-[misc.tsv_to_pin]
-enabled = true
-use extra = true # Whether to insert the 'extra' metadata (inserted by postprocessors)
-user function = None # Function used to generate extra feature based on the input tsv lines
-max scores = 10 # Keep only top `max scores` PSMs in pin output
-
+[rescoring.finetune_rf]
+pin workers = 20
+pin batch size = 2500
+workers = 16
+model = ml/rescorer_rf_all.pkl # Which variant to use? (nospec, nolgt, all, or base)
+score = # Which feature to use as the initial scoring direction (or: autoselect the best one)
+descending = # Feature is better in descending or ascending order?
 
 [pipeline]
 search = true
 postsearch = true
 output = true
 report = true
 rescoring = true
```

### Comparing `pepid-1.1.0/pepid/ml/best_lgt_model.py` & `pepid-1.2.0/pepid/ml/best_lgt_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 TOL = 0.1
 OFFSET=6
 GT_MIN_LGT = 6
 GT_MAX_LGT = 40
 PROT_BLIT_LEN = (int)(5000 / SIZE_RESOLUTION_FACTOR)
 PROT_TGT_LEN = (int)(2000 / SIZE_RESOLUTION_FACTOR)
 
-torch.backends.cudnn.enabled = True
-
 numpy.random.seed(0)
 
 class Model(nn.Module):
     def __init__(self):
         super(Model, self).__init__()
 
         self.emb_dim = 500
```

### Comparing `pepid-1.1.0/pepid/ml/train_best_lgt_model.py` & `pepid-1.2.0/pepid/ml/train_best_lgt_model.py`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/LICENSE.md` & `pepid-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pepid-1.1.0/README.md` & `pepid-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 
 ## Fast
 
 While pepid has some overhead compared to other engines due to its organization, it makes effective use of vectorization and JIT compilation via numba where it counts. Pepid also implements optimizations, such as a simple linear-time version of the hyperscore algorithm, which makes it faster than x!tandem with similar parameters despite being written in python.
 
 ![Pepid is faster than X!Tandem with similar search parameters](https://raw.githubusercontent.com/lemieux-lab/pepid/master/images/runtime_perf.svg)
 
+## Good
+
+Pepid achieves competitive identification performance on datasets such as ProteomeTools, a prerequisite for an effective peptide identification research platform.
+
+![Pepid identifies peptides about as well as popular alternatives](https://raw.githubusercontent.com/lemieux-lab/pepid/master/images/idents.svg)
+
 ## Scoring Functions
 
 Pepid supports baseline scoring functions based on the popular search engines Comet and X!Tandem with improvements that let it identify significantly more peptides at low FDR in realistic scenarios.
 
 Pepid currently implements two basic scoring functions, plus the combination of the two. Namely, pepid implements the Xcorr function based on the Comet codebase as of Dec 14, 2022 as well as the Hyperscore function from the X!Tandem codebase as of the same date.
 
 Pepid differs from those algorithms in a few ways: firstly, many of the parameters that are hardcoded into these search engines are exposed as parameters in pepid (for example, the factor by which to multiply the peak intensity after normalization in both cases, or the norm to use for the normalization step, or the amount of windows to use for normalization in the xcorr algorithm).
@@ -73,13 +79,12 @@
 
 Pepid also outputs a graphical report that can be used to quickly ascertain the quality of the search results, and helps identify potential sources of bias (such as the well-known peptide length bias in the Xcorr and Hyperscore functions). In addition, pepid offers a utility called `pepid_compare.py` which can be used to plot two different analyses on the same graph for comparison. The output of `pepid_compare.py` to examine rescoring by Percolator is shown below.
 
 ![Pepid with Xcorr on the 1h yeast proteome data (batched runs), comparing before and after rescoring by percolator](https://raw.githubusercontent.com/lemieux-lab/pepid/master/images/plot_compare_output_rescored.svg)
 
 ## State of the Art Features
 
-Experimental deep learning-based features are available for experimentation. Future releases will include better supported use of those features.
-Pepid includes a peptide length prediction module that can be enabled by adding extensions.predict\_length in preprocessing and extensions.postprocess\_for\_length in postprocessing, a rescoring algorithm based on a pretrained ground truth separation paradigm trained on Massive-KB along with a finetuning phase for experimental condition correction, and a whole-spectrum prediction algorithm similar to PredFull.
+Experimental deep learning-based features are available for experimentation, including a length prediction module, a custom random forest-based rescoring algorithm, and a full-spectrum generator (jointly pedicting both m/z and intensity, not just intensity).
 
 ## Citing
 
 See upcoming paper for more details.
```

### Comparing `pepid-1.1.0/pyproject.toml` & `pepid-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "pepid/example_*.cfg",
 
     "pepid/data/default.cfg",
     "pepid/ml/*",
 ]
 
 [project]
-version = "1.1.0"
+version = "1.2.0"
 name = "pepid"
 authors = [
     { name="Jeremie Zumer", email="jeremie.zumer@umontreal.ca" },
 ]
 description = "Pepid: a Highly Modifiable, Bioinformatics-Oriented Peptide Search Engine"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pepid-1.1.0/PKG-INFO` & `pepid-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepid
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pepid: a Highly Modifiable, Bioinformatics-Oriented Peptide Search Engine
 Project-URL: Homepage, https://github.com/lemieux-lab/pepid
 Project-URL: Bug Tracker, https://github.com/lemieux-lab/pepid/issues
 Author-email: Jeremie Zumer <jeremie.zumer@umontreal.ca>
 License-File: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -65,14 +65,20 @@
 
 ## Fast
 
 While pepid has some overhead compared to other engines due to its organization, it makes effective use of vectorization and JIT compilation via numba where it counts. Pepid also implements optimizations, such as a simple linear-time version of the hyperscore algorithm, which makes it faster than x!tandem with similar parameters despite being written in python.
 
 ![Pepid is faster than X!Tandem with similar search parameters](https://raw.githubusercontent.com/lemieux-lab/pepid/master/images/runtime_perf.svg)
 
+## Good
+
+Pepid achieves competitive identification performance on datasets such as ProteomeTools, a prerequisite for an effective peptide identification research platform.
+
+![Pepid identifies peptides about as well as popular alternatives](https://raw.githubusercontent.com/lemieux-lab/pepid/master/images/idents.svg)
+
 ## Scoring Functions
 
 Pepid supports baseline scoring functions based on the popular search engines Comet and X!Tandem with improvements that let it identify significantly more peptides at low FDR in realistic scenarios.
 
 Pepid currently implements two basic scoring functions, plus the combination of the two. Namely, pepid implements the Xcorr function based on the Comet codebase as of Dec 14, 2022 as well as the Hyperscore function from the X!Tandem codebase as of the same date.
 
 Pepid differs from those algorithms in a few ways: firstly, many of the parameters that are hardcoded into these search engines are exposed as parameters in pepid (for example, the factor by which to multiply the peak intensity after normalization in both cases, or the norm to use for the normalization step, or the amount of windows to use for normalization in the xcorr algorithm).
@@ -91,13 +97,12 @@
 
 Pepid also outputs a graphical report that can be used to quickly ascertain the quality of the search results, and helps identify potential sources of bias (such as the well-known peptide length bias in the Xcorr and Hyperscore functions). In addition, pepid offers a utility called `pepid_compare.py` which can be used to plot two different analyses on the same graph for comparison. The output of `pepid_compare.py` to examine rescoring by Percolator is shown below.
 
 ![Pepid with Xcorr on the 1h yeast proteome data (batched runs), comparing before and after rescoring by percolator](https://raw.githubusercontent.com/lemieux-lab/pepid/master/images/plot_compare_output_rescored.svg)
 
 ## State of the Art Features
 
-Experimental deep learning-based features are available for experimentation. Future releases will include better supported use of those features.
-Pepid includes a peptide length prediction module that can be enabled by adding extensions.predict\_length in preprocessing and extensions.postprocess\_for\_length in postprocessing, a rescoring algorithm based on a pretrained ground truth separation paradigm trained on Massive-KB along with a finetuning phase for experimental condition correction, and a whole-spectrum prediction algorithm similar to PredFull.
+Experimental deep learning-based features are available for experimentation, including a length prediction module, a custom random forest-based rescoring algorithm, and a full-spectrum generator (jointly pedicting both m/z and intensity, not just intensity).
 
 ## Citing
 
 See upcoming paper for more details.
```

