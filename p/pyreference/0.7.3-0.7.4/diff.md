# Comparing `tmp/pyreference-0.7.3.tar.gz` & `tmp/pyreference-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreference-0.7.3.tar", last modified: Thu Jul  6 06:44:42 2023, max compression
+gzip compressed data, was "pyreference-0.7.4.tar", last modified: Mon Jul 10 09:10:48 2023, max compression
```

## Comparing `pyreference-0.7.3.tar` & `pyreference-0.7.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/
--rw-rw-r--   0 root         (0) root         (0)     1092 2023-03-21 01:08:04.000000 pyreference-0.7.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3237 2023-07-06 06:44:42.961318 pyreference-0.7.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2465 2023-03-21 01:08:04.000000 pyreference-0.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/bin/
--rwxrwxr-x   0 root         (0) root         (0)     8179 2023-03-21 01:08:04.000000 pyreference-0.7.3/bin/pyreference_biotype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/pyreference/
--rw-rw-r--   0 root         (0) root         (0)      188 2023-07-06 06:39:49.000000 pyreference-0.7.3/pyreference/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2818 2023-07-06 06:33:40.000000 pyreference-0.7.3/pyreference/gene.py
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/genomic_region.py
--rw-rw-r--   0 root         (0) root         (0)      746 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/mirna.py
--rw-rw-r--   0 root         (0) root         (0)     2102 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/pyreference_config.py
--rw-rw-r--   0 root         (0) root         (0)    20304 2023-07-06 05:45:06.000000 pyreference-0.7.3/pyreference/reference.py
--rw-rw-r--   0 root         (0) root         (0)     1246 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/referenceargparse.py
--rw-rw-r--   0 root         (0) root         (0)      325 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/settings.py
--rw-rw-r--   0 root         (0) root         (0)     9533 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/transcript.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/pyreference/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1173 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/file_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3631 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/genomics_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1295 2023-03-21 01:08:04.000000 pyreference-0.7.3/pyreference/utils/iv_iterators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/pyreference.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3237 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-06 06:44:42.000000 pyreference-0.7.3/pyreference.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 06:44:42.961318 pyreference-0.7.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1815 2023-03-21 01:08:04.000000 pyreference-0.7.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 06:44:42.961318 pyreference-0.7.3/tests/
--rw-rw-r--   0 root         (0) root         (0)     9509 2023-07-06 06:31:17.000000 pyreference-0.7.3/tests/test_reference.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1092 2022-11-18 06:19:30.000000 pyreference-0.7.4/LICENSE.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2023-07-10 09:10:48.371362 pyreference-0.7.4/PKG-INFO
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2465 2022-11-21 06:01:21.000000 pyreference-0.7.4/README.md
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.367362 pyreference-0.7.4/bin/
+-rwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)     8179 2022-11-18 06:19:30.000000 pyreference-0.7.4/bin/pyreference_biotype.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.367362 pyreference-0.7.4/pyreference/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      188 2023-07-10 05:08:40.000000 pyreference-0.7.4/pyreference/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3617 2023-07-10 09:05:02.000000 pyreference-0.7.4/pyreference/gene.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2216 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/genomic_region.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      746 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/mirna.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2145 2023-07-10 09:03:50.000000 pyreference-0.7.4/pyreference/pyreference_config.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    24834 2023-07-10 09:04:47.000000 pyreference-0.7.4/pyreference/reference.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1246 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/referenceargparse.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      325 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/settings.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9621 2023-07-10 08:55:55.000000 pyreference-0.7.4/pyreference/transcript.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/pyreference/utils/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1173 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/file_utils.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3631 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/genomics_utils.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1295 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/iv_iterators.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/pyreference.egg-info/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/PKG-INFO
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      642 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/SOURCES.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        1 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/dependency_links.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       84 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/requires.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       12 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/top_level.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       38 2023-07-10 09:10:48.371362 pyreference-0.7.4/setup.cfg
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1815 2023-03-02 00:49:39.000000 pyreference-0.7.4/setup.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/tests/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.4/tests/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9509 2023-07-07 01:17:20.000000 pyreference-0.7.4/tests/test_reference.py
```

### Comparing `pyreference-0.7.3/LICENSE.txt` & `pyreference-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/PKG-INFO` & `pyreference-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreference
-Version: 0.7.3
+Version: 0.7.4
 Summary: Library for working with reference genomes and gene GTF/GFFs
 Home-page: https://github.com/SACGF/pyreference
 Author: David Lawrence
 Author-email: davmlaw@gmail.com
 Keywords: genomics,gtf,gff,genome,genes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreference-0.7.3/README.md` & `pyreference-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/bin/pyreference_biotype.py` & `pyreference-0.7.4/bin/pyreference_biotype.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference/gene.py` & `pyreference-0.7.4/pyreference/gene.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,39 @@
 """
 
 from lazy import lazy
 from pyreference.genomic_region import GenomicRegion
 from pyreference.transcript import Transcript
 import sys
 
+try:
+    _big_int = sys.maxsize  # Python 3
+except AttributeError:
+    _big_int = sys.maxint  # Python 2
+
+def min_transcript_key(t):
+    # We want the MAX length - and MIN ID, so sort by min but use maxint-length
+    # We also want NM_007041 (len 2209) over NM_001001976 (len 2209)
+    # Which is annoyingly zero padded - so use smallest ID length, then only if equal do alpha sort
+    return _big_int - t.length, len(t.get_id()), t.get_id()
+
+
+def min_canonical_tag(t):
+    # we use 'not in' as False < True (so will get minimum)
+    CANONICAL_TAGS = ["MANE Select", "MANE_Select", "RefSeq Select", "Ensembl Select"]
+    return tuple([x not in t.tags for x in CANONICAL_TAGS])
+
 
 class Gene(GenomicRegion):
     """ Gene (which could contain multiple transcripts) """
 
     @property
     def name(self):
         return self.get_gene_name()
+
     @property
     def description(self):
         return self._dict.get("description")
 
     @property
     def biotype(self):
         return self._dict.get("biotype")
@@ -48,43 +66,50 @@
     def is_coding(self):
         return any(t.is_coding for t in self.transcripts)
 
     @lazy
     def representative_transcript(self):
         """ Returns longest coding transcript if gene is coding, otherwise longest transcript
             Sort transcript ID alphabetically if equal length """
-        
-        transcript = self.get_longest_coding_transcript()
-        if transcript is None:
-            transcript = self.get_longest_transcript()
+
+        methods = {
+            "tags": self.get_canonical_transcript_from_tags,
+            "longest_coding": self.get_longest_coding_transcript,
+            "longest": self.get_longest_transcript,
+        }
+
+        transcript = None
+        for rt_method in self.reference.representative_transcript_list:
+            func = methods[rt_method]
+            transcript = func()
+            if transcript:
+                return transcript
         return transcript
 
+    def get_canonical_transcript_from_tags(self):
+        """ Using the GTF tag (eg 'MANE_select') """
+        transcripts = self.transcripts
+        transcripts = filter(lambda t: t.tags, transcripts)
+        canonical_transcript = None
+        if transcripts:
+            canonical_transcript = min(transcripts, key=min_canonical_tag)
+        return canonical_transcript
+
     def get_representative_transcript(self):
         return self.representative_transcript
 
     def get_longest_coding_transcript(self):
         return self.get_longest_transcript(coding_only=True)
-    
+
     def get_longest_transcript(self, coding_only=False):
         transcripts = self.transcripts
         if coding_only:
             transcripts = filter(lambda t: t.is_coding, transcripts)
         
         longest_transcript = None
         if transcripts:
-            try:
-                big_int = sys.maxint  # Python 2
-            except AttributeError:
-                big_int = sys.maxsize  # Python 3
-
-            # We want the MAX length - and MIN ID, so sort by min but use maxint-length
-            # We also want NM_007041 (len 2209) over NM_001001976 (len 2209)
-            # Which is annoyingly zero padded - so use smallest ID length, then only if equal do alpha sort 
-            def min_transcript_key(t):
-                return big_int - t.length, len(t.get_id()), t.get_id()
-
             longest_transcript = min(transcripts, key=min_transcript_key)
         return longest_transcript
 
     def __repr__(self):
         return "%s (%s) %d transcripts" % (self.get_gene_name(), self.accession_id, len(self.transcripts))
```

### Comparing `pyreference-0.7.3/pyreference/genomic_region.py` & `pyreference-0.7.4/pyreference/genomic_region.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference/mirna.py` & `pyreference-0.7.4/pyreference/mirna.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference/pyreference_config.py` & `pyreference-0.7.4/pyreference/pyreference_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     defaults = {
         'genome_accession': None,
         'genes_json': None,
         'trna_json': None,
         'mature_mir_sequence_fasta': None,
         'genome_sequence_fasta': None,
         "genome_sequence_lookup": None,
+        "representative_transcript": None,
     }
     cfg = ConfigParser(allow_no_value=True, defaults=defaults)
     cfg.read(config)
 
     if build is None:
         try:
             build = cfg.get("global", "default_build")
```

### Comparing `pyreference-0.7.3/pyreference/reference.py` & `pyreference-0.7.4/pyreference/reference.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,63 +42,67 @@
 
     if use_gzip_open:
         try:
             with gzip.open(gz_json_file_name, "rb") as f:
                 json_bytes = f.read()
         except IOError as e:
             # We sometimes get [Errno 5] Input/output error using CIFS (SMB)
-            print(e, file=sys.stderr)
+            logging.warning(e)
             if e.errno == 5:
                 decompress_in_memory = True
 
     if decompress_in_memory:
         with open(gz_json_file_name, "rb") as f:
             gzip_bytes = f.read()
             json_bytes = gzip.GzipFile(fileobj=six.StringIO(gzip_bytes)).read()
 
         if use_gzip_open:
             msg = "gzip.open failed, successfully fell back on in-memory decompression\n"
             msg += "Please set use_gzip_open=False in your settings to speed up load times."
-            print(msg, file=sys.stderr)
+            logging.warning(msg)
 
     if six.PY2:
         json_str = json_bytes
     else:
         json_str = json_bytes.decode('ascii')
     data = json.loads(json_str)
 
     extra_message = None
-    if raw_json_version := data.get(settings.CDOT_JSON_VERSION_KEY):
+    raw_json_version = data.get(settings.CDOT_JSON_VERSION_KEY)
+    if raw_json_version:
         json_version = get_schema_version(raw_json_version.split("."))
         version_key = settings.CDOT_JSON_VERSION_KEY
-    elif old_pyreference_version := data.get("pyreference_json_version"):
-        json_version = "Old pre-cot Pyreference v%d" % old_pyreference_version
-        version_key = "pyreference_json_version"
-        extra_message = "PyReference switched to using cdot generated files in November 2022\n"
     else:
-        raise ValueError('Invalid PyReference genes_json file: %s' % gz_json_file_name)
-
-    cdot_schema_version = get_schema_version(CDOT_VERSION_SCHEMA)
-    if cdot_schema_version != json_version:
+        old_pyreference_version = data.get("pyreference_json_version")
+        if old_pyreference_version:
+            json_version = "Old pre-cot Pyreference v%d" % old_pyreference_version
+            version_key = "pyreference_json_version"
+            extra_message = "PyReference switched to using cdot generated files in November 2022\n"
+        else:
+            raise ValueError('Invalid PyReference genes_json file: %s' % gz_json_file_name)
+
+    required_cdot_schema_version = get_schema_version(CDOT_VERSION_SCHEMA)
+    if required_cdot_schema_version != json_version:
+        import pyreference
         params = {
             "pyreference_version": pyreference.__version__,
-            "cdot_schema_version": cdot_schema_version,
+            "required_cdot_schema_version": required_cdot_schema_version,
             "version_key": version_key,
             "json_version": json_version,
             "file_name": gz_json_file_name,
             "wiki_url": "https://github.com/SACGF/pyreference/wiki/genes_json_file",
         }
-        msg = "PyReference %(pyreference_version)s requires cdot genes JSON file of schema v.%(cdot_schema_version)d\n"
+        msg = "PyReference %(pyreference_version)s requires cdot genes JSON file of schema v.%(required_cdot_schema_version)d\n"
         msg += "Genes JSON file '%(file_name)s' has %(version_key)s: %(json_version)s.\n"
         if extra_message:
             msg += extra_message
         msg += "Please download or re-create a genes JSON file from GTF. See %(wiki_url)s"
         raise ValueError(msg % params)
 
-    return data
+    return data, json_version
 
 
 class Reference(object):
     def __init__(self, build=None, config=None, load_config_file=True, **kwargs):
         """ Construct a new reference object via:
         
             build - from pyreference config file (defaults to [global] default_build from config file) 
