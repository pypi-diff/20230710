# Comparing `tmp/StORF-Reporter-1.0.2.tar.gz` & `tmp/StORF-Reporter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StORF-Reporter-1.0.2.tar", last modified: Mon Jul 10 20:51:51 2023, max compression
+gzip compressed data, was "StORF-Reporter-1.0.3.tar", last modified: Mon Jul 10 21:07:43 2023, max compression
```

## Comparing `StORF-Reporter-1.0.2.tar` & `StORF-Reporter-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/
--rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/LICENSE
--rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-07-10 20:50:43.000000 StORF-Reporter-1.0.2/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-19 15:34:48.000000 StORF-Reporter-1.0.2/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/setup.cfg
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.521597 StORF-Reporter-1.0.2/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/src/StORF_Reporter/
--rw-r--r--   0 nick      (1000) nick      (1000)       34 2023-07-10 20:50:43.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Constants.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16601 2023-07-10 18:01:01.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Extractor.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Finder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5220 2023-07-10 18:01:01.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Remover.py
--rw-r--r--   0 nick      (1000) nick      (1000)    52121 2023-07-10 20:39:48.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Reporter.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/
--rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/StORF_Adder.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/UR_Lenghts.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/Un_StORFed.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/__init__.py
--rwxr-xr-x   0 nick      (1000) nick      (1000)    15208 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/UR_Extractor.py
--rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 19:37:38.000000 StORF-Reporter-1.0.2/src/StORF_Reporter/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 20:51:51.525597 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-07-10 20:51:51.000000 StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 21:07:43.796499 StORF-Reporter-1.0.3/
+-rw-r--r--   0 nick      (1000) nick      (1000)    35149 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.3/LICENSE
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-07-10 21:07:43.796499 StORF-Reporter-1.0.3/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    19279 2023-07-10 21:05:47.000000 StORF-Reporter-1.0.3/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)      147 2022-12-19 15:34:48.000000 StORF-Reporter-1.0.3/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-07-10 21:07:43.796499 StORF-Reporter-1.0.3/setup.cfg
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 21:07:43.792499 StORF-Reporter-1.0.3/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 21:07:43.792499 StORF-Reporter-1.0.3/src/StORF_Reporter/
+-rw-r--r--   0 nick      (1000) nick      (1000)       34 2023-07-10 21:05:47.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/Constants.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16601 2023-07-10 18:01:01.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Extractor.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    47406 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Finder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5220 2023-07-10 18:01:01.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Remover.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    52121 2023-07-10 20:39:48.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Reporter.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 21:07:43.796499 StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2075 2023-05-29 18:06:24.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/StORF_Adder.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1270 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/UR_Lenghts.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9682 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/Un_StORFed.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2022-12-19 15:31:53.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/__init__.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)    15212 2023-07-10 21:02:02.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/UR_Extractor.py
+-rw-r--r--   0 nick      (1000) nick      (1000)        0 2023-01-06 19:37:38.000000 StORF-Reporter-1.0.3/src/StORF_Reporter/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-07-10 21:07:43.796499 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19923 2023-07-10 21:07:43.000000 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      695 2023-07-10 21:07:43.000000 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-07-10 21:07:43.000000 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      269 2023-07-10 21:07:43.000000 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       25 2023-07-10 21:07:43.000000 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       15 2023-07-10 21:07:43.000000 StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/top_level.txt
```

### Comparing `StORF-Reporter-1.0.2/LICENSE` & `StORF-Reporter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/PKG-INFO` & `StORF-Reporter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 1.0.2
+Version: 1.0.3
 Summary: StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 Home-page: https://github.com/NickJD/StORF-Reporter
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/StORF-Reporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -73,15 +73,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.3: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -183,15 +183,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.3: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -221,15 +221,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.3: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -285,15 +285,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.3: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -318,15 +318,15 @@
 StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
 ```
 
 ```python
 usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
                         [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.3: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.2/README.md` & `StORF-Reporter-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.3: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -168,15 +168,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.3: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -206,15 +206,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.3: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -270,15 +270,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.3: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -303,15 +303,15 @@
 StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
 ```
 
 ```python
 usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
                         [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.3: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.2/setup.cfg` & `StORF-Reporter-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = StORF-Reporter
-version = v1.0.2
+version = v1.0.3
 author = Nicholas Dimonaco
 author_email = nicholas@dimonaco.co.uk
 description = StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NickJD/StORF-Reporter
 project_urls =
```

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Extractor.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Extractor.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Finder.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Finder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Remover.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Remover.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/StORF_Reporter.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/StORF_Reporter.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/StORF_Adder.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/StORF_Adder.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/UR_Lenghts.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/UR_Lenghts.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/Tools/Un_StORFed.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/Tools/Un_StORFed.py`

 * *Files identical despite different names*

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter/UR_Extractor.py` & `StORF-Reporter-1.0.3/src/StORF_Reporter/UR_Extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                                 dna_regions[line_data[0]][2].append(pos) # This will add to list
                 except IndexError:
                     continue
     return dna_regions
 
 def gff_load(options,gff_in,dna_regions):
     for line in gff_in:  # Get gene loci from GFF - ID=Gene will also classify Pseudogenes as genes
-        line_data = line.split()
+        line_data = line.split('\t')
         if line.startswith('\n') or line.startswith('#') or 'European Nucleotide Archive' in line:  # Not to crash on empty lines in GFF
             continue
         elif options.gene_ident[0] == 'ID=gene':
             if line_data[0] in dna_regions and options.gene_ident[0] in line_data[8]:
                 pos = line_data[3] + '_' + line_data[4]
                 dna_regions[line_data[0]][2].append(pos) # This will add to list
         else:
```

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/PKG-INFO` & `StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StORF-Reporter
-Version: 1.0.2
+Version: 1.0.3
 Summary: StORF-Reporter - A a tool that takes an annotated genome and returns missing CDS genes (Stop-to-Stop) from unannotated regions.
 Home-page: https://github.com/NickJD/StORF-Reporter
 Author: Nicholas Dimonaco
 Author-email: nicholas@dimonaco.co.uk
 Project-URL: Bug Tracker, https://github.com/NickJD/StORF-Reporter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -73,15 +73,15 @@
                          [-ex_len EXLEN] [-spos {True,False}] [-rs {True,False}] [-con_storfs {True,False}]
                          [-con_only {True,False}] [-ps {True,False}] [-wc {True,False}] [-short_storfs {False,Nolap,Olap}]
                          [-short_storfs_only {True,False}] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS]
                          [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-so [{start_pos,strand}]]
                          [-f_type [{StORF,CDS,ORF}]] [-olap OVERLAP_NT] [-ao ALLOWED_OVERLAP] [-overwrite {True,False}]
                          [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Reporter Run Parameters.
+StORF-Reporter v1.0.3: StORF-Reporter Run Parameters.
 
 Required Options:
   -anno [{Prokka,Bakta,Out_Dir,Single_GFF,Multiple_GFFs,Ensembl,Feature_Types,Single_Genome,Multiple_Genomes,Single_Combined_GFF,Multiple_Combined_GFFs,Pyrodigal,Single_FASTA,Multiple_FASTA} ...]
                         Select Annotation and Input options for one of the 3 options listed below
                         ### Prokka/Bakta Annotation Option 1: 
                         	Prokka = Report StORFs for a Prokka annotation; 
                         	Bakta = Report StORFs for a Bakta annotation; 
@@ -183,15 +183,15 @@
 ```console
 UR-Extractor -f .../Test_Datasets/Matching_GFF_FASTA/E-coli.fa -gff .../Test_Datasets/Matching_GFF_FASTA/E-coli.gff
 ```
 
 ```python
 usage: UR_Extractor.py [-h] [-f FASTA] [-gff GFF] [-ident IDENT] [-min_len MINLEN] [-max_len MAXLEN] [-ex_len EXLEN] [-gene_ident GENE_IDENT] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.3: UR-Extractor Run Parameters.
 
 Required Arguments:
   -f FASTA              FASTA file for Unannotated Region seq extraction
   -gff GFF              GFF annotation file for the FASTA
 
 Optional Arguments:
   -ident IDENT          Identifier given for Unannotated Region output sequences - Do not modify if output is to be used by StORF-Finder: Default "Sequence-ID"_UR
@@ -221,15 +221,15 @@
 ```
 
 ```python
 usage: StORF_Finder.py [-h] [-f FASTA] [-ua {True,False}] [-wc {True,False}] [-ps {True,False}] [-olap_filt [{none,single-strand,both-strand}]] [-start_filt {True,False}] [-con_storfs {True,False}] [-con_only {True,False}] [-short_storfs {False,Nolap,Olap}] [-short_storfs_only {True,False}]
                        [-stop_ident {True,False}] [-f_type [{StORF,CDS,ORF}]] [-minorf MIN_ORF] [-maxorf MAX_ORF] [-codons STOP_CODONS] [-olap OVERLAP_NT] [-s SUFFIX] [-so [{start_pos,strand}]] [-spos {True,False}] [-oname O_NAME] [-odir O_DIR] [-gff {True,False}] [-aa {True,False}] [-aa_only {True,False}]
                        [-lw {True,False}] [-gff_fasta {True,False}] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Finder Run Parameters.
+StORF-Reporter v1.0.3: StORF-Finder Run Parameters.
 
 Required Arguments:
   -f FASTA              Input FASTA File - (UR_Extractor output)
 
 Optional Arguments:
   -ua {True,False}      Default - Treat input as Unannotated: Use "-ua False" for standard fasta
   -wc {True,False}      Default - False: StORFs reported across entire sequence
@@ -285,15 +285,15 @@
 ```console
 StORF-Extractor -storf_input Combined -p .../Test_Datasets/Combined_GFFs/E-coli_Combined_StORF-Reporter_Extended.gff 
 ```
 
 ```python
 usage: StORF_Extractor.py [-h] [-storf_input {Combined,Separate}] [-p PATH] [-gff_out {True,False}] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}] [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: StORF-Extractor Run Parameters.
+StORF-Reporter v1.0.3: StORF-Extractor Run Parameters.
 
 Required Arguments:
   -storf_input {Combined,Separate}
                         Are StORFs to be extracted from Combined GFF/FASTA or Separate GFF/FASTA files?
   -p PATH               Provide input file or directory path
 
 Output:
@@ -318,15 +318,15 @@
 StORF-Remover -gff .../Test_Datasets/StORF_Extractor_And_Remover/Myco_UR_StORF-R.gff -blast .../Test_Datasets/StORF_Extractor_And_Remover/Myco_URs_StORFs_aa_Swiss.tab 
 ```
 
 ```python
 usage: StORF_Remover.py [-h] [-gff GFF] [-blast BLAST] [-min_score MINSCORE] [-oname O_NAME] [-odir O_DIR] [-gz {True,False}]
                         [-verbose {True,False}] [-v]
 
-StORF-Reporter v1.0.2: UR-Extractor Run Parameters.
+StORF-Reporter v1.0.3: UR-Extractor Run Parameters.
 
 Required Arguments:
   -gff GFF              GFF annotation file for the FASTA
   -blast BLAST          BLAST format 6 annotation file
 
 Optional Arguments:
   -min_score MINSCORE   Minimum BitScore to keep StORF: Default 30
```

### Comparing `StORF-Reporter-1.0.2/src/StORF_Reporter.egg-info/SOURCES.txt` & `StORF-Reporter-1.0.3/src/StORF_Reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

