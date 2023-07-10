# Comparing `tmp/pyreference-0.7.4.tar.gz` & `tmp/pyreference-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreference-0.7.4.tar", last modified: Mon Jul 10 09:10:48 2023, max compression
+gzip compressed data, was "pyreference-0.7.5.tar", last modified: Mon Jul 10 09:21:11 2023, max compression
```

## Comparing `pyreference-0.7.4.tar` & `pyreference-0.7.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1092 2022-11-18 06:19:30.000000 pyreference-0.7.4/LICENSE.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2023-07-10 09:10:48.371362 pyreference-0.7.4/PKG-INFO
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2465 2022-11-21 06:01:21.000000 pyreference-0.7.4/README.md
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.367362 pyreference-0.7.4/bin/
--rwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)     8179 2022-11-18 06:19:30.000000 pyreference-0.7.4/bin/pyreference_biotype.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.367362 pyreference-0.7.4/pyreference/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      188 2023-07-10 05:08:40.000000 pyreference-0.7.4/pyreference/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3617 2023-07-10 09:05:02.000000 pyreference-0.7.4/pyreference/gene.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2216 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/genomic_region.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      746 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/mirna.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2145 2023-07-10 09:03:50.000000 pyreference-0.7.4/pyreference/pyreference_config.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    24834 2023-07-10 09:04:47.000000 pyreference-0.7.4/pyreference/reference.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1246 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/referenceargparse.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      325 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/settings.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9621 2023-07-10 08:55:55.000000 pyreference-0.7.4/pyreference/transcript.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/pyreference/utils/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1173 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/file_utils.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3631 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/genomics_utils.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1295 2022-11-18 06:19:30.000000 pyreference-0.7.4/pyreference/utils/iv_iterators.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/pyreference.egg-info/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/PKG-INFO
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      642 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/SOURCES.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        1 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/dependency_links.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       84 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/requires.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       12 2023-07-10 09:10:48.000000 pyreference-0.7.4/pyreference.egg-info/top_level.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       38 2023-07-10 09:10:48.371362 pyreference-0.7.4/setup.cfg
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1815 2023-03-02 00:49:39.000000 pyreference-0.7.4/setup.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:10:48.371362 pyreference-0.7.4/tests/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.4/tests/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9509 2023-07-07 01:17:20.000000 pyreference-0.7.4/tests/test_reference.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:21:11.102495 pyreference-0.7.5/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1092 2022-11-18 06:19:30.000000 pyreference-0.7.5/LICENSE.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2023-07-10 09:21:11.102495 pyreference-0.7.5/PKG-INFO
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2465 2022-11-21 06:01:21.000000 pyreference-0.7.5/README.md
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:21:11.098495 pyreference-0.7.5/bin/
+-rwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)     8179 2022-11-18 06:19:30.000000 pyreference-0.7.5/bin/pyreference_biotype.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:21:11.102495 pyreference-0.7.5/pyreference/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      188 2023-07-10 09:18:32.000000 pyreference-0.7.5/pyreference/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3617 2023-07-10 09:05:02.000000 pyreference-0.7.5/pyreference/gene.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2216 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/genomic_region.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      746 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/mirna.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2145 2023-07-10 09:03:50.000000 pyreference-0.7.5/pyreference/pyreference_config.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    24836 2023-07-10 09:16:15.000000 pyreference-0.7.5/pyreference/reference.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1246 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/referenceargparse.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      325 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/settings.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9621 2023-07-10 08:55:55.000000 pyreference-0.7.5/pyreference/transcript.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:21:11.102495 pyreference-0.7.5/pyreference/utils/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/utils/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1173 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/utils/file_utils.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3631 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/utils/genomics_utils.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1295 2022-11-18 06:19:30.000000 pyreference-0.7.5/pyreference/utils/iv_iterators.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:21:11.102495 pyreference-0.7.5/pyreference.egg-info/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3237 2023-07-10 09:21:11.000000 pyreference-0.7.5/pyreference.egg-info/PKG-INFO
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      642 2023-07-10 09:21:11.000000 pyreference-0.7.5/pyreference.egg-info/SOURCES.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        1 2023-07-10 09:21:11.000000 pyreference-0.7.5/pyreference.egg-info/dependency_links.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       84 2023-07-10 09:21:11.000000 pyreference-0.7.5/pyreference.egg-info/requires.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       12 2023-07-10 09:21:11.000000 pyreference-0.7.5/pyreference.egg-info/top_level.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       38 2023-07-10 09:21:11.102495 pyreference-0.7.5/setup.cfg
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1815 2023-03-02 00:49:39.000000 pyreference-0.7.5/setup.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2023-07-10 09:21:11.102495 pyreference-0.7.5/tests/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-11-18 06:19:30.000000 pyreference-0.7.5/tests/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     9509 2023-07-07 01:17:20.000000 pyreference-0.7.5/tests/test_reference.py
```

### Comparing `pyreference-0.7.4/LICENSE.txt` & `pyreference-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/PKG-INFO` & `pyreference-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreference
-Version: 0.7.4
+Version: 0.7.5
 Summary: Library for working with reference genomes and gene GTF/GFFs
 Home-page: https://github.com/SACGF/pyreference
 Author: David Lawrence
 Author-email: davmlaw@gmail.com
 Keywords: genomics,gtf,gff,genome,genes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreference-0.7.4/README.md` & `pyreference-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/bin/pyreference_biotype.py` & `pyreference-0.7.5/bin/pyreference_biotype.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/gene.py` & `pyreference-0.7.5/pyreference/gene.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/genomic_region.py` & `pyreference-0.7.5/pyreference/genomic_region.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/mirna.py` & `pyreference-0.7.5/pyreference/mirna.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/pyreference_config.py` & `pyreference-0.7.5/pyreference/pyreference_config.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/reference.py` & `pyreference-0.7.5/pyreference/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         self._mature_mir_sequence_fasta = params.get("mature_mir_sequence_fasta")
         self._cdot_schema_version = None  # Set on load
         self.use_gzip_open = params.get("use_gzip_open", True)
         self.stranded = params.get("stranded", True)
         self._gene_by_id = {}  # Object pool for Gene objects
 
         REPRESENTATIVE_TRANSCRIPT_METHODS = ["tags", "longest_coding", "longest"]