@@ -132,16 +136,34 @@
         params.update({k: v for (k, v) in kwargs.items() if v is not None})
         self._genome_accession = params.get("genome_accession")
         self._genes_json = params.get("genes_json")
         self._trna_json = params.get("trna_json")
         self._genome_sequence_fasta = params.get("genome_sequence_fasta")
         self._genome_sequence_lookup = params.get("genome_sequence_lookup")
         self._mature_mir_sequence_fasta = params.get("mature_mir_sequence_fasta")
+        self._cdot_schema_version = None  # Set on load
         self.use_gzip_open = params.get("use_gzip_open", True)
         self.stranded = params.get("stranded", True)
+        self._gene_by_id = {}  # Object pool for Gene objects
+
+        REPRESENTATIVE_TRANSCRIPT_METHODS = ["tags", "longest_coding", "longest"]
+        representative_transcript_raw = params.get("representative_transcript", ["longest_coding" , "longest"])
+        if isinstance(representative_transcript_raw, str):
+            self.representative_transcript_list = representative_transcript_raw.split(",")
+        else:
+            self.representative_transcript_list = representative_transcript_raw
+        if not (self.representative_transcript_list and
+                all([r in REPRESENTATIVE_TRANSCRIPT_METHODS for r in self.representative_transcript_list])):
+            msg = "representative_transcript='%(representative_transcript)s' must be list or comma " \
+                  "separated list of '%(valid_representative_transcript)s'"
+            msg_params = {
+                'representative_transcript': representative_transcript_raw,
+                'valid_representative_transcript': ', '.join(REPRESENTATIVE_TRANSCRIPT_METHODS),
+            }
+            raise ValueError(msg % msg_params)
 
         # Need at least this
         REQUIRED = {
             "genome_accession": self._genome_accession,
             "genes_json": self._genes_json,
         }
 
@@ -165,17 +187,58 @@
             logging.warning(f"Bioutils does not support genome build '{self._genome_accession}' cannot perform chrom/contig mapping")
 
         # Store this so we can ask about config later
         self.build = params["build"]
         self._args = {"build": build, "config": config}
         self._build_params = params
 
+    def info(self):
+        import pyreference
+        return {
+            "python": sys.version,
+            "pyreference_version": pyreference.__version__,
+            "cdot_schema_version": self._cdot_schema_version,
+            "genome_accession": self._genome_accession,
+            "genes_json": self._genes_json,
+        }
+
+    @staticmethod
+    def _merge_genes_with_duplicate_symbols(genes_dict):
+        # There are occasionally multiple genes per symbol in Ensembl GTF files. Merge these
+        # taking the first one in file. This isn't correct but is a simplifying assumption of how people want to work
+        # @see https://github.com/SACGF/pyreference/issues/10
+        genes_by_symbol = {}
+        gene_merges = {}  # key = original gene ID (which will be lost), value = merge gene ID (kept)
+        for gene_id, gene_data in genes_dict["genes"].items():
+            gene_symbol = gene_data.get("gene_symbol")
+            if gene_symbol:
+                existing_gene_id = genes_by_symbol.get(gene_symbol)
+                if existing_gene_id:
+                    logging.warning("GeneID with duplicate symbol for %s: merging %s into %s",
+                                    gene_symbol, gene_id, existing_gene_id)
+                    gene_merges[gene_id] = existing_gene_id
+                else:
+                    genes_by_symbol[gene_symbol] = gene_id
+
+        # Replace transcripts
+        for transcript_data in genes_dict["transcripts"].values():
+            gene_version = transcript_data["gene_version"]
+            existing_gene_id = gene_merges.get(gene_version)
+            if existing_gene_id:
+                transcript_data["gene_version"] = existing_gene_id
+
+        for gene_id, existing_gene_id in gene_merges.items():
+            del genes_dict["genes"][gene_id]
+
     @lazy
     def _genes_dict(self):