-        representative_transcript_raw = params.get("representative_transcript", ["longest_coding" , "longest"])
+        representative_transcript_raw = params.get("representative_transcript") or ["longest_coding" , "longest"]
         if isinstance(representative_transcript_raw, str):
             self.representative_transcript_list = representative_transcript_raw.split(",")
         else:
             self.representative_transcript_list = representative_transcript_raw
         if not (self.representative_transcript_list and
                 all([r in REPRESENTATIVE_TRANSCRIPT_METHODS for r in self.representative_transcript_list])):
             msg = "representative_transcript='%(representative_transcript)s' must be list or comma " \
```

### Comparing `pyreference-0.7.4/pyreference/referenceargparse.py` & `pyreference-0.7.5/pyreference/referenceargparse.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/transcript.py` & `pyreference-0.7.5/pyreference/transcript.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/utils/file_utils.py` & `pyreference-0.7.5/pyreference/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/utils/genomics_utils.py` & `pyreference-0.7.5/pyreference/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference/utils/iv_iterators.py` & `pyreference-0.7.5/pyreference/utils/iv_iterators.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/pyreference.egg-info/PKG-INFO` & `pyreference-0.7.5/pyreference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreference
-Version: 0.7.4
+Version: 0.7.5
 Summary: Library for working with reference genomes and gene GTF/GFFs
 Home-page: https://github.com/SACGF/pyreference
 Author: David Lawrence
 Author-email: davmlaw@gmail.com
 Keywords: genomics,gtf,gff,genome,genes
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyreference-0.7.4/pyreference.egg-info/SOURCES.txt` & `pyreference-0.7.5/pyreference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/setup.py` & `pyreference-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyreference-0.7.4/tests/test_reference.py` & `pyreference-0.7.5/tests/test_reference.py`

 * *Files identical despite different names*