-        return _load_gzip_json(self._genes_json, self.use_gzip_open)
+        genes_dict, cdot_schema_version = _load_gzip_json(self._genes_json, self.use_gzip_open)
+        self._cdot_schema_version = cdot_schema_version
+        self._merge_genes_with_duplicate_symbols(genes_dict)
+        return genes_dict
 
     def get_transcript_dict(self, transcript_id):
         """ Moves 'genome_build' down into 1st level of dict as we only need 1 """
         transcripts_by_id = self._genes_dict["transcripts"]
         tdata = transcripts_by_id[transcript_id].copy()
         genome_build = tdata.pop("genome_builds")
         tdata.update(genome_build[self._genome_accession])
@@ -187,25 +250,35 @@
         return tdata
 
     @lazy
     def _gene_id_lookups(self):
         gene_transcripts = defaultdict(set)
         gene_version_by_biotype = defaultdict(set)  # Set from both genes/transcripts
         for transcript_id, tdata in self._genes_dict["transcripts"].items():
-            if gene_version := tdata["gene_version"]:
+            gene_version = tdata.get("gene_version")
+            if gene_version:
                 gene_transcripts[gene_version].add(transcript_id)
+                # In cdot 0.2.20 onwards gene version will have biotype of any transcripts, but earlier this wasn't so
                 for biotype in tdata["biotype"]:
                     gene_version_by_biotype[biotype].add(gene_version)
 
         gene_version_by_symbol = {}
         for gene_version, gdata in self._genes_dict["genes"].items():
-            if gene_symbol := gdata.get("gene_symbol"):
+            gene_symbol = gdata.get("gene_symbol")
+            if gene_symbol:
                 gene_version_by_symbol[gene_symbol] = gene_version
-            if biotype := gdata.get("biotype"):
-                gene_version_by_biotype[biotype].add(gene_version)
+            raw_biotype = gdata.get("biotype")
+            if raw_biotype:
+                # Previously biotype was a string. In cdot 0.2.20 gene biotype is now a list (to match transcript)
+                if isinstance(raw_biotype, list):
+                    biotype_list = raw_biotype
+                else:
+                    biotype_list = [raw_biotype]
+                for biotype in biotype_list:
+                    gene_version_by_biotype[biotype].add(gene_version)
 
         return gene_transcripts, gene_version_by_symbol, gene_version_by_biotype
 
     @property
     def gene_transcripts(self):
         return self._gene_id_lookups[0]
 
@@ -258,43 +331,63 @@
                 genes.append(self.get_gene_by_id(gene_id))
 
             genes_by_biotype[biotype] = genes
 
         return genes_by_biotype
 
     def get_gene_by_id(self, gene_id):
+        gene = self._gene_by_id.get(gene_id)  # Re-use from shared pool
+        if gene:
+            return gene
         genes_by_id = self._genes_dict["genes"]
         gene_dict = genes_by_id.get(gene_id)
         if gene_dict is None:
             msg = "No Gene found with ID=%s" % gene_id
             raise ValueError(msg)
 
         gene_dict = gene_dict.copy()
         # Add generated transcript array
         transcripts = self.gene_transcripts.get(gene_id, [])
         gene_dict["transcripts"] = transcripts
         # Retrieve gene extents from transcript
         start = sys.maxsize
         end = 0
-        chrom = None
-        strand = None
+        chrom_set = set()
+        strand_set = set()
         for transcript_id in transcripts:
             tdata = self.get_transcript_dict(transcript_id)
             exons = tdata["exons"]
             start = min(start, exons[0][0])
             end = max(end, exons[-1][1])
-            if chrom is None:
-                chrom = tdata[settings.CHROM]
-                strand = tdata[settings.STRAND]
+            chrom_set.add(tdata[settings.CHROM])
+            strand_set.add(tdata[settings.STRAND])
 
+        num_chrom = len(chrom_set)
+
+        gene_symbol = gene_dict["gene_symbol"]
+        if num_chrom == 1:
+            chrom = chrom_set.pop()
+        else:
+            logging.warning("Transcripts for gene %s were on %d chromosomes (expected 1)", gene_symbol, num_chrom)
+            chrom = ""
         gene_dict[settings.CHROM] = chrom
+
+        num_strand = len(strand_set)
+        if num_strand == 1:
+            strand = strand_set.pop()
+        else:
+            strand = ""
+            logging.warning("Transcripts for gene %s were on %d strands (expected 1)", gene_symbol, num_strand)
+
         gene_dict[settings.STRAND] = strand
         gene_dict[settings.START] = start
         gene_dict[settings.END] = end
-        return Gene(self, gene_id, gene_dict)
+        gene = Gene(self, gene_id, gene_dict)
+        self._gene_by_id[gene_id] = gene
+        return gene
 
     def get_transcript_by_id(self, transcript_id):
         transcript_dict = self.get_transcript_dict(transcript_id)
         if transcript_dict is None:
             msg = "No Transcript found with ID=%s" % transcript_dict
             raise ValueError(msg)
         return Transcript(self, transcript_id, transcript_dict)
```

### Comparing `pyreference-0.7.3/pyreference/referenceargparse.py` & `pyreference-0.7.4/pyreference/referenceargparse.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference/transcript.py` & `pyreference-0.7.4/pyreference/transcript.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     def get_gene_id(self):
         return self.gene.get_id() 
 
     @lazy
     def is_coding(self):
         return "start_codon" in self._dict
 
+    @lazy
+    def tags(self):
+        return set(self._dict.get("tag", "").split(","))
+
     @property
     def is_forward_strand(self):
         return self._dict["strand"] == "+"
 
     def get_representative_transcript(self):
         return self
```

### Comparing `pyreference-0.7.3/pyreference/utils/file_utils.py` & `pyreference-0.7.4/pyreference/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference/utils/genomics_utils.py` & `pyreference-0.7.4/pyreference/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference/utils/iv_iterators.py` & `pyreference-0.7.4/pyreference/utils/iv_iterators.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/pyreference.egg-info/PKG-INFO` & `pyreference-0.7.4/pyreference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreference
-Version: 0.7.3
+Version: 0.7.4
 Summary: Library for working with reference genomes and gene GTF/GFFs
 Home-page: https://github.com/SACGF/pyreference
 Author: David Lawrence
 Author-email: davmlaw@gmail.com
 Keywords: genomics,gtf,gff,genome,genes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreference-0.7.3/pyreference.egg-info/SOURCES.txt` & `pyreference-0.7.4/pyreference.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 pyreference.egg-info/dependency_links.txt
 pyreference.egg-info/requires.txt
 pyreference.egg-info/top_level.txt
 pyreference/utils/__init__.py
 pyreference/utils/file_utils.py
 pyreference/utils/genomics_utils.py
 pyreference/utils/iv_iterators.py
+tests/__init__.py
 tests/test_reference.py
```

### Comparing `pyreference-0.7.3/setup.py` & `pyreference-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.3/tests/test_reference.py` & `pyreference-0.7.4/tests/test_reference.py`

 * *Files identical despite different names*

